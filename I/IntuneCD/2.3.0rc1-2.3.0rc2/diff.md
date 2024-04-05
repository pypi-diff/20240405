# Comparing `tmp/IntuneCD-2.3.0rc1.tar.gz` & `tmp/IntuneCD-2.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IntuneCD-2.3.0rc1.tar", last modified: Fri Mar 22 11:55:32 2024, max compression
+gzip compressed data, was "IntuneCD-2.3.0rc2.tar", last modified: Mon Mar 25 13:16:26 2024, max compression
```

## Comparing `IntuneCD-2.3.0rc1.tar` & `IntuneCD-2.3.0rc2.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:32.101178 IntuneCD-2.3.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-03-22 11:55:32.101178 IntuneCD-2.3.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-22 11:55:32.101178 IntuneCD-2.3.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:32.077178 IntuneCD-2.3.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:32.081178 IntuneCD-2.3.0rc1/src/IntuneCD/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:32.081178 IntuneCD-2.3.0rc1/src/IntuneCD/backup/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:32.085178 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/Applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/AuthenticationFlows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/AuthenticationMethods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/AuthorizationPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/B2B.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/DeviceRegistration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/Domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/ExternalIdentities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/GroupSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/RoamingSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/SSPR.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/SecurityDefaults.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:32.089178 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/APNs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/Activationlock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/AppConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/AppProtection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/AppleEnrollmentProfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/Applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/AutopilotDevices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/Compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/CompliancePartner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ComplianceScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ConditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/CustomAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/DeviceCategories.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/DeviceCompliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/DeviceConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/DeviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/EnrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/EnrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/Filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/GroupPolicyConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ManagedGooglePlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ManagementIntents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ManagementPartner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/NotificationTemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/PowershellScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ProactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/RemoteAssistancePartner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ReusableSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/Roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ScopeTags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/SettingsCatalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ShellScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/VolumePurchaseProgram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/WindowsDriverUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/WindowsEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/WindowsFeatureUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/WindowsQualityUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup_entra.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/backup_intune.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/document_entra.py
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/document_intune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:32.093178 IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/BaseBackupModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    36404 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/BaseGraphModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/BaseUpdateModule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/IntuneCDBase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/assignment_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    17908 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/get_accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/get_authparams.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/process_audit_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/process_scope_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    11182 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/run_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/run_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10891 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/run_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:32.093178 IntuneCD-2.3.0rc1/src/IntuneCD/update/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:32.093178 IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/AuthenticationFlows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/AuthenticationMethodsConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/AuthenticationMethodsPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/AuthorizationPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/B2B.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/DeviceRegistration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/Domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/ExternalIdentitiesPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/GroupSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/RoamingSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/SSPR.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/SecurityDefaults.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:32.101178 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/AppConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/AppProtection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/AppleEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/Compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/ComplianceScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/ConditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/CustomAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/DeviceCategories.py
--rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/DeviceCompliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/DeviceConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/DeviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/EnrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/EnrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/Filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    23308 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/GroupPolicyConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/ManagementIntents.py
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/NotificationTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/PowerShellScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/ProactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/ReusableSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/Roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/ScopeTags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/SettingsCatalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/ShellScripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/WindowsDriverUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/WindowsEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/WindowsFeatureUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/WindowsQualityUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update_entra.py
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/src/IntuneCD/update_intune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:32.101178 IntuneCD-2.3.0rc1/src/IntuneCD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-03-22 11:55:32.000000 IntuneCD-2.3.0rc1/src/IntuneCD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-03-22 11:55:32.000000 IntuneCD-2.3.0rc1/src/IntuneCD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 11:55:32.000000 IntuneCD-2.3.0rc1/src/IntuneCD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-22 11:55:32.000000 IntuneCD-2.3.0rc1/src/IntuneCD.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-22 11:55:32.000000 IntuneCD-2.3.0rc1/src/IntuneCD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-22 11:55:32.000000 IntuneCD-2.3.0rc1/src/IntuneCD.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:55:32.101178 IntuneCD-2.3.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/tests/test_documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-03-22 11:55:25.000000 IntuneCD-2.3.0rc1/tests/test_get_authparams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:26.599439 IntuneCD-2.3.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-03-25 13:16:26.599439 IntuneCD-2.3.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-25 13:16:26.599439 IntuneCD-2.3.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:26.575440 IntuneCD-2.3.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:26.579439 IntuneCD-2.3.0rc2/src/IntuneCD/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:26.579439 IntuneCD-2.3.0rc2/src/IntuneCD/backup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:26.583439 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/Applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/AuthenticationFlows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/AuthenticationMethods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/AuthorizationPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/B2B.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/DeviceRegistration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/Domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/ExternalIdentities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/GroupSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/RoamingSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/SSPR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/SecurityDefaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:26.587439 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/APNs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/Activationlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/AppConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/AppProtection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/AppleEnrollmentProfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/Applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/AutopilotDevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/Compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/CompliancePartner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ComplianceScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ConditionalAccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/CustomAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/DeviceCategories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/DeviceCompliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/DeviceConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/DeviceManagementSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/EnrollmentConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/EnrollmentStatusPage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/Filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/GroupPolicyConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ManagedGooglePlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ManagementIntents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ManagementPartner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/NotificationTemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/PowershellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ProactiveRemediation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/RemoteAssistancePartner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ReusableSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/Roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ScopeTags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/SettingsCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ShellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/VolumePurchaseProgram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/WindowsDriverUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/WindowsEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/WindowsFeatureUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/WindowsQualityUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup_entra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/backup_intune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/document_entra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/document_intune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:26.591439 IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/BaseBackupModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36404 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/BaseGraphModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/BaseUpdateModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/IntuneCDBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/assignment_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17908 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/documentation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/get_accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/get_authparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/process_audit_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/process_scope_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/run_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/run_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/run_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:26.591439 IntuneCD-2.3.0rc2/src/IntuneCD/update/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:26.591439 IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/AuthenticationFlows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/AuthenticationMethodsConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/AuthenticationMethodsPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/AuthorizationPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/B2B.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/DeviceRegistration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/Domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/ExternalIdentitiesPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/GroupSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/RoamingSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/SSPR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/SecurityDefaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:26.599439 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/AppConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/AppProtection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/AppleEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/Compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/ComplianceScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/ConditionalAccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/CustomAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/DeviceCategories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/DeviceCompliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/DeviceConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/DeviceManagementSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/EnrollmentConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/EnrollmentStatusPage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/Filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23308 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/GroupPolicyConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/ManagementIntents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/NotificationTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/PowerShellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/ProactiveRemediation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/ReusableSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/Roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/ScopeTags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/SettingsCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/ShellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/WindowsDriverUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/WindowsEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/WindowsFeatureUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/WindowsQualityUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update_entra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/src/IntuneCD/update_intune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:26.599439 IntuneCD-2.3.0rc2/src/IntuneCD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-03-25 13:16:26.000000 IntuneCD-2.3.0rc2/src/IntuneCD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-03-25 13:16:26.000000 IntuneCD-2.3.0rc2/src/IntuneCD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 13:16:26.000000 IntuneCD-2.3.0rc2/src/IntuneCD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-25 13:16:26.000000 IntuneCD-2.3.0rc2/src/IntuneCD.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-25 13:16:26.000000 IntuneCD-2.3.0rc2/src/IntuneCD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-25 13:16:26.000000 IntuneCD-2.3.0rc2/src/IntuneCD.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:26.599439 IntuneCD-2.3.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/tests/test_documentation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-03-25 13:16:20.000000 IntuneCD-2.3.0rc2/tests/test_get_authparams.py
```

### Comparing `IntuneCD-2.3.0rc1/LICENSE` & `IntuneCD-2.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/PKG-INFO` & `IntuneCD-2.3.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 2.3.0rc1
+Version: 2.3.0rc2
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-2.3.0rc1/README.md` & `IntuneCD-2.3.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/setup.cfg` & `IntuneCD-2.3.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = IntuneCD
-version = 2.3.0.rc1
+version = 2.3.0.rc2
 author = Tobias Almén
 author_email = almenscorner@outlook.com
 description = Tool to backup and update configurations in Intune
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/almenscorner/IntuneCD
 project_urls =
```

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/Applications.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/Applications.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/AuthenticationFlows.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/AuthenticationFlows.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/AuthenticationMethods.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/AuthenticationMethods.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/AuthorizationPolicy.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/AuthorizationPolicy.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/B2B.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/B2B.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/DeviceRegistration.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/DeviceRegistration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/Domains.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/Domains.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/ExternalIdentities.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/ExternalIdentities.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/GroupSettings.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/GroupSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/RoamingSettings.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/RoamingSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/SSPR.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/SSPR.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Entra/SecurityDefaults.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Entra/SecurityDefaults.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/APNs.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/APNs.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/Activationlock.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/Activationlock.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/AppConfiguration.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/AppConfiguration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+import json
+
 from ...intunecdlib.BaseBackupModule import BaseBackupModule
 
 
 class AppConfigurationBackupModule(BaseBackupModule):
     """A class used to backup Intune App Configurations
 
     Attributes:
@@ -53,16 +55,17 @@
                         endpoint=self.endpoint + self.APP_ENDPOINT + "/" + app
                     )
                     if app_data:
                         item.pop("targetedMobileApps")
                         item["targetedMobileApps"] = {}
                         item["targetedMobileApps"]["appName"] = app_data["displayName"]
                         item["targetedMobileApps"]["type"] = app_data["@odata.type"]
-            if item.get("payloadJson"):
-                item["payloadJson"] = self.decode_base64(item["payloadJson"])
+                if item.get("payloadJson"):
+                    item["payloadJson"] = self.decode_base64(item["payloadJson"])
+                    item["payloadJson"] = json.loads(item["payloadJson"])
 
         try:
             self.results = self.process_data(
                 data=self.graph_data["value"],
                 filetype=self.filetype,
                 path=self.path,
                 name_key="displayName",
```

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/AppProtection.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/AppProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/AppleEnrollmentProfiles.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/AppleEnrollmentProfiles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/Applications.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/Applications.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,19 @@
         """The main method to backup the Applications
 
         Returns:
             dict[str, any]: The results of the backup
         """
         try:
             self.graph_data = self.make_graph_request(
-                endpoint=self.endpoint + self.CONFIG_ENDPOINT
+                endpoint=self.endpoint + self.CONFIG_ENDPOINT,
+                params={
+                    "$filter": "(microsoft.graph.managedApp/appAvailability) eq null or (microsoft.graph.managedApp/appAvailability) "
+                    "eq 'lineOfBusiness' or isAssigned eq true"
+                },
             )
         except Exception as e:
             self.log(
                 tag="error",
                 msg=f"Error getting Application data from {self.endpoint + self.CONFIG_ENDPOINT}: {e}",
             )
             return None
@@ -59,14 +63,15 @@
         )
 
         # as we must process each app individually, get the audit data up front
         self.audit_data = self.make_audit_request(self.audit_filter)
 
         for app in self.graph_data["value"]:
             self.platform_path = ""
+            app.pop("description", None)
             scope_tag_data = [v for v in scope_tag_responses if app["id"] == v["id"]]
             if scope_tag_data:
                 app["roleScopeTagIds"] = scope_tag_data[0]["roleScopeTagIds"]
 
             def generate_app_name(app, app_type, suffix=""):
                 try:
                     return app["displayName"] + "_" + app_type + suffix
```

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/AutopilotDevices.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/AutopilotDevices.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/Compliance.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/Compliance.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,16 @@
             return None
 
         for item in self.graph_data["value"]:
             # Remove the keys that are not needed from each scheduledActionsForRule
             for rule in item["scheduledActionsForRule"]:
                 self.remove_keys(rule)
                 self._get_notification_template(rule)
+                for action in rule["scheduledActionConfigurations"]:
+                    self.remove_keys(action)
 
             # If there is a deviceCompliancePolicyScript, get the name of the script
             if item.get("deviceCompliancePolicyScript", None):
                 # Get the name of the script
                 script_name = self.make_graph_request(
                     self.endpoint
                     + "/beta/deviceManagement/deviceComplianceScripts/"
```

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/CompliancePartner.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/CompliancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ComplianceScripts.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ComplianceScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ConditionalAccess.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ConditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/CustomAttributes.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/CustomAttributes.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/DeviceCategories.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/DeviceCategories.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/DeviceCompliance.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/DeviceCompliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/DeviceConfigurations.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/DeviceConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/DeviceManagementSettings.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/DeviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/EnrollmentConfigurations.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/EnrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/EnrollmentStatusPage.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/EnrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/Filters.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/Filters.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/GroupPolicyConfigurations.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/GroupPolicyConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ManagedGooglePlay.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ManagedGooglePlay.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ManagementIntents.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ManagementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ManagementPartner.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ManagementPartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/NotificationTemplates.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/NotificationTemplates.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/PowershellScripts.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/PowershellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ProactiveRemediation.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ProactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/RemoteAssistancePartner.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/RemoteAssistancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ReusableSettings.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ReusableSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/Roles.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/Roles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ScopeTags.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ScopeTags.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/SettingsCatalog.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/SettingsCatalog.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/ShellScripts.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/ShellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/VolumePurchaseProgram.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/VolumePurchaseProgram.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/WindowsDriverUpdates.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/WindowsDriverUpdates.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/WindowsEnrollmentProfile.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/WindowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/WindowsFeatureUpdates.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/WindowsFeatureUpdates.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup/Intune/WindowsQualityUpdates.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup/Intune/WindowsQualityUpdates.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup_entra.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup_entra.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/backup_intune.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/backup_intune.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/document_entra.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/document_entra.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/document_intune.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/document_intune.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/BaseBackupModule.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/BaseBackupModule.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/BaseGraphModule.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/BaseGraphModule.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/BaseUpdateModule.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/BaseUpdateModule.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/IntuneCDBase.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/IntuneCDBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
     def remove_keys(self, data: dict):
         """
         This function removes keys from the data.
         :param data: The data to remove keys from.
         :return: The data with removed keys.
         """
-        self.exclude = []
 
         keys = {
             "id",
             "version",
             "topicIdentifier",
             "certificate",
             "createdDateTime",
```

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/archive.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/assignment_report.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/assignment_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/documentation_functions.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/get_accesstoken.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/get_accesstoken.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/get_authparams.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/process_audit_data.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/process_audit_data.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/intunecdlib/process_scope_tags.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/intunecdlib/process_scope_tags.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/run_backup.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/run_backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,20 +153,14 @@
     parser.add_argument(
         "-ap",
         "--autopilot",
         help="If set, a record of autopilot devices will be saved",
         action="store_true",
     )
     parser.add_argument(
-        "-f",
-        "--frontend",
-        help="***This parameter is deprecated and will be removed in a future release***",
-        type=str,
-    )
-    parser.add_argument(
         "--prefix",
         help="When set, only backs up configurations whose name starts with the configured prefix",
         type=str,
     )
     parser.add_argument(
         "--append-id",
         help="When set, the id of the configuration will be appended to the name of the exported file",
@@ -286,22 +280,14 @@
         ]
 
         move_to_archive(path, created_files, output)
 
         return config_count
 
     if args.output == "json" or args.output == "yaml":
-        if args.frontend:
-            print(
-                "***The --forntend argument is deprecated and will be removed in a future release***"
-            )
-            print(
-                "***Please migrate to --intunecdmonitor instead, see https;//github.com/almenscorner/intunecd/wiki***"
-            )
-
         if token is None:
             raise Exception("Token is empty, please check os.environ variables")
 
         if args.exclude:
             exclude = args.exclude
         else:
             exclude = []
```

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/run_documentation.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/run_documentation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/run_update.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/run_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,20 +148,14 @@
     )
     parser.add_argument(
         "--intunecdmonitor",
         help="When this parameter is set, the script is run in the IntuneCDMonitor context",
         action="store_true",
     )
     parser.add_argument(
-        "-f",
-        "--frontend",
-        help="***This parameter is deprecated and will be removed in a future release***",
-        type=str,
-    )
-    parser.add_argument(
         "--entraupdate",
         help="When this parameter is set, the script will also update Entra configurations",
         action="store_true",
     )
     parser.add_argument(
         "--scopes",
         help="The scopes to use when obtaining an access token interactively separated by space. Only used when using interactive auth. Default is: DeviceManagementApps.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementRBAC.ReadWrite.All, Group.Read.All, Policy.ReadWrite.ConditionalAccess, Policy.Read.All",
@@ -256,22 +250,14 @@
                 diff_count += config.get("count")
 
         return diff_count, diff_summary
 
     if token is None:
         raise Exception("Token is empty, please check os.environ variables")
     else:
-        if args.frontend:
-            print(
-                "***The --frontend argument is deprecated and will be removed in a future release***"
-            )
-            print(
-                "***Please migrate to --intunecdmonitor instead, see https;//github.com/almenscorner/intunecd/wiki***"
-            )
-
         if args.exclude:
             exclude = args.exclude
         else:
             exclude = []
 
         if args.report:
             print("***Running in report mode, no updates will be pushed to Intune***")
```

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/AuthenticationFlows.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/AuthenticationFlows.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/AuthenticationMethodsConfigurations.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/AuthenticationMethodsConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/AuthenticationMethodsPolicy.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/AuthenticationMethodsPolicy.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/AuthorizationPolicy.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/AuthorizationPolicy.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/B2B.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/B2B.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/DeviceRegistration.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/DeviceRegistration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/Domains.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/Domains.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/ExternalIdentitiesPolicy.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/ExternalIdentitiesPolicy.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/GroupSettings.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/GroupSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/RoamingSettings.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/RoamingSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/SSPR.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/SSPR.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Entra/SecurityDefaults.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Entra/SecurityDefaults.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/AppConfiguration.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/AppConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/AppProtection.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/AppProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/AppleEnrollmentProfile.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/AppleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/Compliance.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/Compliance.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,17 +256,17 @@
                     },
                 )
                 if notification_template["value"]:
                     action["notificationTemplateId"] = notification_template["value"][
                         0
                     ]["id"]
                 else:
-                    action[
-                        "notificationTemplateId"
-                    ] = "00000000-0000-0000-0000-000000000000"
+                    action["notificationTemplateId"] = (
+                        "00000000-0000-0000-0000-000000000000"
+                    )
 
                 action.pop("notificationTemplateName")
 
         return rule
 
     def main(self) -> dict[str, any]:
         """The main method to update the Intune data"""
@@ -318,14 +318,20 @@
                     new_intune_data = []
                     for item in intune_data["value"]:
                         item = self._remove_compliance_keys(item)
                         new_intune_data.append(item)
                     intune_data["value"] = new_intune_data
                     repo_data = self._remove_compliance_keys(repo_data)
 
+                    for item in intune_data["value"]:
+                        for action in item["scheduledActionsForRule"][0][
+                            "scheduledActionConfigurations"
+                        ]:
+                            self.remove_keys(action)
+
                     try:
                         self.process_update(
                             downstream_data=intune_data["value"],
                             repo_data=repo_data,
                             method="patch",
                             status_code=204,
                             config_endpoint=self.CONFIG_ENDPOINT,
```

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/ComplianceScripts.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/ComplianceScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/ConditionalAccess.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/ConditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/CustomAttributes.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/CustomAttributes.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/DeviceCategories.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/DeviceCategories.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/DeviceCompliance.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/DeviceCompliance.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,30 +25,34 @@
         self.path = f"{self.path}/Compliance Policies/Policies/"
         self.assignment_endpoint = "/deviceManagement/deviceCompliancePolicies/"
         self.assignment_extra_url = "/assign"
         self.exclude_paths = [
             "root['assignments']",
             "root['scheduledActionsForRule']",
             "root['deviceComplianceScriptName']",
+            "root['scheduledActionConfigurations']",
+            "root['scheduledActionConfigurations'][0]['id']",
+            "root['assignments']",
+            "root['scheduledActionsForRule'][0]['scheduledActionConfigurations']",
         ]
         self.params = {
             "expand": "scheduledActionsForRule($expand=scheduledActionConfigurations)"
         }
 
     def _set_compliance_script_id(self, data: dict) -> dict[str, any]:
         compliance_script_id = self.make_graph_request(
             endpoint=self.endpoint + "/beta/deviceManagement/deviceComplianceScripts",
             params={
                 "$filter": f"displayName eq '{data['deviceComplianceScriptName']}'"
             },
         )
         if compliance_script_id.get("value"):
-            data["deviceCompliancePolicyScript"][
-                "deviceComplianceScriptId"
-            ] = compliance_script_id["value"][0]["id"]
+            data["deviceCompliancePolicyScript"]["deviceComplianceScriptId"] = (
+                compliance_script_id["value"][0]["id"]
+            )
 
             return data
 
         return False
 
     def _compliance_script_check(self, repo_data: dict) -> dict[str, any]:
         """Checks if the detection script exists
@@ -120,17 +124,17 @@
                     },
                 )
                 if notification_template["value"]:
                     action["notificationTemplateId"] = notification_template["value"][
                         0
                     ]["id"]
                 else:
-                    action[
-                        "notificationTemplateId"
-                    ] = "00000000-0000-0000-0000-000000000000"
+                    action["notificationTemplateId"] = (
+                        "00000000-0000-0000-0000-000000000000"
+                    )
 
                 action.pop("notificationTemplateName")
 
         return rule
 
     def main(self) -> dict[str, any]:
         """The main method to update the Intune data"""
@@ -164,14 +168,20 @@
                     repo_data = self._compliance_script_check(repo_data)
                     if repo_data is False:
                         continue
 
                     for rule in repo_data.get("scheduledActionsForRule"):
                         self._get_notification_template_id(rule)
 
+                    for item in intune_data["value"]:
+                        for action in item["scheduledActionsForRule"][0][
+                            "scheduledActionConfigurations"
+                        ]:
+                            self.remove_keys(action)
+
                     try:
                         self.process_update(
                             downstream_data=intune_data["value"],
                             repo_data=repo_data,
                             method="patch",
                             status_code=204,
                             config_endpoint=self.CONFIG_ENDPOINT,
```

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/DeviceConfigurations.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/DeviceConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/DeviceManagementSettings.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/DeviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/EnrollmentConfigurations.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/EnrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/EnrollmentStatusPage.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/EnrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/Filters.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/Filters.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/GroupPolicyConfigurations.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/GroupPolicyConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/ManagementIntents.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/ManagementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/NotificationTemplate.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/NotificationTemplate.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
         Args:
             *args: The positional arguments to pass to the base class's __init__ method.
             **kwargs: The keyword arguments to pass to the base class's __init__ method.
         """
         super().__init__(*args, **kwargs)
         self.path = f"{self.path}/Compliance Policies/Message Templates/"
-        self.config_type = "Notification Template"
         self.handle_assignment = False
         self.params = {"$expand": "localizedNotificationMessages"}
         self.exclude_paths = [
             "root['defaultLocale']",
             "root['localizedNotificationMessages']",
             "root['localizedNotificationMessages@odata.context']",
         ]
@@ -44,15 +43,17 @@
             repo_data (dict[str, any]): The repo data
         """
         for intune_locale, repo_locale in zip(
             intune_data["localizedNotificationMessages"],
             repo_data["localizedNotificationMessages"],
         ):
             self.name = repo_locale.get("locale")
-            if locale_diff := self.get_diffs(intune_locale, repo_locale, None):
+            if locale_diff := self.get_diffs(
+                intune_locale, repo_locale, "root['isDefault']"
+            ):
                 self.config_type = "Notification Template Locale"
                 data = repo_data.copy()
                 data.pop("isDefault", None)
                 data.pop("locale", None)
                 self.update_downstream_data(
                     self.endpoint
                     + self.CONFIG_ENDPOINT
@@ -85,14 +86,19 @@
             if (
                 intune_locale.get("isDefault") != repo_locale.get("isDefault")
                 and repo_locale.get("isDefault") is not None
             ):
                 if repo_locale["isDefault"] is False:
                     repo_locale.pop("isDefault", None)
 
+                self.log(
+                    msg=f"Updating isDefault for {self.name} to {repo_locale.get('isDefault')}",
+                    tag="info",
+                )
+
                 self.update_downstream_data(
                     self.endpoint
                     + self.CONFIG_ENDPOINT
                     + self.downstream_id
                     + "/"
                     + "localizedNotificationMessages"
                     + "/"
@@ -134,14 +140,15 @@
                 for val in intune_data["value"]
                 if val["displayName"] != "EnrollmentNotificationInternalMEO"
             ]
 
             for filename in os.listdir(self.path):
                 # Reset the paramters
                 self.create_request = None
+                self.config_type = "Notification Template"
 
                 repo_data = self.load_repo_data(filename)
                 if repo_data:
                     self.match_info = {
                         "displayName": repo_data.get("displayName"),
                     }
                     self.name = repo_data.get("displayName")
```

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/PowerShellScripts.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/PowerShellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/ProactiveRemediation.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/ProactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/ReusableSettings.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/ReusableSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/Roles.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/Roles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/ScopeTags.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/ScopeTags.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/SettingsCatalog.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/SettingsCatalog.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/ShellScripts.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/ShellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/WindowsDriverUpdates.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/WindowsDriverUpdates.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/WindowsEnrollmentProfile.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/WindowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/WindowsFeatureUpdates.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/WindowsFeatureUpdates.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update/Intune/WindowsQualityUpdates.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update/Intune/WindowsQualityUpdates.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update_entra.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update_entra.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD/update_intune.py` & `IntuneCD-2.3.0rc2/src/IntuneCD/update_intune.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD.egg-info/PKG-INFO` & `IntuneCD-2.3.0rc2/src/IntuneCD.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 2.3.0rc1
+Version: 2.3.0rc2
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-2.3.0rc1/src/IntuneCD.egg-info/SOURCES.txt` & `IntuneCD-2.3.0rc2/src/IntuneCD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/tests/test_archive.py` & `IntuneCD-2.3.0rc2/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/tests/test_documentation_functions.py` & `IntuneCD-2.3.0rc2/tests/test_documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-2.3.0rc1/tests/test_get_authparams.py` & `IntuneCD-2.3.0rc2/tests/test_get_authparams.py`

 * *Files identical despite different names*

