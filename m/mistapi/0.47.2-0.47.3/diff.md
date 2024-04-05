# Comparing `tmp/mistapi-0.47.2.tar.gz` & `tmp/mistapi-0.47.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistapi-0.47.2.tar", last modified: Wed Feb  7 18:20:46 2024, max compression
+gzip compressed data, was "mistapi-0.47.3.tar", last modified: Fri Apr  5 16:02:18 2024, max compression
```

## Comparing `mistapi-0.47.2.tar` & `mistapi-0.47.3.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.582663 mistapi-0.47.2/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.47.2/LICENSE
--rw-r--r--   0 tmunzer    (502) staff       (20)    11443 2024-02-07 18:20:46.582431 mistapi-0.47.2/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)    10541 2023-10-05 14:00:29.000000 mistapi-0.47.2/README.md
--rw-r--r--   0 tmunzer    (502) staff       (20)      976 2024-02-07 18:20:34.000000 mistapi-0.47.2/pyproject.toml
--rw-r--r--   0 tmunzer    (502) staff       (20)      125 2024-02-07 18:20:46.582991 mistapi-0.47.2/setup.cfg
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.503741 mistapi-0.47.2/src/
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.511111 mistapi-0.47.2/src/mistapi/
--rw-r--r--   0 tmunzer    (502) staff       (20)    15410 2023-10-10 06:25:01.000000 mistapi-0.47.2/src/mistapi/__api_request.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3275 2023-10-10 08:14:00.000000 mistapi-0.47.2/src/mistapi/__api_response.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    34150 2024-02-07 18:20:10.000000 mistapi-0.47.2/src/mistapi/__api_session.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      615 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2297 2023-10-19 16:39:16.000000 mistapi-0.47.2/src/mistapi/__logger.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.513178 mistapi-0.47.2/src/mistapi/__models/
--rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.47.2/src/mistapi/__models/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.47.2/src/mistapi/__models/privilege.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2079 2023-10-10 06:34:01.000000 mistapi-0.47.2/src/mistapi/__pagination.py
--rw-r--r--   0 tmunzer    (502) staff       (20)       74 2023-10-10 14:55:37.000000 mistapi-0.47.2/src/mistapi/__version.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.513557 mistapi-0.47.2/src/mistapi/api/
--rw-r--r--   0 tmunzer    (502) staff       (20)      446 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.513845 mistapi-0.47.2/src/mistapi/api/v1/
--rw-r--r--   0 tmunzer    (502) staff       (20)      869 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.520311 mistapi-0.47.2/src/mistapi/api/v1/const/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1341 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/alarm_defs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2047 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/ap_channels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1760 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/ap_led_status.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/applications.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/client_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1737 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/countries.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1412 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/default_gateway_config.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/device_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/device_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1794 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/gateway_applications.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/insight_metrics.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1742 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/languages.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/license_types.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/mxedge_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/mxedge_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1779 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/nac_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1835 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/otherdevice_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1825 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/otherdevice_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/const/traffic_types.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.520602 mistapi-0.47.2/src/mistapi/api/v1/installer/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/installer/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.523441 mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)      798 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7099 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1992 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1967 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1960 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8000 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/sites.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.524367 mistapi-0.47.2/src/mistapi/api/v1/installer/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)      471 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/installer/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1178 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/installer/sites/optimize.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.524989 mistapi-0.47.2/src/mistapi/api/v1/invite/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/invite/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1109 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/invite/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.526263 mistapi-0.47.2/src/mistapi/api/v1/login/
--rw-r--r--   0 tmunzer    (502) staff       (20)      584 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/login/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1154 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/login/login.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1163 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/login/lookup.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2656 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/login/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1173 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/login/two_factor.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.526731 mistapi-0.47.2/src/mistapi/api/v1/logout/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/logout/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      999 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/logout/logout.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.527244 mistapi-0.47.2/src/mistapi/api/v1/mobile/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/mobile/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1270 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/mobile/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.532889 mistapi-0.47.2/src/mistapi/api/v1/msps/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3925 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1683 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1210 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2653 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1851 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/logo.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4542 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3032 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/msps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/orggroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6691 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1674 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/search.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4048 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7398 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3709 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1518 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/suggestion.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3269 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/msps/tickets.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.555825 mistapi-0.47.2/src/mistapi/api/v1/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)     3378 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3288 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6526 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8412 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5213 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/aptemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5245 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6580 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2337 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/cert.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    12343 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1249 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/clone.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1869 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/crl.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7161 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    19522 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5295 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5353 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/gatewaytemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6601 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5213 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/idpprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2959 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6616 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7004 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/jsi.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2536 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5309 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1931 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1293 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/mist_nac.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5237 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/mxclusters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    24910 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5157 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    12704 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/nac_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/nacrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5101 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/nactags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5355 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/networktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1417 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/ocdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3018 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9689 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2365 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/pma.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    10543 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/pskportals.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8448 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5213 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1324 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/sdkclients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6964 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/sdkinvites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4770 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/sdktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5204 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5308 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    19166 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5185 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9353 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5271 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/sitetemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8754 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5758 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    32781 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1767 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5940 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/templates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7361 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/tickets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1764 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/troubleshoot.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1611 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/vars.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5024 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1374 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/wan_client.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4985 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/wan_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7229 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3722 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7464 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5729 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6385 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5157 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/orgs/wxtunnels.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.556637 mistapi-0.47.2/src/mistapi/api/v1/recover/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/recover/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1176 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/recover/recover.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1120 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/recover/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.557954 mistapi-0.47.2/src/mistapi/api/v1/register/
--rw-r--r--   0 tmunzer    (502) staff       (20)      555 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/register/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1308 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/register/recaptcha.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1179 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/register/register.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1113 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/register/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.560258 mistapi-0.47.2/src/mistapi/api/v1/self/
--rw-r--r--   0 tmunzer    (502) staff       (20)      707 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/self/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4317 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/self/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2654 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/self/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2033 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/self/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2157 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/self/self.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1773 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/self/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1953 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/self/two_factor.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1784 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/self/update.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.580415 mistapi-0.47.2/src/mistapi/api/v1/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)     2876 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8779 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2660 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/anomaly.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1881 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/apps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1358 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/aptemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5280 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6629 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5142 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/beacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2349 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    18402 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2418 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/count.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2356 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    65592 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4040 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4114 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1373 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/gatewaytemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7121 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9228 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1167 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7146 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/location.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    16638 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9250 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1189 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    12392 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/nac_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2314 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1373 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/networktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5875 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5899 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/pcaps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7696 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5817 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/rfdiags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1358 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5809 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/rogues.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3862 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/rrm.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5194 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/rssizones.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2363 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6185 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6746 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2437 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1364 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/sitetemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3886 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/skyatp.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    20772 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/sle.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1983 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    66094 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1751 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1928 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/synthetic_test.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5425 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/uisettings.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5166 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/vbeacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2308 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/visits.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2286 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1380 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/wan_client.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5003 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/wan_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7212 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3986 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8790 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5772 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6434 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5194 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/wxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5082 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/sites/zones.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.581385 mistapi-0.47.2/src/mistapi/api/v1/utils/
--rw-r--r--   0 tmunzer    (502) staff       (20)      511 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/utils/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1205 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/utils/test_telstra.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1202 2024-02-07 18:20:34.000000 mistapi-0.47.2/src/mistapi/api/v1/utils/test_twilio.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    13223 2023-10-11 11:11:09.000000 mistapi-0.47.2/src/mistapi/cli.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-02-07 18:20:46.581877 mistapi-0.47.2/src/mistapi.egg-info/
--rw-r--r--   0 tmunzer    (502) staff       (20)    11443 2024-02-07 18:20:46.000000 mistapi-0.47.2/src/mistapi.egg-info/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)     8339 2024-02-07 18:20:46.000000 mistapi-0.47.2/src/mistapi.egg-info/SOURCES.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        1 2024-02-07 18:20:46.000000 mistapi-0.47.2/src/mistapi.egg-info/dependency_links.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)       66 2024-02-07 18:20:46.000000 mistapi-0.47.2/src/mistapi.egg-info/requires.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        8 2024-02-07 18:20:46.000000 mistapi-0.47.2/src/mistapi.egg-info/top_level.txt
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.898271 mistapi-0.47.3/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.47.3/LICENSE
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11443 2024-04-05 16:02:18.898044 mistapi-0.47.3/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10541 2023-10-05 14:00:29.000000 mistapi-0.47.3/README.md
+-rw-r--r--   0 tmunzer    (502) staff       (20)      976 2024-04-05 15:59:10.000000 mistapi-0.47.3/pyproject.toml
+-rw-r--r--   0 tmunzer    (502) staff       (20)      125 2024-04-05 16:02:18.898506 mistapi-0.47.3/setup.cfg
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.847443 mistapi-0.47.3/src/
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.852853 mistapi-0.47.3/src/mistapi/
+-rw-r--r--   0 tmunzer    (502) staff       (20)    15410 2023-10-10 06:25:01.000000 mistapi-0.47.3/src/mistapi/__api_request.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3275 2023-10-10 08:14:00.000000 mistapi-0.47.3/src/mistapi/__api_response.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    34224 2024-03-28 19:12:14.000000 mistapi-0.47.3/src/mistapi/__api_session.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      615 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2297 2023-10-19 16:39:16.000000 mistapi-0.47.3/src/mistapi/__logger.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.854732 mistapi-0.47.3/src/mistapi/__models/
+-rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.47.3/src/mistapi/__models/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.47.3/src/mistapi/__models/privilege.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2079 2023-10-10 06:34:01.000000 mistapi-0.47.3/src/mistapi/__pagination.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)       74 2023-10-10 14:55:37.000000 mistapi-0.47.3/src/mistapi/__version.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.854984 mistapi-0.47.3/src/mistapi/api/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      446 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.855117 mistapi-0.47.3/src/mistapi/api/v1/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      869 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.858090 mistapi-0.47.3/src/mistapi/api/v1/const/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1341 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/alarm_defs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2047 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/ap_channels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1760 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/ap_led_status.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/applications.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/client_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1737 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/countries.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1412 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/default_gateway_config.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/device_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/device_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1794 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/gateway_applications.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/insight_metrics.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1742 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/languages.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/license_types.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/mxedge_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/mxedge_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1779 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/nac_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1835 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/otherdevice_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1825 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/otherdevice_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/const/traffic_types.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.858218 mistapi-0.47.3/src/mistapi/api/v1/installer/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/installer/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.859810 mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      798 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7099 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1992 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1967 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1960 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8000 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/sites.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.860307 mistapi-0.47.3/src/mistapi/api/v1/installer/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      471 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/installer/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1178 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/installer/sites/optimize.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.860591 mistapi-0.47.3/src/mistapi/api/v1/invite/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/invite/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1109 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/invite/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.861395 mistapi-0.47.3/src/mistapi/api/v1/login/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      584 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/login/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1154 2024-04-05 15:59:10.000000 mistapi-0.47.3/src/mistapi/api/v1/login/login.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1163 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/login/lookup.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2656 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/login/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1173 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/login/two_factor.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.861939 mistapi-0.47.3/src/mistapi/api/v1/logout/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/logout/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      999 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/logout/logout.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.862349 mistapi-0.47.3/src/mistapi/api/v1/mobile/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/mobile/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1270 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/mobile/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.866511 mistapi-0.47.3/src/mistapi/api/v1/msps/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3925 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1683 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1210 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2653 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1851 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/logo.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4542 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3032 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/msps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/orggroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6691 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1674 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/search.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4048 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7398 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3709 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1518 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/suggestion.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3269 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/msps/tickets.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.882240 mistapi-0.47.3/src/mistapi/api/v1/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3378 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3288 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6526 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8412 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5213 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/aptemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5245 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6580 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2337 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/cert.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    12343 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1249 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/clone.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1869 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/crl.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7161 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    19522 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5295 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5353 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/gatewaytemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6601 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5213 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/idpprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2959 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6616 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7004 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/jsi.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2536 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5309 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1931 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1293 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/mist_nac.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5237 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/mxclusters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    24910 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5157 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    12704 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/nac_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/nacrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5101 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/nactags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5355 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/networktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1417 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/ocdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3018 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9689 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2365 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/pma.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10543 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/pskportals.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8448 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5213 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1324 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/sdkclients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6964 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/sdkinvites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4770 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/sdktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5204 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5308 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    19166 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5185 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9353 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5271 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/sitetemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8754 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5758 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    32781 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1767 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5940 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/templates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7361 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/tickets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1764 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/troubleshoot.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1611 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/vars.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5024 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1374 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/wan_client.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4985 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/wan_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7229 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3722 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7464 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5729 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6385 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5157 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/orgs/wxtunnels.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.882639 mistapi-0.47.3/src/mistapi/api/v1/recover/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/recover/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1176 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/recover/recover.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1120 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/recover/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.883152 mistapi-0.47.3/src/mistapi/api/v1/register/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      555 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/register/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1308 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/register/recaptcha.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1179 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/register/register.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1113 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/register/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.884374 mistapi-0.47.3/src/mistapi/api/v1/self/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      707 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/self/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4317 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/self/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2654 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/self/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2033 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/self/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2157 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/self/self.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1773 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/self/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1953 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/self/two_factor.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1784 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/self/update.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.896736 mistapi-0.47.3/src/mistapi/api/v1/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2876 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8779 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2660 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/anomaly.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1881 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/apps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1358 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/aptemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5280 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6629 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5142 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/beacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2349 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    18402 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2418 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/count.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2356 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    65592 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4040 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4114 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1373 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/gatewaytemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7121 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9228 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1167 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7146 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/location.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    16638 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9250 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1189 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    12392 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/nac_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2314 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1373 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/networktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5875 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5899 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/pcaps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7696 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5817 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/rfdiags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1358 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5809 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/rogues.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3862 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/rrm.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5194 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/rssizones.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2363 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6185 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6746 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2437 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1364 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/sitetemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3886 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/skyatp.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    20772 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/sle.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1983 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    66094 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1751 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1928 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/synthetic_test.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5425 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/uisettings.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5166 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/vbeacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2308 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/visits.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2286 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1380 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/wan_client.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5003 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/wan_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7212 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3986 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8790 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5772 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6434 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5194 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/wxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5082 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/sites/zones.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.897279 mistapi-0.47.3/src/mistapi/api/v1/utils/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      511 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/utils/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1205 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/utils/test_telstra.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1202 2024-04-05 15:59:11.000000 mistapi-0.47.3/src/mistapi/api/v1/utils/test_twilio.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    13223 2023-10-11 11:11:09.000000 mistapi-0.47.3/src/mistapi/cli.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-04-05 16:02:18.897475 mistapi-0.47.3/src/mistapi.egg-info/
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11443 2024-04-05 16:02:18.000000 mistapi-0.47.3/src/mistapi.egg-info/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8339 2024-04-05 16:02:18.000000 mistapi-0.47.3/src/mistapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        1 2024-04-05 16:02:18.000000 mistapi-0.47.3/src/mistapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)       66 2024-04-05 16:02:18.000000 mistapi-0.47.3/src/mistapi.egg-info/requires.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        8 2024-04-05 16:02:18.000000 mistapi-0.47.3/src/mistapi.egg-info/top_level.txt
```

### Comparing `mistapi-0.47.2/LICENSE` & `mistapi-0.47.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/PKG-INFO` & `mistapi-0.47.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.47.2
+Version: 0.47.3
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.47.2/README.md` & `mistapi-0.47.3/README.md`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/pyproject.toml` & `mistapi-0.47.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mistapi"
-version = "0.47.2"
+version = "0.47.3"
 authors = [{name="Thomas Munzer", email="tmunzer@juniper.net"}]
 description = "Python package to simplify the Mist System APIs usage"
 keywords = ["Mist", "Juniper", "API"]
 license = {text =  "MIT"}
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mistapi-0.47.2/src/mistapi/__api_request.py` & `mistapi-0.47.3/src/mistapi/__api_request.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/__api_response.py` & `mistapi-0.47.3/src/mistapi/__api_response.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/__api_session.py` & `mistapi-0.47.3/src/mistapi/__api_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 from mistapi.__api_request import APIRequest
 from mistapi.__api_response import APIResponse
 from mistapi.__models.privilege import Privileges
 from mistapi.__version import __version__
 ###### GLOBALS ######
 CLOUDS = [
     {"short": "APAC 01", "host": "api.ac5.mist.com", "cookies_ext": ".ac5"},
-    {"short": "Europe 01", "host": "api.eu.mist.com", "cookies_ext": ".eu"},
+    {"short": "EMEA 01", "host": "api.eu.mist.com", "cookies_ext": ".eu"},
+    {"short": "EMEA 02", "host": "api.gc3.mist.com", "cookies_ext": ".gc3"},
     {"short": "Global 01", "host": "api.mist.com", "cookies_ext": ""},
     {"short": "Global 02", "host": "api.gc1.mist.com", "cookies_ext": ".gc1"},
     {"short": "Global 03", "host": "api.ac2.mist.com", "cookies_ext": ".ac2"},
     {"short": "Global 04", "host": "api.gc2.mist.com", "cookies_ext": ".gc2"},
 ]
 
-
 #### PARAMETERS #####
 
 
 class APISession(APIRequest):
     """Class managing REST API Session"""
 
     def __init__(
```

### Comparing `mistapi-0.47.2/src/mistapi/__init__.py` & `mistapi-0.47.3/src/mistapi/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/__logger.py` & `mistapi-0.47.3/src/mistapi/__logger.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/__models/privilege.py` & `mistapi-0.47.3/src/mistapi/__models/privilege.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/__pagination.py` & `mistapi-0.47.3/src/mistapi/__pagination.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/__init__.py` & `mistapi-0.47.3/src/mistapi/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/__init__.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/alarm_defs.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/alarm_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listAlarmDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listAlarmDefinitions")  
 def getAlarmDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAlarmDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/ap_channels.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/ap_channels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listApChannels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listApChannels")  
 def getApChannels(mist_session:_APISession, country_code:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApChannels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/ap_led_status.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/ap_led_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listApLedDefinition")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listApLedDefinition")  
 def getApLedDefinition(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApLedDefinition
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/applications.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/applications.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listApplications")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listApplications")  
 def getApplications(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApplications
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/client_events.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/client_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listClientEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listClientEventsDefinitions")  
 def getClientEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listClientEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/countries.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/countries.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listCountryCodes")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listCountryCodes")  
 def getCountryCodes(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listCountryCodes
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/default_gateway_config.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/default_gateway_config.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/device_events.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/device_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listDeviceEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listDeviceEventsDefinitions")  
 def getDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listDeviceEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/device_models.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/device_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listDeviceModels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listDeviceModels")  
 def getDeviceModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listDeviceModels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/gateway_applications.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/gateway_applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listGatewayApplications")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listGatewayApplications")  
 def getGatewayApplications(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listGatewayApplications
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/insight_metrics.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/insight_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listInsightMetrics")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listInsightMetrics")  
 def getInsightMetrics(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInsightMetrics
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/languages.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/languages.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteLanguages")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteLanguages")  
 def getSiteLanguages(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteLanguages
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/license_types.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/license_types.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/mxedge_events.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/mxedge_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listMxEdgeEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listMxEdgeEventsDefinitions")  
 def getMxEdgeEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/mxedge_models.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/mxedge_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listMxEdgeModels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listMxEdgeModels")  
 def getMxEdgeModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeModels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/nac_events.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/nac_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listNacEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listNacEventsDefinitions")  
 def getNacEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listNacEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/otherdevice_events.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/otherdevice_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOtherDeviceEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOtherDeviceEventsDefinitions")  
 def getOtherDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOtherDeviceEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/otherdevice_models.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/otherdevice_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSupportedOtherDeviceModels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSupportedOtherDeviceModels")  
 def getSupportedOtherDeviceModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSupportedOtherDeviceModels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/const/traffic_types.py` & `mistapi-0.47.3/src/mistapi/api/v1/const/traffic_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listTrafficTypes")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listTrafficTypes")  
 def getTrafficTypes(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/__init__.py` & `mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/alarmtemplates.py` & `mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/alarmtemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listInstallerAlarmTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listInstallerAlarmTemplates")  
 def getInstallerAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerAlarmTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/deviceprofiles.py` & `mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/deviceprofiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listInstallerDeviceProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listInstallerDeviceProfiles")  
 def getInstallerDeviceProfiles(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerDeviceProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/devices.py` & `mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listInstallerListOfRenctlyClaimedDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listInstallerListOfRenctlyClaimedDevices")  
 def getInstallerListOfRenctlyClaimedDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerListOfRenctlyClaimedDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/rftemplates.py` & `mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/rftemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listInstallerRfTemplatesNames")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listInstallerRfTemplatesNames")  
 def getInstallerRfTemplatesNames(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerRfTemplatesNames
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/secpolicies.py` & `mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/secpolicies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listInstallerSecPolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listInstallerSecPolicies")  
 def getInstallerSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSecPolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/sitegroups.py` & `mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/sitegroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listInstallerSiteGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listInstallerSiteGroups")  
 def getInstallerSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSiteGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/installer/orgs/sites.py` & `mistapi-0.47.3/src/mistapi/api/v1/installer/orgs/sites.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listInstallerSites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listInstallerSites")  
 def getInstallerSites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -85,15 +85,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listInstallerMaps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listInstallerMaps")  
 def getInstallerMaps(mist_session:_APISession, org_id:str, site_name:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerMaps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/installer/sites/optimize.py` & `mistapi-0.47.3/src/mistapi/api/v1/installer/sites/optimize.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/invite/verify.py` & `mistapi-0.47.3/src/mistapi/api/v1/invite/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/login/__init__.py` & `mistapi-0.47.3/src/mistapi/api/v1/login/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/login/login.py` & `mistapi-0.47.3/src/mistapi/api/v1/login/login.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/login/lookup.py` & `mistapi-0.47.3/src/mistapi/api/v1/login/lookup.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/login/oauth.py` & `mistapi-0.47.3/src/mistapi/api/v1/login/oauth.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/login/two_factor.py` & `mistapi-0.47.3/src/mistapi/api/v1/login/two_factor.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/logout/logout.py` & `mistapi-0.47.3/src/mistapi/api/v1/logout/logout.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/mobile/verify.py` & `mistapi-0.47.3/src/mistapi/api/v1/mobile/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/__init__.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/admins.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/admins.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listMspAdmins")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listMspAdmins")  
 def getMspAdmins(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspAdmins
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/claim.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/insights.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/inventory.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/invites.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/licenses.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/licenses.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listMspLicenses")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listMspLicenses")  
 def getMspLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLicenses
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/logo.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/logo.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/logs.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listMspLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listMspLogs")  
 def getMspLogs(mist_session:_APISession, msp_id:str, site_id:str=None, admin_name:str=None, message:str=None, sort:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/msps.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/msps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/orggroups.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/orggroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listMspOrgGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listMspOrgGroups")  
 def getMspOrgGroups(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/orgs.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/orgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listMspOrgs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listMspOrgs")  
 def getMspOrgs(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/search.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/search.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/ssoroles.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/ssoroles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listMspSsoRoles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listMspSsoRoles")  
 def getMspSsoRoles(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoRoles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/ssos.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/ssos.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listMspSsos")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listMspSsos")  
 def getMspSsos(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsos
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -160,15 +160,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listMspSsoLatestFailures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listMspSsoLatestFailures")  
 def getMspSsoLatestFailures(mist_session:_APISession, msp_id:str, sso_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoLatestFailures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/stats.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listMspOrgLicenses")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listMspOrgLicenses")  
 def getMspOrgLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgLicenses
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -57,15 +57,15 @@
         response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/stats/licenses"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listMspOrgStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listMspOrgStats")  
 def getMspOrgStats(mist_session:_APISession, msp_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/suggestion.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/suggestion.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/msps/tickets.py` & `mistapi-0.47.3/src/mistapi/api/v1/msps/tickets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listMspTickets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listMspTickets")  
 def getMspTickets(mist_session:_APISession, msp_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspTickets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/__init__.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/admins.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/admins.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgAdmins")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgAdmins")  
 def getOrgAdmins(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAdmins
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/alarms.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/alarmtemplates.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/alarmtemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgAlarmTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgAlarmTemplates")  
 def getOrgAlarmTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAlarmTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -98,15 +98,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/alarmtemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgSuppressedAlarms")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgSuppressedAlarms")  
 def getOrgSuppressedAlarms(mist_session:_APISession, org_id:str, scope:str="site") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSuppressedAlarms
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/apitokens.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/apitokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgApiTokens")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgApiTokens")  
 def getOrgApiTokens(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApiTokens
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/aptemplates.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/aptemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgAptemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgAptemplates")  
 def getOrgAptemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAptemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/assetfilters.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/assetfilters.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgAssetFilters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgAssetFilters")  
 def getOrgAssetFilters(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetFilters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/assets.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgAssets")  
 def getOrgAssets(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/call.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/cert.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/cert.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/claim.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/clients.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/clone.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/clone.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/crl.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/crl.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/deviceprofiles.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/deviceprofiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgDeviceProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgDeviceProfiles")  
 def getOrgDeviceProfiles(mist_session:_APISession, org_id:str, type:str="ap", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDeviceProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/devices.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgDevices")  
 def getOrgDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -322,15 +322,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if limit: query_params["limit"]=limit
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgApsMacs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgApsMacs")  
 def getOrgApsMacs(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApsMacs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -476,15 +476,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgMultiSitesDevicesUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgMultiSitesDevicesUpgrades")  
 def getOrgMultiSitesDevicesUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMultiSitesDevicesUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/evpn_topologies.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/evpn_topologies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgEvpnTopologies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgEvpnTopologies")  
 def getOrgEvpnTopologies(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgEvpnTopologies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/gatewaytemplates.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/gatewaytemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgGatewayTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgGatewayTemplates")  
 def getOrgGatewayTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGatewayTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/guests.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/guests.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgGuestAuthorizations")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgGuestAuthorizations")  
 def getOrgGuestAuthorizations(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGuestAuthorizations
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/idpprofiles.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/idpprofiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgIdpProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgIdpProfiles")  
 def getOrgIdpProfiles(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgIdpProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/insights.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/inventory.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/invites.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/jsi.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/jsi.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgJsiDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgJsiDevices")  
 def getOrgJsiDevices(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None, mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -157,15 +157,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/jsi/devices/{device_mac}/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgJsiPastPurchases")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgJsiPastPurchases")  
 def getOrgJsiPastPurchases(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiPastPurchases
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/licenses.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/logs.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgLogs")  
 def getOrgLogs(mist_session:_APISession, org_id:str, site_id:str=None, admin_name:str=None, message:str=None, sort:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/maps.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/maps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/mist_nac.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/mist_nac.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/mxclusters.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/mxclusters.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgMxEdgeClusters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgMxEdgeClusters")  
 def getOrgMxEdgeClusters(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeClusters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/mxedges.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/mxedges.py`

 * *Files identical despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgMxEdges")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgMxEdges")  
 def getOrgMxEdges(mist_session:_APISession, org_id:str, for_sites:str="any", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdges
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -405,15 +405,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/unassign"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgMxEdgeUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgMxEdgeUpgrades")  
 def getOrgMxEdgeUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/mxtunnels.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/mxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgMxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgMxTunnels")  
 def getOrgMxTunnels(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/nac_clients.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/nac_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/nacrules.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/nacrules.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgNacRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgNacRules")  
 def getOrgNacRules(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/nactags.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/nactags.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgNacTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgNacTags")  
 def getOrgNacTags(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/networks.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgNetworks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgNetworks")  
 def getOrgNetworks(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/networktemplates.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/networktemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgNetworkTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgNetworkTemplates")  
 def getOrgNetworkTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworkTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/ocdevices.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/ocdevices.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/orgs.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/orgs.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/otherdevices.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/otherdevices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgOtherDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgOtherDevices")  
 def getOrgOtherDevices(mist_session:_APISession, org_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgOtherDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/pma.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/pma.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgPmaDashboards")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgPmaDashboards")  
 def getOrgPmaDashboards(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPmaDashboards
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/pskportals.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/pskportals.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgPskPortals")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgPskPortals")  
 def getOrgPskPortals(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPskPortals
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -98,15 +98,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/pskportals"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgPskPortalLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgPskPortalLogs")  
 def getOrgPskPortalLogs(mist_session:_APISession, org_id:str, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPskPortalLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/psks.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/psks.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgPsks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgPsks")  
 def getOrgPsks(mist_session:_APISession, org_id:str, name:str=None, ssid:str=None, role:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPsks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/rftemplates.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/rftemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgRfTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgRfTemplates")  
 def getOrgRfTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgRfTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/sdkclients.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/sdkclients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/sdkinvites.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/sdkinvites.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSdkInvites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSdkInvites")  
 def getSdkInvites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkInvites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/sdktemplates.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/sdktemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSdkTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSdkTemplates")  
 def getSdkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/secpolicies.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/secpolicies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgSecPolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgSecPolicies")  
 def getOrgSecPolicies(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSecPolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/servicepolicies.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/servicepolicies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgServicePolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgServicePolicies")  
 def getOrgServicePolicies(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServicePolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/services.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgServices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgServices")  
 def getOrgServices(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/setting.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/setting.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/sitegroups.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/sitegroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgSiteGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgSiteGroups")  
 def getOrgSiteGroups(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/sites.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/sites.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgSites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgSites")  
 def getOrgSites(mist_session:_APISession, org_id:str, limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/sitetemplates.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/sitetemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgSiteTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgSiteTemplates")  
 def getOrgSiteTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/ssoroles.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/ssoroles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgSsoRoles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgSsoRoles")  
 def getOrgSsoRoles(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoRoles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/ssos.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/ssos.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgSsos")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgSsos")  
 def getOrgSsos(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsos
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -174,15 +174,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgSsoLatestFailures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgSsoLatestFailures")  
 def getOrgSsoLatestFailures(mist_session:_APISession, org_id:str, sso_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoLatestFailures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/ssr.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/ssr.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/128routers/register_cmd"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgSsrUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgSsrUpgrades")  
 def getOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -135,15 +135,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssr/upgrade/{upgrade_id}/cancel"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgAvailableSsrVersions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgAvailableSsrVersions")  
 def getOrgAvailableSsrVersions(mist_session:_APISession, org_id:str, channel:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAvailableSsrVersions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/stats.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgAssetsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgAssetsStats")  
 def getOrgAssetsStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -255,15 +255,15 @@
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/stats/bgp_peers/search"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgDevicesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgDevicesStats")  
 def getOrgDevicesStats(mist_session:_APISession, org_id:str, type:str="ap", status:str="all", site_id:str=None, mac:str=None, evpntopo_id:str=None, evpn_unused:str=None, fields:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevicesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -360,15 +360,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgMxEdgesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgMxEdgesStats")  
 def getOrgMxEdgesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", for_site:str="false") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/subscriptions.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/templates.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgTemplates")  
 def getOrgTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/tickets.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/tickets.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgTickets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgTickets")  
 def getOrgTickets(mist_session:_APISession, org_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTickets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/troubleshoot.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/troubleshoot.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/vars.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/vars.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/vpns.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/vpns.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgsVpns")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgsVpns")  
 def getOrgsVpns(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/wan_client.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/wan_client.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/wan_clients.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/wan_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/webhooks.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/webhooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgWebhooks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgWebhooks")  
 def getOrgWebhooks(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWebhooks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/wired_clients.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/wlans.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/wlans.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgWlans")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgWlans")  
 def getOrgWlans(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWlans
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/wxrules.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/wxrules.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgWxRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgWxRules")  
 def getOrgWxRules(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/wxtags.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/wxtags.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgWxTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgWxTags")  
 def getOrgWxTags(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/orgs/wxtunnels.py` & `mistapi-0.47.3/src/mistapi/api/v1/orgs/wxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listOrgWxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listOrgWxTunnels")  
 def getOrgWxTunnels(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/recover/recover.py` & `mistapi-0.47.3/src/mistapi/api/v1/recover/recover.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/recover/verify.py` & `mistapi-0.47.3/src/mistapi/api/v1/recover/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/register/__init__.py` & `mistapi-0.47.3/src/mistapi/api/v1/register/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/register/recaptcha.py` & `mistapi-0.47.3/src/mistapi/api/v1/register/recaptcha.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/register/register.py` & `mistapi-0.47.3/src/mistapi/api/v1/register/register.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/register/verify.py` & `mistapi-0.47.3/src/mistapi/api/v1/register/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/self/__init__.py` & `mistapi-0.47.3/src/mistapi/api/v1/self/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/self/apitokens.py` & `mistapi-0.47.3/src/mistapi/api/v1/self/apitokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listApiTokens")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listApiTokens")  
 def getApiTokens(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApiTokens
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/self/logs.py` & `mistapi-0.47.3/src/mistapi/api/v1/self/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSelfAuditLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSelfAuditLogs")  
 def getSelfAuditLogs(mist_session:_APISession, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSelfAuditLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/self/oauth.py` & `mistapi-0.47.3/src/mistapi/api/v1/self/oauth.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/self/self.py` & `mistapi-0.47.3/src/mistapi/api/v1/self/self.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/self/subscriptions.py` & `mistapi-0.47.3/src/mistapi/api/v1/self/subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listAlarmSubscriptions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listAlarmSubscriptions")  
 def getAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAlarmSubscriptions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/self/two_factor.py` & `mistapi-0.47.3/src/mistapi/api/v1/self/two_factor.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/self/update.py` & `mistapi-0.47.3/src/mistapi/api/v1/self/update.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/__init__.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/alarms.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/anomaly.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/anomaly.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/apps.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/apps.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteApps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteApps")  
 def getSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteApps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/aptemplates.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/aptemplates.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/assetfilters.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/assetfilters.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteAssetFilters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteAssetFilters")  
 def getSiteAssetFilters(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetFilters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/assets.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteAssets")  
 def getSiteAssets(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/beacons.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/beacons.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteBeacons")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteBeacons")  
 def getSiteBeacons(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeacons
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/call.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/clients.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/count.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/count.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/deviceprofiles.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/deviceprofiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteDeviceProfilesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteDeviceProfilesDerived")  
 def getSiteDeviceProfilesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDeviceProfilesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/devices.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteDevices")  
 def getSiteDevices(mist_session:_APISession, site_id:str, type:str="ap", name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -682,15 +682,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/send_ble_beacon"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteDevicesUpgrade")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteDevicesUpgrade")  
 def getSiteDevicesUpgrade(mist_session:_APISession, site_id:str, status:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesUpgrade
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -840,15 +840,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/upgrade_bios"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteAvailableDeviceVersions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteAvailableDeviceVersions")  
 def getSiteAvailableDeviceVersions(mist_session:_APISession, site_id:str, type:str="ap", model:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAvailableDeviceVersions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/events.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/events.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/evpn_topologies.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/evpn_topologies.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/gatewaytemplates.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/gatewaytemplates.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/guests.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/guests.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteAllGuestAuthorizations")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteAllGuestAuthorizations")  
 def getSiteAllGuestAuthorizations(mist_session:_APISession, site_id:str, wlan_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAllGuestAuthorizations
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/insights.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/insights.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteRogueAPs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteRogueAPs")  
 def getSiteRogueAPs(mist_session:_APISession, site_id:str, type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueAPs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -167,15 +167,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteRogueClients")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteRogueClients")  
 def getSiteRogueClients(mist_session:_APISession, site_id:str, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueClients
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/licenses.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/location.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/location.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/maps.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteMaps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteMaps")  
 def getSiteMaps(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMaps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/mxedges.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/mxedges.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteMxEdges")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteMxEdges")  
 def getSiteMxEdges(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdges
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/mxtunnels.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/mxtunnels.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/nac_clients.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/nac_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/networks.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/networks.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteNetworksDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteNetworksDerived")  
 def getSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/networktemplates.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/networktemplates.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/otherdevices.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/otherdevices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteOtherDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteOtherDevices")  
 def getSiteOtherDevices(mist_session:_APISession, site_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteOtherDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/pcaps.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/pcaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSitePacketCaptures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSitePacketCaptures")  
 def getSitePacketCaptures(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", client_mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePacketCaptures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/psks.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/psks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSitePsks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSitePsks")  
 def getSitePsks(mist_session:_APISession, site_id:str, ssid:str=None, role:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePsks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/rfdiags.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/rfdiags.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/rftemplates.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/rftemplates.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/rogues.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/rogues.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/rrm.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/rrm.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/rssizones.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/rssizones.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteRssiZones")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteRssiZones")  
 def getSiteRssiZones(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRssiZones
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/servicepolicies.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/servicepolicies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteServicePoliciesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteServicePoliciesDerived")  
 def getSiteServicePoliciesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteServicePoliciesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/services.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteServicesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteServicesDerived")  
 def getSiteServicesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteServicesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/setting.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/setting.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/sites.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/sites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/sitetemplates.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/sitetemplates.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/skyatp.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/skyatp.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/sle.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/sle.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/ssr.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/ssr.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/stats.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     if distinct: query_params["distinct"]=distinct
     if device_mac: query_params["device_mac"]=device_mac
     if app: query_params["app"]=app
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteAssetsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteAssetsStats")  
 def getSiteAssetsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -266,15 +266,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteBeaconsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteBeaconsStats")  
 def getSiteBeaconsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeaconsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -515,15 +515,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteWirelessClientsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteWirelessClientsStats")  
 def getSiteWirelessClientsStats(mist_session:_APISession, site_id:str, wired:bool=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWirelessClientsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -617,15 +617,15 @@
     """
     uri = f"/api/v1/sites/{site_id}/stats/clients/{client_mac}"
     query_params={}
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteDevicesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteDevicesStats")  
 def getSiteDevicesStats(mist_session:_APISession, site_id:str, type:str="ap", status:str="all", page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -734,15 +734,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/devices/{device_id}/clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteDiscoveredAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteDiscoveredAssets")  
 def getSiteDiscoveredAssets(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDiscoveredAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1107,15 +1107,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/sdkclients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteUnconnectedClientStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteUnconnectedClientStats")  
 def getSiteUnconnectedClientStats(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteUnconnectedClientStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1156,15 +1156,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/unconnected_clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteMxEdgesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteMxEdgesStats")  
 def getSiteMxEdgesStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdgesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1827,15 +1827,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/wxrules"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteZonesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteZonesStats")  
 def getSiteZonesStats(mist_session:_APISession, site_id:str, map_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteZonesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/subscriptions.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/synthetic_test.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/uisettings.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/uisettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteUiSettings")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteUiSettings")  
 def getSiteUiSettings(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteUiSettings
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/vbeacons.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/vbeacons.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteVBeacons")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteVBeacons")  
 def getSiteVBeacons(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteVBeacons
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/visits.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/visits.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/vpns.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/vpns.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteVpnsDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteVpnsDerived")  
 def getSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteVpnsDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/wan_client.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/wan_client.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/wan_clients.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/wan_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/webhooks.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/webhooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteWebhooks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteWebhooks")  
 def getSiteWebhooks(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWebhooks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/wired_clients.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/wlans.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/wlans.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteWlans")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteWlans")  
 def getSiteWlans(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWlans
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -98,15 +98,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wlans"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteWlanDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteWlanDerived")  
 def getSiteWlanDerived(mist_session:_APISession, site_id:str, resolve:bool=None, wlan_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWlanDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/wxrules.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/wxrules.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteWxRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteWxRules")  
 def getSiteWxRules(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/wxtags.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/wxtags.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteWxTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteWxTags")  
 def getSiteWxTags(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/wxtunnels.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/wxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteWxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteWxTunnels")  
 def getSiteWxTunnels(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/sites/zones.py` & `mistapi-0.47.3/src/mistapi/api/v1/sites/zones.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.2", details="function replaced with listSiteZones")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.3", details="function replaced with listSiteZones")  
 def getSiteZones(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteZones
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/utils/test_telstra.py` & `mistapi-0.47.3/src/mistapi/api/v1/utils/test_telstra.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/api/v1/utils/test_twilio.py` & `mistapi-0.47.3/src/mistapi/api/v1/utils/test_twilio.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi/cli.py` & `mistapi-0.47.3/src/mistapi/cli.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.2/src/mistapi.egg-info/PKG-INFO` & `mistapi-0.47.3/src/mistapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.47.2
+Version: 0.47.3
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.47.2/src/mistapi.egg-info/SOURCES.txt` & `mistapi-0.47.3/src/mistapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

