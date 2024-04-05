# Comparing `tmp/paystackease-0.1.3.tar.gz` & `tmp/paystackease-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paystackease-0.1.3.tar", max compression
+gzip compressed data, was "paystackease-1.0.0.tar", max compression
```

## Comparing `paystackease-0.1.3.tar` & `paystackease-1.0.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rwxr-xr-x   0        0        0     1090 2024-02-21 14:06:29.101210 paystackease-0.1.3/LICENSE
--rwxr-xr-x   0        0        0     4557 2024-03-26 17:44:14.747576 paystackease-0.1.3/README.md
--rwxr-xr-x   0        0        0     1089 2024-03-19 17:40:27.406049 paystackease-0.1.3/paystackease/__init__.py
--rwxr-xr-x   0        0        0     7146 2024-03-26 00:13:38.591967 paystackease-0.1.3/paystackease/_abase.py
--rwxr-xr-x   0        0        0     6903 2024-03-26 00:13:38.648961 paystackease-0.1.3/paystackease/_base.py
--rwxr-xr-x   0        0        0     5787 2024-03-19 18:44:47.663437 paystackease-0.1.3/paystackease/apaystack.py
--rwxr-xr-x   0        0        0     1549 2024-03-19 18:18:06.367036 paystackease-0.1.3/paystackease/apis/__init__.py
--rwxr-xr-x   0        0        0     1988 2024-03-20 14:42:24.804568 paystackease-0.1.3/paystackease/apis/apple_pay.py
--rwxr-xr-x   0        0        0     4017 2024-03-23 13:17:18.727768 paystackease-0.1.3/paystackease/apis/bulk_charges.py
--rwxr-xr-x   0        0        0     5465 2024-03-25 12:11:17.275074 paystackease-0.1.3/paystackease/apis/charges.py
--rwxr-xr-x   0        0        0     6433 2024-03-20 14:42:24.807568 paystackease-0.1.3/paystackease/apis/customers.py
--rwxr-xr-x   0        0        0     8607 2024-03-25 16:26:48.731906 paystackease-0.1.3/paystackease/apis/dedicated_virtual_accounts.py
--rwxr-xr-x   0        0        0     7457 2024-03-20 14:42:24.810568 paystackease-0.1.3/paystackease/apis/disputes.py
--rwxr-xr-x   0        0        0     1070 2024-03-20 14:42:24.811568 paystackease-0.1.3/paystackease/apis/integration.py
--rwxr-xr-x   0        0        0     3710 2024-03-26 01:16:48.683011 paystackease-0.1.3/paystackease/apis/miscellaneous.py
--rwxr-xr-x   0        0        0     5265 2024-03-20 14:42:24.815567 paystackease-0.1.3/paystackease/apis/payment_pages.py
--rwxr-xr-x   0        0        0     8681 2024-03-20 14:42:24.816567 paystackease-0.1.3/paystackease/apis/payment_requests.py
--rwxr-xr-x   0        0        0     4012 2024-03-20 14:42:24.817567 paystackease-0.1.3/paystackease/apis/plans.py
--rwxr-xr-x   0        0        0     4046 2024-03-20 14:42:24.819568 paystackease-0.1.3/paystackease/apis/products.py
--rwxr-xr-x   0        0        0     2969 2024-03-20 14:42:24.820567 paystackease-0.1.3/paystackease/apis/refund.py
--rwxr-xr-x   0        0        0     3050 2024-03-20 14:42:24.821567 paystackease-0.1.3/paystackease/apis/settlements.py
--rwxr-xr-x   0        0        0     5849 2024-03-20 14:42:24.822567 paystackease-0.1.3/paystackease/apis/subaccounts.py
--rwxr-xr-x   0        0        0     4092 2024-03-20 14:42:24.823567 paystackease-0.1.3/paystackease/apis/subscriptions.py
--rwxr-xr-x   0        0        0     4836 2024-03-20 14:42:24.824567 paystackease-0.1.3/paystackease/apis/terminal.py
--rwxr-xr-x   0        0        0     5507 2024-03-20 14:42:24.826569 paystackease-0.1.3/paystackease/apis/transaction_splits.py
--rwxr-xr-x   0        0        0    11650 2024-03-20 14:42:24.827569 paystackease-0.1.3/paystackease/apis/transactions.py
--rwxr-xr-x   0        0        0     4915 2024-03-20 14:42:24.829568 paystackease-0.1.3/paystackease/apis/transfer_recipients.py
--rwxr-xr-x   0        0        0     4469 2024-03-20 14:42:24.832570 paystackease-0.1.3/paystackease/apis/transfers.py
--rwxr-xr-x   0        0        0     2466 2024-03-20 14:42:24.834567 paystackease-0.1.3/paystackease/apis/transfers_control.py
--rwxr-xr-x   0        0        0     2703 2024-03-20 14:42:24.835568 paystackease-0.1.3/paystackease/apis/verification.py
--rwxr-xr-x   0        0        0     1826 2024-03-19 18:18:06.382037 paystackease-0.1.3/paystackease/async_apis/__init__.py
--rwxr-xr-x   0        0        0     2049 2024-03-20 14:42:24.836569 paystackease-0.1.3/paystackease/async_apis/aapple_pay.py
--rwxr-xr-x   0        0        0     4119 2024-03-23 12:52:28.819297 paystackease-0.1.3/paystackease/async_apis/abulk_charges.py
--rwxr-xr-x   0        0        0     5570 2024-03-25 12:21:55.889800 paystackease-0.1.3/paystackease/async_apis/acharges.py
--rwxr-xr-x   0        0        0     6541 2024-03-20 14:42:24.840568 paystackease-0.1.3/paystackease/async_apis/acustomers.py
--rwxr-xr-x   0        0        0     8744 2024-03-25 16:26:48.747905 paystackease-0.1.3/paystackease/async_apis/adedicated_virtual_accounts.py
--rwxr-xr-x   0        0        0     7582 2024-03-20 14:42:24.843568 paystackease-0.1.3/paystackease/async_apis/adisputes.py
--rwxr-xr-x   0        0        0     1115 2024-03-20 14:42:24.844567 paystackease-0.1.3/paystackease/async_apis/aintegration.py
--rwxr-xr-x   0        0        0     3762 2024-03-26 01:16:52.839007 paystackease-0.1.3/paystackease/async_apis/amiscellaneous.py
--rwxr-xr-x   0        0        0     5358 2024-03-20 14:42:24.847569 paystackease-0.1.3/paystackease/async_apis/apayment_pages.py
--rwxr-xr-x   0        0        0     8818 2024-03-20 14:42:24.848567 paystackease-0.1.3/paystackease/async_apis/apayment_requests.py
--rwxr-xr-x   0        0        0     4089 2024-03-20 14:42:24.849568 paystackease-0.1.3/paystackease/async_apis/aplans.py
--rwxr-xr-x   0        0        0     4123 2024-03-20 14:42:24.850569 paystackease-0.1.3/paystackease/async_apis/aproducts.py
--rwxr-xr-x   0        0        0     3034 2024-03-20 14:42:24.852571 paystackease-0.1.3/paystackease/async_apis/arefund.py
--rwxr-xr-x   0        0        0     3095 2024-03-20 14:42:24.854569 paystackease-0.1.3/paystackease/async_apis/asettlements.py
--rwxr-xr-x   0        0        0     5932 2024-03-20 14:42:24.855570 paystackease-0.1.3/paystackease/async_apis/asubaccounts.py
--rwxr-xr-x   0        0        0     4192 2024-03-20 14:42:24.857575 paystackease-0.1.3/paystackease/async_apis/asubscriptions.py
--rwxr-xr-x   0        0        0     4959 2024-03-20 14:42:24.859569 paystackease-0.1.3/paystackease/async_apis/aterminal.py
--rwxr-xr-x   0        0        0     5614 2024-03-20 14:42:24.861583 paystackease-0.1.3/paystackease/async_apis/atransaction_splits.py
--rwxr-xr-x   0        0        0    11799 2024-03-20 14:42:24.863568 paystackease-0.1.3/paystackease/async_apis/atransactions.py
--rwxr-xr-x   0        0        0     5016 2024-03-20 14:42:24.865568 paystackease-0.1.3/paystackease/async_apis/atransfer_recipients.py
--rwxr-xr-x   0        0        0     4570 2024-03-20 14:42:24.866568 paystackease-0.1.3/paystackease/async_apis/atransfers.py
--rwxr-xr-x   0        0        0     2567 2024-03-20 14:42:24.868568 paystackease-0.1.3/paystackease/async_apis/atransfers_control.py
--rwxr-xr-x   0        0        0     2767 2024-03-20 14:42:24.869569 paystackease-0.1.3/paystackease/async_apis/averification.py
--rwxr-xr-x   0        0        0      511 2024-03-10 15:44:25.653891 paystackease-0.1.3/paystackease/errors.py
--rwxr-xr-x   0        0        0      417 2024-03-11 15:23:54.460221 paystackease-0.1.3/paystackease/helpers/__init__.py
--rwxr-xr-x   0        0        0      716 2024-03-11 00:29:44.848173 paystackease-0.1.3/paystackease/helpers/convert.py
--rwxr-xr-x   0        0        0     2442 2024-03-04 09:58:45.036874 paystackease-0.1.3/paystackease/helpers/tool_kit.py
--rwxr-xr-x   0        0        0     3079 2024-03-19 18:44:47.645434 paystackease-0.1.3/paystackease/paystack.py
--rwxr-xr-x   0        0        0     2032 2024-03-26 17:55:39.368439 paystackease-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5798 1970-01-01 00:00:00.000000 paystackease-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1090 2024-02-21 14:06:29.101210 paystackease-1.0.0/LICENSE
+-rwxr-xr-x   0        0        0     4976 2024-04-05 08:20:03.228602 paystackease-1.0.0/README.md
+-rwxr-xr-x   0        0        0     1437 2024-04-05 08:20:03.231124 paystackease-1.0.0/paystackease/__init__.py
+-rwxr-xr-x   0        0        0     8198 2024-04-05 01:26:16.260246 paystackease-1.0.0/paystackease/_abase.py
+-rwxr-xr-x   0        0        0     7815 2024-04-05 01:26:16.262246 paystackease-1.0.0/paystackease/_base.py
+-rwxr-xr-x   0        0        0      353 2024-04-05 01:26:16.263248 paystackease-1.0.0/paystackease/_utils.py
+-rwxr-xr-x   0        0        0     5787 2024-03-19 18:44:47.663437 paystackease-1.0.0/paystackease/apaystack.py
+-rwxr-xr-x   0        0        0     1549 2024-03-19 18:18:06.367036 paystackease-1.0.0/paystackease/apis/__init__.py
+-rwxr-xr-x   0        0        0     2123 2024-04-05 08:20:03.232124 paystackease-1.0.0/paystackease/apis/apple_pay.py
+-rwxr-xr-x   0        0        0     4314 2024-04-05 01:26:16.265246 paystackease-1.0.0/paystackease/apis/bulk_charges.py
+-rwxr-xr-x   0        0        0     5821 2024-04-05 01:26:16.267246 paystackease-1.0.0/paystackease/apis/charges.py
+-rwxr-xr-x   0        0        0     6728 2024-04-05 01:26:16.268247 paystackease-1.0.0/paystackease/apis/customers.py
+-rwxr-xr-x   0        0        0     9220 2024-04-05 01:26:16.270245 paystackease-1.0.0/paystackease/apis/dedicated_virtual_accounts.py
+-rwxr-xr-x   0        0        0     7920 2024-04-05 01:26:16.271246 paystackease-1.0.0/paystackease/apis/disputes.py
+-rwxr-xr-x   0        0        0     1140 2024-04-05 01:26:16.272247 paystackease-1.0.0/paystackease/apis/integration.py
+-rwxr-xr-x   0        0        0     4355 2024-04-05 01:26:16.273246 paystackease-1.0.0/paystackease/apis/miscellaneous.py
+-rwxr-xr-x   0        0        0     5610 2024-04-05 01:26:16.275247 paystackease-1.0.0/paystackease/apis/payment_pages.py
+-rwxr-xr-x   0        0        0     9778 2024-04-05 01:26:16.276247 paystackease-1.0.0/paystackease/apis/payment_requests.py
+-rwxr-xr-x   0        0        0     4572 2024-04-05 01:26:16.277245 paystackease-1.0.0/paystackease/apis/plans.py
+-rwxr-xr-x   0        0        0     4254 2024-04-05 01:26:16.279250 paystackease-1.0.0/paystackease/apis/products.py
+-rwxr-xr-x   0        0        0     3250 2024-04-05 01:26:16.280246 paystackease-1.0.0/paystackease/apis/refund.py
+-rwxr-xr-x   0        0        0     3302 2024-04-05 01:26:16.282247 paystackease-1.0.0/paystackease/apis/settlements.py
+-rwxr-xr-x   0        0        0     6263 2024-04-05 01:26:16.283246 paystackease-1.0.0/paystackease/apis/subaccounts.py
+-rwxr-xr-x   0        0        0     4306 2024-04-05 01:26:16.284248 paystackease-1.0.0/paystackease/apis/subscriptions.py
+-rwxr-xr-x   0        0        0     5278 2024-04-05 01:26:16.285247 paystackease-1.0.0/paystackease/apis/terminal.py
+-rwxr-xr-x   0        0        0     5758 2024-04-05 01:26:16.287246 paystackease-1.0.0/paystackease/apis/transaction_splits.py
+-rwxr-xr-x   0        0        0    12570 2024-04-05 01:26:16.288246 paystackease-1.0.0/paystackease/apis/transactions.py
+-rwxr-xr-x   0        0        0     5228 2024-04-05 01:26:16.289246 paystackease-1.0.0/paystackease/apis/transfer_recipients.py
+-rwxr-xr-x   0        0        0     4769 2024-04-05 01:26:16.290248 paystackease-1.0.0/paystackease/apis/transfers.py
+-rwxr-xr-x   0        0        0     2598 2024-04-05 01:26:16.291247 paystackease-1.0.0/paystackease/apis/transfers_control.py
+-rwxr-xr-x   0        0        0     2789 2024-04-05 09:22:55.621501 paystackease-1.0.0/paystackease/apis/verification.py
+-rwxr-xr-x   0        0        0     1826 2024-03-19 18:18:06.382037 paystackease-1.0.0/paystackease/async_apis/__init__.py
+-rwxr-xr-x   0        0        0     2182 2024-04-05 08:20:03.234654 paystackease-1.0.0/paystackease/async_apis/aapple_pay.py
+-rwxr-xr-x   0        0        0     4416 2024-04-05 01:26:16.295246 paystackease-1.0.0/paystackease/async_apis/abulk_charges.py
+-rwxr-xr-x   0        0        0     5926 2024-04-05 01:26:16.296246 paystackease-1.0.0/paystackease/async_apis/acharges.py
+-rwxr-xr-x   0        0        0     6836 2024-04-05 01:26:16.297246 paystackease-1.0.0/paystackease/async_apis/acustomers.py
+-rwxr-xr-x   0        0        0     9357 2024-04-05 01:26:16.299246 paystackease-1.0.0/paystackease/async_apis/adedicated_virtual_accounts.py
+-rwxr-xr-x   0        0        0     8045 2024-04-05 01:26:16.300246 paystackease-1.0.0/paystackease/async_apis/adisputes.py
+-rwxr-xr-x   0        0        0     1185 2024-04-05 01:26:16.301247 paystackease-1.0.0/paystackease/async_apis/aintegration.py
+-rwxr-xr-x   0        0        0     4409 2024-04-05 01:26:16.303247 paystackease-1.0.0/paystackease/async_apis/amiscellaneous.py
+-rwxr-xr-x   0        0        0     5703 2024-04-05 01:26:16.305247 paystackease-1.0.0/paystackease/async_apis/apayment_pages.py
+-rwxr-xr-x   0        0        0     9915 2024-04-05 01:26:16.306246 paystackease-1.0.0/paystackease/async_apis/apayment_requests.py
+-rwxr-xr-x   0        0        0     4649 2024-04-05 01:26:16.308247 paystackease-1.0.0/paystackease/async_apis/aplans.py
+-rwxr-xr-x   0        0        0     4331 2024-04-05 01:26:16.309248 paystackease-1.0.0/paystackease/async_apis/aproducts.py
+-rwxr-xr-x   0        0        0     3315 2024-04-05 01:26:16.310247 paystackease-1.0.0/paystackease/async_apis/arefund.py
+-rwxr-xr-x   0        0        0     3347 2024-04-05 01:26:16.311248 paystackease-1.0.0/paystackease/async_apis/asettlements.py
+-rwxr-xr-x   0        0        0     6346 2024-04-05 01:26:16.312246 paystackease-1.0.0/paystackease/async_apis/asubaccounts.py
+-rwxr-xr-x   0        0        0     4406 2024-04-05 01:26:16.313248 paystackease-1.0.0/paystackease/async_apis/asubscriptions.py
+-rwxr-xr-x   0        0        0     5400 2024-04-05 01:26:16.314248 paystackease-1.0.0/paystackease/async_apis/aterminal.py
+-rwxr-xr-x   0        0        0     5863 2024-04-05 01:26:16.315248 paystackease-1.0.0/paystackease/async_apis/atransaction_splits.py
+-rwxr-xr-x   0        0        0    12717 2024-04-05 01:26:16.316249 paystackease-1.0.0/paystackease/async_apis/atransactions.py
+-rwxr-xr-x   0        0        0     5329 2024-04-05 01:26:16.318246 paystackease-1.0.0/paystackease/async_apis/atransfer_recipients.py
+-rwxr-xr-x   0        0        0     4870 2024-04-05 01:26:16.319247 paystackease-1.0.0/paystackease/async_apis/atransfers.py
+-rwxr-xr-x   0        0        0     2699 2024-04-05 01:26:16.320247 paystackease-1.0.0/paystackease/async_apis/atransfers_control.py
+-rwxr-xr-x   0        0        0     2854 2024-04-05 09:23:13.351851 paystackease-1.0.0/paystackease/async_apis/averification.py
+-rwxr-xr-x   0        0        0      544 2024-04-05 08:20:03.235653 paystackease-1.0.0/paystackease/errors.py
+-rwxr-xr-x   0        0        0      582 2024-04-05 08:20:03.238175 paystackease-1.0.0/paystackease/helpers/__init__.py
+-rwxr-xr-x   0        0        0      768 2024-04-03 01:47:46.289946 paystackease-1.0.0/paystackease/helpers/convert.py
+-rwxr-xr-x   0        0        0     3756 2024-04-04 20:07:23.519543 paystackease-1.0.0/paystackease/helpers/tool_kit.py
+-rwxr-xr-x   0        0        0     3079 2024-03-19 18:44:47.645434 paystackease-1.0.0/paystackease/paystack.py
+-rwxr-xr-x   0        0        0     2012 2024-04-05 08:18:54.694176 paystackease-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6133 1970-01-01 00:00:00.000000 paystackease-1.0.0/PKG-INFO
```

### Comparing `paystackease-0.1.3/LICENSE` & `paystackease-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paystackease-0.1.3/README.md` & `paystackease-1.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-# PayStackEase Library  ![paystackease](docs/images/paystackease.png)
+# PayStackEase Library  
+
+------
+
+![Python Versions](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue) ![License](https://img.shields.io/pypi/l/paystackease) ![pypi](https://img.shields.io/pypi/v/paystackease.svg)
 
---------------------------------------------------------------------
 
 **PayStackEase API Library**  is a Python library that simplifies interacting with the Paystack API. 
 It provides both asynchronous and synchronous wrappers for various Paystack functionalities, 
 making it easier to integrate payment processing into your Python projects.
 
-> 📝: Read more on paystack api documentation: https://paystack.com/docs/api/
+> 📝: Read more on paystack api documentation: [Paystack API DOCUMENTATION](https://paystack.com/docs/api/)
 
-> 📝: Read more on paystackease api documentation: https://paystackease.readthedocs.io/en/latest/
+> 📝: Read more on paystackease api documentation: [PayStackEase DOCUMENTATION](https://paystackease.readthedocs.io/en/latest/)
 
 
 ## Getting Started
 
 You should create a Paystack account to generate a **Paystack Secret Key**. You can see this in the *settings page >> API keys and Webhook section*.
 
 > ⚠️: **Warning:** Do not expose your secret key or commit your secret key to git, or use them in client-side code.
@@ -55,25 +58,39 @@
 ## Install paystackease library:
 
 
 * #### Install paystackease using pip.
 
 > pip install paystackease
 
-or Download the wheel distribution file and install using pip
+* #### Install paystackease using pipx.
+
+> pipx install paystackease
+
+* #### Install paystackease using poetry.
+
+> poetry add paystackease
+
+
+## If you want to download the sdist packages directly:
+
+Download the wheel distribution file and install using pip
+
+>  pip install paystackease-1.0.0-py3-none-any.whl 
+
+Download the source distribution file, and install using pip
 
->  pip install paystackease-0.1.2-py3-none-any.whl 
+> pip install paystackease-1.0.0.tar.gz 
 
-or Download the source distribution file, and install using pip
 
-> pip install paystackease-0.1.2.tar.gz 
+## To get a development version of paystackease
 
-or clone from the github repository, unzip and install:
+Clone from the ``dev`` branch github repository, unzip and install:
 
-> git clone https://github.com/cla-bit/PayStackEase.git
+> git clone -b dev https://github.com/cla-bit/PayStackEase.git
 
 > cd PayStackEase
 
 > pip install paystackease
 
 ----------------------------------------------------------------------
 
@@ -163,8 +180,8 @@
     val1 = DocumentType.IDENTITY_NUMBER.value
     
     print(val1)
 ```
 
 > "identityNumber"
 
-Others are: ***EventType, Interval, MobileMoney, PWT, QRCODE, RecipientType, ResendOTP, Resolution, RiskAction, SplitType, STATUS, and USSD***.
+Others are: ***EventType, Interval, MobileMoney, PWT, QRCODE, RecipientType, ResendOTP, Resolution, RiskAction, SplitType, STATUS, etc***.
```

### Comparing `paystackease-0.1.3/paystackease/__init__.py` & `paystackease-1.0.0/paystackease/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,49 +7,67 @@
     TypeValueError,
     InvalidRequestMethodError
 )
 from paystackease.paystack import PayStackBase
 from paystackease.helpers import convert_to_subunit
 from paystackease.helpers import (
     AccountType,
+    Bearer,
     Currency,
     Channels,
+    DisputeStatus,
     DocumentType,
+    DVABank,
+    EFT,
+    EventAction,
     EventType,
+    GateWay,
     Interval,
     MobileMoney,
+    PayMentRequestStatus,
     PWT,
     QRCODE,
     RecipientType,
     ResendOTP,
     Resolution,
     RiskAction,
+    SettlementSchedule,
     SplitType,
     STATUS,
+    TransactionStatus,
     USSD,
 )
 
 __all__ = [
     'PayStackBase',
     'AsyncPayStackBase',
     'PayStackError',
     'SecretKeyError',
     'TypeValueError',
     'InvalidRequestMethodError',
     'convert_to_subunit',
     'AccountType',
+    'Bearer',
     'Currency',
     'Channels',
+    'DisputeStatus',
     'DocumentType',
+    'DVABank',
+    'EFT',
+    'EventAction',
     'EventType',
+    'GateWay',
     'Interval',
     'MobileMoney',
+    'PayMentRequestStatus',
     'PWT',
     'QRCODE',
     'RecipientType',
     'ResendOTP',
     'Resolution',
     'RiskAction',
+    'SettlementSchedule',
     'SplitType',
     'STATUS',
+    'TransactionStatus',
     'USSD',
 ]
```

### Comparing `paystackease-0.1.3/paystackease/_abase.py` & `paystackease-1.0.0/paystackease/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 """
-Async Base client API for Paystack API with methods for handling asynchronous AIOHTTP requests,
+Base client API for Paystack API with methods for handling HTTP requests,
 authentication using a secret key,
 constructing HTTP headers, joining URLs with the API base URL, and logging response information.
 """
 
 import json
 import logging
 
 from datetime import date, datetime
-from typing import Union
+from typing import Union, Dict, List, Any, Optional
 from urllib.parse import urljoin
 from decouple import config
 
-import aiohttp
+import requests
+from paystackease._utils import Response
 
 from paystackease.errors import (
     SecretKeyError,
     TypeValueError,
     InvalidRequestMethodError,
     PayStackError,
 )
 
 
 logger = logging.getLogger(__name__)
 
 PAYSTACK_SECRET_KEY = config("PAYSTACK_SECRET_KEY")
 
 
-class AsyncBaseClientAPI:
+class BaseClientAPI:
     """Base Client API for Paystack API"""
 
-    _PAYSTACK_API_URL = "https://api.paystack.co/"
-    _VALID_HTTP_METHODS = {"GET", "POST", "PUT", "DELETE"}
+    _PAYSTACK_API_URL: str = "https://api.paystack.co/"
+    _VALID_HTTP_METHODS: set[str] = {"GET", "POST", "PUT", "DELETE"}
 
     # pylint: disable=too-few-public-methods
-    def __init__(self, secret_key: str = None):
+    def __init__(self, secret_key: str = None) -> None:
         self._secret_key = secret_key
 
         # Default to PAYSTACK_SECRET_KEY if not provided in the instance
         if not self._secret_key:
             self._secret_key = PAYSTACK_SECRET_KEY  # or environment variables
 
         # Raise an error if PAYSTACK_SECRET_KEY is not set in the instance or environment variables
@@ -46,31 +47,24 @@
             logger.error(
                 "Please provide a secret key or set the environment variable PAYSTACK_SECRET_KEY"
             )
             raise SecretKeyError(
                 "Please provide a secret key or set the environment variable PAYSTACK_SECRET_KEY"
             )
 
-        self._session = aiohttp.ClientSession(
-            headers=self._make_paystack_http_headers()
-        )
-
-    async def __aenter__(self):
-        return self
+        self._session = requests.Session()
 
-    async def __aexit__(self, exc_type, exc, tb):
-        if not self._session.closed:
-            await self._session.close()
+        self._headers = self._make_paystack_http_headers()
 
     @classmethod
     def _set_secret_key(cls, secret_key: str) -> None:
         """Set the secret key for all instances of this class"""
         cls._secret_key = secret_key
 
-    def _join_url(self, path) -> str:
+    def _join_url(self, path: str) -> str:
         """
         Join URL with Paystack API URL
         :param path:
         :return:
         """
         if path.startswith("/"):
             path = path[1:]
@@ -83,55 +77,64 @@
         """
         return {
             "Authorization": f"Bearer {self._secret_key}",
             "content-type": "application/json",
         }
 
     @staticmethod
-    def _convert_to_string(value: Union[bool, date, datetime, None]) -> Union[str, int, None]:
+    def _convert_to_string(
+        value: Union[bool, date, datetime, None]
+    ) -> Union[str, int, None]:
         """
         Convert the type of value to a string
         :param value: The value to be converted
 
         :raise TypeError: if the value is not a supported type
 
         :return: The value as a string
         :rtype: str
         """
         # each supported type is mapped to its corresponding conversion function
         conversion_functions = {
-            bool: lambda val: str(val).lower(),
+            bool: lambda val: str(val),
             date: lambda val: val.strftime("%Y-%m-%d"),
             datetime: lambda val: val.strftime("%Y-%m-%d %H:%M:%S"),  # Added a datetime
         }
 
         if value is None:
             return None
         if type(value) in conversion_functions:
             return conversion_functions[type(value)](value)
-        logger.error("Unsupported type: %s Expected type -bool, -date, -datetime", {type(value)})
+        logger.error(
+            "Unsupported type: %s Expected type -bool, -date, -datetime", {type(value)}
+        )
         raise TypeValueError(
             f"Unsupported type: {type(value)}. Expected type -bool, -date, -datetime"
         )
 
-    async def _request_url(
-        self, method: str, url: str, data: dict = None, params: dict = None, **kwargs
-    ) -> dict:
+    def _request_url(
+        self,
+        method: str,
+        url: str,
+        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        params: Optional[Union[Dict[str, Any], None]] = None,
+        **kwargs,
+    ) -> Response:
         """
         Handles the request to Paystack API
         :param method:
         :param url:
         :param data:
         :param params:
         :param kwargs:
         :return:
         """
         if method.upper() not in self._VALID_HTTP_METHODS:
             logger.error(
-                "Invalid HTTP method. Supported methods are GET, POST, PUT, DELETE. : %s",
+                "Invalid HTTP method. Supported methods are GET, POST, PUT, DELETE : %s",
                 {method},
             )
             raise InvalidRequestMethodError(
                 f"Invalid HTTP method. Supported methods are GET, POST, PUT, DELETE. : {method}"
             )
 
         url = self._join_url(url)
@@ -139,81 +142,105 @@
         params = (
             {key: value for key, value in params.items() if value is not None}
             if params
             else None
         )
         data = json.dumps(data) if data else None
         try:
-            async with self._session.request(
-                method, url=url, data=data, params=params, **kwargs
+            with self._session.request(
+                method,
+                url=url,
+                headers=self._headers,
+                data=data,
+                params=params,
+                **kwargs,
+                timeout=30,
             ) as response:
-                response_json = await response.json()
-                logger.info("Response Status Code: %s", response.status)
-                logger.info("Response JSON: %s", response_json)
-                return response_json
-        except aiohttp.ClientError as error:
-            logger.error("Error: %s", error)
-            raise PayStackError(str(error)) from error
+                logger.info("Response Status Code: %s", response.status_code)
+                logger.info("Response JSON: %s", response.json())
+                return response.json()
+        except requests.RequestException as error:
+            # Extract status code if available from the exception
+            status_code = getattr(error, "response", None) and getattr(
+                error.response, "status_code", None
+            )
+            logger.error("Error %s", error)
+            raise PayStackError(
+                f"Error making request to Paystack API: {str(error)}", status_code
+            ) from error
 
 
-class AsyncPayStackBaseClientAPI(AsyncBaseClientAPI):
+class PayStackBaseClientAPI(BaseClientAPI):
     """Requests methods to Paystack API"""
 
-    async def _request(
+    def _request(
         self,
         method: str,
         endpoint: str,
-        data: dict = None,
-        params: dict = None,
+        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        params: Optional[Union[Dict[str, Any], None]] = None,
         **kwargs,
-    ) -> dict:
+    ) -> Response:
         """
         Handles the request to Paystack API
         :param method:
         :param endpoint:
         :param data:
         :param params:
         :param kwargs:
         :return:
         """
-        return await self._request_url(
-            method, endpoint, data=data, params=params, **kwargs
-        )
+        return self._request_url(method, endpoint, data=data, params=params, **kwargs)
 
-    async def _get_request(self, endpoint: str, params: dict = None, **kwargs) -> dict:
+    def _get_request(
+        self,
+        endpoint: str,
+        params: Optional[Union[Dict[str, Any], None]] = None,
+        **kwargs,
+    ) -> Response:
         """
         Makes the GET request to Paystack API
         :param endpoint:
         :param params:
         :param kwargs:
         :return:
         """
-        return await self._request("GET", endpoint, params=params, **kwargs)
+        return self._request("GET", endpoint, params=params, **kwargs)
 
-    async def _post_request(self, endpoint: str, data: dict = None, **kwargs) -> dict:
+    def _post_request(
+        self,
+        endpoint: str,
+        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        **kwargs,
+    ) -> Response:
         """
         Makes the POST request to Paystack API
         :param endpoint:
         :param data:
         :param kwargs:
         :return:
         """
-        return await self._request("POST", endpoint, data=data, **kwargs)
+        return self._request("POST", endpoint, data=data, **kwargs)
 
-    async def _put_request(self, endpoint: str, data: dict = None, **kwargs) -> dict:
+    def _put_request(
+        self,
+        endpoint: str,
+        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        **kwargs,
+    ) -> Response:
         """
         Makes the PUT request to Paystack API
         :param endpoint:
         :param data:
         :param kwargs:
         :return:
         """
-        return await self._request("PUT", endpoint, data=data, **kwargs)
+        return self._request("PUT", endpoint, data=data, **kwargs)
 
-    async def _delete_request(self, endpoint: str, **kwargs) -> dict:
+    def _delete_request(self, endpoint: str, **kwargs) -> Response:
         """
         Makes the DELETE request to Paystack API
         :param endpoint:
         :param kwargs:
         :return:
         """
-        return await self._request("DELETE", endpoint, **kwargs)
+        return self._request("DELETE", endpoint, **kwargs)
```

### Comparing `paystackease-0.1.3/paystackease/apaystack.py` & `paystackease-1.0.0/paystackease/apaystack.py`

 * *Files identical despite different names*

### Comparing `paystackease-0.1.3/paystackease/apis/__init__.py` & `paystackease-1.0.0/paystackease/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `paystackease-0.1.3/paystackease/apis/apple_pay.py` & `paystackease-1.0.0/paystackease/apis/apple_pay.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 """
 Wrapper class for Paystack Apple Pay API.
 
 The Apple Pay API allows you register your application's top-level domain or subdomain.
 """
 
-from typing import Optional
+from typing import Optional, Union
+
 from paystackease._base import PayStackBaseClientAPI
+from paystackease._utils import Response
 
 
 class ApplePayClientAPI(PayStackBaseClientAPI):
     """
     Paystack Apple Pay API
     Reference: https://paystack.com/docs/api/apple-pay/
     """
 
-    def register_domain(self, domain_name: str) -> dict:
+    def register_domain(self, domain_name: str) -> Response:
         """
         Register a domain or subdomain for Apple Pay
 
         :param: domain_name  # domain name or subdomain
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "domainName": domain_name,
         }
         return self._post_request("/apple-pay/domain", data=data)
 
     def list_domains(
             self,
-            use_cursor: Optional[bool] = False,
-            next_page: Optional[int] = None,
-            previous_page: Optional[int] = None,
-    ) -> dict:
+            use_cursor: Optional[Union[bool, None]] = False,
+            next_page: Optional[Union[int, None]] = None,
+            previous_page: Optional[Union[int, None]] = None,
+    ) -> Response:
         """
         List all registered domains
 
         :param: use_cursor  # use cursor for pagination
         :param: next_page  # next page
         :param: previous_page  # previous page
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert bool to string
         use_cursor = self._convert_to_string(use_cursor)
 
         params = {
             "use_cursor": use_cursor,
             "next": next_page,
             "previous": previous_page,
         }
         return self._get_request("/apple-pay/domain", params=params)
 
-    def unregister_domain(self, domain_name: str) -> dict:
+    def unregister_domain(self, domain_name: str) -> Response:
         """
         Unregister a domain or subdomain for Apple Pay
 
         :param: domain_name  # domain name or subdomain
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "domainName": domain_name,
         }
         return self._delete_request("/apple-pay/domain", data=data)
```

### Comparing `paystackease-0.1.3/paystackease/apis/bulk_charges.py` & `paystackease-1.0.0/paystackease/async_apis/abulk_charges.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,98 @@
-""" Wrapper for Paystack Bulk Charges API.
+"""
+Wrapper for Asynchronous Paystack Bulk Charges API.
 
 The Bulk Charges API allows you to create and manage multiple recurring payments from your customers.
 """
 
 from datetime import date
 
-from typing import List, Dict, Optional
-from paystackease._base import PayStackBaseClientAPI
+from typing import List, Dict, Optional, Any, Union
+from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import STATUS
 
 
-class BulkChargesClientAPI(PayStackBaseClientAPI):
+class AsyncBulkChargesClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Bulk Charges API
     Reference: https://paystack.com/docs/api/bulk-charge/
     """
 
-    def initiate_bulk_charge(self, objects: List[Dict[str, str]] = None) -> dict:
+    async def initiate_bulk_charge(self, objects: List[Dict[str, Any]]) -> Response:
         """
         Send an array of objects with authorization codes and amount
 
         :param: objects
 
         note::
 
             A list of dictionary with authorization codes, amount and reference as keys
             [{"authorization_code": "123456", "amount": 1000, "reference": "123456" }]
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._post_request("/bulkcharge", data=objects)
+        return await self._post_request("/bulkcharge", data=objects)
 
-    def list_bulk_charge_batches(
+    async def list_bulk_charge_batches(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all bulk charges
 
         :param: per_page
         :param: page
         :param: from_date
         :param: to_date
 
         note::
 
             Date Time format: 2016-09-24T00:00:05.000Z, 2016-09-21
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # Convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
-        return self._get_request("/bulkcharge", params=params)
+        return await self._get_request("/bulkcharge", params=params)
 
-    def fetch_bulk_charge_batch(self, id_or_code: str) -> dict:
+    async def fetch_bulk_charge_batch(self, id_or_code: str) -> Response:
         """
         Fetch a bulk charge of a specific batch
 
         :param: id_or_code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._get_request(f"/bulkcharge/{id_or_code}")
+        return await self._get_request(f"/bulkcharge/{id_or_code}")
 
-    def fetch_charge_bulk_batch(
+    async def fetch_charge_bulk_batch(
             self,
             id_or_code: str,
-            status: Optional[str] = None,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            status: Optional[Union[STATUS, None]] = None,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         Fetch a bulk charge of a specific batch
 
         :param: id_or_code
         :param: status:  {STATUS.value.value}
         :param: per_page
         :param: page
@@ -98,44 +101,44 @@
 
         note::
 
             Date Time format: 2016-09-24T00:00:05.000Z, 2016-09-21
             status: STATUS.value.value
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # Convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
             "status": status,
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
-        return self._get_request(f"/bulkcharge/{id_or_code}/charges", params=params)
+        return await self._get_request(f"/bulkcharge/{id_or_code}/charges", params=params)
 
-    def pause_bulk_charge_batch(self, batch_code: str) -> dict:
+    async def pause_bulk_charge_batch(self, batch_code: str) -> Response:
         """
         Pause a bulk charge of a specific batch
 
         :param: batch_code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._get_request(f"/bulkcharge/pause/{batch_code}")
+        return await self._get_request(f"/bulkcharge/pause/{batch_code}")
 
-    def resume_bulk_charge_batch(self, batch_code: str) -> dict:
+    async def resume_bulk_charge_batch(self, batch_code: str) -> Response:
         """
         Resume a bulk charge of a specific batch
 
         :param: batch_code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._get_request(f"/bulkcharge/resume/{batch_code}")
+        return await self._get_request(f"/bulkcharge/resume/{batch_code}")
```

### Comparing `paystackease-0.1.3/paystackease/apis/charges.py` & `paystackease-1.0.0/paystackease/apis/charges.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 """
 Wrapper for Paystack Charges API.
 
 The Charge API allows you to configure payment channel of your choice when initiating a payment.
 """
+
 from datetime import date
-from typing import Optional, Dict, Any
+from typing import Optional, Dict, Any, List, Union
 from paystackease._base import PayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import PWT
 
 
 class ChargesClientAPI(PayStackBaseClientAPI):
     """
     Paystack Charges API
     Reference: https://paystack.com/docs/api/charge/
     """
 
     def create_charge(
             self,
             email: str,
             amount: int,
-            pin: Optional[int] = None,
-            authorization_code: Optional[str] = None,
-            reference: Optional[str] = None,
-            device_id: Optional[str] = None,
-            bank: Optional[Dict[str, str]] = None,
-            bank_transfer: Optional[Dict[str, Any]] = None,
-            qr: Optional[Dict[str, str]] = None,
-            ussd: Optional[Dict[str, str]] = None,
-            mobile_money: Optional[Dict[str, str]] = None,
-            metadata: Optional[Dict[str, str]] = None,
-    ) -> dict:
+            pin: Optional[Union[int, None]] = None,
+            authorization_code: Optional[Union[str, None]] = None,
+            reference: Optional[Union[str, None]] = None,
+            device_id: Optional[Union[str, None]] = None,
+            bank: Optional[Union[Dict[str, str], None]] = None,
+            bank_transfer: Optional[Union[Dict[PWT, Any], None]] = None,
+            qr: Optional[Union[Dict[str, str], None]] = None,
+            ussd: Optional[Union[Dict[str, str], None]] = None,
+            mobile_money: Optional[Union[Dict[str, str], None]] = None,
+            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
+    ) -> Response:
         """
         Create a charge
 
         :param: email
         :param: amount
         :param: bank. (Set key ass: {code, account_number})
         :param: bank_transfer. (Set key as: {account_expires_at} and value: {datetime iso format})
@@ -58,15 +61,15 @@
 
             Send with a non-reusable authorization code:
             * pin
 
             mobile_money is only available in Ghana and Kenya
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "email": email,
             "amount": amount,
             "authorization_code": authorization_code,
             "bank": bank,
             "bank_transfer": bank_transfer,
@@ -76,111 +79,111 @@
             "ussd": ussd,
             "mobile_money": mobile_money,
             "device_id": device_id,
             "metadata": metadata,
         }
         return self._post_request("/charge", data=data)
 
-    def submit_pin(self, pin: int, reference: str) -> dict:
+    def submit_pin(self, pin: int, reference: str) -> Response:
         """
         Submit a PIN for a charge
 
         :param: pin
         :param: reference
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "pin": pin,
             "reference": reference,
         }
         return self._post_request("/charge/submit_pin", data=data)
 
-    def submit_otp(self, otp: int, reference: str) -> dict:
+    def submit_otp(self, otp: int, reference: str) -> Response:
         """
         Submit OTP to complete a charge
 
         :param: otp
         :param: reference
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "otp": otp,
             "reference": reference,
         }
         return self._post_request("/charge/submit_otp", data=data)
 
-    def submit_phone(self, phone: str, reference: str) -> dict:
+    def submit_phone(self, phone: str, reference: str) -> Response:
         """
         Submit a phone number to complete a charge
 
         :param: phone
         :param: reference
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "phone": phone,
             "reference": reference,
         }
         return self._post_request("/charge/submit_phone", data=data)
 
-    def submit_birthday(self, birthday: date, reference: str) -> dict:
+    def submit_birthday(self, birthday: date, reference: str) -> Response:
         """
         Submit birthday when required
 
         :param: birthday
         :param: reference
 
         note::
 
             Birthday submitted by user e.g. 2016-09-21
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         birthday = self._convert_to_string(birthday)
 
         data = {
             "birthday": birthday,
             "reference": reference,
         }
         return self._post_request("/charge/submit_birthday", data=data)
 
     def submit_address(
             self, reference: str, address: str, city: str, state: str, zipcode: str
-    ) -> dict:
+    ) -> Response:
         """
         Submit address to continue a charge
 
         :param: reference
         :param: address
         :param: city
         :param: state
         :param: zipcode
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "reference": reference,
             "address": address,
             "city": city,
             "state": state,
             "zip_code": zipcode,
         }
         return self._post_request("/charge/submit_address", data=data)
 
-    def check_pending_charge(self, reference: str) -> dict:
+    def check_pending_charge(self, reference: str) -> Response:
         """
         Check pending charge
 
         :param: reference
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request(f"/charge/{reference}")
```

### Comparing `paystackease-0.1.3/paystackease/apis/customers.py` & `paystackease-1.0.0/paystackease/async_apis/acustomers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 """
-Wrapper for Paystack Customers API.
+Wrapper for Asynchronous Paystack Customers API.
 
 The Customers API allows you to create and manage customers on your integration.
 """
 
 from datetime import date
 
-from typing import Optional, Dict, Any
-from paystackease._base import PayStackBaseClientAPI
+from typing import Optional, Dict, Any, Union
+from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import RiskAction
 
 
-class CustomerClientAPI(PayStackBaseClientAPI):
+class AsyncCustomerClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Customer API
     Reference: https://paystack.com/docs/api/customer/
     """
 
-    def create_customer(
-            self, 
-            email: str, 
-            first_name: str, 
-            last_name: str, 
-            phone: str, 
-            metadata: Optional[Dict[str, Any]] = None
-    ) -> dict:
+    async def create_customer(
+            self,
+            email: str,
+            first_name: str,
+            last_name: str,
+            phone: str,
+            metadata: Optional[Union[Dict[str, Any], None]] = None
+    ) -> Response:
         """
         Create a customer
 
         :param: email: The email associated with the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: phone: The phone number of the customer.
         :param: metadata: The metadata of the customer in JSON format.
-                            (Set key as: {"custom_fields": [{ "label": "First Name", "value": "John" }] })
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "email": email,
             "first_name": first_name,
             "last_name": last_name,
             "phone": phone,
             "metadata": metadata,
         }
-        return self._post_request("/customer", data=data)
+        return await self._post_request("/customer", data=data)
 
-    def validate_customer(
+    async def validate_customer(
             self,
             email_or_code: str,
             first_name: str,
             last_name: str,
             account_type: str,
             country: str,
             bank_code: str,
             account_number: str,
             bvn: str,
-            customer_id_num: Optional[str] = None,
-            middle_name: Optional[str] = None
-    ) -> dict:
+            customer_id_num: Optional[Union[str, None]] = None,
+            middle_name: Optional[Union[str, None]] = None
+    ) -> Response:
         """
         Validate a customer's identity
 
         :param: email_or_code: The email or code of the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: middle_name: The middle name of the customer.
@@ -70,113 +71,116 @@
         :param: customer_id_num: The customer identification number
         :param: country: The country of the customer. 2-letter country code of identification issuer
         :param: bvn: The Bank Verification Number
         :param: bank_code: The bank code of the customer
         :param: account_number: The account number of the customer
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "first_name": first_name,
             "last_name": last_name,
             "middle_name": middle_name,
             "type": account_type,
             "value": customer_id_num,
             "country": country,
             "bvn": bvn,
             "bank_code": bank_code,
             "account_number": account_number,
         }
-        return self._post_request(f"customer/{email_or_code}/identification", data=data)
+        return await self._post_request(f"customer/{email_or_code}/identification", data=data)
 
-    def whitelist_blacklist_customer(
-            self, email_or_code: str, risk_action: Optional[str] = None
-    ) -> dict:
+    async def whitelist_blacklist_customer(
+            self, email_or_code: str, risk_action: Optional[Union[RiskAction, None]] = None
+    ) -> Response:
         """
         Whitelist or blacklist a customer
 
         :param: email_or_code: The code or email of the customer.
         :param: risk_action: The action to take on the customer. value: RiskAction.value.value = "allow" pr "deny"
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        data = {"customer": email_or_code, "risk_action": risk_action}
-        return self._post_request("/customer/set_risk_action", data=data)
+        data = {
+            "customer": email_or_code,
+            "risk_action": risk_action
+        }
+        return await self._post_request("/customer/set_risk_action", data=data)
 
-    def deactivate_authorization(self, authorization_code: str) -> dict:
+    async def deactivate_authorization(self, authorization_code: str) -> Response:
         """
         Deactivate an authorization when the card needs to be forgotten
 
         :param: authorization_code: The authorization code to be deactivated.
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"authorization_code": authorization_code}
-        return self._post_request("/customer/deactivate_authorization", data=data)
+        return await self._post_request("/customer/deactivate_authorization", data=data)
 
-    def update_customer(
+    async def update_customer(
             self,
             customer_code: str,
-            first_name: Optional[str] = None,
-            last_name: Optional[str] = None,
-            phone: Optional[str] = None,
-            metadata: Optional[Dict[str, Any]] = None
-    ) -> dict:
+            first_name: Optional[Union[str, None]] = None,
+            last_name: Optional[Union[str, None]] = None,
+            phone: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, Any], None]] = None
+    ) -> Response:
         """
         Update a customer
 
         :param: customer_code: The code of the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: phone: The phone number of the customer.
         :param: metadata: The metadata of the customer in JSON format. {"key1": "value1", "key2": "value2"}
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "first_name": first_name,
             "last_name": last_name,
             "phone": phone,
             "metadata": metadata,
         }
-        return self._put_request(f"/customer/{customer_code}", data=data)
+        return await self._put_request(f"/customer/{customer_code}", data=data)
 
-    def fetch_customer(self, email_or_code: str) -> dict:
+    async def fetch_customer(self, email_or_code: str) -> Response:
         """
         Fetch details of a specific customer
 
         :param: email_or_code: The email or code of the customer.
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._get_request(f"/customer/{email_or_code}")
+        return await self._get_request(f"/customer/{email_or_code}")
 
-    def list_customers(
+    async def list_customers(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all customers
 
         :param: per_page: The number of records to return.
         :param: page: The page number to return.
         :param: from_date: The date to start returning customers from
         :param: to_date: The date to stop returning customers from
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date  to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return self._get_request("/customer", params=params)
+        return await self._get_request("/customer", params=params)
```

### Comparing `paystackease-0.1.3/paystackease/apis/dedicated_virtual_accounts.py` & `paystackease-1.0.0/paystackease/async_apis/adedicated_virtual_accounts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 """
-Wrapper for Paystack Dedicated Virtual Account API
+Wrapper for Asynchronous Paystack Dedicated Virtual Account API
 
 The Dedicated Virtual Account API enables Nigerian merchants to manage unique payment accounts of their customers.
 """
 
 from datetime import date
-from typing import Optional
-from paystackease._base import PayStackBaseClientAPI
+from typing import Optional, Union
+from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import Currency
 
 
-class DedicatedVirtualAccountClientAPI(PayStackBaseClientAPI):
+class AsyncDedicatedVirtualAccountClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Dedicated Virtual Account API
     Reference: https://paystack.com/docs/api/dedicated-virtual-account/
 
     note::
         Ensure Dedicated NUBAN is available for your business. Contact Paystack Support
     """
 
-    def create_virtual_account(
+    async def create_virtual_account(
             self,
             customer_id_or_code: str,
-            preferred_bank: Optional[str] = None,
-            subaccount: Optional[str] = None,
-            split_code: Optional[str] = None,
-            first_name: Optional[str] = None,
-            last_name: Optional[str] = None,
-            phone: Optional[str] = None,
-    ) -> dict:
+            preferred_bank: Optional[Union[str, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            first_name: Optional[Union[str, None]] = None,
+            last_name: Optional[Union[str, None]] = None,
+            phone: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Create a dedicated virtual account for existing customers.
         Currently, support Wema Bank and Titan Paystack.
 
         :param: customer_id_or_code: The customer's ID or Code
         :param: preferred_bank: Preferred bank slug for the virtual account. Eg: "wema-bank"
 
@@ -42,41 +44,41 @@
         :param: subaccount: Subaccount code of the account you want to split the transaction.
         :param: split_code: Split code
         :param: first_name: First name of the customer
         :param: last_name: Last name of the customer
         :param: phone: Phone number of the customer
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "customer": customer_id_or_code,
             "preferred_bank": preferred_bank,
             "subaccount": subaccount,
             "split_code": split_code,
             "first_name": first_name,
             "last_name": last_name,
             "phone": phone,
         }
-        return self._post_request("/dedicated_account", data=data)
+        return await self._post_request("/dedicated_account", data=data)
 
-    def assign_dedicated_virtual_account(
+    async def assign_dedicated_virtual_account(
             self,
             email: str,
             first_name: str,
             last_name: str,
             phone: str,
             preferred_bank: str,
             country: str,
-            account_number: Optional[str] = None,
-            bvn: Optional[str] = None,
-            bank_code: Optional[str] = None,
-            subaccount: Optional[str] = None,
-            split_code: Optional[str] = None,
-    ) -> dict:
+            account_number: Optional[Union[str, None]] = None,
+            bvn: Optional[Union[str, None]] = None,
+            bank_code: Optional[Union[str, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         create a customer, validate the customer, and assign a DVA to the customer
 
         :param: email: The email associated with the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: phone: The phone number of the customer.
@@ -95,150 +97,153 @@
         :param: account_number: The account number of the customer
         :param: bvn: The Bank Verification Number
         :param: bank_code: The bank code of the customer
         :param: subaccount: Subaccount code of the account you want to split the transaction.
         :param: split_code: Split code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "email": email,
             "first_name": first_name,
             "last_name": last_name,
             "phone": phone,
             "preferred_bank": preferred_bank,
             "country": country,
             "account_number": account_number,
             "bvn": bvn,
             "bank_code": bank_code,
             "subaccount": subaccount,
             "split_code": split_code,
         }
-        return self._post_request("/dedicated_account", data=data)
+        return await self._post_request("/dedicated_account", data=data)
 
-    def list_dedicated_account(
+    async def list_dedicated_account(
             self,
-            active: Optional[bool] = True,
-            currency: Optional[str] = None,
-            provider_slug: Optional[str] = None,
-            bank_id: Optional[str] = None,
-            customer_id: Optional[str] = None,
-    ) -> dict:
+            active: Optional[Union[bool, None]] = True,
+            currency: Optional[Union[Currency, None]] = None,
+            provider_slug: Optional[Union[str, None]] = None,
+            bank_id: Optional[Union[str, None]] = None,
+            customer_id: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         List dedicated accounts
 
         :param: active: Shows the status of the dedicated virtual account
         :param: currency: Currency of the dedicated virtual account
         :param: provider_slug: Provider slug in lowercase eg: wema-bank
         :param: bank_id: Bank ID of the dedicated virtual account eg: 035
         :param: customer_id: Customer ID of the dedicated virtual account
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
+        # convert date to string
+        active = self._convert_to_string(active)
+
         params = {
             "active": active,
             "currency": currency,
             "provider_slug": provider_slug,
             "bank_id": bank_id,
             "customer": customer_id,
         }
-        return self._get_request("/dedicated_account", params=params)
+        return await self._get_request("/dedicated_account", params=params)
 
-    def fetch_dedicated_account(self, dedicated_account_id: int) -> dict:
+    async def fetch_dedicated_account(self, dedicated_account_id: int) -> Response:
         """
         Get details of a dedicated virtual account
 
         :param: dedicated_account_id: Dedicated account ID
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._get_request(f"/dedicated_account/{dedicated_account_id}")
+        return await self._get_request(f"/dedicated_account/{dedicated_account_id}")
 
-    def requery_dedicated_account(
+    async def requery_dedicated_account(
             self,
-            account_number: Optional[str] = None,
-            provider_slug: Optional[str] = None,
-            date_transfer: Optional[date] = None,
-    ) -> dict:
+            account_number: Optional[Union[str, None]] = None,
+            provider_slug: Optional[Union[str, None]] = None,
+            date_transfer: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         Requery a dedicated virtual account for new transactions
 
         :param: account_number: Virtual Account number to requery
         :param: provider_slug: Provider slug in lowercase eg: wema-bank
         :param: date_transfer: Date of when the transfer was made
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         date_transfer = self._convert_to_string(date_transfer)
 
         params = {
             "account_number": account_number,
             "provider_slug": provider_slug,
             "date": date_transfer,
         }
-        return self._get_request("/dedicated_account/requery", params=params)
+        return await self._get_request("/dedicated_account/requery", params=params)
 
-    def deactivate_dedicated_account(self, dedicated_account_id: int) -> dict:
+    async def deactivate_dedicated_account(self, dedicated_account_id: int) -> Response:
         """
         Deactivate a dedicated virtual account
 
         :param: dedicated_account_id: Dedicated account ID
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._delete_request(f"/dedicated_account/{dedicated_account_id}")
+        return await self._delete_request(f"/dedicated_account/{dedicated_account_id}")
 
-    def split_dedicated_account(
+    async def split_dedicated_account(
             self,
             customer_id_or_code: str,
-            subaccount: Optional[str] = None,
-            split_code: Optional[str] = None,
-            preferred_bank: Optional[str] = None,
-    ) -> dict:
+            subaccount: Optional[Union[str, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            preferred_bank: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Split a dedicated virtual account transaction with one or more accounts
 
         :param: customer_id_or_code: Customer's ID or Code
         :param: subaccount: Subaccount code of the account you want to split the transaction
         :param: split_code: Split code
         :param: preferred_bank: Preferred bank for the virtual account
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "customer": customer_id_or_code,
             "preferred_bank": preferred_bank,
             "subaccount": subaccount,
             "split_code": split_code,
         }
-        return self._post_request("/dedicated_account/split", data=data)
+        return await self._post_request("/dedicated_account/split", data=data)
 
-    def remove_split_dedicated_account(self, account_number: str) -> dict:
+    async def remove_split_dedicated_account(self, account_number: str) -> Response:
         """
         Remove a split dedicated virtual account
 
         :param: account_number: the account number of the dedicated virtual account
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "account_number": account_number,
         }
-        return self._delete_request("/dedicated_account/split", data=data)
+        return await self._delete_request("/dedicated_account/split", data=data)
 
-    def fetch_bank_providers(self) -> dict:
+    async def fetch_bank_providers(self) -> Response:
         """
         Fetch bank providers
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._get_request("/dedicated_account/available_providers")
+        return await self._get_request("/dedicated_account/available_providers")
```

### Comparing `paystackease-0.1.3/paystackease/apis/disputes.py` & `paystackease-1.0.0/paystackease/apis/disputes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 """
 Wrapper for Paystack Disputes API
 
 The Disputes API allows you manage transaction disputes on your integration.
 """
 
 from datetime import date
-from typing import Optional
+from typing import Optional, Union
 from paystackease._base import PayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import DisputeStatus, Resolution
 
 
 class DisputesClientAPI(PayStackBaseClientAPI):
     """
     Paystack Disputes API
     Reference: https://paystack.com/docs/api/dispute/
     """
 
     def list_disputes(
             self,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            transaction_id: Optional[str] = None,
-            status: Optional[str] = None,
-    ) -> dict:
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            transaction_id: Optional[Union[str, None]] = None,
+            status: Optional[Union[DisputeStatus, None]] = None,
+    ) -> Response:
         """
         List disputes filed against you
 
         :param: from_date: A timestamp from which to start listing dispute e.g. 2016-09-21
         :param: to_date: A timestamp from which to start listing dispute e.g. 2016-09-21
         :param: per_page:
         :param: page:
         :param: transaction_id:
         :param: status: Dispute Status. Acceptable values:
                         { awaiting-merchant-feedback | awaiting-bank-feedback | pending | resolved }
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
@@ -49,79 +51,79 @@
             "from": from_date,
             "to": to_date,
             "transaction": transaction_id,
             "status": status,
         }
         return self._get_request("/dispute", params=params)
 
-    def fetch_dispute(self, dispute_id: str) -> dict:
+    def fetch_dispute(self, dispute_id: str) -> Response:
         """
         Fetch details about a dispute
 
         :param: dispute_id: The dispute ID to fetch
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request(f"/dispute/{dispute_id}")
 
-    def list_transaction_disputes(self, transaction_id: str) -> dict:
+    def list_transaction_disputes(self, transaction_id: str) -> Response:
         """
         List disputes for a transaction
 
         :param: transaction_id: The transaction id to fetch
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request(f"/dispute/transaction/{transaction_id}")
 
     def update_dispute(
             self,
             dispute_id: str,
             refund_amount: int,
-            uploaded_filename: Optional[str] = None,
-    ) -> dict:
+            uploaded_filename: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Update details of a dispute
 
         :param: dispute_id: The dispute id to fetch
         :param: refund_amount: The amount to refund to the customer
         :param: uploaded_filename: filename of attachment returned via
                                     response from upload url(GET /dispute/:id/upload_url)
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"refund_amount": refund_amount, "uploaded_filename": uploaded_filename}
         return self._put_request(f"/dispute/{dispute_id}", data=data)
 
     def add_evidence(
             self,
             dispute_id: str,
             customer_email: str,
             customer_name: str,
             customer_phone: str,
             service_details: str,
-            delivery_address: Optional[str] = None,
-            delivery_date: Optional[date] = None,
-    ) -> dict:
+            delivery_address: Optional[Union[str, None]] = None,
+            delivery_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         Add evidence to a dispute
 
         :param: dispute_id: The dispute id to fetch
         :param: customer_email: The customer email
         :param: customer_name: The customer name
         :param: customer_phone: The customer phone
         :param: service_details: The service details
         :param: delivery_address: The delivery address
         :param: delivery_date: The delivery date: YYYY-MM-DD
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         delivery_date = self._convert_to_string(delivery_date)
 
         data = {
             "customer_email": customer_email,
@@ -129,80 +131,80 @@
             "customer_phone": customer_phone,
             "service_details": service_details,
             "delivery_address": delivery_address,
             "delivery_date": delivery_date,
         }
         return self._post_request(f"/dispute/{dispute_id}/evidence", data=data)
 
-    def get_upload_url(self, dispute_id: str, uploaded_filename: str) -> dict:
+    def get_upload_url(self, dispute_id: str, uploaded_filename: str) -> Response:
         """
         Get upload url for dispute evidence
 
         :param: dispute_id: The dispute id to fetch
         :param: uploaded_filename: The file name, with its extension, that you want to upload. e.g. filename.pdf
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         params = {"uploaded_filename": uploaded_filename}
         return self._get_request(f"/dispute/{dispute_id}/upload_url", params=params)
 
     def resolve_dispute(
             self,
             dispute_id: str,
-            resolution: str,
+            resolution: Resolution,
             message: str,
             refund_amount: int,
             uploaded_filename: str,
-            evidence: Optional[int] = None,
-    ) -> dict:
+            evidence: Optional[Union[int, None]] = None,
+    ) -> Response:
         """
         Resolve a dispute
 
         :param: dispute_id: The dispute id to fetch
         :param: resolution: The resolution to resolve the dispute: Accepted values: { merchant-accepted | declined }.
         :param: message: The message for resolution
         :param: refund_amount: The amount to refund to the customer
         :param: uploaded_filename: filename of attachment returned via response from method get_upload_url
         :param: evidence: The evidence id for fraud claims
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "resolution": resolution,
             "message": message,
             "refund_amount": refund_amount,
             "uploaded_filename": uploaded_filename,
             "evidence": evidence,
         }
         return self._put_request(f"/dispute/{dispute_id}/resolve", data=data)
 
     def export_disputes(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-            transaction_id: Optional[str] = None,
-            status: Optional[str] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+            transaction_id: Optional[Union[str, None]] = None,
+            status: Optional[Union[DisputeStatus, None]] = None,
+    ) -> Response:
         """
         Export disputes
 
         :param: per_page:
         :param: page:
         :param: from_date: The start date to fetch disputes from
         :param: to_date: The end date to fetch disputes from
         :param: transaction_id: The transaction ID
         :param: status: The dispute status:
                         Acceptable values: { awaiting-merchant-feedback | awaiting-bank-feedback | pending | resolved }
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
```

### Comparing `paystackease-0.1.3/paystackease/apis/integration.py` & `paystackease-1.0.0/paystackease/apis/integration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
 Wrapper for Paystack Integration API
 
 The Integration API allows you manage some settings on your integration.
 """
-
+from paystackease._utils import Response
 from paystackease._base import PayStackBaseClientAPI
 
 
 class IntegrationClientAPI(PayStackBaseClientAPI):
     """
     Paystack Integration API
     Reference: https://paystack.com/docs/api/integration/
     """
 
-    def fetch_timeout(self) -> dict:
+    def fetch_timeout(self) -> Response:
         """
         Fetch payment session timeout
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request("/integration/payment_session_timeout")
 
-    def update_timeout(self, timeout: int) -> dict:
+    def update_timeout(self, timeout: int) -> Response:
         """
         Update payment session timeout
 
         :param: timeout: The new payment session timeout before session
         
         note::
 
             timeout is in seconds. Set 0 to cancel the timeout
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         data = {"timeout": timeout}
         return self._put_request("/integration/payment_session_timeout", data=data)
```

### Comparing `paystackease-0.1.3/paystackease/apis/miscellaneous.py` & `paystackease-1.0.0/paystackease/apis/miscellaneous.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 """
 Wrapper for Paystack Miscellaneous API.
 
 The Miscellaneous API are supporting APIs that can be used to provide more details to other APIs.
 """
 
-from typing import Optional
+from typing import Optional, Union
 from paystackease._base import PayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import GateWay, Channels, Currency
 
 
 class MiscellaneousClientAPI(PayStackBaseClientAPI):
     """
     Paystack Miscellaneous API
     Reference: https://paystack.com/docs/api/miscellaneous/
     """
 
     def list_banks(
             self,
-            country: Optional[str] = None,
-            use_cursor: Optional[bool] = False,
-            per_page: Optional[int] = None,
-            pay_with_bank_transfer: Optional[bool] = None,
-            pay_with_bank: Optional[bool] = None,
-            enabled_for_verification: Optional[bool] = None,
-            next_cursor: Optional[str] = None,
-            previous_cursor: Optional[str] = None,
-            gateway: Optional[str] = None,
-            channel_type: Optional[str] = None,
-            currency: Optional[str] = None,
-    ) -> dict:
+            country: Optional[Union[str, None]] = None,
+            use_cursor: Optional[Union[bool, None]] = False,
+            per_page: Optional[Union[int, None]] = 50,
+            pay_with_bank_transfer: Optional[Union[bool, None]] = False,
+            pay_with_bank: Optional[Union[bool, None]] = False,
+            enabled_for_verification: Optional[Union[bool, None]] = False,
+            next_cursor: Optional[Union[str, None]] = None,
+            previous_cursor: Optional[Union[str, None]] = None,
+            gateway: Optional[Union[GateWay, None]] = None,
+            channel_type: Optional[Union[Channels, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+    ) -> Response:
         """
         Get a list of all supported banks and their properties
 
         :param: country: The country to obtain the list of supported banks.
                         Values { country=ghana or country=nigeria }
         :param: use_cursor: Use cursor to paginate through the list of supported banks
         :param: per_page: The number of records to return per page: 10, 20 or 50
@@ -47,16 +49,22 @@
         :param: channel_type: Type of financial channel. { Channels.value.value}
 
         **note::**
 
         For Ghanaian channels, please use either mobile_money for mobile money channels OR ghipps for bank channels
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
+        # convert to strings
+        use_cursor = self._convert_to_string(use_cursor)
+        pay_with_bank_transfer = self._convert_to_string(pay_with_bank_transfer)
+        pay_with_bank = self._convert_to_string(pay_with_bank)
+        enabled_for_verification = self._convert_to_string(enabled_for_verification)
+
         params = {
             "country": country,
             "use_cursor": use_cursor,
             "perPage": per_page,
             "supports_transfer": pay_with_bank_transfer,
             "pay_with_bank": pay_with_bank,
             "enabled_for_verification": enabled_for_verification,
@@ -64,27 +72,27 @@
             "previous": previous_cursor,
             "gateway": gateway,
             "type": channel_type,
             "currency": currency,
         }
         return self._get_request("/bank", params=params)
 
-    def list_countries(self) -> dict:
+    def list_countries(self) -> Response:
         """
         Get a list of all supported countries and their properties
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request("/country")
 
-    def list_states(self, country: str) -> dict:
+    def list_states(self, country: str) -> Response:
         """
         Get a list of all supported states and their properties
 
         :param: country: The country code from which to obtain the list of supported states
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         params = {"country": country}
         return self._get_request("/address_verification/states", params=params)
```

### Comparing `paystackease-0.1.3/paystackease/apis/payment_pages.py` & `paystackease-1.0.0/paystackease/async_apis/apayment_pages.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,156 +1,157 @@
 """
-Wrapper for Paystack Payment Pages API.
+Wrapper for Asynchronous Paystack Payment Pages API.
 
 The Payment Pages API provides a quick and secure way to collect payment for products.
 """
 
 from datetime import date
-from typing import Optional, Dict, List
-from paystackease._base import PayStackBaseClientAPI
+from typing import Optional, Dict, List, Any, Union
+from paystackease._utils import Response
+from paystackease._abase import AsyncPayStackBaseClientAPI
 
 
-class PaymentPagesClientAPI(PayStackBaseClientAPI):
+class AsyncPaymentPagesClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Payment Pages API
     Reference: https://paystack.com/docs/api/page/
     """
 
-    def create_payment_page(
+    async def create_payment_page(
             self,
             name: str,
-            description: Optional[str] = None,
-            amount: Optional[int] = None,
-            split_code: Optional[str] = None,
-            page_slug: Optional[str] = None,
-            redirect_url: Optional[str] = None,
-            metadata: Optional[Dict[str, str]] = None,
-            custom_fields: Optional[List[str]] = None,
-    ) -> dict:
+            description: Optional[Union[str, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            page_slug: Optional[Union[str, None]] = None,
+            redirect_url: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, Any], None]] = None,
+            custom_fields: Optional[Union[List[Dict[str, Any]], None]] = None,
+    ) -> Response:
         """
         Create a payment page
 
         :param: name: Name of the page
         :param: description: Description of the page
         :param: amount: Amount of the page
         :param: split_code: Split code of the transaction split
         :param: page_slug: URL slug you would like to be associated with this page.
-        
+
         note::
 
             Page will be accessible at https://paystack.com/pay/page_slug
 
         :param: redirect_url: If you would like Paystack to redirect someplace
                                 upon successful payment, specify the URL here.
         :param: metadata: Extra data to configure the payment page including subaccount,logo image, transaction charge
         :param: custom_fields: If you would like to accept custom fields, specify them here.
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "name": name,
             "description": description,
             "amount": amount,
             "split_code": split_code,
             "slug": page_slug,
             "redirect_url": redirect_url,
             "metadata": metadata,
             "custom_fields": custom_fields,
         }
-        return self._post_request("/page", data=data)
+        return await self._post_request("/page", data=data)
 
-    def list_payment_pages(
+    async def list_payment_pages(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all the payment pages
 
         :param: per_page: Number of records to return
         :param: page: number to return
         :param: from_date: A timestamp from which to start listing page
         :param: to_date: A timestamp from which to start listing page
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
 
         note::
             Date Time value is in this format: 2016-09-24T00:00:05.000Z, 2016-09-21
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return self._get_request("/page", params=params)
+        return await self._get_request("/page", params=params)
 
-    def fetch_payment_page(self, page_id_or_slug: str) -> dict:
+    async def fetch_payment_page(self, page_id_or_slug: str) -> Response:
         """
         Get details of a payment page
 
         :param: page_id_or_slug: ID or slug of the payment page
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._get_request(f"/page/{page_id_or_slug}")
+        return await self._get_request(f"/page/{page_id_or_slug}")
 
-    def update_payment_page(
+    async def update_payment_page(
             self,
             page_id_or_slug: str,
-            name: Optional[str] = None,
-            description: Optional[str] = None,
-            amount: Optional[int] = None,
-            active: Optional[bool] = None,
-    ) -> dict:
+            name: Optional[Union[str, None]] = None,
+            description: Optional[Union[str, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            active: Optional[Union[bool, None]] = True,
+    ) -> Response:
         """
         Update a payment page detail
 
         :param: page_id_or_slug: ID or slug of the payment page
         :param: name: Name of the page
         :param: description: Description of the page
         :param: amount: Amount of the page
         :param: active: Set false to deactivate the page url
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert bool to string
         active = self._convert_to_string(active)
 
         data = {
             "name": name,
             "description": description,
             "amount": amount,
             "active": active,
         }
-        return self._put_request(f"/page/{page_id_or_slug}", data=data)
+        return await self._put_request(f"/page/{page_id_or_slug}", data=data)
 
-    def check_slug_available(self, page_slug: str) -> dict:
+    async def check_slug_available(self, page_slug: str) -> Response:
         """
         Check if a slug is available
 
         :param: page_slug: URL slug you would like to be associated with this page.
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._get_request(f"/page/check_slug_availability/{page_slug}")
+        return await self._get_request(f"/page/check_slug_availability/{page_slug}")
 
-    def add_products(self, payment_id: int, product: List[int]) -> dict:
+    async def add_products(self, payment_id: int, product: List[int]) -> Response:
         """
         Add products to a payment page
 
         :param: payment_id: ID of the payment page
         :param: product: List of IDS of all the products
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"product": product}
-        return self._post_request(f"/page/{payment_id}/product", data=data)
+        return await self._post_request(f"/page/{payment_id}/product", data=data)
```

### Comparing `paystackease-0.1.3/paystackease/apis/payment_requests.py` & `paystackease-1.0.0/paystackease/apis/payment_requests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Wrapper for Paystack Payment Requests API.
 
 The Payment Requests API allows you manage requests for payment of goods and services.
 """
 
 from datetime import date
-from typing import Optional, List, Dict
+from typing import Optional, List, Dict, Any, Union
+from paystackease._utils import Response
 from paystackease._base import PayStackBaseClientAPI
+from paystackease.helpers.tool_kit import PayMentRequestStatus, Currency
 
 
 class PaymentRequestClientAPI(PayStackBaseClientAPI):
     """
     Paystack Payment Request API
     Reference: https://paystack.com/docs/api/payment-request/
     """
@@ -18,22 +20,22 @@
     def create_payment_request(
             self,
             customer: str,
             amount: int,
             draft: bool,
             has_invoice: bool,
             send_notification: bool,
-            due_date: Optional[date] = None,
-            description: Optional[str] = None,
-            line_items: Optional[List[Dict[str, str]]] = None,
-            tax: Optional[List[Dict[str, str]]] = None,
-            currency: Optional[str] = None,
-            invoice_number: Optional[int] = None,
-            split_code: Optional[str] = None,
-    ) -> dict:
+            due_date: Optional[Union[date, None]] = None,
+            description: Optional[Union[str, Any]] = None,
+            line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
+            tax: Optional[Union[List[Dict[str, Any]], None]] = None,
+            currency: Optional[Union[Currency, Any]] = None,
+            invoice_number: Optional[Union[int, Any]] = None,
+            split_code: Optional[Union[str, Any]] = None,
+    ) -> Response:
         """
         Create a payment request for a transaction
 
         :param: customer: Customer ID of the customer
         :param: amount: Amount of the payment request
         :param: due_date: Due date of the payment request
         :param: description: Description of the payment request
@@ -43,18 +45,21 @@
         :param: send_notification: Set true if you want to send a notification to the customer email
         :param: draft: Set true if you want to create a draft payment request
         :param: has_invoice: Set true if you want to create a draft payment request
         :param: invoice_number: Invoice number of the payment request
         :param: split_code: split code of the transaction split
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         # convert date and bool to string
         due_date = self._convert_to_string(due_date)
+        draft = self._convert_to_string(draft)
+        has_invoice = self._convert_to_string(has_invoice)
+        send_notification = self._convert_to_string(send_notification)
 
         data = {
             "customer": customer,
             "amount": amount,
             "due_date": due_date,
             "description": description,
             "line_items": line_items,
@@ -66,125 +71,129 @@
             "invoice_number": invoice_number,
             "split_code": split_code,
         }
         return self._post_request("/paymentrequest", data=data)
 
     def list_payment_requests(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            customer: Optional[str] = None,
-            status: Optional[str] = None,
-            currency: Optional[str] = None,
-            include_archive: Optional[str] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[str, None]] = None,
+            status: Optional[Union[PayMentRequestStatus, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            include_archive: Optional[Union[bool, None]] = True,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all the payment requests
 
         :param: per_page: Number of records to return
         :param: page:  number to return
         :param: customer: Filter by customer ID
         :param: status: Filter by payment request status
         :param: currency:
         :param: include_archive: Show archived payment requests
         :param: from_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
         :param: to_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
+        include_archive = self._convert_to_string(include_archive)
 
         params = {
             "perPage": per_page,
             "page": page,
             "customer": customer,
             "status": status,
             "currency": currency,
             "include_archive": include_archive,
             "from": from_date,
             "to": to_date,
         }
         return self._get_request("/paymentrequest", params=params)
 
-    def fetch_payment_request(self, id_or_code: str) -> dict:
+    def fetch_payment_request(self, id_or_code: str) -> Response:
         """
         Get details of a payment request on your integration
 
         :param: id_or_code: ID or Code of the payment request
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request(f"/paymentrequest/{id_or_code}")
 
-    def verify_payment_request(self, code: str) -> dict:
+    def verify_payment_request(self, code: str) -> Response:
         """
         Verify details of a payment request on your integration
 
         :param: code: Payment request code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request(f"/paymentrequest/verify/{code}")
 
-    def send_notification(self, code: str) -> dict:
+    def send_notification(self, code: str) -> Response:
         """
         Send notification of a payment request to a customer
 
         :param: code: Payment request code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._post_request(f"/paymentrequest/notify/{code}")
 
-    def payment_request_total(self) -> dict:
+    def payment_request_total(self) -> Response:
         """
         Get total of a payment request metric
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request("/paymentrequest/totals")
 
-    def finalize_payment_request(self, code: str, send_notification: bool) -> dict:
+    def finalize_payment_request(self, code: str, send_notification: bool) -> Response:
         """
         Finalize a draft payment request
 
         :param: code: Payment request code
         :param: send_notification: Set true if you want to send a notification to the customer email
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
+        # convert to strings
+        send_notification = self._convert_to_string(send_notification)
+
         data = {"send_notification": send_notification}
         return self._post_request(f"/paymentrequest/finalize/{code}", data=data)
 
     def update_payment_request(
             self,
             id_or_code: str,
-            customer: Optional[str] = None,
-            amount: Optional[int] = None,
-            description: Optional[str] = None,
-            line_items: Optional[List[Dict[str, str]]] = None,
-            tax: Optional[List[Dict[str, str]]] = None,
-            currency: Optional[str] = None,
-            due_date: Optional[date] = None,
-            send_notification: Optional[bool] = None,
-            draft: Optional[bool] = None,
-            invoice_number: Optional[int] = None,
-            split_code: Optional[str] = None,
-    ) -> dict:
+            customer: Optional[Union[str, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            description: Optional[Union[str, None]] = None,
+            line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
+            tax: Optional[Union[List[Dict[str, Any]], None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            due_date: Optional[Union[date, None]] = None,
+            send_notification: Optional[Union[bool, None]] = True,
+            draft: Optional[Union[bool, None]] = True,
+            invoice_number: Optional[Union[int, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Update a payment request
 
         :param: id_or_code: ID or Code of the payment request
         :param: customer: Customer ID or code of the customer
         :param: amount: Amount of the payment request
         :param: due_date: Due date of the payment request
@@ -194,19 +203,21 @@
         :param: currency: Currency of the payment request
         :param: send_notification: Set true if you want to send a notification to the customer email
         :param: draft: Set true if you want to create a draft payment request
         :param: invoice_number: Invoice number of the payment request starts from 1 and autoincrement
         :param: split_code: split code of the transaction split
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date and bool to string
         due_date = self._convert_to_string(due_date)
+        draft = self._convert_to_string(draft)
+        send_notification = self._convert_to_string(send_notification)
 
         data = {
             "customer": customer,
             "amount": amount,
             "due_date": due_date,
             "description": description,
             "line_items": line_items,
@@ -215,17 +226,17 @@
             "send_notification": send_notification,
             "draft": draft,
             "invoice_number": invoice_number,
             "split_code": split_code,
         }
         return self._put_request(f"/paymentrequest/{id_or_code}", data=data)
 
-    def archive_payment_request(self, code: str) -> dict:
+    def archive_payment_request(self, code: str) -> Response:
         """
         Archive a payment request
 
         :param: code: Payment request code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._post_request(f"/paymentrequest/archive/{code}")
```

### Comparing `paystackease-0.1.3/paystackease/apis/plans.py` & `paystackease-1.0.0/paystackease/async_apis/aplans.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,134 +1,143 @@
 """
-Wrapper for Paystack Plans API
+Wrapper for Asynchronous Paystack Plans API
 
 The Plans API allows you to create and manage installment payment options on your integration.
 """
 
-from typing import Optional
-from paystackease._base import PayStackBaseClientAPI
+from typing import Optional, Union
+from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import Interval
 
 
-class PlanClientAPI(PayStackBaseClientAPI):
+class AsyncPlanClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Plan API
     Reference: https://paystack.com/docs/api/plan/
     """
 
-    def create_plan(
+    async def create_plan(
             self,
             name: str,
             amount: int,
-            interval: str,
+            interval: Interval,
             currency: str,
             invoice_limit: int,
             send_invoices: bool,
             send_sms: bool,
-            description: Optional[str] = None,
-    ) -> dict:
+            description: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Create a plan
 
         :param: name: Name of the plan
         :param: amount: Amount of the plan
         :param: interval: Interval of the plan. Values [Interval.value.value]
         :param: description: Description of the plan
         :param: send_invoices: Send invoices to customer
         :param: send_sms: Send SMS to customer
         :param: currency: Currency of the plan
         :param: invoice_limit: Invoice limit of the plan
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
+        # convert to strings
+        send_invoices = self._convert_to_string(send_invoices)
+        send_sms = self._convert_to_string(send_sms)
+
         data = {
             "name": name,
             "amount": amount,
             "interval": interval,
             "description": description,
             "send_invoices": send_invoices,
             "send_sms": send_sms,
             "currency": currency,
             "invoice_limit": invoice_limit,
         }
-        return self._post_request("/plan", data=data)
+        return await self._post_request("/plan", data=data)
 
-    def list_plans(
+    async def list_plans(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            status: Optional[str] = None,
-            interval: Optional[str] = None,
-            amount: Optional[int] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            status: Optional[Union[str, None]] = None,
+            interval: Optional[Union[Interval, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+    ) -> Response:
         """
         List all the plans
 
         :param: per_page: Number of records to return
         :param: page:  number to return
         :param: status: Filter list by plans with specified status
         :param: interval: Filter list by plans with specified interval
         :param: amount
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         params = {
             "perPage": per_page,
             "page": page,
             "status": status,
             "interval": interval,
             "amount": amount,
         }
-        return self._get_request("/plan", params=params)
+        return await self._get_request("/plan", params=params)
 
-    def fetch_plan(self, id_or_code: str) -> dict:
+    async def fetch_plan(self, id_or_code: str) -> Response:
         """
         Get details of a plan
 
         :param: id_or_code: ID or Code of the plan
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._get_request(f"/plan/{id_or_code}")
+        return await self._get_request(f"/plan/{id_or_code}")
 
-    def update_plan(
+    async def update_plan(
             self,
             id_or_code: str,
             name: str,
             amount: int,
-            interval: str,
+            interval: Interval,
             send_invoices: bool,
             send_sms: bool,
             currency: str,
             invoice_limit: int,
-            description: Optional[str] = None,
-    ) -> dict:
+            description: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Update a plan detail
 
         :param: id_or_code: ID or Code of the plan
         :param: name: Name of the plan
         :param: amount: Amount of the plan
         :param: interval: Interval of the plan. [Interval.value.value]
         :param: description:
         :param: send_invoices:
         :param: send_sms:
         :param: currency:
         :param: invoice_limit:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
+        # convert to strings
+        send_invoices = self._convert_to_string(send_invoices)
+        send_sms = self._convert_to_string(send_sms)
 
         data = {
             "name": name,
             "amount": amount,
             "interval": interval,
             "description": description,
             "send_invoices": send_invoices,
             "send_sms": send_sms,
             "currency": currency,
             "invoice_limit": invoice_limit,
         }
-        return self._put_request(f"/plan/{id_or_code}", data=data)
+        return await self._put_request(f"/plan/{id_or_code}", data=data)
```

### Comparing `paystackease-0.1.3/paystackease/apis/products.py` & `paystackease-1.0.0/paystackease/apis/products.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Wrapper for Paystack Products API
 
 The Products API allows you to create and manage inventories on your integration.
 """
 
 from datetime import date
-from typing import Optional
+from typing import Optional, Union
+from paystackease._utils import Response
 from paystackease._base import PayStackBaseClientAPI
 
 
 class ProductClientAPI(PayStackBaseClientAPI):
     """
     Paystack Product API
     Reference: https://paystack.com/docs/api/product/
@@ -17,29 +18,29 @@
 
     def create_product(
             self,
             name: str,
             description: str,
             amount: int,
             currency: str,
-            unlimited: Optional[bool] = None,
-            quantity: Optional[int] = None,
-    ) -> dict:
+            unlimited: Optional[Union[bool, None]] = True,
+            quantity: Optional[Union[int, None]] = None,
+    ) -> Response:
         """
         Create a product
 
         :param: name: Name of the product
         :param: description: Description of the product
         :param: amount: Price of the product
         :param: currency: Currency of the product
         :param: unlimited: Set true if the product has unlimited stock,
         :param: quantity: Quantity of the product in stock Use if unlimited is false
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert bool to string
         unlimited = self._convert_to_string(unlimited)
 
         data = {
             "name": name,
@@ -49,72 +50,72 @@
             "unlimited": unlimited,
             "quantity": quantity,
         }
         return self._post_request("/product", data=data)
 
     def list_products(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all the products
 
         :param: per_page: Number of records to return
         :param: page:  number to return
         :param: from_date: A timestamp from which to start listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
         :param: to_date: A timestamp from which to start listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to strings
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
         return self._get_request("/product", params=params)
 
-    def fetch_product(self, product_id: str) -> dict:
+    def fetch_product(self, product_id: str) -> Response:
         """
         Get details of a product
 
         :param: product_id: ID or Code of the product
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request(f"/product/{product_id}")
 
     def update_product(
             self,
             product_id: str,
             name: str,
             description: str,
             amount: int,
             currency: str,
-            unlimited: Optional[bool] = None,
-            quantity: Optional[int] = None,
-    ) -> dict:
+            unlimited: Optional[Union[bool, None]] = True,
+            quantity: Optional[Union[int, None]] = None,
+    ) -> Response:
         """
         Update a product detail
 
         :param: product_id: ID or Code of the product
         :param: name: Name of the product
         :param: description: Description of the product
         :param: amount: Price of the product
         :param: currency: Currency of the product
         :param: unlimited: Set true if the product has unlimited stock,
         :param: quantity: Quantity of the product in stock Use if unlimited is false
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert bool to string
         unlimited = self._convert_to_string(unlimited)
 
         data = {
             "name": name,
```

### Comparing `paystackease-0.1.3/paystackease/apis/refund.py` & `paystackease-1.0.0/paystackease/apis/refund.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,76 @@
 """
 Wrapper for Paystack Refund API
 
 The Refunds API allows you to create and manage transaction refunds.
 """
 
 from datetime import date
-from typing import Optional
+from typing import Optional, Union
+from paystackease._utils import Response
 from paystackease._base import PayStackBaseClientAPI
+from paystackease.helpers.tool_kit import Currency
 
 
 class RefundClientAPI(PayStackBaseClientAPI):
     """
     Paystack Refund API
     Reference: https://paystack.com/docs/api/refund/
     """
 
     def create_refund(
             self,
             transaction_ref_or_id: str,
-            amount: Optional[int] = None,
-            currency: Optional[str] = None,
-            customer_note: Optional[str] = None,
-            merchant_note: Optional[str] = None,
-    ) -> dict:
+            amount: Optional[Union[int, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            customer_note: Optional[Union[str, None]] = None,
+            merchant_note: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Create a refund
 
         :param: transaction_ref_or_id: The transaction id or reference to fetch
         :param: amount: The amount to refund
         :param: currency: The currency to refund { Currency.value.value }
         :param: customer_note: The customer note or reason
         :param: merchant_note: The merchant note or reason
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "transaction": transaction_ref_or_id,
             "amount": amount,
             "currency": currency,
             "customer_note": customer_note,
             "merchant_note": merchant_note,
         }
         return self._post_request("/refund", data=data)
 
     def list_refunds(
             self,
-            reference: Optional[str] = None,
-            currency: Optional[str] = None,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            reference: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List refunds
 
         :param: reference: The transaction reference to fetch for the refund
         :param: currency: The currency to refund
         :param: per_page
         :param: page
         :param: from_date: A timestamp at which to stop listing refund
         :param: to_date: A timestamp at which to stop listing refund
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
 
         note::
 
             Date time format: 2016-09-21
         """
 
         # convert date to string
@@ -81,17 +83,17 @@
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
         return self._get_request("/refund", params=params)
 
-    def fetch_refund(self, reference: str) -> dict:
+    def fetch_refund(self, reference: str) -> Response:
         """
         Fetch a refund
 
         :param: reference: The transaction reference to fetch for the refund
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request(f"/refund/{reference}")
```

### Comparing `paystackease-0.1.3/paystackease/apis/settlements.py` & `paystackease-1.0.0/paystackease/apis/settlements.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 """
 Wrapper for Paystack Settlements API
 
 The Settlements API allows you to gain insights into payouts made by Paystack to your bank account.
 """
 
 from datetime import date
-from typing import Optional
+from typing import Optional, Union
+from paystackease._utils import Response
 from paystackease._base import PayStackBaseClientAPI
+from paystackease.helpers.tool_kit import STATUS
 
 
 class SettlementClientAPI(PayStackBaseClientAPI):
     """
     Paystack Settlement API
     Reference: https://paystack.com/docs/api/settlement/
     """
 
     def list_settlements(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            status: Optional[str] = None,
-            subaccount: Optional[str] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            status: Optional[Union[STATUS, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List settlements made to your settlement accounts
 
         :param: per_page: The number of records to return per page.
         :param: page: the number to retrieve.
         :param: status: Value can be one of success, processing, pending or failed.
         :param: subaccount:
         :param: from_date: A timestamp from which to start listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
         :param: to_date: A timestamp from which to start listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
@@ -51,30 +53,30 @@
             "to": to_date,
         }
         return self._get_request("/settlement", params=params)
 
     def list_settlement_transactions(
             self,
             settlement_id: int,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         Get the transactions that make up a particular settlement
 
         :param: settlement_id: The id of the settlement.
         :param: per_page: The number of records to return per page.
         :param: page: the number to retrieve.
         :param: from_date: A timestamp from which to start listing settlements
         :param: to_date: A timestamp from which to start listing settlements
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         
         note::
 
             Date and time format: 2016-09-24T00:00:05.000Z, 2016-09-21
 
         """
```

### Comparing `paystackease-0.1.3/paystackease/apis/subaccounts.py` & `paystackease-1.0.0/paystackease/async_apis/asubaccounts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,81 +1,83 @@
 """
-Wrapper for Paystack SubAccounts API
+Wrapper for Asynchronous Paystack SubAccounts API
 
 The Subaccounts API allows you to create and manage subaccounts on your integration.
 Subaccounts can be used to split payment between two accounts (your main account and a subaccount).
 """
 
 from datetime import date
-from typing import Optional, Dict, List, Any
-from paystackease._base import PayStackBaseClientAPI
+from typing import Optional, Dict, List, Any, Union
+from paystackease._utils import Response
+from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease.helpers.tool_kit import SettlementSchedule
 
 
-class SubAccountClientAPI(PayStackBaseClientAPI):
+class AsyncSubAccountClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack SubAccount API
     Reference: https://paystack.com/docs/api/subaccount/
     """
 
-    def create_subaccount(
+    async def create_subaccount(
             self,
             business_name: str,
             settlement_bank: str,
             account_number: str,
             percentage_charge: float,
             description: str,
-            primary_contact_email: Optional[str] = None,
-            primary_contact_name: Optional[str] = None,
-            primary_contact_phone: Optional[str] = None,
-            metadata: Optional[Dict[str, List[Dict[str, Any]]]] = None,
-    ) -> dict:
+            primary_contact_email: Optional[Union[str, None]] = None,
+            primary_contact_name: Optional[Union[str, None]] = None,
+            primary_contact_phone: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
+    ) -> Response:
         """
         Create a subaccount
 
         :param: business_name: The business name of the subaccount.
         :param: settlement_bank: Bank Code for the bank
         :param: account_number: The account number of the subaccount.
         :param: percentage_charge: The percentage charge receives from each payment made to the subaccount
         :param: description: The description of the subaccount.
         :param: primary_contact_email: A contact email for the subaccount
         :param: primary_contact_name: A name for the contact person for this subaccount
         :param: primary_contact_phone: A phone number to call for this subaccount
         :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "business_name": business_name,
             "settlement_bank": settlement_bank,
             "account_number": account_number,
             "percentage_charge": percentage_charge,
             "description": description,
             "primary_contact_email": primary_contact_email,
             "primary_contact_name": primary_contact_name,
             "primary_contact_phone": primary_contact_phone,
             "metadata": metadata,
         }
-        return self._post_request("/subaccount", data=data)
+        return await self._post_request("/subaccount", data=data)
 
-    def update_subaccount(
+    async def update_subaccount(
             self,
             id_or_code: str,
             business_name: str,
             settlement_bank: str,
             account_number: str,
-            active: Optional[bool] = None,
-            percentage_charge: Optional[float] = None,
-            description: Optional[str] = None,
-            primary_contact_email: Optional[str] = None,
-            primary_contact_name: Optional[str] = None,
-            primary_contact_phone: Optional[str] = None,
-            settlement_schedule: Optional[str] = None,
-            metadata: Optional[Dict[str, List[Dict[str, Any]]]] = None,
-    ) -> dict:
+            active: Optional[Union[bool, None]] = True,
+            percentage_charge: Optional[Union[float, None]] = None,
+            description: Optional[Union[str, None]] = None,
+            primary_contact_email: Optional[Union[str, None]] = None,
+            primary_contact_name: Optional[Union[str, None]] = None,
+            primary_contact_phone: Optional[Union[str, None]] = None,
+            settlement_schedule: Optional[Union[SettlementSchedule, None]] = SettlementSchedule.AUTO.value,
+            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
+    ) -> Response:
         """
         Update a subaccount
 
         :param: id_or_code: The id or code of the subaccount.
         :param: business_name: The business name of the subaccount.
         :param: settlement_bank: The settlement bank of the subaccount.
         :param: account_number
@@ -85,20 +87,20 @@
         :param: primary_contact_email
         :param: primary_contact_name
         :param: primary_contact_phone
         :param: settlement_schedule: Values: [ auto, weekly, `monthly`, `manual` ].
 
         note::
             Auto means payout is T+1
-            Manual means payout to the subaccount should only be made when requested. Defaults to auto
+            Manual means payout to the subaccount should only be made when requested. async defaults to auto
 
         :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert bool to string
         active = self._convert_to_string(active)
 
         data = {
             "business_name": business_name,
@@ -109,45 +111,45 @@
             "description": description,
             "primary_contact_email": primary_contact_email,
             "primary_contact_name": primary_contact_name,
             "primary_contact_phone": primary_contact_phone,
             "settlement_schedule": settlement_schedule,
             "metadata": metadata,
         }
-        return self._put_request(f"/subaccount/{id_or_code}", data=data)
+        return await self._put_request(f"/subaccount/{id_or_code}", data=data)
 
-    def list_subaccounts(
+    async def list_subaccounts(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all subaccounts
 
         :param: per_page: The number of records to return per page.
         :param: page: The number to retrieve.
         :param: from_date:
         :param: to_date:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return self._get_request("/subaccount", params=params)
+        return await self._get_request("/subaccount", params=params)
 
-    def fetch_subaccount(self, id_or_code: str) -> dict:
+    async def fetch_subaccount(self, id_or_code: str) -> Response:
         """
         Fetch details of a specific subaccount
 
         :param: id_or_code: The id or code of the subaccount.
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._get_request(f"/subaccount/{id_or_code}")
+        return await self._get_request(f"/subaccount/{id_or_code}")
```

### Comparing `paystackease-0.1.3/paystackease/apis/subscriptions.py` & `paystackease-1.0.0/paystackease/apis/subscriptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 """
 Wrapper for Paystack Subscriptions API
 
 The Subscriptions API allows you to create and manage recurring payment on your integration.
 """
 
 from datetime import date
-from typing import Optional
+from typing import Optional, Union
+from paystackease._utils import Response
 from paystackease._base import PayStackBaseClientAPI
 
 
 class SubscriptionClientAPI(PayStackBaseClientAPI):
     """
     Paystack Subscription API
     Reference: https://paystack.com/docs/api/subscription/
     """
 
     def create_subscription(
             self,
             customer: str,
             plan_code: str,
             authorization: str,
-            start_date: Optional[date] = None,
-    ) -> dict:
+            start_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         Create a subscription
 
         :param: customer: Email or Code of the customer
         :param: plan_code: Code of the plan
         :param: authorization: Code of the authorization
         :param: start_date: Start date of the subscription
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         start_date = self._convert_to_string(start_date)
 
         data = {
             "customer": customer,
@@ -43,89 +44,89 @@
             "authorization": authorization,
             "start_date": start_date,
         }
         return self._post_request("/subscription", data=data)
 
     def list_subscriptions(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            customer: Optional[int] = None,
-            plan_code: Optional[int] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[int, None]] = None,
+            plan_code: Optional[Union[int, None]] = None,
+    ) -> Response:
         """
         List all the subscriptions
 
         :param: per_page: Number of records to return per page.
         :param: page: THe number to return
         :param: customer:
         :param: plan_code:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         params = {
             "perPage": per_page,
             "page": page,
             "customer": customer,
             "plan": plan_code,
         }
         return self._get_request("/subscription", params=params)
 
-    def fetch_subscription(self, id_or_code: str) -> dict:
+    def fetch_subscription(self, id_or_code: str) -> Response:
         """
         Get details of a subscription
 
         :param: id_or_code: ID or Code of the subscription
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request(f"/subscription/{id_or_code}")
 
-    def enable_subscription(self, subscription_code: str, token: str) -> dict:
+    def enable_subscription(self, subscription_code: str, token: str) -> Response:
         """
         Enable a subscription
 
         :param: subscription_code: Code of the subscription
         :param: token: Email token of the customer
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"code": subscription_code, "token": token}
         return self._post_request("/subscription/enable", data=data)
 
-    def disable_subscription(self, subscription_code: str, token: str) -> dict:
+    def disable_subscription(self, subscription_code: str, token: str) -> Response:
         """
         Disable a subscription
 
         :param: subscription_code: Code of the subscription
         :param: token: Email token of the customer
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"code": subscription_code, "token": token}
         return self._post_request("/subscription/disable", data=data)
 
-    def generate_update_subscription(self, subscription_code: str) -> dict:
+    def generate_update_subscription(self, subscription_code: str) -> Response:
         """
         Generate a link for updating the card on subscription
 
         :param: subscription_code: Code of the subscription
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._post_request(f"/subscription/{subscription_code}/manage/link")
 
-    def send_update_subscription_link(self, subscription_code: str) -> dict:
+    def send_update_subscription_link(self, subscription_code: str) -> Response:
         """
         Email a customer a link for updating the card on their subscription
 
         :param: subscription_code: Code of the subscription
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._post_request(f"/subscription/{subscription_code}/manage/email")
```

### Comparing `paystackease-0.1.3/paystackease/apis/terminal.py` & `paystackease-1.0.0/paystackease/apis/terminal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,133 +1,139 @@
 """
 Wrapper for Paystack Terminal APIs
 
 The Terminal API allows you to build delightful in-person payment experiences.
 """
 
-from typing import Optional, Dict
+from typing import Optional, Dict, Union
+from paystackease._utils import Response
 from paystackease._base import PayStackBaseClientAPI
+from paystackease.helpers.tool_kit import EventAction, EventType
 
 
 class TerminalClientAPI(PayStackBaseClientAPI):
     """
     Paystack Terminal API
     Reference: https://paystack.com/docs/api/terminal/
     """
 
     def send_event(
             self,
             terminal_id: str,
-            event_type: str,
-            terminal_action: str,
+            event_type: EventType,
+            terminal_action: EventAction,
             data_object: Dict[str, str],
-    ) -> dict:
+    ) -> Response:
         """
         Send an event from your application to the Paystack Terminal
 
         :param: terminal_id: The terminal iD the event is sent to
         :param: event_type: The type of event to send. We currently support [ invoice | transaction ]
         :param: terminal_action: The action to perform on the terminal
                                     [invoice type]:the action can either be [ process || view ]
                                     [transaction type], the action can either be [ process || print ].
         :param: data_object: parameters needed to perform the specified action.
                             [invoice type]: you need to pass {id: invoice_id, reference: offline_reference}.
                             [transaction type], you can pass {id: transaction_id}
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"type": event_type, "action": terminal_action, "data": data_object}
         return self._post_request(f"/terminal/{terminal_id}/event", data=data)
 
-    def commission_terminal(self, serial_number: str) -> dict:
+    def commission_terminal(self, serial_number: str) -> Response:
         """
         Activate debug device by linking it to your integration
 
         :param: serial_number: The serial number of the device
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"serial_number": serial_number}
         return self._post_request("/terminal/commission_device", data=data)
 
-    def decommission_terminal(self, serial_number: str) -> dict:
+    def decommission_terminal(self, serial_number: str) -> Response:
         """
         Deactivate debug device by unlinking it from your integration
 
         :param: serial_number: The serial number of the device
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"serial_number": serial_number}
         return self._post_request("/terminal/decommission_device", data=data)
 
     def update_terminal(
             self, terminal_id: str, terminal_name: str, terminal_address: str
-    ) -> dict:
+    ) -> Response:
         """
         Update details of a terminal
 
         :param: terminal_id: The terminal iD the event is sent to
         :param: terminal_name: Name of the terminal
         :param: terminal_address: Address of the terminal
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"name": terminal_name, "address": terminal_address}
         return self._put_request(f"/terminal/{terminal_id}", data=data)
 
-    def fetch_event_status(self, terminal_id: str, event_id: str) -> dict:
+    def fetch_event_status(self, terminal_id: str, event_id: str) -> Response:
         """
         Fetch details of a specific event status sent to the terminal
 
         :param: terminal_id: iD of the terminal the event is sent to
         :param: event_id: The event id sent to the terminal
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request(f"/terminal/{terminal_id}/event/{event_id}")
 
-    def fetch_terminal_status(self, terminal_id: str) -> dict:
+    def fetch_terminal_status(self, terminal_id: str) -> Response:
         """
         Fetch the availability of a terminal before sending an event
 
         :param: terminal_id: The terminal iD the event is sent to
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request(f"/terminal/{terminal_id}/presence")
 
     def list_terminals(
             self,
-            per_page: int,
-            next_cursor: Optional[str] = None,
-            previous_cursor: Optional[str] = None,
-    ) -> dict:
+            per_page: int = 50,
+            next_cursor: Optional[Union[bool, None]] = True,
+            previous_cursor: Optional[Union[bool, None]] = True,
+    ) -> Response:
         """
         List the Terminals available on your integration
 
         :param: per_page: The number of records to return. Default value is 50
         :param: next_cursor:
         :param: previous_cursor:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
+        # convert to strings
+        next_cursor = self._convert_to_string(next_cursor)
+        previous_cursor = self._convert_to_string(previous_cursor)
+
         params = {"perPage": per_page, "next": next_cursor, "previous": previous_cursor}
         return self._get_request("/terminal", params=params)
 
-    def fetch_terminal(self, terminal_id: str) -> dict:
+    def fetch_terminal(self, terminal_id: str) -> Response:
         """
         Get the details of a terminal
 
         :param: terminal_id: The terminal iD the event is sent to
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request(f"/terminal/timeline/{terminal_id}")
```

### Comparing `paystackease-0.1.3/paystackease/apis/transaction_splits.py` & `paystackease-1.0.0/paystackease/async_apis/atransaction_splits.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,143 +1,143 @@
 """
-Wrapper for Paystack Transaction Splits APIs
+Wrapper for Asynchronous Paystack Transaction Splits APIs
 
 The Transaction Splits API enables merchants split the settlement for a transaction
 across their payout account, and one or more subaccounts.
 """
-
 from datetime import date
-from typing import Optional, List, Dict, Any
-from paystackease._base import PayStackBaseClientAPI
+from typing import Optional, List, Dict, Any, Union
+from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
 
 
-class TransactionSplitClientAPI(PayStackBaseClientAPI):
+class AsyncTransactionSplitClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Transaction Split API
     Reference: https://paystack.com/docs/api/split/
     """
 
-    def create_split(
+    async def create_split(
             self,
             transaction_split_name: str,
             transaction_split_type: str,
             currency: str,
             subaccounts: List[Dict[str, Any]],
             bearer_type: str,
             bearer_subaccount: str,
-    ) -> dict:
+    ) -> Response:
         """
         Create a split payment on your integration
 
         :param: transaction_split_name: Name of the transaction split
         :param: transaction_split_type: The type of transaction split you want to create [ percentage | flat ]
         :param: currency: [ Currency.value.value ]
         :param: subaccounts: A list of object containing subaccount code and number of shares
                             [{subaccount: ‘ACT_xxxxxxxxxx’, share: xxx},{...}]
         :param: bearer_type: Any of subaccount | account | all-proportional | all
         :param: bearer_subaccount: Subaccount code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "name": transaction_split_name,
             "type": transaction_split_type,
             "currency": currency,
             "subaccounts": subaccounts,
             "bearer_type": bearer_type,
             "bearer_subaccount": bearer_subaccount,
         }
-        return self._post_request("/split", data=data)
+        return await self._post_request("/split", data=data)
 
-    def add_or_update_subaccount_split(
+    async def add_or_update_subaccount_split(
             self, split_id: str, subaccount: str, transaction_share: int
-    ) -> dict:
+    ) -> Response:
         """
         Add a Subaccount to a Transaction Split, or update the share of
         an existing Subaccount in a Transaction Split
 
         :param: split_id: The split ID
         :param: subaccount: The subaccount code
         :param: transaction_share: The number of shares
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"subaccount": subaccount, "share": transaction_share}
-        return self._post_request(f"/split/{split_id}/subaccount/add", data=data)
+        return await self._post_request(f"/split/{split_id}/subaccount/add", data=data)
 
-    def remove_sub_account_split(self, split_id: str, subaccount: str) -> dict:
+    async def remove_sub_account_split(self, split_id: str, subaccount: str) -> Response:
         """
         Remove a Sub Account from a transaction split
 
         :param: split_id: The split ID
         :param: subaccount: The subaccount code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"subaccount": subaccount}
-        return self._post_request(f"/split/{split_id}/subaccount/remove", data=data)
+        return await self._post_request(f"/split/{split_id}/subaccount/remove", data=data)
 
-    def update_split(
+    async def update_split(
             self,
             split_id: str,
             transaction_split_name: str,
             active: bool,
-            bearer_type: Optional[str] = None,
-            bearer_subaccount: Optional[str] = None,
-    ) -> dict:
+            bearer_type: Optional[Union[str, None]] = None,
+            bearer_subaccount: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Update a specific transaction split details
 
         :param: split_id: The split ID
         :param: transaction_split_name: Name of the transaction split
         :param: active: True or False
         :param: bearer_type:
         :param: bearer_subaccount:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert bool to string
         active = self._convert_to_string(active)
 
         data = {
             "name": transaction_split_name,
             "active": active,
             "bearer_type": bearer_type,
             "bearer_subaccount": bearer_subaccount,
         }
-        return self._put_request(f"/split/{split_id}", data=data)
+        return await self._put_request(f"/split/{split_id}", data=data)
 
-    def list_split(
+    async def list_split(
             self,
-            split_name: Optional[str] = None,
-            active: Optional[bool] = None,
-            sort_by: Optional[str] = None,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            split_name: Optional[Union[str, None]] = None,
+            active: Optional[Union[bool, None]] = True,
+            sort_by: Optional[Union[str, None]] = None,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all the transaction splits
 
         :param: split_name: Name of the transaction split
         :param: active: True or False
-        :param: sort_by: Sort by name, defaults to createdAt date,
+        :param: sort_by: Sort by name, async defaults to createdAt date,
         :param: per_page:
         :param: page:
         :param: from_date:
         :param: to_date:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date and bool to string
         active = self._convert_to_string(active)
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
@@ -146,19 +146,19 @@
             "active": active,
             "sort_by": sort_by,
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
-        return self._get_request("/split", params=params)
+        return await self._get_request("/split", params=params)
 
-    def fetch_split(self, split_id: str) -> dict:
+    async def fetch_split(self, split_id: str) -> Response:
         """
         Fetch details of a specific transaction split
 
         :param: split_id: The split ID
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._get_request(f"/split/{split_id}")
+        return await self._get_request(f"/split/{split_id}")
```

### Comparing `paystackease-0.1.3/paystackease/apis/transactions.py` & `paystackease-1.0.0/paystackease/async_apis/atransactions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 """
-Wrapper for Paystack Transactions API
+Wrapper for Asynchronous Paystack Transactions API
 
 The Transactions API allows you to create and manage payments on your integration.
 """
 
 from datetime import date
-from typing import List, Optional, Dict, Any
+from typing import List, Optional, Dict, Any, Union
+from paystackease.helpers.tool_kit import TransactionStatus, Channels, Bearer, Currency
+from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
 
-from paystackease._base import PayStackBaseClientAPI
 
-
-class TransactionClientAPI(PayStackBaseClientAPI):
+class AsyncTransactionClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Transaction API
     Reference: https://paystack.com/docs/api/transaction/
     """
 
-    def initialize(
+    async def initialize(
             self,
             email: str,
             amount: int,
-            currency: Optional[str] = None,
-            reference: Optional[str] = None,
-            callback_url: Optional[str] = None,
-            plan: Optional[str] = None,
-            invoice_limit: Optional[int] = None,
-            channels: Optional[List[str]] = None,
-            split_code: Optional[str] = None,
-            subaccount: Optional[str] = None,
-            transaction_charge: Optional[int] = None,
-            bearer: Optional[str] = None,
-            metadata: Optional[Dict[str, str]] = None,
-    ) -> dict:
+            currency: Optional[Union[Currency, None]] = Currency.NGN.value,
+            reference: Optional[Union[str, None]] = None,
+            callback_url: Optional[Union[str, None]] = None,
+            plan: Optional[Union[str, None]] = None,
+            invoice_limit: Optional[Union[int, None]] = None,
+            channels: Optional[Union[List[Channels], None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            transaction_charge: Optional[Union[int, None]] = None,
+            bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
+            metadata: Optional[Union[Dict[str, Any], None]] = None,
+    ) -> Response:
         """
         Initialize a transaction
 
         :param: email:
         :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
                         Use convert_currency() to convert to subunit
         :param: currency:  # Currency.value.value
         :param: reference:
         :param: callback_url: # Use this to override the callback url provided on the  dashboard
-                            # https://example.com/callback
-        :param: plan:  # If transaction is to create a subscription to a predefined plan, provide plan code here.
+                                # https://example.com/callback
+        :param: plan:  # If transaction is to create a subscription to a preasync defined plan, provide plan code here.
         :param: invoice_limit:  # Number of times to charge customer during subscription to plan
         :param: channels:  # [Channels.value.value, Channels.value.value, ...]
         :param: split_code:  # The split code of the transaction split. e.g. SPL_98WF13Eb3w
         :param: subaccount:  # The code for the subaccount that owns the payment. e.g. ACCT_8f4s1eq7ml6rlzj
         :param: transaction_charge: # An amount used to override the split configuration for a
                                     # single split payment
         :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
         :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "email": email,
             "amount": amount,
             "currency": currency,
             "reference": reference,
             "callback_url": callback_url,
@@ -66,30 +67,30 @@
             "channels": channels,
             "split_code": split_code,
             "subaccount": subaccount,
             "transaction_charge": transaction_charge,
             "bearer": bearer,
             "metadata": metadata,
         }
-        return self._post_request("/transaction/initialize", data=data)
+        return await self._post_request("/transaction/initialize", data=data)
 
-    def charge_authorization(
+    async def charge_authorization(
             self,
             email: str,
             amount: int,
             authorization_code: str,
-            reference: Optional[str] = None,
-            currency: Optional[str] = None,
-            channels: Optional[List[str]] = None,
-            subaccount: Optional[str] = None,
+            reference: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            channels: Optional[Union[List[Channels], None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
             transaction_charge: Optional[int] = None,
-            bearer: Optional[str] = None,
-            queue: Optional[bool] = None,
-            metadata: Optional[Dict[str, List[Dict[str, Any]]]] = None,
-    ) -> dict:
+            bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
+            queue: Optional[Union[bool, None]] = True,
+            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
+    ) -> Response:
         """
         Charge an authorization transaction
 
         :param: email:
         :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
                         Use convert_currency() to convert to subunit
         :param: authorization_code:  # value = AUTH_1234234WRFW
@@ -99,15 +100,15 @@
         :param: subaccount:  # value = ACCT_8f4s1eq7ml6rlzj
         :param: transaction_charge:
         :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
         :param: queue:  # If set to true, the transaction will be queued for processing
         :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert bool to string
         queue = self._convert_to_string(queue)
 
         data = {
             "email": email,
@@ -118,74 +119,74 @@
             "channels": channels,
             "subaccount": subaccount,
             "transaction_charge": transaction_charge,
             "bearer": bearer,
             "queue": queue,
             "metadata": metadata,
         }
-        return self._post_request("/transaction/charge_authorization", data=data)
+        return await self._post_request("/transaction/charge_authorization", data=data)
 
-    def partial_debit(
+    async def partial_debit(
             self,
             email: str,
             authorization_code: str,
             amount: int,
             currency: str,
-            reference: Optional[str] = None,
-            at_least: Optional[int] = None,
-    ) -> dict:
+            reference: Optional[Union[str, None]] = None,
+            at_least: Optional[Union[int, None]] = None,
+    ) -> Response:
         """
         Charge a partial debit transaction
 
         :param: email:
         :param: authorization_code:  # value = AUTH_1234234WRFW
         :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
                         Use convert_currency() to convert to subunit
         :param: currency:  # value = Currency.value.value
         :param: reference:  # Unique transaction reference.
         :param: at_least:  # Minimum amount to charge
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "email": email,
             "authorization_code": authorization_code,
             "amount": amount,
             "currency": currency,
             "reference": reference,
             "at_least": at_least,
         }
-        return self._post_request("/transaction/partial_debit", data=data)
+        return await self._post_request("/transaction/partial_debit", data=data)
 
-    def list_transactions(
+    async def list_transactions(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            customer: Optional[int] = None,
-            terminal_id: Optional[str] = None,
-            amount: Optional[int] = None,
-            status: Optional[str] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[int, None]] = None,
+            terminal_id: Optional[Union[str, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            status: Optional[Union[TransactionStatus, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all transactions
 
         :param: per_page:  # Specify how many records you want to retrieve per page.
         :param: page:  # Specify a page number to retrieve
         :param: customer:  # Specify an ID for the customer whose transactions you want to retrieve
         :param: terminal_id:  # Specify an ID for the terminal whose transactions you want to retrieve
         :param: amount:  # Specify an amount for the transactions you want to retrieve
         :param: status:  # Specify a status for the transactions you want to retrieve [success, failed, abandoned]
         :param: from_date:  # A timestamp from which to start listing transaction 2016-09-24T00:00:05.000Z, 2016-09-21
         :param: to_date:  # A timestamp at which to stop listing transaction 2016-09-24T00:00:05.000Z
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
@@ -194,94 +195,94 @@
             "customer": customer,
             "terminalid": terminal_id,
             "amount": amount,
             "status": status,
             "from": from_date,
             "to": to_date,
         }
-        return self._get_request("/transaction", params=params)
+        return await self._get_request("/transaction", params=params)
 
-    def verify_transaction(self, reference: str) -> dict:
+    async def verify_transaction(self, reference: str) -> Response:
         """
         Verify a transaction by reference
 
         :param: reference:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._get_request(f"/transaction/verify/{reference}")
+        return await self._get_request(f"/transaction/verify/{reference}")
 
-    def fetch_transaction(self, transaction_id: int) -> dict:
+    async def fetch_transaction(self, transaction_id: int) -> Response:
         """
         Fetch details of a specific transaction
 
         :param: transaction_id:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._get_request(f"/transaction/{transaction_id}")
+        return await self._get_request(f"/transaction/{transaction_id}")
 
-    def transaction_timeline(self, id_or_reference: str) -> dict:
+    async def transaction_timeline(self, id_or_reference: str) -> Response:
         """
         Get the timeline of a transaction
 
         :param: id_or_reference:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return self._get_request(f"/transaction/timeline/{id_or_reference}")
+        return await self._get_request(f"/transaction/timeline/{id_or_reference}")
 
-    def transaction_totals(
+    async def transaction_totals(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         Get totals of all transactions
 
         :param: per_page:
         :param: page:
         :param: from_date:
         :param: to_date:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
-        return self._get_request("/transaction/totals", params=params)
+        return await self._get_request("/transaction/totals", params=params)
 
-    def export_transactions(
+    async def export_transactions(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            customer: Optional[int] = None,
-            currency: Optional[str] = None,
-            amount: Optional[int] = None,
-            status: Optional[str] = None,
-            settled: Optional[bool] = None,
-            settlement: Optional[int] = None,
-            payment_page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[int, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            status: Optional[Union[TransactionStatus, None]] = None,
+            settled: Optional[Union[bool, None]] = True,
+            settlement: Optional[Union[int, None]] = None,
+            payment_page: Optional[Union[int, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         Export transactions
 
         :param: per_page:
         :param: page:
         :param: customer:
         :param: currency:  # value = Currency.value.value
@@ -290,15 +291,15 @@
         :param: settled:  # true or false
         :param: settlement:
         :param: payment_page:
         :param: from_date:  # 2016-09-24T00:00:05.000Z
         :param: to_date:  # 2016-09-24T00:00:05.000Z
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date and bool to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
         settled = self._convert_to_string(settled)
 
@@ -311,8 +312,8 @@
             "status": status,
             "settled": settled,
             "settlement": settlement,
             "payment_page": payment_page,
             "from": from_date,
             "to": to_date,
         }
-        return self._get_request("/transaction/export", params=params)
+        return await self._get_request("/transaction/export", params=params)
```

### Comparing `paystackease-0.1.3/paystackease/apis/transfer_recipients.py` & `paystackease-1.0.0/paystackease/apis/transfer_recipients.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,135 +1,137 @@
 """
 Wrapper for Paystack Transfer Recipient APIs
 
 The Transfer Recipients API allows you to create and manage beneficiaries that you send money to.
 """
 
 from datetime import date
-from typing import Optional, Dict, List
+from typing import Optional, Dict, List, Any, Union
 from paystackease._base import PayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import Currency
 
 
 class TransferRecipientsClientAPI(PayStackBaseClientAPI):
     """
     Paystack Transfer Recipients API
     Reference: https://paystack.com/docs/api/transfer-recipient/
     """
 
     def create_transfer_recipients(
             self,
             recipient_type: str,
             recipient_name: str,
             account_number: str,
             bank_code: str,
-            description: Optional[str] = None,
-            currency: Optional[str] = None,
-            authorization_code: Optional[str] = None,
-            metadata: Optional[Dict[str, str]] = None,
-    ) -> dict:
+            description: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            authorization_code: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, Any], None]] = None,
+    ) -> Response:
         """
         Create a transfer recipient
 
         :param: recipient_type: The type of transfer recipient:[ nuban | ghipss | mobile_money | basa ]
         :param: recipient_name: The name of the transfer recipient according to their account registration
         :param: account_number: transfer recipient's account number.
                                 Required for all recipient types except authorization
         :param: bank_code: transfer recipient's bank code. Required for all recipient types except authorization
         :param: description:
         :param: currency: transfer recipient's currency. [Currency.value.value ]
         :param: authorization_code: transfer recipient's authorization code from previous transaction
         :param: metadata: transfer recipient's metadata
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "type": recipient_type,
             "name": recipient_name,
             "account_number": account_number,
             "bank_code": bank_code,
             "description": description,
             "currency": currency,
             "authorization_code": authorization_code,
             "metadata": metadata,
         }
         return self._post_request("/transferrecipient", data=data)
 
-    def bulk_create_transfer_recipient(self, batch: List[Dict[str, str]]) -> dict:
+    def bulk_create_transfer_recipient(self, batch: List[Dict[str, Any]]) -> Response:
         """
         Create multiple transfer recipients in batches.
 
         :param: batch: A list of transfer recipient object
                         keys [ { type, name, account_number, bank_code, currency etc. }]
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"batch": batch}
         return self._post_request("/transferrecipient/bulk", data=data)
 
     def list_transfer_recipients(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List transfer recipients
 
         :param: per_page: The number of records to return per page.
         :param: page: The page number to retrieve.
         :param: from_date:
         :param: to_date:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to strings
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
         return self._get_request("/transferrecipient", params=params)
 
-    def fetch_transfer_recipient(self, id_or_code: str) -> dict:
+    def fetch_transfer_recipient(self, id_or_code: str) -> Response:
         """
         Fetch details of a transfer recipient
 
         :param: id_or_code: The id or code of the transfer recipient
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request(f"/transferrecipient/{id_or_code}")
 
     def update_transfer_recipient(
             self,
             id_or_code: str,
             recipient_name: str,
-            recipient_email: Optional[str] = None,
-    ) -> dict:
+            recipient_email: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Update a transfer recipient
 
         :param: id_or_code: The id or code of the transfer recipient
         :param: recipient_name: The name of the transfer recipient
         :param: recipient_email: The email of the transfer recipient
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"name": recipient_name, "email": recipient_email}
         return self._put_request(f"/transferrecipient/{id_or_code}", data=data)
 
-    def delete_transfer_recipient(self, id_or_code: str) -> dict:
+    def delete_transfer_recipient(self, id_or_code: str) -> Response:
         """
         Delete a transfer recipient
 
         :param: id_or_code: The id or code of the transfer recipient
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._delete_request(f"/transferrecipient/{id_or_code}")
```

### Comparing `paystackease-0.1.3/paystackease/apis/transfers.py` & `paystackease-1.0.0/paystackease/apis/transfers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,105 +1,107 @@
 """
 Wrapper for Paystack Transfers APIs
 
 The Transfers API allows you to automate sending money to your customers.
 """
 
 from datetime import date
-from typing import Optional, List, Dict
+from typing import Optional, List, Dict, Any, Union
 
 from paystackease._base import PayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import Currency
 
 
 class TransfersClientAPI(PayStackBaseClientAPI):
     """
     Paystack Transfers API
     Reference: https://paystack.com/docs/api/transfer/
     """
 
     def initiate_transfer(
             self,
             transfer_source: str,
             amount: int,
             transfer_recipient: str,
-            reason: Optional[str] = None,
-            currency: Optional[str] = None,
-            reference: Optional[str] = None,
-    ) -> dict:
+            reason: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            reference: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Initiate a transfer. Upgrade your business to a Registered Business to use
 
         :param: transfer_source: Where should we transfer from? Only balance for now
         :param: amount: Amount to transfer in kobo if currency is NGN and pesewas if currency is GHS.
         :param: transfer_recipient: The code of the recipient
         :param: currency: The currency of the transfer
         :param: reason: The reason for the transfer
         :param: reference: If specified, the field should be a unique identifier (in lowercase) for the object.
                             Only -,_ and alphanumeric characters allowed.
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "source": transfer_source,
             "amount": amount,
             "recipient": transfer_recipient,
             "reason": reason,
             "currency": currency,
             "reference": reference,
         }
         return self._post_request("/transfer", data=data)
 
-    def finalize_transfer(self, transfer_code: str, otp: str) -> dict:
+    def finalize_transfer(self, transfer_code: str, otp: str) -> Response:
         """
         Finalize an initiated transfer
 
         :param: transfer_code: The code of the transfer to finalize
         :param: otp: The OTP sent to the business phone to verify transfer
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"transfer_code": transfer_code, "otp": otp}
         return self._post_request("/transfer/finalize_transfer", data=data)
 
     def initiate_bulk_transfer(
-            self, transfer_source: str, transfers: List[Dict[str, str]]
-    ) -> dict:
+            self, transfer_source: str, transfers: List[Dict[str, Any]]
+    ) -> Response:
         """
         Batch multiple transfers in a single request
 
         :param: transfer_source: Where should we transfer from? Only balance for now
         :param: transfers: A list of transfer objects keys [ { amount | recipient | reference | reason } ]
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"source": transfer_source, "transfers": transfers}
         return self._post_request("/transfer/bulk", data=data)
 
     def list_transfers(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            customer_id: Optional[str] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer_id: Optional[Union[str, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List transfers
 
         :param: per_page: The number of records to return per page.
         :param: page: The page number to retrieve.
         :param: customer_id
         :param: from_date
         :param: to_date
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
@@ -107,28 +109,28 @@
             "page": page,
             "customer": customer_id,
             "from": from_date,
             "to": to_date,
         }
         return self._get_request("/transfer", params=params)
 
-    def fetch_transfer(self, id_or_code: str) -> dict:
+    def fetch_transfer(self, id_or_code: str) -> Response:
         """
         Get details of a transfer
 
         :param: id_or_code: The id or code of the transfer
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request(f"/transfer/{id_or_code}")
 
-    def verify_transfer(self, reference: str) -> dict:
+    def verify_transfer(self, reference: str) -> Response:
         """
         Verify a transfer
 
         :param: reference: The reference of the transfer to verify
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._post_request(f"/transfer/verify/{reference}")
```

### Comparing `paystackease-0.1.3/paystackease/apis/transfers_control.py` & `paystackease-1.0.0/paystackease/apis/transfers_control.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 """
 Wrapper for Paystack Transfer Control APIs
 
 The Transfers Control API allows you manage settings of your transfers.
 """
 
 from paystackease._base import PayStackBaseClientAPI
+from paystackease._utils import Response
 
 
 class TransferControlClientAPI(PayStackBaseClientAPI):
     """
     Paystack Transfers Control API
     Reference: https://paystack.com/docs/api/transfer-control/
     """
 
-    def check_balance(self) -> dict:
+    def check_balance(self) -> Response:
         """
         Get the available balance
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request("/balance")
 
-    def fetch_balance_ledger(self) -> dict:
+    def fetch_balance_ledger(self) -> Response:
         """
         Fetch all pay-ins and pay-outs that occurred on your integration
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request("/balance/ledger")
 
-    def resend_otp(self, transfer_code: str, reason: str) -> dict:
+    def resend_otp(self, transfer_code: str, reason: str) -> Response:
         """
         Generates a new OTP and sends to customer in the event
         they are having trouble receiving one.
 
         :param: transfer_code: The code of the transfer to finalize
         :param: reason: Either resend_otp or transfer as the value of this field
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"transfer_code": transfer_code, "reason": reason}
         return self._post_request("/transfer/resend_otp", data=data)
 
-    def disable_otp(self) -> dict:
+    def disable_otp(self) -> Response:
         """
         This is used in the event that you want to be able to
          complete transfers programmatically without use of OTPs
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._post_request("/transfer/disable_otp")
 
-    def finalize_disable_otp(self, otp: str) -> dict:
+    def finalize_disable_otp(self, otp: str) -> Response:
         """
         Finalize the request to disable OTP on your transfers.
 
         :param: otp: The OTP sent to the business phone to verify disabling of OTP
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"otp": otp}
         return self._post_request("/transfer/disable_otp_finalize", data=data)
 
-    def enable_otp(self) -> dict:
+    def enable_otp(self) -> Response:
         """
         This is used in the event that you want to stop
         being able to complete transfers programmatically with use of OTPs
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._post_request("/transfer/enable_otp")
```

### Comparing `paystackease-0.1.3/paystackease/apis/verification.py` & `paystackease-1.0.0/paystackease/apis/verification.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,77 @@
 """
 Wrapper for Paystack Verification APIs
-\
+
 The Verification API allows you to perform KYC processes.
 """
 
 from paystackease._base import PayStackBaseClientAPI
+from paystackease._utils import Response
 
 
 class VerificationClientAPI(PayStackBaseClientAPI):
     """
     Paystack Verification API
     Reference: https://paystack.com/docs/api/verification/
     """
 
-    def resolve_account(self, account_number: str, bank_code: str) -> dict:
+    def resolve_account(self, account_number: str, bank_code: str) -> Response:
         """
         Confirm an account belongs to the right customer.
         This feature is available to business in Nigeria and Ghana.
 
         :param: account_number: The account number to verify
         :param: bank_code: The bank code to verify
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         params = {"account_number": account_number, "bank_code": bank_code}
         return self._get_request("/bank/resolve", params=params)
 
     def validate_account(
             self,
             account_name: str,
             account_number: str,
             account_type: str,
             bank_code: str,
             country_code: str,
             document_type: str,
             document_number: str,
-    ) -> dict:
+    ) -> Response:
         """
         Confirm the authenticity of a customer's account number before sending money.
         This feature is only available to businesses in South Africa.
 
         :param: account_name: The account name to validate: first and last name
         :param: account_number: The account number to validate
         :param: account_type: The account type to validate: personal or business
         :param: bank_code: The bank code to validate
         :param: country_code: The country code to validate
         :param: document_type: The customer's mode of identity:
                                 identityNumber, passportNumber or businessRegistrationNumber
         :param: document_number: The customer's document number
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "account_name": account_name,
             "account_number": account_number,
             "account_type": account_type,
             "bank_code": bank_code,
             "country_code": country_code,
             "document_type": document_type,
             "document_number": document_number,
         }
         return self._post_request("/bank/validate", data=data)
 
-    def resolve_card_bin(self, bin_code: str) -> dict:
+    def resolve_card_bin(self, bin_code: str) -> Response:
         """
         Resolve a card BIN
 
         :param: bin_code: First 6 characters of card
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return self._get_request(f"/decision/bin/{bin_code}")
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/__init__.py` & `paystackease-1.0.0/paystackease/async_apis/__init__.py`

 * *Files identical despite different names*

### Comparing `paystackease-0.1.3/paystackease/async_apis/aapple_pay.py` & `paystackease-1.0.0/paystackease/async_apis/aapple_pay.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 """
 Wrapper class for Asynchronous Paystack Apple Pay API.
 
 The Apple Pay API allows you register your application's top-level domain or subdomain.
 """
 
-from typing import Optional
+from typing import Optional, Union
 from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
 
 
 class AsyncApplePayClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Apple Pay API
     Reference: https://paystack.com/docs/api/apple-pay/
     """
 
-    async def register_domain(self, domain_name: str) -> dict:
+    async def register_domain(self, domain_name: str) -> Response:
         """
         Register a domain or subdomain for Apple Pay
 
         :param: domain_name  # domain name or subdomain
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "domainName": domain_name,
         }
         return await self._post_request("/apple-pay/domain", data=data)
 
     async def list_domains(
         self,
-            use_cursor: Optional[bool] = False,
-            next_page: Optional[int] = None,
-            previous_page: Optional[int] = None,
-    ) -> dict:
+            use_cursor: Optional[Union[bool, None]] = False,
+            next_page: Optional[Union[int, None]] = None,
+            previous_page: Optional[Union[int, None]] = None,
+    ) -> Response:
         """
         List all registered domains
 
         :param: use_cursor  # use cursor for pagination
         :param: next_page  # next page
         :param: previous_page  # previous page
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert bool to string
         use_cursor = self._convert_to_string(use_cursor)
 
         params = {
             "use_cursor": use_cursor,
             "next": next_page,
             "previous": previous_page,
         }
         return await self._get_request("/apple-pay/domain", params=params)
 
-    async def unregister_domain(self, domain_name: str) -> dict:
+    async def unregister_domain(self, domain_name: str) -> Response:
         """
         Unregister a domain or subdomain for Apple Pay
 
         :param: domain_name  # domain name or subdomain
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "domainName": domain_name,
         }
         return await self._delete_request("/apple-pay/domain", data=data)
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/abulk_charges.py` & `paystackease-1.0.0/paystackease/apis/bulk_charges.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,96 +1,97 @@
-"""
-Wrapper for Asynchronous Paystack Bulk Charges API.
+""" Wrapper for Paystack Bulk Charges API.
 
 The Bulk Charges API allows you to create and manage multiple recurring payments from your customers.
 """
 
 from datetime import date
+from typing import List, Dict, Optional, Any, Union
 
-from typing import List, Dict, Optional
-from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._base import PayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import STATUS
 
 
-class AsyncBulkChargesClientAPI(AsyncPayStackBaseClientAPI):
+class BulkChargesClientAPI(PayStackBaseClientAPI):
     """
     Paystack Bulk Charges API
     Reference: https://paystack.com/docs/api/bulk-charge/
     """
 
-    async def initiate_bulk_charge(self, objects: List[Dict[str, str]] = None) -> dict:
+    def initiate_bulk_charge(self, objects: List[Dict[str, Any]]) -> Response:
         """
         Send an array of objects with authorization codes and amount
 
         :param: objects
 
         note::
 
             A list of dictionary with authorization codes, amount and reference as keys
             [{"authorization_code": "123456", "amount": 1000, "reference": "123456" }]
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._post_request("/bulkcharge", data=objects)
+        return self._post_request("/bulkcharge", data=objects)
 
-    async def list_bulk_charge_batches(
+    def list_bulk_charge_batches(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all bulk charges
 
         :param: per_page
         :param: page
         :param: from_date
         :param: to_date
 
         note::
 
             Date Time format: 2016-09-24T00:00:05.000Z, 2016-09-21
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # Convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
-        return await self._get_request("/bulkcharge", params=params)
+        return self._get_request("/bulkcharge", params=params)
 
-    async def fetch_bulk_charge_batch(self, id_or_code: str) -> dict:
+    def fetch_bulk_charge_batch(self, id_or_code: str) -> Response:
         """
         Fetch a bulk charge of a specific batch
 
         :param: id_or_code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._get_request(f"/bulkcharge/{id_or_code}")
+        return self._get_request(f"/bulkcharge/{id_or_code}")
 
-    async def fetch_charge_bulk_batch(
+    def fetch_charge_bulk_batch(
             self,
             id_or_code: str,
-            status: Optional[str] = None,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            status: Optional[Union[STATUS, None]] = None,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         Fetch a bulk charge of a specific batch
 
         :param: id_or_code
         :param: status:  {STATUS.value.value}
         :param: per_page
         :param: page
@@ -99,44 +100,44 @@
 
         note::
 
             Date Time format: 2016-09-24T00:00:05.000Z, 2016-09-21
             status: STATUS.value.value
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # Convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
             "status": status,
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
-        return await self._get_request(f"/bulkcharge/{id_or_code}/charges", params=params)
+        return self._get_request(f"/bulkcharge/{id_or_code}/charges", params=params)
 
-    async def pause_bulk_charge_batch(self, batch_code: str) -> dict:
+    def pause_bulk_charge_batch(self, batch_code: str) -> Response:
         """
         Pause a bulk charge of a specific batch
 
         :param: batch_code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._get_request(f"/bulkcharge/pause/{batch_code}")
+        return self._get_request(f"/bulkcharge/pause/{batch_code}")
 
-    async def resume_bulk_charge_batch(self, batch_code: str) -> dict:
+    def resume_bulk_charge_batch(self, batch_code: str) -> Response:
         """
         Resume a bulk charge of a specific batch
 
         :param: batch_code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._get_request(f"/bulkcharge/resume/{batch_code}")
+        return self._get_request(f"/bulkcharge/resume/{batch_code}")
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/acharges.py` & `paystackease-1.0.0/paystackease/async_apis/acharges.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 """
 Wrapper for Asynchronous Paystack Charges API.
 
 The Charge API allows you to configure payment channel of your choice when initiating a payment.
 """
+
 from datetime import date
-from typing import Optional, Dict, Any
+from typing import Optional, Dict, Any, List, Union
 from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import PWT
 
 
 class AsyncChargesClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Charges API
     Reference: https://paystack.com/docs/api/charge/
     """
 
     async def create_charge(
         self,
             email: str,
             amount: int,
-            pin: Optional[int] = None,
-            authorization_code: Optional[str] = None,
-            reference: Optional[str] = None,
-            device_id: Optional[str] = None,
-            bank: Optional[Dict[str, str]] = None,
-            bank_transfer: Optional[Dict[str, Any]] = None,
-            qr: Optional[Dict[str, str]] = None,
-            ussd: Optional[Dict[str, str]] = None,
-            mobile_money: Optional[Dict[str, str]] = None,
-            metadata: Optional[Dict[str, str]] = None,
-    ) -> dict:
+            pin: Optional[Union[int, None]] = None,
+            authorization_code: Optional[Union[str, None]] = None,
+            reference: Optional[Union[str, None]] = None,
+            device_id: Optional[Union[str, None]] = None,
+            bank: Optional[Union[Dict[str, str], None]] = None,
+            bank_transfer: Optional[Union[Dict[PWT, Any], None]] = None,
+            qr: Optional[Union[Dict[str, str], None]] = None,
+            ussd: Optional[Union[Dict[str, str], None]] = None,
+            mobile_money: Optional[Union[Dict[str, str], None]] = None,
+            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
+    ) -> Response:
         """
         Create a charge
 
         :param: email
         :param: amount
         :param: bank. (Set key ass: {code, account_number})
         :param: bank_transfer. (Set key as: {account_expires_at} and value: {datetime iso format})
@@ -58,15 +61,15 @@
 
             Send with a non-reusable authorization code:
             * pin
 
             mobile_money is only available in Ghana and Kenya
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "email": email,
             "amount": amount,
             "authorization_code": authorization_code,
             "bank": bank,
             "bank_transfer": bank_transfer,
@@ -76,111 +79,111 @@
             "ussd": ussd,
             "mobile_money": mobile_money,
             "device_id": device_id,
             "metadata": metadata,
         }
         return await self._post_request("/charge", data=data)
 
-    async def submit_pin(self, pin: int, reference: str) -> dict:
+    async def submit_pin(self, pin: int, reference: str) -> Response:
         """
         Submit a PIN for a charge
 
         :param: pin
         :param: reference
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "pin": pin,
             "reference": reference,
         }
         return await self._post_request("/charge/submit_pin", data=data)
 
-    async def submit_otp(self, otp: int, reference: str) -> dict:
+    async def submit_otp(self, otp: int, reference: str) -> Response:
         """
         Submit OTP to complete a charge
 
         :param: otp
         :param: reference
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "otp": otp,
             "reference": reference,
         }
         return await self._post_request("/charge/submit_otp", data=data)
 
-    async def submit_phone(self, phone: str, reference: str) -> dict:
+    async def submit_phone(self, phone: str, reference: str) -> Response:
         """
         Submit a phone number to complete a charge
 
         :param: phone
         :param: reference
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "phone": phone,
             "reference": reference,
         }
         return await self._post_request("/charge/submit_phone", data=data)
 
-    async def submit_birthday(self, birthday: date, reference: str) -> dict:
+    async def submit_birthday(self, birthday: date, reference: str) -> Response:
         """
         Submit birthday when required
 
         :param: birthday
         :param: reference
 
         note::
 
             Birthday submitted by user e.g. 2016-09-21
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         birthday = self._convert_to_string(birthday)
 
         data = {
             "birthday": birthday,
             "reference": reference,
         }
         return await self._post_request("/charge/submit_birthday", data=data)
 
     async def submit_address(
         self, reference: str, address: str, city: str, state: str, zipcode: str
-    ) -> dict:
+    ) -> Response:
         """
         Submit address to continue a charge
 
         :param: reference
         :param: address
         :param: city
         :param: state
         :param: zipcode
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "reference": reference,
             "address": address,
             "city": city,
             "state": state,
             "zip_code": zipcode,
         }
         return await self._post_request("/charge/submit_address", data=data)
 
-    async def check_pending_charge(self, reference: str) -> dict:
+    async def check_pending_charge(self, reference: str) -> Response:
         """
         Check pending charge
 
         :param: reference
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request(f"/charge/{reference}")
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/acustomers.py` & `paystackease-1.0.0/paystackease/apis/customers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 """
-Wrapper for Asynchronous Paystack Customers API.
+Wrapper for Paystack Customers API.
 
 The Customers API allows you to create and manage customers on your integration.
 """
 
 from datetime import date
 
-from typing import Optional, Dict, Any
-from paystackease._abase import AsyncPayStackBaseClientAPI
+from typing import Optional, Dict, Any, Union
+from paystackease.helpers.tool_kit import RiskAction
+from paystackease._utils import Response
+from paystackease._base import PayStackBaseClientAPI
 
 
-class AsyncCustomerClientAPI(AsyncPayStackBaseClientAPI):
+class CustomerClientAPI(PayStackBaseClientAPI):
     """
     Paystack Customer API
     Reference: https://paystack.com/docs/api/customer/
     """
 
-    async def create_customer(
-            self,
-            email: str,
-            first_name: str,
-            last_name: str,
-            phone: str,
-            metadata: Optional[Dict[str, Any]] = None
-    ) -> dict:
+    def create_customer(
+            self, 
+            email: str, 
+            first_name: str, 
+            last_name: str, 
+            phone: str, 
+            metadata: Optional[Union[Dict[str, Any], None]] = None
+    ) -> Response:
         """
         Create a customer
 
         :param: email: The email associated with the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: phone: The phone number of the customer.
         :param: metadata: The metadata of the customer in JSON format.
-                            (Set key as: {"custom_fields": [{ "label": "First Name", "value": "John" }] })
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "email": email,
             "first_name": first_name,
             "last_name": last_name,
             "phone": phone,
             "metadata": metadata,
         }
-        return await self._post_request("/customer", data=data)
+        return self._post_request("/customer", data=data)
 
-    async def validate_customer(
+    def validate_customer(
             self,
             email_or_code: str,
             first_name: str,
             last_name: str,
             account_type: str,
             country: str,
             bank_code: str,
             account_number: str,
             bvn: str,
-            customer_id_num: Optional[str] = None,
-            middle_name: Optional[str] = None
-    ) -> dict:
+            customer_id_num: Optional[Union[str, None]] = None,
+            middle_name: Optional[Union[str, None]] = None
+    ) -> Response:
         """
         Validate a customer's identity
 
         :param: email_or_code: The email or code of the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: middle_name: The middle name of the customer.
@@ -70,113 +71,116 @@
         :param: customer_id_num: The customer identification number
         :param: country: The country of the customer. 2-letter country code of identification issuer
         :param: bvn: The Bank Verification Number
         :param: bank_code: The bank code of the customer
         :param: account_number: The account number of the customer
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "first_name": first_name,
             "last_name": last_name,
             "middle_name": middle_name,
             "type": account_type,
             "value": customer_id_num,
             "country": country,
             "bvn": bvn,
             "bank_code": bank_code,
             "account_number": account_number,
         }
-        return await self._post_request(f"customer/{email_or_code}/identification", data=data)
+        return self._post_request(f"customer/{email_or_code}/identification", data=data)
 
-    async def whitelist_blacklist_customer(
-            self, email_or_code: str, risk_action: Optional[str] = None
-    ) -> dict:
+    def whitelist_blacklist_customer(
+            self, email_or_code: str, risk_action: Optional[Union[RiskAction, None]] = None
+    ) -> Response:
         """
         Whitelist or blacklist a customer
 
         :param: email_or_code: The code or email of the customer.
         :param: risk_action: The action to take on the customer. value: RiskAction.value.value = "allow" pr "deny"
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        data = {"customer": email_or_code, "risk_action": risk_action}
-        return await self._post_request("/customer/set_risk_action", data=data)
+        data = {
+            "customer": email_or_code,
+            "risk_action": risk_action
+        }
+        return self._post_request("/customer/set_risk_action", data=data)
 
-    async def deactivate_authorization(self, authorization_code: str) -> dict:
+    def deactivate_authorization(self, authorization_code: str) -> Response:
         """
         Deactivate an authorization when the card needs to be forgotten
 
         :param: authorization_code: The authorization code to be deactivated.
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"authorization_code": authorization_code}
-        return await self._post_request("/customer/deactivate_authorization", data=data)
+        return self._post_request("/customer/deactivate_authorization", data=data)
 
-    async def update_customer(
+    def update_customer(
             self,
             customer_code: str,
-            first_name: Optional[str] = None,
-            last_name: Optional[str] = None,
-            phone: Optional[str] = None,
-            metadata: Optional[Dict[str, Any]] = None
-    ) -> dict:
+            first_name: Optional[Union[str, None]] = None,
+            last_name: Optional[Union[str, None]] = None,
+            phone: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, Any], None]] = None
+    ) -> Response:
         """
         Update a customer
 
         :param: customer_code: The code of the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: phone: The phone number of the customer.
         :param: metadata: The metadata of the customer in JSON format. {"key1": "value1", "key2": "value2"}
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "first_name": first_name,
             "last_name": last_name,
             "phone": phone,
             "metadata": metadata,
         }
-        return await self._put_request(f"/customer/{customer_code}", data=data)
+        return self._put_request(f"/customer/{customer_code}", data=data)
 
-    async def fetch_customer(self, email_or_code: str) -> dict:
+    def fetch_customer(self, email_or_code: str) -> Response:
         """
         Fetch details of a specific customer
 
         :param: email_or_code: The email or code of the customer.
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._get_request(f"/customer/{email_or_code}")
+        return self._get_request(f"/customer/{email_or_code}")
 
-    async def list_customers(
+    def list_customers(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all customers
 
         :param: per_page: The number of records to return.
         :param: page: The page number to return.
         :param: from_date: The date to start returning customers from
         :param: to_date: The date to stop returning customers from
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date  to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return await self._get_request("/customer", params=params)
+        return self._get_request("/customer", params=params)
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/adedicated_virtual_accounts.py` & `paystackease-1.0.0/paystackease/apis/dedicated_virtual_accounts.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 """
-Wrapper for Asynchronous Paystack Dedicated Virtual Account API
+Wrapper for Paystack Dedicated Virtual Account API
 
 The Dedicated Virtual Account API enables Nigerian merchants to manage unique payment accounts of their customers.
 """
 
 from datetime import date
-from typing import Optional
-from paystackease._abase import AsyncPayStackBaseClientAPI
+from typing import Optional, Union
+from paystackease._base import PayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import Currency
 
 
-class AsyncDedicatedVirtualAccountClientAPI(AsyncPayStackBaseClientAPI):
+class DedicatedVirtualAccountClientAPI(PayStackBaseClientAPI):
     """
     Paystack Dedicated Virtual Account API
     Reference: https://paystack.com/docs/api/dedicated-virtual-account/
 
     note::
         Ensure Dedicated NUBAN is available for your business. Contact Paystack Support
     """
 
-    async def create_virtual_account(
+    def create_virtual_account(
             self,
             customer_id_or_code: str,
-            preferred_bank: Optional[str] = None,
-            subaccount: Optional[str] = None,
-            split_code: Optional[str] = None,
-            first_name: Optional[str] = None,
-            last_name: Optional[str] = None,
-            phone: Optional[str] = None,
-    ) -> dict:
+            preferred_bank: Optional[Union[str, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            first_name: Optional[Union[str, None]] = None,
+            last_name: Optional[Union[str, None]] = None,
+            phone: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Create a dedicated virtual account for existing customers.
         Currently, support Wema Bank and Titan Paystack.
 
         :param: customer_id_or_code: The customer's ID or Code
         :param: preferred_bank: Preferred bank slug for the virtual account. Eg: "wema-bank"
 
@@ -42,41 +44,41 @@
         :param: subaccount: Subaccount code of the account you want to split the transaction.
         :param: split_code: Split code
         :param: first_name: First name of the customer
         :param: last_name: Last name of the customer
         :param: phone: Phone number of the customer
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "customer": customer_id_or_code,
             "preferred_bank": preferred_bank,
             "subaccount": subaccount,
             "split_code": split_code,
             "first_name": first_name,
             "last_name": last_name,
             "phone": phone,
         }
-        return await self._post_request("/dedicated_account", data=data)
+        return self._post_request("/dedicated_account", data=data)
 
-    async def assign_dedicated_virtual_account(
+    def assign_dedicated_virtual_account(
             self,
             email: str,
             first_name: str,
             last_name: str,
             phone: str,
             preferred_bank: str,
             country: str,
-            account_number: Optional[str] = None,
-            bvn: Optional[str] = None,
-            bank_code: Optional[str] = None,
-            subaccount: Optional[str] = None,
-            split_code: Optional[str] = None,
-    ) -> dict:
+            account_number: Optional[Union[str, None]] = None,
+            bvn: Optional[Union[str, None]] = None,
+            bank_code: Optional[Union[str, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         create a customer, validate the customer, and assign a DVA to the customer
 
         :param: email: The email associated with the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: phone: The phone number of the customer.
@@ -95,150 +97,153 @@
         :param: account_number: The account number of the customer
         :param: bvn: The Bank Verification Number
         :param: bank_code: The bank code of the customer
         :param: subaccount: Subaccount code of the account you want to split the transaction.
         :param: split_code: Split code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "email": email,
             "first_name": first_name,
             "last_name": last_name,
             "phone": phone,
             "preferred_bank": preferred_bank,
             "country": country,
             "account_number": account_number,
             "bvn": bvn,
             "bank_code": bank_code,
             "subaccount": subaccount,
             "split_code": split_code,
         }
-        return await self._post_request("/dedicated_account", data=data)
+        return self._post_request("/dedicated_account", data=data)
 
-    async def list_dedicated_account(
+    def list_dedicated_account(
             self,
-            active: Optional[bool] = True,
-            currency: Optional[str] = None,
-            provider_slug: Optional[str] = None,
-            bank_id: Optional[str] = None,
-            customer_id: Optional[str] = None,
-    ) -> dict:
+            active: Optional[Union[bool, None]] = True,
+            currency: Optional[Union[Currency, None]] = None,
+            provider_slug: Optional[Union[str, None]] = None,
+            bank_id: Optional[Union[str, None]] = None,
+            customer_id: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         List dedicated accounts
 
         :param: active: Shows the status of the dedicated virtual account
         :param: currency: Currency of the dedicated virtual account
         :param: provider_slug: Provider slug in lowercase eg: wema-bank
         :param: bank_id: Bank ID of the dedicated virtual account eg: 035
         :param: customer_id: Customer ID of the dedicated virtual account
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
+        # convert date to string
+        active = self._convert_to_string(active)
+
         params = {
             "active": active,
             "currency": currency,
             "provider_slug": provider_slug,
             "bank_id": bank_id,
             "customer": customer_id,
         }
-        return await self._get_request("/dedicated_account", params=params)
+        return self._get_request("/dedicated_account", params=params)
 
-    async def fetch_dedicated_account(self, dedicated_account_id: int) -> dict:
+    def fetch_dedicated_account(self, dedicated_account_id: int) -> Response:
         """
         Get details of a dedicated virtual account
 
         :param: dedicated_account_id: Dedicated account ID
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._get_request(f"/dedicated_account/{dedicated_account_id}")
+        return self._get_request(f"/dedicated_account/{dedicated_account_id}")
 
-    async def requery_dedicated_account(
+    def requery_dedicated_account(
             self,
-            account_number: Optional[str] = None,
-            provider_slug: Optional[str] = None,
-            date_transfer: Optional[date] = None,
-    ) -> dict:
+            account_number: Optional[Union[str, None]] = None,
+            provider_slug: Optional[Union[str, None]] = None,
+            date_transfer: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         Requery a dedicated virtual account for new transactions
 
         :param: account_number: Virtual Account number to requery
         :param: provider_slug: Provider slug in lowercase eg: wema-bank
         :param: date_transfer: Date of when the transfer was made
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         date_transfer = self._convert_to_string(date_transfer)
 
         params = {
             "account_number": account_number,
             "provider_slug": provider_slug,
             "date": date_transfer,
         }
-        return await self._get_request("/dedicated_account/requery", params=params)
+        return self._get_request("/dedicated_account/requery", params=params)
 
-    async def deactivate_dedicated_account(self, dedicated_account_id: int) -> dict:
+    def deactivate_dedicated_account(self, dedicated_account_id: int) -> Response:
         """
         Deactivate a dedicated virtual account
 
         :param: dedicated_account_id: Dedicated account ID
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._delete_request(f"/dedicated_account/{dedicated_account_id}")
+        return self._delete_request(f"/dedicated_account/{dedicated_account_id}")
 
-    async def split_dedicated_account(
+    def split_dedicated_account(
             self,
             customer_id_or_code: str,
-            subaccount: Optional[str] = None,
-            split_code: Optional[str] = None,
-            preferred_bank: Optional[str] = None,
-    ) -> dict:
+            subaccount: Optional[Union[str, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            preferred_bank: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Split a dedicated virtual account transaction with one or more accounts
 
         :param: customer_id_or_code: Customer's ID or Code
         :param: subaccount: Subaccount code of the account you want to split the transaction
         :param: split_code: Split code
         :param: preferred_bank: Preferred bank for the virtual account
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "customer": customer_id_or_code,
             "preferred_bank": preferred_bank,
             "subaccount": subaccount,
             "split_code": split_code,
         }
-        return await self._post_request("/dedicated_account/split", data=data)
+        return self._post_request("/dedicated_account/split", data=data)
 
-    async def remove_split_dedicated_account(self, account_number: str) -> dict:
+    def remove_split_dedicated_account(self, account_number: str) -> Response:
         """
         Remove a split dedicated virtual account
 
         :param: account_number: the account number of the dedicated virtual account
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "account_number": account_number,
         }
-        return await self._delete_request("/dedicated_account/split", data=data)
+        return self._delete_request("/dedicated_account/split", data=data)
 
-    async def fetch_bank_providers(self) -> dict:
+    def fetch_bank_providers(self) -> Response:
         """
         Fetch bank providers
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._get_request("/dedicated_account/available_providers")
+        return self._get_request("/dedicated_account/available_providers")
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/adisputes.py` & `paystackease-1.0.0/paystackease/async_apis/adisputes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 """
 Wrapper for Asynchronous Paystack Disputes API
 
 The Disputes API allows you manage transaction disputes on your integration.
 """
 
 from datetime import date
-from typing import Optional
+from typing import Optional, Union
 from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import DisputeStatus, Resolution
 
 
 class AsyncDisputesClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Disputes API
     Reference: https://paystack.com/docs/api/dispute/
     """
 
     async def list_disputes(
             self,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            transaction_id: Optional[str] = None,
-            status: Optional[str] = None,
-    ) -> dict:
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            transaction_id: Optional[Union[str, None]] = None,
+            status: Optional[Union[DisputeStatus, None]] = None,
+    ) -> Response:
         """
         List disputes filed against you
 
         :param: from_date: A timestamp from which to start listing dispute e.g. 2016-09-21
         :param: to_date: A timestamp from which to start listing dispute e.g. 2016-09-21
         :param: per_page:
         :param: page:
         :param: transaction_id:
         :param: status: Dispute Status. Acceptable values:
                         { awaiting-merchant-feedback | awaiting-bank-feedback | pending | resolved }
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
@@ -49,79 +51,79 @@
             "from": from_date,
             "to": to_date,
             "transaction": transaction_id,
             "status": status,
         }
         return await self._get_request("/dispute", params=params)
 
-    async def fetch_dispute(self, dispute_id: str) -> dict:
+    async def fetch_dispute(self, dispute_id: str) -> Response:
         """
         Fetch details about a dispute
 
         :param: dispute_id: The dispute ID to fetch
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request(f"/dispute/{dispute_id}")
 
-    async def list_transaction_disputes(self, transaction_id: str) -> dict:
+    async def list_transaction_disputes(self, transaction_id: str) -> Response:
         """
         List disputes for a transaction
 
         :param: transaction_id: The transaction id to fetch
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request(f"/dispute/transaction/{transaction_id}")
 
     async def update_dispute(
             self,
             dispute_id: str,
             refund_amount: int,
-            uploaded_filename: Optional[str] = None,
-    ) -> dict:
+            uploaded_filename: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Update details of a dispute
 
         :param: dispute_id: The dispute id to fetch
         :param: refund_amount: The amount to refund to the customer
         :param: uploaded_filename: filename of attachment returned via
                                     response from upload url(GET /dispute/:id/upload_url)
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"refund_amount": refund_amount, "uploaded_filename": uploaded_filename}
         return await self._put_request(f"/dispute/{dispute_id}", data=data)
 
     async def add_evidence(
             self,
             dispute_id: str,
             customer_email: str,
             customer_name: str,
             customer_phone: str,
             service_details: str,
-            delivery_address: Optional[str] = None,
-            delivery_date: Optional[date] = None,
-    ) -> dict:
+            delivery_address: Optional[Union[str, None]] = None,
+            delivery_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         Add evidence to a dispute
 
         :param: dispute_id: The dispute id to fetch
         :param: customer_email: The customer email
         :param: customer_name: The customer name
         :param: customer_phone: The customer phone
         :param: service_details: The service details
         :param: delivery_address: The delivery address
         :param: delivery_date: The delivery date: YYYY-MM-DD
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         delivery_date = self._convert_to_string(delivery_date)
 
         data = {
             "customer_email": customer_email,
@@ -129,80 +131,80 @@
             "customer_phone": customer_phone,
             "service_details": service_details,
             "delivery_address": delivery_address,
             "delivery_date": delivery_date,
         }
         return await self._post_request(f"/dispute/{dispute_id}/evidence", data=data)
 
-    async def get_upload_url(self, dispute_id: str, uploaded_filename: str) -> dict:
+    async def get_upload_url(self, dispute_id: str, uploaded_filename: str) -> Response:
         """
         Get upload url for dispute evidence
 
         :param: dispute_id: The dispute id to fetch
         :param: uploaded_filename: The file name, with its extension, that you want to upload. e.g. filename.pdf
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         params = {"uploaded_filename": uploaded_filename}
         return await self._get_request(f"/dispute/{dispute_id}/upload_url", params=params)
 
     async def resolve_dispute(
             self,
             dispute_id: str,
-            resolution: str,
+            resolution: Resolution,
             message: str,
             refund_amount: int,
             uploaded_filename: str,
-            evidence: Optional[int] = None,
-    ) -> dict:
+            evidence: Optional[Union[int, None]] = None,
+    ) -> Response:
         """
         Resolve a dispute
 
         :param: dispute_id: The dispute id to fetch
         :param: resolution: The resolution to resolve the dispute: Accepted values: { merchant-accepted | declined }.
         :param: message: The message for resolution
         :param: refund_amount: The amount to refund to the customer
         :param: uploaded_filename: filename of attachment returned via response from method get_upload_url
         :param: evidence: The evidence id for fraud claims
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "resolution": resolution,
             "message": message,
             "refund_amount": refund_amount,
             "uploaded_filename": uploaded_filename,
             "evidence": evidence,
         }
         return await self._put_request(f"/dispute/{dispute_id}/resolve", data=data)
 
     async def export_disputes(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-            transaction_id: Optional[str] = None,
-            status: Optional[str] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+            transaction_id: Optional[Union[str, None]] = None,
+            status: Optional[Union[DisputeStatus, None]] = None,
+    ) -> Response:
         """
         Export disputes
 
         :param: per_page:
         :param: page:
         :param: from_date: The start date to fetch disputes from
         :param: to_date: The end date to fetch disputes from
         :param: transaction_id: The transaction ID
         :param: status: The dispute status:
                         Acceptable values: { awaiting-merchant-feedback | awaiting-bank-feedback | pending | resolved }
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/aintegration.py` & `paystackease-1.0.0/paystackease/async_apis/aintegration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
 Wrapper for Asynchronous Paystack Integration API
 
 The Integration API allows you manage some settings on your integration.
 """
-
+from paystackease._utils import Response
 from paystackease._abase import AsyncPayStackBaseClientAPI
 
 
 class AsyncIntegrationClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Integration API
     Reference: https://paystack.com/docs/api/integration/
     """
 
-    async def fetch_timeout(self) -> dict:
+    async def fetch_timeout(self) -> Response:
         """
         Fetch payment session timeout
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request("/integration/payment_session_timeout")
 
-    async def update_timeout(self, timeout: int) -> dict:
+    async def update_timeout(self, timeout: int) -> Response:
         """
         Update payment session timeout
 
         :param: timeout: The new payment session timeout before session
 
         note::
 
             timeout is in seconds. Set 0 to cancel the timeout
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         data = {"timeout": timeout}
         return await self._put_request("/integration/payment_session_timeout", data=data)
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/amiscellaneous.py` & `paystackease-1.0.0/paystackease/async_apis/amiscellaneous.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 """
 Wrapper for Paystack Miscellaneous API.
 
 The Miscellaneous API are supporting APIs that can be used to provide more details to other APIs.
 """
 
-from typing import Optional
+from typing import Optional, Union
 from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import GateWay, Channels, Currency
 
 
 class AsyncMiscellaneousClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Miscellaneous API
     Reference: https://paystack.com/docs/api/miscellaneous/
     """
 
     async def list_banks(
             self,
-            country: Optional[str] = None,
-            use_cursor: Optional[bool] = False,
-            per_page: Optional[int] = None,
-            pay_with_bank_transfer: Optional[bool] = None,
-            pay_with_bank: Optional[bool] = None,
-            enabled_for_verification: Optional[bool] = None,
-            next_cursor: Optional[str] = None,
-            previous_cursor: Optional[str] = None,
-            gateway: Optional[str] = None,
-            channel_type: Optional[str] = None,
-            currency: Optional[str] = None,
-    ) -> dict:
+            country: Optional[Union[str, None]] = None,
+            use_cursor: Optional[Union[bool, None]] = False,
+            per_page: Optional[Union[int, None]] = 50,
+            pay_with_bank_transfer: Optional[Union[bool, None]] = False,
+            pay_with_bank: Optional[Union[bool, None]] = False,
+            enabled_for_verification: Optional[Union[bool, None]] = False,
+            next_cursor: Optional[Union[str, None]] = None,
+            previous_cursor: Optional[Union[str, None]] = None,
+            gateway: Optional[Union[GateWay, None]] = None,
+            channel_type: Optional[Union[Channels, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+    ) -> Response:
         """
         Get a list of all supported banks and their properties
 
         :param: country: The country to obtain the list of supported banks.
                         Values { country=ghana or country=nigeria }
         :param: use_cursor: Use cursor to paginate through the list of supported banks
         :param: per_page: The number of records to return per page: 10, 20 or 50
@@ -47,16 +49,23 @@
         :param: channel_type: Type of financial channel. { Channels.value.value}
 
         **note::**
 
         For Ghanaian channels, please use either mobile_money for mobile money channels OR ghipps for bank channels
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
+
+        # convert to strings
+        use_cursor = self._convert_to_string(use_cursor)
+        pay_with_bank_transfer = self._convert_to_string(pay_with_bank_transfer)
+        pay_with_bank = self._convert_to_string(pay_with_bank)
+        enabled_for_verification = self._convert_to_string(enabled_for_verification)
+
         params = {
             "country": country,
             "use_cursor": use_cursor,
             "perPage": per_page,
             "supports_transfer": pay_with_bank_transfer,
             "pay_with_bank": pay_with_bank,
             "enabled_for_verification": enabled_for_verification,
@@ -64,27 +73,27 @@
             "previous": previous_cursor,
             "gateway": gateway,
             "type": channel_type,
             "currency": currency,
         }
         return await self._get_request("/bank", params=params)
 
-    async def list_countries(self) -> dict:
+    async def list_countries(self) -> Response:
         """
         Get a list of all supported countries and their properties
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request("/country")
 
-    async def list_states(self, country: str) -> dict:
+    async def list_states(self, country: str) -> Response:
         """
         Get a list of all supported states and their properties
 
         :param: country: The country code from which to obtain the list of supported states
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         params = {"country": country}
         return await self._get_request("/address_verification/states", params=params)
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/apayment_pages.py` & `paystackease-1.0.0/paystackease/async_apis/atransfer_recipients.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,156 +1,137 @@
 """
-Wrapper for Asynchronous Paystack Payment Pages API.
+Wrapper for Asynchronous Paystack Transfer Recipient APIs
 
-The Payment Pages API provides a quick and secure way to collect payment for products.
+The Transfer Recipients API allows you to create and manage beneficiaries that you send money to.
 """
 
 from datetime import date
-from typing import Optional, Dict, List
+from typing import Optional, Dict, List, Any, Union
 from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import Currency
 
 
-class AsyncPaymentPagesClientAPI(AsyncPayStackBaseClientAPI):
+class AsyncTransferRecipientsClientAPI(AsyncPayStackBaseClientAPI):
     """
-    Paystack Payment Pages API
-    Reference: https://paystack.com/docs/api/page/
+    Paystack Transfer Recipients API
+    Reference: https://paystack.com/docs/api/transfer-recipient/
     """
 
-    async def create_payment_page(
+    async def create_transfer_recipients(
             self,
-            name: str,
-            description: Optional[str] = None,
-            amount: Optional[int] = None,
-            split_code: Optional[str] = None,
-            page_slug: Optional[str] = None,
-            redirect_url: Optional[str] = None,
-            metadata: Optional[Dict[str, str]] = None,
-            custom_fields: Optional[List[str]] = None,
-    ) -> dict:
-        """
-        Create a payment page
-
-        :param: name: Name of the page
-        :param: description: Description of the page
-        :param: amount: Amount of the page
-        :param: split_code: Split code of the transaction split
-        :param: page_slug: URL slug you would like to be associated with this page.
-
-        note::
-
-            Page will be accessible at https://paystack.com/pay/page_slug
-
-        :param: redirect_url: If you would like Paystack to redirect someplace
-                                upon successful payment, specify the URL here.
-        :param: metadata: Extra data to configure the payment page including subaccount,logo image, transaction charge
-        :param: custom_fields: If you would like to accept custom fields, specify them here.
+            recipient_type: str,
+            recipient_name: str,
+            account_number: str,
+            bank_code: str,
+            description: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            authorization_code: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, Any], None]] = None,
+    ) -> Response:
+        """
+        Create a transfer recipient
+
+        :param: recipient_type: The type of transfer recipient:[ nuban | ghipss | mobile_money | basa ]
+        :param: recipient_name: The name of the transfer recipient according to their account registration
+        :param: account_number: transfer recipient's account number.
+                                Required for all recipient types except authorization
+        :param: bank_code: transfer recipient's bank code. Required for all recipient types except authorization
+        :param: description:
+        :param: currency: transfer recipient's currency. [Currency.value.value ]
+        :param: authorization_code: transfer recipient's authorization code from previous transaction
+        :param: metadata: transfer recipient's metadata
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
-            "name": name,
+            "type": recipient_type,
+            "name": recipient_name,
+            "account_number": account_number,
+            "bank_code": bank_code,
             "description": description,
-            "amount": amount,
-            "split_code": split_code,
-            "slug": page_slug,
-            "redirect_url": redirect_url,
+            "currency": currency,
+            "authorization_code": authorization_code,
             "metadata": metadata,
-            "custom_fields": custom_fields,
         }
-        return await self._post_request("/page", data=data)
+        return await self._post_request("/transferrecipient", data=data)
 
-    async def list_payment_pages(
-            self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+    async def bulk_create_transfer_recipient(self, batch: List[Dict[str, Any]]) -> Response:
         """
-        List all the payment pages
+        Create multiple transfer recipients in batches.
 
-        :param: per_page: Number of records to return
-        :param: page: number to return
-        :param: from_date: A timestamp from which to start listing page
-        :param: to_date: A timestamp from which to start listing page
+        :param: batch: A list of transfer recipient object
+                        keys [ { type, name, account_number, bank_code, currency etc. }]
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
+        """
+        data = {"batch": batch}
+        return await self._post_request("/transferrecipient/bulk", data=data)
 
-        note::
-            Date Time value is in this format: 2016-09-24T00:00:05.000Z, 2016-09-21
+    async def list_transfer_recipients(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
+        List transfer recipients
 
-        # convert date to string
+        :param: per_page: The number of records to return per page.
+        :param: page: The page number to retrieve.
+        :param: from_date:
+        :param: to_date:
+
+        :return: The response from the API
+        :rtype: Response object
+        """
+
+        # convert date to strings
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return await self._get_request("/page", params=params)
+        return await self._get_request("/transferrecipient", params=params)
 
-    async def fetch_payment_page(self, page_id_or_slug: str) -> dict:
+    async def fetch_transfer_recipient(self, id_or_code: str) -> Response:
         """
-        Get details of a payment page
+        Fetch details of a transfer recipient
 
-        :param: page_id_or_slug: ID or slug of the payment page
+        :param: id_or_code: The id or code of the transfer recipient
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._get_request(f"/page/{page_id_or_slug}")
+        return await self._get_request(f"/transferrecipient/{id_or_code}")
 
-    async def update_payment_page(
+    async def update_transfer_recipient(
             self,
-            page_id_or_slug: str,
-            name: Optional[str] = None,
-            description: Optional[str] = None,
-            amount: Optional[int] = None,
-            active: Optional[bool] = None,
-    ) -> dict:
-        """
-        Update a payment page detail
-
-        :param: page_id_or_slug: ID or slug of the payment page
-        :param: name: Name of the page
-        :param: description: Description of the page
-        :param: amount: Amount of the page
-        :param: active: Set false to deactivate the page url
-
-        :return: The response from the API
-        :rtype: dict
-        """
-
-        # convert bool to string
-        active = self._convert_to_string(active)
-
-        data = {
-            "name": name,
-            "description": description,
-            "amount": amount,
-            "active": active,
-        }
-        return await self._put_request(f"/page/{page_id_or_slug}", data=data)
-
-    async def check_slug_available(self, page_slug: str) -> dict:
+            id_or_code: str,
+            recipient_name: str,
+            recipient_email: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
-        Check if a slug is available
+        Update a transfer recipient
 
-        :param: page_slug: URL slug you would like to be associated with this page.
+        :param: id_or_code: The id or code of the transfer recipient
+        :param: recipient_name: The name of the transfer recipient
+        :param: recipient_email: The email of the transfer recipient
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._get_request(f"/page/check_slug_availability/{page_slug}")
+        data = {"name": recipient_name, "email": recipient_email}
+        return await self._put_request(f"/transferrecipient/{id_or_code}", data=data)
 
-    async def add_products(self, payment_id: int, product: List[int]) -> dict:
+    async def delete_transfer_recipient(self, id_or_code: str) -> Response:
         """
-        Add products to a payment page
+        Delete a transfer recipient
 
-        :param: payment_id: ID of the payment page
-        :param: product: List of IDS of all the products
+        :param: id_or_code: The id or code of the transfer recipient
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        data = {"product": product}
-        return await self._post_request(f"/page/{payment_id}/product", data=data)
+        return await self._delete_request(f"/transferrecipient/{id_or_code}")
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/apayment_requests.py` & `paystackease-1.0.0/paystackease/async_apis/apayment_requests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Wrapper for Asynchronous Paystack Payment Requests API.
 
 The Payment Requests API allows you manage requests for payment of goods and services.
 """
 
 from datetime import date
-from typing import Optional, List, Dict
+from typing import Optional, List, Dict, Any, Union
 from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import PayMentRequestStatus, Currency
 
 
 class AsyncPaymentRequestClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Payment Request API
     Reference: https://paystack.com/docs/api/payment-request/
     """
@@ -18,22 +20,22 @@
     async def create_payment_request(
             self,
             customer: str,
             amount: int,
             draft: bool,
             has_invoice: bool,
             send_notification: bool,
-            due_date: Optional[date] = None,
-            description: Optional[str] = None,
-            line_items: Optional[List[Dict[str, str]]] = None,
-            tax: Optional[List[Dict[str, str]]] = None,
-            currency: Optional[str] = None,
-            invoice_number: Optional[int] = None,
-            split_code: Optional[str] = None,
-    ) -> dict:
+            due_date: Optional[Union[date, None]] = None,
+            description: Optional[Union[str, Any]] = None,
+            line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
+            tax: Optional[Union[List[Dict[str, Any]], None]] = None,
+            currency: Optional[Union[Currency, Any]] = None,
+            invoice_number: Optional[Union[int, Any]] = None,
+            split_code: Optional[Union[str, Any]] = None,
+    ) -> Response:
         """
         Create a payment request for a transaction
 
         :param: customer: Customer ID of the customer
         :param: amount: Amount of the payment request
         :param: due_date: Due date of the payment request
         :param: description: Description of the payment request
@@ -43,18 +45,21 @@
         :param: send_notification: Set true if you want to send a notification to the customer email
         :param: draft: Set true if you want to create a draft payment request
         :param: has_invoice: Set true if you want to create a draft payment request
         :param: invoice_number: Invoice number of the payment request
         :param: split_code: split code of the transaction split
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         # convert date and bool to string
         due_date = self._convert_to_string(due_date)
+        draft = self._convert_to_string(draft)
+        has_invoice = self._convert_to_string(has_invoice)
+        send_notification = self._convert_to_string(send_notification)
 
         data = {
             "customer": customer,
             "amount": amount,
             "due_date": due_date,
             "description": description,
             "line_items": line_items,
@@ -66,125 +71,129 @@
             "invoice_number": invoice_number,
             "split_code": split_code,
         }
         return await self._post_request("/paymentrequest", data=data)
 
     async def list_payment_requests(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            customer: Optional[str] = None,
-            status: Optional[str] = None,
-            currency: Optional[str] = None,
-            include_archive: Optional[str] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[str, None]] = None,
+            status: Optional[Union[PayMentRequestStatus, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            include_archive: Optional[Union[bool, None]] = True,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all the payment requests
 
         :param: per_page: Number of records to return
         :param: page:  number to return
         :param: customer: Filter by customer ID
         :param: status: Filter by payment request status
         :param: currency:
         :param: include_archive: Show archived payment requests
         :param: from_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
         :param: to_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
+        include_archive = self._convert_to_string(include_archive)
 
         params = {
             "perPage": per_page,
             "page": page,
             "customer": customer,
             "status": status,
             "currency": currency,
             "include_archive": include_archive,
             "from": from_date,
             "to": to_date,
         }
         return await self._get_request("/paymentrequest", params=params)
 
-    async def fetch_payment_request(self, id_or_code: str) -> dict:
+    async def fetch_payment_request(self, id_or_code: str) -> Response:
         """
         Get details of a payment request on your integration
 
         :param: id_or_code: ID or Code of the payment request
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request(f"/paymentrequest/{id_or_code}")
 
-    async def verify_payment_request(self, code: str) -> dict:
+    async def verify_payment_request(self, code: str) -> Response:
         """
         Verify details of a payment request on your integration
 
         :param: code: Payment request code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request(f"/paymentrequest/verify/{code}")
 
-    async def send_notification(self, code: str) -> dict:
+    async def send_notification(self, code: str) -> Response:
         """
         Send notification of a payment request to a customer
 
         :param: code: Payment request code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._post_request(f"/paymentrequest/notify/{code}")
 
-    async def payment_request_total(self) -> dict:
+    async def payment_request_total(self) -> Response:
         """
         Get total of a payment request metric
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request("/paymentrequest/totals")
 
-    async def finalize_payment_request(self, code: str, send_notification: bool) -> dict:
+    async def finalize_payment_request(self, code: str, send_notification: bool) -> Response:
         """
         Finalize a draft payment request
 
         :param: code: Payment request code
         :param: send_notification: Set true if you want to send a notification to the customer email
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
+        # convert to strings
+        send_notification = self._convert_to_string(send_notification)
+
         data = {"send_notification": send_notification}
         return await self._post_request(f"/paymentrequest/finalize/{code}", data=data)
 
     async def update_payment_request(
             self,
             id_or_code: str,
-            customer: Optional[str] = None,
-            amount: Optional[int] = None,
-            description: Optional[str] = None,
-            line_items: Optional[List[Dict[str, str]]] = None,
-            tax: Optional[List[Dict[str, str]]] = None,
-            currency: Optional[str] = None,
-            due_date: Optional[date] = None,
-            send_notification: Optional[bool] = None,
-            draft: Optional[bool] = None,
-            invoice_number: Optional[int] = None,
-            split_code: Optional[str] = None,
-    ) -> dict:
+            customer: Optional[Union[str, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            description: Optional[Union[str, None]] = None,
+            line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
+            tax: Optional[Union[List[Dict[str, Any]], None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            due_date: Optional[Union[date, None]] = None,
+            send_notification: Optional[Union[bool, None]] = True,
+            draft: Optional[Union[bool, None]] = True,
+            invoice_number: Optional[Union[int, None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Update a payment request
 
         :param: id_or_code: ID or Code of the payment request
         :param: customer: Customer ID or code of the customer
         :param: amount: Amount of the payment request
         :param: due_date: Due date of the payment request
@@ -194,19 +203,21 @@
         :param: currency: Currency of the payment request
         :param: send_notification: Set true if you want to send a notification to the customer email
         :param: draft: Set true if you want to create a draft payment request
         :param: invoice_number: Invoice number of the payment request starts from 1 and autoincrement
         :param: split_code: split code of the transaction split
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date and bool to string
         due_date = self._convert_to_string(due_date)
+        draft = self._convert_to_string(draft)
+        send_notification = self._convert_to_string(send_notification)
 
         data = {
             "customer": customer,
             "amount": amount,
             "due_date": due_date,
             "description": description,
             "line_items": line_items,
@@ -215,17 +226,17 @@
             "send_notification": send_notification,
             "draft": draft,
             "invoice_number": invoice_number,
             "split_code": split_code,
         }
         return await self._put_request(f"/paymentrequest/{id_or_code}", data=data)
 
-    async def archive_payment_request(self, code: str) -> dict:
+    async def archive_payment_request(self, code: str) -> Response:
         """
         Archive a payment request
 
         :param: code: Payment request code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._post_request(f"/paymentrequest/archive/{code}")
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/aproducts.py` & `paystackease-1.0.0/paystackease/async_apis/aproducts.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 """
 Wrapper for Asynchronous Paystack Products API
 
 The Products API allows you to create and manage inventories on your integration.
 """
 
 from datetime import date
-from typing import Optional
+from typing import Optional, Union
 from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
 
 
 class AsyncProductClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Product API
     Reference: https://paystack.com/docs/api/product/
     """
 
     async def create_product(
             self,
             name: str,
             description: str,
             amount: int,
             currency: str,
-            unlimited: Optional[bool] = None,
-            quantity: Optional[int] = None,
-    ) -> dict:
+            unlimited: Optional[Union[bool, None]] = True,
+            quantity: Optional[Union[int, None]] = None,
+    ) -> Response:
         """
         Create a product
 
         :param: name: Name of the product
         :param: description: Description of the product
         :param: amount: Price of the product
         :param: currency: Currency of the product
         :param: unlimited: Set true if the product has unlimited stock,
         :param: quantity: Quantity of the product in stock Use if unlimited is false
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert bool to string
         unlimited = self._convert_to_string(unlimited)
 
         data = {
             "name": name,
@@ -49,72 +50,72 @@
             "unlimited": unlimited,
             "quantity": quantity,
         }
         return await self._post_request("/product", data=data)
 
     async def list_products(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all the products
 
         :param: per_page: Number of records to return
         :param: page:  number to return
         :param: from_date: A timestamp from which to start listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
         :param: to_date: A timestamp from which to start listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to strings
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
         return await self._get_request("/product", params=params)
 
-    async def fetch_product(self, product_id: str) -> dict:
+    async def fetch_product(self, product_id: str) -> Response:
         """
         Get details of a product
 
         :param: product_id: ID or Code of the product
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request(f"/product/{product_id}")
 
     async def update_product(
             self,
             product_id: str,
             name: str,
             description: str,
             amount: int,
             currency: str,
-            unlimited: Optional[bool] = None,
-            quantity: Optional[int] = None,
-    ) -> dict:
+            unlimited: Optional[Union[bool, None]] = True,
+            quantity: Optional[Union[int, None]] = None,
+    ) -> Response:
         """
         Update a product detail
 
         :param: product_id: ID or Code of the product
         :param: name: Name of the product
         :param: description: Description of the product
         :param: amount: Price of the product
         :param: currency: Currency of the product
         :param: unlimited: Set true if the product has unlimited stock,
         :param: quantity: Quantity of the product in stock Use if unlimited is false
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert bool to string
         unlimited = self._convert_to_string(unlimited)
 
         data = {
             "name": name,
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/arefund.py` & `paystackease-1.0.0/paystackease/async_apis/arefund.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,74 +1,76 @@
 """
 Wrapper for Asynchronous Paystack Refund API
 
 The Refunds API allows you to create and manage transaction refunds.
 """
 
 from datetime import date
-from typing import Optional
+from typing import Optional, Union
 from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import Currency
 
 
 class AsyncRefundClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Refund API
     Reference: https://paystack.com/docs/api/refund/
     """
 
     async def create_refund(
             self,
             transaction_ref_or_id: str,
-            amount: Optional[int] = None,
-            currency: Optional[str] = None,
-            customer_note: Optional[str] = None,
-            merchant_note: Optional[str] = None,
-    ) -> dict:
+            amount: Optional[Union[int, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            customer_note: Optional[Union[str, None]] = None,
+            merchant_note: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Create a refund
 
         :param: transaction_ref_or_id: The transaction id or reference to fetch
         :param: amount: The amount to refund
         :param: currency: The currency to refund { Currency.value.value }
         :param: customer_note: The customer note or reason
         :param: merchant_note: The merchant note or reason
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "transaction": transaction_ref_or_id,
             "amount": amount,
             "currency": currency,
             "customer_note": customer_note,
             "merchant_note": merchant_note,
         }
         return await self._post_request("/refund", data=data)
 
     async def list_refunds(
             self,
-            reference: Optional[str] = None,
-            currency: Optional[str] = None,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            reference: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List refunds
 
         :param: reference: The transaction reference to fetch for the refund
         :param: currency: The currency to refund
         :param: per_page
         :param: page
         :param: from_date: A timestamp at which to stop listing refund
         :param: to_date: A timestamp at which to stop listing refund
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
 
         note::
 
             Date time format: 2016-09-21
         """
 
         # convert date to string
@@ -81,17 +83,17 @@
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
         return await self._get_request("/refund", params=params)
 
-    async def fetch_refund(self, reference: str) -> dict:
+    async def fetch_refund(self, reference: str) -> Response:
         """
         Fetch a refund
 
         :param: reference: The transaction reference to fetch for the refund
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request(f"/refund/{reference}")
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/asettlements.py` & `paystackease-1.0.0/paystackease/async_apis/asettlements.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 """
 Wrapper for Asynchronous Paystack Settlements API
 
 The Settlements API allows you to gain insights into payouts made by Paystack to your bank account.
 """
 
 from datetime import date
-from typing import Optional
+from typing import Optional, Union
+from paystackease._utils import Response
 from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease.helpers.tool_kit import STATUS
 
 
 class AsyncSettlementClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Settlement API
     Reference: https://paystack.com/docs/api/settlement/
     """
 
     async def list_settlements(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            status: Optional[str] = None,
-            subaccount: Optional[str] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            status: Optional[Union[STATUS, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List settlements made to your settlement accounts
 
         :param: per_page: The number of records to return per page.
         :param: page: the number to retrieve.
         :param: status: Value can be one of success, processing, pending or failed.
         :param: subaccount:
         :param: from_date: A timestamp from which to start listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
         :param: to_date: A timestamp from which to start listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
@@ -51,30 +53,30 @@
             "to": to_date,
         }
         return await self._get_request("/settlement", params=params)
 
     async def list_settlement_transactions(
             self,
             settlement_id: int,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         Get the transactions that make up a particular settlement
 
         :param: settlement_id: The id of the settlement.
         :param: per_page: The number of records to return per page.
         :param: page: the number to retrieve.
         :param: from_date: A timestamp from which to start listing settlements
         :param: to_date: A timestamp from which to start listing settlements
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
 
         note::
 
             Date and time format: 2016-09-24T00:00:05.000Z, 2016-09-21
 
         """
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/asubaccounts.py` & `paystackease-1.0.0/paystackease/apis/subaccounts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,83 @@
 """
-Wrapper for Asynchronous Paystack SubAccounts API
+Wrapper for Paystack SubAccounts API
 
 The Subaccounts API allows you to create and manage subaccounts on your integration.
 Subaccounts can be used to split payment between two accounts (your main account and a subaccount).
 """
 
 from datetime import date
-from typing import Optional, Dict, List, Any
-from paystackease._abase import AsyncPayStackBaseClientAPI
+from typing import Optional, Dict, List, Any, Union
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import SettlementSchedule
+from paystackease._base import PayStackBaseClientAPI
 
 
-class AsyncSubAccountClientAPI(AsyncPayStackBaseClientAPI):
+class SubAccountClientAPI(PayStackBaseClientAPI):
     """
     Paystack SubAccount API
     Reference: https://paystack.com/docs/api/subaccount/
     """
 
-    async def create_subaccount(
+    def create_subaccount(
             self,
             business_name: str,
             settlement_bank: str,
             account_number: str,
             percentage_charge: float,
             description: str,
-            primary_contact_email: Optional[str] = None,
-            primary_contact_name: Optional[str] = None,
-            primary_contact_phone: Optional[str] = None,
-            metadata: Optional[Dict[str, List[Dict[str, Any]]]] = None,
-    ) -> dict:
+            primary_contact_email: Optional[Union[str, None]] = None,
+            primary_contact_name: Optional[Union[str, None]] = None,
+            primary_contact_phone: Optional[Union[str, None]] = None,
+            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
+    ) -> Response:
         """
         Create a subaccount
 
         :param: business_name: The business name of the subaccount.
         :param: settlement_bank: Bank Code for the bank
         :param: account_number: The account number of the subaccount.
         :param: percentage_charge: The percentage charge receives from each payment made to the subaccount
         :param: description: The description of the subaccount.
         :param: primary_contact_email: A contact email for the subaccount
         :param: primary_contact_name: A name for the contact person for this subaccount
         :param: primary_contact_phone: A phone number to call for this subaccount
         :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "business_name": business_name,
             "settlement_bank": settlement_bank,
             "account_number": account_number,
             "percentage_charge": percentage_charge,
             "description": description,
             "primary_contact_email": primary_contact_email,
             "primary_contact_name": primary_contact_name,
             "primary_contact_phone": primary_contact_phone,
             "metadata": metadata,
         }
-        return await self._post_request("/subaccount", data=data)
+        return self._post_request("/subaccount", data=data)
 
-    async def update_subaccount(
+    def update_subaccount(
             self,
             id_or_code: str,
             business_name: str,
             settlement_bank: str,
             account_number: str,
-            active: Optional[bool] = None,
-            percentage_charge: Optional[float] = None,
-            description: Optional[str] = None,
-            primary_contact_email: Optional[str] = None,
-            primary_contact_name: Optional[str] = None,
-            primary_contact_phone: Optional[str] = None,
-            settlement_schedule: Optional[str] = None,
-            metadata: Optional[Dict[str, List[Dict[str, Any]]]] = None,
-    ) -> dict:
+            active: Optional[Union[bool, None]] = True,
+            percentage_charge: Optional[Union[float, None]] = None,
+            description: Optional[Union[str, None]] = None,
+            primary_contact_email: Optional[Union[str, None]] = None,
+            primary_contact_name: Optional[Union[str, None]] = None,
+            primary_contact_phone: Optional[Union[str, None]] = None,
+            settlement_schedule: Optional[Union[SettlementSchedule, None]] = SettlementSchedule.AUTO.value,
+            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
+    ) -> Response:
         """
         Update a subaccount
 
         :param: id_or_code: The id or code of the subaccount.
         :param: business_name: The business name of the subaccount.
         :param: settlement_bank: The settlement bank of the subaccount.
         :param: account_number
@@ -85,20 +87,20 @@
         :param: primary_contact_email
         :param: primary_contact_name
         :param: primary_contact_phone
         :param: settlement_schedule: Values: [ auto, weekly, `monthly`, `manual` ].
 
         note::
             Auto means payout is T+1
-            Manual means payout to the subaccount should only be made when requested. async defaults to auto
+            Manual means payout to the subaccount should only be made when requested. Defaults to auto
 
         :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert bool to string
         active = self._convert_to_string(active)
 
         data = {
             "business_name": business_name,
@@ -109,45 +111,45 @@
             "description": description,
             "primary_contact_email": primary_contact_email,
             "primary_contact_name": primary_contact_name,
             "primary_contact_phone": primary_contact_phone,
             "settlement_schedule": settlement_schedule,
             "metadata": metadata,
         }
-        return await self._put_request(f"/subaccount/{id_or_code}", data=data)
+        return self._put_request(f"/subaccount/{id_or_code}", data=data)
 
-    async def list_subaccounts(
+    def list_subaccounts(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all subaccounts
 
         :param: per_page: The number of records to return per page.
         :param: page: The number to retrieve.
         :param: from_date:
         :param: to_date:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return await self._get_request("/subaccount", params=params)
+        return self._get_request("/subaccount", params=params)
 
-    async def fetch_subaccount(self, id_or_code: str) -> dict:
+    def fetch_subaccount(self, id_or_code: str) -> Response:
         """
         Fetch details of a specific subaccount
 
         :param: id_or_code: The id or code of the subaccount.
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._get_request(f"/subaccount/{id_or_code}")
+        return self._get_request(f"/subaccount/{id_or_code}")
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/asubscriptions.py` & `paystackease-1.0.0/paystackease/async_apis/asubscriptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 """
 Wrapper for Paystack Subscriptions API
 
 The Subscriptions API allows you to create and manage recurring payment on your integration.
 """
 
 from datetime import date
-from typing import Optional
+from typing import Optional, Union
+from paystackease._utils import Response
 from paystackease._abase import AsyncPayStackBaseClientAPI
 
 
 class AsyncSubscriptionClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Subscription API
     Reference: https://paystack.com/docs/api/subscription/
     """
 
     async def create_subscription(
             self,
             customer: str,
             plan_code: str,
             authorization: str,
-            start_date: Optional[date] = None,
-    ) -> dict:
+            start_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         Create a subscription
 
         :param: customer: Email or Code of the customer
         :param: plan_code: Code of the plan
         :param: authorization: Code of the authorization
         :param: start_date: Start date of the subscription
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         start_date = self._convert_to_string(start_date)
 
         data = {
             "customer": customer,
@@ -43,89 +44,89 @@
             "authorization": authorization,
             "start_date": start_date,
         }
         return await self._post_request("/subscription", data=data)
 
     async def list_subscriptions(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            customer: Optional[int] = None,
-            plan_code: Optional[int] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[int, None]] = None,
+            plan_code: Optional[Union[int, None]] = None,
+    ) -> Response:
         """
         List all the subscriptions
 
         :param: per_page: Number of records to return per page.
         :param: page: THe number to return
         :param: customer:
         :param: plan_code:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         params = {
             "perPage": per_page,
             "page": page,
             "customer": customer,
             "plan": plan_code,
         }
         return await self._get_request("/subscription", params=params)
 
-    async def fetch_subscription(self, id_or_code: str) -> dict:
+    async def fetch_subscription(self, id_or_code: str) -> Response:
         """
         Get details of a subscription
 
         :param: id_or_code: ID or Code of the subscription
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request(f"/subscription/{id_or_code}")
 
-    async def enable_subscription(self, subscription_code: str, token: str) -> dict:
+    async def enable_subscription(self, subscription_code: str, token: str) -> Response:
         """
         Enable a subscription
 
         :param: subscription_code: Code of the subscription
         :param: token: Email token of the customer
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"code": subscription_code, "token": token}
         return await self._post_request("/subscription/enable", data=data)
 
-    async def disable_subscription(self, subscription_code: str, token: str) -> dict:
+    async def disable_subscription(self, subscription_code: str, token: str) -> Response:
         """
         Disable a subscription
 
         :param: subscription_code: Code of the subscription
         :param: token: Email token of the customer
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"code": subscription_code, "token": token}
         return await self._post_request("/subscription/disable", data=data)
 
-    async def generate_update_subscription(self, subscription_code: str) -> dict:
+    async def generate_update_subscription(self, subscription_code: str) -> Response:
         """
         Generate a link for updating the card on subscription
 
         :param: subscription_code: Code of the subscription
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._post_request(f"/subscription/{subscription_code}/manage/link")
 
-    async def send_update_subscription_link(self, subscription_code: str) -> dict:
+    async def send_update_subscription_link(self, subscription_code: str) -> Response:
         """
         Email a customer a link for updating the card on their subscription
 
         :param: subscription_code: Code of the subscription
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._post_request(f"/subscription/{subscription_code}/manage/email")
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/aterminal.py` & `paystackease-1.0.0/paystackease/async_apis/aterminal.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,133 +1,138 @@
 """
 Wrapper for Asynchronous Paystack Terminal APIs
 
 The Terminal API allows you to build delightful in-person payment experiences.
 """
 
-from typing import Optional, Dict
+from typing import Optional, Dict, Union
+from paystackease._utils import Response
 from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease.helpers.tool_kit import EventAction, EventType
 
 
 class AsyncTerminalClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Terminal API
     Reference: https://paystack.com/docs/api/terminal/
     """
 
     async def send_event(
             self,
             terminal_id: str,
-            event_type: str,
-            terminal_action: str,
+            event_type: EventType,
+            terminal_action: EventAction,
             data_object: Dict[str, str],
-    ) -> dict:
+    ) -> Response:
         """
         Send an event from your application to the Paystack Terminal
 
         :param: terminal_id: The terminal iD the event is sent to
         :param: event_type: The type of event to send. We currently support [ invoice | transaction ]
         :param: terminal_action: The action to perform on the terminal
                                 [invoice type]:the action can either be [ process || view ]
                                 [transaction type], the action can either be [ process || print ].
         :param: data_object: parameters needed to perform the specified action.
                             [invoice type]: you need to pass {id: invoice_id, reference: offline_reference}.
                             [transaction type], you can pass {id: transaction_id}
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"type": event_type, "action": terminal_action, "data": data_object}
         return await self._post_request(f"/terminal/{terminal_id}/event", data=data)
 
-    async def commission_terminal(self, serial_number: str) -> dict:
+    async def commission_terminal(self, serial_number: str) -> Response:
         """
         Activate debug device by linking it to your integration
 
         :param: serial_number: The serial number of the device
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"serial_number": serial_number}
         return await self._post_request("/terminal/commission_device", data=data)
 
-    async def decommission_terminal(self, serial_number: str) -> dict:
+    async def decommission_terminal(self, serial_number: str) -> Response:
         """
         Deactivate debug device by unlinking it from your integration
 
         :param: serial_number: The serial number of the device
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"serial_number": serial_number}
         return await self._post_request("/terminal/decommission_device", data=data)
 
     async def update_terminal(
             self, terminal_id: str, terminal_name: str, terminal_address: str
-    ) -> dict:
+    ) -> Response:
         """
         Update details of a terminal
 
         :param: terminal_id: The terminal iD the event is sent to
         :param: terminal_name: Name of the terminal
         :param: terminal_address: Address of the terminal
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"name": terminal_name, "address": terminal_address}
         return await self._put_request(f"/terminal/{terminal_id}", data=data)
 
-    async def fetch_event_status(self, terminal_id: str, event_id: str) -> dict:
+    async def fetch_event_status(self, terminal_id: str, event_id: str) -> Response:
         """
         Fetch details of a specific event status sent to the terminal
 
         :param: terminal_id: iD of the terminal the event is sent to
         :param: event_id: The event id sent to the terminal
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request(f"/terminal/{terminal_id}/event/{event_id}")
 
-    async def fetch_terminal_status(self, terminal_id: str) -> dict:
+    async def fetch_terminal_status(self, terminal_id: str) -> Response:
         """
         Fetch the availability of a terminal before sending an event
 
         :param: terminal_id: The terminal iD the event is sent to
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request(f"/terminal/{terminal_id}/presence")
 
     async def list_terminals(
             self,
-            per_page: int,
-            next_cursor: Optional[str] = None,
-            previous_cursor: Optional[str] = None,
-    ) -> dict:
+            per_page: int = 50,
+            next_cursor: Optional[Union[bool, None]] = True,
+            previous_cursor: Optional[Union[bool, None]] = True,
+    ) -> Response:
         """
         List the Terminals available on your integration
 
         :param: per_page: The number of records to return. async default value is 50
         :param: next_cursor:
         :param: previous_cursor:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
+        # convert toi strings
+        next_cursor = self._convert_to_string(next_cursor)
+        previous_cursor = self._convert_to_string(previous_cursor)
         params = {"perPage": per_page, "next": next_cursor, "previous": previous_cursor}
         return await self._get_request("/terminal", params=params)
 
-    async def fetch_terminal(self, terminal_id: str) -> dict:
+    async def fetch_terminal(self, terminal_id: str) -> Response:
         """
         Get the details of a terminal
 
         :param: terminal_id: The terminal iD the event is sent to
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request(f"/terminal/timeline/{terminal_id}")
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/atransaction_splits.py` & `paystackease-1.0.0/paystackease/apis/transaction_splits.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,143 +1,144 @@
 """
-Wrapper for Asynchronous Paystack Transaction Splits APIs
+Wrapper for Paystack Transaction Splits APIs
 
 The Transaction Splits API enables merchants split the settlement for a transaction
 across their payout account, and one or more subaccounts.
 """
 
 from datetime import date
-from typing import Optional, List, Dict, Any
-from paystackease._abase import AsyncPayStackBaseClientAPI
+from typing import Optional, List, Dict, Any, Union
+from paystackease._utils import Response
+from paystackease._base import PayStackBaseClientAPI
 
 
-class AsyncTransactionSplitClientAPI(AsyncPayStackBaseClientAPI):
+class TransactionSplitClientAPI(PayStackBaseClientAPI):
     """
     Paystack Transaction Split API
     Reference: https://paystack.com/docs/api/split/
     """
 
-    async def create_split(
+    def create_split(
             self,
             transaction_split_name: str,
             transaction_split_type: str,
             currency: str,
             subaccounts: List[Dict[str, Any]],
             bearer_type: str,
             bearer_subaccount: str,
-    ) -> dict:
+    ) -> Response:
         """
         Create a split payment on your integration
 
         :param: transaction_split_name: Name of the transaction split
         :param: transaction_split_type: The type of transaction split you want to create [ percentage | flat ]
         :param: currency: [ Currency.value.value ]
         :param: subaccounts: A list of object containing subaccount code and number of shares
                             [{subaccount: ‘ACT_xxxxxxxxxx’, share: xxx},{...}]
         :param: bearer_type: Any of subaccount | account | all-proportional | all
         :param: bearer_subaccount: Subaccount code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "name": transaction_split_name,
             "type": transaction_split_type,
             "currency": currency,
             "subaccounts": subaccounts,
             "bearer_type": bearer_type,
             "bearer_subaccount": bearer_subaccount,
         }
-        return await self._post_request("/split", data=data)
+        return self._post_request("/split", data=data)
 
-    async def add_or_update_subaccount_split(
+    def add_or_update_subaccount_split(
             self, split_id: str, subaccount: str, transaction_share: int
-    ) -> dict:
+    ) -> Response:
         """
         Add a Subaccount to a Transaction Split, or update the share of
         an existing Subaccount in a Transaction Split
 
         :param: split_id: The split ID
         :param: subaccount: The subaccount code
         :param: transaction_share: The number of shares
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"subaccount": subaccount, "share": transaction_share}
-        return await self._post_request(f"/split/{split_id}/subaccount/add", data=data)
+        return self._post_request(f"/split/{split_id}/subaccount/add", data=data)
 
-    async def remove_sub_account_split(self, split_id: str, subaccount: str) -> dict:
+    def remove_sub_account_split(self, split_id: str, subaccount: str) -> Response:
         """
         Remove a Sub Account from a transaction split
 
         :param: split_id: The split ID
         :param: subaccount: The subaccount code
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"subaccount": subaccount}
-        return await self._post_request(f"/split/{split_id}/subaccount/remove", data=data)
+        return self._post_request(f"/split/{split_id}/subaccount/remove", data=data)
 
-    async def update_split(
+    def update_split(
             self,
             split_id: str,
             transaction_split_name: str,
             active: bool,
-            bearer_type: Optional[str] = None,
-            bearer_subaccount: Optional[str] = None,
-    ) -> dict:
+            bearer_type: Optional[Union[str, None]] = None,
+            bearer_subaccount: Optional[Union[str, None]] = None,
+    ) -> Response:
         """
         Update a specific transaction split details
 
         :param: split_id: The split ID
         :param: transaction_split_name: Name of the transaction split
         :param: active: True or False
         :param: bearer_type:
         :param: bearer_subaccount:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert bool to string
         active = self._convert_to_string(active)
 
         data = {
             "name": transaction_split_name,
             "active": active,
             "bearer_type": bearer_type,
             "bearer_subaccount": bearer_subaccount,
         }
-        return await self._put_request(f"/split/{split_id}", data=data)
+        return self._put_request(f"/split/{split_id}", data=data)
 
-    async def list_split(
+    def list_split(
             self,
-            split_name: Optional[str] = None,
-            active: Optional[bool] = None,
-            sort_by: Optional[str] = None,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            split_name: Optional[Union[str, None]] = None,
+            active: Optional[Union[bool, None]] = True,
+            sort_by: Optional[Union[str, None]] = None,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all the transaction splits
 
         :param: split_name: Name of the transaction split
         :param: active: True or False
-        :param: sort_by: Sort by name, async defaults to createdAt date,
+        :param: sort_by: Sort by name, defaults to createdAt date,
         :param: per_page:
         :param: page:
         :param: from_date:
         :param: to_date:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date and bool to string
         active = self._convert_to_string(active)
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
@@ -146,19 +147,19 @@
             "active": active,
             "sort_by": sort_by,
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
-        return await self._get_request("/split", params=params)
+        return self._get_request("/split", params=params)
 
-    async def fetch_split(self, split_id: str) -> dict:
+    def fetch_split(self, split_id: str) -> Response:
         """
         Fetch details of a specific transaction split
 
         :param: split_id: The split ID
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._get_request(f"/split/{split_id}")
+        return self._get_request(f"/split/{split_id}")
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/atransactions.py` & `paystackease-1.0.0/paystackease/apis/transactions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 """
-Wrapper for Asynchronous Paystack Transactions API
+Wrapper for Paystack Transactions API
 
 The Transactions API allows you to create and manage payments on your integration.
 """
 
 from datetime import date
+from typing import List, Optional, Dict, Any, Union
+from paystackease.helpers.tool_kit import Channels, Currency, Bearer, TransactionStatus
+from paystackease._base import PayStackBaseClientAPI
+from paystackease._utils import Response
 
-from typing import List, Optional, Dict, Any
 
-from paystackease._abase import AsyncPayStackBaseClientAPI
-
-
-class AsyncTransactionClientAPI(AsyncPayStackBaseClientAPI):
+class TransactionClientAPI(PayStackBaseClientAPI):
     """
     Paystack Transaction API
     Reference: https://paystack.com/docs/api/transaction/
     """
 
-    async def initialize(
+    def initialize(
             self,
             email: str,
             amount: int,
-            currency: Optional[str] = None,
-            reference: Optional[str] = None,
-            callback_url: Optional[str] = None,
-            plan: Optional[str] = None,
-            invoice_limit: Optional[int] = None,
-            channels: Optional[List[str]] = None,
-            split_code: Optional[str] = None,
-            subaccount: Optional[str] = None,
-            transaction_charge: Optional[int] = None,
-            bearer: Optional[str] = None,
-            metadata: Optional[Dict[str, str]] = None,
-    ) -> dict:
+            currency: Optional[Union[Currency, None]] = Currency.NGN.value,
+            reference: Optional[Union[str, None]] = None,
+            callback_url: Optional[Union[str, None]] = None,
+            plan: Optional[Union[str, None]] = None,
+            invoice_limit: Optional[Union[int, None]] = None,
+            channels: Optional[Union[List[Channels], None]] = None,
+            split_code: Optional[Union[str, None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
+            transaction_charge: Optional[Union[int, None]] = None,
+            bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
+            metadata: Optional[Union[Dict[str, Any], None]] = None,
+    ) -> Response:
         """
         Initialize a transaction
 
         :param: email:
         :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
                         Use convert_currency() to convert to subunit
         :param: currency:  # Currency.value.value
         :param: reference:
         :param: callback_url: # Use this to override the callback url provided on the  dashboard
-                                # https://example.com/callback
-        :param: plan:  # If transaction is to create a subscription to a preasync defined plan, provide plan code here.
+                            # https://example.com/callback
+        :param: plan:  # If transaction is to create a subscription to a predefined plan, provide plan code here.
         :param: invoice_limit:  # Number of times to charge customer during subscription to plan
         :param: channels:  # [Channels.value.value, Channels.value.value, ...]
         :param: split_code:  # The split code of the transaction split. e.g. SPL_98WF13Eb3w
         :param: subaccount:  # The code for the subaccount that owns the payment. e.g. ACCT_8f4s1eq7ml6rlzj
         :param: transaction_charge: # An amount used to override the split configuration for a
                                     # single split payment
         :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
         :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "email": email,
             "amount": amount,
             "currency": currency,
             "reference": reference,
             "callback_url": callback_url,
@@ -67,30 +67,30 @@
             "channels": channels,
             "split_code": split_code,
             "subaccount": subaccount,
             "transaction_charge": transaction_charge,
             "bearer": bearer,
             "metadata": metadata,
         }
-        return await self._post_request("/transaction/initialize", data=data)
+        return self._post_request("/transaction/initialize", data=data)
 
-    async def charge_authorization(
+    def charge_authorization(
             self,
             email: str,
             amount: int,
             authorization_code: str,
-            reference: Optional[str] = None,
-            currency: Optional[str] = None,
-            channels: Optional[List[str]] = None,
-            subaccount: Optional[str] = None,
+            reference: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            channels: Optional[Union[List[Channels], None]] = None,
+            subaccount: Optional[Union[str, None]] = None,
             transaction_charge: Optional[int] = None,
-            bearer: Optional[str] = None,
-            queue: Optional[bool] = None,
-            metadata: Optional[Dict[str, List[Dict[str, Any]]]] = None,
-    ) -> dict:
+            bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
+            queue: Optional[Union[bool, None]] = True,
+            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
+    ) -> Response:
         """
         Charge an authorization transaction
 
         :param: email:
         :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
                         Use convert_currency() to convert to subunit
         :param: authorization_code:  # value = AUTH_1234234WRFW
@@ -100,15 +100,15 @@
         :param: subaccount:  # value = ACCT_8f4s1eq7ml6rlzj
         :param: transaction_charge:
         :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
         :param: queue:  # If set to true, the transaction will be queued for processing
         :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert bool to string
         queue = self._convert_to_string(queue)
 
         data = {
             "email": email,
@@ -119,74 +119,74 @@
             "channels": channels,
             "subaccount": subaccount,
             "transaction_charge": transaction_charge,
             "bearer": bearer,
             "queue": queue,
             "metadata": metadata,
         }
-        return await self._post_request("/transaction/charge_authorization", data=data)
+        return self._post_request("/transaction/charge_authorization", data=data)
 
-    async def partial_debit(
+    def partial_debit(
             self,
             email: str,
             authorization_code: str,
             amount: int,
             currency: str,
-            reference: Optional[str] = None,
-            at_least: Optional[int] = None,
-    ) -> dict:
+            reference: Optional[Union[str, None]] = None,
+            at_least: Optional[Union[int, None]] = None,
+    ) -> Response:
         """
         Charge a partial debit transaction
 
         :param: email:
         :param: authorization_code:  # value = AUTH_1234234WRFW
         :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
                         Use convert_currency() to convert to subunit
         :param: currency:  # value = Currency.value.value
         :param: reference:  # Unique transaction reference.
         :param: at_least:  # Minimum amount to charge
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "email": email,
             "authorization_code": authorization_code,
             "amount": amount,
             "currency": currency,
             "reference": reference,
             "at_least": at_least,
         }
-        return await self._post_request("/transaction/partial_debit", data=data)
+        return self._post_request("/transaction/partial_debit", data=data)
 
-    async def list_transactions(
+    def list_transactions(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            customer: Optional[int] = None,
-            terminal_id: Optional[str] = None,
-            amount: Optional[int] = None,
-            status: Optional[str] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[int, None]] = None,
+            terminal_id: Optional[Union[str, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            status: Optional[Union[TransactionStatus, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         List all transactions
 
         :param: per_page:  # Specify how many records you want to retrieve per page.
         :param: page:  # Specify a page number to retrieve
         :param: customer:  # Specify an ID for the customer whose transactions you want to retrieve
         :param: terminal_id:  # Specify an ID for the terminal whose transactions you want to retrieve
         :param: amount:  # Specify an amount for the transactions you want to retrieve
         :param: status:  # Specify a status for the transactions you want to retrieve [success, failed, abandoned]
         :param: from_date:  # A timestamp from which to start listing transaction 2016-09-24T00:00:05.000Z, 2016-09-21
         :param: to_date:  # A timestamp at which to stop listing transaction 2016-09-24T00:00:05.000Z
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
@@ -195,94 +195,94 @@
             "customer": customer,
             "terminalid": terminal_id,
             "amount": amount,
             "status": status,
             "from": from_date,
             "to": to_date,
         }
-        return await self._get_request("/transaction", params=params)
+        return self._get_request("/transaction", params=params)
 
-    async def verify_transaction(self, reference: str) -> dict:
+    def verify_transaction(self, reference: str) -> Response:
         """
         Verify a transaction by reference
 
         :param: reference:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._get_request(f"/transaction/verify/{reference}")
+        return self._get_request(f"/transaction/verify/{reference}")
 
-    async def fetch_transaction(self, transaction_id: int) -> dict:
+    def fetch_transaction(self, transaction_id: int) -> Response:
         """
         Fetch details of a specific transaction
 
         :param: transaction_id:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._get_request(f"/transaction/{transaction_id}")
+        return self._get_request(f"/transaction/{transaction_id}")
 
-    async def transaction_timeline(self, id_or_reference: str) -> dict:
+    def transaction_timeline(self, id_or_reference: str) -> Response:
         """
         Get the timeline of a transaction
 
         :param: id_or_reference:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._get_request(f"/transaction/timeline/{id_or_reference}")
+        return self._get_request(f"/transaction/timeline/{id_or_reference}")
 
-    async def transaction_totals(
+    def transaction_totals(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         Get totals of all transactions
 
         :param: per_page:
         :param: page:
         :param: from_date:
         :param: to_date:
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
-        return await self._get_request("/transaction/totals", params=params)
+        return self._get_request("/transaction/totals", params=params)
 
-    async def export_transactions(
+    def export_transactions(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            customer: Optional[int] = None,
-            currency: Optional[str] = None,
-            amount: Optional[int] = None,
-            status: Optional[str] = None,
-            settled: Optional[bool] = None,
-            settlement: Optional[int] = None,
-            payment_page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer: Optional[Union[int, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            amount: Optional[Union[int, None]] = None,
+            status: Optional[Union[TransactionStatus, None]] = None,
+            settled: Optional[Union[bool, None]] = True,
+            settlement: Optional[Union[int, None]] = None,
+            payment_page: Optional[Union[int, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
         Export transactions
 
         :param: per_page:
         :param: page:
         :param: customer:
         :param: currency:  # value = Currency.value.value
@@ -291,15 +291,15 @@
         :param: settled:  # true or false
         :param: settlement:
         :param: payment_page:
         :param: from_date:  # 2016-09-24T00:00:05.000Z
         :param: to_date:  # 2016-09-24T00:00:05.000Z
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
         # convert date and bool to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
         settled = self._convert_to_string(settled)
 
@@ -312,8 +312,8 @@
             "status": status,
             "settled": settled,
             "settlement": settlement,
             "payment_page": payment_page,
             "from": from_date,
             "to": to_date,
         }
-        return await self._get_request("/transaction/export", params=params)
+        return self._get_request("/transaction/export", params=params)
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/atransfer_recipients.py` & `paystackease-1.0.0/paystackease/async_apis/atransfers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,136 @@
 """
-Wrapper for Asynchronous Paystack Transfer Recipient APIs
+Wrapper for Asynchronous Paystack Transfers APIs
 
-The Transfer Recipients API allows you to create and manage beneficiaries that you send money to.
+The Transfers API allows you to automate sending money to your customers.
 """
 
 from datetime import date
-from typing import Optional, Dict, List
+from typing import Optional, List, Dict, Any, Union
+
+from paystackease._utils import Response
+from paystackease.helpers.tool_kit import Currency
 from paystackease._abase import AsyncPayStackBaseClientAPI
 
 
-class AsyncTransferRecipientsClientAPI(AsyncPayStackBaseClientAPI):
+class AsyncTransfersClientAPI(AsyncPayStackBaseClientAPI):
     """
-    Paystack Transfer Recipients API
-    Reference: https://paystack.com/docs/api/transfer-recipient/
+    Paystack Transfers API
+    Reference: https://paystack.com/docs/api/transfer/
     """
 
-    async def create_transfer_recipients(
+    async def initiate_transfer(
             self,
-            recipient_type: str,
-            recipient_name: str,
-            account_number: str,
-            bank_code: str,
-            description: Optional[str] = None,
-            currency: Optional[str] = None,
-            authorization_code: Optional[str] = None,
-            metadata: Optional[Dict[str, str]] = None,
-    ) -> dict:
-        """
-        Create a transfer recipient
-
-        :param: recipient_type: The type of transfer recipient:[ nuban | ghipss | mobile_money | basa ]
-        :param: recipient_name: The name of the transfer recipient according to their account registration
-        :param: account_number: transfer recipient's account number.
-                                Required for all recipient types except authorization
-        :param: bank_code: transfer recipient's bank code. Required for all recipient types except authorization
-        :param: description:
-        :param: currency: transfer recipient's currency. [Currency.value.value ]
-        :param: authorization_code: transfer recipient's authorization code from previous transaction
-        :param: metadata: transfer recipient's metadata
+            transfer_source: str,
+            amount: int,
+            transfer_recipient: str,
+            reason: Optional[Union[str, None]] = None,
+            currency: Optional[Union[Currency, None]] = None,
+            reference: Optional[Union[str, None]] = None,
+    ) -> Response:
+        """
+        Initiate a transfer. Upgrade your business to a Registered Business to use
+
+        :param: transfer_source: Where should we transfer from? Only balance for now
+        :param: amount: Amount to transfer in kobo if currency is NGN and pesewas if currency is GHS.
+        :param: transfer_recipient: The code of the recipient
+        :param: currency: The currency of the transfer
+        :param: reason: The reason for the transfer
+        :param: reference: If specified, the field should be a unique identifier (in lowercase) for the object.
+                            Only -,_ and alphanumeric characters allowed.
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
-            "type": recipient_type,
-            "name": recipient_name,
-            "account_number": account_number,
-            "bank_code": bank_code,
-            "description": description,
+            "source": transfer_source,
+            "amount": amount,
+            "recipient": transfer_recipient,
+            "reason": reason,
             "currency": currency,
-            "authorization_code": authorization_code,
-            "metadata": metadata,
+            "reference": reference,
         }
-        return await self._post_request("/transferrecipient", data=data)
+        return await self._post_request("/transfer", data=data)
+
+    async def finalize_transfer(self, transfer_code: str, otp: str) -> Response:
+        """
+        Finalize an initiated transfer
+
+        :param: transfer_code: The code of the transfer to finalize
+        :param: otp: The OTP sent to the business phone to verify transfer
 
-    async def bulk_create_transfer_recipient(self, batch: List[Dict[str, str]]) -> dict:
+        :return: The response from the API
+        :rtype: Response object
+        """
+        data = {"transfer_code": transfer_code, "otp": otp}
+        return await self._post_request("/transfer/finalize_transfer", data=data)
+
+    async def initiate_bulk_transfer(
+            self, transfer_source: str, transfers: List[Dict[str, Any]]
+    ) -> Response:
         """
-        Create multiple transfer recipients in batches.
+        Batch multiple transfers in a single request
 
-        :param: batch: A list of transfer recipient object
-                        keys [ { type, name, account_number, bank_code, currency etc. }]
+        :param: transfer_source: Where should we transfer from? Only balance for now
+        :param: transfers: A list of transfer objects keys [ { amount | recipient | reference | reason } ]
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        data = {"batch": batch}
-        return await self._post_request("/transferrecipient/bulk", data=data)
+        data = {"source": transfer_source, "transfers": transfers}
+        return await self._post_request("/transfer/bulk", data=data)
 
-    async def list_transfer_recipients(
+    async def list_transfers(
             self,
-            per_page: Optional[int] = None,
-            page: Optional[int] = None,
-            from_date: Optional[date] = None,
-            to_date: Optional[date] = None,
-    ) -> dict:
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            customer_id: Optional[Union[str, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> Response:
         """
-        List transfer recipients
+        List transfers
 
         :param: per_page: The number of records to return per page.
         :param: page: The page number to retrieve.
-        :param: from_date:
-        :param: to_date:
+        :param: customer_id
+        :param: from_date
+        :param: to_date
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
 
-        # convert date to strings
+        # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
-        params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return await self._get_request("/transferrecipient", params=params)
-
-    async def fetch_transfer_recipient(self, id_or_code: str) -> dict:
-        """
-        Fetch details of a transfer recipient
-
-        :param: id_or_code: The id or code of the transfer recipient
-
-        :return: The response from the API
-        :rtype: dict
-        """
-        return await self._get_request(f"/transferrecipient/{id_or_code}")
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "customer": customer_id,
+            "from": from_date,
+            "to": to_date,
+        }
+        return await self._get_request("/transfer", params=params)
 
-    async def update_transfer_recipient(
-            self,
-            id_or_code: str,
-            recipient_name: str,
-            recipient_email: Optional[str] = None,
-    ) -> dict:
+    async def fetch_transfer(self, id_or_code: str) -> Response:
         """
-        Update a transfer recipient
+        Get details of a transfer
 
-        :param: id_or_code: The id or code of the transfer recipient
-        :param: recipient_name: The name of the transfer recipient
-        :param: recipient_email: The email of the transfer recipient
+        :param: id_or_code: The id or code of the transfer
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        data = {"name": recipient_name, "email": recipient_email}
-        return await self._put_request(f"/transferrecipient/{id_or_code}", data=data)
+        return await self._get_request(f"/transfer/{id_or_code}")
 
-    async def delete_transfer_recipient(self, id_or_code: str) -> dict:
+    async def verify_transfer(self, reference: str) -> Response:
         """
-        Delete a transfer recipient
+        Verify a transfer
 
-        :param: id_or_code: The id or code of the transfer recipient
+        :param: reference: The reference of the transfer to verify
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
-        return await self._delete_request(f"/transferrecipient/{id_or_code}")
+        return await self._post_request(f"/transfer/verify/{reference}")
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/atransfers_control.py` & `paystackease-1.0.0/paystackease/async_apis/atransfers_control.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 """
 Wrapper for Asynchronous Paystack Transfer Control APIs
 
 The Transfers Control API allows you manage settings of your transfers.
 """
 
 from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
 
 
 class AsyncTransferControlClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Transfers Control API
     Reference: https://paystack.com/docs/api/transfer-control/
     """
 
-    async def check_balance(self) -> dict:
+    async def check_balance(self) -> Response:
         """
         Get the available balance
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request("/balance")
 
-    async def fetch_balance_ledger(self) -> dict:
+    async def fetch_balance_ledger(self) -> Response:
         """
         Fetch all pay-ins and pay-outs that occurred on your integration
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request("/balance/ledger")
 
-    async def resend_otp(self, transfer_code: str, reason: str) -> dict:
+    async def resend_otp(self, transfer_code: str, reason: str) -> Response:
         """
         Generates a new OTP and sends to customer in the event
         they are having trouble receiving one.
 
         :param: transfer_code: The code of the transfer to finalize
         :param: reason: Either resend_otp or transfer as the value of this field
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"transfer_code": transfer_code, "reason": reason}
         return await self._post_request("/transfer/resend_otp", data=data)
 
-    async def disable_otp(self) -> dict:
+    async def disable_otp(self) -> Response:
         """
         This is used in the event that you want to be able to
          complete transfers programmatically without use of OTPs
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._post_request("/transfer/disable_otp")
 
-    async def finalize_disable_otp(self, otp: str) -> dict:
+    async def finalize_disable_otp(self, otp: str) -> Response:
         """
         Finalize the request to disable OTP on your transfers.
 
         :param: otp: The OTP sent to the business phone to verify disabling of OTP
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {"otp": otp}
         return await self._post_request("/transfer/disable_otp_finalize", data=data)
 
-    async def enable_otp(self) -> dict:
+    async def enable_otp(self) -> Response:
         """
         This is used in the event that you want to stop
         being able to complete transfers programmatically with use of OTPs
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._post_request("/transfer/enable_otp")
```

### Comparing `paystackease-0.1.3/paystackease/async_apis/averification.py` & `paystackease-1.0.0/paystackease/async_apis/averification.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,77 @@
 """
 Wrapper for Asynchronous Paystack Verification APIs
 
 The Verification API allows you to perform KYC processes.
 """
 
 from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease._utils import Response
 
 
 class AsyncVerificationClientAPI(AsyncPayStackBaseClientAPI):
     """
     Paystack Verification API
     Reference: https://paystack.com/docs/api/verification/
     """
 
-    async def resolve_account(self, account_number: str, bank_code: str) -> dict:
+    async def resolve_account(self, account_number: str, bank_code: str) -> Response:
         """
         Confirm an account belongs to the right customer.
         This feature is available to business in Nigeria and Ghana.
 
         :param: account_number: The account number to verify
         :param: bank_code: The bank code to verify
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         params = {"account_number": account_number, "bank_code": bank_code}
         return await self._get_request("/bank/resolve", params=params)
 
     async def validate_account(
             self,
             account_name: str,
             account_number: str,
             account_type: str,
             bank_code: str,
             country_code: str,
             document_type: str,
             document_number: str,
-    ) -> dict:
+    ) -> Response:
         """
         Confirm the authenticity of a customer's account number before sending money.
         This feature is only available to businesses in South Africa.
 
         :param: account_name: The account name to validate: first and last name
         :param: account_number: The account number to validate
         :param: account_type: The account type to validate: personal or business
         :param: bank_code: The bank code to validate
         :param: country_code: The country code to validate
         :param: document_type: The customer's mode of identity:
                                 identityNumber, passportNumber or businessRegistrationNumber
         :param: document_number: The customer's document number
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         data = {
             "account_name": account_name,
             "account_number": account_number,
             "account_type": account_type,
             "bank_code": bank_code,
             "country_code": country_code,
             "document_type": document_type,
             "document_number": document_number,
         }
         return await self._post_request("/bank/validate", data=data)
 
-    async def resolve_card_bin(self, bin_code: str) -> dict:
+    async def resolve_card_bin(self, bin_code: str) -> Response:
         """
         Resolve a card BIN
 
         :param: bin_code: First 6 characters of card
 
         :return: The response from the API
-        :rtype: dict
+        :rtype: Response object
         """
         return await self._get_request(f"/decision/bin/{bin_code}")
```

### Comparing `paystackease-0.1.3/paystackease/helpers/convert.py` & `paystackease-1.0.0/paystackease/helpers/convert.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This holds function to convert to subunits in NGN, GHS, USD, ZAR and KES
 """
-
+from typing import Union
 from paystackease.helpers.tool_kit import Currency
 
 
-def convert_to_subunit(amount: int, currency: Currency) -> int:
+def convert_to_subunit(amount: int, currency: Union[Currency, None] = Currency.NGN) -> int:
     """
     Convert a subunit amount to a base amount
     :param amount:
     :param currency:
     :return:
     """
     subunit_multipliers = {
```

### Comparing `paystackease-0.1.3/paystackease/helpers/tool_kit.py` & `paystackease-1.0.0/paystackease/helpers/tool_kit.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 class AccountType(Enum):
     """Customer’s type of Account."""
 
     PERSONAL = "personal"
     BUSINESS = "business"
 
 
+class Bearer(Enum):
+    """Bearer supported by Paystack."""
+    ACCOUNT = "account"
+    SUB_ACCOUNT = "subaccount"
+
+
 class Currency(Enum):
     """Currencies supported by Paystack."""
 
     GHS = "GHS"
     KES = "KES"
     NGN = "NGN"
     USD = "USD"
@@ -30,27 +36,60 @@
     CARD = "card"
     ETF = "etf"
     MOBILE_MONEY = "mobile_money"
     QR = "qr"
     USSD = "ussd"
 
 
+class DisputeStatus(Enum):
+    """Dispute status."""
+    MERCHANT_FEEDBACK = "awaiting-merchant-feedback"
+    BANK_FEEDBACK = "awaiting-bank-feedback"
+    PENDING = "pending"
+    RESOLVED = "resolved"
+
+
 class DocumentType(Enum):
     """Customer’s mode of identity."""
 
     IDENTITY_NUMBER = "identityNumber"
     PASSPORT_NUMBER = "passportNumber"
     BUSINESS_REG_NUMBER = "businessRegistrationNumber"
 
 
+class DVABank(Enum):
+    """DVA_BANK supported by Paystack."""
+    WEMA_BANK = "wema-bank"
+    TITAN = "titan-paystack"
+
+
+class EFT(Enum):
+    """EFT supported by Paystack."""
+
+    OZOW = "ozow"
+
+
+class EventAction(Enum):
+    """Event action supported by Paystack."""
+    PROCESS = "process"
+    VIEW = "view"
+    PRINT = "print"
+
+
 class EventType(Enum):
     INVOICE = "invoice"
     TRANSACTION = "transaction"
 
 
+class GateWay(Enum):
+    """ Gateway supported bt Paystack"""
+    E_MANDATE = "emandate"
+    DIGITAL_BANK_MANDATE = "digitalbankmandate"
+
+
 class Interval(Enum):
     """Interval supported by Paystack."""
 
     DAILY = "daily"
     WEEKLY = "weekly"
     MONTHLY = "monthly"
     QUARTERLY = "quarterly"
@@ -65,14 +104,20 @@
 
     MTN = "mtn"
     AIRTEL_TIGO = "atl"
     VODAFONE = "vod"
     M_PESA = "mpesa"
 
 
+class PayMentRequestStatus(Enum):
+    """ Payment request status supported by Paystack"""
+    DRAFT = "draft"
+    PENDING = "pending"
+
+
 class PWT(Enum):
     """PWT supported by Paystack."""
 
     ACCOUNT_EXPIRES_AT = "account_expires_at"
 
 
 class QRCODE(Enum):
@@ -91,37 +136,53 @@
 
 class ResendOTP(Enum):
     RESEND_OTP = "resend_otp"
     TRANSFER = "transfer"
 
 
 class Resolution(Enum):
-    MERCHANT = ("merchant-accepted",)
+    MERCHANT = "merchant-accepted"
     DECLINED = "declined"
 
 
 class RiskAction(Enum):
     """Risk Action supported by Paystack."""
 
     ALLOW = "allow"
     DEFAULT = "default"
     DENY = "deny"
 
 
+class SettlementSchedule(Enum):
+    """ Schedule"""
+    AUTO = "auto"
+    WEEKLY = "weekly"
+    MANUAL = "manual"
+    MONTHLY = "monthly"
+
+
 class SplitType(Enum):
     PERCENTAGE = "percentage"
     FLAT = "flat"
 
 
 class STATUS(Enum):
     """Status supported by Paystack."""
 
     SUCCESS = "success"
     FAILED = "failed"
     PENDING = "pending"
+    PROCESSING = "processing"
+
+
+class TransactionStatus(Enum):
+    """Transaction status supported by Paystack."""
+    FAILED = "failed"
+    SUCCESS = "success"
+    ABANDONED = "abandoned"
 
 
 class USSD(Enum):
     """USSD supported by Paystack."""
 
     GUARANTY_BANK = "737"
     UNITED_BANK_OF_AFRICA = "919"
```

### Comparing `paystackease-0.1.3/paystackease/paystack.py` & `paystackease-1.0.0/paystackease/paystack.py`

 * *Files identical despite different names*

### Comparing `paystackease-0.1.3/pyproject.toml` & `paystackease-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "paystackease"
-version = "0.1.3"
+version = "1.0.0"
 description = "This is a simple api wrapper for paystack"
 authors = ["Peter Mbachu <doublep098@gmail.com>"]
 maintainers = [
     "petermbachu.bincom <petermbachu.bincom@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
-keywords = ["paystack", "api", "wrapper"]
+keywords = ["paystack", "paystackease", "python", "api", "payment integration"]
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
@@ -26,39 +26,38 @@
 
 [license]
 text = "Copyright ©2024 Peter Mbachu"
 
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/cla-bit/PayStackEase"
-"Repository" = "https://github.com/cla-bit/PayStackEase"
 "Source Code" = "https://github.com/cla-bit/PayStackEase"
 "Documentation" = "https://paystackease.readthedocs.io/en/latest/"
 "Bug Tracker" = "https://github.com/cla-bit/PayStackEase/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 aiohttp = "^3.8"
 requests = "^2.31"
 python-decouple = "^3.8"
-twine = "^5.0"
 
 
 [tool.poetry.group.docs.dependencies]
 pdflatex = "^0.1.3"
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
 sphinxawesome-theme = "^5.1.1"
 sphinx-autobuild = "^2024.2.4"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2"
 pylint = "^3.1"
+twine = "^5.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0"
 responses = "^0.25"
 pytest-asyncio = "^0.23"
 aioresponses = "^0.7"
```

### Comparing `paystackease-0.1.3/PKG-INFO` & `paystackease-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: paystackease
-Version: 0.1.3
+Version: 1.0.0
 Summary: This is a simple api wrapper for paystack
 License: MIT
-Keywords: paystack,api,wrapper
+Keywords: paystack,paystackease,python,api,payment integration
 Author: Peter Mbachu
 Author-email: doublep098@gmail.com
 Maintainer: petermbachu.bincom
 Maintainer-email: petermbachu.bincom@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,33 +19,34 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: python-decouple (>=3.8,<4.0)
 Requires-Dist: requests (>=2.31,<3.0)
-Requires-Dist: twine (>=5.0,<6.0)
 Project-URL: Bug Tracker, https://github.com/cla-bit/PayStackEase/issues
 Project-URL: Documentation, https://paystackease.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/cla-bit/PayStackEase
-Project-URL: Repository, https://github.com/cla-bit/PayStackEase
 Project-URL: Source Code, https://github.com/cla-bit/PayStackEase
 Description-Content-Type: text/markdown
 
-# PayStackEase Library  ![paystackease](docs/images/paystackease.png)
+# PayStackEase Library  
+
+------
+
+![Python Versions](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue) ![License](https://img.shields.io/pypi/l/paystackease) ![pypi](https://img.shields.io/pypi/v/paystackease.svg)
 
---------------------------------------------------------------------
 
 **PayStackEase API Library**  is a Python library that simplifies interacting with the Paystack API. 
 It provides both asynchronous and synchronous wrappers for various Paystack functionalities, 
 making it easier to integrate payment processing into your Python projects.
 
-> 📝: Read more on paystack api documentation: https://paystack.com/docs/api/
+> 📝: Read more on paystack api documentation: [Paystack API DOCUMENTATION](https://paystack.com/docs/api/)
 
-> 📝: Read more on paystackease api documentation: https://paystackease.readthedocs.io/en/latest/
+> 📝: Read more on paystackease api documentation: [PayStackEase DOCUMENTATION](https://paystackease.readthedocs.io/en/latest/)
 
 
 ## Getting Started
 
 You should create a Paystack account to generate a **Paystack Secret Key**. You can see this in the *settings page >> API keys and Webhook section*.
 
 > ⚠️: **Warning:** Do not expose your secret key or commit your secret key to git, or use them in client-side code.
@@ -88,25 +89,39 @@
 ## Install paystackease library:
 
 
 * #### Install paystackease using pip.
 
 > pip install paystackease
 
-or Download the wheel distribution file and install using pip
+* #### Install paystackease using pipx.
+
+> pipx install paystackease
+
+* #### Install paystackease using poetry.
+
+> poetry add paystackease
+
+
+## If you want to download the sdist packages directly:
+
+Download the wheel distribution file and install using pip
+
+>  pip install paystackease-1.0.0-py3-none-any.whl 
+
+Download the source distribution file, and install using pip
 
->  pip install paystackease-0.1.2-py3-none-any.whl 
+> pip install paystackease-1.0.0.tar.gz 
 
-or Download the source distribution file, and install using pip
 
-> pip install paystackease-0.1.2.tar.gz 
+## To get a development version of paystackease
 
-or clone from the github repository, unzip and install:
+Clone from the ``dev`` branch github repository, unzip and install:
 
-> git clone https://github.com/cla-bit/PayStackEase.git
+> git clone -b dev https://github.com/cla-bit/PayStackEase.git
 
 > cd PayStackEase
 
 > pip install paystackease
 
 ----------------------------------------------------------------------
 
@@ -196,9 +211,9 @@
     val1 = DocumentType.IDENTITY_NUMBER.value
     
     print(val1)
 ```
 
 > "identityNumber"
 
-Others are: ***EventType, Interval, MobileMoney, PWT, QRCODE, RecipientType, ResendOTP, Resolution, RiskAction, SplitType, STATUS, and USSD***.
+Others are: ***EventType, Interval, MobileMoney, PWT, QRCODE, RecipientType, ResendOTP, Resolution, RiskAction, SplitType, STATUS, etc***.
```

