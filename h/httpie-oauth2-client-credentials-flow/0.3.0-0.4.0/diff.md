# Comparing `tmp/httpie-oauth2-client-credentials-flow-0.3.0.tar.gz` & `tmp/httpie-oauth2-client-credentials-flow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpie-oauth2-client-credentials-flow-0.3.0.tar", last modified: Mon Mar  4 15:24:10 2024, max compression
+gzip compressed data, was "httpie-oauth2-client-credentials-flow-0.4.0.tar", last modified: Fri Apr  5 14:22:57 2024, max compression
```

## Comparing `httpie-oauth2-client-credentials-flow-0.3.0.tar` & `httpie-oauth2-client-credentials-flow-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:24:10.481692 httpie-oauth2-client-credentials-flow-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-04 15:24:04.000000 httpie-oauth2-client-credentials-flow-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-03-04 15:24:10.481692 httpie-oauth2-client-credentials-flow-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-03-04 15:24:04.000000 httpie-oauth2-client-credentials-flow-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:24:10.481692 httpie-oauth2-client-credentials-flow-0.3.0/httpie_oauth2_client_credentials_flow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-03-04 15:24:10.000000 httpie-oauth2-client-credentials-flow-0.3.0/httpie_oauth2_client_credentials_flow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-04 15:24:10.000000 httpie-oauth2-client-credentials-flow-0.3.0/httpie_oauth2_client_credentials_flow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:24:10.000000 httpie-oauth2-client-credentials-flow-0.3.0/httpie_oauth2_client_credentials_flow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-04 15:24:10.000000 httpie-oauth2-client-credentials-flow-0.3.0/httpie_oauth2_client_credentials_flow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-04 15:24:10.000000 httpie-oauth2-client-credentials-flow-0.3.0/httpie_oauth2_client_credentials_flow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 15:24:10.000000 httpie-oauth2-client-credentials-flow-0.3.0/httpie_oauth2_client_credentials_flow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-03-04 15:24:04.000000 httpie-oauth2-client-credentials-flow-0.3.0/httpie_oauth2_client_credentials_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 15:24:10.481692 httpie-oauth2-client-credentials-flow-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-03-04 15:24:04.000000 httpie-oauth2-client-credentials-flow-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:24:10.481692 httpie-oauth2-client-credentials-flow-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-03-04 15:24:04.000000 httpie-oauth2-client-credentials-flow-0.3.0/tests/test_httpie_oauth2_client_credentials_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:57.482836 httpie-oauth2-client-credentials-flow-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 14:22:50.000000 httpie-oauth2-client-credentials-flow-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-04-05 14:22:57.482836 httpie-oauth2-client-credentials-flow-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-04-05 14:22:50.000000 httpie-oauth2-client-credentials-flow-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:57.482836 httpie-oauth2-client-credentials-flow-0.4.0/httpie_oauth2_client_credentials_flow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-04-05 14:22:57.000000 httpie-oauth2-client-credentials-flow-0.4.0/httpie_oauth2_client_credentials_flow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-05 14:22:57.000000 httpie-oauth2-client-credentials-flow-0.4.0/httpie_oauth2_client_credentials_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:22:57.000000 httpie-oauth2-client-credentials-flow-0.4.0/httpie_oauth2_client_credentials_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-05 14:22:57.000000 httpie-oauth2-client-credentials-flow-0.4.0/httpie_oauth2_client_credentials_flow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 14:22:57.000000 httpie-oauth2-client-credentials-flow-0.4.0/httpie_oauth2_client_credentials_flow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:22:57.000000 httpie-oauth2-client-credentials-flow-0.4.0/httpie_oauth2_client_credentials_flow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-05 14:22:50.000000 httpie-oauth2-client-credentials-flow-0.4.0/httpie_oauth2_client_credentials_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:22:57.482836 httpie-oauth2-client-credentials-flow-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-05 14:22:50.000000 httpie-oauth2-client-credentials-flow-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:57.482836 httpie-oauth2-client-credentials-flow-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-04-05 14:22:50.000000 httpie-oauth2-client-credentials-flow-0.4.0/tests/test_httpie_oauth2_client_credentials_flow.py
```

### Comparing `httpie-oauth2-client-credentials-flow-0.3.0/LICENSE` & `httpie-oauth2-client-credentials-flow-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `httpie-oauth2-client-credentials-flow-0.3.0/PKG-INFO` & `httpie-oauth2-client-credentials-flow-0.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: httpie-oauth2-client-credentials-flow
-Version: 0.3.0
-Summary: httpie auth plugin for OAuth2.0 client credentials flow.
-Home-page: https://github.com/cliffcotino/httpie-oauth2-client-credentials
-Download-URL: https://github.com/cliffcotino/httpie-oauth2-client-credentials
-Author: satdoc
-Author-email: satodoc-develop-public@outlook.com
-Maintainer: cliffcotino
-Maintainer-email: cliffcotino@gmail.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: Environment :: Plugins
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: httpie>=3.2.2
-Requires-Dist: pyjwt[crypto]>=2.8.0
-Provides-Extra: testing
-Requires-Dist: pytest; extra == "testing"
-Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pytest_httpserver; extra == "testing"
-Requires-Dist: werkzeug; extra == "testing"
-
 # httpie-oauth2-client-credentials-flow
 
 As an auth plugin for httpie, it obtains a token with the OAuth2.0 client_credentials flow before executing http, and adds the `Authorization: Bearer ${token}` header to the executed request.
 
 **This implementation builds upon the work done by [satodoc](https://github.com/satodoc/httpie-oauth2-client-credentials)**
 
 ## Installation
@@ -160,22 +131,38 @@
 }
 ```
 
 ### Private Key JWT request (application/x-www-form-urlencoded)
 
 Sends a request with `client_assertion_type` set to `urn:ietf:params:oauth:client-assertion-type:jwt-bearer` as defined by the [private_key_jwt](https://openid.net/specs/openid-connect-core-1_0.html#ClientAuthentication) client authentication method.
 The `${CLIENT_SECRET}` value must be a private key in PEM format (or a reference to a certificate in PEM format if the value starts with a `@`-character).
+The `${CLIENT_SECRET}` value can also contain a key in JWK format (or a reference to a file with a JWK if the value starts with a `@`-character).
 
 Private key example:
 ```text
 -----BEGIN PRIVATE KEY-----
 ....
 -----END PRIVATE KEY-----
 ```
 
+Private JWK example:
+```json
+{
+  "p": "4Rbv6bQKVPdT5DOjvM8jaD95uQ3TIOYawN5aNemrt6tUBWZHFYA-XhL-bPo-i6BFMc0bOGaAuEEGXLXO6iiCV8Cuel7y1zULoWM4-Yv4xwbwG00nNQKajftbBkC0AfSdWw5H-3cCT35C8FdrbB-uB6q5h7JRcM28NzjXMDZZ9u0",
+  "kty": "RSA",
+  "q": "8kGdDO2zS9SbInE7DHCGzW9GNTXB4zLlerL0KmkJ1OM9eIrxkycsqZsXJK9-h-S93HCD7gAITCYefMsyGVBc76VmzyQ5GCGHZoYNVInsGi5_yZP_5CijPO_xAG_ptwThxZznMGCLQllpcaXgE0Y6Z86tUWRoz1PUepjoxFBLJBE",
+  "d": "Ho5rZceJdzgU1B0o88w-ghIlOS-D8IJuzsGP_aysevFL5Gst_EcrmU_-V0PrsHWOqiWyny6bEjhkqPI8TbzLQ8SMFK9fRFY9ttFKeQHpGlhCCc1y0p4pMXP4tNtQHag83UPCZHwA7HW4xD6tFbE7Z4j7Qz_8r3f4q-JNKbfymKXmmVWlQIc6Yyb0FOismh-JuM_PDwpMCjzMsgT4arR4XSeX7Uek47IKdqeB6qSoRiwBBY-9jmA0oFE5twPYz8JRy_FKyzGqXDpNo26IL2eJyFXnv4HBBJuBnAm__9XY04qMAgTBHjWOcJSQV7U-P_pW6APLACVXXfxhe0w7tP8IIQ",
+  "e": "AQAB",
+  "qi": "BamCvtzPOnm0GR6LmJxQrjuH4VxdCXBGuElNNe8N5LhqalKyJaYufKF8IaFbyc53SHYkg-GVW4DkfQl60T15OwQCuwPjrSzM-6kXtviHYXN8_NNLN8doMkf_uZ1ImSVTUms9AhzK96FEOGULkVVJafmJQR6ZLI3E_wA5Gn5mJrU",
+  "dp": "X5xcoErHsLu2ONLulD7wbVG5JLAIpIrZhl9stkXhmQz_jaOaQjnNRCyRQj0x4CFeAv96toRj3OBSEYNwtuoqI5hHBNfcEyoHHLCG_QlFzVTXHOGy68OFXxYL3iYR0FrVlF4GmXw90QJy8KBRkwYJ6FvOnyNRkLbzYgmU7nfH0yk",
+  "dq": "uUSEnwaKQEvv-H8v8Wt9LE8VGkxqYx7hcNy67lQ2OKEwuadI6IjlFzCMmnm8AqFksdk6jCFqNxJP7pBXWBSlfoC4B2JkZ5f8vON3_lccQUmeYMLWx95sOIYngXYU_uq03zQHem_bEHrgsRFyNEtZD1p4Ie7wWN57eObH3JqrXIE",
+  "n": "1QFftEW97yHqd3TUsKT3QRVJu8FZDi7l7sYP2qixM07ruEBvvGSVSU4LY5mIjby--yY84eBkqdgh6QPqDVhfwUH1tqfQuKiNn41z21v4p6m_KvDdG2EHIyT3-eas9lRYNe6JU3TJIZQDYCWBF6hZqTq-GMkr1q7mcOTCChP3yvoqyXAhJ9wtcseCJ3iJ9huQDcu7NEZrb2_tVO3G9OLcc8XsynmzmI_4rohii9Ct68HVCGwHifDiixw-9Ge0pSM7bMHAvLvtUf2XNsLpSwZ4_0vDNSSNknTJ96DSB63K4AUO5zEpqaKG6dlrKN1hLdupXE_vRAUT_LB4hPDRqiG5vQ"
+}
+```
+
 The private key is used to generate a signature for the JWT with the following header and payload:
 
 Header:
 ```json
 {
   "alg": "RS256",
   "typ": "JWT"
```

### Comparing `httpie-oauth2-client-credentials-flow-0.3.0/httpie_oauth2_client_credentials_flow.py` & `httpie-oauth2-client-credentials-flow-0.4.0/httpie_oauth2_client_credentials_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 OAuth2.0 client credentials flow plugin for HTTPie.
 """
 import json
-import sys
 import uuid
 from base64 import b64encode
 from datetime import datetime, timedelta
+from json import JSONDecodeError
 from pathlib import Path
 from urllib.error import HTTPError
 from urllib.parse import urlencode
 from urllib.request import Request, urlopen
 
 import jwt
+import sys
 from httpie.cli.definition import parser as httpie_args_parser
 from httpie.plugins import AuthPlugin
+from jwt import PyJWK
 
 
 class OAuth2ClientCredentials:
 
     def __init__(self, client_id, client_secret):
         if not client_id:
             raise ValueError('client_id is required.')
@@ -111,14 +113,24 @@
         key = self.client_secret
         if self.client_secret.startswith('@'):
             key_path = Path(self.client_secret[1:])
             if not key_path.is_file():
                 raise ValueError(f'client_secret "{self.client_secret}" is not a file')
             key = key_path.read_bytes()
 
+        try:
+            jwk = PyJWK(json.loads(key))
+            key = jwk.key
+            jwk_format = True
+        except JSONDecodeError:
+            jwk_format = False
+
+        if jwk_format and self.print_token_request:
+            sys.stdout.write('client_secret was in JWK format\n')
+
         headers = {}
         extra_headers = self.token_assertion_headers
         if extra_headers:
             headers = dict(item.split(':') for item in extra_headers.split(';'))
 
         return jwt.encode(payload, algorithm=algorithm, key=key, headers=headers)
```

### Comparing `httpie-oauth2-client-credentials-flow-0.3.0/setup.py` & `httpie-oauth2-client-credentials-flow-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 setup(
     name='httpie-oauth2-client-credentials-flow',
     description="httpie auth plugin for OAuth2.0 client credentials flow.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
-    version="0.3.0",
+    version="0.4.0",
     author='satdoc',
     author_email='satodoc-develop-public@outlook.com',
     maintainer='cliffcotino',
     maintainer_email='cliffcotino@gmail.com',
     license='MIT',
     url='https://github.com/cliffcotino/httpie-oauth2-client-credentials',
     download_url='https://github.com/cliffcotino/httpie-oauth2-client-credentials',
```

### Comparing `httpie-oauth2-client-credentials-flow-0.3.0/tests/test_httpie_oauth2_client_credentials_flow.py` & `httpie-oauth2-client-credentials-flow-0.4.0/tests/test_httpie_oauth2_client_credentials_flow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import json
-from dataclasses import dataclass
 from pathlib import Path
 from typing import Callable, Union
 
 import jwt
 import pytest
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import serialization
-from cryptography.hazmat.primitives.asymmetric import rsa, ec
 from cryptography.hazmat.primitives.asymmetric.ec import EllipticCurvePublicKey
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
 from httpie.plugins.registry import plugin_manager
+from jwt import PyJWK
 from pytest_httpserver import HTTPServer
 from werkzeug.wrappers import Request, Response
 
-from fixtures import http
+from fixtures import http, generate_key, generate_jwk
 from httpie_oauth2_client_credentials_flow import OAuth2ClientCredentialsPlugin
 
 HTTP_OK = '200 OK'
 BEARER_TOKEN = 'XYZ'
 CLIENT_CREDENTIALS = 'client_credentials'
 CLIENT_ID = 'client-id'
 CLIENT_SECRET = 'client-secret'
@@ -189,14 +186,33 @@
     client_secret = 'T9uMeJ86HugEuaYCABzEOXDBLYDrvp5v'
     r = do_test(httpserver, token_request_type='private-key-jwt', client_secret=client_secret,
                 token_assertions=assertions, extra_args={'--token-assertion-algorithm': alg})
     assert HTTP_OK in r.stdout
     assert r.stderr == ''
 
 
+def test_token_request_type_private_key_jwt_when_given_jwk(httpserver: HTTPServer, tmp_path):
+    def assertions(request: Request):
+        assert request.headers['Content-Type'] == APPLICATION_WWW_FORM_URLENCODED
+        assert request.form['grant_type'] == CLIENT_CREDENTIALS
+        assert request.form['client_assertion_type'] == JWT_BEARER
+        verify_client_assertion(request.form['client_assertion'], httpserver.url_for('/token'), key.public_key(), 'RS256')
+
+    jwk = generate_jwk()
+    jwk_string = json.dumps(jwk)
+
+    key = PyJWK.from_dict(jwk).key
+
+    client_secret = jwk_string
+    r = do_test(httpserver, token_request_type='private-key-jwt', client_secret=client_secret,
+                token_assertions=assertions)
+    assert HTTP_OK in r.stdout
+    assert r.stderr == ''
+
+
 def test_token_request_type_private_key_jwt_when_given_secret_file(httpserver: HTTPServer, tmp_path):
     def assertions(request: Request):
         assert request.headers['Content-Type'] == APPLICATION_WWW_FORM_URLENCODED
         assert request.form['grant_type'] == CLIENT_CREDENTIALS
         assert request.form['client_assertion_type'] == JWT_BEARER
         verify_client_assertion(request.form['client_assertion'], httpserver.url_for('/token'), key.public_key, 'RS256')
 
@@ -207,41 +223,33 @@
     client_secret = f'@{private_key_pem_path}'
     r = do_test(httpserver, token_request_type='private-key-jwt', client_secret=client_secret,
                 token_assertions=assertions)
     assert HTTP_OK in r.stdout
     assert r.stderr == ''
 
 
-@dataclass
-class GeneratedKey:
-    private_key_pem: bytes
-    public_key: Union[RSAPublicKey, EllipticCurvePublicKey]
-
-
-def generate_key(alg: str):
-    if alg.startswith('ES'):
-        private_key = ec.generate_private_key(
-            curve=ec.SECP192R1(),
-            backend=default_backend()
-        )
-    elif alg.startswith('PS') or alg.startswith('RS'):
-        private_key = rsa.generate_private_key(
-            public_exponent=65537,
-            key_size=2048,
-            backend=default_backend()
-        )
-    else:
-        raise ValueError(f'Unexpected value for alg: {alg}')
-    public_key = private_key.public_key()
-    private_key_pem = private_key.private_bytes(
-        encoding=serialization.Encoding.PEM,
-        format=serialization.PrivateFormat.PKCS8,
-        encryption_algorithm=serialization.NoEncryption()
-    )
-    return GeneratedKey(private_key_pem, public_key)
+def test_token_request_type_private_key_jwt_when_given_jwk_file(httpserver: HTTPServer, tmp_path):
+    def assertions(request: Request):
+        assert request.headers['Content-Type'] == APPLICATION_WWW_FORM_URLENCODED
+        assert request.form['grant_type'] == CLIENT_CREDENTIALS
+        assert request.form['client_assertion_type'] == JWT_BEARER
+        verify_client_assertion(request.form['client_assertion'], httpserver.url_for('/token'), key.public_key(), 'RS256')
+
+    jwk = generate_jwk()
+    jwk_string = json.dumps(jwk)
+    jwk_path = Path(tmp_path / 'private_key.jwk')
+    jwk_path.write_bytes(jwk_string.encode('utf8'))
+
+    key = PyJWK.from_dict(jwk).key
+
+    client_secret = f'@{jwk_path}'
+    r = do_test(httpserver, token_request_type='private-key-jwt', client_secret=client_secret,
+                token_assertions=assertions)
+    assert HTTP_OK in r.stdout
+    assert r.stderr == ''
 
 
 def verify_client_assertion(client_assertion: str,
                             audience: str,
                             key: Union[RSAPublicKey, EllipticCurvePublicKey, str, bytes],
                             algorithm: str):
     jwt.decode(client_assertion, issuer=CLIENT_ID, audience=audience, algorithms=algorithm, verify=True, key=key)
```

