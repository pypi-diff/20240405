# Comparing `tmp/avtomat_aws-0.0.2.tar.gz` & `tmp/avtomat_aws-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avtomat_aws-0.0.2.tar", max compression
+gzip compressed data, was "avtomat_aws-0.0.3.tar", max compression
```

## Comparing `avtomat_aws-0.0.2.tar` & `avtomat_aws-0.0.3.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0       59 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0    18091 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/LICENSE
--rw-r--r--   0        0        0     3512 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/README.md
--rw-r--r--   0        0        0       69 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/cli/__init__.py
--rw-r--r--   0        0        0     1495 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/cli/backup/create_backups.py
--rw-r--r--   0        0        0      833 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/cli/backup/delete_backups.py
--rw-r--r--   0        0        0      897 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/cli/cloudtrail/discover_events.py
--rw-r--r--   0        0        0     1125 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/cli/cloudtrail/discover_resource_events.py
--rw-r--r--   0        0        0     1114 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/cli/cloudtrail/discover_user_events.py
--rw-r--r--   0        0        0     1269 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/copy_snapshots.py
--rw-r--r--   0        0        0      824 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/delete_images.py
--rw-r--r--   0        0        0      687 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/delete_security_groups.py
--rw-r--r--   0        0        0      657 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/delete_snapshots.py
--rw-r--r--   0        0        0      803 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/delete_volumes.py
--rw-r--r--   0        0        0      472 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_active_regions.py
--rw-r--r--   0        0        0      451 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py
--rw-r--r--   0        0        0     1203 2024-04-04 23:14:55.136080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_images.py
--rw-r--r--   0        0        0     1369 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_instances.py
--rw-r--r--   0        0        0      634 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_no_ssm_instances.py
--rw-r--r--   0        0        0     1401 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_snapshots.py
--rw-r--r--   0        0        0     1172 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_tags.py
--rw-r--r--   0        0        0      481 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_unused_security_groups.py
--rw-r--r--   0        0        0     1207 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_volumes.py
--rw-r--r--   0        0        0      899 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/encrypt_instance_volumes.py
--rw-r--r--   0        0        0      823 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/encrypt_volume.py
--rw-r--r--   0        0        0     1175 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py
--rw-r--r--   0        0        0     1220 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/modify_tags.py
--rw-r--r--   0        0        0     1100 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/modify_volumes.py
--rw-r--r--   0        0        0      793 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/ec2/share_snapshots.py
--rw-r--r--   0        0        0      816 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/general/get_date.py
--rw-r--r--   0        0        0      760 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/iam/discover_inactive_console_users.py
--rw-r--r--   0        0        0      750 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/iam/discover_inactive_users.py
--rw-r--r--   0        0        0      468 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/iam/discover_no_mfa_users.py
--rw-r--r--   0        0        0      701 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/iam/discover_old_access_keys.py
--rw-r--r--   0        0        0      732 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/iam/discover_old_password_users.py
--rw-r--r--   0        0        0      735 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/iam/discover_unused_access_keys.py
--rw-r--r--   0        0        0      715 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/iam/discover_unused_roles.py
--rw-r--r--   0        0        0     1231 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/iam/modify_access_keys.py
--rw-r--r--   0        0        0     1333 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/iam/modify_users_console_access.py
--rw-r--r--   0        0        0      593 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/iam/quarantine_user.py
--rw-r--r--   0        0        0     2006 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/main.py
--rw-r--r--   0        0        0     1211 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/s3/create_objects.py
--rw-r--r--   0        0        0      864 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/s3/delete_objects.py
--rw-r--r--   0        0        0     1194 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/s3/discover_objects.py
--rw-r--r--   0        0        0     1337 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/services.py
--rw-r--r--   0        0        0     1375 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/sts/create_session.py
--rw-r--r--   0        0        0      391 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/cli/sts/whoami.py
--rw-r--r--   0        0        0        0 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/decorators/__init__.py
--rw-r--r--   0        0        0      963 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/decorators/authenticate.py
--rw-r--r--   0        0        0      610 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/decorators/set_logger.py
--rw-r--r--   0        0        0      724 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/decorators/validate.py
--rw-r--r--   0        0        0        0 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/helpers/__init__.py
--rw-r--r--   0        0        0      285 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/helpers/set_defaults.py
--rw-r--r--   0        0        0      805 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/helpers/set_region.py
--rw-r--r--   0        0        0     2502 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/helpers/set_session.py
--rw-r--r--   0        0        0      890 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/helpers/set_session_objects.py
--rw-r--r--   0        0        0        0 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/loggers/__init__.py
--rw-r--r--   0        0        0      457 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/loggers/config.py
--rw-r--r--   0        0        0      138 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/loggers/set_logging.py
--rw-r--r--   0        0        0        0 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/__init__.py
--rw-r--r--   0        0        0       86 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/backup/__init__.py
--rw-r--r--   0        0        0     3810 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/backup/create_backups.py
--rw-r--r--   0        0        0     1629 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/backup/delete_backups.py
--rw-r--r--   0        0        0      163 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/cloudtrail/__init__.py
--rw-r--r--   0        0        0     2784 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/cloudtrail/discover_events.py
--rw-r--r--   0        0        0     3383 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/cloudtrail/discover_resource_events.py
--rw-r--r--   0        0        0     3252 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/cloudtrail/discover_user_events.py
--rw-r--r--   0        0        0     1052 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/__init__.py
--rw-r--r--   0        0        0     2771 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/copy_snapshots.py
--rw-r--r--   0        0        0     2264 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/delete_images.py
--rw-r--r--   0        0        0     1532 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/delete_security_groups.py
--rw-r--r--   0        0        0     1430 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/delete_snapshots.py
--rw-r--r--   0        0        0     2663 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/delete_volumes.py
--rw-r--r--   0        0        0      902 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_active_regions.py
--rw-r--r--   0        0        0     1346 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_default_ebs_encryption.py
--rw-r--r--   0        0        0     2929 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_images.py
--rw-r--r--   0        0        0     3662 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_instances.py
--rw-r--r--   0        0        0     1800 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_no_ssm_instances.py
--rw-r--r--   0        0        0     3247 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_snapshots.py
--rw-r--r--   0        0        0     5192 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_tags.py
--rw-r--r--   0        0        0    16665 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_unused_security_groups.py
--rw-r--r--   0        0        0     2625 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_volumes.py
--rw-r--r--   0        0        0     4757 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/encrypt_instance_volumes.py
--rw-r--r--   0        0        0     3973 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/encrypt_volume.py
--rw-r--r--   0        0        0     1853 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/modify_default_ebs_encryption.py
--rw-r--r--   0        0        0     4818 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/modify_tags.py
--rw-r--r--   0        0        0     2983 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/modify_volumes.py
--rw-r--r--   0        0        0     1819 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/ec2/share_snapshots.py
--rw-r--r--   0        0        0       31 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/general/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/general/get_date.py
--rw-r--r--   0        0        0      618 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/iam/__init__.py
--rw-r--r--   0        0        0     2674 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/iam/discover_inactive_console_users.py
--rw-r--r--   0        0        0     3228 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/iam/discover_inactive_users.py
--rw-r--r--   0        0        0     1538 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/iam/discover_no_mfa_users.py
--rw-r--r--   0        0        0     2138 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/iam/discover_old_access_keys.py
--rw-r--r--   0        0        0     2026 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/iam/discover_old_password_users.py
--rw-r--r--   0        0        0     2808 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/iam/discover_unused_access_keys.py
--rw-r--r--   0        0        0     1945 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/iam/discover_unused_roles.py
--rw-r--r--   0        0        0     2081 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/iam/modify_access_keys.py
--rw-r--r--   0        0        0     3175 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/iam/modify_users_console_access.py
--rw-r--r--   0        0        0     1719 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/iam/quarantine_user.py
--rw-r--r--   0        0        0      133 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/s3/__init__.py
--rw-r--r--   0        0        0     1908 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/s3/create_objects.py
--rw-r--r--   0        0        0     2141 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/s3/delete_objects.py
--rw-r--r--   0        0        0     2517 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/s3/discover_objects.py
--rw-r--r--   0        0        0       70 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/sts/__init__.py
--rw-r--r--   0        0        0      750 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/sts/create_session.py
--rw-r--r--   0        0        0      717 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/services/sts/whoami.py
--rw-r--r--   0        0        0        0 2024-04-04 23:14:55.140080 avtomat_aws-0.0.2/avtomat_aws/validations/__init__.py
--rw-r--r--   0        0        0      291 2024-04-04 23:14:55.144080 avtomat_aws-0.0.2/avtomat_aws/validations/config.py
--rw-r--r--   0        0        0     3417 2024-04-04 23:14:55.144080 avtomat_aws-0.0.2/avtomat_aws/validations/rules.py
--rw-r--r--   0        0        0      496 2024-04-04 23:14:55.144080 avtomat_aws-0.0.2/avtomat_aws/validations/validate.py
--rw-r--r--   0        0        0     1733 2024-04-04 23:14:55.144080 avtomat_aws-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4829 1970-01-01 00:00:00.000000 avtomat_aws-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      128 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0    18091 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3512 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/README.md
+-rw-r--r--   0        0        0       69 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/__init__.py
+-rw-r--r--   0        0        0     1495 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/backup/create_backups.py
+-rw-r--r--   0        0        0      833 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/backup/delete_backups.py
+-rw-r--r--   0        0        0      897 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/cloudtrail/discover_events.py
+-rw-r--r--   0        0        0     1125 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/cloudtrail/discover_resource_events.py
+-rw-r--r--   0        0        0     1114 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/cloudtrail/discover_user_events.py
+-rw-r--r--   0        0        0     1269 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/copy_snapshots.py
+-rw-r--r--   0        0        0      824 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_images.py
+-rw-r--r--   0        0        0      687 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_security_groups.py
+-rw-r--r--   0        0        0      657 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_snapshots.py
+-rw-r--r--   0        0        0      803 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_volumes.py
+-rw-r--r--   0        0        0      472 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_active_regions.py
+-rw-r--r--   0        0        0      451 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_default_ebs_encryption.py
+-rw-r--r--   0        0        0     1203 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_images.py
+-rw-r--r--   0        0        0     1369 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_instances.py
+-rw-r--r--   0        0        0      634 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_no_ssm_instances.py
+-rw-r--r--   0        0        0     1401 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_snapshots.py
+-rw-r--r--   0        0        0     1172 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_tags.py
+-rw-r--r--   0        0        0      481 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_unused_security_groups.py
+-rw-r--r--   0        0        0     1207 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_volumes.py
+-rw-r--r--   0        0        0      899 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/encrypt_instance_volumes.py
+-rw-r--r--   0        0        0      823 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/encrypt_volume.py
+-rw-r--r--   0        0        0     1175 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py
+-rw-r--r--   0        0        0     1220 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/modify_tags.py
+-rw-r--r--   0        0        0     1100 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/modify_volumes.py
+-rw-r--r--   0        0        0      793 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/ec2/share_snapshots.py
+-rw-r--r--   0        0        0      816 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/general/get_date.py
+-rw-r--r--   0        0        0      760 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_inactive_console_users.py
+-rw-r--r--   0        0        0      750 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_inactive_users.py
+-rw-r--r--   0        0        0      468 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_no_mfa_users.py
+-rw-r--r--   0        0        0      701 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_old_access_keys.py
+-rw-r--r--   0        0        0      732 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_old_password_users.py
+-rw-r--r--   0        0        0      735 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_unused_access_keys.py
+-rw-r--r--   0        0        0      715 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_unused_roles.py
+-rw-r--r--   0        0        0     1231 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/modify_access_keys.py
+-rw-r--r--   0        0        0     1333 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/modify_users_console_access.py
+-rw-r--r--   0        0        0      593 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/iam/quarantine_user.py
+-rw-r--r--   0        0        0     2006 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/main.py
+-rw-r--r--   0        0        0     1211 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/s3/create_objects.py
+-rw-r--r--   0        0        0      864 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/s3/delete_objects.py
+-rw-r--r--   0        0        0     1194 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/s3/discover_objects.py
+-rw-r--r--   0        0        0     1337 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/services.py
+-rw-r--r--   0        0        0     1375 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/sts/create_session.py
+-rw-r--r--   0        0        0      391 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/cli/sts/whoami.py
+-rw-r--r--   0        0        0        0 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/decorators/__init__.py
+-rw-r--r--   0        0        0      963 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/decorators/authenticate.py
+-rw-r--r--   0        0        0      610 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/decorators/set_logger.py
+-rw-r--r--   0        0        0      724 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/decorators/validate.py
+-rw-r--r--   0        0        0        0 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/helpers/__init__.py
+-rw-r--r--   0        0        0      288 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/helpers/set_defaults.py
+-rw-r--r--   0        0        0      805 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/helpers/set_region.py
+-rw-r--r--   0        0        0     2502 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/helpers/set_session.py
+-rw-r--r--   0        0        0      890 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/helpers/set_session_objects.py
+-rw-r--r--   0        0        0        0 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/loggers/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/loggers/config.py
+-rw-r--r--   0        0        0      138 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/loggers/set_logging.py
+-rw-r--r--   0        0        0        0 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/backup/__init__.py
+-rw-r--r--   0        0        0     3810 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/backup/create_backups.py
+-rw-r--r--   0        0        0     1629 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/backup/delete_backups.py
+-rw-r--r--   0        0        0      163 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/cloudtrail/__init__.py
+-rw-r--r--   0        0        0     2784 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/cloudtrail/discover_events.py
+-rw-r--r--   0        0        0     3383 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/cloudtrail/discover_resource_events.py
+-rw-r--r--   0        0        0     3252 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/cloudtrail/discover_user_events.py
+-rw-r--r--   0        0        0     1052 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/__init__.py
+-rw-r--r--   0        0        0     2771 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/copy_snapshots.py
+-rw-r--r--   0        0        0     2264 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_images.py
+-rw-r--r--   0        0        0     1532 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_security_groups.py
+-rw-r--r--   0        0        0     1430 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_snapshots.py
+-rw-r--r--   0        0        0     2663 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_volumes.py
+-rw-r--r--   0        0        0      902 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_active_regions.py
+-rw-r--r--   0        0        0     1346 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_default_ebs_encryption.py
+-rw-r--r--   0        0        0     2929 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_images.py
+-rw-r--r--   0        0        0     3662 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_instances.py
+-rw-r--r--   0        0        0     1800 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_no_ssm_instances.py
+-rw-r--r--   0        0        0     3247 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_snapshots.py
+-rw-r--r--   0        0        0     5192 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_tags.py
+-rw-r--r--   0        0        0    16665 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_unused_security_groups.py
+-rw-r--r--   0        0        0     2625 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_volumes.py
+-rw-r--r--   0        0        0     4757 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/encrypt_instance_volumes.py
+-rw-r--r--   0        0        0     3973 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/encrypt_volume.py
+-rw-r--r--   0        0        0     1853 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/modify_default_ebs_encryption.py
+-rw-r--r--   0        0        0     4818 2024-04-04 23:24:53.140177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/modify_tags.py
+-rw-r--r--   0        0        0     2983 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/modify_volumes.py
+-rw-r--r--   0        0        0     1819 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/ec2/share_snapshots.py
+-rw-r--r--   0        0        0       31 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/general/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/general/get_date.py
+-rw-r--r--   0        0        0      618 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/__init__.py
+-rw-r--r--   0        0        0     2674 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_inactive_console_users.py
+-rw-r--r--   0        0        0     3228 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_inactive_users.py
+-rw-r--r--   0        0        0     1538 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_no_mfa_users.py
+-rw-r--r--   0        0        0     2138 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_old_access_keys.py
+-rw-r--r--   0        0        0     2026 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_old_password_users.py
+-rw-r--r--   0        0        0     2808 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_unused_access_keys.py
+-rw-r--r--   0        0        0     1945 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_unused_roles.py
+-rw-r--r--   0        0        0     2081 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/modify_access_keys.py
+-rw-r--r--   0        0        0     3175 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/modify_users_console_access.py
+-rw-r--r--   0        0        0     1719 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/iam/quarantine_user.py
+-rw-r--r--   0        0        0      133 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/s3/__init__.py
+-rw-r--r--   0        0        0     1908 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/s3/create_objects.py
+-rw-r--r--   0        0        0     2141 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/s3/delete_objects.py
+-rw-r--r--   0        0        0     2517 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/s3/discover_objects.py
+-rw-r--r--   0        0        0       70 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/sts/__init__.py
+-rw-r--r--   0        0        0      750 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/sts/create_session.py
+-rw-r--r--   0        0        0      717 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/services/sts/whoami.py
+-rw-r--r--   0        0        0        0 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/validations/__init__.py
+-rw-r--r--   0        0        0      291 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/validations/config.py
+-rw-r--r--   0        0        0     3417 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/validations/rules.py
+-rw-r--r--   0        0        0      496 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/avtomat_aws/validations/validate.py
+-rw-r--r--   0        0        0     1733 2024-04-04 23:24:53.144177 avtomat_aws-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4829 1970-01-01 00:00:00.000000 avtomat_aws-0.0.3/PKG-INFO
```

### Comparing `avtomat_aws-0.0.2/LICENSE` & `avtomat_aws-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/README.md` & `avtomat_aws-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/backup/create_backups.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/backup/create_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/backup/delete_backups.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/backup/delete_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/cloudtrail/discover_events.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/cloudtrail/discover_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/cloudtrail/discover_resource_events.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/cloudtrail/discover_resource_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/cloudtrail/discover_user_events.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/cloudtrail/discover_user_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/copy_snapshots.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/copy_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/delete_images.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/delete_security_groups.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/delete_snapshots.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/delete_volumes.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/delete_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_images.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_instances.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_no_ssm_instances.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_no_ssm_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_snapshots.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_tags.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/discover_volumes.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/discover_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/encrypt_instance_volumes.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/encrypt_instance_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/encrypt_volume.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/encrypt_volume.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/modify_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/modify_tags.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/modify_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/modify_volumes.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/modify_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/ec2/share_snapshots.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/ec2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/general/get_date.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/general/get_date.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/iam/discover_inactive_console_users.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_inactive_console_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/iam/discover_inactive_users.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_inactive_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/iam/discover_old_access_keys.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_old_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/iam/discover_old_password_users.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_old_password_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/iam/discover_unused_access_keys.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_unused_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/iam/discover_unused_roles.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/iam/discover_unused_roles.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/iam/modify_access_keys.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/iam/modify_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/iam/modify_users_console_access.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/iam/modify_users_console_access.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/iam/quarantine_user.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/iam/quarantine_user.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/main.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/main.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/s3/create_objects.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/s3/create_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/s3/delete_objects.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/s3/delete_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/s3/discover_objects.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/s3/discover_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/services.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/services.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/cli/sts/create_session.py` & `avtomat_aws-0.0.3/avtomat_aws/cli/sts/create_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/decorators/authenticate.py` & `avtomat_aws-0.0.3/avtomat_aws/decorators/authenticate.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/decorators/set_logger.py` & `avtomat_aws-0.0.3/avtomat_aws/decorators/set_logger.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/decorators/validate.py` & `avtomat_aws-0.0.3/avtomat_aws/decorators/validate.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/helpers/set_region.py` & `avtomat_aws-0.0.3/avtomat_aws/helpers/set_region.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/helpers/set_session.py` & `avtomat_aws-0.0.3/avtomat_aws/helpers/set_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/helpers/set_session_objects.py` & `avtomat_aws-0.0.3/avtomat_aws/helpers/set_session_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/backup/create_backups.py` & `avtomat_aws-0.0.3/avtomat_aws/services/backup/create_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/backup/delete_backups.py` & `avtomat_aws-0.0.3/avtomat_aws/services/backup/delete_backups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/cloudtrail/discover_events.py` & `avtomat_aws-0.0.3/avtomat_aws/services/cloudtrail/discover_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/cloudtrail/discover_resource_events.py` & `avtomat_aws-0.0.3/avtomat_aws/services/cloudtrail/discover_resource_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/cloudtrail/discover_user_events.py` & `avtomat_aws-0.0.3/avtomat_aws/services/cloudtrail/discover_user_events.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/__init__.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/copy_snapshots.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/copy_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/delete_images.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/delete_security_groups.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/delete_snapshots.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/delete_volumes.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/delete_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_active_regions.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_active_regions.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_default_ebs_encryption.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_images.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_images.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_instances.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_no_ssm_instances.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_no_ssm_instances.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_snapshots.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_tags.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_unused_security_groups.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_unused_security_groups.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/discover_volumes.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/discover_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/encrypt_instance_volumes.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/encrypt_instance_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/encrypt_volume.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/encrypt_volume.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/modify_default_ebs_encryption.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/modify_default_ebs_encryption.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/modify_tags.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/modify_tags.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/modify_volumes.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/modify_volumes.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/ec2/share_snapshots.py` & `avtomat_aws-0.0.3/avtomat_aws/services/ec2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/general/get_date.py` & `avtomat_aws-0.0.3/avtomat_aws/services/general/get_date.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/iam/__init__.py` & `avtomat_aws-0.0.3/avtomat_aws/services/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/iam/discover_inactive_console_users.py` & `avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_inactive_console_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/iam/discover_inactive_users.py` & `avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_inactive_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/iam/discover_no_mfa_users.py` & `avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_no_mfa_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/iam/discover_old_access_keys.py` & `avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_old_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/iam/discover_old_password_users.py` & `avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_old_password_users.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/iam/discover_unused_access_keys.py` & `avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_unused_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/iam/discover_unused_roles.py` & `avtomat_aws-0.0.3/avtomat_aws/services/iam/discover_unused_roles.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/iam/modify_access_keys.py` & `avtomat_aws-0.0.3/avtomat_aws/services/iam/modify_access_keys.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/iam/modify_users_console_access.py` & `avtomat_aws-0.0.3/avtomat_aws/services/iam/modify_users_console_access.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/iam/quarantine_user.py` & `avtomat_aws-0.0.3/avtomat_aws/services/iam/quarantine_user.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/s3/create_objects.py` & `avtomat_aws-0.0.3/avtomat_aws/services/s3/create_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/s3/delete_objects.py` & `avtomat_aws-0.0.3/avtomat_aws/services/s3/delete_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/s3/discover_objects.py` & `avtomat_aws-0.0.3/avtomat_aws/services/s3/discover_objects.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/sts/create_session.py` & `avtomat_aws-0.0.3/avtomat_aws/services/sts/create_session.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/services/sts/whoami.py` & `avtomat_aws-0.0.3/avtomat_aws/services/sts/whoami.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/avtomat_aws/validations/rules.py` & `avtomat_aws-0.0.3/avtomat_aws/validations/rules.py`

 * *Files identical despite different names*

### Comparing `avtomat_aws-0.0.2/pyproject.toml` & `avtomat_aws-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "avtomat-aws"
-version = "0.0.2"
+version = "0.0.3"
 description = "Automate AWS cloud operations by using pre-defined actions instead of scripting from scratch."
 authors = ["Dimitar Atanasov <dimitar@avtomat.io>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://avtomat.io"
 documentation = "https://docs.avtomat.io/aws/get_started"
 keywords = ["aws", "cloud", "automation", "cli", "python", "boto3"]
```

### Comparing `avtomat_aws-0.0.2/PKG-INFO` & `avtomat_aws-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avtomat-aws
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automate AWS cloud operations by using pre-defined actions instead of scripting from scratch.
 Home-page: https://avtomat.io
 License: GPL-2.0-only
 Keywords: aws,cloud,automation,cli,python,boto3
 Author: Dimitar Atanasov
 Author-email: dimitar@avtomat.io
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: avtomat-aws Version: 0.0.2 Summary: Automate AWS
+Metadata-Version: 2.1 Name: avtomat-aws Version: 0.0.3 Summary: Automate AWS
 cloud operations by using pre-defined actions instead of scripting from
 scratch. Home-page: https://avtomat.io License: GPL-2.0-only Keywords:
 aws,cloud,automation,cli,python,boto3 Author: Dimitar Atanasov Author-email:
 dimitar@avtomat.io Requires-Python: >=3.9,<4.0 Classifier: Development Status
 :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

