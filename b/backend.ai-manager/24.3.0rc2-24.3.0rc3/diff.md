# Comparing `tmp/backend.ai-manager-24.3.0rc2.tar.gz` & `tmp/backend.ai-manager-24.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-manager-24.3.0rc2.tar", last modified: Sun Mar 31 14:09:10 2024, max compression
+gzip compressed data, was "backend.ai-manager-24.3.0rc3.tar", last modified: Fri Apr  5 02:25:36 2024, max compression
```

## Comparing `backend.ai-manager-24.3.0rc2.tar` & `backend.ai-manager-24.3.0rc3.tar`

### file list

```diff
@@ -1,292 +1,293 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.379435 backend.ai-manager-24.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-03-31 14:09:10.375435 backend.ai-manager-24.3.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.315434 backend.ai-manager-24.3.0rc2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.315434 backend.ai-manager-24.3.0rc2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.319434 backend.ai-manager-24.3.0rc2/ai/backend/manager/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/agent_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.327434 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    41681 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/domainconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11715 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/groupconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (127)    37072 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    43070 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    80926 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/session_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    32952 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/userconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   133919 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/api/wsproxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.327434 backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/dbschema.py
--rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/image_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)    34463 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.327434 backend.ai-manager-24.3.0rc2/ai/backend/manager/container_registry/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/container_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16294 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/container_registry/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/container_registry/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    18946 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/container_registry/harbor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/container_registry/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/idle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.335434 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    22657 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.335434 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.363435 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/02535458c0b3_add_model_service_token_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/308bcecec5c2_add_groups_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/3f47af213b05_add_max_pending_session_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/41f332243bf9_add_missing_vfolder_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/4871d46ba31b_add_sudo_session_enabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/4b0128c49210_remove_size_limit_for_model_service_.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/589c764a18f1_change_endpoint_to_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/5ba7fde56ddb_add_vfolder_purge_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/69c059996cbd_add_agent_ids_col_to_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/75ea2b136830_add_user_resource_policies_max_session_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/7ff52ff68bfc_detail_vfolder_deletion_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/85615e005fa3_kernel_requested_slots_to_not_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/8b2ec7e3d22a_remove_unique_constraint_of_endpoint_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/8c74e7df26f8_make_routings_contain_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/97d8c7aa5e96_add_agent_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/a083c6c962e5_add_foreign_key_constraints_to_columns_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/a5319bfc7d7c_add_unique_constraints_to_association_.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/ae7d4cd92aa7_add_endpoint_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
--rw-r--r--   0 runner    (1001) docker     (127)    29365 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/b86b341fd9c9_update_resource_policy_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/c5ed277b7f7b_change_main_access_key_ondelete_to_set_.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/caf54fcc17ab_add_id_columns_to_association_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d04592473df7_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d3f8c74bf148_user_main_keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d643752544de_.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/e812d42bc34f_remove_unique_constraint_of_endpoints_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/eb9441fcf90a_add_images_col_to_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
--rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
--rw-r--r--   0 runner    (1001) docker     (127)    50166 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    33902 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/error_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)    66039 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/gql_relay.py
--rw-r--r--   0 runner    (1001) docker     (127)    32192 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    34812 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    52477 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    24284 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.363435 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/minilang/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/minilang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/minilang/ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/minilang/queryfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)    28498 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/resource_preset.py
--rw-r--r--   0 runner    (1001) docker     (127)    24189 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/resource_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)    24702 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    57200 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/session_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    56317 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    80293 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/models/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/pglock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.363435 backend.ai-manager-24.3.0rc2/ai/backend/manager/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/plugin/error_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/plugin/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/plugin/webapp.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   170343 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.363435 backend.ai-manager-24.3.0rc2/ai/backend/manager/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72808 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/scheduler/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/scheduler/drf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/scheduler/fifo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/scheduler/mof.py
--rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/scheduler/predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)    14044 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/scheduler/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    36027 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.375435 backend.ai-manager-24.3.0rc2/ai/backend/manager/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/vendor/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1851 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/vendor/bai-icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)   413294 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/vendor/graphiql.min.css
--r-xr-xr-x   0 runner    (1001) docker     (127)  3122938 2024-03-31 14:09:00.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/vendor/graphiql.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   131882 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/vendor/react-dom.production.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/vendor/react.production.min.js
--r-xr-xr-x   0 runner    (1001) docker     (127)   870146 2024-03-31 14:09:00.000000 backend.ai-manager-24.3.0rc2/ai/backend/manager/vendor/spec-viewer.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:09:10.375435 backend.ai-manager-24.3.0rc2/backend.ai_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-03-31 14:09:10.000000 backend.ai-manager-24.3.0rc2/backend.ai_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17492 2024-03-31 14:09:10.000000 backend.ai-manager-24.3.0rc2/backend.ai_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:10.000000 backend.ai-manager-24.3.0rc2/backend.ai_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-31 14:09:10.000000 backend.ai-manager-24.3.0rc2/backend.ai_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:10.000000 backend.ai-manager-24.3.0rc2/backend.ai_manager.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:09:09.000000 backend.ai-manager-24.3.0rc2/backend.ai_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-31 14:09:10.000000 backend.ai-manager-24.3.0rc2/backend.ai_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-31 14:09:10.000000 backend.ai-manager-24.3.0rc2/backend.ai_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 14:09:10.379435 backend.ai-manager-24.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-03-31 14:09:08.000000 backend.ai-manager-24.3.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.798038 backend.ai-manager-24.3.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-04-05 02:25:36.798038 backend.ai-manager-24.3.0rc3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.722037 backend.ai-manager-24.3.0rc3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.722037 backend.ai-manager-24.3.0rc3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.730037 backend.ai-manager-24.3.0rc3/ai/backend/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/agent_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.738037 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41681 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/domainconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11715 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/groupconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37072 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43070 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90344 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32952 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/userconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   133871 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/api/wsproxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.738037 backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/dbschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/image_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34463 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.742037 backend.ai-manager-24.3.0rc3/ai/backend/manager/container_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/container_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16474 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/container_registry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/container_registry/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19719 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/container_registry/harbor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/container_registry/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/idle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.746037 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22657 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.746037 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.782037 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/02535458c0b3_add_model_service_token_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/308bcecec5c2_add_groups_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/3f47af213b05_add_max_pending_session_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/41f332243bf9_add_missing_vfolder_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/4871d46ba31b_add_sudo_session_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/4b0128c49210_remove_size_limit_for_model_service_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/589c764a18f1_change_endpoint_to_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/5ba7fde56ddb_add_vfolder_purge_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/69c059996cbd_add_agent_ids_col_to_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/75ea2b136830_add_user_resource_policies_max_session_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/7ff52ff68bfc_detail_vfolder_deletion_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/85615e005fa3_kernel_requested_slots_to_not_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/857b763b8618_add_groups_per_user_image_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/8b2ec7e3d22a_remove_unique_constraint_of_endpoint_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/8c74e7df26f8_make_routings_contain_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/97d8c7aa5e96_add_agent_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/a083c6c962e5_add_foreign_key_constraints_to_columns_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/a5319bfc7d7c_add_unique_constraints_to_association_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/ae7d4cd92aa7_add_endpoint_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29365 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/b86b341fd9c9_update_resource_policy_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/c5ed277b7f7b_change_main_access_key_ondelete_to_set_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/caf54fcc17ab_add_id_columns_to_association_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d04592473df7_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d3f8c74bf148_user_main_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d643752544de_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/e812d42bc34f_remove_unique_constraint_of_endpoints_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/eb9441fcf90a_add_images_col_to_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50166 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33902 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/error_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67131 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/gql_relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33085 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37155 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52925 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24284 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.782037 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/minilang/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/minilang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/minilang/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/minilang/queryfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29395 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/resource_preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24189 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/resource_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24702 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57462 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56384 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80293 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/models/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/pglock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.782037 backend.ai-manager-24.3.0rc3/ai/backend/manager/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/plugin/error_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/plugin/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/plugin/webapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   172351 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.786038 backend.ai-manager-24.3.0rc3/ai/backend/manager/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72808 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/scheduler/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/scheduler/drf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/scheduler/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/scheduler/mof.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/scheduler/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14044 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/scheduler/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36027 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.794037 backend.ai-manager-24.3.0rc3/ai/backend/manager/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/vendor/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1851 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/vendor/bai-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   413294 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/vendor/graphiql.min.css
+-r-xr-xr-x   0 runner    (1001) docker     (127)  3122938 2024-04-05 02:25:21.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/vendor/graphiql.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   131882 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/vendor/react-dom.production.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/vendor/react.production.min.js
+-r-xr-xr-x   0 runner    (1001) docker     (127)   870146 2024-04-05 02:25:21.000000 backend.ai-manager-24.3.0rc3/ai/backend/manager/vendor/spec-viewer.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:25:36.798038 backend.ai-manager-24.3.0rc3/backend.ai_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-04-05 02:25:36.000000 backend.ai-manager-24.3.0rc3/backend.ai_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17585 2024-04-05 02:25:36.000000 backend.ai-manager-24.3.0rc3/backend.ai_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-manager-24.3.0rc3/backend.ai_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-05 02:25:36.000000 backend.ai-manager-24.3.0rc3/backend.ai_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-manager-24.3.0rc3/backend.ai_manager.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:25:36.000000 backend.ai-manager-24.3.0rc3/backend.ai_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-05 02:25:36.000000 backend.ai-manager-24.3.0rc3/backend.ai_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 02:25:36.000000 backend.ai-manager-24.3.0rc3/backend.ai_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:25:36.798038 backend.ai-manager-24.3.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-04-05 02:25:35.000000 backend.ai-manager-24.3.0rc3/setup.py
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/agent_cache.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/agent_cache.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/acl.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/admin.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/auth.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/cluster_template.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/cluster_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/context.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/domainconfig.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/domainconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/etcd.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/events.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/events.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/exceptions.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/groupconfig.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/groupconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/image.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/logs.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/manager.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/ratelimit.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/ratelimit.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/resource.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/scaling_group.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/service.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/session.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 REST-style session management APIs.
 """
 
 from __future__ import annotations
 
 import asyncio
 import base64
+import enum
 import functools
 import json
 import logging
 import re
 import secrets
 import uuid
 from datetime import datetime, timedelta
 from decimal import Decimal
 from pathlib import PurePosixPath
 from typing import (
     TYPE_CHECKING,
+    Annotated,
     Any,
     Dict,
     Iterable,
     List,
     Mapping,
     MutableMapping,
     Set,
@@ -37,80 +39,101 @@
 import attrs
 import multidict
 import sqlalchemy as sa
 import sqlalchemy.exc
 import trafaret as t
 from aiohttp import hdrs, web
 from dateutil.tz import tzutc
+from pydantic import BaseModel, Field
 from redis.asyncio import Redis
 from sqlalchemy.orm import noload, selectinload
 from sqlalchemy.sql.expression import null, true
 
+from ai.backend.common.bgtask import ProgressReporter
+from ai.backend.common.docker import ImageRef
+from ai.backend.manager.models.group import GroupRow
+from ai.backend.manager.models.image import rescan_images
+
 if TYPE_CHECKING:
     from sqlalchemy.ext.asyncio import AsyncConnection as SAConnection
     from sqlalchemy.ext.asyncio import AsyncSession as SASession
 
 from ai.backend.common import redis_helper
 from ai.backend.common import validators as tx
-from ai.backend.common.events import AgentTerminatedEvent
+from ai.backend.common.events import (
+    AgentTerminatedEvent,
+    BgtaskCancelledEvent,
+    BgtaskDoneEvent,
+    BgtaskFailedEvent,
+)
 from ai.backend.common.exception import UnknownImageReference
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.plugin.monitor import GAUGE
 from ai.backend.common.types import (
     AccessKey,
     AgentId,
     ClusterMode,
+    ImageRegistry,
     MountPermission,
     MountTypes,
     SessionTypes,
     VFolderID,
 )
 
 from ..config import DEFAULT_CHUNK_SIZE
 from ..defs import DEFAULT_IMAGE_ARCH, DEFAULT_ROLE
 from ..models import (
     AGENT_RESOURCE_OCCUPYING_KERNEL_STATUSES,
     DEAD_SESSION_STATUSES,
+    ImageRow,
     KernelLoadingStrategy,
     KernelRole,
+    SessionDependencyRow,
     SessionRow,
     SessionStatus,
     UserRole,
     groups,
     kernels,
     keypairs,
     query_accessible_vfolders,
     scaling_groups,
     session_templates,
     vfolders,
 )
-from ..models.session import SessionDependencyRow
 from ..types import UserScope
 from ..utils import query_userinfo as _query_userinfo
 from .auth import auth_required
 from .exceptions import (
     AppNotFound,
     BackendError,
     GenericForbidden,
     InsufficientPrivilege,
     InternalServerError,
     InvalidAPIParameters,
     ObjectNotFound,
+    QuotaExceeded,
     ServiceUnavailable,
     SessionAlreadyExists,
     SessionNotFound,
     StorageProxyError,
     TaskTemplateNotFound,
     TooManySessionsMatched,
     UnknownImageReferenceError,
 )
 from .manager import ALL_ALLOWED, READ_ALLOWED, server_status_required
 from .scaling_group import query_wsproxy_status
 from .types import CORSOptions, WebMiddleware
-from .utils import catch_unexpected, check_api_params, get_access_key_scopes, undefined
+from .utils import (
+    BaseResponseModel,
+    catch_unexpected,
+    check_api_params,
+    get_access_key_scopes,
+    pydantic_params_api_handler,
+    undefined,
+)
 
 if TYPE_CHECKING:
     from .context import RootContext
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 _json_loads = functools.partial(json.loads, parse_float=Decimal)
@@ -974,23 +997,232 @@
                 session_name,
                 owner_access_key,
                 kernel_loading_strategy=KernelLoadingStrategy.MAIN_KERNEL_ONLY,
             )
 
         resp: Mapping[str, Any] = await asyncio.shield(
             app_ctx.rpc_ptask_group.create_task(
-                root_ctx.registry.commit_session(session, filename=filename),
+                root_ctx.registry.commit_session_to_file(session, filename),
             ),
         )
     except BackendError:
         log.exception("COMMIT_SESSION: exception")
         raise
     return web.json_response(resp, status=201)
 
 
+class CustomizedImageVisibilityScope(str, enum.Enum):
+    USER = "user"
+    PROJECT = "project"
+
+
+class ConvertSessionToImageRequesteModel(BaseModel):
+    image_name: str = Field(
+        pattern=r"[a-zA-Z0-9\.\-_]+",
+        description="Name of the image to be created.",
+    )
+    login_session_token: Annotated[str | None, Field(default=None)]
+    image_visibility: CustomizedImageVisibilityScope = Field(
+        default=CustomizedImageVisibilityScope.USER,
+        description="Visibility scope of newly created image. currently only supports `USER` scope. Setting this to value other than `USER` will raise error.",
+    )
+
+
+class ConvertSessionToImageResponseModel(BaseResponseModel):
+    task_id: str
+
+
+@auth_required
+@server_status_required(ALL_ALLOWED)
+@pydantic_params_api_handler(ConvertSessionToImageRequesteModel)
+async def convert_session_to_image(
+    request: web.Request, params: ConvertSessionToImageRequesteModel
+) -> ConvertSessionToImageResponseModel:
+    root_ctx: RootContext = request.app["_root.context"]
+    background_task_manager = root_ctx.background_task_manager
+
+    session_name: str = request.match_info["session_name"]
+    requester_access_key, owner_access_key = await get_access_key_scopes(request)
+
+    myself = asyncio.current_task()
+    assert myself is not None
+
+    if params.image_visibility != CustomizedImageVisibilityScope.USER:
+        raise InvalidAPIParameters(f"Unsupported visibility scope {params.image_visibility}")
+
+    log.info(
+        "CONVERT_SESSION_TO_IMAGE (ak:{}/{}, s:{})",
+        requester_access_key,
+        owner_access_key,
+        session_name,
+    )
+    async with root_ctx.db.begin_readonly_session() as db_sess:
+        session = await SessionRow.get_session(
+            db_sess,
+            session_name,
+            owner_access_key,
+            kernel_loading_strategy=KernelLoadingStrategy.MAIN_KERNEL_ONLY,
+            eager_loading_op=[selectinload(SessionRow.group)],
+        )
+
+    project: GroupRow = session.group
+    if not project.container_registry:
+        raise InvalidAPIParameters(
+            "Project not ready to convert session image (registry configuration not populated)"
+        )
+
+    registry_hostname = project.container_registry["registry"]
+    registry_project = project.container_registry["project"]
+    registry_conf = await root_ctx.shared_config.get_container_registry(registry_hostname)
+    if not registry_conf:
+        raise InvalidAPIParameters(f"Registry {registry_hostname} not found")
+    if registry_project not in registry_conf.get("project", ""):
+        raise InvalidAPIParameters(f"Project {registry_project} not found")
+
+    base_image_ref = session.main_kernel.image_ref
+
+    image_owner_id = request["user"]["uuid"]
+
+    async def _commit_and_upload(reporter: ProgressReporter) -> None:
+        reporter.total_progress = 3
+        await reporter.update(message="Commit started")
+        try:
+            if "/" in base_image_ref.name:
+                new_name = base_image_ref.name.split("/", maxsplit=1)[1]
+            else:
+                # for cases where project name is not specified (e.g. redis, nginx, ...)
+                new_name = base_image_ref.name
+
+            # remove any existing customized related tag from base canonical
+            filtered_tag_set = [
+                x for x in base_image_ref.tag.split("-") if not x.startswith("customized_")
+            ]
+
+            new_canonical = (
+                f"{registry_hostname}/{registry_project}/{new_name}:{'-'.join(filtered_tag_set)}"
+            )
+
+            async with root_ctx.db.begin_readonly_session() as sess:
+                # check if user has passed its limit of customized image count
+                query = (
+                    sa.select([sa.func.count()])
+                    .select_from(ImageRow)
+                    .where(
+                        (
+                            ImageRow.labels["ai.backend.customized-image.owner"].as_string()
+                            == f"{params.image_visibility.value}:{image_owner_id}"
+                        )
+                    )
+                )
+                existing_image_count = await sess.scalar(query)
+
+                customized_image_count_limit = request["user"]["resource_policy"][
+                    "max_customized_image_count"
+                ]
+                if customized_image_count_limit <= existing_image_count:
+                    raise QuotaExceeded(
+                        extra_msg="You have reached your customized image count quota",
+                        extra_data={
+                            "limit": customized_image_count_limit,
+                            "current": existing_image_count,
+                        },
+                    )
+
+                # check if image with same name exists and reuse ID it if is
+                query = sa.select(ImageRow).where(
+                    ImageRow.name.like(f"{new_canonical}%")
+                    & (
+                        ImageRow.labels["ai.backend.customized-image.owner"].as_string()
+                        == f"{params.image_visibility.value}:{image_owner_id}"
+                    )
+                    & (
+                        ImageRow.labels["ai.backend.customized-image.name"].as_string()
+                        == params.image_name
+                    )
+                )
+                existing_row = await sess.scalar(query)
+
+                customized_image_id: str
+                if existing_row:
+                    customized_image_id = existing_row.labels["ai.backend.customized-image.id"]
+                    log.debug("reusing existing customized image ID {}", customized_image_id)
+                else:
+                    customized_image_id = str(uuid.uuid4())
+
+            new_canonical += f"-customized_{customized_image_id.replace('-', '')}"
+            new_image_ref: ImageRef = ImageRef(
+                new_canonical,
+                architecture=base_image_ref.architecture,
+                known_registries=["*"],
+                is_local=base_image_ref.is_local,
+            )
+
+            # commit image with new tag set
+            resp = await root_ctx.registry.commit_session(
+                session,
+                new_image_ref,
+                extra_labels={
+                    "ai.backend.customized-image.owner": f"{params.image_visibility.value}:{image_owner_id}",
+                    "ai.backend.customized-image.name": params.image_name,
+                    "ai.backend.customized-image.id": customized_image_id,
+                },
+            )
+            async for event, _ in background_task_manager.poll_bgtask_event(
+                uuid.UUID(resp["bgtask_id"])
+            ):
+                match event:
+                    case BgtaskDoneEvent():
+                        await reporter.update(increment=1, message="Committed image")
+                        break
+                    case BgtaskFailedEvent():
+                        raise BackendError(extra_msg=event.message)
+                    case BgtaskCancelledEvent():
+                        raise BackendError(extra_msg="Operation cancelled")
+
+            if not new_image_ref.is_local:
+                # push image to registry from local agent
+                image_registry = ImageRegistry(
+                    name=registry_hostname,
+                    url=str(registry_conf[""]),
+                    username=registry_conf.get("username"),
+                    password=registry_conf.get("password"),
+                )
+                resp = await root_ctx.registry.push_image(
+                    session.main_kernel.agent,
+                    new_image_ref,
+                    image_registry,
+                )
+                async for event, _ in background_task_manager.poll_bgtask_event(
+                    uuid.UUID(resp["bgtask_id"])
+                ):
+                    match event:
+                        case BgtaskDoneEvent():
+                            break
+                        case BgtaskFailedEvent():
+                            raise BackendError(extra_msg=event.message)
+                        case BgtaskCancelledEvent():
+                            raise BackendError(extra_msg="Operation cancelled")
+
+            await reporter.update(increment=1, message="Pushed image to registry")
+            # rescan updated image only
+            await rescan_images(
+                root_ctx.shared_config.etcd,
+                root_ctx.db,
+                new_image_ref.canonical,
+                local=new_image_ref.is_local,
+            )
+            await reporter.update(increment=1, message="Completed")
+        except BackendError:
+            log.exception("CONVERT_SESSION_TO_IMAGE: exception")
+            raise
+
+    task_id = await background_task_manager.start(_commit_and_upload)
+    return ConvertSessionToImageResponseModel(task_id=str(task_id))
+
+
 @catch_unexpected(log)
 async def check_agent_lost(root_ctx: RootContext, interval: float) -> None:
     try:
         now = datetime.now(tzutc())
         timeout = timedelta(seconds=root_ctx.local_config["manager"]["heartbeat-timeout"])
 
         async def _check_impl(r: Redis):
@@ -2050,11 +2282,12 @@
     cors.add(app.router.add_route("POST", "/{session_name}/shutdown-service", shutdown_service))
     cors.add(app.router.add_route("POST", "/{session_name}/upload", upload_files))
     cors.add(app.router.add_route("GET", "/{session_name}/download", download_files))
     cors.add(app.router.add_route("GET", "/{session_name}/download_single", download_single))
     cors.add(app.router.add_route("GET", "/{session_name}/files", list_files))
     cors.add(app.router.add_route("POST", "/{session_name}/start-service", start_service))
     cors.add(app.router.add_route("POST", "/{session_name}/commit", commit_session))
+    cors.add(app.router.add_route("POST", "/{session_name}/imagify", convert_session_to_image))
     cors.add(app.router.add_route("GET", "/{session_name}/commit", get_commit_status))
     cors.add(app.router.add_route("GET", "/{session_name}/abusing-report", get_abusing_report))
     cors.add(app.router.add_route("GET", "/{session_name}/dependency-graph", get_dependency_graph))
     return app, []
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/session_template.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/spec.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 """
 
 
 GRAPHIQL_HTML = """
 <html>
   <head>
     <title>Backend.AI GraphQL API Reference</title>
+	<meta charset="UTF-8">
     <link href="../static/vendor/graphiql.min.css" rel="stylesheet" />
   </head>
   <body style="margin: 0;">
     <div id="graphiql" style="height: 100vh;"></div>
 
     <script src="../static/vendor/react.production.min.js"
     ></script>
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/stream.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/stream.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/types.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/userconfig.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/userconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/utils.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,36 +210,38 @@
             set_handler_attr(wrapped, "request_examples", request_examples)
         return wrapped
 
     return wrap
 
 
 class BaseResponseModel(BaseModel):
-    status: Annotated[int, Field(strict=True, ge=100, lt=600)] = 200
+    status: Annotated[int, Field(strict=True, exclude=True, ge=100, lt=600)] = 200
 
 
 TParamModel = TypeVar("TParamModel", bound=BaseModel)
 TQueryModel = TypeVar("TQueryModel", bound=BaseModel)
-TResponseModel = TypeVar("TResponseModel", bound=BaseResponseModel)
+TResponseModel = TypeVar("TResponseModel", bound=BaseModel)
 
 TPydanticResponse: TypeAlias = TResponseModel | list
 THandlerFuncWithoutParam: TypeAlias = Callable[
     Concatenate[web.Request, P], Awaitable[TPydanticResponse | TAnyResponse]
 ]
 THandlerFuncWithParam: TypeAlias = Callable[
     Concatenate[web.Request, TParamModel, P], Awaitable[TPydanticResponse | TAnyResponse]
 ]
 
 
 def ensure_stream_response_type(
-    response: BaseResponseModel | list[TResponseModel] | web.StreamResponse,
+    response: BaseResponseModel | BaseModel | list[TResponseModel] | web.StreamResponse,
 ) -> web.StreamResponse:
     match response:
         case BaseResponseModel(status=status):
             return web.json_response(response.model_dump(mode="json"), status=status)
+        case BaseModel():
+            return web.json_response(response.model_dump(mode="json"))
         case list():
             return web.json_response(TypeAdapter(type(response)).dump_python(response, mode="json"))
         case web.StreamResponse():
             return response
         case _:
             raise RuntimeError(f"Unsupported response type ({type(response)})")
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/vfolder.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/vfolder.py`

 * *Files 0% similar despite different names*

```diff
@@ -2396,15 +2396,15 @@
     )
 
 
 @auth_required
 @pydantic_params_api_handler(DeleteFromTrashRequestModel)
 async def delete_from_trash_bin(
     request: web.Request, params: DeleteFromTrashRequestModel
-) -> SuccessResponseModel:
+) -> web.Response:
     """
     Delete `delete-pending` vfolders in storage proxy
     """
     root_ctx: RootContext = request.app["_root.context"]
     app_ctx: PrivateContext = request.app["folders.context"]
     folder_id = params.vfolder_id
     access_key = request["keypair"]["access_key"]
@@ -2451,28 +2451,28 @@
     # fs-level deletion may fail or take longer time
     await initiate_vfolder_deletion(
         root_ctx.db,
         [VFolderDeletionInfo(VFolderID.from_row(entry), folder_host)],
         root_ctx.storage_manager,
         app_ctx.storage_ptask_group,
     )
-    return SuccessResponseModel(status=204)
+    return web.Response(status=204)
 
 
 class PurgeRequestModel(BaseModel):
     vfolder_id: uuid.UUID = Field(
         validation_alias=AliasChoices("vfolder_id", "vfolderId", "id"),
         description="Target vfolder id to purge, permanently remove from DB",
     )
 
 
 @auth_required
 @server_status_required(ALL_ALLOWED)
 @pydantic_params_api_handler(PurgeRequestModel)
-async def purge(request: web.Request, params: PurgeRequestModel) -> SuccessResponseModel:
+async def purge(request: web.Request, params: PurgeRequestModel) -> web.Response:
     """
     Delete `delete-complete`d vfolder rows in DB
     """
     root_ctx: RootContext = request.app["_root.context"]
     folder_id = params.vfolder_id
     access_key = request["keypair"]["access_key"]
     domain_name = request["user"]["domain_name"]
@@ -2513,28 +2513,28 @@
         elif len(entries) == 0:
             raise InvalidAPIParameters("No such vfolder.")
         # query_accesible_vfolders returns list
         entry = entries[0]
         delete_stmt = sa.delete(vfolders).where(vfolders.c.id == entry["id"])
         await conn.execute(delete_stmt)
 
-    return SuccessResponseModel(status=204)
+    return web.Response(status=204)
 
 
 class RestoreRequestModel(BaseModel):
     vfolder_id: uuid.UUID = Field(
         validation_alias=AliasChoices("vfolder_id", "vfolderId", "id"),
         description="Target vfolder id to restore",
     )
 
 
 @auth_required
 @server_status_required(ALL_ALLOWED)
 @pydantic_params_api_handler(RestoreRequestModel)
-async def restore(request: web.Request, params: RestoreRequestModel) -> SuccessResponseModel:
+async def restore(request: web.Request, params: RestoreRequestModel) -> web.Response:
     """
     Recover vfolder from trash bin, by changing status.
     """
     root_ctx: RootContext = request.app["_root.context"]
     folder_id = params.vfolder_id
     access_key = request["keypair"]["access_key"]
     domain_name = request["user"]["domain_name"]
@@ -2581,15 +2581,15 @@
         # Folder owner OR user who have DELETE permission can restore folder.
         if not entry["is_owner"] and entry["permission"] != VFolderPermission.RW_DELETE:
             raise InvalidAPIParameters("Cannot restore the vfolder that is not owned by myself.")
 
     # fs-level mv may fail or take longer time
     # but let's complete the db transaction to reflect that it's deleted.
     await update_vfolder_status(root_ctx.db, (entry["id"],), VFolderOperationStatus.READY)
-    return SuccessResponseModel(status=204)
+    return web.Response(status=204)
 
 
 @auth_required
 @server_status_required(ALL_ALLOWED)
 @vfolder_permission_required(VFolderPermission.READ_ONLY)
 @check_api_params(
     t.Dict({
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/api/wsproxy.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/api/wsproxy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/__main__.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/agent.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/api.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/api.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/context.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/dbschema.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/dbschema.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/etcd.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/fixture.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/fixture.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/gql.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/gql.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/image.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/image_impl.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/image_impl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/cli/redis.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/cli/redis.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/config.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/container_registry/__init__.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/container_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/container_registry/base.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/container_registry/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         async with aiohttp.ClientSession(connector=connector) as sess:
             yield self.registry_url, sess
 
     async def rescan_single_registry(
         self,
         reporter: ProgressReporter | None = None,
     ) -> None:
+        log.info("rescan_single_registry()")
         all_updates_token = all_updates.set({})
         concurrency_sema.set(asyncio.Semaphore(self.max_concurrency_per_registry))
         progress_reporter.set(reporter)
         try:
             username = self.registry_info["username"]
             if username is not None:
                 self.credentials["username"] = username
@@ -147,14 +148,20 @@
                 ])
                 await session.flush()
 
     async def scan_single_ref(self, image_ref: str) -> None:
         all_updates_token = all_updates.set({})
         sema_token = concurrency_sema.set(asyncio.Semaphore(1))
         try:
+            username = self.registry_info["username"]
+            if username is not None:
+                self.credentials["username"] = username
+            password = self.registry_info["password"]
+            if password is not None:
+                self.credentials["password"] = password
             async with self.prepare_client_session() as (url, sess):
                 image, tag = ImageRef._parse_image_tag(image_ref)
                 rqst_args = await registry_login(
                     sess,
                     self.registry_url,
                     self.credentials,
                     f"repository:{image}:pull",
@@ -167,14 +174,15 @@
             all_updates.reset(all_updates_token)
 
     async def _scan_image(
         self,
         sess: aiohttp.ClientSession,
         image: str,
     ) -> None:
+        log.info("_scan_image()")
         rqst_args = await registry_login(
             sess,
             self.registry_url,
             self.credentials,
             f"repository:{image}:pull",
         )
         rqst_args["headers"].update(**self.base_hdrs)
@@ -230,14 +238,15 @@
                         manifest_list = [
                             item
                             for item in resp_json["manifests"]
                             if "annotations" not in item  # skip attestation manifests
                         ]
                         request_type = self.MEDIA_TYPE_OCI_MANIFEST
                     case _:
+                        log.warn("Unknown content type: {}", content_type)
                         raise RuntimeError(
                             "The registry does not support the standard way of "
                             "listing multiarch images."
                         )
             rqst_args["headers"]["Accept"] = request_type
             for manifest in manifest_list:
                 platform_arg = (
@@ -255,36 +264,26 @@
                 size_bytes = sum(layer["size"] for layer in data["layers"]) + data["config"]["size"]
                 async with sess.get(
                     self.registry_url / f"v2/{image}/blobs/{config_digest}", **rqst_args
                 ) as resp:
                     resp.raise_for_status()
                     data = json.loads(await resp.read())
                 labels = {}
-                if "container_config" in data:
-                    raw_labels = data["container_config"].get("Labels")
-                    if raw_labels:
-                        labels.update(raw_labels)
-                    else:
-                        log.warning(
-                            "label not found on image {}:{}/{}",
-                            image,
-                            tag,
-                            architecture,
-                        )
-                else:
-                    raw_labels = data["config"].get("Labels")
-                    if raw_labels:
-                        labels.update(raw_labels)
-                    else:
-                        log.warning(
-                            "label not found on image {}:{}/{}",
-                            image,
-                            tag,
-                            architecture,
-                        )
+                # we should favor `config` instead of `container_config` since `config` can contain additional datas
+                # set when commiting image via `--change` flag
+                if _config_labels := data.get("config", {}).get("Labels"):
+                    labels = _config_labels
+                elif _container_config_labels := data.get("container_config", {}).get("Labels"):
+                    labels = _container_config_labels
+
+                if not labels:
+                    log.warning(
+                        "Labels section not found on image {}:{}/{}", image, tag, architecture
+                    )
+
                 manifests[architecture] = {
                     "size": size_bytes,
                     "labels": labels,
                     "digest": config_digest,
                 }
             await self._read_manifest(image, tag, manifests)
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/container_registry/docker.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/container_registry/docker.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/container_registry/harbor.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/container_registry/harbor.py`

 * *Files 13% similar despite different names*

```diff
@@ -98,26 +98,26 @@
                 async with sess.get(
                     self.registry_url / f"v2/{image}/blobs/{config_digest}", **rqst_args
                 ) as resp:
                     resp.raise_for_status()
                     data = json.loads(await resp.read())
                     architecture = arch_name_aliases.get(data["architecture"], data["architecture"])
                     labels = {}
-                    if "container_config" in data:
-                        raw_labels = data["container_config"].get("Labels")
-                        if raw_labels:
-                            labels.update(raw_labels)
-                        else:
-                            log.warn("label not found on image {}:{}/{}", image, tag, architecture)
-                    else:
-                        raw_labels = data["config"].get("Labels")
-                        if raw_labels:
-                            labels.update(raw_labels)
-                        else:
-                            log.warn("label not found on image {}:{}/{}", image, tag, architecture)
+
+                    # we should favor `config` instead of `container_config` since `config` can contain additional datas
+                    # set when commiting image via `--change` flag
+                    if _config_labels := data.get("config", {}).get("Labels"):
+                        labels = _config_labels
+                    elif _container_config_labels := data.get("container_config", {}).get("Labels"):
+                        labels = _container_config_labels
+
+                    if not labels:
+                        log.warning(
+                            "Labels section not found on image {}:{}/{}", image, tag, architecture
+                        )
                     manifest = {
                         architecture: {
                             "size": size_bytes,
                             "labels": labels,
                             "digest": config_digest,
                         },
                     }
@@ -223,14 +223,50 @@
                     next_page_link = resp.links.get("next")
                     if next_page_link:
                         next_page_url = cast(yarl.URL, next_page_link["url"])
                         artifact_url = self.registry_url.with_path(next_page_url.path).with_query(
                             next_page_url.query
                         )
 
+    async def _scan_tag(
+        self,
+        sess: aiohttp.ClientSession,
+        rqst_args: dict[str, Any],
+        image: str,
+        tag: str,
+    ) -> None:
+        project, _, repository = image.partition("/")
+        project, repository, tag = [
+            urllib.parse.urlencode({"": x})[1:] for x in [project, repository, tag]
+        ]
+        api_url = self.registry_url / "api" / "v2.0"
+        rqst_args["headers"] = {}
+        async with sess.get(
+            api_url / "projects" / project / "repositories" / repository / "artifacts" / tag,
+            **rqst_args,
+        ) as resp:
+            if resp.status == 404:
+                # ignore missing tags
+                # (may occur after deleting an image from the docker hub)
+                return
+            resp.raise_for_status()
+            resp_json = await resp.json()
+            async with aiotools.TaskGroup() as tg:
+                match resp_json["manifest_media_type"]:
+                    case self.MEDIA_TYPE_OCI_INDEX:
+                        await self._process_oci_index(tg, sess, rqst_args, image, resp_json)
+                    case self.MEDIA_TYPE_DOCKER_MANIFEST_LIST:
+                        await self._process_docker_v2_multiplatform_image(
+                            tg, sess, rqst_args, image, resp_json
+                        )
+                    case self.MEDIA_TYPE_DOCKER_MANIFEST:
+                        await self._process_docker_v2_image(tg, sess, rqst_args, image, resp_json)
+                    case _ as media_type:
+                        raise RuntimeError(f"Unsupported artifact media-type: {media_type}")
+
     async def _process_oci_index(
         self,
         tg: aiotools.TaskGroup,
         sess: aiohttp.ClientSession,
         _rqst_args: Mapping[str, Any],
         image: str,
         image_info: Mapping[str, Any],
@@ -360,36 +396,22 @@
             )
             async with sess.get(
                 self.registry_url / f"v2/{image}/blobs/{config_digest}", **rqst_args
             ) as resp:
                 resp.raise_for_status()
                 data = json.loads(await resp.read())
             labels = {}
-            if "container_config" in data:
-                raw_labels = data["container_config"].get("Labels")
-                if raw_labels:
-                    labels.update(raw_labels)
-                else:
-                    log.warning(
-                        "label not found on image {}:{}/{}",
-                        image,
-                        tag,
-                        architecture,
-                    )
-            else:
-                raw_labels = data["config"].get("Labels")
-                if raw_labels:
-                    labels.update(raw_labels)
-                else:
-                    log.warning(
-                        "label not found on image {}:{}/{}",
-                        image,
-                        tag,
-                        architecture,
-                    )
+            if _config_labels := data.get("config", {}).get("Labels"):
+                labels = _config_labels
+            elif _container_config_labels := data.get("container_config", {}).get("Labels"):
+                labels = _container_config_labels
+
+            if not labels:
+                log.warning("Labels section not found on image {}:{}/{}", image, tag, architecture)
+
             manifests[architecture] = {
                 "size": size_bytes,
                 "labels": labels,
                 "digest": config_digest,
             }
             await self._read_manifest(image, tag, manifests)
 
@@ -422,35 +444,20 @@
                 size_bytes = sum(layer["size"] for layer in data["layers"]) + data["config"]["size"]
             async with sess.get(
                 self.registry_url / f"v2/{image}/blobs/{config_digest}", **rqst_args
             ) as resp:
                 resp.raise_for_status()
                 data = json.loads(await resp.read())
             labels = {}
-            if "container_config" in data:
-                raw_labels = data["container_config"].get("Labels")
-                if raw_labels:
-                    labels.update(raw_labels)
-                else:
-                    log.warning(
-                        "label not found on image {}:{}/{}",
-                        image,
-                        tag,
-                        architecture,
-                    )
-            else:
-                raw_labels = data["config"].get("Labels")
-                if raw_labels:
-                    labels.update(raw_labels)
-                else:
-                    log.warning(
-                        "label not found on image {}:{}/{}",
-                        image,
-                        tag,
-                        architecture,
-                    )
+            if _config_labels := data.get("config", {}).get("Labels"):
+                labels = _config_labels
+            elif _container_config_labels := data.get("container_config", {}).get("Labels"):
+                labels = _container_config_labels
+
+            if not labels:
+                log.warning("Labels section not found on image {}:{}/{}", image, tag, architecture)
             manifests[architecture] = {
                 "size": size_bytes,
                 "labels": labels,
                 "digest": config_digest,
             }
             await self._read_manifest(image, tag, manifests)
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/container_registry/local.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/container_registry/local.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/defs.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/defs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/exceptions.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/idle.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/idle.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/__init__.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/acl.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/agent.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/env.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/env.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/02535458c0b3_add_model_service_token_log.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/02535458c0b3_add_model_service_token_log.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/308bcecec5c2_add_groups_type.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/308bcecec5c2_add_groups_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/3f47af213b05_add_max_pending_session_count.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/3f47af213b05_add_max_pending_session_count.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/41f332243bf9_add_missing_vfolder_indexes.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/41f332243bf9_add_missing_vfolder_indexes.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/4871d46ba31b_add_sudo_session_enabled.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/4871d46ba31b_add_sudo_session_enabled.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/4b0128c49210_remove_size_limit_for_model_service_.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/4b0128c49210_remove_size_limit_for_model_service_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/589c764a18f1_change_endpoint_to_nullable.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/589c764a18f1_change_endpoint_to_nullable.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/5ba7fde56ddb_add_vfolder_purge_status.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/5ba7fde56ddb_add_vfolder_purge_status.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/69c059996cbd_add_agent_ids_col_to_session.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/69c059996cbd_add_agent_ids_col_to_session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/75ea2b136830_add_user_resource_policies_max_session_.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/75ea2b136830_add_user_resource_policies_max_session_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/7ff52ff68bfc_detail_vfolder_deletion_status.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/7ff52ff68bfc_detail_vfolder_deletion_status.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/85615e005fa3_kernel_requested_slots_to_not_nullable.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/85615e005fa3_kernel_requested_slots_to_not_nullable.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/8b2ec7e3d22a_remove_unique_constraint_of_endpoint_url.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/8b2ec7e3d22a_remove_unique_constraint_of_endpoint_url.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/8c74e7df26f8_make_routings_contain_error.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/8c74e7df26f8_make_routings_contain_error.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/a083c6c962e5_add_foreign_key_constraints_to_columns_.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/a083c6c962e5_add_foreign_key_constraints_to_columns_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/a5319bfc7d7c_add_unique_constraints_to_association_.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/a5319bfc7d7c_add_unique_constraints_to_association_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/b86b341fd9c9_update_resource_policy_tables.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/b86b341fd9c9_update_resource_policy_tables.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/c5ed277b7f7b_change_main_access_key_ondelete_to_set_.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/c5ed277b7f7b_change_main_access_key_ondelete_to_set_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/caf54fcc17ab_add_id_columns_to_association_tables.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/caf54fcc17ab_add_id_columns_to_association_tables.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d3f8c74bf148_user_main_keypair.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d3f8c74bf148_user_main_keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/eb9441fcf90a_add_images_col_to_session.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/eb9441fcf90a_add_images_col_to_session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/base.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/domain.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/dotfile.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/endpoint.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/error_logs.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/error_logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/etcd.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/gql.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/gql.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,17 @@
     PurgeGroup,
 )
 from .image import (
     AliasImage,
     ClearImages,
     DealiasImage,
     ForgetImage,
+    ForgetImageById,
     Image,
+    ImageLoadFilter,
     ModifyImage,
     PreloadImage,
     RescanImages,
     UnloadImage,
 )
 from .kernel import (
     ComputeContainer,
@@ -197,14 +199,15 @@
     delete_keypair = DeleteKeyPair.Field()
 
     # admin only
     rescan_images = RescanImages.Field()
     preload_image = PreloadImage.Field()
     unload_image = UnloadImage.Field()
     modify_image = ModifyImage.Field()
+    forget_image_by_id = ForgetImageById.Field(description="Added since 24.03.0")
     forget_image = ForgetImage.Field()
     alias_image = AliasImage.Field()
     dealias_image = DealiasImage.Field()
     clear_images = ClearImages.Field()
 
     # super-admin only
     create_keypair_resource_policy = CreateKeyPairResourcePolicy.Field()
@@ -349,14 +352,16 @@
 
     images = graphene.List(
         Image,
         is_installed=graphene.Boolean(),
         is_operation=graphene.Boolean(),
     )
 
+    customized_images = graphene.List(Image, description="Added since 24.03.0")
+
     user = graphene.Field(
         User,
         domain_name=graphene.String(),
         email=graphene.String(),
     )
 
     user_from_uuid = graphene.Field(
@@ -1013,34 +1018,59 @@
                 raise ImageNotFound
             item = items[0]
         else:
             raise InvalidAPIParameters("Unknown client role")
         return item
 
     @staticmethod
+    async def resolve_customized_images(
+        root: Any,
+        info: graphene.ResolveInfo,
+    ) -> Sequence[Image]:
+        ctx: GraphQueryContext = info.context
+        client_role = ctx.user["role"]
+        client_domain = ctx.user["domain_name"]
+        items = await Image.load_all(ctx, filters=set((ImageLoadFilter.CUSTOMIZED_ONLY,)))
+        if client_role == UserRole.SUPERADMIN:
+            pass
+        elif client_role in (UserRole.ADMIN, UserRole.USER):
+            items = await Image.filter_allowed(
+                info.context,
+                items,
+                client_domain,
+            )
+        else:
+            raise InvalidAPIParameters("Unknown client role")
+        return items
+
+    @staticmethod
     async def resolve_images(
         root: Any,
         info: graphene.ResolveInfo,
         *,
         is_installed=None,
         is_operation=False,
     ) -> Sequence[Image]:
         ctx: GraphQueryContext = info.context
         client_role = ctx.user["role"]
         client_domain = ctx.user["domain_name"]
-        items = await Image.load_all(ctx, is_installed=is_installed, is_operation=is_operation)
+        image_load_filters: set[ImageLoadFilter] = set()
+        if is_installed is not None:
+            image_load_filters.add(ImageLoadFilter.INSTALLED)
+        if is_operation is not None:
+            image_load_filters.add(ImageLoadFilter.EXCLUDE_OPERATIONAL)
+
+        items = await Image.load_all(ctx, filters=image_load_filters)
         if client_role == UserRole.SUPERADMIN:
             pass
         elif client_role in (UserRole.ADMIN, UserRole.USER):
             items = await Image.filter_allowed(
                 info.context,
                 items,
                 client_domain,
-                is_installed=is_installed,
-                is_operation=is_operation,
             )
         else:
             raise InvalidAPIParameters("Unknown client role")
         return items
 
     @staticmethod
     @scoped_query(autofill_user=True, user_key="email")
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/gql_relay.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/gql_relay.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/group.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     Union,
     overload,
 )
 
 import aiotools
 import graphene
 import sqlalchemy as sa
+import trafaret as t
 from graphene.types.datetime import DateTime as GQLDateTime
 from graphql import Undefined
 from sqlalchemy.engine.row import Row
 from sqlalchemy.ext.asyncio import AsyncConnection as SAConnection
 from sqlalchemy.orm import relationship
 
 from ai.backend.common import msgpack
@@ -37,14 +38,15 @@
     Base,
     EnumValueType,
     FilterExprArg,
     IDColumn,
     OrderExprArg,
     PaginatedConnectionField,
     ResourceSlotColumn,
+    StructuredJSONColumn,
     VFolderHostPermissionColumn,
     batch_multiresult,
     batch_result,
     generate_sql_info_for_gql_connection,
     mapper_registry,
     privileged_mutation,
     set_if_set,
@@ -107,14 +109,19 @@
         GUID,
         sa.ForeignKey("groups.id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     ),
     sa.UniqueConstraint("user_id", "group_id", name="uq_association_user_id_group_id"),
 )
 
+container_registry_iv = t.Dict({}) | t.Dict({
+    t.Key("registry"): t.String(),
+    t.Key("project"): t.String(),
+})
+
 
 class AssocGroupUserRow(Base):
     __table__ = association_groups_users
     user = relationship("UserRow", back_populates="groups")
     group = relationship("GroupRow", back_populates="users")
 
 
@@ -166,27 +173,34 @@
     ),
     sa.Column(
         "type",
         EnumValueType(ProjectType),
         nullable=False,
         default=ProjectType.GENERAL,
     ),
+    sa.Column(
+        "container_registry",
+        StructuredJSONColumn(container_registry_iv),
+        nullable=True,
+        default=None,
+    ),
     sa.UniqueConstraint("name", "domain_name", name="uq_groups_name_domain_name"),
 )
 
 
 class GroupRow(Base):
     __table__ = groups
     sessions = relationship("SessionRow", back_populates="group")
     domain = relationship("DomainRow", back_populates="groups")
     scaling_groups = relationship(
         "ScalingGroupRow", secondary="sgroups_for_groups", back_populates="groups"
     )
     users = relationship("AssocGroupUserRow", back_populates="group")
     resource_policy_row = relationship("ProjectResourcePolicyRow", back_populates="projects")
+    kernels = relationship("KernelRow", back_populates="group_row")
 
 
 def _build_group_query(cond: sa.sql.BinaryExpression, domain_name: str) -> sa.sql.Select:
     query = (
         sa.select([groups.c.id])
         .select_from(groups)
         .where(
@@ -259,14 +273,15 @@
     modified_at = GQLDateTime()
     domain_name = graphene.String()
     total_resource_slots = graphene.JSONString()
     allowed_vfolder_hosts = graphene.JSONString()
     integration_id = graphene.String()
     resource_policy = graphene.String()
     type = graphene.String(description="Added since 24.03.0.")
+    container_registry = graphene.JSONString(description="Added since 24.03.0.")
 
     scaling_groups = graphene.List(lambda: graphene.String)
 
     @classmethod
     def from_row(cls, graph_ctx: GraphQueryContext, row: Row) -> Optional[Group]:
         if row is None:
             return None
@@ -279,14 +294,15 @@
             modified_at=row["modified_at"],
             domain_name=row["domain_name"],
             total_resource_slots=row["total_resource_slots"].to_json(),
             allowed_vfolder_hosts=row["allowed_vfolder_hosts"].to_json(),
             integration_id=row["integration_id"],
             resource_policy=row["resource_policy"],
             type=row["type"].name,
+            container_registry=row["container_registry"],
         )
 
     async def resolve_scaling_groups(self, info: graphene.ResolveInfo) -> Sequence[ScalingGroup]:
         graph_ctx: GraphQueryContext = info.context
         loader = graph_ctx.dataloader_manager.get_loader(
             graph_ctx,
             "ScalingGroup.by_group",
@@ -417,27 +433,33 @@
     description = graphene.String(required=False, default_value="")
     is_active = graphene.Boolean(required=False, default_value=True)
     domain_name = graphene.String(required=True)
     total_resource_slots = graphene.JSONString(required=False, default_value={})
     allowed_vfolder_hosts = graphene.JSONString(required=False, default_value={})
     integration_id = graphene.String(required=False, default_value="")
     resource_policy = graphene.String(required=False, default_value="default")
+    container_registry = graphene.JSONString(
+        required=False, default_value={}, description="Added since 24.03.0"
+    )
 
 
 class ModifyGroupInput(graphene.InputObjectType):
     name = graphene.String(required=False)
     description = graphene.String(required=False)
     is_active = graphene.Boolean(required=False)
     domain_name = graphene.String(required=False)
     total_resource_slots = graphene.JSONString(required=False)
     user_update_mode = graphene.String(required=False)
     user_uuids = graphene.List(lambda: graphene.String, required=False)
     allowed_vfolder_hosts = graphene.JSONString(required=False)
     integration_id = graphene.String(required=False)
     resource_policy = graphene.String(required=False)
+    container_registry = graphene.JSONString(
+        required=False, default_value={}, description="Added since 24.03.0"
+    )
 
 
 class CreateGroup(graphene.Mutation):
     allowed_roles = (UserRole.ADMIN, UserRole.SUPERADMIN)
 
     class Arguments:
         name = graphene.String(required=True)
@@ -466,14 +488,15 @@
             "name": name,
             "type": ProjectType[props.type],
             "description": props.description,
             "is_active": props.is_active,
             "domain_name": props.domain_name,
             "integration_id": props.integration_id,
             "resource_policy": props.resource_policy,
+            "container_registry": props.container_registry,
         }
         # set_if_set() applies to optional without defaults
         set_if_set(
             props,
             data,
             "total_resource_slots",
             clean_func=lambda v: ResourceSlot.from_user_input(v, None),
@@ -517,14 +540,15 @@
             data,
             "total_resource_slots",
             clean_func=lambda v: ResourceSlot.from_user_input(v, None),
         )
         set_if_set(props, data, "allowed_vfolder_hosts")
         set_if_set(props, data, "integration_id")
         set_if_set(props, data, "resource_policy")
+        set_if_set(props, data, "container_registry")
 
         if "name" in data and _rx_slug.search(data["name"]) is None:
             raise ValueError("invalid name format. slug format required.")
         if props.user_update_mode not in (None, Undefined, "add", "remove"):
             raise ValueError("invalid user_update_mode")
         if not props.user_uuids:
             props.user_update_mode = None
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/image.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Optional,
     Sequence,
     Tuple,
     Union,
     cast,
     overload,
 )
+from uuid import UUID
 
 import aiotools
 import graphene
 import sqlalchemy as sa
 import trafaret as t
 from graphql import Undefined
 from redis.asyncio import Redis
@@ -32,15 +33,15 @@
 from ai.backend.common import redis_helper
 from ai.backend.common.docker import ImageRef
 from ai.backend.common.etcd import AsyncEtcd
 from ai.backend.common.exception import UnknownImageReference
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.types import BinarySize, ImageAlias, ResourceSlot
 
-from ..api.exceptions import ImageNotFound
+from ..api.exceptions import ImageNotFound, ObjectNotFound
 from ..container_registry import get_container_registry_cls
 from ..defs import DEFAULT_IMAGE_ARCH
 from .base import (
     Base,
     BigInt,
     ForeignKeyIDColumn,
     IDColumn,
@@ -63,26 +64,33 @@
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 __all__ = (
     "rescan_images",
     "ImageType",
     "ImageAliasRow",
+    "ImageLoadFilter",
     "ImageRow",
     "Image",
     "PreloadImage",
     "RescanImages",
     "ForgetImage",
     "ModifyImage",
     "AliasImage",
     "DealiasImage",
     "ClearImages",
 )
 
 
+class ImageLoadFilter(str, enum.Enum):
+    INSTALLED = "installed"
+    EXCLUDE_OPERATIONAL = "operational"
+    CUSTOMIZED_ONLY = "customized"
+
+
 async def rescan_images(
     etcd: AsyncEtcd,
     db: ExtendedAsyncSAEngine,
     registry_or_image: str | None = None,
     *,
     local: bool | None = False,
     reporter: ProgressReporter | None = None,
@@ -187,15 +195,14 @@
                 }),
             ),
         ),
         nullable=False,
     )
     aliases: relationship
     # sessions = relationship("SessionRow", back_populates="image_row")
-    # kernels = relationship("KernelRow", back_populates="image_row")
     endpoints = relationship("EndpointRow", back_populates="image_row")
 
     def __init__(
         self,
         name,
         architecture,
         is_local=False,
@@ -329,14 +336,24 @@
                 if row := await resolver_func(session, reference, load_aliases=load_aliases):
                     return row
             except UnknownImageReference:
                 continue
         raise ImageNotFound("Unknown image references: " + ", ".join(searched_refs))
 
     @classmethod
+    async def get(
+        cls, session: AsyncSession, image_id: UUID, load_aliases=False
+    ) -> ImageRow | None:
+        query = sa.select(ImageRow).where(ImageRow.id == image_id)
+        if load_aliases:
+            query = query.options(selectinload(ImageRow.aliases))
+        result = await session.execute(query)
+        return result.scalar()
+
+    @classmethod
     async def list(cls, session: AsyncSession, load_aliases=False) -> List[ImageRow]:
         query = sa.select(ImageRow)
         if load_aliases:
             query = query.options(selectinload(ImageRow.aliases))
         result = await session.execute(query)
         return result.scalars().all()
 
@@ -620,66 +637,69 @@
         return await cls.from_row(ctx, row)
 
     @classmethod
     async def load_all(
         cls,
         ctx: GraphQueryContext,
         *,
-        is_installed: bool = None,
-        is_operation: bool = None,
+        filters: set[ImageLoadFilter] = set(),
     ) -> Sequence[Image]:
         async with ctx.db.begin_readonly_session() as session:
             rows = await ImageRow.list(session, load_aliases=True)
-        items = [item async for item in cls.bulk_load(ctx, rows)]
-        # Convert to GQL objects
-        if is_installed is not None:
-            items = [*filter(lambda item: item.installed == is_installed, items)]
-        if is_operation is not None:
-
-            def _filter_operation(item):
-                for label in item.labels:
-                    if label.key == "ai.backend.features" and "operation" in label.value:
-                        return not is_operation
-                return not is_operation
+        items: list[Image] = [
+            item async for item in cls.bulk_load(ctx, rows) if item.matches_filter(ctx, filters)
+        ]
 
-            items = [*filter(_filter_operation, items)]
         return items
 
     @staticmethod
     async def filter_allowed(
         ctx: GraphQueryContext,
         items: Sequence[Image],
         domain_name: str,
-        *,
-        is_installed: bool = None,
-        is_operation: bool = None,
     ) -> Sequence[Image]:
         from .domain import domains
 
         async with ctx.db.begin() as conn:
             query = (
                 sa.select([domains.c.allowed_docker_registries])
                 .select_from(domains)
                 .where(domains.c.name == domain_name)
             )
             result = await conn.execute(query)
             allowed_docker_registries = result.scalar()
-        items = [item for item in items if item.registry in allowed_docker_registries]
-        if is_installed is not None:
-            items = [*filter(lambda item: item.installed == is_installed, items)]
-        if is_operation is not None:
-
-            def _filter_operation(item):
-                for label in item.labels:
-                    if label.key == "ai.backend.features" and "operation" in label.value:
-                        return not is_operation
-                return not is_operation
 
-            items = [*filter(_filter_operation, items)]
-        return items
+        filtered_items: list[Image] = [
+            item for item in items if item.registry in allowed_docker_registries
+        ]
+
+        return filtered_items
+
+    def matches_filter(
+        self,
+        ctx: GraphQueryContext,
+        filters: set[ImageLoadFilter],
+    ) -> bool:
+        if ImageLoadFilter.INSTALLED in filters and not self.installed:
+            return False
+
+        is_customized_image = False
+        for label in self.labels:
+            match label.key:
+                case "ai.backend.features" if "operation" in label.value and ImageLoadFilter.EXCLUDE_OPERATIONAL in filters:
+                    return False
+                case "ai.backend.customized-image.owner":
+                    if label.value != f"user:{ctx.user['uuid']}":
+                        return False
+                    is_customized_image = True
+
+        if not is_customized_image and ImageLoadFilter.CUSTOMIZED_ONLY in filters:
+            return False
+
+        return True
 
 
 class ImageNode(graphene.ObjectType):
     class Meta:
         interfaces = (AsyncNode,)
 
     name = graphene.String()
@@ -808,16 +828,67 @@
         async def _rescan_task(reporter: ProgressReporter) -> None:
             await rescan_images(ctx.etcd, ctx.db, registry, reporter=reporter)
 
         task_id = await ctx.background_task_manager.start(_rescan_task)
         return RescanImages(ok=True, msg="", task_id=task_id)
 
 
+class ForgetImageById(graphene.Mutation):
+    """Added since 24.03.0."""
+
+    allowed_roles = (
+        UserRole.SUPERADMIN,
+        UserRole.ADMIN,
+        UserRole.USER,
+    )
+
+    class Arguments:
+        image_id = graphene.String(required=True)
+
+    ok = graphene.Boolean()
+    msg = graphene.String()
+
+    @staticmethod
+    async def mutate(
+        root: Any,
+        info: graphene.ResolveInfo,
+        image_id: str,
+    ) -> ForgetImageById:
+        log.info("forget image {0} by API request", image_id)
+        ctx: GraphQueryContext = info.context
+        client_role = ctx.user["role"]
+
+        async with ctx.db.begin_session() as session:
+            try:
+                _image_id = UUID(image_id)
+            except ValueError:
+                raise ObjectNotFound("image")
+
+            image_row = await ImageRow.get(session, _image_id)
+            if not image_row:
+                raise ObjectNotFound("image")
+            if client_role != UserRole.SUPERADMIN:
+                customized_image_owner = (image_row.labels or {}).get(
+                    "ai.backend.customized-image.owner"
+                )
+                if (
+                    not customized_image_owner
+                    or customized_image_owner != f"user:{ctx.user['uuid']}"
+                ):
+                    return ForgetImageById(ok=False, msg="Forbidden")
+            await session.delete(image_row)
+        return ForgetImageById(ok=True, msg="")
+
+
 class ForgetImage(graphene.Mutation):
-    allowed_roles = (UserRole.SUPERADMIN,)
+    allowed_roles = (
+        UserRole.SUPERADMIN,
+        UserRole.ADMIN,
+        UserRole.USER,
+    )
 
     class Arguments:
         reference = graphene.String(required=True)
         architecture = graphene.String(default_value=DEFAULT_IMAGE_ARCH)
 
     ok = graphene.Boolean()
     msg = graphene.String()
@@ -827,22 +898,33 @@
         root: Any,
         info: graphene.ResolveInfo,
         reference: str,
         architecture: str,
     ) -> ForgetImage:
         log.info("forget image {0} by API request", reference)
         ctx: GraphQueryContext = info.context
+        client_role = ctx.user["role"]
+
         async with ctx.db.begin_session() as session:
             image_row = await ImageRow.resolve(
                 session,
                 [
                     ImageRef(reference, ["*"], architecture),
                     ImageAlias(reference),
                 ],
             )
+            if client_role != UserRole.SUPERADMIN:
+                customized_image_owner = (image_row.labels or {}).get(
+                    "ai.backend.customized-image.owner"
+                )
+                if (
+                    not customized_image_owner
+                    or customized_image_owner != f"user:{ctx.user['uuid']}"
+                ):
+                    return ForgetImage(ok=False, msg="Forbidden")
             await session.delete(image_row)
         return ForgetImage(ok=True, msg="")
 
 
 class AliasImage(graphene.Mutation):
     allowed_roles = (UserRole.SUPERADMIN,)
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/kernel.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/kernel.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     StructuredJSONObjectListColumn,
     URLColumn,
     batch_multiresult,
     batch_result,
     mapper_registry,
 )
 from .group import groups
+from .image import ImageNode
 from .minilang import JSONFieldItem
 from .minilang.ordering import ColumnMapType, QueryOrderParser
 from .minilang.queryfilter import FieldSpecType, QueryFilterParser, enum_field_getter
 from .user import users
 from .utils import ExtendedAsyncSAEngine, execute_with_retry, sql_json_merge
 
 if TYPE_CHECKING:
@@ -545,16 +546,22 @@
     ),
 )
 
 
 class KernelRow(Base):
     __table__ = kernels
     session = relationship("SessionRow", back_populates="kernels")
-    # image_row = relationship("ImageRow", back_populates="kernels")
+    image_row = relationship(
+        "ImageRow",
+        foreign_keys="KernelRow.image",
+        primaryjoin="KernelRow.image == ImageRow.name",
+    )
     agent_row = relationship("AgentRow", back_populates="kernels")
+    group_row = relationship("GroupRow", back_populates="kernels")
+    user_row = relationship("UserRow", back_populates="kernels")
 
     @property
     def image_ref(self) -> ImageRef:
         return ImageRef(self.image, [self.registry], self.architecture)
 
     @property
     def cluster_name(self) -> str:
@@ -788,15 +795,16 @@
     cluster_idx = graphene.Int()
     local_rank = graphene.Int()
     cluster_role = graphene.String()
     cluster_hostname = graphene.String()
     session_id = graphene.UUID()  # owner session
 
     # image
-    image = graphene.String()
+    image = graphene.String(description="Deprecated since 24.03.0; use image_object.name")
+    image_object = graphene.Field(ImageNode, description="Added since 24.03.0")
     architecture = graphene.String()
     registry = graphene.String()
 
     # status
     status = graphene.String()
     status_changed = GQLDateTime()
     status_info = graphene.String()
@@ -814,55 +822,56 @@
     resource_opts = graphene.JSONString()
     occupied_slots = graphene.JSONString()
     live_stat = graphene.JSONString()
     last_stat = graphene.JSONString()
     preopen_ports = graphene.List(lambda: graphene.Int, required=False)
 
     @classmethod
-    def parse_row(cls, ctx: GraphQueryContext, row: Row) -> Mapping[str, Any]:
+    def parse_row(cls, ctx: GraphQueryContext, row: KernelRow) -> Mapping[str, Any]:
         assert row is not None
         from .user import UserRole
 
         is_superadmin = ctx.user["role"] == UserRole.SUPERADMIN
         if is_superadmin:
             hide_agents = False
         else:
             hide_agents = ctx.local_config["manager"]["hide-agents"]
-        status_history = row["status_history"] or {}
+        status_history = row.status_history or {}
         return {
             # identity
-            "id": row["id"],
-            "idx": row["cluster_idx"],
-            "role": row["cluster_role"],
-            "hostname": row["cluster_hostname"],
-            "cluster_idx": row["cluster_idx"],
-            "local_rank": row["local_rank"],
-            "cluster_role": row["cluster_role"],
-            "cluster_hostname": row["cluster_hostname"],
-            "session_id": row["session_id"],
+            "id": row.id,
+            "idx": row.cluster_idx,
+            "role": row.cluster_role,
+            "hostname": row.cluster_hostname,
+            "cluster_idx": row.cluster_idx,
+            "local_rank": row.local_rank,
+            "cluster_role": row.cluster_role,
+            "cluster_hostname": row.cluster_hostname,
+            "session_id": row.session_id,
             # image
-            "image": row["image"],
-            "architecture": row["architecture"],
-            "registry": row["registry"],
+            "image": row.image,
+            "image_object": ImageNode.from_row(row.image_row),
+            "architecture": row.architecture,
+            "registry": row.registry,
             # status
-            "status": row["status"].name,
-            "status_changed": row["status_changed"],
-            "status_info": row["status_info"],
-            "status_data": row["status_data"],
-            "created_at": row["created_at"],
-            "terminated_at": row["terminated_at"],
-            "starts_at": row["starts_at"],
+            "status": row.status.name,
+            "status_changed": row.status_changed,
+            "status_info": row.status_info,
+            "status_data": row.status_data,
+            "created_at": row.created_at,
+            "terminated_at": row.terminated_at,
+            "starts_at": row.starts_at,
             "scheduled_at": status_history.get(KernelStatus.SCHEDULED.name),
-            "occupied_slots": row["occupied_slots"].to_json(),
+            "occupied_slots": row.occupied_slots.to_json(),
             # resources
-            "agent": row["agent"] if not hide_agents else None,
-            "agent_addr": row["agent_addr"] if not hide_agents else None,
-            "container_id": row["container_id"] if not hide_agents else None,
-            "resource_opts": row["resource_opts"],
-            "preopen_ports": row["preopen_ports"],
+            "agent": row.agent if not hide_agents else None,
+            "agent_addr": row.agent_addr if not hide_agents else None,
+            "container_id": row.container_id if not hide_agents else None,
+            "resource_opts": row.resource_opts,
+            "preopen_ports": row.preopen_ports,
             # statistics
             # last_stat is resolved by Graphene (resolve_last_stat method)
         }
 
     @classmethod
     def from_row(cls, ctx: GraphQueryContext, row: Row) -> Optional[ComputeContainer]:
         if row is None:
@@ -935,29 +944,29 @@
         domain_name: str = None,
         group_id: uuid.UUID = None,
         access_key: str = None,
         filter: str = None,
     ) -> int:
         query = (
             sa.select([sa.func.count()])
-            .select_from(kernels)
-            .where(kernels.c.session_id == session_id)
+            .select_from(KernelRow)
+            .where(KernelRow.session_id == session_id)
         )
         if cluster_role is not None:
-            query = query.where(kernels.c.cluster_role == cluster_role)
+            query = query.where(KernelRow.cluster_role == cluster_role)
         if domain_name is not None:
-            query = query.where(kernels.c.domain_name == domain_name)
+            query = query.where(KernelRow.domain_name == domain_name)
         if group_id is not None:
-            query = query.where(kernels.c.group_id == group_id)
+            query = query.where(KernelRow.group_id == group_id)
         if access_key is not None:
-            query = query.where(kernels.c.access_key == access_key)
+            query = query.where(KernelRow.access_key == access_key)
         if filter is not None:
             qfparser = QueryFilterParser(cls._queryfilter_fieldspec)
             query = qfparser.append_filter(query, filter)
-        async with ctx.db.begin_readonly() as conn:
+        async with ctx.db.begin_readonly_session() as conn:
             result = await conn.execute(query)
             return result.scalar()
 
     @classmethod
     async def load_slice(
         cls,
         ctx: GraphQueryContext,
@@ -969,92 +978,91 @@
         domain_name: str = None,
         group_id: uuid.UUID = None,
         access_key: AccessKey = None,
         filter: str = None,
         order: str = None,
     ) -> Sequence[Optional[ComputeContainer]]:
         query = (
-            sa.select([kernels])
-            .select_from(kernels)
-            .where(kernels.c.session_id == session_id)
+            sa.select(KernelRow)
+            .where(KernelRow.session_id == session_id)
             .limit(limit)
             .offset(offset)
+            .options(selectinload(KernelRow.image_row))
         )
         if cluster_role is not None:
-            query = query.where(kernels.c.cluster_role == cluster_role)
+            query = query.where(KernelRow.cluster_role == cluster_role)
         if domain_name is not None:
-            query = query.where(kernels.c.domain_name == domain_name)
+            query = query.where(KernelRow.domain_name == domain_name)
         if group_id is not None:
-            query = query.where(kernels.c.group_id == group_id)
+            query = query.where(KernelRow.group_id == group_id)
         if access_key is not None:
-            query = query.where(kernels.c.access_key == access_key)
+            query = query.where(KernelRow.access_key == access_key)
         if filter is not None:
             qfparser = QueryFilterParser(cls._queryfilter_fieldspec)
             query = qfparser.append_filter(query, filter)
         if order is not None:
             qoparser = QueryOrderParser(cls._queryorder_colmap)
             query = qoparser.append_ordering(query, order)
         else:
             query = query.order_by(*DEFAULT_KERNEL_ORDERING)
-        async with ctx.db.begin_readonly() as conn:
+        async with ctx.db.begin_readonly_session() as conn:
             return [cls.from_row(ctx, r) async for r in (await conn.stream(query))]
 
     @classmethod
     async def batch_load_by_session(
         cls,
         ctx: GraphQueryContext,
         session_ids: Sequence[SessionId],
     ) -> Sequence[Sequence[ComputeContainer]]:
         query = (
-            sa.select([kernels])
-            .select_from(kernels)
+            sa.select(KernelRow)
             # TODO: use "owner session ID" when we implement multi-container session
-            .where(kernels.c.session_id.in_(session_ids))
+            .where(KernelRow.session_id.in_(session_ids))
+            .options(selectinload(KernelRow.image_row))
         )
-        async with ctx.db.begin_readonly() as conn:
+        async with ctx.db.begin_readonly_session() as conn:
             return await batch_multiresult(
                 ctx,
                 conn,
                 query,
                 cls,
                 session_ids,
-                lambda row: row["session_id"],
+                lambda row: row.session_id,
             )
 
     @classmethod
     async def batch_load_detail(
         cls,
         ctx: GraphQueryContext,
         container_ids: Sequence[KernelId],
         *,
         domain_name: str = None,
         access_key: AccessKey = None,
     ) -> Sequence[Optional[ComputeContainer]]:
-        j = kernels.join(groups, groups.c.id == kernels.c.group_id).join(
-            users, users.c.uuid == kernels.c.user_uuid
-        )
         query = (
-            sa.select([kernels])
-            .select_from(j)
+            sa.select(KernelRow)
             .where(
-                (kernels.c.id.in_(container_ids)),
+                (KernelRow.id.in_(container_ids)),
             )
+            .options(selectinload(KernelRow.group_row))
+            .options(selectinload(KernelRow.user_row))
+            .options(selectinload(KernelRow.image_row))
         )
         if domain_name is not None:
-            query = query.where(kernels.c.domain_name == domain_name)
+            query = query.where(KernelRow.domain_name == domain_name)
         if access_key is not None:
-            query = query.where(kernels.c.access_key == access_key)
-        async with ctx.db.begin_readonly() as conn:
+            query = query.where(KernelRow.access_key == access_key)
+        async with ctx.db.begin_readonly_session() as conn:
             return await batch_result(
                 ctx,
                 conn,
                 query,
                 cls,
                 container_ids,
-                lambda row: row["id"],
+                lambda row: row.id,
             )
 
 
 class ComputeContainerList(graphene.ObjectType):
     class Meta:
         interfaces = (PaginatedList,)
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/keypair.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/minilang/__init__.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/minilang/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/minilang/ordering.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/minilang/ordering.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/minilang/queryfilter.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/minilang/queryfilter.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/resource_policy.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/resource_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,28 +98,35 @@
     "user_resource_policies",
     mapper_registry.metadata,
     sa.Column("name", sa.String(length=256), primary_key=True),
     sa.Column("created_at", sa.DateTime(timezone=True), server_default=sa.func.now()),
     sa.Column("max_vfolder_count", sa.Integer(), nullable=False),
     sa.Column("max_quota_scope_size", sa.BigInteger(), nullable=False),
     sa.Column("max_session_count_per_model_session", sa.Integer(), nullable=False),
+    sa.Column("max_customized_image_count", sa.Integer(), nullable=False, default=3),
 )
 
 
 class UserResourcePolicyRow(Base):
     __table__ = user_resource_policies
     users = relationship("UserRow", back_populates="resource_policy_row")
 
     def __init__(
-        self, name, max_vfolder_count, max_quota_scope_size, max_session_count_per_model_session
+        self,
+        name,
+        max_vfolder_count,
+        max_quota_scope_size,
+        max_session_count_per_model_session,
+        max_customized_image_count,
     ) -> None:
         self.name = name
         self.max_vfolder_count = max_vfolder_count
         self.max_quota_scope_size = max_quota_scope_size
         self.max_session_count_per_model_session = max_session_count_per_model_session
+        self.max_customized_image_count = max_customized_image_count
 
 
 project_resource_policies = sa.Table(
     "project_resource_policies",
     mapper_registry.metadata,
     sa.Column("name", sa.String(length=256), primary_key=True),
     sa.Column("created_at", sa.DateTime(timezone=True), server_default=sa.func.now()),
@@ -436,14 +443,17 @@
     max_quota_scope_size = BigInt(
         description="Added since 24.03.1. Limitation of the quota size of user vfolders."
     )
     max_vfolder_size = BigInt(deprecation_reason="Deprecated since 23.09.1")
     max_session_count_per_model_session = graphene.Int(
         description="Added since 23.09.10. Maximum available number of sessions per single model service which the user is in charge of."
     )
+    max_customized_image_count = graphene.Int(
+        description="Added since 24.03.0. Maximum available number of customized images one can publish to."
+    )
 
     @classmethod
     def from_row(
         cls,
         ctx: GraphQueryContext,
         row: UserResourcePolicyRow | None,
     ) -> UserResourcePolicy | None:
@@ -452,14 +462,15 @@
         return cls(
             id=f"UserResourcePolicy:{row.name}",
             name=row.name,
             created_at=row.created_at,
             max_vfolder_count=row.max_vfolder_count,
             max_quota_scope_size=row.max_quota_scope_size,
             max_session_count_per_model_session=row.max_session_count_per_model_session,
+            max_customized_image_count=row.max_customized_image_count,
         )
 
     @classmethod
     async def load_all(cls, ctx: GraphQueryContext) -> Sequence[UserResourcePolicy]:
         query = sa.select(UserResourcePolicyRow)
         async with ctx.db.begin_readonly_session() as sess:
             return [
@@ -517,26 +528,32 @@
     )
     max_quota_scope_size = BigInt(
         description="Added since 24.03.1. Limitation of the quota size of user vfolders."
     )
     max_session_count_per_model_session = graphene.Int(
         description="Added since 24.03.1. Maximum available number of sessions per single model service which the user is in charge of."
     )
+    max_customized_image_count = graphene.Int(
+        description="Added since 24.03.0. Maximum available number of customized images one can publish to."
+    )
 
 
 class ModifyUserResourcePolicyInput(graphene.InputObjectType):
     max_vfolder_count = graphene.Int(
         description="Added since 24.03.1. Limitation of the number of user vfolders."
     )
     max_quota_scope_size = BigInt(
         description="Added since 24.03.1. Limitation of the quota size of user vfolders."
     )
     max_session_count_per_model_session = graphene.Int(
         description="Added since 24.03.1. Maximum available number of sessions per single model service which the user is in charge of."
     )
+    max_customized_image_count = graphene.Int(
+        description="Added since 24.03.0. Maximum available number of customized images one can publish to."
+    )
 
 
 class CreateUserResourcePolicy(graphene.Mutation):
     allowed_roles = (UserRole.SUPERADMIN,)
 
     class Arguments:
         name = graphene.String(required=True)
@@ -559,14 +576,15 @@
         async def _do_mutate() -> UserResourcePolicy:
             async with graph_ctx.db.begin_session() as sess:
                 row = UserResourcePolicyRow(
                     name,
                     props.max_vfolder_count,
                     props.max_quota_scope_size,
                     props.max_session_count_per_model_session,
+                    props.max_customized_image_count,
                 )
                 sess.add(row)
                 await sess.flush()
                 query = sa.select(UserResourcePolicyRow).where(UserResourcePolicyRow.name == name)
                 return cls(
                     True,
                     "success",
@@ -594,14 +612,15 @@
         name: str,
         props: ModifyUserResourcePolicyInput,
     ) -> ModifyUserResourcePolicy:
         data: Dict[str, Any] = {}
         set_if_set(props, data, "max_vfolder_count")
         set_if_set(props, data, "max_quota_scope_size")
         set_if_set(props, data, "max_session_count_per_model_session")
+        set_if_set(props, data, "max_customized_image_count")
         update_query = (
             sa.update(UserResourcePolicyRow).values(data).where(UserResourcePolicyRow.name == name)
         )
         return await simple_db_mutate(cls, info.context, update_query)
 
 
 class DeleteUserResourcePolicy(graphene.Mutation):
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/resource_preset.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/resource_preset.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/resource_usage.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/resource_usage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/routing.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/routing.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/scaling_group.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/session.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -919,15 +919,15 @@
         db_session: SASession,
         session_name_or_id: Union[str, UUID],
         access_key: Optional[AccessKey] = None,
         *,
         allow_stale: bool = False,
         for_update: bool = False,
         kernel_loading_strategy: KernelLoadingStrategy = KernelLoadingStrategy.NONE,
-        eager_loading_op: list[Any] = [],
+        eager_loading_op: list[Any] | None = None,
     ) -> SessionRow:
         """
         Retrieve the session information by session's UUID,
         or session's name paired with access_key.
         This will return the information of the session and the sibling kernel(s).
 
         :param db_session: Database connection to use when fetching row.
@@ -935,41 +935,42 @@
         :param access_key: Access key used to create session.
         :param allow_stale: If set to True, filter "inactive" sessions as well as "active" ones.
                             Otherwise filter "active" sessions only.
         :param for_update: Apply for_update during executing select query.
         :param kernel_loading_strategy: Determines JOIN strategy of `kernels` relation when fetching session rows.
         :param eager_loading_op: Extra loading operators to be passed directly to `match_sessions()` API.
         """
+        _eager_loading_op = eager_loading_op or []
         match kernel_loading_strategy:
             case KernelLoadingStrategy.ALL_KERNELS:
-                eager_loading_op.extend([
+                _eager_loading_op.extend([
                     noload("*"),
                     selectinload(SessionRow.kernels).options(
                         noload("*"),
                         selectinload(KernelRow.agent_row).noload("*"),
                     ),
                 ])
             case KernelLoadingStrategy.MAIN_KERNEL_ONLY:
                 kernel_rel = SessionRow.kernels
                 kernel_rel.and_(KernelRow.cluster_role == DEFAULT_ROLE)
-                eager_loading_op.extend([
+                _eager_loading_op.extend([
                     noload("*"),
                     selectinload(kernel_rel).options(
                         noload("*"),
                         selectinload(KernelRow.agent_row).noload("*"),
                     ),
                 ])
 
         session_list = await cls.match_sessions(
             db_session,
             session_name_or_id,
             access_key,
             allow_stale=allow_stale,
             for_update=for_update,
-            eager_loading_op=eager_loading_op,
+            eager_loading_op=_eager_loading_op,
         )
         if not session_list:
             raise SessionNotFound(f"Session (id={session_name_or_id}) does not exist.")
         if len(session_list) > 1:
             session_infos = [
                 {
                     "session_id": sess.id,
@@ -988,43 +989,44 @@
         db_session: SASession,
         session_ids: list[UUID],
         access_key: Optional[AccessKey] = None,
         *,
         allow_stale: bool = False,
         for_update: bool = False,
         kernel_loading_strategy=KernelLoadingStrategy.NONE,
-        eager_loading_op: list[Any] = [],
+        eager_loading_op: list[Any] | None = None,
     ) -> Iterable[SessionRow]:
+        _eager_loading_op = eager_loading_op or []
         match kernel_loading_strategy:
             case KernelLoadingStrategy.ALL_KERNELS:
-                eager_loading_op.extend([
+                _eager_loading_op.extend([
                     noload("*"),
                     selectinload(SessionRow.kernels).options(
                         noload("*"),
                         selectinload(KernelRow.agent_row).noload("*"),
                     ),
                 ])
             case KernelLoadingStrategy.MAIN_KERNEL_ONLY:
                 kernel_rel = SessionRow.kernels
                 kernel_rel.and_(KernelRow.cluster_role == DEFAULT_ROLE)
-                eager_loading_op.extend([
+                _eager_loading_op.extend([
                     noload("*"),
                     selectinload(kernel_rel).options(
                         noload("*"),
                         selectinload(KernelRow.agent_row).noload("*"),
                     ),
                 ])
 
         session_list = await cls.match_sessions(
             db_session,
             session_ids,
             access_key,
             allow_stale=allow_stale,
             for_update=for_update,
-            eager_loading_op=eager_loading_op,
+            eager_loading_op=_eager_loading_op,
         )
         try:
             return session_list
         except IndexError:
             raise SessionNotFound(f"Session (ids={session_ids}) does not exist.")
 
     @classmethod
@@ -1187,14 +1189,15 @@
     resource_opts = graphene.JSONString()
     scaling_group = graphene.String()
     service_ports = graphene.JSONString()
     mounts = graphene.List(lambda: graphene.String)
     vfolder_mounts = graphene.List(lambda: graphene.String)
     occupying_slots = graphene.JSONString()
     occupied_slots = graphene.JSONString()  # legacy
+    requested_slots = graphene.JSONString(description="Added in 24.03.0")
 
     # statistics
     num_queries = BigInt()
 
     # owned containers (aka kernels)
     containers = graphene.List(lambda: ComputeContainer)
 
@@ -1255,14 +1258,15 @@
             # resources
             "agent_ids": row.agent_ids,
             "agents": row.agent_ids,  # for backward compatibility
             "scaling_group": row.scaling_group_name,
             "service_ports": row.main_kernel.service_ports,
             "mounts": [mount.name for mount in row.vfolder_mounts],
             "vfolder_mounts": row.vfolder_mounts,
+            "requested_slots": row.requested_slots.to_json(),
             # statistics
             "num_queries": row.num_queries,
         }
 
     @classmethod
     def from_row(cls, ctx: GraphQueryContext, row: Row) -> ComputeSession | None:
         if row is None:
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/session_template.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/storage.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/user.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,14 +171,15 @@
     # from .keypair import KeyPairRow
 
     sessions = relationship("SessionRow", back_populates="user")
     domain = relationship("DomainRow", back_populates="users")
     groups = relationship("AssocGroupUserRow", back_populates="user")
     resource_policy_row = relationship("UserResourcePolicyRow", back_populates="users")
     keypairs = relationship("KeyPairRow", back_populates="user_row", foreign_keys="KeyPairRow.user")
+    kernels = relationship("KernelRow", back_populates="user_row")
 
     created_endpoints = relationship(
         "EndpointRow", back_populates="created_user_row", foreign_keys="EndpointRow.created_user"
     )
     owned_endpoints = relationship(
         "EndpointRow", back_populates="session_owner_row", foreign_keys="EndpointRow.session_owner"
     )
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/utils.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/models/vfolder.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/models/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/openapi.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/openapi.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/pglock.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/pglock.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/plugin/error_monitor.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/plugin/error_monitor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/plugin/webapp.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/plugin/webapp.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/registry.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     ClusterMode,
     ClusterSSHKeyPair,
     ClusterSSHPortMapping,
     CommitStatus,
     DeviceId,
     HardwareMetadata,
     ImageAlias,
+    ImageRegistry,
     KernelEnqueueingConfig,
     KernelId,
     ModelServiceStatus,
     RedisConnectionInfo,
     ResourceSlot,
     SessionEnqueueingConfig,
     SessionId,
@@ -453,14 +454,18 @@
                     session,
                     [
                         ImageRef(image, ["*"], architecture),
                         ImageAlias(image),
                     ],
                 )
             requested_image_ref = image_row.image_ref
+            if (
+                _owner_id := image_row.labels.get("ai.backend.customized-image.owner")
+            ) and _owner_id != f"user:{user_scope.user_uuid}":
+                raise ImageNotFound
             if not requested_image_ref.is_local:
                 async with self.db.begin_readonly() as conn:
                     query = (
                         sa.select([domains.c.allowed_docker_registries])
                         .select_from(domains)
                         .where(domains.c.name == user_scope.domain_name)
                     )
@@ -3164,15 +3169,62 @@
             "kernel": kern_id,
             "status": str(result, "utf-8") if result is not None else CommitStatus.READY.value,
         }
 
     async def commit_session(
         self,
         session: SessionRow,
+        new_image_ref: ImageRef,
+        *,
+        extra_labels: dict[str, str] = {},
+    ) -> Mapping[str, Any]:
+        """
+        Commit a main kernel's container of the given session.
+        """
+
+        kernel: KernelRow = session.main_kernel
+        if kernel.status != KernelStatus.RUNNING:
+            raise InvalidAPIParameters(
+                f"Unable to commit since the kernel k:{kernel.id} (of s:{session.id}) is"
+                " currently not in RUNNING state."
+            )
+        email = await self._get_user_email(kernel)
+        async with handle_session_exception(self.db, "commit_session", session.id):
+            async with self.agent_cache.rpc_context(kernel.agent, order_key=kernel.id) as rpc:
+                resp: Mapping[str, Any] = await rpc.call.commit(
+                    str(kernel.id),
+                    email,
+                    canonical=new_image_ref.canonical,
+                    extra_labels=extra_labels,
+                )
+        return resp
+
+    async def push_image(
+        self,
+        agent: AgentId,
+        image_ref: ImageRef,
+        registry: ImageRegistry,
+    ) -> Mapping[str, Any]:
+        """
+        Commit a main kernel's container of the given session.
+        """
+        async with self.agent_cache.rpc_context(agent) as rpc:
+            resp: Mapping[str, Any] = await rpc.call.push_image(
+                image_ref.canonical,
+                image_ref.architecture,
+                {**registry, "url": str(registry["url"])},
+                is_local=image_ref.is_local,
+            )
+        return resp
+
+    async def commit_session_to_file(
+        self,
+        session: SessionRow,
         filename: str | None,
+        extra_labels: dict[str, str] = {},
     ) -> Mapping[str, Any]:
         """
         Commit a main kernel's container of the given session.
         """
 
         kernel: KernelRow = session.main_kernel
         if kernel.status != KernelStatus.RUNNING:
@@ -3183,17 +3235,19 @@
         email = await self._get_user_email(kernel)
         now = datetime.now(tzutc()).strftime("%Y-%m-%dT%HH%MM%SS")
         shortend_sname = session.name[:SESSION_NAME_LEN_LIMIT]
         registry, _, filtered = kernel.image.partition("/")
         img_path, _, image_name = filtered.partition("/")
         filename = f"{now}_{shortend_sname}_{image_name}.tar.gz"
         filename = filename.replace(":", "-")
-        async with handle_session_exception(self.db, "commit_session", session.id):
+        async with handle_session_exception(self.db, "commit_session_to_file", session.id):
             async with self.agent_cache.rpc_context(kernel.agent, order_key=kernel.id) as rpc:
-                resp: Mapping[str, Any] = await rpc.call.commit(str(kernel.id), email, filename)
+                resp: Mapping[str, Any] = await rpc.call.commit(
+                    str(kernel.id), email, filename=filename, extra_labels=extra_labels
+                )
         return resp
 
     async def get_agent_local_config(
         self,
         agent_id: AgentId,
         agent_addr: str,
     ) -> Mapping[str, str]:
```

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/scheduler/dispatcher.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/scheduler/dispatcher.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/scheduler/drf.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/scheduler/drf.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/scheduler/fifo.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/scheduler/fifo.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/scheduler/mof.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/scheduler/mof.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/scheduler/predicates.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/scheduler/predicates.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/scheduler/types.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/scheduler/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/server.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/server.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/types.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/utils.py` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/vendor/bai-icon.svg` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/vendor/bai-icon.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/vendor/graphiql.min.css` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/vendor/graphiql.min.css`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/vendor/graphiql.min.js` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/vendor/graphiql.min.js`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/vendor/react-dom.production.min.js` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/vendor/react-dom.production.min.js`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/vendor/react.production.min.js` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/vendor/react.production.min.js`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/ai/backend/manager/vendor/spec-viewer.js` & `backend.ai-manager-24.3.0rc3/ai/backend/manager/vendor/spec-viewer.js`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/backend.ai_manager.egg-info/SOURCES.txt` & `backend.ai-manager-24.3.0rc3/backend.ai_manager.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -164,14 +164,15 @@
 ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
 ai/backend/manager/models/alembic/versions/7ff52ff68bfc_detail_vfolder_deletion_status.py
 ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
 ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
 ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
 ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
 ai/backend/manager/models/alembic/versions/85615e005fa3_kernel_requested_slots_to_not_nullable.py
+ai/backend/manager/models/alembic/versions/857b763b8618_add_groups_per_user_image_storage.py
 ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
 ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py
 ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
 ai/backend/manager/models/alembic/versions/8b2ec7e3d22a_remove_unique_constraint_of_endpoint_url.py
 ai/backend/manager/models/alembic/versions/8c74e7df26f8_make_routings_contain_error.py
 ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
 ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
```

### Comparing `backend.ai-manager-24.3.0rc2/backend_shim.py` & `backend.ai-manager-24.3.0rc3/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-24.3.0rc2/setup.py` & `backend.ai-manager-24.3.0rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
         'Development Status :: 4 - Beta',
-        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
     ],
     'description': 'Backend.AI Manager',
     'entry_points': {
         'backendai_cli_v10': [
             'mgr = ai.backend.manager.cli.__main__:main',
             'mgr.start-server = ai.backend.manager.server:main',
@@ -46,19 +46,19 @@
         'aiohttp_sse>=2.0',
         'aiohttp~=3.9.1',
         'aiomonitor~=0.7.0',
         'aiotools~=1.7.0',
         'alembic~=1.12.0',
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
         'bcrypt>=4.1.2',
         'callosum~=1.0.3',
         'click~=8.1.7',
         'cryptography>=2.8',
         'etcd-client-py==0.2.4',
         'graphene~=3.3.0',
@@ -77,15 +77,15 @@
         'types-PyYAML',
         'types-aiofiles',
         'types-python-dateutil',
         'types-redis',
         'types-six',
         'types-tabulate',
         'typing_extensions~=4.3',
-        'uvloop~=0.17.0; sys_platform != "Windows"',
+        'uvloop~=0.19.0; sys_platform != "Windows"',
         'yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2',
     ),
     'license': 'LGPLv3',
     'long_description': """Backend.AI Manager with API Gateway
 ===================================
 
 Package Structure
@@ -386,13 +386,13 @@
         'ai.backend.manager.scheduler',
         'ai.backend.manager.vendor',
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

