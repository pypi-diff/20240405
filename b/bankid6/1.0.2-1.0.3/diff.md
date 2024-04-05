# Comparing `tmp/bankid6-1.0.2.tar.gz` & `tmp/bankid6-1.0.3.tar.gz`

## Comparing `bankid6-1.0.2.tar` & `bankid6-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bankid6-1.0.2/requirements-dev.txt
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bankid6-1.0.2/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 bankid6-1.0.2/tox.ini
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/__init__.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/client.py
--rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/exceptions.py
--rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/handlers.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/listify.py
--rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/message.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/certs/testCARootCert.pem
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/certs/testCert.pem
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 bankid6-1.0.2/src/bankid6/certs/testPrivateKey.pem
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bankid6-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 bankid6-1.0.2/tests/factories.py
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 bankid6-1.0.2/tests/test_client.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 bankid6-1.0.2/tests/test_exceptions.py
--rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 bankid6-1.0.2/tests/test_handlers.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 bankid6-1.0.2/tests/test_message.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bankid6-1.0.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bankid6-1.0.2/LICENSE
--rw-r--r--   0        0        0    25681 2020-02-02 00:00:00.000000 bankid6-1.0.2/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 bankid6-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    26206 2020-02-02 00:00:00.000000 bankid6-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bankid6-1.0.3/requirements-dev.txt
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bankid6-1.0.3/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 bankid6-1.0.3/tox.ini
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/__init__.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/client.py
+-rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/exceptions.py
+-rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/handlers.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/listify.py
+-rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/message.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/certs/testCARootCert.pem
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/certs/testCert.pem
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/certs/testPrivateKey.pem
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bankid6-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 bankid6-1.0.3/tests/factories.py
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 bankid6-1.0.3/tests/test_client.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 bankid6-1.0.3/tests/test_exceptions.py
+-rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 bankid6-1.0.3/tests/test_handlers.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 bankid6-1.0.3/tests/test_message.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bankid6-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bankid6-1.0.3/LICENSE
+-rw-r--r--   0        0        0    25888 2020-02-02 00:00:00.000000 bankid6-1.0.3/README.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 bankid6-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 bankid6-1.0.3/PKG-INFO
```

### Comparing `bankid6-1.0.2/src/bankid6/client.py` & `bankid6-1.0.3/src/bankid6/client.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.2/src/bankid6/exceptions.py` & `bankid6-1.0.3/src/bankid6/exceptions.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.2/src/bankid6/handlers.py` & `bankid6-1.0.3/src/bankid6/handlers.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.2/src/bankid6/listify.py` & `bankid6-1.0.3/src/bankid6/listify.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.2/src/bankid6/message.py` & `bankid6-1.0.3/src/bankid6/message.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.2/src/bankid6/certs/testCARootCert.pem` & `bankid6-1.0.3/src/bankid6/certs/testCARootCert.pem`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.2/src/bankid6/certs/testCert.pem` & `bankid6-1.0.3/src/bankid6/certs/testCert.pem`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.2/src/bankid6/certs/testPrivateKey.pem` & `bankid6-1.0.3/src/bankid6/certs/testPrivateKey.pem`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.2/tests/factories.py` & `bankid6-1.0.3/tests/factories.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.2/tests/test_client.py` & `bankid6-1.0.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.2/tests/test_exceptions.py` & `bankid6-1.0.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.2/tests/test_handlers.py` & `bankid6-1.0.3/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.2/tests/test_message.py` & `bankid6-1.0.3/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.2/LICENSE` & `bankid6-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.2/README.md` & `bankid6-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # bankid6
 
 <br/>
 
 ## Overview
 
-A complete implementation of swedish BankID authentication system version 6. It includes initiating/collect/cancel authentication order, User Message and exceptaion handling according to [BankID Documentaion](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide/rp-introduktion).
+A complete implementation of Swedish BankID authentication system version 6.  It includes initiating/collecting/canceling authentication orders, user Messages and exception handling according to [BankID Documentaion](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide/rp-introduktion).
 <br/>
 <br/>
 
 ## Installation
 
 ```
 pip install bankid6
@@ -16,15 +16,15 @@
 Supports python version 3.6 and later.
 
 <br/>
 <br/>
 
 ## Quick Start
 
-The following sample script can get you started quickly. There are more functionalities and customization options than what has shown here.
+The following sample script can get you started quickly. There are more functionalities and customization options than what has been shown here.
 
 
 ```python
 import time
 from bankid6 import BankIdClient, CollectStatuses, UseTypes, Languages, BankIdError, HintCodes
 
 
@@ -117,22 +117,22 @@
 <br/>
 <br/>
 
 ## User Guide
 
 ### 1. Instantiate `BankIdClient` Class
 
-`BankIdClient` provides functionality to initiate authentication or signing order, collect order result or cancel the order.
+`BankIdClient` provides functionality to initiate authentication or signing orders, collect order results or cancel the order.
 
 Instantiate for `BankIdClient` for test environment.
 ```
 >>> from bankid6 import BankIdClient
 >>> bankid_client = BankIdClient()
 ```
-This instance will use BankID test url, test certificates which are provided in the package. It's configured for computers. It can be initialized for mobile devices which helps to render correct message and correct url for launching the app.
+This instance will use BankID test url, test certificates which are provided in the package. It's configured for computers. It can be initialized for mobile devices which helps to render correct messages and correct urls for launching the app.
 ```
 >>> bankid_client = BankIdClient(is_mobile=True)            # Default to False
 ```
 <br/>
 
 To initialize for a production environment, ensure that the `prod_env` parameter is set to `True`. Additionally, you must provide the file paths for the certificate, the private key associated with the certificate, and the CA certificate.
 ```
@@ -158,30 +158,30 @@
 >>> start_response.launch_url('https://www.google.com')     # Takes a redirect url as parameter
 'bankid:///?autostarttoken=aaba5bef-1066-42da-b6c6-0730b8c53997&redirect=https%3A%2F%2Fwww.google.com'
 
 >>> [attr for attr in dir(start_response) if not attr.startswith('_')]
 ['autoStartToken', 'data', 'launch_url', 'orderRef', 'order_time', 'qrStartSecret', 'qrStartToken', 'qr_data', 'response', 'status_code', 'url']
 ```
 
-Subsequent QR data can be found in response of `collect` method or from `generate_qr_data` function.
+Subsequent QR data can be found in response of the `collect` method or from the `generate_qr_data` function.
 ```
 >>> from bankid6 import generate_qr_data
 >>> generate_qr_data(start_response.order_time, start_response.qrStartToken, start_response.qrStartSecret)
 'bankid.c03da000-d5de-4435-b81b-66154960784d.250.16f0f42bb4f1a99d41a31e38cd54866fce5a193e277f4d48339a7579ac51fe4e'
 ```
 <br>
 
-The `BankIdClient` also has `phone_auth` and `phone_sign` methods initiate authentication and signing orders while the customer is on the phone. You need to pass a personal number and the BankID will send the request to the customer's BankID app. These methods return a `BankIdPhoneStartResponse` object.
+The `BankIdClient` also has `phone_auth` and `phone_sign` methods that initiate authentication and signing orders while the customer is on the phone. You need to pass a personal number and the BankID will send the request to the customer's BankID app. These methods return a `BankIdPhoneStartResponse` object.
 ```
 >>> phone_start_response = BankIdClient().phone_auth('199002113166', callInitiator="RP")
 >>> [attr for attr in dir(phone_start_response) if not attr.startswith('_')]
 ['data', 'orderRef', 'response', 'status_code', 'url']
 ```
 
-Both `sign` and `phone_sign` methods require `userVisibleData` parameter.
+Both `sign` and `phone_sign` methods require the `userVisibleData` parameter.
 ```
 >>> BankIdClient().sign('192.168.0.1', userVisibleData="Hello! Sign this test documents")
 <class 'bankid6.handlers.BankIdStartResponse'> response status: 200;
 response data: {"orderRef": "6eaf4368-22ae-4309-8768-f58b772d1617", "autoStartToken": "3d973332-8abe-4273-b292-b16c975a1a39", "qrStartToken": "29d0b198-487d-42b8-91a8-c63fc94a2733", "qrStartSecret": "a611ccd5-5940-4160-9fde-20a251716bfb"}
 ```
 
 These methods have required or optional parameters exactly as described in BankID documentation. These parameters are validated, processed as BankID requires and sent as the data of the request to the BankID.
@@ -231,19 +231,19 @@
 
 ```
 >>> sr = BankIdClient().auth('192.168.0.1')
 >>> cr = BankIdClient().collect(orderRef=sr.orderRef, qrStartToken=sr.qrStartToken, qrStartSecret=sr.qrStartSecret, order_time=sr.order_time)
 >>> cr.qr_data
 'bankid.d9c9339c-b9d3-48a2-8289-8d66e1d28a08.21.941023af5b86d5b16aaa226ad7130ee08a1dcdca89e199639a3986336a0569fb'
 ```
-`orderRef` parameter is used to find the order and `qrStartToken`, `qrStartSecret` and `order_time` parameters are used to calculate the QR code. `qr_data` attribute in `BankIdCollectResponse` object is accessible if the `collect` method is invoked from the same client where order was initiated, or if these parameters are provided.
+The `orderRef` parameter is used to find the order and `qrStartToken`, `qrStartSecret` and `order_time` parameters are used to calculate the QR code. The `qr_data` attribute in the `BankIdCollectResponse` object is accessible if the `collect` method is invoked from the same client where order was initiated, or if these parameters are provided.
 
 #### User Message
 
-`BankIdCollectResponse` also has `message` attribute which contains user message according to BankID documentation when the status is 'pending' or 'failed'. A message depends on how order was initiated and the language. Each message is a dict constructed like this:
+`BankIdCollectResponse` also has a `message` attribute which contains user messages according to BankID documentation when the status is 'pending' or 'failed'. A message depends on how order was initiated and the language. Each message is a dict constructed like this:
 ```python
 {
     "qrcode": {             # order initiated by scanning qr code
         "swedish": "",
         "english": ""
     },
     "onfile": {             # order initiated by starting the bankid app on the same device
@@ -258,15 +258,15 @@
 ```
 >>> cr = bankid_client.collect()
 >>> from bankid6 import UseTypes, Languages
 >>> print(cr.message[UseTypes.qrcode][Languages.en]) if cr.status in [CollectStatuses.complete, CollectStatuses.failed]
 'Start your BankID app.'
 ```
 
-You can make a subclass of `Messages`, override it's existing messages and pass it to`BankIdClient` as a parameter. Any message in `Messages` class is a attribute which starts with 'RFA' as in BankID documentation.
+You can make a subclass of `Messages`, override its existing messages and pass it to`BankIdClient` as a parameter. Any message in `Messages` class is an attribute which starts with 'RFA' as in BankID documentation.
 ```python
 from bankid6 import Messages
 
 print(Messages.RFA1.help_text) # prints 'status=pending, hintCode=outstandingTransaction, hintCode=noClient'
 
 class MyMessage(Messages):
     RFA1 = {'test': 'yes'}
@@ -288,95 +288,95 @@
 response data: {"orderRef": "ccc9b028-4c83-49f8-b5ae-a3bac54a7427", "autoStartToken": "96c45dea-d14c-4bc5-bf30-db4015d39da9", "qrStartToken": "d550a68e-1e4d-4d66-8dce-3c6497c8da73", "qrStartSecret": "4b3bba21-ebaa-4bf4-8856-e66271550b78"}
 
 >>> bankid_client.cancel()
 <class 'bankid6.handlers.BankIdCancelResponse'> response status: 200;
 response data: {}
 ```
 
-This can be decouple by using it's `orderRef` parameter.
+This can be decoupled by using its `orderRef` parameter.
 
 ```
 >>> start_response = BankIdClient().auth('192.168.0.1')
 >>> BankIdClient().auth(orderRef=start_response.orderRef)
 <class 'bankid6.handlers.BankIdCancelResponse'> response status: 200;
 response data: {}
 ```
 <br/>
 <br/>
 
 ### 5. Exceptions
 
 All methods in `BankIdClient` can raise `BankIdError` or `BankIdValidationError`. 
 
-`BankIdError` is raised when a request is made to BankID server and it returned an error. It has `message` attribute with structure like:
+`BankIdError` is raised when a request is made to BankID server and it returns an error. It has `message` attribute with structure like:
 ```json
 {
     "swedish": "",
     "english": ""
 }
 ```
-If the message is available, it indicates that the message should be presented to the customer without any additional action required. Otherwise, the `reason` and `action` attributes can provide information on why the error occurred and what steps need to be taken to address it according to BankID documentation. Attribute `response_data` has the data received from bankid in dict format. See Api Reference section for more functionalities.
+If the message is available, it indicates that the message should be presented to the customer without any additional action required. Otherwise, the `reason` and `action` attributes can provide information on why the error occurred and what steps need to be taken to address it according to BankID documentation. Attribute `response_data` has the data received from BankID in dict format. See Api Reference section for more functionalities.
 
 
 `BankIdValidationError` is raised before sending the request to BankID if any parameter is invalid.
 
 <br/>
 <br/>
 <br/>
 <br/>
 
 ## API Reference
 
 
 #### class BankIdClient()
 
-##### def __init__(self, prod_env: bool=False, cert_pem: str=None, key_pem: str=None, ca_pem: str=None, request_timeout: int=None, messages: Messages=Messages, is_mobile: bool=False)
+**def __init__(self, prod_env: bool=False, cert_pem: str=None, key_pem: str=None, ca_pem: str=None, request_timeout: int=None, messages: Messages=Messages, is_mobile: bool=False)**
 
 **Parameters:**
 - `prod_env` indicates if it's a production environment. Test or prod urls are chosen based on this. If it is `True` then `key_pem`, `cert_pem` and `ca_pem` are required. Otherwise test certificates which are already included in the package will be used. Any or all of the certificates can also be provided when the value is `False`
 - `cert_pem` file path of the certificate file
 - `key_pem` file path of the private key of the certificate.
 - `ca_pem` file path of CA certificate file
 - `request_timeout` number of seconds to wait for response
 - `messages` class or subclass of `Messages` class to override existing message
 - `is_mobile` if it's being used in a mobile device.
 <br/>
 <br/>
 
-##### def auth(endUserIp: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None):
+**def auth(endUserIp: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None):**
 
-Starts the bankid auth process. Use this when only user authentication is needed.
+Starts the BankID auth process. Use this when only user authentication is needed.
 
 **Parameters:**
-- `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 is allowed.
+- `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 are allowed.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userVisibleData` *Optional*. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdStartResponse`
 <br/>
 <br/>
 
-##### def sign(endUserIp: str, userVisibleData: str, requirement: dict=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)
+**def sign(endUserIp: str, userVisibleData: str, requirement: dict=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)**
 
-Starts the bankid sign process. Use this when user is authenticated to sign something.
+Starts the BankID sign process. Use this when user is authenticated to sign something.
 
 **Parameters:**
-- `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 is allowed.
+- `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 are allowed.
 - `userVisibleData` ***Required***. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdStartResponse`
 <br/>
 <br/>
 
-##### def phone_auth(personalNumber: str, callInitiator: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)
+**def phone_auth(personalNumber: str, callInitiator: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)**
 
 Initiates an authentication order when the user is talking to the RP over the phone. 
 
 **Parameters:**
 - `personalNumber` ***Required***. *str*. Any valid 12 digit personal number of the user.
 - `callInitiator` ***Required***. *str*. choice between 'user' or 'RP'.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
@@ -384,15 +384,15 @@
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdPhoneStartResponse`
 <br/>
 <br/>
 
-##### def phone_sign(personalNumber, callInitiator, userVisibleData, requirement=None, userNonVisibleData=None, userVisibleDataFormat=None)
+**def phone_sign(personalNumber, callInitiator, userVisibleData, requirement=None, userNonVisibleData=None, userVisibleDataFormat=None)**
 
 Initiates an signing order when the user is talking to the RP over the phone.
 
 **Parameters:**
 - `personalNumber` ***Required***. *str*. Any valid 12 digit personal number of the user.
 - `callInitiator` ***Required***. *str*. choice between 'user' or 'RP'.
 - `userVisibleData` ***Required***. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
@@ -400,32 +400,32 @@
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdPhoneStartResponse`
 <br/>
 <br/>
 
-##### def collect(orderRef: str=None, qrStartToken: str=None, qrStartSecret: str=None, order_time: int=None)
+**def collect(orderRef: str=None, qrStartToken: str=None, qrStartSecret: str=None, order_time: int=None)**
 
 Collect the result of the `auth`, `sign`, `phone_auth` or `phone_sign` methods. If used from same client instance when order was initiated, it doesn't require any parameters
 
-- `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then corresponding order result will be requested. Usefull when the method is being used from different client instance than where the order was started.
+- `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then the corresponding order result will be requested. Useful when the method is being used from the different client instance than where the order was started.
 - `qrStartToken` *Optional*. *str*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 - `qrStartSecret` *Optional*. *str*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 - `order_time` *Optional*. *int*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 
 **Return:** `BankIdCollectResponse`
 <br/>
 <br/>
 
-##### def cancel(orderRef: str=None):
+**def cancel(orderRef: str=None):**
 
 Cancels an ongoing sign or auth order. If used from same client instance when order was initiated, it doesn't require any parameters
 
-- `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then corresponding order result will be requested. Usefull when the method is being used from different client instance than where the order was started.
+- `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then the corresponding order result will be requested. Useful when the method is being used from the different client instance than where the order was started.
 
 **Return:** `BankIdCancelResponse`
 
 <br/>
 <br/>
 <br/>
 
@@ -476,58 +476,67 @@
     "onfile": {             # order initiated by starting the bankid app on the same device
         "swedish": "",
         "english": ""
     }
 } 
 ```
 <br/>
+<br/>
 
-##### class BankIdCompletionData()
+### class BankIdCompletionData()
 `user`: *BankIdCompletionUserData*. Authenticated user information.
 `device`: *BankIdCompletionDeviceData*. Authenticated user's device information.
-`bankIdIssueDate`: *datatime*. The date the BankID was issued to the user.
+`bankIdIssueDate`: *datetime*. The date the BankID was issued to the user.
 `stepUp`: *str*. Information about extra verifications that were part of the transaction.
 `signature`: *str*. The signature as described in the BankID Signature Profile specification. Base64-encoded.
 `ocspResponse`: *str*. The OCSP response. Base64-encoded. The OCSP response is signed by a certificate that has the same issuer as the certificate being verified. The OSCP response has an extension for Nonce. The nonce is calculated as:
 - SHA-1 hash over the base 64 XML signature encoded as UTF-8.
-- 12 random bytes is added after the hash.
+- 12 random bytes are added after the hash.
 - The nonce is 32 bytes (20 + 12).
 `json`: *dict*. Completion data in dict format.
 <br/>
 
-##### class BankIdCompletionUserData()
+### class BankIdCompletionUserData()
 `personalNumber`: *str*. The personal identity number.
 `name`: *str*. The given name and surname of the user.
 `givenName`: *str*. The given name of the user.
 `surname`: *str*. The surname of the user.
 <br/>
+<br/>
 
-##### class BankIdCompletionDeviceData()
-`ipAddress`: *str*. The IP address of the user agent as the BankID server discovers it. When an order is started with autoStartToken the RP can check that this match the IP they observe to ensure session fixation String.
-`uhi`: *str*. Unique hardware identifier for the users device.
+### class BankIdCompletionDeviceData()
+`ipAddress`: *str*. The IP address of the user agent as the BankID server discovers it. When an order is started with autoStartToken the RP can check that this matchs the IP they observe to ensure session fixation String.
+`uhi`: *str*. Unique hardware identifier for the user's device.
 
 <br/>
 <br/>
 <br/>
 
-#### class BankIdCancelResponse(BankIdBaseResponse)
+### class BankIdCancelResponse(BankIdBaseResponse)
 ***...***
 
 <br/>
 <br/>
 <br/>
 
-#### class BankIdError(Exception)
-`reason`: *str*. Reason of the exception according to BankID Documentation
+### class BankIdError(Exception)
+`reason`: *str*. Reason of the exception according to the BankID Documentation
 `action`: *str*. What action is needed for this exception according to BankID Documentation
-`message`: *dict*. Message for user.
+`message`: *dict*. Message for users.
 `errorCode`: *str*. Error code received in response data
 `response`: *requests.Response*. object which was returned from sending the request.
 `response_status`: *int*. Http response code of the response
 `response_data`: *dict*. returned data in dict format
 
 <br/>
 <br/>
 <br/>
 
-#### class BankIdValidationError(Exception)
+### class BankIdValidationError(Exception)
 ***...***
+
+<br/>
+<br/>
+<br/>
+
+
+***Any comments or reports on the Github [issue page]("https://github.com/mdamire/bankid-6/issues") are much appreciated.***
```

### Comparing `bankid6-1.0.2/pyproject.toml` & `bankid6-1.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bankid6"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Amir Ebrahim", email="md.amire02@gmail.com" },
 ]
 description = """
   A complete implementation of swedish BankID version 6. 
   Easily initiate, collect and cancel authentication orders, 
   show user message and handle errors.
@@ -19,7 +19,11 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "requests"
 ]
+
+[project.urls]
+Homepage = "https://github.com/mdamire/bankid-6"
+Issues = "https://github.com/mdamire/bankid-6/issues"
```

### Comparing `bankid6-1.0.2/PKG-INFO` & `bankid6-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.3
 Name: bankid6
-Version: 1.0.2
+Version: 1.0.3
 Summary:   A complete implementation of swedish BankID version 6.    Easily initiate, collect and cancel authentication orders,    show user message and handle errors.
+Project-URL: Homepage, https://github.com/mdamire/bankid-6
+Project-URL: Issues, https://github.com/mdamire/bankid-6/issues
 Author-email: Amir Ebrahim <md.amire02@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: requests
@@ -13,15 +15,15 @@
 
 # bankid6
 
 <br/>
 
 ## Overview
 
-A complete implementation of swedish BankID authentication system version 6. It includes initiating/collect/cancel authentication order, User Message and exceptaion handling according to [BankID Documentaion](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide/rp-introduktion).
+A complete implementation of Swedish BankID authentication system version 6.  It includes initiating/collecting/canceling authentication orders, user Messages and exception handling according to [BankID Documentaion](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide/rp-introduktion).
 <br/>
 <br/>
 
 ## Installation
 
 ```
 pip install bankid6
@@ -29,15 +31,15 @@
 Supports python version 3.6 and later.
 
 <br/>
 <br/>
 
 ## Quick Start
 
-The following sample script can get you started quickly. There are more functionalities and customization options than what has shown here.
+The following sample script can get you started quickly. There are more functionalities and customization options than what has been shown here.
 
 
 ```python
 import time
 from bankid6 import BankIdClient, CollectStatuses, UseTypes, Languages, BankIdError, HintCodes
 
 
@@ -130,22 +132,22 @@
 <br/>
 <br/>
 
 ## User Guide
 
 ### 1. Instantiate `BankIdClient` Class
 
-`BankIdClient` provides functionality to initiate authentication or signing order, collect order result or cancel the order.
+`BankIdClient` provides functionality to initiate authentication or signing orders, collect order results or cancel the order.
 
 Instantiate for `BankIdClient` for test environment.
 ```
 >>> from bankid6 import BankIdClient
 >>> bankid_client = BankIdClient()
 ```
-This instance will use BankID test url, test certificates which are provided in the package. It's configured for computers. It can be initialized for mobile devices which helps to render correct message and correct url for launching the app.
+This instance will use BankID test url, test certificates which are provided in the package. It's configured for computers. It can be initialized for mobile devices which helps to render correct messages and correct urls for launching the app.
 ```
 >>> bankid_client = BankIdClient(is_mobile=True)            # Default to False
 ```
 <br/>
 
 To initialize for a production environment, ensure that the `prod_env` parameter is set to `True`. Additionally, you must provide the file paths for the certificate, the private key associated with the certificate, and the CA certificate.
 ```
@@ -171,30 +173,30 @@
 >>> start_response.launch_url('https://www.google.com')     # Takes a redirect url as parameter
 'bankid:///?autostarttoken=aaba5bef-1066-42da-b6c6-0730b8c53997&redirect=https%3A%2F%2Fwww.google.com'
 
 >>> [attr for attr in dir(start_response) if not attr.startswith('_')]
 ['autoStartToken', 'data', 'launch_url', 'orderRef', 'order_time', 'qrStartSecret', 'qrStartToken', 'qr_data', 'response', 'status_code', 'url']
 ```
 
-Subsequent QR data can be found in response of `collect` method or from `generate_qr_data` function.
+Subsequent QR data can be found in response of the `collect` method or from the `generate_qr_data` function.
 ```
 >>> from bankid6 import generate_qr_data
 >>> generate_qr_data(start_response.order_time, start_response.qrStartToken, start_response.qrStartSecret)
 'bankid.c03da000-d5de-4435-b81b-66154960784d.250.16f0f42bb4f1a99d41a31e38cd54866fce5a193e277f4d48339a7579ac51fe4e'
 ```
 <br>
 
-The `BankIdClient` also has `phone_auth` and `phone_sign` methods initiate authentication and signing orders while the customer is on the phone. You need to pass a personal number and the BankID will send the request to the customer's BankID app. These methods return a `BankIdPhoneStartResponse` object.
+The `BankIdClient` also has `phone_auth` and `phone_sign` methods that initiate authentication and signing orders while the customer is on the phone. You need to pass a personal number and the BankID will send the request to the customer's BankID app. These methods return a `BankIdPhoneStartResponse` object.
 ```
 >>> phone_start_response = BankIdClient().phone_auth('199002113166', callInitiator="RP")
 >>> [attr for attr in dir(phone_start_response) if not attr.startswith('_')]
 ['data', 'orderRef', 'response', 'status_code', 'url']
 ```
 
-Both `sign` and `phone_sign` methods require `userVisibleData` parameter.
+Both `sign` and `phone_sign` methods require the `userVisibleData` parameter.
 ```
 >>> BankIdClient().sign('192.168.0.1', userVisibleData="Hello! Sign this test documents")
 <class 'bankid6.handlers.BankIdStartResponse'> response status: 200;
 response data: {"orderRef": "6eaf4368-22ae-4309-8768-f58b772d1617", "autoStartToken": "3d973332-8abe-4273-b292-b16c975a1a39", "qrStartToken": "29d0b198-487d-42b8-91a8-c63fc94a2733", "qrStartSecret": "a611ccd5-5940-4160-9fde-20a251716bfb"}
 ```
 
 These methods have required or optional parameters exactly as described in BankID documentation. These parameters are validated, processed as BankID requires and sent as the data of the request to the BankID.
@@ -244,19 +246,19 @@
 
 ```
 >>> sr = BankIdClient().auth('192.168.0.1')
 >>> cr = BankIdClient().collect(orderRef=sr.orderRef, qrStartToken=sr.qrStartToken, qrStartSecret=sr.qrStartSecret, order_time=sr.order_time)
 >>> cr.qr_data
 'bankid.d9c9339c-b9d3-48a2-8289-8d66e1d28a08.21.941023af5b86d5b16aaa226ad7130ee08a1dcdca89e199639a3986336a0569fb'
 ```
-`orderRef` parameter is used to find the order and `qrStartToken`, `qrStartSecret` and `order_time` parameters are used to calculate the QR code. `qr_data` attribute in `BankIdCollectResponse` object is accessible if the `collect` method is invoked from the same client where order was initiated, or if these parameters are provided.
+The `orderRef` parameter is used to find the order and `qrStartToken`, `qrStartSecret` and `order_time` parameters are used to calculate the QR code. The `qr_data` attribute in the `BankIdCollectResponse` object is accessible if the `collect` method is invoked from the same client where order was initiated, or if these parameters are provided.
 
 #### User Message
 
-`BankIdCollectResponse` also has `message` attribute which contains user message according to BankID documentation when the status is 'pending' or 'failed'. A message depends on how order was initiated and the language. Each message is a dict constructed like this:
+`BankIdCollectResponse` also has a `message` attribute which contains user messages according to BankID documentation when the status is 'pending' or 'failed'. A message depends on how order was initiated and the language. Each message is a dict constructed like this:
 ```python
 {
     "qrcode": {             # order initiated by scanning qr code
         "swedish": "",
         "english": ""
     },
     "onfile": {             # order initiated by starting the bankid app on the same device
@@ -271,15 +273,15 @@
 ```
 >>> cr = bankid_client.collect()
 >>> from bankid6 import UseTypes, Languages
 >>> print(cr.message[UseTypes.qrcode][Languages.en]) if cr.status in [CollectStatuses.complete, CollectStatuses.failed]
 'Start your BankID app.'
 ```
 
-You can make a subclass of `Messages`, override it's existing messages and pass it to`BankIdClient` as a parameter. Any message in `Messages` class is a attribute which starts with 'RFA' as in BankID documentation.
+You can make a subclass of `Messages`, override its existing messages and pass it to`BankIdClient` as a parameter. Any message in `Messages` class is an attribute which starts with 'RFA' as in BankID documentation.
 ```python
 from bankid6 import Messages
 
 print(Messages.RFA1.help_text) # prints 'status=pending, hintCode=outstandingTransaction, hintCode=noClient'
 
 class MyMessage(Messages):
     RFA1 = {'test': 'yes'}
@@ -301,95 +303,95 @@
 response data: {"orderRef": "ccc9b028-4c83-49f8-b5ae-a3bac54a7427", "autoStartToken": "96c45dea-d14c-4bc5-bf30-db4015d39da9", "qrStartToken": "d550a68e-1e4d-4d66-8dce-3c6497c8da73", "qrStartSecret": "4b3bba21-ebaa-4bf4-8856-e66271550b78"}
 
 >>> bankid_client.cancel()
 <class 'bankid6.handlers.BankIdCancelResponse'> response status: 200;
 response data: {}
 ```
 
-This can be decouple by using it's `orderRef` parameter.
+This can be decoupled by using its `orderRef` parameter.
 
 ```
 >>> start_response = BankIdClient().auth('192.168.0.1')
 >>> BankIdClient().auth(orderRef=start_response.orderRef)
 <class 'bankid6.handlers.BankIdCancelResponse'> response status: 200;
 response data: {}
 ```
 <br/>
 <br/>
 
 ### 5. Exceptions
 
 All methods in `BankIdClient` can raise `BankIdError` or `BankIdValidationError`. 
 
-`BankIdError` is raised when a request is made to BankID server and it returned an error. It has `message` attribute with structure like:
+`BankIdError` is raised when a request is made to BankID server and it returns an error. It has `message` attribute with structure like:
 ```json
 {
     "swedish": "",
     "english": ""
 }
 ```
-If the message is available, it indicates that the message should be presented to the customer without any additional action required. Otherwise, the `reason` and `action` attributes can provide information on why the error occurred and what steps need to be taken to address it according to BankID documentation. Attribute `response_data` has the data received from bankid in dict format. See Api Reference section for more functionalities.
+If the message is available, it indicates that the message should be presented to the customer without any additional action required. Otherwise, the `reason` and `action` attributes can provide information on why the error occurred and what steps need to be taken to address it according to BankID documentation. Attribute `response_data` has the data received from BankID in dict format. See Api Reference section for more functionalities.
 
 
 `BankIdValidationError` is raised before sending the request to BankID if any parameter is invalid.
 
 <br/>
 <br/>
 <br/>
 <br/>
 
 ## API Reference
 
 
 #### class BankIdClient()
 
-##### def __init__(self, prod_env: bool=False, cert_pem: str=None, key_pem: str=None, ca_pem: str=None, request_timeout: int=None, messages: Messages=Messages, is_mobile: bool=False)
+**def __init__(self, prod_env: bool=False, cert_pem: str=None, key_pem: str=None, ca_pem: str=None, request_timeout: int=None, messages: Messages=Messages, is_mobile: bool=False)**
 
 **Parameters:**
 - `prod_env` indicates if it's a production environment. Test or prod urls are chosen based on this. If it is `True` then `key_pem`, `cert_pem` and `ca_pem` are required. Otherwise test certificates which are already included in the package will be used. Any or all of the certificates can also be provided when the value is `False`
 - `cert_pem` file path of the certificate file
 - `key_pem` file path of the private key of the certificate.
 - `ca_pem` file path of CA certificate file
 - `request_timeout` number of seconds to wait for response
 - `messages` class or subclass of `Messages` class to override existing message
 - `is_mobile` if it's being used in a mobile device.
 <br/>
 <br/>
 
-##### def auth(endUserIp: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None):
+**def auth(endUserIp: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None):**
 
-Starts the bankid auth process. Use this when only user authentication is needed.
+Starts the BankID auth process. Use this when only user authentication is needed.
 
 **Parameters:**
-- `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 is allowed.
+- `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 are allowed.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userVisibleData` *Optional*. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdStartResponse`
 <br/>
 <br/>
 
-##### def sign(endUserIp: str, userVisibleData: str, requirement: dict=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)
+**def sign(endUserIp: str, userVisibleData: str, requirement: dict=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)**
 
-Starts the bankid sign process. Use this when user is authenticated to sign something.
+Starts the BankID sign process. Use this when user is authenticated to sign something.
 
 **Parameters:**
-- `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 is allowed.
+- `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 are allowed.
 - `userVisibleData` ***Required***. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdStartResponse`
 <br/>
 <br/>
 
-##### def phone_auth(personalNumber: str, callInitiator: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)
+**def phone_auth(personalNumber: str, callInitiator: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)**
 
 Initiates an authentication order when the user is talking to the RP over the phone. 
 
 **Parameters:**
 - `personalNumber` ***Required***. *str*. Any valid 12 digit personal number of the user.
 - `callInitiator` ***Required***. *str*. choice between 'user' or 'RP'.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
@@ -397,15 +399,15 @@
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdPhoneStartResponse`
 <br/>
 <br/>
 
-##### def phone_sign(personalNumber, callInitiator, userVisibleData, requirement=None, userNonVisibleData=None, userVisibleDataFormat=None)
+**def phone_sign(personalNumber, callInitiator, userVisibleData, requirement=None, userNonVisibleData=None, userVisibleDataFormat=None)**
 
 Initiates an signing order when the user is talking to the RP over the phone.
 
 **Parameters:**
 - `personalNumber` ***Required***. *str*. Any valid 12 digit personal number of the user.
 - `callInitiator` ***Required***. *str*. choice between 'user' or 'RP'.
 - `userVisibleData` ***Required***. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
@@ -413,32 +415,32 @@
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdPhoneStartResponse`
 <br/>
 <br/>
 
-##### def collect(orderRef: str=None, qrStartToken: str=None, qrStartSecret: str=None, order_time: int=None)
+**def collect(orderRef: str=None, qrStartToken: str=None, qrStartSecret: str=None, order_time: int=None)**
 
 Collect the result of the `auth`, `sign`, `phone_auth` or `phone_sign` methods. If used from same client instance when order was initiated, it doesn't require any parameters
 
-- `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then corresponding order result will be requested. Usefull when the method is being used from different client instance than where the order was started.
+- `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then the corresponding order result will be requested. Useful when the method is being used from the different client instance than where the order was started.
 - `qrStartToken` *Optional*. *str*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 - `qrStartSecret` *Optional*. *str*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 - `order_time` *Optional*. *int*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 
 **Return:** `BankIdCollectResponse`
 <br/>
 <br/>
 
-##### def cancel(orderRef: str=None):
+**def cancel(orderRef: str=None):**
 
 Cancels an ongoing sign or auth order. If used from same client instance when order was initiated, it doesn't require any parameters
 
-- `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then corresponding order result will be requested. Usefull when the method is being used from different client instance than where the order was started.
+- `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then the corresponding order result will be requested. Useful when the method is being used from the different client instance than where the order was started.
 
 **Return:** `BankIdCancelResponse`
 
 <br/>
 <br/>
 <br/>
 
@@ -489,58 +491,67 @@
     "onfile": {             # order initiated by starting the bankid app on the same device
         "swedish": "",
         "english": ""
     }
 } 
 ```
 <br/>
+<br/>
 
-##### class BankIdCompletionData()
+### class BankIdCompletionData()
 `user`: *BankIdCompletionUserData*. Authenticated user information.
 `device`: *BankIdCompletionDeviceData*. Authenticated user's device information.
-`bankIdIssueDate`: *datatime*. The date the BankID was issued to the user.
+`bankIdIssueDate`: *datetime*. The date the BankID was issued to the user.
 `stepUp`: *str*. Information about extra verifications that were part of the transaction.
 `signature`: *str*. The signature as described in the BankID Signature Profile specification. Base64-encoded.
 `ocspResponse`: *str*. The OCSP response. Base64-encoded. The OCSP response is signed by a certificate that has the same issuer as the certificate being verified. The OSCP response has an extension for Nonce. The nonce is calculated as:
 - SHA-1 hash over the base 64 XML signature encoded as UTF-8.
-- 12 random bytes is added after the hash.
+- 12 random bytes are added after the hash.
 - The nonce is 32 bytes (20 + 12).
 `json`: *dict*. Completion data in dict format.
 <br/>
 
-##### class BankIdCompletionUserData()
+### class BankIdCompletionUserData()
 `personalNumber`: *str*. The personal identity number.
 `name`: *str*. The given name and surname of the user.
 `givenName`: *str*. The given name of the user.
 `surname`: *str*. The surname of the user.
 <br/>
+<br/>
 
-##### class BankIdCompletionDeviceData()
-`ipAddress`: *str*. The IP address of the user agent as the BankID server discovers it. When an order is started with autoStartToken the RP can check that this match the IP they observe to ensure session fixation String.
-`uhi`: *str*. Unique hardware identifier for the users device.
+### class BankIdCompletionDeviceData()
+`ipAddress`: *str*. The IP address of the user agent as the BankID server discovers it. When an order is started with autoStartToken the RP can check that this matchs the IP they observe to ensure session fixation String.
+`uhi`: *str*. Unique hardware identifier for the user's device.
 
 <br/>
 <br/>
 <br/>
 
-#### class BankIdCancelResponse(BankIdBaseResponse)
+### class BankIdCancelResponse(BankIdBaseResponse)
 ***...***
 
 <br/>
 <br/>
 <br/>
 
-#### class BankIdError(Exception)
-`reason`: *str*. Reason of the exception according to BankID Documentation
+### class BankIdError(Exception)
+`reason`: *str*. Reason of the exception according to the BankID Documentation
 `action`: *str*. What action is needed for this exception according to BankID Documentation
-`message`: *dict*. Message for user.
+`message`: *dict*. Message for users.
 `errorCode`: *str*. Error code received in response data
 `response`: *requests.Response*. object which was returned from sending the request.
 `response_status`: *int*. Http response code of the response
 `response_data`: *dict*. returned data in dict format
 
 <br/>
 <br/>
 <br/>
 
-#### class BankIdValidationError(Exception)
+### class BankIdValidationError(Exception)
 ***...***
+
+<br/>
+<br/>
+<br/>
+
+
+***Any comments or reports on the Github [issue page]("https://github.com/mdamire/bankid-6/issues") are much appreciated.***
```

