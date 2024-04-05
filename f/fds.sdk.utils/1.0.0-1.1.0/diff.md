# Comparing `tmp/fds.sdk.utils-1.0.0.tar.gz` & `tmp/fds_sdk_utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fds.sdk.utils-1.0.0.tar", max compression
+gzip compressed data, was "fds_sdk_utils-1.1.0.tar", max compression
```

## Comparing `fds.sdk.utils-1.0.0.tar` & `fds_sdk_utils-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    11357 2022-03-24 14:43:03.915946 fds.sdk.utils-1.0.0/LICENSE
--rw-r--r--   0        0        0     4592 2022-03-24 14:43:03.915946 fds.sdk.utils-1.0.0/README.md
--rw-r--r--   0        0        0      796 2022-03-24 14:43:03.915946 fds.sdk.utils-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-03-24 14:43:03.915946 fds.sdk.utils-1.0.0/src/fds/__init__.py
--rw-r--r--   0        0        0        0 2022-03-24 14:43:03.915946 fds.sdk.utils-1.0.0/src/fds/sdk/__init__.py
--rw-r--r--   0        0        0      253 2022-03-24 14:43:03.915946 fds.sdk.utils-1.0.0/src/fds/sdk/utils/__init__.py
--rw-r--r--   0        0        0      273 2022-03-24 14:43:03.915946 fds.sdk.utils-1.0.0/src/fds/sdk/utils/authentication/__init__.py
--rw-r--r--   0        0        0     9531 2022-03-24 14:43:03.915946 fds.sdk.utils-1.0.0/src/fds/sdk/utils/authentication/confidential.py
--rw-r--r--   0        0        0      722 2022-03-24 14:43:03.915946 fds.sdk.utils-1.0.0/src/fds/sdk/utils/authentication/constants.py
--rw-r--r--   0        0        0      724 2022-03-24 14:43:03.915946 fds.sdk.utils-1.0.0/src/fds/sdk/utils/authentication/exceptions.py
--rw-r--r--   0        0        0      332 2022-03-24 14:43:03.915946 fds.sdk.utils-1.0.0/src/fds/sdk/utils/authentication/oauth2client.py
--rw-r--r--   0        0        0     5611 2022-03-24 14:43:24.135423 fds.sdk.utils-1.0.0/setup.py
--rw-r--r--   0        0        0     5386 2022-03-24 14:43:24.135937 fds.sdk.utils-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6461 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/README.md
+-rw-r--r--   0        0        0      796 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/sdk/__init__.py
+-rw-r--r--   0        0        0      253 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/sdk/utils/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/__init__.py
+-rw-r--r--   0        0        0    12392 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/confidential.py
+-rw-r--r--   0        0        0      722 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/constants.py
+-rw-r--r--   0        0        0      724 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/exceptions.py
+-rw-r--r--   0        0        0      332 2024-04-05 14:05:16.093186 fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/oauth2client.py
+-rw-r--r--   0        0        0     7357 1970-01-01 00:00:00.000000 fds_sdk_utils-1.1.0/PKG-INFO
```

### Comparing `fds.sdk.utils-1.0.0/LICENSE` & `fds_sdk_utils-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fds.sdk.utils-1.0.0/pyproject.toml` & `fds_sdk_utils-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fds.sdk.utils"
-version = "1.0.0"
+version = "1.1.0"
 description = "Utilities for interacting with FactSet APIs."
 authors=["FactSet Research Systems"]
 license="Apache-2.0"
 readme="README.md"
 homepage="https://developer.factset.com"
 keywords=[
   "FactSet",
@@ -13,27 +13,27 @@
 ]
 packages=[
   { include = "fds", from = "src" }
 ]
 exclude=["tests"]
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.7.0"
 python-jose = "^3.3.0"
 requests-oauthlib = "^1.3.0"
-requests = "^2.25.1"
-oauthlib = "^3.1.1"
+requests = "^2.28.2"
+oauthlib = "^3.2.2"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.0"
-black = {version = "^22.1", allow-prereleases = true}
-pytest-cov = "^3.0.0"
-pytest-mock = "^3.6.1"
-tox = "^3.24.1"
-tox-gh-actions = "^2.6.0"
+pytest = "^7.4"
+black = {version = "^23.3", allow-prereleases = true}
+pytest-cov = "^4.1.0"
+pytest-mock = "^3.11.1"
+tox = "^4.8.0"
+tox-gh-actions = "^3.2.0"
 
 [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fds.sdk.utils-1.0.0/src/fds/sdk/utils/authentication/confidential.py` & `fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/confidential.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 import logging
 import time
 import uuid
 
 import requests
 from jose import JWSError, jws
 from oauthlib.oauth2 import BackendApplicationClient
+from requests import Session
+from requests.adapters import HTTPAdapter
 from requests_oauthlib import OAuth2Session
+from urllib3 import Retry
 
 from .constants import CONSTS
 from .oauth2client import OAuth2Client
 from .exceptions import (
     AccessTokenError,
     ConfidentialClientError,
     ConfigurationError,
@@ -29,15 +32,24 @@
     client credentials flow.
 
     The main purpose of this class is to provide an access token that can
     be used to authenticate against FactSet's APIs. It takes care of fetching
     the access token, caching it and refreshing it as needed.
     """
 
-    def __init__(self, config_path: str = "", config: dict = None) -> None:
+    def __init__(
+        self,
+        config_path: str = None,
+        config: dict = None,
+        proxy: str = None,
+        proxy_headers: dict = None,
+        verify_ssl: bool = True,
+        ssl_ca_cert: str = None,
+        retry: Retry = None,
+    ) -> None:
         """
         Creates a new ConfidentialClient.
 
         When setting up the OAuth 2.0 client, this constructor reaches out to
         FactSet's well-known URI to retrieve metadata about its authorization
         server. This information along with information about the OAuth 2.0
         client is stored and used whenever a new access token is fetched.
@@ -66,45 +78,84 @@
                         "q": "Second Prime Factor",
                         "dp": "First Factor CRT Exponent",
                         "dq": "Second Factor CRT Exponent",
                         "qi": "First CRT Coefficient",
                     }
                 }
 
-                `NB`: Within the JWK parameters kty, alg, use, kid, n, e, d, p, q, dp, dq, qi are required for authorization.
+                `NB`: Within the JWK parameters kty, alg, use, kid, n, e, d, p, q, dp, dq, qi are
+                required for authorization.
+
+            `proxy` (str) : Proxy URL
+
+            `proxy_headers` (dict) : Sometimes it is necessary to add custom headers to http requests to be able to
+            use a proxy or firewall
+
+            `verify_ssl` (bool): Set this to ``False`` to skip verifying SSL certificate when calling API from
+            https server. When set to ``False``, requests will accept any TLS certificate presented by the server,
+            and will ignore hostname mismatches and/or expired certificates, which will make your application
+            vulnerable to man-in-the-middle (MitM) attacks. Setting verify to ``False`` may be useful during
+            local development or testing.
+
+            `ssl_ca_cert` (str): Set this to customize the certificate file to verify the peer. If ``ssl_ca_cert`` is
+            set, the ca_cert will be verified whether ``verify_ssl`` is enabled
+
+            `retry` (Retry): Set this to custommize the retry policy for the requests. If not set, the default is used.
+
+
         Raises:
             AuthServerMetadataError: Raised if there's an issue retrieving the authorization server metadata
             AuthServerMetadataContentError: Raised if the authorization server metadata is incomplete
             ConfidentialClientError: Raised if instantiation errors occur
             ConfigurationError: Raised if there's an issue reading the configuration file
             KeyError: Raised if configuration is missing a required property
             ValueError: Raised if `config_path` or `config` are not provided properly
         """
 
         if not config_path and not config:
             raise ValueError("Either 'config_path' or 'config' must be set.")
 
         if config_path and config:
-            raise ValueError("Either 'config_path' or 'config' must be set.  Not Both.")
+            raise ValueError("Either 'config_path' or 'config' must be set. Not Both.")
 
         if config_path:
             try:
                 with open(config_path, "r") as config_file:
                     self._config = json.load(config_file)
                     log.debug("Retrieved configuration from file: %s", config_path)
             except Exception as e:
                 raise ConfigurationError(f"Error retrieving contents of {config_path}") from e
 
         if config:
             self._config = config
 
+        if proxy:
+            self._proxy = {"http": proxy, "https": proxy}
+        else:
+            self._proxy = None
+
+        self._verify_ssl = verify_ssl
+        self._proxy_headers = proxy_headers
+        self._ssl_ca_cert = ssl_ca_cert
+
+        if retry is not None:
+            self._retry = retry
+        else:
+            self._retry = Retry(
+                total=3,
+                backoff_factor=1,
+                status_forcelist=[413, 429, 500, 502, 503, 504],
+                allowed_methods={"DELETE", "GET", "HEAD", "OPTIONS", "POST", "PUT", "TRACE"},
+            )
+
         try:
             self._oauth_session = OAuth2Session(
                 client=BackendApplicationClient(client_id=self._config[CONSTS.CONFIG_CLIENT_ID])
             )
+            self._oauth_session.mount("https://", HTTPAdapter(max_retries=self._retry))
         except Exception as e:
             raise ConfidentialClientError(
                 f"Error instantiating OAuth2 session with {CONSTS.CONFIG_CLIENT_ID}:{self._config[CONSTS.CONFIG_CLIENT_ID]}"
             ) from e
 
         log.debug("Reviewing credentials format and completeness")
 
@@ -114,24 +165,38 @@
             raise KeyError(f"'{CONSTS.CONFIG_JWK}' must be contained within configuration")
 
         if not set(CONSTS.CONFIG_JWK_REQUIRED_KEYS).issubset(set(self._config[CONSTS.CONFIG_JWK].keys())):
             raise KeyError(f"JWK must contain the following items: '{CONSTS.CONFIG_JWK_REQUIRED_KEYS}'")
 
         log.debug("Credentials are complete and formatted correctly")
 
+        self._requests_session = Session()
+        self._requests_session.mount("https://", HTTPAdapter(max_retries=self._retry))
+
         self._init_auth_server_metadata()
 
         self._cached_token = {}
 
     def _init_auth_server_metadata(self) -> None:
         try:
             log.debug(
                 "Attempting metadata retrieval from well_known_uri: %s", self._config[CONSTS.CONFIG_WELL_KNOWN_URI]
             )
-            res = requests.get(self._config[CONSTS.CONFIG_WELL_KNOWN_URI])
+
+            verify = self._verify_ssl
+
+            if self._ssl_ca_cert:
+                verify = self._ssl_ca_cert
+
+            res = self._requests_session.get(
+                url=self._config[CONSTS.CONFIG_WELL_KNOWN_URI],
+                proxies=self._proxy,
+                verify=verify,
+                headers=self._proxy_headers,
+            )
             log.debug("Request from well_known_uri completed with status: %s", res.status_code)
             log.debug("Response headers from well_known_uri were %s", res.headers)
             self._well_known_uri_metadata = res.json()
         except Exception as e:
             raise AuthServerMetadataError(
                 f"Error retrieving contents from the well_known_uri: {self._config[CONSTS.CONFIG_WELL_KNOWN_URI]}"
             ) from e
@@ -204,18 +269,34 @@
                 "Retrieving cached token. Expires in '%s' seconds.",
                 int(self._cached_token[CONSTS.TOKEN_EXPIRES_AT] - time.time()),
             )
             return self._cached_token[CONSTS.TOKEN_ACCESS_TOKEN]
 
         try:
             log.debug("Fetching new access token")
+
+            headers = {
+                "Accept": "application/json",
+                "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
+            }
+
+            if self._proxy_headers:
+                headers |= self._proxy_headers
+
+            verify = self._verify_ssl
+            if self._ssl_ca_cert:
+                verify = self._ssl_ca_cert
+
             token = self._oauth_session.fetch_token(
                 token_url=self._well_known_uri_metadata[CONSTS.META_TOKEN_ENDPOINT],
                 client_id=self._config[CONSTS.CONFIG_CLIENT_ID],
                 client_assertion_type="urn:ietf:params:oauth:client-assertion-type:jwt-bearer",
                 client_assertion=self._get_client_assertion_jws(),
+                verify=verify,
+                proxies=self._proxy,
+                headers=headers,
             )
             self._cached_token = token
             log.info("Caching token that expires at %s", token[CONSTS.TOKEN_EXPIRES_AT])
             return token[CONSTS.TOKEN_ACCESS_TOKEN]
         except Exception as e:
             raise AccessTokenError("Error attempting to get access token") from e
```

### Comparing `fds.sdk.utils-1.0.0/src/fds/sdk/utils/authentication/constants.py` & `fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/constants.py`

 * *Files identical despite different names*

### Comparing `fds.sdk.utils-1.0.0/src/fds/sdk/utils/authentication/exceptions.py` & `fds_sdk_utils-1.1.0/src/fds/sdk/utils/authentication/exceptions.py`

 * *Files identical despite different names*

### Comparing `fds.sdk.utils-1.0.0/setup.py` & `fds_sdk_utils-1.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,203 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+<img alt="FactSet" src="https://www.factset.com/hubfs/Assets/images/factset-logo.svg" height="56" width="290">
 
-package_dir = \
-{'': 'src'}
+# FactSet SDK Utilities for Python
 
-packages = \
-['fds', 'fds.sdk', 'fds.sdk.utils', 'fds.sdk.utils.authentication']
+[![PyPi](https://img.shields.io/pypi/v/fds.sdk.utils)](https://pypi.org/project/fds.sdk.utils/)
+[![Apache-2 license](https://img.shields.io/badge/license-Apache2-brightgreen.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['oauthlib>=3.1.1,<4.0.0',
- 'python-jose>=3.3.0,<4.0.0',
- 'requests-oauthlib>=1.3.0,<2.0.0',
- 'requests>=2.25.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'fds.sdk.utils',
-    'version': '1.0.0',
-    'description': 'Utilities for interacting with FactSet APIs.',
-    'long_description': '<img alt="FactSet" src="https://www.factset.com/hubfs/Assets/images/factset-logo.svg" height="56" width="290">\n\n# FactSet SDK Utilities for Python\n\n[![PyPi](https://img.shields.io/pypi/v/fds.sdk.utils)](https://pypi.org/project/fds.sdk.utils/)\n[![Apache-2 license](https://img.shields.io/badge/license-Apache2-brightgreen.svg)](https://www.apache.org/licenses/LICENSE-2.0)\n\nThis repository contains a collection of utilities that supports FactSet\'s SDK in Python and facilitate usage of FactSet APIs.\n\n## Installation\n\n### Poetry\n\n```python\npoetry add fds.sdk.utils\n```\n\n### pip\n\n```python\npip install fds.sdk.utils\n```\n\n## Usage\n\nThis library contains multiple modules, sample usage of each module is below.\n\n### Authentication\n\nFirst, you need to create the OAuth 2.0 client configuration that will be used to authenticate against FactSet\'s APIs:\n\n1. Create a [new application](https://developer.factset.com/applications) on FactSet\'s Developer Portal.\n2. When prompted, download the configuration file and move it to your development environment.\n\n```python\nfrom fds.sdk.utils.authentication import ConfidentialClient\nimport requests\n\nclient = ConfidentialClient(\'/path/to/config.json\')\nres = requests.get(\n  \'https://api.factset.com/analytics/lookups/v3/currencies\',\n  headers={\n    \'Authorization\': \'Bearer \' + client.get_access_token()\n  })\n\nprint(res.text)\n```\n\n## Modules\n\nInformation about the various utility modules contained in this library can be found below.\n\n### Authentication\n\nThe [authentication module](src/fds/sdk/utils/authentication) provides helper classes that facilitate [OAuth 2.0](https://github.com/factset/oauth2-guidelines) authentication and authorization with FactSet\'s APIs. Currently the module has support for the [client credentials flow](https://github.com/factset/oauth2-guidelines#client-credentials-flow-1).\n\nEach helper class in the module has the following features:\n\n* Accepts a configuration file or `dict` that contains information about the OAuth 2.0 client, including the client ID and private key.\n* Performs authentication with FactSet\'s OAuth 2.0 authorization server and retrieves an access token.\n* Caches the access token for reuse and requests a new access token as needed when one expires.\n\n#### Configuration\n\nClasses in the authentication module require OAuth 2.0 client configuration information to be passed to constructors through a JSON-formatted file or a `dict`. In either case the format is the same:\n\n```json\n{\n    "name": "Application name registered with FactSet\'s Developer Portal",\n    "clientId": "OAuth 2.0 Client ID registered with FactSet\'s Developer Portal",\n    "clientAuthType": "Confidential",\n    "owners": ["USERNAME-SERIAL"],\n    "jwk": {\n        "kty": "RSA",\n        "use": "sig",\n        "alg": "RS256",\n        "kid": "Key ID",\n        "d": "ECC Private Key",\n        "n": "Modulus",\n        "e": "Exponent",\n        "p": "First Prime Factor",\n        "q": "Second Prime Factor",\n        "dp": "First Factor CRT Exponent",\n        "dq": "Second Factor CRT Exponent",\n        "qi": "First CRT Coefficient",\n    }\n}\n```\n\nIf you\'re just starting out, you can visit FactSet\'s Developer Portal to [create a new application](https://developer.factset.com/applications) and download a configuration file in this format.\n\nIf you\'re creating and managing your signing key pair yourself, see the required [JWK parameters](https://github.com/factset/oauth2-guidelines#jwk-parameters) for public-private key pairs.\n\n## Debugging\n\nThis library uses the [logging module](https://docs.python.org/3/howto/logging.html) to log various messages that will help you understand what it\'s doing. You can increase the log level to see additional debug information using standard conventions. For example:\n\n```python\nlogging.getLogger(\'fds.sdk.utils\').setLevel(logging.DEBUG)\n```\n\nor\n\n```python\nlogging.getLogger(\'fds.sdk.utils.authentication\').setLevel(logging.DEBUG)\n```\n\n# Contributing\n\nPlease refer to the [contributing guide](CONTRIBUTING.md).\n\n# Copyright\n\nCopyright 2022 FactSet Research Systems Inc\n\nLicensed under the Apache License, Version 2.0 (the "License");\nyou may not use this file except in compliance with the License.\nYou may obtain a copy of the License at\n\n    http://www.apache.org/licenses/LICENSE-2.0\n\nUnless required by applicable law or agreed to in writing, software\ndistributed under the License is distributed on an "AS IS" BASIS,\nWITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\nSee the License for the specific language governing permissions and\nlimitations under the License.\n',
-    'author': 'FactSet Research Systems',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://developer.factset.com',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6.2,<4.0.0',
+This repository contains a collection of utilities that supports FactSet's SDK in Python and facilitate usage of FactSet
+APIs.
+
+## Installation
+
+### Poetry
+
+```sh
+poetry add fds.sdk.utils
+```
+
+### pip
+
+```sh
+pip install fds.sdk.utils
+```
+
+## Usage
+
+This library contains multiple modules, sample usage of each module is below.
+
+### Authentication
+
+First, you need to create the OAuth 2.0 client configuration that will be used to authenticate against FactSet's APIs:
+
+1. [Create a new application](https://developer.factset.com/learn/authentication-oauth2#creating-an-application) on
+   FactSet's Developer Portal.
+2. When prompted, download the configuration file and move it to your development environment.
+
+```python
+from fds.sdk.utils.authentication import ConfidentialClient
+import requests
+
+# The ConfidentialClient instance should be reused in production environments.
+client = ConfidentialClient(
+  config_path='/path/to/config.json'
+)
+res = requests.get(
+  'https://api.factset.com/analytics/lookups/v3/currencies',
+  headers={
+    'Authorization': 'Bearer ' + client.get_access_token()
+  })
+
+print(res.text)
+```
+
+### Configure a Proxy
+
+You can pass proxy settings to the ConfidentialClient if necessary.
+The `proxy` parameter takes a URL to tell the request library which proxy should be used.
+
+If necessary it is possible to set custom `proxy_headers` as dictionary.
+
+```python
+from fds.sdk.utils.authentication import ConfidentialClient
+
+client = ConfidentialClient(
+  config_path='/path/to/config.json',
+  proxy="http://secret:password@localhost:5050",
+  proxy_headers={
+    "Custom-Proxy-Header": "Custom-Proxy-Header-Value"
+  }
+)
+```
+
+### Custom SSL Certificate
+
+If you have proxies or firewalls which are using custom TLS certificates,
+you are able to pass a custom pem file (`ssl_ca_cert` parameter) so that the
+request library is able to verify the validity of that certificate. If a
+ca cert is passed it is validated regardless if `verify_ssl` is set to false.
+
+With `verify_ssl` it is possible to disable the verifications of certificates.
+Disabling the verification is not recommended, but it might be useful during
+local development or testing
+
+```python
+from fds.sdk.utils.authentication import ConfidentialClient
+
+client = ConfidentialClient(
+  config_path='/path/to/config.json',
+  verify_ssl=True,
+  ssl_ca_cert='/path/to/ca.pem'
+)
+```
+
+### Request Retries
+
+In case the request retry behaviour should be customized, it is possible to pass a `urllib3.Retry` object to
+the `ConfidentialClient`.
+
+```python
+from urllib3 import Retry
+from fds.sdk.utils.authentication import ConfidentialClient
+
+client = ConfidentialClient(
+  config_path='/path/to/config.json',
+  retry=Retry(
+    total=5,
+    backoff_factor=0.1,
+    status_forcelist=[500, 502, 503, 504]
+  )
+)
+```
+
+## Modules
+
+Information about the various utility modules contained in this library can be found below.
+
+### Authentication
+
+The [authentication module](src/fds/sdk/utils/authentication) provides helper classes that
+facilitate [OAuth 2.0](https://developer.factset.com/learn/authentication-oauth2) authentication and authorization with
+FactSet's APIs. Currently the module has support for
+the [client credentials flow](https://github.com/factset/oauth2-guidelines#client-credentials-flow-1).
+
+Each helper class in the module has the following features:
+
+* Accepts a configuration file or `dict` that contains information about the OAuth 2.0 client, including the client ID
+  and private key.
+* Performs authentication with FactSet's OAuth 2.0 authorization server and retrieves an access token.
+* Caches the access token for reuse and requests a new access token as needed when one expires.
+  * In order for this to work correctly, the helper class instance should be reused in production environments.
+
+#### Configuration
+
+Classes in the authentication module require OAuth 2.0 client configuration information to be passed to constructors
+through a JSON-formatted file or a `dict`. In either case the format is the same:
+
+```json
+{
+  "name": "Application name registered with FactSet's Developer Portal",
+  "clientId": "OAuth 2.0 Client ID registered with FactSet's Developer Portal",
+  "clientAuthType": "Confidential",
+  "owners": [
+    "USERNAME-SERIAL"
+  ],
+  "jwk": {
+    "kty": "RSA",
+    "use": "sig",
+    "alg": "RS256",
+    "kid": "Key ID",
+    "d": "ECC Private Key",
+    "n": "Modulus",
+    "e": "Exponent",
+    "p": "First Prime Factor",
+    "q": "Second Prime Factor",
+    "dp": "First Factor CRT Exponent",
+    "dq": "Second Factor CRT Exponent",
+    "qi": "First CRT Coefficient"
+  }
 }
+```
 
+If you're just starting out, you can visit FactSet's Developer Portal
+to [create a new application](https://developer.factset.com/applications) and download a configuration file in this
+format.
 
-setup(**setup_kwargs)
+If you're creating and managing your signing key pair yourself, see the
+required [JWK parameters](https://github.com/factset/oauth2-guidelines#jwk-parameters) for public-private key pairs.
+
+## Debugging
+
+This library uses the [logging module](https://docs.python.org/3/howto/logging.html) to log various messages that will
+help you understand what it's doing. You can increase the log level to see additional debug information using standard
+conventions. For example:
+
+```python
+logging.getLogger('fds.sdk.utils').setLevel(logging.DEBUG)
+```
+
+or
+
+```python
+logging.getLogger('fds.sdk.utils.authentication').setLevel(logging.DEBUG)
+```
+
+# Contributing
+
+Please refer to the [contributing guide](CONTRIBUTING.md).
+
+# Copyright
+
+Copyright 2022 FactSet Research Systems Inc
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

