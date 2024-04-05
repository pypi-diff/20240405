# Comparing `tmp/jj-2.9.0.tar.gz` & `tmp/jj-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jj-2.9.0.tar", last modified: Thu Dec 21 18:37:39 2023, max compression
+gzip compressed data, was "jj-2.9.1.tar", last modified: Sun Feb 25 05:35:16 2024, max compression
```

## Comparing `jj-2.9.0.tar` & `jj-2.9.1.tar`

### file list

```diff
@@ -1,126 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.897750 jj-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-21 18:37:28.000000 jj-2.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-12-21 18:37:39.897750 jj-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2023-12-21 18:37:28.000000 jj-2.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.885750 jj-2.9.0/jj/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-12-21 18:37:28.000000 jj-2.9.0/jj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-12-21 18:37:28.000000 jj-2.9.0/jj/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2023-12-21 18:37:28.000000 jj-2.9.0/jj/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-12-21 18:37:28.000000 jj-2.9.0/jj/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.885750 jj-2.9.0/jj/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-12-21 18:37:28.000000 jj-2.9.0/jj/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-21 18:37:28.000000 jj-2.9.0/jj/apps/_abstract_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2023-12-21 18:37:28.000000 jj-2.9.0/jj/apps/_base_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-12-21 18:37:28.000000 jj-2.9.0/jj/apps/_default_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.885750 jj-2.9.0/jj/expiration_policy/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-12-21 18:37:28.000000 jj-2.9.0/jj/expiration_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-12-21 18:37:28.000000 jj-2.9.0/jj/expiration_policy/_expiration_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2023-12-21 18:37:28.000000 jj-2.9.0/jj/expiration_policy/_expire_after_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2023-12-21 18:37:28.000000 jj-2.9.0/jj/expiration_policy/_expire_never.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.885750 jj-2.9.0/jj/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-21 18:37:28.000000 jj-2.9.0/jj/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-21 18:37:28.000000 jj-2.9.0/jj/handlers/_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-21 18:37:28.000000 jj-2.9.0/jj/handlers/_handler_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.885750 jj-2.9.0/jj/http/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-12-21 18:37:28.000000 jj-2.9.0/jj/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.885750 jj-2.9.0/jj/http/codes/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-12-21 18:37:28.000000 jj-2.9.0/jj/http/codes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.885750 jj-2.9.0/jj/http/headers/
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2023-12-21 18:37:28.000000 jj-2.9.0/jj/http/headers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.889750 jj-2.9.0/jj/http/methods/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-12-21 18:37:28.000000 jj-2.9.0/jj/http/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.889750 jj-2.9.0/jj/logs/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-12-21 18:37:28.000000 jj-2.9.0/jj/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-21 18:37:28.000000 jj-2.9.0/jj/logs/_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-21 18:37:28.000000 jj-2.9.0/jj/logs/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-21 18:37:28.000000 jj-2.9.0/jj/logs/_request_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.889750 jj-2.9.0/jj/logs/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-21 18:37:28.000000 jj-2.9.0/jj/logs/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-21 18:37:28.000000 jj-2.9.0/jj/logs/formatters/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-12-21 18:37:28.000000 jj-2.9.0/jj/logs/formatters/_simple_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.889750 jj-2.9.0/jj/matchers/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/_resolvable_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.889750 jj-2.9.0/jj/matchers/attribute_matchers/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/attribute_matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/attribute_matchers/_attribute_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/attribute_matchers/_contain_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/attribute_matchers/_equal_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/attribute_matchers/_exist_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/attribute_matchers/_multi_dict_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/attribute_matchers/_regex_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/attribute_matchers/_route_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.889750 jj-2.9.0/jj/matchers/logical_matchers/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/logical_matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/logical_matchers/_all_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/logical_matchers/_any_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/logical_matchers/_logical_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.893750 jj-2.9.0/jj/matchers/request_matchers/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/request_matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/request_matchers/_header_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/request_matchers/_method_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/request_matchers/_param_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/request_matchers/_path_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-21 18:37:28.000000 jj-2.9.0/jj/matchers/request_matchers/_request_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.893750 jj-2.9.0/jj/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-12-21 18:37:28.000000 jj-2.9.0/jj/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-12-21 18:37:28.000000 jj-2.9.0/jj/middlewares/_abstract_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-12-21 18:37:28.000000 jj-2.9.0/jj/middlewares/_base_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2023-12-21 18:37:28.000000 jj-2.9.0/jj/middlewares/_logger_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-21 18:37:28.000000 jj-2.9.0/jj/middlewares/_middleware_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2023-12-21 18:37:28.000000 jj-2.9.0/jj/middlewares/_root_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-21 18:37:28.000000 jj-2.9.0/jj/middlewares/_self_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.893750 jj-2.9.0/jj/mock/
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.897750 jj-2.9.0/jj/mock/_history/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_history/_body_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_history/_history_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.897750 jj-2.9.0/jj/mock/_history/_history_formatter/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_history/_history_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_history/_history_formatter/_history_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_history/_history_formatter/_pretty_history_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_history/_history_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_history/_history_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_history/_history_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_history/_history_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6773 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_mocked.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_remote_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_remote_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_stacked.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_system_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-12-21 18:37:28.000000 jj-2.9.0/jj/mock/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:28.000000 jj-2.9.0/jj/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.897750 jj-2.9.0/jj/requests/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-21 18:37:28.000000 jj-2.9.0/jj/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2023-12-21 18:37:28.000000 jj-2.9.0/jj/requests/_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.897750 jj-2.9.0/jj/resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-12-21 18:37:28.000000 jj-2.9.0/jj/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-12-21 18:37:28.000000 jj-2.9.0/jj/resolvers/_matcher_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2023-12-21 18:37:28.000000 jj-2.9.0/jj/resolvers/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2023-12-21 18:37:28.000000 jj-2.9.0/jj/resolvers/_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-12-21 18:37:28.000000 jj-2.9.0/jj/resolvers/_reversed_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.897750 jj-2.9.0/jj/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-21 18:37:28.000000 jj-2.9.0/jj/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2023-12-21 18:37:28.000000 jj-2.9.0/jj/responses/_delayed_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2023-12-21 18:37:28.000000 jj-2.9.0/jj/responses/_relay_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2023-12-21 18:37:28.000000 jj-2.9.0/jj/responses/_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2023-12-21 18:37:28.000000 jj-2.9.0/jj/responses/_static_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2023-12-21 18:37:28.000000 jj-2.9.0/jj/responses/_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-21 18:37:28.000000 jj-2.9.0/jj/responses/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.897750 jj-2.9.0/jj/runners/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-21 18:37:28.000000 jj-2.9.0/jj/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2023-12-21 18:37:28.000000 jj-2.9.0/jj/runners/_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.897750 jj-2.9.0/jj/servers/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-21 18:37:28.000000 jj-2.9.0/jj/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2023-12-21 18:37:28.000000 jj-2.9.0/jj/servers/_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 18:37:39.897750 jj-2.9.0/jj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-12-21 18:37:39.000000 jj-2.9.0/jj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2023-12-21 18:37:39.000000 jj-2.9.0/jj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 18:37:39.000000 jj-2.9.0/jj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-12-21 18:37:39.000000 jj-2.9.0/jj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2023-12-21 18:37:39.000000 jj-2.9.0/jj.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-21 18:37:39.901750 jj-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2023-12-21 18:37:28.000000 jj-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.183235 jj-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-25 05:35:09.000000 jj-2.9.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-02-25 05:35:16.183235 jj-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-02-25 05:35:09.000000 jj-2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.171235 jj-2.9.1/jj/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-02-25 05:35:09.000000 jj-2.9.1/jj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-25 05:35:09.000000 jj-2.9.1/jj/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-02-25 05:35:09.000000 jj-2.9.1/jj/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-25 05:35:09.000000 jj-2.9.1/jj/_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-25 05:35:09.000000 jj-2.9.1/jj/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.171235 jj-2.9.1/jj/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-25 05:35:09.000000 jj-2.9.1/jj/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-25 05:35:09.000000 jj-2.9.1/jj/apps/_abstract_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-02-25 05:35:09.000000 jj-2.9.1/jj/apps/_base_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-25 05:35:09.000000 jj-2.9.1/jj/apps/_default_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.171235 jj-2.9.1/jj/expiration_policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-25 05:35:09.000000 jj-2.9.1/jj/expiration_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-25 05:35:09.000000 jj-2.9.1/jj/expiration_policy/_expiration_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-02-25 05:35:09.000000 jj-2.9.1/jj/expiration_policy/_expire_after_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-02-25 05:35:09.000000 jj-2.9.1/jj/expiration_policy/_expire_never.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.175235 jj-2.9.1/jj/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 05:35:09.000000 jj-2.9.1/jj/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-25 05:35:09.000000 jj-2.9.1/jj/handlers/_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-25 05:35:09.000000 jj-2.9.1/jj/handlers/_handler_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.175235 jj-2.9.1/jj/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 05:35:09.000000 jj-2.9.1/jj/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.175235 jj-2.9.1/jj/http/codes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-02-25 05:35:09.000000 jj-2.9.1/jj/http/codes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.175235 jj-2.9.1/jj/http/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-02-25 05:35:09.000000 jj-2.9.1/jj/http/headers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.175235 jj-2.9.1/jj/http/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-25 05:35:09.000000 jj-2.9.1/jj/http/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.175235 jj-2.9.1/jj/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-25 05:35:09.000000 jj-2.9.1/jj/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-25 05:35:09.000000 jj-2.9.1/jj/logs/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-25 05:35:09.000000 jj-2.9.1/jj/logs/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-25 05:35:09.000000 jj-2.9.1/jj/logs/_request_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.175235 jj-2.9.1/jj/logs/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-25 05:35:09.000000 jj-2.9.1/jj/logs/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-25 05:35:09.000000 jj-2.9.1/jj/logs/formatters/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-25 05:35:09.000000 jj-2.9.1/jj/logs/formatters/_simple_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.175235 jj-2.9.1/jj/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/_resolvable_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.175235 jj-2.9.1/jj/matchers/attribute_matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/attribute_matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/attribute_matchers/_attribute_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/attribute_matchers/_contain_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/attribute_matchers/_equal_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/attribute_matchers/_exist_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/attribute_matchers/_multi_dict_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/attribute_matchers/_regex_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/attribute_matchers/_route_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.175235 jj-2.9.1/jj/matchers/logical_matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/logical_matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/logical_matchers/_all_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/logical_matchers/_any_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/logical_matchers/_logical_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.179235 jj-2.9.1/jj/matchers/request_matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/request_matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/request_matchers/_header_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/request_matchers/_method_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/request_matchers/_param_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/request_matchers/_path_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 05:35:09.000000 jj-2.9.1/jj/matchers/request_matchers/_request_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.179235 jj-2.9.1/jj/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-25 05:35:09.000000 jj-2.9.1/jj/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-02-25 05:35:09.000000 jj-2.9.1/jj/middlewares/_abstract_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-02-25 05:35:09.000000 jj-2.9.1/jj/middlewares/_base_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-02-25 05:35:09.000000 jj-2.9.1/jj/middlewares/_logger_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-25 05:35:09.000000 jj-2.9.1/jj/middlewares/_middleware_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-25 05:35:09.000000 jj-2.9.1/jj/middlewares/_root_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-25 05:35:09.000000 jj-2.9.1/jj/middlewares/_self_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.179235 jj-2.9.1/jj/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.179235 jj-2.9.1/jj/mock/_history/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_history/_body_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_history/_history_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.183235 jj-2.9.1/jj/mock/_history/_history_formatter/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_history/_history_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_history/_history_formatter/_history_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_history/_history_formatter/_pretty_history_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_history/_history_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_history/_history_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_history/_history_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_history/_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_mocked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_remote_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_remote_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_system_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-02-25 05:35:09.000000 jj-2.9.1/jj/mock/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:09.000000 jj-2.9.1/jj/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.183235 jj-2.9.1/jj/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-25 05:35:09.000000 jj-2.9.1/jj/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-02-25 05:35:09.000000 jj-2.9.1/jj/requests/_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.183235 jj-2.9.1/jj/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-25 05:35:09.000000 jj-2.9.1/jj/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-25 05:35:09.000000 jj-2.9.1/jj/resolvers/_matcher_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-02-25 05:35:09.000000 jj-2.9.1/jj/resolvers/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-02-25 05:35:09.000000 jj-2.9.1/jj/resolvers/_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-25 05:35:09.000000 jj-2.9.1/jj/resolvers/_reversed_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.183235 jj-2.9.1/jj/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-25 05:35:09.000000 jj-2.9.1/jj/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-02-25 05:35:09.000000 jj-2.9.1/jj/responses/_delayed_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-02-25 05:35:09.000000 jj-2.9.1/jj/responses/_relay_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-02-25 05:35:09.000000 jj-2.9.1/jj/responses/_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-25 05:35:09.000000 jj-2.9.1/jj/responses/_static_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-02-25 05:35:09.000000 jj-2.9.1/jj/responses/_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-02-25 05:35:09.000000 jj-2.9.1/jj/responses/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.183235 jj-2.9.1/jj/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-25 05:35:09.000000 jj-2.9.1/jj/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-02-25 05:35:09.000000 jj-2.9.1/jj/runners/_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.183235 jj-2.9.1/jj/servers/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-25 05:35:09.000000 jj-2.9.1/jj/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-02-25 05:35:09.000000 jj-2.9.1/jj/servers/_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 05:35:16.183235 jj-2.9.1/jj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-02-25 05:35:16.000000 jj-2.9.1/jj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-02-25 05:35:16.000000 jj-2.9.1/jj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 05:35:16.000000 jj-2.9.1/jj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 05:35:16.000000 jj-2.9.1/jj.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-25 05:35:16.000000 jj-2.9.1/jj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-25 05:35:16.000000 jj-2.9.1/jj.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-25 05:35:16.187234 jj-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-25 05:35:09.000000 jj-2.9.1/setup.py
```

### Comparing `jj-2.9.0/LICENSE.txt` & `jj-2.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/PKG-INFO` & `jj-2.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: jj
-Version: 2.9.0
+Version: 2.9.1
 Summary: Remote HTTP Mock
 Home-page: https://github.com/jj-mock/jj
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
+Project-URL: Docs, https://jj.vedro.io
+Project-URL: GitHub, https://github.com/jj-mock/jj
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
```

### Comparing `jj-2.9.0/README.md` & `jj-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/__init__.py` & `jj-2.9.1/jj/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/_core.py` & `jj-2.9.1/jj/_core.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/apps/_base_app.py` & `jj-2.9.1/jj/apps/_base_app.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/expiration_policy/_expire_after_requests.py` & `jj-2.9.1/jj/expiration_policy/_expire_after_requests.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/expiration_policy/_expire_never.py` & `jj-2.9.1/jj/expiration_policy/_expire_never.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/http/codes/__init__.py` & `jj-2.9.1/jj/http/codes/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/http/headers/__init__.py` & `jj-2.9.1/jj/http/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/logs/__init__.py` & `jj-2.9.1/jj/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/logs/_filter.py` & `jj-2.9.1/jj/logs/_filter.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/logs/formatters/_formatter.py` & `jj-2.9.1/jj/logs/formatters/_formatter.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/logs/formatters/_simple_formatter.py` & `jj-2.9.1/jj/logs/formatters/_simple_formatter.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/matchers/__init__.py` & `jj-2.9.1/jj/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/matchers/_resolvable_matcher.py` & `jj-2.9.1/jj/matchers/_resolvable_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/matchers/attribute_matchers/__init__.py` & `jj-2.9.1/jj/matchers/attribute_matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/matchers/attribute_matchers/_contain_matcher.py` & `jj-2.9.1/jj/matchers/attribute_matchers/_contain_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/matchers/attribute_matchers/_equal_matcher.py` & `jj-2.9.1/jj/matchers/attribute_matchers/_equal_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/matchers/attribute_matchers/_multi_dict_matcher.py` & `jj-2.9.1/jj/matchers/attribute_matchers/_multi_dict_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/matchers/attribute_matchers/_regex_matcher.py` & `jj-2.9.1/jj/matchers/attribute_matchers/_regex_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/matchers/attribute_matchers/_route_matcher.py` & `jj-2.9.1/jj/matchers/attribute_matchers/_route_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/matchers/logical_matchers/_all_matcher.py` & `jj-2.9.1/jj/matchers/logical_matchers/_all_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/matchers/logical_matchers/_any_matcher.py` & `jj-2.9.1/jj/matchers/logical_matchers/_any_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/matchers/request_matchers/_header_matcher.py` & `jj-2.9.1/jj/matchers/request_matchers/_header_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/matchers/request_matchers/_method_matcher.py` & `jj-2.9.1/jj/matchers/request_matchers/_method_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/matchers/request_matchers/_param_matcher.py` & `jj-2.9.1/jj/matchers/request_matchers/_param_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/matchers/request_matchers/_path_matcher.py` & `jj-2.9.1/jj/matchers/request_matchers/_path_matcher.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/middlewares/_abstract_middleware.py` & `jj-2.9.1/jj/middlewares/_abstract_middleware.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/middlewares/_base_middleware.py` & `jj-2.9.1/jj/middlewares/_base_middleware.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/middlewares/_logger_middleware.py` & `jj-2.9.1/jj/middlewares/_logger_middleware.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/middlewares/_self_middleware.py` & `jj-2.9.1/jj/middlewares/_self_middleware.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/mock/__init__.py` & `jj-2.9.1/jj/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/mock/_history/__init__.py` & `jj-2.9.1/jj/mock/_history/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/mock/_history/_body_parser.py` & `jj-2.9.1/jj/mock/_history/_body_parser.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/mock/_history/_history_formatter/_pretty_history_formatter.py` & `jj-2.9.1/jj/mock/_history/_history_formatter/_pretty_history_formatter.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/mock/_history/_history_repository.py` & `jj-2.9.1/jj/mock/_history/_history_repository.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/mock/_history/_history_request.py` & `jj-2.9.1/jj/mock/_history/_history_request.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/mock/_history/_history_response.py` & `jj-2.9.1/jj/mock/_history/_history_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/mock/_mock.py` & `jj-2.9.1/jj/mock/_mock.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/mock/_mocked.py` & `jj-2.9.1/jj/mock/_mocked.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 class Mocked:
     def __init__(self, handler: RemoteHandler, *,
                  disposable: bool = True,
                  prefetch_history: bool = True,
                  history_formatter: Optional[HistoryFormatter] = None
                  ) -> None:
         self._handler = handler
-        self._disposable = disposable
-        self._prefetch_history = prefetch_history
+        self._disposable = disposable  # Deprecated, will be removed in future versions
+        self._prefetch_history = prefetch_history  # Enable history prefetching in a `with` context
         self._history: Union[List[HistoryItem], None] = None
         self._history_formatter = history_formatter
 
     @property
     def handler(self) -> RemoteHandler:
         return self._handler
```

### Comparing `jj-2.9.0/jj/mock/_remote_handler.py` & `jj-2.9.1/jj/mock/_remote_handler.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/mock/_remote_mock.py` & `jj-2.9.1/jj/mock/_remote_mock.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/mock/_stacked.py` & `jj-2.9.1/jj/mock/_stacked.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/mock/_utils.py` & `jj-2.9.1/jj/mock/_utils.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/requests/_request.py` & `jj-2.9.1/jj/requests/_request.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/resolvers/_registry.py` & `jj-2.9.1/jj/resolvers/_registry.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/resolvers/_resolver.py` & `jj-2.9.1/jj/resolvers/_resolver.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/responses/_delayed_response.py` & `jj-2.9.1/jj/responses/_delayed_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/responses/_relay_response.py` & `jj-2.9.1/jj/responses/_relay_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/responses/_response.py` & `jj-2.9.1/jj/responses/_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/responses/_static_response.py` & `jj-2.9.1/jj/responses/_static_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/responses/_stream_response.py` & `jj-2.9.1/jj/responses/_stream_response.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/responses/_utils.py` & `jj-2.9.1/jj/responses/_utils.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/runners/_runner.py` & `jj-2.9.1/jj/runners/_runner.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj/servers/_server.py` & `jj-2.9.1/jj/servers/_server.py`

 * *Files identical despite different names*

### Comparing `jj-2.9.0/jj.egg-info/PKG-INFO` & `jj-2.9.1/jj.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: jj
-Version: 2.9.0
+Version: 2.9.1
 Summary: Remote HTTP Mock
 Home-page: https://github.com/jj-mock/jj
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
+Project-URL: Docs, https://jj.vedro.io
+Project-URL: GitHub, https://github.com/jj-mock/jj
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
```

### Comparing `jj-2.9.0/jj.egg-info/SOURCES.txt` & `jj-2.9.1/jj.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE.txt
 README.md
 setup.cfg
 setup.py
 jj/__init__.py
 jj/__main__.py
 jj/_core.py
+jj/_entry_point.py
 jj/_version.py
 jj/py.typed
 jj.egg-info/PKG-INFO
 jj.egg-info/SOURCES.txt
 jj.egg-info/dependency_links.txt
+jj.egg-info/entry_points.txt
 jj.egg-info/requires.txt
 jj.egg-info/top_level.txt
 jj/apps/__init__.py
 jj/apps/_abstract_app.py
 jj/apps/_base_app.py
 jj/apps/_default_app.py
 jj/expiration_policy/__init__.py
```

### Comparing `jj-2.9.0/setup.cfg` & `jj-2.9.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.9.0
+current_version = 2.9.1
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `jj-2.9.0/setup.py` & `jj-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,30 +9,36 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="jj",
-    version="2.9.0",
+    version="2.9.1",
     description="Remote HTTP Mock",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.8",
     url="https://github.com/jj-mock/jj",
+    project_urls={
+        "Docs": "https://jj.vedro.io",
+        "GitHub": "https://github.com/jj-mock/jj",
+    },
     license="Apache-2.0",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"jj": ["py.typed"]},
+    entry_points={
+        "console_scripts": ["jj = jj._entry_point:run"]
+    },
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Typing :: Typed",
     ],
```

