# Comparing `tmp/types-braintree-4.28.0.20240402.tar.gz` & `tmp/types-braintree-4.28.0.20240405.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-braintree-4.28.0.20240402.tar", last modified: Tue Apr  2 02:17:28 2024, max compression
+gzip compressed data, was "types-braintree-4.28.0.20240405.tar", last modified: Fri Apr  5 02:14:50 2024, max compression
```

## Comparing `types-braintree-4.28.0.20240402.tar` & `types-braintree-4.28.0.20240405.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.548281 types-braintree-4.28.0.20240402/
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-02 02:17:27.000000 types-braintree-4.28.0.20240402/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 02:17:27.000000 types-braintree-4.28.0.20240402/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-02 02:17:28.548281 types-braintree-4.28.0.20240402/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.540281 types-braintree-4.28.0.20240402/braintree-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 02:17:27.000000 types-braintree-4.28.0.20240402/braintree-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/account_updater_daily_report.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/ach_mandate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/add_on.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/add_on_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/address.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/address_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/amex_express_checkout_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/android_pay_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/apple_pay_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/apple_pay_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/apple_pay_options.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/attribute_getter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/authorization_adjustment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/bin_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/braintree_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/client_token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/client_token_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/configuration.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/connected_merchant_paypal_status_changed.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/connected_merchant_status_transitioned.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/credentials_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/credit_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/credit_card_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/credit_card_verification.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/credit_card_verification_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/credit_card_verification_search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/customer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/customer_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/customer_search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/descriptor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/disbursement.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/disbursement_detail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/discount.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/discount_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/dispute.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.540281 types-braintree-4.28.0.20240402/braintree-stubs/dispute_details/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/dispute_details/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/dispute_details/evidence.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/dispute_details/paypal_message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/dispute_details/status_history.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/dispute_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/dispute_search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/document_upload.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/document_upload_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/enriched_customer_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    38081 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/error_codes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/error_result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/europe_bank_account.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.544281 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/authentication_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/authorization_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/braintree_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/configuration_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/gateway_timeout_error.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.544281 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/http/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/http/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/http/connection_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/http/invalid_response_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/http/timeout_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/invalid_challenge_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/invalid_signature_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/not_found_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/request_timeout_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/server_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/service_unavailable_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/test_operation_performed_in_production_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/too_many_requests_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/unexpected_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exceptions/upgrade_required_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exchange_rate_quote.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exchange_rate_quote_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exchange_rate_quote_input.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exchange_rate_quote_payload.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/exchange_rate_quote_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/facilitated_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/facilitator_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/granted_payment_instrument_update.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/iban_bank_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/ids_search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/liability_shift.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/local_payment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/local_payment_completed.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/local_payment_expired.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/local_payment_funded.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/local_payment_reversed.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/masterpass_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.544281 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/address_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/business_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/funding_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/individual_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/merchant_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_account_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/merchant_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/meta_checkout_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/meta_checkout_token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/modification.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/montary_amount.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/oauth_access_revocation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/oauth_credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/oauth_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/package_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/paginated_collection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/paginated_result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/partner_merchant.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/payment_instrument_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/payment_method.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/payment_method_customer_data_updated_metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/payment_method_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/payment_method_nonce.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/payment_method_nonce_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/payment_method_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/paypal_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/paypal_account_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/paypal_here.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/plan.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/plan_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/processor_response_types.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:27.000000 types-braintree-4.28.0.20240402/braintree-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/resource_collection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/revoked_payment_method_metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/risk_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/samsung_pay_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/sepa_direct_debit_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/sepa_direct_debit_account_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/settlement_batch_summary.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/settlement_batch_summary_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/signature_service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/status_event.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/subscription.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/subscription_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/subscription_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/subscription_search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/subscription_status_event.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/successful_result.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.544281 types-braintree-4.28.0.20240402/braintree-stubs/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/test/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/test/authentication_ids.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/test/credit_card_defaults.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/test/credit_card_numbers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/test/merchant_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/test/nonces.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/test/venmo_sdk.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/testing_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/three_d_secure_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction_amounts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction_details.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction_line_item.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction_line_item_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction_review.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/transaction_search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/unknown_payment_method.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/us_bank_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/us_bank_account_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/us_bank_account_verification.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/us_bank_account_verification_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/us_bank_account_verification_search.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.548281 types-braintree-4.28.0.20240402/braintree-stubs/util/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/crypto.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/datetime_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/generator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/graphql_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/http.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/util/xml_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/validation_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/validation_error_collection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/venmo_account.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/venmo_profile_data.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/visa_checkout_card.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/webhook_notification.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/webhook_notification_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/webhook_testing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-02 02:17:06.000000 types-braintree-4.28.0.20240402/braintree-stubs/webhook_testing_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 02:17:28.548281 types-braintree-4.28.0.20240402/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-02 02:17:27.000000 types-braintree-4.28.0.20240402/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:17:28.548281 types-braintree-4.28.0.20240402/types_braintree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-02 02:17:28.000000 types-braintree-4.28.0.20240402/types_braintree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-02 02:17:28.000000 types-braintree-4.28.0.20240402/types_braintree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:17:28.000000 types-braintree-4.28.0.20240402/types_braintree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 02:17:28.000000 types-braintree-4.28.0.20240402/types_braintree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:50.430178 types-braintree-4.28.0.20240405/
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-05 02:14:48.000000 types-braintree-4.28.0.20240405/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 02:14:48.000000 types-braintree-4.28.0.20240405/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-05 02:14:50.430178 types-braintree-4.28.0.20240405/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:50.422178 types-braintree-4.28.0.20240405/braintree-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 02:14:48.000000 types-braintree-4.28.0.20240405/braintree-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/account_updater_daily_report.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/ach_mandate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/add_on.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/add_on_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/address.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/address_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/amex_express_checkout_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/android_pay_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/apple_pay_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/apple_pay_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/apple_pay_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/attribute_getter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/authorization_adjustment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/bin_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/braintree_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/client_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/client_token_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/configuration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/connected_merchant_paypal_status_changed.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/connected_merchant_status_transitioned.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/credentials_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/credit_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/credit_card_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/credit_card_verification.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/credit_card_verification_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/credit_card_verification_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/customer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/customer_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/customer_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/descriptor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/disbursement.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/disbursement_detail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/discount.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/discount_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/dispute.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:50.422178 types-braintree-4.28.0.20240405/braintree-stubs/dispute_details/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/dispute_details/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/dispute_details/evidence.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/dispute_details/paypal_message.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/dispute_details/status_history.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/dispute_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/dispute_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/document_upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/document_upload_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/enriched_customer_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    38081 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/error_codes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/error_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/europe_bank_account.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:50.422178 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/authentication_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/authorization_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/braintree_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/configuration_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/gateway_timeout_error.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:50.426178 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/http/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/http/connection_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/http/invalid_response_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/http/timeout_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/invalid_challenge_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/invalid_signature_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/not_found_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/request_timeout_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/server_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/service_unavailable_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/test_operation_performed_in_production_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/too_many_requests_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/unexpected_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exceptions/upgrade_required_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exchange_rate_quote.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exchange_rate_quote_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exchange_rate_quote_input.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exchange_rate_quote_payload.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/exchange_rate_quote_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/facilitated_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/facilitator_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/granted_payment_instrument_update.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/iban_bank_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/ids_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/liability_shift.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/local_payment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/local_payment_completed.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/local_payment_expired.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/local_payment_funded.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/local_payment_reversed.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/masterpass_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/merchant.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:50.426178 types-braintree-4.28.0.20240405/braintree-stubs/merchant_account/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/merchant_account/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/merchant_account/address_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/merchant_account/business_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/merchant_account/funding_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/merchant_account/individual_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/merchant_account/merchant_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/merchant_account_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/merchant_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/meta_checkout_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/meta_checkout_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/modification.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/montary_amount.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/oauth_access_revocation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/oauth_credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/oauth_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/package_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/paginated_collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/paginated_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/partner_merchant.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/payment_instrument_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/payment_method.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/payment_method_customer_data_updated_metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/payment_method_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/payment_method_nonce.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/payment_method_nonce_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/payment_method_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/paypal_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/paypal_account_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/paypal_here.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/plan.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/plan_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/processor_response_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:48.000000 types-braintree-4.28.0.20240405/braintree-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/resource_collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/revoked_payment_method_metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/risk_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/samsung_pay_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/sepa_direct_debit_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/sepa_direct_debit_account_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/settlement_batch_summary.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/settlement_batch_summary_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/signature_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/status_event.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/subscription.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/subscription_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/subscription_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/subscription_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/subscription_status_event.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/successful_result.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:50.426178 types-braintree-4.28.0.20240405/braintree-stubs/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/test/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/test/authentication_ids.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/test/credit_card_defaults.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/test/credit_card_numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/test/merchant_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/test/nonces.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/test/venmo_sdk.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/testing_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/three_d_secure_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/transaction_amounts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/transaction_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/transaction_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/transaction_line_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/transaction_line_item_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/transaction_review.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/transaction_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/unknown_payment_method.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/us_bank_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/us_bank_account_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/us_bank_account_verification.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/us_bank_account_verification_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/us_bank_account_verification_search.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:50.426178 types-braintree-4.28.0.20240405/braintree-stubs/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/util/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/util/crypto.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/util/datetime_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/util/generator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/util/graphql_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/util/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/util/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/util/xml_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/validation_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/validation_error_collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/venmo_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/venmo_profile_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/visa_checkout_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/webhook_notification.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/webhook_notification_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/webhook_testing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-05 02:14:36.000000 types-braintree-4.28.0.20240405/braintree-stubs/webhook_testing_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:14:50.430178 types-braintree-4.28.0.20240405/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-05 02:14:48.000000 types-braintree-4.28.0.20240405/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:14:50.430178 types-braintree-4.28.0.20240405/types_braintree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-05 02:14:50.000000 types-braintree-4.28.0.20240405/types_braintree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-05 02:14:50.000000 types-braintree-4.28.0.20240405/types_braintree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:14:50.000000 types-braintree-4.28.0.20240405/types_braintree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 02:14:50.000000 types-braintree-4.28.0.20240405/types_braintree.egg-info/top_level.txt
```

### Comparing `types-braintree-4.28.0.20240402/CHANGELOG.md` & `types-braintree-4.28.0.20240405/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 4.28.0.20240405 (2024-04-05)
+
+Braintree: `PaymentMethodNonce.three_d_secure_info` can be `None` (#11711)
+
 ## 4.28.0.20240402 (2024-04-02)
 
 braintree: Cleanup overzealous reexports from non `__init__` modules (#11692)
 
 braintree: Use `Final` for string constants (#11680)
 
 braintree: Replace usages of `Any` (#11679)
```

### Comparing `types-braintree-4.28.0.20240402/PKG-INFO` & `types-braintree-4.28.0.20240405/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-braintree
-Version: 4.28.0.20240402
+Version: 4.28.0.20240405
 Summary: Typing stubs for braintree
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/braintree.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-braintree` aims to provide accurate annotations
 for `braintree==4.28.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/braintree. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `325577cb760c8539435ea6c78c87dc8cd218991c` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
+This package was generated from typeshed commit `130a04905c0cab48604ac7be1f3d18ce96567c68` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
 pytype 2024.3.19.
```

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/__init__.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/address.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/address.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/android_pay_card.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/android_pay_card.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/apple_pay_card.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/apple_pay_card.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/braintree_gateway.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/braintree_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/configuration.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/configuration.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/credentials_parser.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/credentials_parser.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/credit_card.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/credit_card.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/credit_card_gateway.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/credit_card_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/credit_card_verification.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/credit_card_verification.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/credit_card_verification_search.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/credit_card_verification_search.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/customer.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/customer.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/customer_search.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/customer_search.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/dispute.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/dispute.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/dispute_gateway.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/dispute_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/dispute_search.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/dispute_search.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/environment.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/environment.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/error_codes.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/error_codes.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/error_result.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/error_result.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/exceptions/__init__.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/exceptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/merchant_account/merchant_account.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/merchant_account/merchant_account.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/payment_instrument_type.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/payment_instrument_type.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/payment_method.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/payment_method.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/payment_method_gateway.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/payment_method_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/plan.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/plan.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/search.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/search.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/subscription.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/subscription.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/subscription_gateway.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/subscription_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/subscription_search.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/subscription_search.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/test/authentication_ids.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/test/authentication_ids.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/test/credit_card_numbers.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/test/credit_card_numbers.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/test/nonces.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/test/nonces.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/testing_gateway.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/testing_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/transaction.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/transaction.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/transaction_gateway.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/transaction_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/transaction_search.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/transaction_search.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/us_bank_account_verification.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/us_bank_account_verification.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/us_bank_account_verification_search.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/us_bank_account_verification_search.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/util/http.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/util/http.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/validation_error_collection.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/validation_error_collection.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/braintree-stubs/webhook_notification.pyi` & `types-braintree-4.28.0.20240405/braintree-stubs/webhook_notification.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.28.0.20240402/setup.py` & `types-braintree-4.28.0.20240405/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-braintree` aims to provide accurate annotations
 for `braintree==4.28.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/braintree. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `325577cb760c8539435ea6c78c87dc8cd218991c` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
+This package was generated from typeshed commit `130a04905c0cab48604ac7be1f3d18ce96567c68` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
 pytype 2024.3.19.
 '''.lstrip()
 
 setup(name=name,
-      version="4.28.0.20240402",
+      version="4.28.0.20240405",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/braintree.md",
```

### Comparing `types-braintree-4.28.0.20240402/types_braintree.egg-info/PKG-INFO` & `types-braintree-4.28.0.20240405/types_braintree.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-braintree
-Version: 4.28.0.20240402
+Version: 4.28.0.20240405
 Summary: Typing stubs for braintree
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/braintree.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-braintree` aims to provide accurate annotations
 for `braintree==4.28.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/braintree. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `325577cb760c8539435ea6c78c87dc8cd218991c` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
+This package was generated from typeshed commit `130a04905c0cab48604ac7be1f3d18ce96567c68` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
 pytype 2024.3.19.
```

### Comparing `types-braintree-4.28.0.20240402/types_braintree.egg-info/SOURCES.txt` & `types-braintree-4.28.0.20240405/types_braintree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

