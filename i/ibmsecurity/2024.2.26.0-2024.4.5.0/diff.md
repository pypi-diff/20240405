# Comparing `tmp/ibmsecurity-2024.2.26.0.tar.gz` & `tmp/ibmsecurity-2024.4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibmsecurity-2024.2.26.0.tar", last modified: Tue Feb 27 09:26:29 2024, max compression
+gzip compressed data, was "ibmsecurity-2024.4.5.0.tar", last modified: Fri Apr  5 15:57:57 2024, max compression
```

## Comparing `ibmsecurity-2024.2.26.0.tar` & `ibmsecurity-2024.4.5.0.tar`

### file list

```diff
@@ -1,490 +1,490 @@
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.572319 ibmsecurity-2024.2.26.0/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11357 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/LICENSE
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       20 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/MANIFEST.in
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     8610 2024-02-27 09:26:29.571319 ibmsecurity-2024.2.26.0/PKG-INFO
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7743 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/README.md
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.473319 ibmsecurity-2024.2.26.0/ibmsecurity/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.476319 ibmsecurity-2024.2.26.0/ibmsecurity/appliance/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/appliance/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3433 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/appliance/ibmappliance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    31457 2024-02-23 12:27:24.000000 ibmsecurity-2024.2.26.0/ibmsecurity/appliance/isamappliance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1644 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/appliance/isamappliance_adminproxy.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    18326 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/appliance/isdsappliance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1899 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/appliance/isdsappliance_adminproxy.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    18192 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/appliance/isvgappliance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1899 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/appliance/isvgappliance_adminproxy.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.477319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.481319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.481319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/access_control/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/access_control/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    17797 2023-11-10 14:29:53.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/access_control/policies.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    17324 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/access_control/policy_attachments.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    12329 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/access_control/policy_sets.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9048 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/access_policy.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10224 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/advanced_configuration.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.483319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/api_protection/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/api_protection/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    32357 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/api_protection/clients.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    22725 2021-06-04 12:46:11.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/api_protection/definitions.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2135 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/api_protection/dynamic_clients.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1337 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/api_protection/dynamic_clients_migration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3427 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/api_protection/grants.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1972 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/api_protection/grants_user.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5722 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/attribute_matchers.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7605 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/attributes.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.485319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2140 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/mechanism_types.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11692 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/mechanisms.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    14078 2023-11-10 14:29:53.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/policies.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.486319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      519 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/all.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1674 2023-03-10 12:33:20.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdconf.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2441 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdopts.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1758 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/securid.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5016 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/rsa_otp.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4225 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/database.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.486319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/devices/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/devices/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2845 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/devices/fingerprints.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2450 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/devices/userids.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7519 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/extensions.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.488319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/fido2/
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)        0 2022-05-19 14:24:42.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/fido2/__init__.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     6842 2022-05-19 14:24:42.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/fido2/metadata.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8482 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/fido2/metadata_services.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     2260 2022-05-19 14:24:42.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/fido2/registrations.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7358 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/fido2/relying_parties.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     1002 2022-05-19 14:24:42.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/fido2/u2f_migration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9375 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/mapping_rules.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.489319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/mmfa/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/mmfa/__init__.py
--rwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)     1547 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/mmfa/configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6601 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/mmfa/push_notification_registration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1808 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/mmfa/transactions.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1873 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/obligation_types.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6944 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/obligations.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1767 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/password_vault.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.491319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3504 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/all.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4072 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/database.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4159 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/fiberlink.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7172 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/javascript.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4034 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/ldap.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4238 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/qradar.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4147 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/restful.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1963 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/types.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     8728 2022-05-19 14:24:42.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/risk_profiles.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.491319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/runtime_template/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/runtime_template/__init__.py
--rwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)     6341 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/runtime_template/directory.py
--rwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)     9107 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/runtime_template/file.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5894 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/runtime_template/root.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.494319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2295 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/enterprise_profile.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2900 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/ext_auth_service.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2709 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/general.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2194 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/group.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4086 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/isam_user.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1226 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/ldap_attrs.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      812 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/ldap_objs.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4968 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/mode.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    20221 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/scim.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2635 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/user_profile.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7630 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim_custom_schema_extensions.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.496319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6662 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/ci.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2248 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/connection.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6994 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/isamruntime.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6985 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/jdbc.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7368 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/ldap.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     8952 2022-05-19 14:24:42.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/redis.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7129 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/smtp.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7285 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/ws.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1831 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/user_info.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.497319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/user_registry/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/user_registry/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4826 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/user_registry/group.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3831 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/user_registry/user.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7573 2023-03-10 12:33:20.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/appliance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4287 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/application_logs.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.506319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3882 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/activation.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    20896 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/admin.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5783 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/admin_ssh_keys.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4351 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/advanced_tuning_parameters.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3653 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/application_database_settings.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      912 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/application_locale.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8840 2023-11-10 14:29:53.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/audit_configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6609 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/available_updates.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      863 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cli.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.508319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      652 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/config_database.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    11257 2022-05-19 14:24:42.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2218 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/log.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6205 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/node.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2472 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/property.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      653 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/runtime_database.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      622 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/signature.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1483 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/trace.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4844 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/date_time.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2903 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/dsc.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8366 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/extensions.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1077 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/file_downloads.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5289 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/fips.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3328 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/firmware.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     5699 2021-10-07 13:52:15.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/fixpack.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1839 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/geolocation_db.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.508319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/host/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/host/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2130 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/host/name.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4087 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/host/records.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2902 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/license.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2757 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/lmi.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1914 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/lmi_tracing.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5491 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authentication.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.510319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authorization/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authorization/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1368 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authorization/config.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      793 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authorization/feature.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     4427 2022-05-19 14:24:42.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authorization/role.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2166 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authorization/role_feature.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2474 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authorization/role_group.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2447 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authorization/role_user.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4090 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_ssl_certificate.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.514319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      704 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/active_status.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      344 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3982 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/dns.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.515319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.515319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/advanced_tuning/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/advanced_tuning/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2622 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/advanced_tuning/at_logging.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6312 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/advanced_tuning/config.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.515319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/attributes/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/attributes/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5935 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/attributes/advanced_tuning.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2157 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/attributes/log.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4414 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/config.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4736 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/error_page.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5983 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/ha.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.517319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/services/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/services/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6046 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/services/advanced_tuning.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8785 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/services/config.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2691 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/services/layer.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6110 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/services/servers.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4456 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/ssl.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8331 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/host_records.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1354 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/hostname.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5962 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/interfaces.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     7005 2021-10-07 13:52:15.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/interfaces_ipv4.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6360 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/interfaces_ipv6.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5669 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/interfaces_vlan.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3269 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/packet_trace.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    13725 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/static_routes.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2109 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/test_connection.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      544 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/overview.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.518319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/remote_syslog/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/remote_syslog/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      490 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/remote_syslog/facility.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     6350 2022-05-19 14:24:42.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/remote_syslog/forwarder.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4537 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/remote_syslog/forwarder_sources.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      646 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/remote_syslog/instance_logs.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      582 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/remote_syslog/instances.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      490 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/remote_syslog/severity.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      474 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/remote_syslog/sources.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.519319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/runtime/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/runtime/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1365 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/runtime/cluster.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5240 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/runtime/listening_interfaces.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2927 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/runtime/process.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3765 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/runtime/tuning_parameters.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3567 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/scheduled_security_updates.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1638 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/service_agreement.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)      834 2021-10-07 13:52:15.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/setup_complete.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5499 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/silent_config.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10170 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/snapshots.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4092 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/snmp_monitoring.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.520319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/ssl_certificates/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/ssl_certificates/__init__.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     7048 2022-05-19 14:24:42.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/ssl_certificates/certificate_databases.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4258 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/ssl_certificates/certificate_requests.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     9568 2022-05-19 14:24:42.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/ssl_certificates/personal_certificate.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1782 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/ssl_certificates/replication.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9229 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/ssl_certificates/signer_certificate.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6520 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/support.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.521319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/sysaccount/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/sysaccount/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2147 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/sysaccount/groups.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5938 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/sysaccount/ssh_keys.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3798 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/sysaccount/users.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.523319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/system_alerts/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/system_alerts/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2033 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/system_alerts/alerts.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4748 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/system_alerts/email.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4977 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/system_alerts/logdb.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4755 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/system_alerts/rsyslog.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7408 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/system_alerts/snmp.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      524 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/update_history.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8752 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/update_servers.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      307 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/version.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.523319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.523319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/base/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/base/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.523319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/base/network/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/base/network/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.523319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/base/network/db_configuration/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/base/network/db_configuration/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4851 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/base/network/db_configuration/configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      862 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/publish.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.524319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/service_configuration/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/service_configuration/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4484 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/service_configuration/configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1411 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/event_log.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.526319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1935 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/alias_service.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1703 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/alias_service_settings.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6693 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/attribute_source.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1414 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/connector_instructions.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    13427 2021-06-04 12:46:11.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/federations.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2194 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/partner_templates.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    14331 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/partners.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     9196 2021-06-04 12:46:11.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/point_of_contact.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.527319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/sts/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/sts/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    13879 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/sts/module_chains.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2200 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/sts/modules.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7364 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/sts/templates.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9066 2023-03-10 12:33:20.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/statistics.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.531319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.533319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8798 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/cors_policies.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11745 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/documentation_root.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7880 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/policies.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.534319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/resources/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/resources/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1190 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/resources/instances.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    28901 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/resources/resources.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    53403 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/resources/servers.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.535319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/utilities/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/utilities/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2527 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/utilities/credential.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      522 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/utilities/group.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.536319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3012 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/cleanup.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.537319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/configuration/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/configuration/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    12469 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/configuration/entry.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4436 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/configuration/stanza.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4392 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/configuration/trace.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8025 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/instance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3375 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/logs.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6440 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/trace.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6798 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/client_certificate_mapping.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4502 2023-03-10 12:33:20.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/dsc.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.539319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/embedded_ldap/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/embedded_ldap/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      647 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/embedded_ldap/admin.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3038 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/embedded_ldap/debug.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3262 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/embedded_ldap/group.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2542 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/embedded_ldap/suffix.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3831 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/embedded_ldap/user.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10067 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/fsso.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.539319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/global_settings/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/global_settings/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.539319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/global_settings/redis_configuration/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/global_settings/redis_configuration/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7943 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/global_settings/redis_configuration/collections.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     2387 2022-05-19 14:24:42.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/global_settings/redis_configuration/wrp.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7498 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/global_settings/waf.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8572 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/http_transformation.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.540319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/iag/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/iag/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3274 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/iag/export.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6591 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/junction_mapping.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.542319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3633 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6590 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths_property.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6410 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/defaults.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4593 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/domains.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4092 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/keyfiles.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3231 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/realms.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8384 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/realms_property.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3996 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/realms_subsection.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      808 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/test.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3307 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/ltpa_key.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4930 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/password_strength.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1924 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/query_sitecontents.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7102 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/rate_limiting.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.547319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2314 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/aac_configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1223 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/common_configurations.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2544 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/common_logs.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.548319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/__init__.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    13869 2023-01-20 12:28:18.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/entry.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3853 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/stanza.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4108 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/trace.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2334 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/waf_config.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     4206 2022-05-19 14:24:42.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/federation_configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10967 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/instance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2062 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/interfaces.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1058 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/ivg_configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    54202 2024-02-26 08:45:45.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/junctions.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1138 2024-02-23 12:27:24.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/junctions_config.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11135 2024-02-23 12:27:24.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/junctions_server.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2698 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/logs.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.549319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5472 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/all.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5021 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/directory.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9878 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/file.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2745 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/mmfa_configuration.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     3510 2021-06-04 12:46:11.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/oauth_configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7434 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/statistics.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8251 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/trace.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9736 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/transaction_logging.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5145 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/rsa_securid_config.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.551319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3463 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/acl.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.552319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/configuration/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/configuration/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11148 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/configuration/entry.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     3006 2021-10-07 13:52:15.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/configuration/file.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3402 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/configuration/stanza.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.553319 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/federated_directories/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/federated_directories/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6849 2024-02-23 12:27:24.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/federated_directories/stanza.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2895 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/federated_directories/suffix.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3118 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/object.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      840 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/pdadmin.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4728 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/pop.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8404 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/process.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1242 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/replication.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3765 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/trace.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4361 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/sso_keys.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7154 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/url_mapping.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11682 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/user_name_mapping.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.557319 ibmsecurity-2024.2.26.0/ibmsecurity/isds/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3470 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/admin.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4859 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/advanced_tuning_parameters.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3372 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/appliance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6037 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/available_updates.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1982 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/config.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3468 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/date_time.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2943 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/firmware.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3978 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/fixpack.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2117 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/host_records.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1827 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/hostnames.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1677 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/interfaces.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2930 2021-03-08 12:58:33.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/license.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      267 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/logs.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3849 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/server.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6043 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/snapshots.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4746 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/snmp_monitoring.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1713 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/statistics.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4740 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/support.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.558319 ibmsecurity-2024.2.26.0/ibmsecurity/isds/system_alerts/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/system_alerts/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2018 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/system_alerts/alerts.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4730 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/system_alerts/rsyslog.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7383 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/system_alerts/snmp.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      267 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/token.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8747 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isds/update_servers.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.564319 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3470 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/admin.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4859 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/advanced_tuning_parameters.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4858 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/appliance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7701 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/available_updates.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2448 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/certstore_personal.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2233 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/certstore_signer.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.564319 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/cm/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/cm/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1998 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/cm/process.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3468 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/date_time.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.564319 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/db/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/db/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      340 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/db/process.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2943 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/firmware.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3978 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/fixpack.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2117 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/host_records.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1827 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/hostnames.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.568319 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2418 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/certstore_personal.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4253 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/certstore_signer.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    13698 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/db.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3888 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/external_library.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      921 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/guided_setup.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4584 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/jvm_property.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3691 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/keystore.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7897 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/ldap.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6874 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/mail.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3778 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/nls.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10525 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/openid.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1937 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/process.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6655 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/property.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1000 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/property_file.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4902 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/workflowextension.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1735 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/interfaces.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1425 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/lmi.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7315 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/lmi_auth.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      267 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/logs.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4135 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/management_authentication.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2454 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/management_ssl_certificate.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      329 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/notifications.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.569319 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/sdi/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/sdi/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2088 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/sdi/process.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1781 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/service_agreement.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      946 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/setup_complete.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6043 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/snapshots.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4746 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/snmp_monitoring.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      323 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/startup.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4740 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/support.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.570320 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/system_alerts/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/system_alerts/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2018 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/system_alerts/alerts.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4730 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/system_alerts/rsyslog.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7383 2023-11-10 14:29:41.000000 ibmsecurity-2024.2.26.0/ibmsecurity/isvg/system_alerts/snmp.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.570320 ibmsecurity-2024.2.26.0/ibmsecurity/user/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/user/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      528 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/user/applianceuser.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      483 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/user/isamuser.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      526 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/user/isdsapplianceuser.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      409 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/user/user.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.571319 ibmsecurity-2024.2.26.0/ibmsecurity/utilities/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.2.26.0/ibmsecurity/utilities/__init__.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    10333 2022-05-19 14:24:42.000000 ibmsecurity-2024.2.26.0/ibmsecurity/utilities/tools.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-02-27 09:26:29.571319 ibmsecurity-2024.2.26.0/ibmsecurity.egg-info/
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     8610 2024-02-27 09:26:29.000000 ibmsecurity-2024.2.26.0/ibmsecurity.egg-info/PKG-INFO
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    18594 2024-02-27 09:26:29.000000 ibmsecurity-2024.2.26.0/ibmsecurity.egg-info/SOURCES.txt
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        1 2024-02-27 09:26:29.000000 ibmsecurity-2024.2.26.0/ibmsecurity.egg-info/dependency_links.txt
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        1 2023-03-10 12:34:43.000000 ibmsecurity-2024.2.26.0/ibmsecurity.egg-info/not-zip-safe
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       32 2024-02-27 09:26:29.000000 ibmsecurity-2024.2.26.0/ibmsecurity.egg-info/requires.txt
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       12 2024-02-27 09:26:29.000000 ibmsecurity-2024.2.26.0/ibmsecurity.egg-info/top_level.txt
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      907 2024-02-26 08:45:45.000000 ibmsecurity-2024.2.26.0/pyproject.toml
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       38 2024-02-27 09:26:29.572319 ibmsecurity-2024.2.26.0/setup.cfg
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1172 2024-02-26 08:45:45.000000 ibmsecurity-2024.2.26.0/setup.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.289339 ibmsecurity-2024.4.5.0/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11357 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/LICENSE
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       20 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/MANIFEST.in
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    11122 2024-04-05 15:57:57.289339 ibmsecurity-2024.4.5.0/PKG-INFO
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10256 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/README.md
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.232339 ibmsecurity-2024.4.5.0/ibmsecurity/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.234339 ibmsecurity-2024.4.5.0/ibmsecurity/appliance/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/appliance/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3424 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/ibmsecurity/appliance/ibmappliance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    34558 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/ibmsecurity/appliance/isamappliance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1637 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/ibmsecurity/appliance/isamappliance_adminproxy.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    20475 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/ibmsecurity/appliance/isdsappliance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1899 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/appliance/isdsappliance_adminproxy.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    20345 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/ibmsecurity/appliance/isvgappliance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1899 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/appliance/isvgappliance_adminproxy.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.234339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.236339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.236339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/access_control/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/access_control/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    17797 2023-11-10 14:29:53.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/access_control/policies.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    17324 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/access_control/policy_attachments.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    12329 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/access_control/policy_sets.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9048 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/access_policy.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10224 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/advanced_configuration.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.237339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/api_protection/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/api_protection/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    32357 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/api_protection/clients.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    22725 2021-06-04 12:46:11.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/api_protection/definitions.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2135 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/api_protection/dynamic_clients.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1337 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/api_protection/dynamic_clients_migration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3427 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/api_protection/grants.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1972 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/api_protection/grants_user.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5742 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/attribute_matchers.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7605 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/attributes.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.237339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2140 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/mechanism_types.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11692 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/mechanisms.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    14078 2023-11-10 14:29:53.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/policies.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.238339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/rsa_otp/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/rsa_otp/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      519 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/rsa_otp/all.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1674 2023-03-10 12:33:20.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdconf.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2441 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdopts.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1758 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/rsa_otp/securid.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5016 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/rsa_otp.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4225 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/database.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.238339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/devices/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/devices/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2845 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/devices/fingerprints.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2450 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/devices/userids.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7519 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/extensions.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.239339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/fido2/
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)        0 2022-05-19 14:24:42.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/fido2/__init__.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     6842 2022-05-19 14:24:42.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/fido2/metadata.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8482 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/fido2/metadata_services.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     2260 2022-05-19 14:24:42.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/fido2/registrations.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7358 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/fido2/relying_parties.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     1002 2022-05-19 14:24:42.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/fido2/u2f_migration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9375 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/mapping_rules.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.239339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/mmfa/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/mmfa/__init__.py
+-rwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)     1547 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/mmfa/configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6601 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/mmfa/push_notification_registration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1808 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/mmfa/transactions.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1873 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/obligation_types.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6944 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/obligations.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1767 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/password_vault.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.240339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3504 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/all.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4072 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/database.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4159 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/fiberlink.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7172 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/javascript.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4034 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/ldap.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4238 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/qradar.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4147 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/restful.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1963 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/types.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8747 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/risk_profiles.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.241339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/runtime_template/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/runtime_template/__init__.py
+-rwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)     6341 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/runtime_template/directory.py
+-rwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)     9107 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/runtime_template/file.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5894 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/runtime_template/root.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.243339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2295 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/enterprise_profile.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2900 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/ext_auth_service.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2709 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/general.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2194 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/group.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4086 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/isam_user.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1226 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/ldap_attrs.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      812 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/ldap_objs.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4968 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/mode.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    20221 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/scim.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2635 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/user_profile.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7630 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim_custom_schema_extensions.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.244339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6662 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/ci.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2248 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/connection.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6994 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/isamruntime.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6985 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/jdbc.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7368 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/ldap.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     8952 2022-05-19 14:24:42.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/redis.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7129 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/smtp.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7285 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/ws.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1831 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/user_info.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.245339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/user_registry/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/user_registry/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4826 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/user_registry/group.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3831 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/user_registry/user.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7573 2023-03-10 12:33:20.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/appliance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4287 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/application_logs.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.251339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3882 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/activation.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    20896 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/admin.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5783 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/admin_ssh_keys.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4351 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/advanced_tuning_parameters.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3653 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/application_database_settings.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      912 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/application_locale.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8840 2023-11-10 14:29:53.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/audit_configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6609 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/available_updates.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      863 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cli.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.253339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      652 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/config_database.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    11257 2022-05-19 14:24:42.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2218 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/log.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6205 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/node.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2472 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/property.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      653 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/runtime_database.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      622 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/signature.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1483 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/trace.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4844 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/date_time.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2903 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/dsc.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8365 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/extensions.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1077 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/file_downloads.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5289 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/fips.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3328 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/firmware.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     5699 2021-10-07 13:52:15.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/fixpack.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1839 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/geolocation_db.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.253339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/host/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/host/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2130 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/host/name.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4087 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/host/records.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2902 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/license.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2757 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/lmi.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1914 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/lmi_tracing.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5491 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authentication.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.254339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authorization/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authorization/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1368 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authorization/config.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      793 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authorization/feature.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     4427 2022-05-19 14:24:42.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authorization/role.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2166 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authorization/role_feature.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2474 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authorization/role_group.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2447 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authorization/role_user.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4090 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_ssl_certificate.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.257339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      704 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/active_status.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      344 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3982 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/dns.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.258339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.258339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/advanced_tuning/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/advanced_tuning/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2622 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/advanced_tuning/at_logging.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6312 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/advanced_tuning/config.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.259339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/attributes/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/attributes/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5935 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/attributes/advanced_tuning.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2157 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/attributes/log.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4414 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/config.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4736 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/error_page.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5983 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/ha.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.260339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/services/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/services/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6046 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/services/advanced_tuning.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8785 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/services/config.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2691 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/services/layer.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6110 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/services/servers.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4456 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/ssl.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8331 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/host_records.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1354 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/hostname.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5962 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/interfaces.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     7005 2021-10-07 13:52:15.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/interfaces_ipv4.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6360 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/interfaces_ipv6.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5669 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/interfaces_vlan.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3269 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/packet_trace.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    13725 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/static_routes.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2109 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/test_connection.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      544 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/overview.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.261339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/remote_syslog/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/remote_syslog/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      490 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/remote_syslog/facility.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     6350 2022-05-19 14:24:42.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/remote_syslog/forwarder.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4537 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/remote_syslog/forwarder_sources.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      646 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/remote_syslog/instance_logs.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      582 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/remote_syslog/instances.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      490 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/remote_syslog/severity.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      474 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/remote_syslog/sources.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.262339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/runtime/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/runtime/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1365 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/runtime/cluster.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5240 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/runtime/listening_interfaces.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2927 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/runtime/process.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3765 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/runtime/tuning_parameters.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3567 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/scheduled_security_updates.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1638 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/service_agreement.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)      834 2021-10-07 13:52:15.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/setup_complete.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5499 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/silent_config.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10170 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/snapshots.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4092 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/snmp_monitoring.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.263339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/ssl_certificates/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/ssl_certificates/__init__.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     7048 2022-05-19 14:24:42.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/ssl_certificates/certificate_databases.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4258 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/ssl_certificates/certificate_requests.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     9568 2022-05-19 14:24:42.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/ssl_certificates/personal_certificate.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1782 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/ssl_certificates/replication.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9229 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/ssl_certificates/signer_certificate.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6520 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/support.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.264339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/sysaccount/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/sysaccount/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2147 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/sysaccount/groups.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5938 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/sysaccount/ssh_keys.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3798 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/sysaccount/users.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.265339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/system_alerts/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/system_alerts/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2033 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/system_alerts/alerts.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4748 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/system_alerts/email.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4977 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/system_alerts/logdb.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4755 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/system_alerts/rsyslog.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7408 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/system_alerts/snmp.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      524 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/update_history.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8752 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/update_servers.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      307 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/version.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.265339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.265339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/base/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/base/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.265339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/base/network/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/base/network/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.266339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/base/network/db_configuration/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/base/network/db_configuration/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4851 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/base/network/db_configuration/configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      862 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/publish.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.266339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/service_configuration/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/service_configuration/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4484 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/service_configuration/configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1411 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/event_log.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.267339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1935 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/alias_service.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1703 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/alias_service_settings.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6693 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/attribute_source.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1414 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/connector_instructions.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    13427 2021-06-04 12:46:11.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/federations.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2194 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/partner_templates.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    14331 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/partners.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     9196 2021-06-04 12:46:11.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/point_of_contact.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.268339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/sts/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/sts/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    13879 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/sts/module_chains.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2200 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/sts/modules.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7364 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/sts/templates.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9066 2023-03-10 12:33:20.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/statistics.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.270339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.270339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8798 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/cors_policies.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11745 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/documentation_root.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7880 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/policies.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.271339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/resources/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/resources/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1190 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/resources/instances.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    28901 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/resources/resources.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    53403 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/resources/servers.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.271339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/utilities/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/utilities/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2527 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/utilities/credential.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      522 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/utilities/group.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.272339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3012 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/cleanup.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.272339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/configuration/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/configuration/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    12469 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/configuration/entry.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4436 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/configuration/stanza.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4392 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/configuration/trace.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8025 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/instance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3375 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/logs.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6440 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/trace.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6798 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/client_certificate_mapping.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4502 2023-03-10 12:33:20.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/dsc.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.273339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/embedded_ldap/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/embedded_ldap/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      647 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/embedded_ldap/admin.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3038 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/embedded_ldap/debug.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3262 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/embedded_ldap/group.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2542 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/embedded_ldap/suffix.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3831 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/embedded_ldap/user.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10067 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/fsso.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.273339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/global_settings/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/global_settings/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.273339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/global_settings/redis_configuration/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/global_settings/redis_configuration/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7943 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/global_settings/redis_configuration/collections.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     2387 2022-05-19 14:24:42.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/global_settings/redis_configuration/wrp.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7498 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/global_settings/waf.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8572 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/http_transformation.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.274339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/iag/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/iag/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3274 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/iag/export.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6591 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/junction_mapping.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.275339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3633 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6590 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths_property.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6410 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/defaults.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4593 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/domains.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4092 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/keyfiles.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3231 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/realms.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8384 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/realms_property.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3996 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/realms_subsection.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      808 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/test.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3307 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/ltpa_key.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4930 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/password_strength.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1924 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/query_sitecontents.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7102 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/rate_limiting.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.277339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2749 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/aac_configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1223 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/common_configurations.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2544 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/common_logs.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.277339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/configuration/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/configuration/__init__.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    13869 2023-01-20 12:28:18.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/configuration/entry.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3853 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/configuration/stanza.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4108 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/configuration/trace.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2334 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/configuration/waf_config.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4634 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/federation_configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10967 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/instance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2062 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/interfaces.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1058 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/ivg_configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    54202 2024-02-26 08:45:45.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/junctions.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1138 2024-02-23 12:27:24.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/junctions_config.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11135 2024-02-23 12:27:24.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/junctions_server.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2698 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/logs.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.278339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/management_root/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/management_root/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5472 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/management_root/all.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5021 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/management_root/directory.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9878 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/management_root/file.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2745 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/mmfa_configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3947 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/oauth_configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7434 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/statistics.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8251 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/trace.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9736 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/transaction_logging.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5145 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/rsa_securid_config.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.279339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3463 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/acl.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.279339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/configuration/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/configuration/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11148 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/configuration/entry.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     3006 2021-10-07 13:52:15.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/configuration/file.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3402 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/configuration/stanza.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.279339 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/federated_directories/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/federated_directories/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6722 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/federated_directories/stanza.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2895 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/federated_directories/suffix.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3118 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/object.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      840 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/pdadmin.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4728 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/pop.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8404 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/process.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1242 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/replication.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3765 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/trace.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4361 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/sso_keys.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7154 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/url_mapping.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11682 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/user_name_mapping.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.282339 ibmsecurity-2024.4.5.0/ibmsecurity/isds/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3470 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/admin.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4859 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/advanced_tuning_parameters.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3372 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/appliance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6037 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/available_updates.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1982 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/config.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3468 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/date_time.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2943 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/firmware.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3978 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/fixpack.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2117 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/host_records.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1827 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/hostnames.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1677 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/interfaces.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2930 2021-03-08 12:58:33.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/license.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      267 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/logs.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3849 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/server.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6043 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/snapshots.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4746 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/snmp_monitoring.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1713 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/statistics.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4740 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/support.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.282339 ibmsecurity-2024.4.5.0/ibmsecurity/isds/system_alerts/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/system_alerts/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2018 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/system_alerts/alerts.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4730 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/system_alerts/rsyslog.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7383 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/system_alerts/snmp.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      267 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/token.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8747 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isds/update_servers.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.285339 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3470 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/admin.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4859 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/advanced_tuning_parameters.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4858 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/appliance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7701 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/available_updates.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2448 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/certstore_personal.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2233 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/certstore_signer.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.285339 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/cm/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/cm/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1998 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/cm/process.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3468 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/date_time.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.285339 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/db/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/db/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      340 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/db/process.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2943 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/firmware.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3978 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/fixpack.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2117 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/host_records.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1827 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/hostnames.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.287339 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2418 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/certstore_personal.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4253 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/certstore_signer.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    13698 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/db.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3888 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/external_library.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      921 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/guided_setup.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4584 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/jvm_property.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3691 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/keystore.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7897 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/ldap.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6874 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/mail.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3778 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/nls.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10525 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/openid.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1937 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/process.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6655 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/property.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1000 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/property_file.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4902 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/workflowextension.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1735 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/interfaces.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1425 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/lmi.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7315 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/lmi_auth.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      267 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/logs.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4135 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/management_authentication.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2454 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/management_ssl_certificate.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      329 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/notifications.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.287339 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/sdi/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/sdi/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2088 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/sdi/process.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1781 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/service_agreement.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      946 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/setup_complete.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6043 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/snapshots.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4746 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/snmp_monitoring.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      323 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/startup.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4740 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/support.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.288339 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/system_alerts/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/system_alerts/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2018 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/system_alerts/alerts.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4730 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/system_alerts/rsyslog.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7383 2023-11-10 14:29:41.000000 ibmsecurity-2024.4.5.0/ibmsecurity/isvg/system_alerts/snmp.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.288339 ibmsecurity-2024.4.5.0/ibmsecurity/user/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/user/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      528 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/user/applianceuser.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      483 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/user/isamuser.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      526 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/user/isdsapplianceuser.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      409 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/user/user.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.289339 ibmsecurity-2024.4.5.0/ibmsecurity/utilities/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2024.4.5.0/ibmsecurity/utilities/__init__.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    10333 2022-05-19 14:24:42.000000 ibmsecurity-2024.4.5.0/ibmsecurity/utilities/tools.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2024-04-05 15:57:57.289339 ibmsecurity-2024.4.5.0/ibmsecurity.egg-info/
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    11122 2024-04-05 15:57:57.000000 ibmsecurity-2024.4.5.0/ibmsecurity.egg-info/PKG-INFO
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    18594 2024-04-05 15:57:57.000000 ibmsecurity-2024.4.5.0/ibmsecurity.egg-info/SOURCES.txt
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        1 2024-04-05 15:57:57.000000 ibmsecurity-2024.4.5.0/ibmsecurity.egg-info/dependency_links.txt
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        1 2023-03-10 12:34:43.000000 ibmsecurity-2024.4.5.0/ibmsecurity.egg-info/not-zip-safe
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       32 2024-04-05 15:57:57.000000 ibmsecurity-2024.4.5.0/ibmsecurity.egg-info/requires.txt
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       12 2024-04-05 15:57:57.000000 ibmsecurity-2024.4.5.0/ibmsecurity.egg-info/top_level.txt
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      906 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/pyproject.toml
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       38 2024-04-05 15:57:57.289339 ibmsecurity-2024.4.5.0/setup.cfg
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1171 2024-04-05 15:56:18.000000 ibmsecurity-2024.4.5.0/setup.py
```

### Comparing `ibmsecurity-2024.2.26.0/LICENSE` & `ibmsecurity-2024.4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/PKG-INFO` & `ibmsecurity-2024.4.5.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: ibmsecurity
-Version: 2024.2.26.0
-Summary: Idempotent functions for IBM Security Appliance REST APIs
-Home-page: 
-Author: IBM
-Author-email: IBM <secorch@wwpdl.vnet.ibm.com>
-Project-URL: Homepage, https://github.com/IBM-Security/ibmsecurity
-Project-URL: Bug Tracker, https://github.com/IBM-Security/ibmsecurity/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: System Administrators
-Classifier: Topic :: Software Development :: Build Tools
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: jmespath>=1.0.0
-Requires-Dist: PyYAML
-
 # IBM Sample Code
 
 This repository contains Python code to manage IBM Security Appliances using their respective REST APIs.
 ISAM appliance has the most mature code.
 
 Code for ISDS appliance is under development.
 
@@ -42,15 +19,99 @@
 The following Python Packages are optional:
 1. cryptography - to perform action on certificates (used for idempotency in management_ssl_certificate)
 2. python-dateutil - date utilities (used for idempotency in management_ssl_certificate)
 
 Appliances need to have an ip address defined for their LMI. This may mean that appliances have had their initial setup 
 done with license acceptance.
 
+## TLS verification enabled (v2024.4.5)
+
+These changes are backwards compatible. We default to not verifying but always display a notice:
+
+````markdown
+Certificate verification has been disabled. Python is NOT verifying the SSL 
+certificate of the host appliance and InsecureRequestWarning messages are 
+
+being suppressed for the following host:
+
+https://{0}:{1}
+
+To use certificate verification:
+
+1. When the certificate is trusted by your Python environment:
+   Instantiate all instances of ISAMAppliance with verify=True or set 
+   the environment variable IBMSECLIB_VERIFY_CONNECTION=True.
+2. When the certificate is not already trusted in your Python environment:
+   Instantiate all instances of ISAMAppliance with the verify parameter
+   set to the fully qualified path to a CA bundle.
+
+See the following URL for more details:
+https://requests.readthedocs.io/en/latest/user/advanced/#ssl-cert-verification
+````
+To remediate this cert validation warning, consider the instructions below:
+
+Correct usage:
+
+If you have the cert on disk somewhere,
+instantiate the ISAMAppliance with:
+
+    ISAMAppliance(…, verify=<path to cert>)
+
+You can retrieve this from appliance using a command like:
+
+    openssl s_client -connect ${HOSTNAME}:${PORT} </dev/null 2>/dev/null | openssl x509 -outform pem >  isamAppliance.pem
+
+If the cert is already trusted in your Python environment,
+instantiate the ISAMAppliance with:
+
+    ISAMAppliance(…, verify=True)
+
+or set the environment variable: `IBMSECLIB_VERIFY_CONNECTION=true`
+
+If you receive errors about the hostname not matching the certificate:
+
+This might look like:
+````
+<stack trace>
+
+…
+
+    raise CertificateError("hostname %r doesn't match %r" % (hostname, dnsnames[0]))
+
+urllib3.util.ssl_match_hostname.CertificateError: hostname '192.168.42.111' doesn't match 'appliance.ibm.com'
+
+````
+
+Ensure the hostname used when instantiating your ISAMAppliance matches the Subject Alternative Name of the cert.
+
+Check with: 
+
+    openssl x509 -in <cert-pem-file> -text
+
+Example:
+
+    $ openssl x509 -in /path/to/appliance.pem -text
+
+Certificate:
+
+    Data:
+        Version: 3 (0x2)
+        …
+            X509v3 Subject Alternative Name:
+                DNS:appliance.ibm.com
+…
+
+The following will generate errors:
+
+    ISAMAppliance(host=”192.168.42.111”, lmi_port=443, verify=/path/to/appliance.pem)
+
+as host does not match the Subject Alternative Name.
+Instead, use:
 
+    ISAMAppliance(host=”appliance.ibm.com”, lmi_port=443, verify=/path/to/appliance.pem)
 
 ## Versioning
 
 This package uses a date for versioning. For example: "2017.03.18.0"
 
 It is the date when the package is released with a sequence number at the end to handle when there are 
 multiple releases in one day (expected to be uncommon).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/appliance/ibmappliance.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/appliance/ibmappliance.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
         :return: True if the execution failed.
         """
         if self.get('rc', -1) == 0:
             return False
         return True
 
 
-class IBMAppliance:
-    __metaclass__ = ABCMeta
+class IBMAppliance(metaclass=ABCMeta):
 
     def __init__(self, hostname, user):
         self.logger = logging.getLogger(__name__)
         self.logger.debug('Creating an IBMAppliance')
 
         self.hostname = hostname
         self.user = user
```

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/appliance/isamappliance.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/appliance/isamappliance.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,104 @@
 import json
 import requests
+import traceback
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 import logging
 from .ibmappliance import IBMAppliance
 from .ibmappliance import IBMError
 from .ibmappliance import IBMFatal
 from ibmsecurity.utilities import tools
 from io import open
+from os import environ
 
 try:
     basestring
 except NameError:
     basestring = (str, bytes)
 
 
 class ISAMAppliance(IBMAppliance):
-    def __init__(self, hostname, user, lmi_port=443, cert=None):
+    def __init__(self, hostname, user, lmi_port=443, cert=None, verify=None, debug=True):
         self.logger = logging.getLogger(__name__)
-        self.logger.debug('Creating an ISAMAppliance')
-        if isinstance(lmi_port, basestring):
+        self.debug = debug
+        if self.debug: self.logger.debug('Creating an ISAMAppliance')
+        if isinstance(lmi_port, str):
             self.lmi_port = int(lmi_port)
         else:
             self.lmi_port = lmi_port
+        self.hostname = hostname
         self.session = requests.session()
-        if cert is None:
+
+        # If we did not get a value for verify, try the environment variable
+        if verify is None:
+            verify = str(environ.get("IBMSECLIB_VERIFY_CONNECTION", False)).lower() in ["true", "yes"]
+
+        self.cert = cert
+
+        self.disable_urllib_warnings = False
+        if self.cert is None:
             self.logger.debug('Cert object is None, using BA Auth with userid/password.')
             self.session.auth = (user.username, user.password)
         else:
             self.logger.debug('Using cert based auth, since cert object is not None.')
-            self.session.cert = cert
+            self.session.cert = self.cert
+
+        self._set_ssl_verification(requests_verify_param=verify)
+
         IBMAppliance.__init__(self, hostname, user)
 
+    def _set_ssl_verification(self, requests_verify_param):
+        self.verify = requests_verify_param
+        self.session.verify = self.verify
+        if self.verify is None or self.verify is False:
+            self.disable_urllib_warnings = True
+            self.logger.warning("""
+Certificate verification has been disabled. Python is NOT verifying the SSL 
+certificate of the host appliance and InsecureRequestWarning messages are 
+being suppressed for the following host:
+  https://{0}:{1}
+
+To use certificate verification:
+  1. When the certificate is trusted by your Python environment:
+        Instantiate all instances of ISAMAppliance with verify=True or set 
+        the environment variable IBMSECLIB_VERIFY_CONNECTION=True.
+  2. When the certificate is not already trusted in your Python environment:
+        Instantiate all instances of ISAMAppliance with the verify parameter
+        set to the fully qualified path to a CA bundle.
+        
+See the following URL for more details:
+  https://requests.readthedocs.io/en/latest/user/advanced/#ssl-cert-verification
+""".format(self.hostname, self.lmi_port))
+
     def _url(self, uri):
         # Build up the URL
         url = "https://" + self.hostname + ":" + str(self.lmi_port) + uri
-        self.logger.debug("Issuing request to: " + url)
+        if self.debug: self.logger.debug("Issuing request to: " + url)
 
         return url
 
     def _log_desc(self, description):
         if description != "":
             self.logger.info('*** ' + description + ' ***')
 
     def _suppress_ssl_warning(self):
+        # If we have trust setup correctly, we do not want to suppress these warnings.
+        if not self.disable_urllib_warnings:
+            return
+
         # Disable https warning because of non-standard certs on appliance
         try:
-            self.logger.debug("Suppressing SSL Warnings.")
+            if self.debug: self.logger.debug("Suppressing SSL Warnings.")
             requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
         except AttributeError:
             self.logger.warning("load requests.packages.urllib3.disable_warnings() failed")
 
     def _process_response(self, return_obj, http_response, ignore_error):
 
+        # return_obj['rsp'] = http_response # Do not add this - breaks the ISAM Collection's connection
         return_obj['rc'] = http_response.status_code
 
         # Examine the response.
         if (http_response.status_code == 403):
             self.logger.error("  Request failed: ")
             self.logger.error("     status code: {0}".format(http_response.status_code))
             if http_response.text != "":
@@ -75,61 +118,84 @@
             return_obj['rc'] = 0
 
         # Handle if there was json on input but response was not in json format
         try:
             json_data = json.loads(http_response.text)
             return_obj['data'] = json_data
         except ValueError:
-            try:
-                json_data = json.loads(http_response.content.decode("utf-8"))
-                return_obj['data'] = json_data
-            except UnicodeDecodeError:
+            return_obj['data'] = http_response.content
+            return
+
+        if self.debug: self.logger.debug("Status Code: {0}".format(http_response.status_code))
+        if http_response.text != "":
+            if self.debug: self.logger.debug("Text: " + http_response.content.decode("utf-8"))
+
+        for key in http_response.headers:
+            if key == 'g-type':
+                if http_response.headers[key] == 'application/octet-stream; charset=UTF-8':
+                    json_data = {}
+                    return_obj.data = http_response.content
+                    return
+
+        if http_response.text == "":
+            json_data = {}
+        else:
+            json_data = json.loads(http_response.text)
+
+        return_obj['data'] = json_data
+        try:
+            json_data = json.loads(http_response.content.decode("utf-8"))
+            return_obj['data'] = json_data
+        except UnicodeDecodeError:
+            return_obj['data'] = http_response.content
+        except ValueError:
+            if isinstance(http_response.content, bytes):
+                return_obj['data'] = http_response.content.decode("utf-8")
+            else:
                 return_obj['data'] = http_response.content
-            except ValueError:
-                if isinstance(http_response.content, bytes):
-                    return_obj['data'] = http_response.content.decode("utf-8")
-                else:
-                    return_obj['data'] = http_response.content
 
     def _process_connection_error(self, ignore_error, return_obj):
         if not ignore_error:
             self.logger.critical("Failed to connect to server.")
             raise IBMError("HTTP Return code: 502", "Failed to connect to server")
         else:
             self.logger.debug("Failed to connect to server.")
             return_obj['rc'] = 502
 
     def _process_warnings(self, uri, requires_modules, requires_version, requires_model, warnings=[]):
         # flag to indicate if processing needs to return and not continue
         return_call = False
+        if self.debug: self.logger.debug("Checking for minimum version: {0}.".format(requires_version))
+
         self.logger.debug("Checking for deployment model {0}.".format(requires_model))
         if requires_model is not None and 'model' in self.facts and self.facts['model'] is not None:
             if self.facts['model'] != requires_model:
                 return_call = True
                 warnings.append(
                     "API invoked requires model: {0}, appliance is of deployment model: {1}.".format(
                         requires_model, self.facts['model']))
 
         self.logger.debug("Checking for minimum version: {0}.".format(requires_version))
+
         if requires_version is not None and 'version' in self.facts and self.facts['version'] is not None:
             if tools.version_compare(self.facts['version'], requires_version) < 0:
                 return_call = True
                 warnings.append(
                     "API invoked requires minimum version: {0}, appliance is of lower version: {1}.".format(
                         requires_version, self.facts['version']))
         # Detecting modules from uri if none is provided
         if requires_modules is None and not requires_modules:
             if uri.startswith("/wga"):
                 requires_modules = ['wga']
-                self.logger.debug("Detected module: {0} from uri: {1}.".format(requires_modules, uri))
+                if self.debug: self.logger.debug("Detected module: {0} from uri: {1}.".format(requires_modules, uri))
             elif uri.startswith("/mga"):
                 requires_modules = ['mga']
-                self.logger.debug("Detected module: {0} from uri: {1}.".format(requires_modules, uri))
+                if self.debug: self.logger.debug("Detected module: {0} from uri: {1}.".format(requires_modules, uri))
 
-        self.logger.debug("Checking for one of required modules: {0}.".format(requires_modules))
+        if self.debug: self.logger.debug("Checking for one of required modules: {0}.".format(requires_modules))
         if requires_modules is not None and requires_modules:
             if 'activations' in self.facts and self.facts['activations']:
                 # Find intersection of the two lists
                 iactive = [ia for ia in self.facts['activations'] if ia in requires_modules]
                 if not iactive:
                     return_call = True
                     warnings.append(
@@ -138,15 +204,15 @@
                 else:
                     self.logger.info("Modules satisfying requirement: {0}".format(iactive))
             else:
                 return_call = True
                 warnings.append("API invoked requires module: {0}, appliance has no modules active.".format(
                     requires_modules))
 
-        self.logger.debug("Warnings: {0}".format(warnings))
+        if self.debug: self.logger.debug("Warnings: {0}".format(warnings))
         return warnings, return_call
 
     def invoke_post_files(self, description, uri, fileinfo, data, ignore_error=False, requires_modules=None,
                           requires_version=None, warnings=[], json_response=True, data_as_files=False,
                           requires_model=None):
         """
         Send multipart/form-data upload file request to the appliance.
@@ -165,41 +231,41 @@
             headers = {
                 'Accept': 'application/json,text/html,application/xhtml+xml,application/xml'
             }
         else:
             headers = {
                 'Accept': 'text/html,application/xhtml+xml,application/xml'
             }
-        self.logger.debug("Headers are: {0}".format(headers))
+        if self.debug: self.logger.debug("Headers are: {0}".format(headers))
 
         if data_as_files is False:
             files = list()
             for file2post in fileinfo:
                 files.append((file2post['file_formfield'],
                               (tools.path_leaf(file2post['filename']), open(file2post['filename'], 'rb'),
                                file2post['mimetype'])))
         else:
             files = data
 
         self._suppress_ssl_warning()
 
         try:
             if data_as_files is False:
-                r = self.session.post(url=self._url(uri=uri), data=data, files=files, verify=False, headers=headers)
+                r = self.session.post(url=self._url(uri=uri), data=data, files=files, headers=headers)
             else:
-                r = self.session.post(url=self._url(uri=uri), files=files, verify=False, headers=headers)
+                r = self.session.post(url=self._url(uri=uri), files=files, headers=headers)
             return_obj['changed'] = True  # POST of file would be a change
             self._process_response(return_obj=return_obj, http_response=r, ignore_error=ignore_error)
 
         except requests.exceptions.ConnectionError:
             if not ignore_error:
                 self.logger.critical("Failed to connect to server.")
                 raise IBMError("HTTP Return code: 502", "Failed to connect to server")
             else:
-                self.logger.debug("Failed to connect to server.")
+                if self.debug: self.logger.debug("Failed to connect to server.")
                 return_obj.rc = 502
 
         return return_obj
 
     def invoke_put_files(self, description, uri, fileinfo, data, ignore_error=False, requires_modules=None,
                          requires_version=None, warnings=[], requires_model=None):
         """
@@ -214,35 +280,35 @@
         if return_call:
             return return_obj
 
         # Build up the URL and header information.
         headers = {
             'Accept': 'application/json,text/html,application/xhtml+xml,application/xml'
         }
-        self.logger.debug("Headers are: {0}".format(headers))
+        if self.debug: self.logger.debug("Headers are: {0}".format(headers))
 
         files = list()
 
         for file2post in fileinfo:
             files.append((file2post['file_formfield'],
                           (file2post['filename'], open(file2post['filename'], 'rb'), file2post['mimetype'])))
 
         self._suppress_ssl_warning()
 
         try:
-            r = self.session.put(url=self._url(uri=uri), data=data, files=files, verify=False, headers=headers)
+            r = self.session.put(url=self._url(uri=uri), data=data, files=files, headers=headers)
             return_obj['changed'] = True  # POST of file would be a change
             self._process_response(return_obj=return_obj, http_response=r, ignore_error=ignore_error)
 
         except requests.exceptions.ConnectionError:
             if not ignore_error:
                 self.logger.critical("Failed to connect to server.")
                 raise IBMError("HTTP Return code: 502", "Failed to connect to server")
             else:
-                self.logger.debug("Failed to connect to server.")
+                if self.debug: self.logger.debug("Failed to connect to server.")
                 return_obj.rc = 502
 
         return return_obj
 
     def invoke_get_file(self, description, uri, filename, no_headers=False, ignore_error=False, requires_modules=None,
                         requires_version=None, warnings=[], requires_model=None):
         """
@@ -260,20 +326,20 @@
         # In some cases passing a header causes response to come back as JSON
         if no_headers is True:
             headers = {}
         else:
             headers = {
                 'Accept': 'application/json,application/octet-stream'
             }
-        self.logger.debug("Headers are: {0}".format(headers))
+            if self.debug: self.logger.debug("Headers are: {0}".format(headers))
 
         self._suppress_ssl_warning()
 
         try:
-            r = self.session.get(url=self._url(uri=uri), verify=False, stream=True, headers=headers)
+            r = self.session.get(url=self._url(uri=uri), stream=True, headers=headers)
 
             if (r.status_code != 200 and r.status_code != 204 and r.status_code != 201):
                 self.logger.error("  Request failed: ")
                 self.logger.error("     status code: {0}".format(r.status_code))
                 if r.text != "":
                     self.logger.error("     text: " + r.text)
                 if not ignore_error:
@@ -293,15 +359,15 @@
             self._process_connection_error(ignore_error=ignore_error, return_obj=return_obj)
 
         except IOError:
             if not ignore_error:
                 self.logger.critical("Failed to write to file: " + filename)
                 raise IBMError("HTTP Return code: 999", "Failed to write to file: " + filename)
             else:
-                self.logger.debug("Failed to write to file: " + filename)
+                if self.debug: self.logger.debug("Failed to write to file: " + filename)
                 return_obj['rc'] = 999
 
         return return_obj
 
     def _invoke_request(self, func, description, uri, ignore_error, data={}, requires_modules=None,
                         requires_version=None, warnings=[], requires_model=None):
         """
@@ -320,33 +386,32 @@
             return return_obj
 
         # There maybe some cases when header should be blank (not json)
         headers = {
             'Accept': 'application/json',
             'Content-type': 'application/json'
         }
-        self.logger.debug("Headers are: {0}".format(headers))
+        if self.debug: self.logger.debug("Headers are: {0}".format(headers))
 
         # Process the input data into JSON
         json_data = json.dumps(data)
 
-        self.logger.debug("Input Data: " + json_data)
+        if self.debug: self.logger.debug("Input Data: " + json_data)
 
         self._suppress_ssl_warning()
 
         try:
             if func == self.session.get or func == self.session.delete:
-
                 if data != {}:
-                    r = func(url=self._url(uri), data=json_data, verify=False, headers=headers)
+                    r = func(url=self._url(uri), data=json_data, headers=headers, verify=self.verify)
                 else:
-                    r = func(url=self._url(uri), verify=False, headers=headers)
+                    r = func(url=self._url(uri), headers=headers, verify=self.verify)
             else:
                 r = func(url=self._url(uri), data=json_data,
-                         verify=False, headers=headers)
+                         headers=headers, verify=self.verify, cert=self.cert)
 
             if func != self.session.get:
                 return_obj['changed'] = True  # Anything but GET should result in change
 
             self._process_response(return_obj=return_obj, http_response=r, ignore_error=ignore_error)
 
         except requests.exceptions.ConnectionError:
@@ -378,20 +443,20 @@
 
         self._suppress_ssl_warning()
 
         try:
             if func == self.session.get or func == self.session.delete:
 
                 if data != {}:
-                    r = func(url=self._url(uri), data=json_data, verify=False, headers=headers)
+                    r = func(url=self._url(uri), data=json_data, headers=headers)
                 else:
-                    r = func(url=self._url(uri), verify=False, headers=headers)
+                    r = func(url=self._url(uri), headers=headers)
             else:
                 r = func(url=self._url(uri), data=json_data,
-                         verify=False, headers=headers)
+                         headers=headers, verify=self.verify, cert=self.cert)
 
             if func != self.session.get:
                 return_obj['changed'] = True  # Anything but GET should result in change
 
             self._process_response(return_obj=return_obj, http_response=r, ignore_error=ignore_error)
 
         except requests.exceptions.ConnectionError:
@@ -443,20 +508,20 @@
             return return_obj
 
         headers = {
             'Accept': '*/*',
             'Accept-Encoding': 'gzip, deflate, br',
             'Content-Type': 'application/x-www-form-urlencoded'
         }
-        self.logger.debug("Headers are: {0}".format(headers))
+        if self.debug: self.logger.debug("Headers are: {0}".format(headers))
 
         self._suppress_ssl_warning()
 
         try:
-            r = self.session.post(url=self._url(uri=uri), data=data, verify=False, headers=headers)
+            r = self.session.post(url=self._url(uri=uri), data=data, headers=headers)
             return_obj['changed'] = False  # POST of snapshot id would not be a change
             self._process_response(return_obj=return_obj, http_response=r, ignore_error=ignore_error)
 
         except requests.exceptions.ConnectionError:
             if not ignore_error:
                 self.logger.critical("Failed to connect to server.")
                 raise IBMError("HTTP Return code: 502", "Failed to connect to server")
@@ -531,32 +596,32 @@
             return return_obj
 
         args = {}
 
         for key, value in kwargs.items():
             if key == 'json' and value != {}:
                 json_data = json.dumps(value)
-                self.logger.debug("Input json Data: " + json_data)
+                if self.debug: self.logger.debug("Input json Data: " + json_data)
                 args['json'] = json_data
             elif key == 'data':
                 try:
                     json.loads(value)
-                    self.logger.debug("Input Data: " + value)
+                    if self.debug: self.logger.debug("Input Data: " + value)
                     args['data'] = value
                 except ValueError:
-                    self.logger.debug("Input Data: " + value)
+                    if self.debug: self.logger.debug("Input Data: " + value)
                     args['data'] = value
             else:
                 args[key] = value
 
         self._suppress_ssl_warning()
 
         try:
             streaminargs = False
-            r = self.session.request(method, url=self._url(uri), verify=False, **args)
+            r = self.session.request(method, url=self._url(uri), **args)
             # check for stream=True
             if "stream" in args and args["stream"] == True:
                 streaminargs = True
                 if filename == None:
                     return_obj['warnings'] = return_obj['warnings'].append(
                         "filename is missing, for stream=True, filename needs to be non null")
                     return return_obj
@@ -605,16 +670,18 @@
             import ibmsecurity.isam.base.setup_complete
             ret_obj = ibmsecurity.isam.base.setup_complete.get(self)
             if ret_obj['data'].get('configured') is True:
                 self.get_activations()
         # Be sure to let fatal error unconditionally percolate up the stack
         except IBMFatal:
             raise
+
         # Exceptions like those connection related will be ignored
-        except:
+        except Exception as e:
+            self.logger.error( traceback.print_exc() )
             pass
 
     def get_version(self):
         """
         Get appliance version (versions API or active partition)
 
         When firmware are installed or partition are changed, then this value is updated
@@ -643,22 +710,24 @@
                 if 'firmware_label' in ret_obj['data']:
                     self.facts['firmware_label'] = ret_obj['data']['firmware_label']
 
         # Be sure to let fatal error unconditionally percolate up the stack
         except IBMFatal:
             raise
         except IBMError:
+            self.logger.error( traceback.print_exc() )
             try:
                 ret_obj = ibmsecurity.isam.base.firmware.get(self)
                 for partition in ret_obj['data']:
                     if partition['active'] is True:
                         ver = partition['firmware_version'].split(' ')
                         self.facts['version'] = ver[-1]
                 self.facts['model'] = "Appliance"
             except:
+                self.logger.error( traceback.print_exc() )
                 pass
         return
 
     def get_activations(self):
         """
         Get  appliance activations
```

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/appliance/isamappliance_adminproxy.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/appliance/isamappliance_adminproxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.logger = logging.getLogger(__name__)
         self.logger.debug('Creating an ISAMAppliance over AdminProxy')
 
         self.adminProxyProtocol = adminProxyProtocol
         self.adminProxyHostname = adminProxyHostname
 
         # Type checking and tranformation to safely reuse this variable later on
-        if isinstance(adminProxyPort, basestring):
+        if isinstance(adminProxyPort, str):
             self.adminProxyPort = int(adminProxyPort)
         else:
             self.adminProxyPort = adminProxyPort
 
         self.adminProxyApplianceShortName = adminProxyApplianceShortName
 
         ISAMAppliance.__init__(self, hostname, user, cert=cert)
```

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/appliance/isdsappliance.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/appliance/isdsappliance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,118 @@
 import json
 import requests
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 import logging
 from .ibmappliance import IBMAppliance
 from .ibmappliance import IBMError
+from .ibmappliance import IBMFatal
 from ibmsecurity.utilities import tools
 from io import open
+from os import environ
 
 try:
     basestring
 except NameError:
-
     basestring = (str, bytes)
 
 
 class ISDSAppliance(IBMAppliance):
-    def __init__(self, hostname, user, lmi_port=443):
+    def __init__(self, hostname, user, lmi_port=443, verify=None):
         self.logger = logging.getLogger(__name__)
         self.logger.debug('Creating an ISDSAppliance')
         if isinstance(lmi_port, basestring):
             self.lmi_port = int(lmi_port)
         else:
             self.lmi_port = lmi_port
+        self.hostname = hostname
+        self.session = requests.session()
+
+        # If we did not get a value for verify, try the environment variable
+        if verify is None:
+            verify = str(environ.get("IBMSECLIB_VERIFY_CONNECTION", False)).lower() in ["true", "yes"]
+
+        self.cert = cert
+
+        self.disable_urllib_warnings = False
+        if self.cert is None:
+            self.logger.debug('Cert object is None, using BA Auth with userid/password.')
+            self.session.auth = (user.username, user.password)
+        else:
+            self.logger.debug('Using cert based auth, since cert object is not None.')
+            self.session.cert = self.cert
+
+        self._set_ssl_verification(requests_verify_param=verify)
 
         IBMAppliance.__init__(self, hostname, user)
 
+    def _set_ssl_verification(self, requests_verify_param):
+        self.verify = requests_verify_param
+        self.session.verify = self.verify
+        if self.verify is None or self.verify is False:
+            self.disable_urllib_warnings = True
+            self.logger.warning("""
+Certificate verification has been disabled. Python is NOT verifying the SSL 
+certificate of the host appliance and InsecureRequestWarning messages are 
+being suppressed for the following host:
+  https://{0}:{1}
+
+To use certificate verification:
+  1. When the certificate is trusted by your Python environment:
+        Instantiate all instances of ISDSAppliance with verify=True or set 
+        the environment variable IBMSECLIB_VERIFY_CONNECTION=True.
+  2. When the certificate is not already trusted in your Python environment:
+        Instantiate all instances of ISAMAppliance with the verify parameter
+        set to the fully qualified path to a CA bundle.
+        
+See the following URL for more details:
+  https://requests.readthedocs.io/en/latest/user/advanced/#ssl-cert-verification
+""".format(self.hostname, self.lmi_port))
+
     def _url(self, uri):
         # Build up the URL
         url = "https://" + self.hostname + ":" + str(self.lmi_port) + uri
         self.logger.debug("Issuing request to: " + url)
 
         return url
 
     def _log_desc(self, description):
         if description != "":
             self.logger.info('*** ' + description + ' ***')
 
     def _suppress_ssl_warning(self):
+        # If we have trust setup correctly, we do not want to suppress these warnings.
+        if not self.disable_urllib_warnings:
+            return
+
         # Disable https warning because of non-standard certs on appliance
         try:
-            self.logger.debug("Suppressing SSL Warnings.")
+            self.logger.warning("Suppressing SSL Warnings.")
             requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
         except AttributeError:
             self.logger.warning("load requests.packages.urllib3.disable_warnings() failed")
 
     def _process_response(self, return_obj, http_response, ignore_error):
 
+        return_obj['rsp'] = http_response
         return_obj['rc'] = http_response.status_code
 
         # Examine the response.
         if (http_response.status_code != 200 and http_response.status_code != 204 and http_response.status_code != 201):
             self.logger.error("  Request failed: ")
             self.logger.error("     status code: {0}".format(http_response.status_code))
             if http_response.text != "":
                 self.logger.error("     text: " + http_response.text)
             if not ignore_error:
                 raise IBMError("HTTP Return code: {0}".format(http_response.status_code), http_response.text)
             return_obj['changed'] = False  # force changed to be False as there is an error
         else:
             return_obj['rc'] = 0
 
-            # Handle if there was json on input but response was not in json format
+        # Handle if there was json on input but response was not in json format
+        json_data = {}
         try:
             json_data = json.loads(http_response.text)
         except ValueError:
             return_obj['data'] = http_response.content
             return
 
         self.logger.debug("Status Code: {0}".format(http_response.status_code))
@@ -74,17 +122,15 @@
         for key in http_response.headers:
             if key == 'g-type':
                 if http_response.headers[key] == 'application/octet-stream; charset=UTF-8':
                     json_data = {}
                     return_obj.data = http_response.content
                     return
 
-        if http_response.text == "":
-            json_data = {}
-        else:
+        if http_response.text != "":
             json_data = json.loads(http_response.text)
 
         return_obj['data'] = json_data
 
     def _process_connection_error(self, ignore_error, return_obj):
         if not ignore_error:
             self.logger.critical("Failed to connect to server.")
@@ -163,15 +209,15 @@
                           (tools.path_leaf(file2post['filename']), open(file2post['filename'], 'rb'),
                            file2post['mimetype'])))
 
         self._suppress_ssl_warning()
 
         try:
             r = requests.post(url=self._url(uri=uri), data=data, auth=(self.user.username, self.user.password),
-                              files=files, verify=False, headers=headers)
+                              files=files, verify=self.verify, headers=headers)
             return_obj['changed'] = True  # POST of file would be a change
             self._process_response(return_obj=return_obj, http_response=r, ignore_error=ignore_error)
 
         except requests.exceptions.ConnectionError:
             if not ignore_error:
                 self.logger.critical("Failed to connect to server.")
                 raise IBMError("HTTP Return code: 502", "Failed to connect to server")
@@ -207,15 +253,15 @@
             files.append((file2post['file_formfield'],
                           (file2post['filename'], open(file2post['filename'], 'rb'), file2post['mimetype'])))
 
         self._suppress_ssl_warning()
 
         try:
             r = requests.put(url=self._url(uri=uri), data=data, auth=(self.user.username, self.user.password),
-                             files=files, verify=False, headers=headers)
+                             files=files, verify=self.verify, headers=headers)
             return_obj['changed'] = True  # POST of file would be a change
             self._process_response(return_obj=return_obj, http_response=r, ignore_error=ignore_error)
 
         except requests.exceptions.ConnectionError:
             if not ignore_error:
                 self.logger.critical("Failed to connect to server.")
                 raise IBMError("HTTP Return code: 502", "Failed to connect to server")
@@ -247,15 +293,15 @@
                 'Accept': 'application/json,application/octet-stream'
             }
         self.logger.debug("Headers are: {0}".format(headers))
 
         self._suppress_ssl_warning()
 
         try:
-            r = requests.get(url=self._url(uri=uri), auth=(self.user.username, self.user.password), verify=False,
+            r = requests.get(url=self._url(uri=uri), auth=(self.user.username, self.user.password), verify=self.verify,
                              stream=True, headers=headers)
 
             if (r.status_code != 200 and r.status_code != 204 and r.status_code != 201):
                 self.logger.error("  Request failed: ")
                 self.logger.error("     status code: {0}".format(r.status_code))
                 if r.text != "":
                     self.logger.error("     text: " + r.text)
@@ -315,22 +361,22 @@
         self._suppress_ssl_warning()
 
         try:
             if func == requests.get or func == requests.delete:
 
                 if data != {}:
                     r = func(url=self._url(uri), data=json_data, auth=(self.user.username, self.user.password),
-                             verify=False, headers=headers)
+                             verify=self.verify, headers=headers)
                 else:
                     r = func(url=self._url(uri), auth=(self.user.username, self.user.password),
-                             verify=False, headers=headers)
+                             verify=self.verify, headers=headers)
             else:
                 r = func(url=self._url(uri), data=json_data,
                          auth=(self.user.username, self.user.password),
-                         verify=False, headers=headers)
+                         verify=self.verify, headers=headers)
 
             if func != requests.get:
                 return_obj['changed'] = True  # Anything but GET should result in change
 
             self._process_response(return_obj=return_obj, http_response=r, ignore_error=ignore_error)
 
         except requests.exceptions.ConnectionError:
```

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/appliance/isdsappliance_adminproxy.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/appliance/isdsappliance_adminproxy.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/appliance/isvgappliance.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/appliance/isvgappliance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,78 +1,126 @@
 import json
 import requests
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 import logging
 from .ibmappliance import IBMAppliance
 from .ibmappliance import IBMError
+from .ibmappliance import IBMFatal
 from ibmsecurity.utilities import tools
 from io import open
+from os import environ
 
 try:
     basestring
 except NameError:
-
     basestring = (str, bytes)
 
 
 class ISVGAppliance(IBMAppliance):
-    def __init__(self, hostname, user, lmi_port=443):
+    def __init__(self, hostname, user, lmi_port=443, verify=None):
         self.logger = logging.getLogger(__name__)
         self.logger.debug('Creating an ISVGAppliance')
         if isinstance(lmi_port, basestring):
             self.lmi_port = int(lmi_port)
         else:
             self.lmi_port = lmi_port
+        self.hostname = hostname
+        self.session = requests.session()
+
+        # If we did not get a value for verify, try the environment variable
+        if verify is None:
+            verify = str(environ.get("IBMSECLIB_VERIFY_CONNECTION", False)).lower() in ["true", "yes"]
+
+        self.cert = cert
+
+        self.disable_urllib_warnings = False
+        if self.cert is None:
+            self.logger.debug('Cert object is None, using BA Auth with userid/password.')
+            self.session.auth = (user.username, user.password)
+        else:
+            self.logger.debug('Using cert based auth, since cert object is not None.')
+            self.session.cert = self.cert
+
+        self._set_ssl_verification(requests_verify_param=verify)
 
         IBMAppliance.__init__(self, hostname, user)
 
+    def _set_ssl_verification(self, requests_verify_param):
+        self.verify = requests_verify_param
+        self.session.verify = self.verify
+        if self.verify is None or self.verify is False:
+            self.disable_urllib_warnings = True
+            self.logger.warning("""
+Certificate verification has been disabled. Python is NOT verifying the SSL 
+certificate of the host appliance and InsecureRequestWarning messages are 
+being suppressed for the following host:
+  https://{0}:{1}
+
+To use certificate verification:
+  1. When the certificate is trusted by your Python environment:
+        Instantiate all instances of ISVGAppliance with verify=True or set 
+        the environment variable IBMSECLIB_VERIFY_CONNECTION=True.
+  2. When the certificate is not already trusted in your Python environment:
+        Instantiate all instances of ISAMAppliance with the verify parameter
+        set to the fully qualified path to a CA bundle.
+        
+See the following URL for more details:
+  https://requests.readthedocs.io/en/latest/user/advanced/#ssl-cert-verification
+""".format(self.hostname, self.lmi_port))
+
     def _url(self, uri):
         # Build up the URL
         url = "https://" + self.hostname + ":" + str(self.lmi_port) + uri
         self.logger.debug("Issuing request to: " + url)
 
         return url
 
     def _log_desc(self, description):
         if description != "":
             self.logger.info('*** ' + description + ' ***')
 
     def _suppress_ssl_warning(self):
+        # If we have trust setup correctly, we do not want to suppress these warnings.
+        if not self.disable_urllib_warnings:
+            return
+
         # Disable https warning because of non-standard certs on appliance
         try:
-            self.logger.debug("Suppressing SSL Warnings.")
+            self.logger.warning("Suppressing SSL Warnings.")
             requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
         except AttributeError:
             self.logger.warning("load requests.packages.urllib3.disable_warnings() failed")
 
     def _process_response(self, return_obj, http_response, ignore_error):
 
+        return_obj['rsp'] = http_response
         return_obj['rc'] = http_response.status_code
 
         # Examine the response.
         if (http_response.status_code == 302):
-            self.logger.warning("  Endpoint cannot be use at this time: ")
+            self.logger.warning("  Endpoint cannot be used at this time: ")
             self.logger.warning("     status code: {0}".format(http_response.status_code))
             if http_response.text != "":
                 self.logger.error("     text: " + http_response.text)
-            # Too early to use this endppoint.
+            # Too early to use this endpoint.
             return_obj['changed'] = False
             return_obj['rc'] = 0
         elif (http_response.status_code != 200 and http_response.status_code != 204 and http_response.status_code != 201):
             self.logger.error("  Request failed: ")
             self.logger.error("     status code: {0}".format(http_response.status_code))
             if http_response.text != "":
                 self.logger.error("     text: " + http_response.text)
             if not ignore_error:
                 raise IBMError("HTTP Return code: {0}".format(http_response.status_code), http_response.text)
             return_obj['changed'] = False  # force changed to be False as there is an error
         else:
             return_obj['rc'] = 0
 
         # Handle if there was json on input but response was not in json format
+        json_data = {}
         try:
             json_data = json.loads(http_response.text)
         except ValueError:
             return_obj['data'] = http_response.content
             return
 
         self.logger.debug("Status Code: {0}".format(http_response.status_code))
@@ -82,17 +130,15 @@
         for key in http_response.headers:
             if key == 'g-type':
                 if http_response.headers[key] == 'application/octet-stream; charset=UTF-8':
                     json_data = {}
                     return_obj.data = http_response.content
                     return
 
-        if http_response.text == "":
-            json_data = {}
-        else:
+        if http_response.text != "":
             json_data = json.loads(http_response.text)
 
         return_obj['data'] = json_data
 
     def _process_connection_error(self, ignore_error, return_obj):
         if not ignore_error:
             self.logger.critical("Failed to connect to server.")
@@ -171,15 +217,15 @@
                           (tools.path_leaf(file2post['filename']), open(file2post['filename'], 'rb'),
                            file2post['mimetype'])))
 
         self._suppress_ssl_warning()
 
         try:
             r = requests.post(url=self._url(uri=uri), data=data, auth=(self.user.username, self.user.password),
-                              files=files, verify=False, headers=headers)
+                              files=files, verify=self.verify, headers=headers)
             return_obj['changed'] = True  # POST of file would be a change
             self._process_response(return_obj=return_obj, http_response=r, ignore_error=ignore_error)
 
         except requests.exceptions.ConnectionError:
             if not ignore_error:
                 self.logger.critical("Failed to connect to server.")
                 raise IBMError("HTTP Return code: 502", "Failed to connect to server")
@@ -215,15 +261,15 @@
             files.append((file2post['file_formfield'],
                           (file2post['filename'], open(file2post['filename'], 'rb'), file2post['mimetype'])))
 
         self._suppress_ssl_warning()
 
         try:
             r = requests.put(url=self._url(uri=uri), data=data, auth=(self.user.username, self.user.password),
-                             files=files, verify=False, headers=headers)
+                             files=files, verify=self.verify, headers=headers)
             return_obj['changed'] = True  # POST of file would be a change
             self._process_response(return_obj=return_obj, http_response=r, ignore_error=ignore_error)
 
         except requests.exceptions.ConnectionError:
             if not ignore_error:
                 self.logger.critical("Failed to connect to server.")
                 raise IBMError("HTTP Return code: 502", "Failed to connect to server")
@@ -259,15 +305,15 @@
                 'Accept': mime_types
             }
         self.logger.debug("Headers are: {0}".format(headers))
 
         self._suppress_ssl_warning()
 
         try:
-            r = requests.get(url=self._url(uri=uri), auth=(self.user.username, self.user.password), verify=False,
+            r = requests.get(url=self._url(uri=uri), auth=(self.user.username, self.user.password), verify=self.verify,
                              stream=True, headers=headers, allow_redirects=False)
 
             if (r.status_code != 200 and r.status_code != 204 and r.status_code != 201):
                 self.logger.error("  Request failed: ")
                 self.logger.error("     status code: {0}".format(r.status_code))
                 if r.text != "":
                     self.logger.error("     text: " + r.text)
@@ -327,22 +373,22 @@
         self._suppress_ssl_warning()
 
         try:
             if func == requests.get or func == requests.delete:
 
                 if data != {}:
                     r = func(url=self._url(uri), data=json_data, auth=(self.user.username, self.user.password),
-                             verify=False, headers=headers, allow_redirects=False)
+                             verify=self.verify, headers=headers, allow_redirects=False)
                 else:
                     r = func(url=self._url(uri), auth=(self.user.username, self.user.password),
-                             verify=False, headers=headers, allow_redirects=False)
+                             verify=self.verify, headers=headers, allow_redirects=False)
             else:
                 r = func(url=self._url(uri), data=json_data,
                          auth=(self.user.username, self.user.password),
-                         verify=False, headers=headers)
+                         verify=self.verify, headers=headers)
 
             if func != requests.get:
                 return_obj['changed'] = True  # Anything but GET should result in change
 
             self._process_response(return_obj=return_obj, http_response=r, ignore_error=ignore_error)
 
         except requests.exceptions.ConnectionError:
```

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/appliance/isvgappliance_adminproxy.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/appliance/isvgappliance_adminproxy.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/access_control/policies.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/access_control/policies.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/access_control/policy_attachments.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/access_control/policy_attachments.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/access_control/policy_sets.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/access_control/policy_sets.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/access_policy.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/access_policy.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/advanced_configuration.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/advanced_configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/api_protection/clients.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/api_protection/clients.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/api_protection/definitions.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/api_protection/definitions.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/api_protection/dynamic_clients.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/api_protection/dynamic_clients.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/api_protection/dynamic_clients_migration.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/api_protection/dynamic_clients_migration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/api_protection/grants.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/api_protection/grants.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/api_protection/grants_user.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/api_protection/grants_user.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/attribute_matchers.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/attribute_matchers.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 
 def _check(isamAppliance, description, properties):
     """
     Check and return True if update needed
     """
     update_required = False
     ret_obj = get(isamAppliance, description)
+    json_data = {}
     if ret_obj['data'] == {}:
         logger.warning("Attribute Matcher not found, returning no update required.")
         return None, update_required, json_data
     else:
         json_data = {
             "properties": properties,
             "predefined": ret_obj['data']['predefined'],
```

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/attributes.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/attributes.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/mechanism_types.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/mechanism_types.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/mechanisms.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/mechanisms.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/policies.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/policies.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/all.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/rsa_otp/all.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdconf.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdconf.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdopts.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdopts.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/securid.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/rsa_otp/securid.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/authentication/rsa_otp.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/authentication/rsa_otp.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/database.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/database.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/devices/fingerprints.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/devices/fingerprints.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/devices/userids.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/devices/userids.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/extensions.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/extensions.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/fido2/metadata.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/fido2/metadata.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/fido2/metadata_services.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/fido2/metadata_services.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/fido2/registrations.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/fido2/registrations.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/fido2/relying_parties.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/fido2/relying_parties.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/fido2/u2f_migration.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/fido2/u2f_migration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/mapping_rules.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/mapping_rules.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/mmfa/configuration.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/mmfa/configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/mmfa/push_notification_registration.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/mmfa/push_notification_registration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/mmfa/transactions.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/mmfa/transactions.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/obligation_types.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/obligation_types.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/obligations.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/obligations.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/password_vault.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/password_vault.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/all.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/all.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/database.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/database.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/fiberlink.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/fiberlink.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/javascript.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/javascript.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/ldap.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/ldap.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/qradar.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/qradar.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/restful.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/restful.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/policy_information_points/types.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/policy_information_points/types.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/risk_profiles.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/risk_profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
 
 def _check(isamAppliance, name, active, description, attributes, predefined):
     """
     Check and return True if update needed
     """
     update_required = False
     ret_obj = get(isamAppliance, name)
+    json_data = {}
     if ret_obj['data'] == {}:
         logger.warning("Risk Profile not found, returning no update required.")
         return None, update_required, json_data
     else:
         if ret_obj['data']['predefined'] is True:
             logger.warning("Predefined Risk Profiles can NOT be updated, returning no update required.")
             return ret_obj['data']['id'], update_required, {}
```

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/runtime_template/directory.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/runtime_template/directory.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/runtime_template/file.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/runtime_template/file.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/runtime_template/root.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/runtime_template/root.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/enterprise_profile.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/enterprise_profile.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/ext_auth_service.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/ext_auth_service.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/general.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/general.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/group.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/group.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/isam_user.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/isam_user.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/ldap_attrs.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/ldap_attrs.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/ldap_objs.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/ldap_objs.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/mode.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/mode.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/scim.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/scim.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim/user_profile.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim/user_profile.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/scim_custom_schema_extensions.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/scim_custom_schema_extensions.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/ci.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/ci.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/connection.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/connection.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/isamruntime.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/isamruntime.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/jdbc.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/jdbc.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/ldap.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/ldap.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/redis.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/redis.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/smtp.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/smtp.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/server_connections/ws.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/server_connections/ws.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/user_info.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/user_info.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/user_registry/group.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/user_registry/group.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/aac/user_registry/user.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/aac/user_registry/user.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/appliance.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/appliance.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/application_logs.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/application_logs.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/activation.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/activation.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/admin.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/admin.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/admin_ssh_keys.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/admin_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/advanced_tuning_parameters.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/advanced_tuning_parameters.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/application_database_settings.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/application_database_settings.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/application_locale.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/application_locale.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/audit_configuration.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/audit_configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/available_updates.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/available_updates.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cli.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cli.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/config_database.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/config_database.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/configuration.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/log.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/log.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/node.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/node.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/property.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/property.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/runtime_database.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/runtime_database.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/signature.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/signature.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/cluster/trace.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/cluster/trace.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/date_time.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/date_time.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/dsc.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/dsc.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/extensions.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/extensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 def _get_config_data(extId, config_data):
     """
     Generate a JSON payload for activate/update
     """
     if config_data is None:
         return json.dumps({extId: extId})
     if isinstance(config_data, basestring):
-        return '{extId:}' + extId + ',' + config_data + '}'
+        return '{extId:' + extId + ',' + config_data + '}'
     config_data['extId'] = extId
     return json.dumps(config_data)
 
 def search(isamAppliance, extId, check_mode=False, force=False):
     """
     Search for the extension
     """
```

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/file_downloads.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/file_downloads.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/fips.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/fips.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/firmware.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/firmware.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/fixpack.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/fixpack.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/geolocation_db.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/geolocation_db.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/host/name.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/host/name.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/host/records.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/host/records.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/license.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/license.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/lmi.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/lmi.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/lmi_tracing.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/lmi_tracing.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authentication.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authentication.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authorization/config.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authorization/config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authorization/feature.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authorization/feature.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authorization/role.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authorization/role.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authorization/role_feature.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authorization/role_feature.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authorization/role_group.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authorization/role_group.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_authorization/role_user.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_authorization/role_user.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/management_ssl_certificate.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/management_ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/active_status.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/active_status.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/dns.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/dns.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/advanced_tuning/at_logging.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/advanced_tuning/at_logging.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/advanced_tuning/config.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/advanced_tuning/config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/attributes/advanced_tuning.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/attributes/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/attributes/log.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/attributes/log.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/config.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/error_page.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/error_page.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/ha.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/ha.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/services/advanced_tuning.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/services/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/services/config.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/services/config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/services/layer.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/services/layer.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/services/servers.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/services/servers.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/felb/ssl.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/felb/ssl.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/host_records.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/host_records.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/hostname.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/hostname.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/interfaces.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/interfaces.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/interfaces_ipv4.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/interfaces_ipv4.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/interfaces_ipv6.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/interfaces_ipv6.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/interfaces_vlan.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/interfaces_vlan.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/packet_trace.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/packet_trace.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/static_routes.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/static_routes.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/network/test_connection.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/network/test_connection.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/overview.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/overview.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/remote_syslog/forwarder.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/remote_syslog/forwarder.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/remote_syslog/forwarder_sources.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/remote_syslog/forwarder_sources.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/remote_syslog/instance_logs.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/remote_syslog/instance_logs.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/remote_syslog/instances.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/remote_syslog/instances.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/runtime/cluster.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/runtime/cluster.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/runtime/listening_interfaces.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/runtime/listening_interfaces.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/runtime/process.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/runtime/process.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/runtime/tuning_parameters.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/runtime/tuning_parameters.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/scheduled_security_updates.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/scheduled_security_updates.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/service_agreement.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/service_agreement.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/setup_complete.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/setup_complete.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/silent_config.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/silent_config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/snapshots.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/snapshots.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/snmp_monitoring.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/snmp_monitoring.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/ssl_certificates/certificate_databases.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/ssl_certificates/certificate_databases.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/ssl_certificates/certificate_requests.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/ssl_certificates/certificate_requests.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/ssl_certificates/personal_certificate.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/ssl_certificates/personal_certificate.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/ssl_certificates/replication.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/ssl_certificates/replication.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/ssl_certificates/signer_certificate.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/ssl_certificates/signer_certificate.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/support.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/support.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/sysaccount/groups.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/sysaccount/groups.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/sysaccount/ssh_keys.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/sysaccount/ssh_keys.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/sysaccount/users.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/sysaccount/users.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/system_alerts/alerts.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/system_alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/system_alerts/email.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/system_alerts/email.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/system_alerts/logdb.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/system_alerts/logdb.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/system_alerts/rsyslog.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/system_alerts/rsyslog.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/system_alerts/snmp.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/system_alerts/snmp.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/update_history.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/update_history.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/base/update_servers.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/base/update_servers.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/base/network/db_configuration/configuration.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/base/network/db_configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/publish.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/publish.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/docker/service_configuration/configuration.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/docker/service_configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/event_log.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/event_log.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/alias_service.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/alias_service.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/alias_service_settings.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/alias_service_settings.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/attribute_source.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/attribute_source.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/connector_instructions.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/connector_instructions.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/federations.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/federations.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/partner_templates.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/partner_templates.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/partners.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/partners.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/point_of_contact.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/point_of_contact.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/sts/module_chains.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/sts/module_chains.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/sts/modules.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/sts/modules.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/fed/sts/templates.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/fed/sts/templates.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/statistics.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/statistics.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/cors_policies.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/cors_policies.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/documentation_root.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/documentation_root.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/policies.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/policies.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/resources/instances.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/resources/instances.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/resources/resources.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/resources/resources.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/resources/servers.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/resources/servers.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/utilities/credential.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/utilities/credential.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/api_access_control/utilities/group.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/api_access_control/utilities/group.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/cleanup.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/cleanup.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/configuration/entry.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/configuration/entry.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/configuration/stanza.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/configuration/stanza.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/configuration/trace.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/configuration/trace.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/instance.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/instance.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/logs.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/logs.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/authorization_server/trace.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/authorization_server/trace.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/client_certificate_mapping.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/client_certificate_mapping.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/dsc.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/dsc.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/embedded_ldap/admin.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/embedded_ldap/admin.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/embedded_ldap/debug.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/embedded_ldap/debug.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/embedded_ldap/group.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/embedded_ldap/group.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/embedded_ldap/suffix.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/embedded_ldap/suffix.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/embedded_ldap/user.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/embedded_ldap/user.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/fsso.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/fsso.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/global_settings/redis_configuration/collections.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/global_settings/redis_configuration/collections.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/global_settings/redis_configuration/wrp.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/global_settings/redis_configuration/wrp.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/global_settings/waf.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/global_settings/waf.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/http_transformation.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/http_transformation.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/iag/export.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/iag/export.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/junction_mapping.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/junction_mapping.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths_property.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths_property.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/defaults.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/defaults.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/domains.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/domains.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/keyfiles.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/keyfiles.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/realms.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/realms.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/realms_property.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/realms_property.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/realms_subsection.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/realms_subsection.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/kerberos_configuration/test.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/kerberos_configuration/test.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/ltpa_key.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/ltpa_key.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/password_strength.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/password_strength.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/query_sitecontents.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/query_sitecontents.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/rate_limiting.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/aac_configuration.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/aac_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ibmsecurity.isam.web.reverse_proxy import junctions
 
 logger = logging.getLogger(__name__)
 requires_modules = ["wga"]
 requires_version = "9.0.6.0"
 
 
-def config(isamAppliance, instance_id, hostname='127.0.0.1', port=443, username='easuser', password='passw0rd',
+def config(isamAppliance, instance_id, hostname='127.0.0.1', port=443, username=None, password=None,
            junction="/mga", reuse_certs=False, reuse_acls=False, check_mode=False, force=False):
     """
     Authentication and Context based access configuration for a reverse proxy instance
 
     :param isamAppliance:
     :param instance_id:
     :param junction:
@@ -20,14 +20,21 @@
     :param password:
     :param reuse_certs:
     :param reuse_acls:
     :param check_mode:
     :param force:
     :return:
     """
+    if username is None:
+        logger.info("Required parameter username missing. Skipping config.")
+        return isamAppliance.create_return_object(warning=["Required parameter username missing. Skipping config."])
+
+    if password is None:
+        logger.info("Required parameter password missing. Skipping config.")
+        return isamAppliance.create_return_object(warning=["Required parameter password missing. Skipping config."])
     warnings = [
         "Idempotency logic will check for existence of {} junction. Use force=True to override.".format(junction)]
     if force is True or _check_config(isamAppliance, instance_id, junction) is False:
         json_data = {
             "junction": junction,
             "hostname": hostname,
             "port": port,
```

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/common_configurations.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/common_configurations.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/common_logs.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/common_logs.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/entry.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/configuration/entry.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/stanza.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/configuration/stanza.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/trace.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/configuration/trace.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/waf_config.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/configuration/waf_config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/federation_configuration.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/federation_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import ibmsecurity.isam.fed.federations
 
 logger = logging.getLogger(__name__)
 
 
-def config(isamAppliance, instance_id, federation_id=None, federation_name=None, hostname='127.0.0.1', port='443', username='easuser',
-           password='passw0rd', reuse_certs=False, reuse_acls=False, check_mode=False, force=False):
+def config(isamAppliance, instance_id, federation_id=None, federation_name=None, hostname='127.0.0.1', port='443', username=None,
+           password=None, reuse_certs=False, reuse_acls=False, check_mode=False, force=False):
     """
     Federation configuration for a reverse proxy instance
 
     :param isamAppliance:
     :param instance_id:
     :param federation_id:
     :param federation_name:
@@ -19,14 +19,21 @@
     :param password:
     :param reuse_certs:
     :param reuse_acls:
     :param check_mode:
     :param force:
     :return:
     """
+    if username is None:
+        logger.info("Required parameter username missing. Skipping config.")
+        return isamAppliance.create_return_object(warning=["Required parameter username missing. Skipping config."])
+
+    if password is None:
+        logger.info("Required parameter password missing. Skipping config.")
+        return isamAppliance.create_return_object(warning=["Required parameter password missing. Skipping config."])
 
     if federation_name is not None:
         ret_obj = ibmsecurity.isam.fed.federations.search(isamAppliance, name=federation_name, check_mode=check_mode,
                                                       force=force)
         federation_id = ret_obj['data']
 
         if federation_id == {}:
```

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/instance.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/instance.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/interfaces.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/interfaces.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/ivg_configuration.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/ivg_configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/junctions.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/junctions.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/junctions_config.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/junctions_config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/junctions_server.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/junctions_server.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/logs.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/logs.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/all.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/management_root/all.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/directory.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/management_root/directory.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/file.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/management_root/file.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/mmfa_configuration.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/mmfa_configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/oauth_configuration.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/oauth_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ibmsecurity.isam.web.reverse_proxy import junctions
 
 logger = logging.getLogger(__name__)
 requires_modules = ["wga"]
 requires_version = "9.0.4.0"
 
 
-def config(isamAppliance, instance_id, hostname='127.0.0.1', port=443, username='easuser', password='passw0rd',
+def config(isamAppliance, instance_id, hostname='127.0.0.1', port=443, username=None, password=None,
            junction="/mga", reuse_certs=False, reuse_acls=False, api=False, browser=False, auth_register=None, fapi_compliant=None,
            check_mode=False, force=False):
     """
     Oauth and Oidc configuration for a reverse proxy instance
 
     :param isamAppliance:
     :param instance_id:
@@ -26,14 +26,22 @@
     :param browser:
     :param auth_register:
     :param check_mode:
     :param force:
     :param fapi_compliant:
     :return:
     """
+    if username is None:
+        logger.info("Required parameter username missing. Skipping config.")
+        return isamAppliance.create_return_object(warning=["Required parameter username missing. Skipping config."])
+
+    if password is None:
+        logger.info("Required parameter password missing. Skipping config.")
+        return isamAppliance.create_return_object(warning=["Required parameter password missing. Skipping config."])
+
     warnings = [
         "Idempotency logic will check for existence of {} junction. Use force=True to override.".format(junction)]
     if force is True or _check_config(isamAppliance, instance_id, junction) is False:
         json_data = {
             "junction": junction,
             "hostname": hostname,
             "port": port,
```

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/statistics.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/statistics.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/trace.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/trace.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/reverse_proxy/transaction_logging.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/reverse_proxy/transaction_logging.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/rsa_securid_config.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/rsa_securid_config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/acl.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/acl.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/configuration/entry.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/configuration/entry.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/configuration/file.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/configuration/file.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/configuration/stanza.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/configuration/stanza.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/federated_directories/stanza.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/federated_directories/stanza.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,23 +60,21 @@
             json_data = {
                 'id': id,
                 'hostname': hostname,
                 'port': port,
                 'bind_dn': bind_dn,
                 'bind_pwd': bind_pwd,
                 'use_ssl': use_ssl,
-                'suffix': suffix
+                'suffix': suffix,
+                'client_cert_label': client_cert_label
             }
 
             if tools.version_compare(isamAppliance.facts["version"], "10.0.4") >= 0:
                 json_data['ignore_if_down'] = ignore_if_down
 
-            # Do not pass if there is no value - call fails otherwise
-            if client_cert_label is not None:
-                json_data['client_cert_label'] = client_cert_label
             return isamAppliance.invoke_post(
                 "Create a new federated directory",
                 "/isam/runtime_components/federated_directories/v1", json_data)
 
     return isamAppliance.create_return_object()
```

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/federated_directories/suffix.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/federated_directories/suffix.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/object.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/object.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/pdadmin.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/pdadmin.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/pop.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/pop.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/process.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/process.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/replication.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/replication.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/runtime/trace.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/runtime/trace.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/sso_keys.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/sso_keys.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/url_mapping.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/url_mapping.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isam/web/user_name_mapping.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isam/web/user_name_mapping.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/admin.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/admin.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/advanced_tuning_parameters.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/advanced_tuning_parameters.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/appliance.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/appliance.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/available_updates.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/available_updates.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/config.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/date_time.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/date_time.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/firmware.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/firmware.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/fixpack.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/fixpack.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/host_records.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/host_records.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/hostnames.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/hostnames.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/interfaces.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/interfaces.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/license.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/license.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/server.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/server.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/snapshots.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/snapshots.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/snmp_monitoring.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/snmp_monitoring.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/statistics.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/statistics.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/support.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/support.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/system_alerts/alerts.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/system_alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/system_alerts/rsyslog.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/system_alerts/rsyslog.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/system_alerts/snmp.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/system_alerts/snmp.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isds/update_servers.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isds/update_servers.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/admin.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/admin.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/advanced_tuning_parameters.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/advanced_tuning_parameters.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/appliance.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/appliance.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/available_updates.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/available_updates.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/certstore_personal.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/certstore_personal.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/certstore_signer.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/certstore_signer.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/cm/process.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/cm/process.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/date_time.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/date_time.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/firmware.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/firmware.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/fixpack.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/fixpack.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/host_records.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/host_records.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/hostnames.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/hostnames.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/certstore_personal.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/certstore_personal.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/certstore_signer.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/certstore_signer.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/db.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/db.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/external_library.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/external_library.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/guided_setup.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/guided_setup.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/jvm_property.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/jvm_property.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/keystore.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/keystore.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/ldap.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/ldap.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/mail.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/mail.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/nls.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/nls.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/openid.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/openid.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/process.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/process.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/property.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/property.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/property_file.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/property_file.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/im/workflowextension.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/im/workflowextension.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/interfaces.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/interfaces.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/lmi.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/lmi.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/lmi_auth.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/lmi_auth.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/management_authentication.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/management_authentication.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/management_ssl_certificate.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/management_ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/sdi/process.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/sdi/process.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/service_agreement.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/service_agreement.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/setup_complete.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/setup_complete.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/snapshots.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/snapshots.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/snmp_monitoring.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/snmp_monitoring.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/support.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/support.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/system_alerts/alerts.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/system_alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/system_alerts/rsyslog.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/system_alerts/rsyslog.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/isvg/system_alerts/snmp.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/isvg/system_alerts/snmp.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/user/applianceuser.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/user/applianceuser.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/user/isdsapplianceuser.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/user/isdsapplianceuser.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity/utilities/tools.py` & `ibmsecurity-2024.4.5.0/ibmsecurity/utilities/tools.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity.egg-info/PKG-INFO` & `ibmsecurity-2024.4.5.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmsecurity
-Version: 2024.2.26.0
+Version: 2024.4.5.0
 Summary: Idempotent functions for IBM Security Appliance REST APIs
 Home-page: 
 Author: IBM
 Author-email: IBM <secorch@wwpdl.vnet.ibm.com>
 Project-URL: Homepage, https://github.com/IBM-Security/ibmsecurity
 Project-URL: Bug Tracker, https://github.com/IBM-Security/ibmsecurity/issues
 Classifier: Programming Language :: Python :: 3
@@ -42,15 +42,99 @@
 The following Python Packages are optional:
 1. cryptography - to perform action on certificates (used for idempotency in management_ssl_certificate)
 2. python-dateutil - date utilities (used for idempotency in management_ssl_certificate)
 
 Appliances need to have an ip address defined for their LMI. This may mean that appliances have had their initial setup 
 done with license acceptance.
 
+## TLS verification enabled (v2024.4.5)
 
+These changes are backwards compatible. We default to not verifying but always display a notice:
+
+````markdown
+Certificate verification has been disabled. Python is NOT verifying the SSL 
+certificate of the host appliance and InsecureRequestWarning messages are 
+
+being suppressed for the following host:
+
+https://{0}:{1}
+
+To use certificate verification:
+
+1. When the certificate is trusted by your Python environment:
+   Instantiate all instances of ISAMAppliance with verify=True or set 
+   the environment variable IBMSECLIB_VERIFY_CONNECTION=True.
+2. When the certificate is not already trusted in your Python environment:
+   Instantiate all instances of ISAMAppliance with the verify parameter
+   set to the fully qualified path to a CA bundle.
+
+See the following URL for more details:
+https://requests.readthedocs.io/en/latest/user/advanced/#ssl-cert-verification
+````
+To remediate this cert validation warning, consider the instructions below:
+
+Correct usage:
+
+If you have the cert on disk somewhere,
+instantiate the ISAMAppliance with:
+
+    ISAMAppliance(…, verify=<path to cert>)
+
+You can retrieve this from appliance using a command like:
+
+    openssl s_client -connect ${HOSTNAME}:${PORT} </dev/null 2>/dev/null | openssl x509 -outform pem >  isamAppliance.pem
+
+If the cert is already trusted in your Python environment,
+instantiate the ISAMAppliance with:
+
+    ISAMAppliance(…, verify=True)
+
+or set the environment variable: `IBMSECLIB_VERIFY_CONNECTION=true`
+
+If you receive errors about the hostname not matching the certificate:
+
+This might look like:
+````
+<stack trace>
+
+…
+
+    raise CertificateError("hostname %r doesn't match %r" % (hostname, dnsnames[0]))
+
+urllib3.util.ssl_match_hostname.CertificateError: hostname '192.168.42.111' doesn't match 'appliance.ibm.com'
+
+````
+
+Ensure the hostname used when instantiating your ISAMAppliance matches the Subject Alternative Name of the cert.
+
+Check with: 
+
+    openssl x509 -in <cert-pem-file> -text
+
+Example:
+
+    $ openssl x509 -in /path/to/appliance.pem -text
+
+Certificate:
+
+    Data:
+        Version: 3 (0x2)
+        …
+            X509v3 Subject Alternative Name:
+                DNS:appliance.ibm.com
+…
+
+The following will generate errors:
+
+    ISAMAppliance(host=”192.168.42.111”, lmi_port=443, verify=/path/to/appliance.pem)
+
+as host does not match the Subject Alternative Name.
+Instead, use:
+
+    ISAMAppliance(host=”appliance.ibm.com”, lmi_port=443, verify=/path/to/appliance.pem)
 
 ## Versioning
 
 This package uses a date for versioning. For example: "2017.03.18.0"
 
 It is the date when the package is released with a sequence number at the end to handle when there are 
 multiple releases in one day (expected to be uncommon).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ibmsecurity-2024.2.26.0/ibmsecurity.egg-info/SOURCES.txt` & `ibmsecurity-2024.4.5.0/ibmsecurity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2024.2.26.0/pyproject.toml` & `ibmsecurity-2024.4.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ibmsecurity"
-version = "2024.2.26.0"
+version = "2024.4.5.0"
 authors = [
   { name="IBM", email="secorch@wwpdl.vnet.ibm.com" },
 ]
 description = "Idempotent functions for IBM Security Appliance REST APIs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ibmsecurity-2024.2.26.0/setup.py` & `ibmsecurity-2024.4.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'ibmsecurity',
     packages = find_packages(),
     # Date of release used for version - please be sure to use YYYY.MM.DD.seq#, MM and DD should be two digits e.g. 2017.02.05.0
     # seq# will be zero unless there are multiple release on a given day - then increment by one for additional release for that date
-    version = '2024.2.26.0',
+    version = '2024.4.5.0',
     description = 'Idempotent functions for IBM Security Appliance REST APIs',
     author='IBM',
     author_email='secorch@wwpdl.vnet.ibm.com',
     url='',
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
```

