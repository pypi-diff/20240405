# Comparing `tmp/backend.ai-client-24.3.0rc2.tar.gz` & `tmp/backend.ai-client-24.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-client-24.3.0rc2.tar", last modified: Sun Mar 31 14:09:11 2024, max compression
+gzip compressed data, was "backend.ai-client-24.3.0rc3.tar", last modified: Fri Apr  5 02:25:38 2024, max compression
```

## Comparing `backend.ai-client-24.3.0rc2.tar` & `backend.ai-client-24.3.0rc3.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.835455 backend.ai-client-24.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-03-31 14:09:11.835455 backend.ai-client-24.3.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.819455 backend.ai-client-24.3.0rc2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.819455 backend.ai-client-24.3.0rc2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.819455 backend.ai-client-24.3.0rc2/ai/backend/client/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.823455 backend.ai-client-24.3.0rc2/ai/backend/client/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.827455 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/license.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/quota_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/announcement.py
--rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/pretty.py
--rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/server_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    20889 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.827455 backend.ai-client-24.3.0rc2/ai/backend/client/cli/session/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/session/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    30037 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/session/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)    47309 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/session/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/session/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/session_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    35705 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/cli/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    13291 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.831455 backend.ai-client-24.3.0rc2/ai/backend/client/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/bgtask.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/keypair_resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/quota_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/server_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    12337 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    51604 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/session_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    27656 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/func/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/load_balancing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.835455 backend.ai-client-24.3.0rc2/ai/backend/client/output/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/output/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/output/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    11925 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/output/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/output/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/output/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    29791 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/request.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    16998 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/ai/backend/client/versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:11.835455 backend.ai-client-24.3.0rc2/backend.ai_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/backend.ai_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/backend.ai_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/backend.ai_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/backend.ai_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/backend.ai_client.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/backend.ai_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/backend.ai_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/backend.ai_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 14:09:11.835455 backend.ai-client-24.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-03-31 14:09:11.000000 backend.ai-client-24.3.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.370052 backend.ai-client-24.3.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-04-05 02:25:38.370052 backend.ai-client-24.3.0rc3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.342052 backend.ai-client-24.3.0rc3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.346052 backend.ai-client-24.3.0rc3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.350052 backend.ai-client-24.3.0rc3/ai/backend/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.354052 backend.ai-client-24.3.0rc3/ai/backend/client/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.358052 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/quota_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/server_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20889 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.358052 backend.ai-client-24.3.0rc3/ai/backend/client/cli/session/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/session/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30037 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/session/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49861 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/session/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/session/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35705 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/cli/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13291 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.366052 backend.ai-client-24.3.0rc3/ai/backend/client/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/bgtask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/keypair_resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/quota_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/server_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12337 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52303 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27656 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/func/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/load_balancing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.366052 backend.ai-client-24.3.0rc3/ai/backend/client/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/output/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/output/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/output/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/output/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/output/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    29791 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16998 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/ai/backend/client/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:38.366052 backend.ai-client-24.3.0rc3/backend.ai_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-04-05 02:25:38.000000 backend.ai-client-24.3.0rc3/backend.ai_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-05 02:25:38.000000 backend.ai-client-24.3.0rc3/backend.ai_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:38.000000 backend.ai-client-24.3.0rc3/backend.ai_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 02:25:38.000000 backend.ai-client-24.3.0rc3/backend.ai_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:38.000000 backend.ai-client-24.3.0rc3/backend.ai_client.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:38.000000 backend.ai-client-24.3.0rc3/backend.ai_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-05 02:25:38.000000 backend.ai-client-24.3.0rc3/backend.ai_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 02:25:38.000000 backend.ai-client-24.3.0rc3/backend.ai_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:25:38.370052 backend.ai-client-24.3.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-04-05 02:25:37.000000 backend.ai-client-24.3.0rc3/setup.py
```

### Comparing `backend.ai-client-24.3.0rc2/PKG-INFO` & `backend.ai-client-24.3.0rc3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-client
-Version: 24.3.0rc2
+Version: 24.3.0rc3
 Summary: Backend.AI Client SDK
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,18 +12,42 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/x-rst
+Requires-Dist: aiohttp~=3.9.1
+Requires-Dist: aiotusclient~=0.1.4
+Requires-Dist: appdirs~=1.4.4
+Requires-Dist: async_timeout~=4.0
+Requires-Dist: attrs>=20.3
+Requires-Dist: backend.ai-cli==24.03.0rc3
+Requires-Dist: backend.ai-common==24.03.0rc3
+Requires-Dist: backend.ai-plugin==24.03.0rc3
+Requires-Dist: click~=8.1.7
+Requires-Dist: faker~=13.12.0
+Requires-Dist: humanize>=3.1.0
+Requires-Dist: inquirer~=2.9.2
+Requires-Dist: janus~=1.0.0
+Requires-Dist: multidict>=6.0
+Requires-Dist: python-dateutil>=2.8
+Requires-Dist: python-dotenv~=0.20.0
+Requires-Dist: rich~=13.6
+Requires-Dist: tabulate~=0.8.9
+Requires-Dist: tenacity>=8.0
+Requires-Dist: tqdm>=4.61
+Requires-Dist: treelib==1.6.1
+Requires-Dist: types-python-dateutil
+Requires-Dist: types-tabulate
+Requires-Dist: yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2
 
 Backend.AI Client
 =================
 
 .. image:: https://badge.fury.io/py/backend.ai-client.svg
    :target: https://badge.fury.io/py/backend.ai-client
    :alt: PyPI version
```

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/auth.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/__init__.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from . import admin  # noqa  # type: ignore
 from . import config  # noqa  # type: ignore
 from . import dotfile  # noqa  # type: ignore
 from . import extensions  # noqa  # type: ignore
+from . import image  # noqa  # type: ignore
 from . import model  # noqa  # type: ignore
 from . import server_log  # noqa  # type: ignore
 from . import service  # noqa  # type: ignore
 from . import session  # noqa  # type: ignore
 from . import session_template  # noqa  # type: ignore
 from . import vfolder  # noqa  # type: ignore
 from . import app, logs, proxy  # noqa  # type: ignore
```

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/acl.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/agent.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/domain.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/etcd.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/group.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/image.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/keypair.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/license.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/license.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/manager.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/quota_scope.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/quota_scope.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/resource.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/resource_policy.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/scaling_group.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/session.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/storage.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/user.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/admin/vfolder.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/admin/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/announcement.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/announcement.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/app.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/app.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/config.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/dotfile.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/extensions.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/extensions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/logs.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/main.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/main.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/model.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/pagination.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/pagination.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/pretty.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/pretty.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/proxy.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/proxy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/server_log.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/server_log.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/service.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/session/args.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/session/args.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/session/execute.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/session/execute.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/session/lifecycle.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/session/lifecycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,23 @@
 from ...compat import asyncio_run
 from ...exceptions import BackendAPIError
 from ...func.session import ComputeSession
 from ...output.fields import session_fields
 from ...output.types import FieldSpec
 from ...session import AsyncSession, Session
 from .. import events
-from ..pretty import print_done, print_error, print_fail, print_info, print_wait, print_warn
+from ..pretty import (
+    ProgressViewer,
+    print_done,
+    print_error,
+    print_fail,
+    print_info,
+    print_wait,
+    print_warn,
+)
 from .args import click_start_option
 from .execute import (
     format_stats,
     prepare_env_arg,
     prepare_mount_arg,
     prepare_resource_arg,
 )
@@ -837,14 +845,72 @@
             print_info(f"Request to commit Session(name or id: {session_id})")
         except Exception as e:
             print_error(e)
             sys.exit(ExitCode.FAILURE)
 
 
 @session.command()
+@click.argument("session_id", metavar="SESSID_OR_NAME")
+@click.argument("image_name", metavar="IMAGENAME")
+def convert_to_image(session_id, image_name):
+    """
+    Commits running session to new image and then uploads to designated container registry.
+    Requires Backend.AI server set up for per-user image commit feature (24.03).
+
+    \b
+    SESSID_OR_NAME: Session ID or its alias given when creating the session.
+    IMAGENAME: New image name.
+    """
+
+    with Session() as session:
+        try:
+            _sess = session.ComputeSession(session_id)
+            result = _sess.export_to_image(image_name)
+            print_info(f"Request to commit Session(name or id: {session_id})")
+        except Exception as e:
+            print_error(e)
+            sys.exit(ExitCode.FAILURE)
+
+    async def export_tracker(bgtask_id):
+        async with AsyncSession() as session:
+            try:
+                bgtask = session.BackgroundTask(bgtask_id)
+                completion_msg_func = lambda: print_done("Session export process completed.")
+                async with (
+                    bgtask.listen_events() as response,
+                    ProgressViewer("Starting the session...") as viewer,
+                ):
+                    async for ev in response:
+                        data = json.loads(ev.data)
+                        if ev.event == "bgtask_updated":
+                            if viewer.tqdm is None:
+                                pbar = await viewer.to_tqdm()
+
+                            pbar = viewer.tqdm
+                            pbar.total = data["total_progress"]
+                            pbar.update(data["current_progress"] - pbar.n)
+                            pbar.display(data["message"])
+                        elif ev.event == "bgtask_failed":
+                            error_msg = data["message"]
+                            completion_msg_func = lambda: print_fail(
+                                f"Error during the operation: {error_msg}",
+                            )
+                        elif ev.event == "bgtask_cancelled":
+                            completion_msg_func = lambda: print_warn(
+                                "The operation has been cancelled in the middle. "
+                                "(This may be due to server shutdown.)",
+                            )
+            finally:
+                completion_msg_func()
+                sys.exit()
+
+    asyncio_run(export_tracker(result["task_id"]))
+
+
+@session.command()
 @click.argument("session_id", metavar="SESSID")
 def abuse_history(session_id):
     """
     Get abusing reports of session's sibling kernels.
 
     \b
     SESSID: Session ID or its alias given when creating the session.
```

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/session/ssh.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/session/ssh.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/session_template.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/cli/vfolder.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/cli/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/compat.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/compat.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             loop.close()
             asyncio.set_event_loop(None)
 
 
 if hasattr(asyncio, "run"):  # Python 3.7+
     asyncio_run = asyncio.run
 else:
-    asyncio_run = _asyncio_run
+    asyncio_run = _asyncio_run  # type: ignore[assignment]
 
 
 def asyncio_run_forever(server_context, *, debug=False):
     """
     A proposed-but-not-implemented asyncio.run_forever() API based on
     @vxgmichel's idea.
     See discussions on https://github.com/python/asyncio/pull/465
```

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/config.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/exceptions.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/acl.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/admin.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/agent.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/auth.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/base.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/bgtask.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/bgtask.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/domain.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/dotfile.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/etcd.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/group.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/image.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/image.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,24 +33,44 @@
         cls,
         operation: bool = False,
         fields: Sequence[FieldSpec] = _default_list_fields_admin,
     ) -> Sequence[dict]:
         """
         Fetches the list of registered images in this cluster.
         """
-        q = "query($is_operation: Boolean) {  images(is_operation: $is_operation) {    $fields  }}"
+        q = (
+            "query($is_operation: Boolean) {"
+            "  images(is_operation: $is_operation) {"
+            "    $fields"
+            "  }"
+            "}"
+        )
         q = q.replace("$fields", " ".join(f.field_ref for f in fields))
         variables = {
             "is_operation": operation,
         }
         data = await api_session.get().Admin._query(q, variables)
         return data["images"]
 
     @api_function
     @classmethod
+    async def list_customized(
+        cls,
+        fields: Sequence[FieldSpec] = _default_list_fields_admin,
+    ) -> Sequence[dict]:
+        """
+        Fetches the list of customized images in this cluster.
+        """
+        q = "query {" "  customized_images {" "    $fields" "  }" "}"
+        q = q.replace("$fields", " ".join(f.field_ref for f in fields))
+        data = await api_session.get().Admin._query(q, {})
+        return data["customized_images"]
+
+    @api_function
+    @classmethod
     async def rescan_images(cls, registry: str):
         q = (
             "mutation($registry: String) {"
             "  rescan_images(registry:$registry) {"
             "   ok msg task_id"
             "  }"
             "}"
@@ -59,14 +79,47 @@
             "registry": registry,
         }
         data = await api_session.get().Admin._query(q, variables)
         return data["rescan_images"]
 
     @api_function
     @classmethod
+    async def forget_image_by_id(cls, image_id: str):
+        q = (
+            "mutation($image_id: String!) {"
+            "  forget_image_by_id(image_id: $image_id) {"
+            "   ok msg"
+            "  }"
+            "}"
+        )
+        variables = {
+            "image_id": image_id,
+        }
+        data = await api_session.get().Admin._query(q, variables)
+        return data["forget_image_by_id"]
+
+    @api_function
+    @classmethod
+    async def forget_image(cls, reference: str, architecture: str):
+        q = (
+            "mutation($reference: String!, $architecture: String!) {"
+            "  forget_image(reference: $reference, architecture: $architecture) {"
+            "   ok msg"
+            "  }"
+            "}"
+        )
+        variables = {
+            "reference": reference,
+            "architecture": architecture,
+        }
+        data = await api_session.get().Admin._query(q, variables)
+        return data["forget_image"]
+
+    @api_function
+    @classmethod
     async def alias_image(
         cls,
         alias: str,
         target: str,
         arch: Optional[str] = None,
     ) -> dict:
         q = (
```

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/keypair.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/keypair_resource_policy.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/keypair_resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/manager.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/model.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/quota_scope.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/quota_scope.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/resource.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/scaling_group.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/server_log.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/server_log.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/service.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/session.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -603,14 +603,32 @@
             f"/{prefix}/{self.name}/commit",
             params=params,
         )
         async with rqst.fetch() as resp:
             return await resp.json()
 
     @api_function
+    async def export_to_image(self, new_image_name: str):
+        """
+        Commits running session to new image and then uploads to designated container registry.
+        Requires Backend.AI server set up for per-user image commit feature (24.03).
+        """
+        params = {"image_name": new_image_name}
+        if self.owner_access_key:
+            params["owner_access_key"] = self.owner_access_key
+        prefix = get_naming(api_session.get().api_version, "path")
+        rqst = Request(
+            "POST",
+            f"/{prefix}/{self.name}/imagify",
+            params=params,
+        )
+        async with rqst.fetch() as resp:
+            return await resp.json()
+
+    @api_function
     async def interrupt(self):
         """
         Tries to interrupt the current ongoing code execution.
         This may fail without any explicit errors depending on the code being
         executed.
         """
         params = {}
```

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/session_template.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/storage.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/system.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/system.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/user.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/func/vfolder.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/func/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/load_balancing.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/load_balancing.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/output/__init__.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/output/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/output/console.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/output/console.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/output/fields.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/output/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from .formatters import (
     AgentStatFormatter,
     ContainerListFormatter,
+    CustomizedImageNameOutputFormatter,
     DependencyListFormatter,
     GroupListFormatter,
     InlineRoutingFormatter,
     KernelStatFormatter,
     SubFieldOutputFormatter,
     mibytes_output_formatter,
     nested_dict_formatter,
@@ -83,21 +84,29 @@
     FieldSpec("total_resource_slots", formatter=resource_slot_formatter),
     FieldSpec("allowed_vfolder_hosts"),
     FieldSpec("integration_id"),
 ])
 
 
 image_fields = FieldSet([
+    FieldSpec("id"),
     FieldSpec("name"),
     FieldSpec("registry"),
     FieldSpec("architecture"),
     FieldSpec("tag"),
     FieldSpec("digest"),
     FieldSpec("size_bytes", formatter=sizebytes_output_formatter),
     FieldSpec("aliases"),
+    FieldSpec("labels { key value }", "labels"),
+    FieldSpec(
+        "labels { key value }",
+        "Customized Image Name",
+        alt_name="customized_image_name",
+        formatter=CustomizedImageNameOutputFormatter(),
+    ),
 ])
 
 
 keypair_fields = FieldSet([
     FieldSpec("user_id", "Email"),
     FieldSpec(
         "user_info { full_name }",
```

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/output/formatters.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/output/formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,29 @@
     def format_console(self, value: Any, field: FieldSpec) -> str:
         return super().format_console(value[self._subfield_name], field)
 
     def format_json(self, value: Any, field: FieldSpec) -> Any:
         return super().format_json(value[self._subfield_name], field)
 
 
+class CustomizedImageNameOutputFormatter(OutputFormatter):
+    def _get_name(self, labels: Any) -> str:
+        customized_name = [
+            label["value"] for label in labels if label["key"] == "ai.backend.customized-image.name"
+        ]
+        assert len(customized_name) == 1
+        return customized_name[0]
+
+    def format_console(self, value: Any, field: FieldSpec) -> str:
+        return super().format_console(self._get_name(value), field)
+
+    def format_json(self, value: Any, field: FieldSpec) -> Any:
+        return super().format_json(self._get_name(value), field)
+
+
 class ResourceSlotFormatter(OutputFormatter):
     def format_console(self, value: Any, field: FieldSpec) -> str:
         value = json.loads(value)
         if mem := value.get("mem"):
             value["mem"] = humanize.naturalsize(mem, binary=True, gnu=True)
 
         return ", ".join(f"{k}:{v}" for k, v in value.items())
```

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/output/json.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/output/json.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/output/types.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/output/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/pagination.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/pagination.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/request.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/request.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/session.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/types.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/utils.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/ai/backend/client/versioning.py` & `backend.ai-client-24.3.0rc3/ai/backend/client/versioning.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/backend.ai_client.egg-info/PKG-INFO` & `backend.ai-client-24.3.0rc3/backend.ai_client.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-client
-Version: 24.3.0rc2
+Version: 24.3.0rc3
 Summary: Backend.AI Client SDK
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,18 +12,42 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/x-rst
+Requires-Dist: aiohttp~=3.9.1
+Requires-Dist: aiotusclient~=0.1.4
+Requires-Dist: appdirs~=1.4.4
+Requires-Dist: async_timeout~=4.0
+Requires-Dist: attrs>=20.3
+Requires-Dist: backend.ai-cli==24.03.0rc3
+Requires-Dist: backend.ai-common==24.03.0rc3
+Requires-Dist: backend.ai-plugin==24.03.0rc3
+Requires-Dist: click~=8.1.7
+Requires-Dist: faker~=13.12.0
+Requires-Dist: humanize>=3.1.0
+Requires-Dist: inquirer~=2.9.2
+Requires-Dist: janus~=1.0.0
+Requires-Dist: multidict>=6.0
+Requires-Dist: python-dateutil>=2.8
+Requires-Dist: python-dotenv~=0.20.0
+Requires-Dist: rich~=13.6
+Requires-Dist: tabulate~=0.8.9
+Requires-Dist: tenacity>=8.0
+Requires-Dist: tqdm>=4.61
+Requires-Dist: treelib==1.6.1
+Requires-Dist: types-python-dateutil
+Requires-Dist: types-tabulate
+Requires-Dist: yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2
 
 Backend.AI Client
 =================
 
 .. image:: https://badge.fury.io/py/backend.ai-client.svg
    :target: https://badge.fury.io/py/backend.ai-client
    :alt: PyPI version
```

### Comparing `backend.ai-client-24.3.0rc2/backend.ai_client.egg-info/SOURCES.txt` & `backend.ai-client-24.3.0rc3/backend.ai_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ai/backend/client/cli/__init__.py
 ai/backend/client/cli/announcement.py
 ai/backend/client/cli/app.py
 ai/backend/client/cli/config.py
 ai/backend/client/cli/dotfile.py
 ai/backend/client/cli/events.py
 ai/backend/client/cli/extensions.py
+ai/backend/client/cli/image.py
 ai/backend/client/cli/logs.py
 ai/backend/client/cli/main.py
 ai/backend/client/cli/model.py
 ai/backend/client/cli/pagination.py
 ai/backend/client/cli/pretty.py
 ai/backend/client/cli/proxy.py
 ai/backend/client/cli/server_log.py
```

### Comparing `backend.ai-client-24.3.0rc2/backend_shim.py` & `backend.ai-client-24.3.0rc3/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc2/setup.py` & `backend.ai-client-24.3.0rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,34 +12,34 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
         'Development Status :: 4 - Beta',
-        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: MIT License',
     ],
     'description': 'Backend.AI Client SDK',
     'entry_points': {
         'backendai_cli_v10': [
             '_ = ai.backend.client.cli.main:main',
         ],
     },
     'install_requires': (
         'aiohttp~=3.9.1',
         'aiotusclient~=0.1.4',
         'appdirs~=1.4.4',
         'async_timeout~=4.0',
         'attrs>=20.3',
-        """backend.ai-cli==24.03.0rc2
+        """backend.ai-cli==24.03.0rc3
 """,
-        """backend.ai-common==24.03.0rc2
+        """backend.ai-common==24.03.0rc3
 """,
-        """backend.ai-plugin==24.03.0rc2
+        """backend.ai-plugin==24.03.0rc3
 """,
         'click~=8.1.7',
         'faker~=13.12.0',
         'humanize>=3.1.0',
         'inquirer~=2.9.2',
         'janus~=1.0.0',
         'multidict>=6.0',
@@ -281,13 +281,13 @@
         'ai.backend.client.func',
         'ai.backend.client.output',
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
-    'python_requires': '>=3.11,<3.12',
+    'python_requires': '>=3.12,<3.13',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """24.03.0rc2
+    'version': """24.03.0rc3
 """,
     'zip_safe': False,
 })
```

