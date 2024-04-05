# Comparing `tmp/hamburg-3.0.0.tar.gz` & `tmp/hamburg-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hamburg-3.0.0.tar", max compression
+gzip compressed data, was "hamburg-3.0.1.tar", max compression
```

## Comparing `hamburg-3.0.0.tar` & `hamburg-3.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-12-16 03:40:26.239891 hamburg-3.0.0/LICENSE
--rw-r--r--   0        0        0    10711 2023-12-16 03:40:26.239891 hamburg-3.0.0/README.md
--rw-r--r--   0        0        0     3815 2023-12-16 03:40:38.723931 hamburg-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      380 2023-12-16 03:40:26.243891 hamburg-3.0.0/src/hamburg/__init__.py
--rw-r--r--   0        0        0      281 2023-12-16 03:40:26.243891 hamburg-3.0.0/src/hamburg/exceptions.py
--rw-r--r--   0        0        0     5697 2023-12-16 03:40:26.243891 hamburg-3.0.0/src/hamburg/hamburg.py
--rw-r--r--   0        0        0     6089 2023-12-16 03:40:26.243891 hamburg-3.0.0/src/hamburg/models.py
--rw-r--r--   0        0        0        0 2023-12-16 03:40:26.243891 hamburg-3.0.0/src/hamburg/py.typed
--rw-r--r--   0        0        0    11990 1970-01-01 00:00:00.000000 hamburg-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-05 11:38:23.111509 hamburg-3.0.1/LICENSE
+-rw-r--r--   0        0        0    10924 2024-04-05 11:38:23.111509 hamburg-3.0.1/README.md
+-rw-r--r--   0        0        0     3893 2024-04-05 11:38:34.111678 hamburg-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0      380 2024-04-05 11:38:23.111509 hamburg-3.0.1/src/hamburg/__init__.py
+-rw-r--r--   0        0        0      281 2024-04-05 11:38:23.111509 hamburg-3.0.1/src/hamburg/exceptions.py
+-rw-r--r--   0        0        0     5701 2024-04-05 11:38:23.111509 hamburg-3.0.1/src/hamburg/hamburg.py
+-rw-r--r--   0        0        0     6140 2024-04-05 11:38:23.111509 hamburg-3.0.1/src/hamburg/models.py
+-rw-r--r--   0        0        0        0 2024-04-05 11:38:23.111509 hamburg-3.0.1/src/hamburg/py.typed
+-rw-r--r--   0        0        0    12199 1970-01-01 00:00:00.000000 hamburg-3.0.1/PKG-INFO
```

### Comparing `hamburg-3.0.0/LICENSE` & `hamburg-3.0.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-Copyright (c) 2022-2023 Klaas Schoute
+Copyright (c) 2022-2024 Klaas Schoute
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hamburg-3.0.0/README.md` & `hamburg-3.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 | `latitude` | float | The latitude of the park and ride |
 | `updated_at` | datetime | The date and time the park and ride was last updated |
 
 ### Garages
 
 Extra parameters to filter the data:
 
-- **available** (default: None) - Allows you to filter based on available spaces, using operators such as `<`, `<=`, `>` and `>=`.
+- **set_filter** (default: None) - Allows you to filter based on filter expressions, see [here](https://api.hamburg.de/datasets/v1/parkhaeuser/api?f=html#/Access%20data/verkehr_parkhaeuser.getItems) for more information.
 
 | Variable | Type | Description |
 | :------- | :--- | :---------- |
 | `spot_id` | string | The ID of the garage |
 | `name` | string | The name of the pgarage |
 | `park_type` | string | The parking type of the garage |
 | `disabled_parking_spaces` | int | The number of disabled parking spaces in the garage |
@@ -190,19 +190,25 @@
 
 To run just the Python tests:
 
 ```bash
 poetry run pytest
 ```
 
+To update the [syrupy](https://github.com/tophat/syrupy) snapshot tests:
+
+```bash
+poetry run pytest --snapshot-update
+```
+
 ## License
 
 MIT License
 
-Copyright (c) 2022-2023 Klaas Schoute
+Copyright (c) 2022-2024 Klaas Schoute
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -236,15 +242,15 @@
 [codecov-url]: https://codecov.io/gh/klaasnicolaas/python-hamburg
 [devcontainer-shield]: https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode
 [devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/klaasnicolaas/python-hamburg
 [downloads-shield]: https://img.shields.io/pypi/dm/hamburg
 [downloads-url]: https://pypistats.org/packages/hamburg
 [license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-hamburg.svg
 [last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-hamburg.svg
-[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2024.svg
 [maintainability-shield]: https://api.codeclimate.com/v1/badges/5041849456b7348f3bc7/maintainability
 [maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-hamburg/maintainability
 [project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
 [pypi]: https://pypi.org/project/hamburg/
 [python-versions-shield]: https://img.shields.io/pypi/pyversions/hamburg
 [typing-shield]: https://github.com/klaasnicolaas/python-hamburg/actions/workflows/typing.yaml/badge.svg
 [typing-url]: https://github.com/klaasnicolaas/python-hamburg/actions/workflows/typing.yaml
```

### Comparing `hamburg-3.0.0/pyproject.toml` & `hamburg-3.0.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hamburg"
-version = "3.0.0"
+version = "3.0.1"
 description = "Asynchronous Python client providing Urban Data information of Hamburg"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-hamburg"
 repository = "https://github.com/klaasnicolaas/python-hamburg"
@@ -23,37 +23,37 @@
 packages = [
   { include = "hamburg", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.11"
+pytz = "^2024.1"
 yarl = ">=1.6.0"
-pytz = ">=2022.7.1,<2024.0.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-hamburg/issues"
 Changelog = "https://github.com/klaasnicolaas/python-hamburg/releases"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.1.8"
-aresponses = "2.1.6"
-blacken-docs = "1.16.0"
+aresponses = "3.0.0"
 codespell = "2.2.6"
-coverage = {version = "7.3.3", extras = ["toml"]}
-mypy = "1.7.1"
-pre-commit = "3.6.0"
-pre-commit-hooks = "4.5.0"
-pylint = "3.0.3"
-pytest = "7.4.3"
-pytest-asyncio = "0.23.2"
-pytest-cov = "4.1.0"
-yamllint = "1.33.0"
 covdefaults = "2.3.0"
-types-pytz = "2023.3.1.1"
+coverage = {version = "7.4.4", extras = ["toml"]}
+mypy = "1.9.0"
+pre-commit = "3.7.0"
+pre-commit-hooks = "4.5.0"
+pylint = "3.1.0"
+pytest = "8.1.1"
+pytest-asyncio = "0.23.6"
+pytest-cov = "5.0.0"
+ruff = "0.3.5"
+syrupy = "4.6.1"
+types-pytz = "2024.1.0.20240203"
+yamllint = "1.35.1"
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["hamburg"]
 
 [tool.coverage.report]
 fail_under = 90
@@ -90,26 +90,15 @@
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.pylint.BASIC]
-good-names = [
-  "_",
-  "ex",
-  "fp",
-  "i",
-  "id",
-  "j",
-  "k",
-  "on",
-  "Run",
-  "T",
-]
+good-names = ["_", "ex", "fp", "i", "id", "j", "k", "on", "Run", "T"]
 
 [tool.pylint."MESSAGES CONTROL"]
 disable= [
   "duplicate-code",
   "format",
   "unsubscriptable-object",
 ]
@@ -124,42 +113,37 @@
 max-attributes = 15
 
 [tool.pytest.ini_options]
 addopts = "--cov"
 asyncio_mode = "auto"
 
 [tool.ruff]
-select = ["ALL"]
-ignore = [
-  "ANN101", # Self... explanatory
-  "ANN401", # Opinioated warning on disallowing dynamically typed expressions
-  "D203", # Conflicts with other rules
-  "D213", # Conflicts with other rules
-  "D417", # False positives in some occasions
+target-version = "py311"
+lint.select = ["ALL"]
+lint.ignore = [
+  "ANN101",  # Self... explanatory
+  "ANN102",  # cls... just as useless
+  "ANN401",  # Opinioated warning on disallowing dynamically typed expressions
+  "D203",    # Conflicts with other rules
+  "D213",    # Conflicts with other rules
+  "D417",    # False positives in some occasions
   "PLR2004", # Just annoying, not really useful
+  "SLOT000", # Has a bug with enums: https://github.com/astral-sh/ruff/issues/5748
 
-  # Formatter conflicts
+  # Conflicts with the Ruff formatter
   "COM812",
-  "COM819",
-  "D206",
-  "E501",
   "ISC001",
-  "Q000",
-  "Q001",
-  "Q002",
-  "Q003",
-  "W191",
 ]
 
-[tool.ruff.flake8-pytest-style]
+[tool.ruff.lint.flake8-pytest-style]
 mark-parentheses = false
 fixture-parentheses = false
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["hamburg"]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 25
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `hamburg-3.0.0/src/hamburg/hamburg.py` & `hamburg-3.0.1/src/hamburg/hamburg.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Asynchronous Python client providing Urban Data information of Hamburg."""
+
 from __future__ import annotations
 
 import asyncio
 import socket
 from dataclasses import dataclass
 from importlib import metadata
 from typing import Any, Self, cast
@@ -10,14 +11,16 @@
 from aiohttp import ClientError, ClientSession
 from aiohttp.hdrs import METH_GET
 from yarl import URL
 
 from .exceptions import UDPHamburgConnectionError, UDPHamburgError
 from .models import DisabledParking, Garage, ParkAndRide
 
+VERSION = metadata.version(__package__)
+
 
 @dataclass
 class UDPHamburg:
     """Main class for handling data fetching from Urban Data Platform of Hamburg."""
 
     request_timeout: float = 10.0
     session: ClientSession | None = None
@@ -45,25 +48,25 @@
             the Urban Data Platform API.
 
         Raises:
         ------
             UDPHamburgConnectionError: Timeout occurred while
                 connecting to the Urban Data Platform API.
             UDPHamburgError: If the data is not valid.
+
         """
-        version = metadata.version(__package__)
         url = URL.build(
             scheme="https",
             host="api.hamburg.de",
             path="/datasets/v1/",
         ).join(URL(uri))
 
         headers = {
             "Accept": "application/geo+json",
-            "User-Agent": f"PythonUDPHamburg/{version}",
+            "User-Agent": f"PythonUDPHamburg/{VERSION}",
         }
 
         if self.session is None:
             self.session = ClientSession()
             self._close_session = True
 
         try:
@@ -72,15 +75,15 @@
                     method,
                     url,
                     params=params,
                     headers=headers,
                     ssl=True,
                 )
                 response.raise_for_status()
-        except asyncio.TimeoutError as exception:
+        except TimeoutError as exception:
             msg = "Timeout occurred while connecting to the Urban Data Platform API."
             raise UDPHamburgConnectionError(
                 msg,
             ) from exception
         except (ClientError, socket.gaierror) as exception:
             msg = "Error occurred while communicating with Urban Data Platform API."
             raise UDPHamburgConnectionError(
@@ -107,14 +110,15 @@
         Args:
         ----
             limit: Number of items to return.
 
         Returns:
         -------
             A list of DisabledParking objects.
+
         """
         locations = await self._request(
             "behindertenstellplaetze/collections/verkehr_behindertenparkpl/items",
             params={"limit": limit},
         )
         return [DisabledParking.from_dict(item) for item in locations["features"]]
 
@@ -127,41 +131,43 @@
         Args:
         ----
             limit: Number of items to return.
 
         Returns:
         -------
             A list of ParkAndRide objects.
+
         """
         locations = await self._request(
             "p_und_r/collections/p_und_r/items",
             params={"limit": limit},
         )
         return [ParkAndRide.from_dict(item) for item in locations["features"]]
 
     async def garages(
         self,
         limit: int = 10,
-        available: str | None = None,
+        set_filter: str | None = None,
     ) -> list[Garage]:
         """Get all garages.
 
         Args:
         ----
             limit: Number of items to return.
-            available: Filter based on availability with operators.
+            set_filter: Filter the garages by a defined filter expression.
 
         Returns:
         -------
             A list of Garage objects.
+
         """
         params: dict[str, Any] = {"limit": limit}
 
-        if available is not None:
-            params["frei"] = str(available)
+        if set_filter is not None:
+            params["filter"] = str(set_filter)
 
         locations = await self._request(
             "parkhaeuser/collections/verkehr_parkhaeuser/items",
             params=params,
         )
 
         # By default filter out garages without location coordinates.
@@ -178,18 +184,20 @@
 
     async def __aenter__(self) -> Self:
         """Async enter.
 
         Returns
         -------
             The Urban Data Platform object.
+
         """
         return self
 
     async def __aexit__(self, *_exc_info: object) -> None:
         """Async exit.
 
         Args:
         ----
             _exc_info: Exec type.
+
         """
         await self.close()
```

### Comparing `hamburg-3.0.0/src/hamburg/models.py` & `hamburg-3.0.1/src/hamburg/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Asynchronous Python client providing Urban Data information of Hamburg."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any
 
 import pytz
@@ -26,26 +27,28 @@
         Args:
         ----
             data: The data from the API.
 
         Returns:
         -------
             A DisabledParking object.
+
         """
 
         def strip_spaces(string: str) -> str | None:
             """Strip spaces from a string.
 
             Args:
             ----
                 string: The string to strip.
 
             Returns:
             -------
                 The string without spaces or None if the string is empty.
+
             """
             if string is None:
                 return None
             return string.strip()
 
         attr = data["properties"]
         geo = data["geometry"]["coordinates"]
@@ -88,14 +91,15 @@
         Args:
         ----
             data: The data from the API.
 
         Returns:
         -------
             A ParkAndRide object.
+
         """
         attr = data["properties"]
         geo = data["geometry"]["coordinates"]
         return cls(
             spot_id=str(data.get("id")),
             name=attr.get("name"),
             park_type=attr.get("art"),
@@ -113,32 +117,31 @@
             capacity=int(attr.get("stellplaetze_gesamt")),
             availability_pct=availability_calc(
                 attr.get("stellplaetze_frei"),
                 attr.get("stellplaetze_gesamt"),
             ),
             longitude=geo[0],
             latitude=geo[1],
-            updated_at=datetime.strptime(
-                attr.get("aktualitaet_belegungsdaten"),
-                "%Y-%m-%d %H:%M:%S",
-            ).astimezone(pytz.timezone("Europe/Berlin")),
+            updated_at=strptime(
+                attr.get("aktualitaet_belegungsdaten"), "%Y-%m-%d %H:%M:%S"
+            ),
         )
 
 
 @dataclass
 class Garage:
     """Object representing a garage."""
 
     spot_id: str
     name: str
     park_type: str
     disabled_parking_spaces: int | None
     status: str
-    address: str
-    price: str
+    address: str | None
+    price: str | None
     data_origin: str | None
 
     free_space: int | None
     capacity: int | None
     availability_pct: float | None
 
     longitude: float
@@ -152,25 +155,28 @@
         Args:
         ----
             data: The data from the API.
 
         Returns:
         -------
             A Garage object.
+
         """
         attr = data["properties"]
         geo = data["geometry"]["coordinates"]
         return cls(
             spot_id=str(data.get("id")),
             name=attr.get("name"),
             park_type=attr.get("art"),
             disabled_parking_spaces=attr.get("behindertenst"),
             status=attr.get("situation"),
-            address=f"{attr.get('strasse')} {attr.get('hausnr')}",
-            price=attr.get("preise"),
+            address=f"{attr.get('strasse')} {attr.get('hausnr')}"
+            if attr.get("strasse")
+            else None,
+            price=None if attr.get("preise") == " " else attr.get("preise"),
             data_origin=attr.get("datenherkunft"),
             free_space=attr.get("frei"),
             capacity=attr.get("stellplaetze_gesamt"),
             availability_pct=availability_calc(
                 attr.get("frei"),
                 attr.get("stellplaetze_gesamt"),
             ),
@@ -192,14 +198,15 @@
         free_space: The free space.
         capacity: The capacity.
         default: The default value.
 
     Returns:
     -------
         The availability percentage.
+
     """
     try:
         return round(
             (float(free_space) / float(capacity)) * 100,
             1,
         )
     except TypeError:
@@ -216,14 +223,15 @@
         date_string: The date string.
         date_format: The format of the date string.
         default: The default value.
 
     Returns:
     -------
         The datetime object.
+
     """
     try:
-        return datetime.strptime(date_string, date_format).astimezone(
-            pytz.timezone("Europe/Berlin"),
+        return datetime.strptime(date_string, date_format).replace(
+            tzinfo=pytz.timezone("Europe/Berlin")
         )
     except (ValueError, TypeError):
         return default
```

### Comparing `hamburg-3.0.0/PKG-INFO` & `hamburg-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hamburg
-Version: 3.0.0
+Version: 3.0.1
 Summary: Asynchronous Python client providing Urban Data information of Hamburg
 Home-page: https://github.com/klaasnicolaas/python-hamburg
 License: MIT
 Keywords: urban,data,platform,hamburg,parking,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Klaas Schoute
@@ -15,15 +15,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.0.0)
-Requires-Dist: pytz (>=2022.7.1,<2024.0.0)
+Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: yarl (>=1.6.0)
 Project-URL: Bug Tracker, https://github.com/klaasnicolaas/python-hamburg/issues
 Project-URL: Changelog, https://github.com/klaasnicolaas/python-hamburg/releases
 Project-URL: Documentation, https://github.com/klaasnicolaas/python-hamburg
 Project-URL: Repository, https://github.com/klaasnicolaas/python-hamburg
 Description-Content-Type: text/markdown
 
@@ -107,15 +107,15 @@
 | `latitude` | float | The latitude of the park and ride |
 | `updated_at` | datetime | The date and time the park and ride was last updated |
 
 ### Garages
 
 Extra parameters to filter the data:
 
-- **available** (default: None) - Allows you to filter based on available spaces, using operators such as `<`, `<=`, `>` and `>=`.
+- **set_filter** (default: None) - Allows you to filter based on filter expressions, see [here](https://api.hamburg.de/datasets/v1/parkhaeuser/api?f=html#/Access%20data/verkehr_parkhaeuser.getItems) for more information.
 
 | Variable | Type | Description |
 | :------- | :--- | :---------- |
 | `spot_id` | string | The ID of the garage |
 | `name` | string | The name of the pgarage |
 | `park_type` | string | The parking type of the garage |
 | `disabled_parking_spaces` | int | The number of disabled parking spaces in the garage |
@@ -219,19 +219,25 @@
 
 To run just the Python tests:
 
 ```bash
 poetry run pytest
 ```
 
+To update the [syrupy](https://github.com/tophat/syrupy) snapshot tests:
+
+```bash
+poetry run pytest --snapshot-update
+```
+
 ## License
 
 MIT License
 
-Copyright (c) 2022-2023 Klaas Schoute
+Copyright (c) 2022-2024 Klaas Schoute
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -265,15 +271,15 @@
 [codecov-url]: https://codecov.io/gh/klaasnicolaas/python-hamburg
 [devcontainer-shield]: https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode
 [devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/klaasnicolaas/python-hamburg
 [downloads-shield]: https://img.shields.io/pypi/dm/hamburg
 [downloads-url]: https://pypistats.org/packages/hamburg
 [license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-hamburg.svg
 [last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-hamburg.svg
-[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2024.svg
 [maintainability-shield]: https://api.codeclimate.com/v1/badges/5041849456b7348f3bc7/maintainability
 [maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-hamburg/maintainability
 [project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
 [pypi]: https://pypi.org/project/hamburg/
 [python-versions-shield]: https://img.shields.io/pypi/pyversions/hamburg
 [typing-shield]: https://github.com/klaasnicolaas/python-hamburg/actions/workflows/typing.yaml/badge.svg
 [typing-url]: https://github.com/klaasnicolaas/python-hamburg/actions/workflows/typing.yaml
```

