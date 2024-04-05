# Comparing `tmp/oarepo-dashboard-1.0.3.tar.gz` & `tmp/oarepo-dashboard-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-dashboard-1.0.3.tar", last modified: Wed Apr  3 15:18:30 2024, max compression
+gzip compressed data, was "oarepo-dashboard-1.0.4.tar", last modified: Fri Apr  5 13:56:05 2024, max compression
```

## Comparing `oarepo-dashboard-1.0.3.tar` & `oarepo-dashboard-1.0.4.tar`

### file list

```diff
@@ -1,102 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.875236 oarepo-dashboard-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-03 15:18:30.875236 oarepo-dashboard-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.863236 oarepo-dashboard-1.0.3/oarepo_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.867236 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.859236 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.867236 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/semantic-ui/translations/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/semantic-ui/translations/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.867236 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/semantic-ui/translations/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.859236 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.867236 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.859236 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.867236 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/LC_MESSAGES/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/semantic-ui/translations/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.867236 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.859236 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.867236 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.859236 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.867236 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.867236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.867236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.859236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.859236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.859236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.867236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/CommunityTypeLabel.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/ComputerTabletCommunitiesListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/MobileCommunitiesListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/RestrictedLabel.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.867236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/templates/DashboardCommunitiesPage.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.871236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.859236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.859236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.871236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/custom-components.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.871236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupNameToggler.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupValueToggler.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppLayout.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppResultView.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.871236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/custom-components.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.871236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/templates/Header.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.871236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_records/
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.863236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_records/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.863236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.863236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.871236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.871236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_records/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_records/templates/DashboardRecordsPage.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_records/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.871236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.863236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.863236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.863236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.871236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/ComputerTabletRequestsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/MobileRequestsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/RequestTypeSpecificComponents.jsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.871236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/icons/TypeIcons.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.871236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/TypeLabels.jsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.871236 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/templates/DashboardRequestsPage.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:18:30.875236 oarepo-dashboard-1.0.3/oarepo_dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-03 15:18:30.000000 oarepo-dashboard-1.0.3/oarepo_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-03 15:18:30.000000 oarepo-dashboard-1.0.3/oarepo_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:18:30.000000 oarepo-dashboard-1.0.3/oarepo_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-03 15:18:30.000000 oarepo-dashboard-1.0.3/oarepo_dashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 15:18:30.000000 oarepo-dashboard-1.0.3/oarepo_dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 15:18:30.000000 oarepo-dashboard-1.0.3/oarepo_dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-03 15:18:30.875236 oarepo-dashboard-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:16:38.000000 oarepo-dashboard-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/LC_MESSAGES/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/CommunityTypeLabel.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/ComputerTabletCommunitiesListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/MobileCommunitiesListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/RestrictedLabel.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/templates/DashboardCommunitiesPage.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/custom-components.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupNameToggler.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppLayout.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppResultView.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/custom-components.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/templates/Header.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/templates/DashboardRecordsPage.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/ComputerTabletRequestsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/MobileRequestsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/RequestTypeSpecificComponents.jsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/icons/TypeIcons.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/TypeLabels.jsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/templates/DashboardRequestsPage.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-05 13:56:05.000000 oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-05 13:56:05.000000 oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:56:05.000000 oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-05 13:56:05.000000 oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-05 13:56:05.000000 oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 13:56:05.000000 oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-05 13:56:05.965761 oarepo-dashboard-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/setup.py
```

### Comparing `oarepo-dashboard-1.0.3/PKG-INFO` & `oarepo-dashboard-1.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-dashboard
-Version: 1.0.3
+Version: 1.0.4
 Summary: Support for user dashboard (records, communities, requests)
 Description-Content-Type: text/markdown
 Requires-Dist: oarepo-runtime>=1.4.44
 Requires-Dist: openpyxl
 Requires-Dist: oarepo-ui>=5.0.91
 Requires-Dist: cachetools
 Provides-Extra: dev
```

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/semantic-ui/translations/i18next.js` & `oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/translations.json` & `oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.mo` & `oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.po` & `oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.po` & `oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/i18n/translations/messages.pot` & `oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/__init__.py` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/CommunityTypeLabel.jsx` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/CommunityTypeLabel.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/ComputerTabletCommunitiesListItem.jsx` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/ComputerTabletCommunitiesListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/MobileCommunitiesListItem.jsx` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/MobileCommunitiesListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/index.js` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/index.js`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupNameToggler.jsx` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupNameToggler.jsx`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import React, { useContext } from "react";
 import PropTypes from "prop-types";
-import { i18next } from "@translations/oarepo_dashboard";
 import { Button } from "semantic-ui-react";
 import { withState } from "react-searchkit";
 import { SearchConfigurationContext } from "@js/invenio_search_ui/components";
 
 const FacetsButtonGroupNameTogglerComponent = ({
   currentResultsState,
   currentQueryState,
   updateQueryState,
-  facetNames,
-  firstFacetButtonText,
-  secondFacetButtonText,
+  toggledFilters,
   keepFiltersOnUpdate,
   ...uiProps
 }) => {
   const { initialQueryState } = useContext(SearchConfigurationContext);
   const currentFilter = currentQueryState.filters?.find((f) =>
-    facetNames.includes(f[0])
+    toggledFilters.map((f) => f.filterName).includes(f[0])
   );
   const initialQueryFacets = initialQueryState.filters?.map((f) => f[0]);
   if (!currentFilter)
     console.error(
       "FacetsButtonGroup: Query does not contain any of the facets you wish to toggle between, please make sure you are passing initialFilters properly"
     );
   const facetStatus = currentFilter && JSON.parse(currentFilter?.[1]);
@@ -36,50 +33,48 @@
           ...(currentQueryState?.filters
             ? currentQueryState.filters.filter((element) =>
                 initialQueryFacets.includes(element[0])
               )
             : []),
         ];
     currentQueryState.filters = currentQueryState.filters.filter(
-      (f) => !facetNames.includes(f[0])
+      (f) => !toggledFilters.map((f) => f.filterName).includes(f[0])
     );
 
     currentQueryState.filters.push([facetName, facetStatus]);
     updateQueryState(currentQueryState);
   };
   return (
-    <Button.Group size="mini" className="rel-mb-1" {...uiProps}>
-      <Button
-        onClick={() => handleFacetNameChange(facetNames[0])}
-        className="request-search-filter"
-        active={facetNames[0] === currentFilter[0]}
-      >
-        {firstFacetButtonText}
-      </Button>
-      <Button
-        onClick={() => handleFacetNameChange(facetNames[1])}
-        className="request-search-filter"
-        active={facetNames[1] === currentFilter[0]}
-      >
-        {secondFacetButtonText}
-      </Button>
+    <Button.Group className="rel-mb-1" {...uiProps}>
+      {toggledFilters.map(({ text, filterName }) => (
+        <Button
+          key={filterName}
+          className="request-search-filter"
+          onClick={() => handleFacetNameChange(filterName)}
+          active={filterName === currentFilter[0]}
+        >
+          {text}
+        </Button>
+      ))}
     </Button.Group>
   );
 };
 
 FacetsButtonGroupNameTogglerComponent.propTypes = {
   currentQueryState: PropTypes.object.isRequired,
   updateQueryState: PropTypes.func.isRequired,
   currentResultsState: PropTypes.object.isRequired,
-  facetNames: PropTypes.array.isRequired,
-  firstFacetButtonText: PropTypes.string,
-  secondFacetButtonText: PropTypes.string,
+  toggledFilters: PropTypes.arrayOf(
+    PropTypes.shape({
+      filterName: PropTypes.string.isRequired,
+      text: PropTypes.string.isRequired,
+    })
+  ).isRequired,
   keepFiltersOnUpdate: PropTypes.bool,
 };
+
 FacetsButtonGroupNameTogglerComponent.defaultProps = {
-  firstFacetButtonText: i18next.t("My"),
-  secondFacetButtonText: i18next.t("Others"),
   keepFiltersOnUpdate: true,
 };
 export const FacetsButtonGroupNameToggler = withState(
   FacetsButtonGroupNameTogglerComponent
 );
```

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppLayout.jsx` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppLayout.jsx`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 } from "@js/invenio_search_ui/components";
 import { i18next } from "@translations/oarepo_dashboard";
 import React, { useContext } from "react";
 import { SearchBar, ActiveFilters } from "react-searchkit";
 import { GridResponsiveSidebarColumn } from "react-invenio-forms";
 import { Grid, Button, Container } from "semantic-ui-react";
 import PropTypes from "prop-types";
-import { SearchAppFacets, ClearFiltersButton } from "@js/oarepo_ui";
+import {
+  SearchAppFacets,
+  ClearFiltersButton,
+  ShouldActiveFiltersRender,
+} from "@js/oarepo_ui";
 import { QueryClient, QueryClientProvider } from "@tanstack/react-query";
 import Overridable from "react-overridable";
 
 const queryClient = new QueryClient();
 
 export const UserDashboardSearchAppLayoutHOC = ({
   placeholder,
@@ -43,22 +47,26 @@
               open={sidebarVisible}
               onHideClick={() => setSidebarVisible(false)}
             >
               <SearchAppFacets aggs={config.aggs} appName={appName} />
             </GridResponsiveSidebarColumn>
             <Grid.Column computer={13} mobile={16} tablet={16}>
               <Grid columns="equal">
-                <Grid.Row only="computer" verticalAlign="middle">
-                  <Grid.Column>
-                    <ActiveFilters />
-                    <Overridable id={buildUID("ClearFiltersButton.container")}>
-                      <ClearFiltersButton />
-                    </Overridable>
-                  </Grid.Column>
-                </Grid.Row>
+                <ShouldActiveFiltersRender>
+                  <Grid.Row only="computer" verticalAlign="middle">
+                    <Grid.Column>
+                      <ActiveFilters />
+                      <Overridable
+                        id={buildUID("ClearFiltersButton.container")}
+                      >
+                        <ClearFiltersButton />
+                      </Overridable>
+                    </Grid.Column>
+                  </Grid.Row>
+                </ShouldActiveFiltersRender>
                 <Grid.Row only="computer" verticalAlign="middle">
                   <Grid.Column>
                     <SearchBar placeholder={placeholder} className="rel-pl-1" />
                   </Grid.Column>
                   {extraContent && extraContent()}
                 </Grid.Row>
                 <Grid.Column only="mobile tablet" mobile={2} tablet={2}>
@@ -83,21 +91,25 @@
                   </Grid.Row>
                 )}
                 {mobileOnlyExtraRow && (
                   <Grid.Row verticalAlign="middle" only="mobile">
                     {mobileOnlyExtraRow()}
                   </Grid.Row>
                 )}
-                <Grid.Row only="mobile tablet">
-                  <Grid.Column>
-                    <Overridable id={buildUID("ClearFiltersButton.container")}>
-                      <ClearFiltersButton />
-                    </Overridable>
-                  </Grid.Column>
-                </Grid.Row>
+                <ShouldActiveFiltersRender>
+                  <Grid.Row only="mobile tablet">
+                    <Grid.Column>
+                      <Overridable
+                        id={buildUID("ClearFiltersButton.container")}
+                      >
+                        <ClearFiltersButton />
+                      </Overridable>
+                    </Grid.Column>
+                  </Grid.Row>
+                </ShouldActiveFiltersRender>
                 <Grid.Row>
                   <Grid.Column mobile={16} tablet={16} computer={16}>
                     <SearchAppResultsPane
                       layoutOptions={config.layoutOptions}
                       appName={appName}
                     />
                   </Grid.Column>
```

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppResultView.jsx` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppResultView.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_components/webpack.py` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/webpack.py`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_records/__init__.py` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/index.js` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/index.js`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/__init__.py` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/ComputerTabletRequestsListItem.jsx` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/ComputerTabletRequestsListItem.jsx`

 * *Files 0% similar despite different names*

```diff
@@ -26,26 +26,26 @@
   };
 
   return (
     <Item
       key={result.id}
       className="computer tablet only rel-p-1 rel-mb-1 result-list-item request"
     >
-      <div className="status-icon mr-10 mt-5">
+      <div className="status-icon mr-10">
         <Item.Content verticalAlign="top">
           <Item.Extra>
             <RequestTypeIcon type={result.type} />
           </Item.Extra>
         </Item.Content>
       </div>
       <Item.Content>
         <Item.Extra>
           {result.type && <RequestTypeLabel type={result.type} />}
           {result.status && result.is_closed && (
-            <RequestStatusLabel status={result.status} />
+            <RequestStatusLabel status={result.status_code} />
           )}
         </Item.Extra>
         {result?.topic?.status === "removed" ? (
           <Item.Header className="mt-5">
             {result?.title || result?.name}
           </Item.Header>
         ) : (
```

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/MobileRequestsListItem.jsx` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/MobileRequestsListItem.jsx`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
       key={result.id}
       className="mobile only rel-p-1 rel-mb-1 result-list-item request"
     >
       <Item.Content className="centered">
         <Item.Extra>
           {result.type && <RequestTypeLabel type={result.type} />}
           {result.status && result.is_closed && (
-            <RequestStatusLabel status={result.status} />
+            <RequestStatusLabel status={result.status_code} />
           )}
         </Item.Extra>
         {result?.topic?.status === "removed" ? (
           <Item.Header className="truncate-lines-2 rel-mt-1">
             <RequestTypeIcon type={result.type} />
             {result?.name || result?.title}
           </Item.Header>
```

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/RequestTypeSpecificComponents.jsx` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/RequestTypeSpecificComponents.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/index.js` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/index.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -12,26 +12,26 @@
     ActiveFiltersElement,
     ClearFiltersButton,
 } from "@js/oarepo_ui";
 import {
     withState
 } from "react-searchkit";
 import {
-    RequestsEmptyResultsWithState
+    RequestsEmptyResultsWithState,
+    RequestStatusFilter,
 } from "@js/invenio_requests/search";
 import {
     defaultContribComponents
 } from "@js/invenio_requests/contrib";
 import {
     PropTypes
 } from "prop-types";
 import {
     UserDashboardSearchAppLayoutHOC,
     UserDashboardSearchAppResultView,
-    FacetsButtonGroupValueToggler,
     FacetsButtonGroupNameToggler,
 } from "@js/dashboard_components";
 import {
     i18next
 } from "@translations/oarepo_dashboard";
 import {
     ComputerTabletRequestsListItem
@@ -81,33 +81,45 @@
 };
 export const FacetButtons = () => ( <
     React.Fragment >
     <
     Grid.Column only = "computer"
     textAlign = "right" >
     <
-    FacetsButtonGroupValueToggler facetName = "is_open" / >
+    RequestStatusFilter keepFiltersOnUpdate / >
     <
     span className = "rel-ml-2" > < /span> <
-    FacetsButtonGroupNameToggler facetNames = {
-        ["mine", "assigned"]
+    FacetsButtonGroupNameToggler basic toggledFilters = {
+        [{
+            text: i18next.t("My"),
+            filterName: "mine"
+        }, {
+            text: i18next.t("Others"),
+            filterName: "assigned"
+        }, ]
     }
     /> <
     /Grid.Column> <
     Grid.Column only = "mobile tablet"
     textAlign = "left" >
     <
-    FacetsButtonGroupValueToggler facetName = "is_open" / >
+    RequestStatusFilter keepFiltersOnUpdate / >
     <
     /Grid.Column> <
     Grid.Column only = "mobile tablet"
     textAlign = "right" >
     <
-    FacetsButtonGroupNameToggler facetNames = {
-        ["mine", "assigned"]
+    FacetsButtonGroupNameToggler basic toggledFilters = {
+        [{
+            text: i18next.t("My"),
+            filterName: "mine"
+        }, {
+            text: i18next.t("Others"),
+            filterName: "assigned"
+        }, ]
     }
     /> <
     /Grid.Column> <
     /React.Fragment>
 );
 
 const UserDashboardSearchAppResultViewWAppName = parametrize(
```

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/TypeLabels.jsx` & `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/TypeLabels.jsx`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import React from "react";
 import { Label } from "semantic-ui-react";
 import { i18next } from "@translations/oarepo_dashboard";
 
 export const LabelTypeEditRecord = (props) => (
-  <Label horizontal className="primary" size="small">
+  <Label horizontal size="small">
     {i18next.t("Edit record")}
   </Label>
 );
 
 export const LabelTypeDeleteRecord = (props) => (
-  <Label horizontal className="primary" size="small">
+  <Label horizontal size="small">
     {i18next.t("Delete record")}
   </Label>
 );
 
 export const LabelTypePublishRecord = (props) => (
-  <Label horizontal className="primary" size="small">
+  <Label horizontal size="small">
     {i18next.t("Publish record")}
   </Label>
 );
```

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard.egg-info/PKG-INFO` & `oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-dashboard
-Version: 1.0.3
+Version: 1.0.4
 Summary: Support for user dashboard (records, communities, requests)
 Description-Content-Type: text/markdown
 Requires-Dist: oarepo-runtime>=1.4.44
 Requires-Dist: openpyxl
 Requires-Dist: oarepo-ui>=5.0.91
 Requires-Dist: cachetools
 Provides-Extra: dev
```

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard.egg-info/SOURCES.txt` & `oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/index.js
 oarepo_dashboard/ui/dashboard_communities/templates/DashboardCommunitiesPage.jinja
 oarepo_dashboard/ui/dashboard_components/__init__.py
 oarepo_dashboard/ui/dashboard_components/search.py
 oarepo_dashboard/ui/dashboard_components/webpack.py
 oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/custom-components.js
 oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupNameToggler.jsx
-oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupValueToggler.jsx
 oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppLayout.jsx
 oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppResultView.jsx
 oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/index.js
 oarepo_dashboard/ui/dashboard_components/semantic-ui/less/custom-components.less
 oarepo_dashboard/ui/dashboard_components/templates/Header.jinja
 oarepo_dashboard/ui/dashboard_records/__init__.py
 oarepo_dashboard/ui/dashboard_records/webpack.py
```

### Comparing `oarepo-dashboard-1.0.3/oarepo_dashboard.egg-info/entry_points.txt` & `oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/entry_points.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,7 +6,10 @@
 oarepo_dashboard_requests_ui_theme = oarepo_dashboard.ui.dashboard_requests.webpack:theme
 
 [invenio_base.blueprints]
 oarepo_dashboard_communities = oarepo_dashboard.ui.dashboard_communities:create_blueprint
 oarepo_dashboard_components = oarepo_dashboard.ui.dashboard_components:create_blueprint
 oarepo_dashboard_records = oarepo_dashboard.ui.dashboard_records:create_blueprint
 oarepo_dashboard_requests = oarepo_dashboard.ui.dashboard_requests:create_blueprint
+
+[invenio_i18n.translations]
+oarepo_dashboard_messages = oarepo_dashboard.i18n
```

### Comparing `oarepo-dashboard-1.0.3/setup.cfg` & `oarepo-dashboard-1.0.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-dashboard
-version = 1.0.3
+version = 1.0.4
 description = Support for user dashboard (records, communities, requests)
 authors = Mirek Simek <miroslav.simek@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
@@ -42,12 +42,14 @@
 	oarepo_dashboard_components  = oarepo_dashboard.ui.dashboard_components:create_blueprint
 invenio_assets.webpack = 
 	oarepo_dashboard_i18n = oarepo_dashboard.i18n.webpack:theme
 	oarepo_dashboard_records_ui_theme = oarepo_dashboard.ui.dashboard_records.webpack:theme
 	oarepo_dashboard_requests_ui_theme = oarepo_dashboard.ui.dashboard_requests.webpack:theme
 	oarepo_dashboard_communities_ui_theme = oarepo_dashboard.ui.dashboard_communities.webpack:theme
 	oarepo_dashboard_components_ui_theme = oarepo_dashboard.ui.dashboard_components.webpack:theme
+invenio_i18n.translations = 
+	oarepo_dashboard_messages = oarepo_dashboard.i18n
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

