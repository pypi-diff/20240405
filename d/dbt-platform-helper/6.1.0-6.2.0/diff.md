# Comparing `tmp/dbt_platform_helper-6.1.0.tar.gz` & `tmp/dbt_platform_helper-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_platform_helper-6.1.0.tar", max compression
+gzip compressed data, was "dbt_platform_helper-6.2.0.tar", max compression
```

## Comparing `dbt_platform_helper-6.1.0.tar` & `dbt_platform_helper-6.2.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     1090 2024-03-12 15:16:39.913884 dbt_platform_helper-6.1.0/LICENSE
--rw-r--r--   0        0        0    18895 2024-03-13 18:27:32.470268 dbt_platform_helper-6.1.0/dbt_platform_helper/COMMANDS.md
--rw-r--r--   0        0        0     1763 2024-03-13 16:12:19.742509 dbt_platform_helper-6.1.0/dbt_platform_helper/README.md
--rw-r--r--   0        0        0        0 2024-03-13 16:12:19.742560 dbt_platform_helper-6.1.0/dbt_platform_helper/__init__.py
--rw-r--r--   0        0        0     3842 2024-03-13 16:12:19.743163 dbt_platform_helper-6.1.0/dbt_platform_helper/addon-plans.yml
--rw-r--r--   0        0        0     1278 2024-03-13 16:12:19.743509 dbt_platform_helper-6.1.0/dbt_platform_helper/addons-template-map.yml
--rw-r--r--   0        0        0        0 2024-03-13 16:12:19.743652 dbt_platform_helper-6.1.0/dbt_platform_helper/commands/__init__.py
--rw-r--r--   0        0        0     9957 2024-03-13 16:12:19.743829 dbt_platform_helper-6.1.0/dbt_platform_helper/commands/application.py
--rwxr-xr-x   0        0        0    10582 2024-03-13 16:12:19.743961 dbt_platform_helper-6.1.0/dbt_platform_helper/commands/bootstrap.py
--rwxr-xr-x   0        0        0     3226 2024-03-13 16:12:19.744073 dbt_platform_helper-6.1.0/dbt_platform_helper/commands/check_cloudformation.py
--rw-r--r--   0        0        0    11192 2024-03-13 16:12:19.744379 dbt_platform_helper-6.1.0/dbt_platform_helper/commands/codebase.py
--rw-r--r--   0        0        0    12855 2024-03-13 16:12:19.744515 dbt_platform_helper-6.1.0/dbt_platform_helper/commands/conduit.py
--rw-r--r--   0        0        0     7949 2024-03-13 16:12:19.744888 dbt_platform_helper-6.1.0/dbt_platform_helper/commands/config.py
--rwxr-xr-x   0        0        0    14473 2024-03-13 16:12:19.745053 dbt_platform_helper-6.1.0/dbt_platform_helper/commands/copilot.py
--rwxr-xr-x   0        0        0    34465 2024-03-13 16:12:19.745227 dbt_platform_helper-6.1.0/dbt_platform_helper/commands/dns.py
--rw-r--r--   0        0        0     8670 2024-03-13 16:12:19.745382 dbt_platform_helper-6.1.0/dbt_platform_helper/commands/environment.py
--rw-r--r--   0        0        0      722 2024-03-13 16:12:19.745690 dbt_platform_helper-6.1.0/dbt_platform_helper/commands/generate.py
--rw-r--r--   0        0        0     6218 2024-03-13 18:22:31.207492 dbt_platform_helper-6.1.0/dbt_platform_helper/commands/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-13 16:12:19.745940 dbt_platform_helper-6.1.0/dbt_platform_helper/custom_resources/__init__.py
--rw-r--r--   0        0        0     2396 2024-03-13 16:12:19.746058 dbt_platform_helper-6.1.0/dbt_platform_helper/custom_resources/s3_object.py
--rw-r--r--   0        0        0      346 2024-03-13 16:12:19.746158 dbt_platform_helper-6.1.0/dbt_platform_helper/default-addons.yml
--rw-r--r--   0        0        0      499 2024-03-13 16:12:19.746266 dbt_platform_helper-6.1.0/dbt_platform_helper/exceptions.py
--rw-r--r--   0        0        0      369 2024-03-13 16:12:19.746520 dbt_platform_helper-6.1.0/dbt_platform_helper/jinja2_tags.py
--rw-r--r--   0        0        0      158 2024-03-13 16:12:19.746719 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/.copilot/config.yml
--rwxr-xr-x   0        0        0      164 2024-03-13 16:12:19.746815 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/.copilot/image_build_run.sh
--rwxr-xr-x   0        0        0      121 2024-03-13 16:12:19.746958 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/.copilot/phases/build.sh
--rwxr-xr-x   0        0        0      123 2024-03-13 16:12:19.747039 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/.copilot/phases/install.sh
--rwxr-xr-x   0        0        0      126 2024-03-13 16:12:19.747114 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/.copilot/phases/post_build.sh
--rwxr-xr-x   0        0        0      125 2024-03-13 16:12:19.747208 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
--rw-r--r--   0        0        0     1081 2024-03-13 16:12:19.747394 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/COMMANDS.md.jinja
--rw-r--r--   0        0        0      622 2024-03-13 16:12:19.747525 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addon-instructions.txt
--rw-r--r--   0        0        0      412 2024-03-13 16:12:19.747690 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/README.md
--rw-r--r--   0        0        0      734 2024-03-13 16:12:19.748067 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml
--rw-r--r--   0        0        0    26381 2024-03-13 16:12:19.748258 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
--rw-r--r--   0        0        0     6064 2024-03-13 16:12:19.748411 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/monitoring.yml
--rw-r--r--   0        0        0    10655 2024-03-13 16:12:19.748772 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/opensearch.yml
--rw-r--r--   0        0        0    25624 2024-03-13 16:12:19.748923 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml
--rw-r--r--   0        0        0     7503 2024-03-13 16:12:19.749081 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml
--rw-r--r--   0        0        0     7626 2024-03-13 16:12:19.749218 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/s3.yml
--rw-r--r--   0        0        0     3662 2024-03-13 16:12:19.749488 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/vpc.yml
--rw-r--r--   0        0        0      956 2024-03-13 16:12:19.749648 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
--rw-r--r--   0        0        0     2134 2024-03-13 16:12:19.749747 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml
--rw-r--r--   0        0        0      893 2024-03-13 16:12:19.749847 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
--rw-r--r--   0        0        0     1836 2024-03-13 16:12:19.749940 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json
--rw-r--r--   0        0        0      197 2024-03-13 16:12:19.750039 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/create-codebuild-role.json
--rw-r--r--   0        0        0     1180 2024-03-13 16:12:19.750134 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json
--rw-r--r--   0        0        0      691 2024-03-13 16:12:19.750293 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/manifest.yml
--rw-r--r--   0        0        0      169 2024-03-13 16:12:19.750427 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/overrides/.gitignore
--rw-r--r--   0        0        0      439 2024-03-13 16:12:19.750521 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/overrides/README.md
--rw-r--r--   0        0        0      284 2024-03-13 16:12:19.750661 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/overrides/bin/override.ts
--rw-r--r--   0        0        0      339 2024-03-13 16:12:19.750744 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/overrides/cdk.json
--rw-r--r--   0        0        0     1760 2024-03-13 16:12:19.750832 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
--rw-r--r--   0        0        0   150965 2024-03-13 16:12:19.751379 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/overrides/package-lock.json
--rw-r--r--   0        0        0      534 2024-03-13 16:12:19.751519 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/overrides/package.json
--rw-r--r--   0        0        0     1906 2024-03-13 16:12:19.751623 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/overrides/stack.ts
--rw-r--r--   0        0        0      710 2024-03-13 16:12:19.751717 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/overrides/tsconfig.json
--rw-r--r--   0        0        0     1959 2024-03-13 18:22:31.207764 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
--rw-r--r--   0        0        0      169 2024-03-13 16:12:19.752063 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
--rw-r--r--   0        0        0      227 2024-03-13 16:12:19.752200 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
--rw-r--r--   0        0        0      287 2024-03-13 16:12:19.752285 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
--rw-r--r--   0        0        0      781 2024-03-13 16:12:19.752365 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
--rw-r--r--   0        0        0      339 2024-03-13 16:12:19.752442 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
--rw-r--r--   0        0        0   148134 2024-03-13 16:12:19.752801 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
--rw-r--r--   0        0        0      534 2024-03-13 16:12:19.753240 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
--rw-r--r--   0        0        0    20142 2024-03-13 18:22:31.208105 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
--rw-r--r--   0        0        0      651 2024-03-13 16:12:19.753580 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
--rw-r--r--   0        0        0     1205 2024-03-13 18:22:31.208323 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
--rw-r--r--   0        0        0     3178 2024-03-13 16:12:19.753991 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
--rw-r--r--   0        0        0     1778 2024-03-13 16:12:19.754071 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml
--rw-r--r--   0        0        0      617 2024-03-13 16:12:19.754191 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
--rw-r--r--   0        0        0      741 2024-03-13 16:12:19.754357 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html
--rw-r--r--   0        0        0      783 2024-03-13 16:12:19.754440 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
--rw-r--r--   0        0        0     2881 2024-03-13 18:22:31.208540 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/svc/manifest-backend.yml
--rw-r--r--   0        0        0     3921 2024-03-13 18:22:31.208713 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/svc/manifest-public.yml
--rw-r--r--   0        0        0      386 2024-03-13 16:12:19.754753 dbt_platform_helper-6.1.0/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
--rw-r--r--   0        0        0        0 2024-03-13 16:12:19.754829 dbt_platform_helper-6.1.0/dbt_platform_helper/utils/__init__.py
--rw-r--r--   0        0        0     3907 2024-03-13 16:12:19.754937 dbt_platform_helper-6.1.0/dbt_platform_helper/utils/application.py
--rw-r--r--   0        0        0    10704 2024-03-13 18:22:31.209079 dbt_platform_helper-6.1.0/dbt_platform_helper/utils/aws.py
--rw-r--r--   0        0        0     2943 2024-03-13 16:12:19.755141 dbt_platform_helper-6.1.0/dbt_platform_helper/utils/click.py
--rw-r--r--   0        0        0     1053 2024-03-13 16:12:19.755218 dbt_platform_helper-6.1.0/dbt_platform_helper/utils/cloudformation.py
--rw-r--r--   0        0        0      484 2024-03-13 16:12:19.755292 dbt_platform_helper-6.1.0/dbt_platform_helper/utils/cloudfoundry.py
--rw-r--r--   0        0        0     1720 2024-03-13 16:12:19.755368 dbt_platform_helper-6.1.0/dbt_platform_helper/utils/files.py
--rw-r--r--   0        0        0      304 2024-03-13 16:12:19.755442 dbt_platform_helper-6.1.0/dbt_platform_helper/utils/git.py
--rw-r--r--   0        0        0      507 2024-03-13 16:12:19.755522 dbt_platform_helper-6.1.0/dbt_platform_helper/utils/manifests.py
--rw-r--r--   0        0        0      115 2024-03-13 16:12:19.755593 dbt_platform_helper-6.1.0/dbt_platform_helper/utils/messages.py
--rw-r--r--   0        0        0      469 2024-03-13 16:12:19.755667 dbt_platform_helper-6.1.0/dbt_platform_helper/utils/template.py
--rw-r--r--   0        0        0    16265 2024-03-13 18:22:31.209511 dbt_platform_helper-6.1.0/dbt_platform_helper/utils/validation.py
--rw-r--r--   0        0        0     6408 2024-03-13 16:12:19.756081 dbt_platform_helper-6.1.0/dbt_platform_helper/utils/versioning.py
--rwxr-xr-x   0        0        0     1936 2024-03-13 16:12:19.756572 dbt_platform_helper-6.1.0/platform_helper.py
--rw-r--r--   0        0        0     1362 2024-03-13 18:26:30.814038 dbt_platform_helper-6.1.0/pyproject.toml
--rw-r--r--   0        0        0     3273 1970-01-01 00:00:00.000000 dbt_platform_helper-6.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-03-12 15:16:39.913884 dbt_platform_helper-6.2.0/LICENSE
+-rw-r--r--   0        0        0    19003 2024-04-05 09:36:23.425488 dbt_platform_helper-6.2.0/dbt_platform_helper/COMMANDS.md
+-rw-r--r--   0        0        0     1762 2024-04-05 09:30:20.384763 dbt_platform_helper-6.2.0/dbt_platform_helper/README.md
+-rw-r--r--   0        0        0        0 2024-03-14 13:13:32.491170 dbt_platform_helper-6.2.0/dbt_platform_helper/__init__.py
+-rw-r--r--   0        0        0     3842 2024-03-14 13:13:32.492175 dbt_platform_helper-6.2.0/dbt_platform_helper/addon-plans.yml
+-rw-r--r--   0        0        0     1278 2024-03-14 13:13:32.492883 dbt_platform_helper-6.2.0/dbt_platform_helper/addons-template-map.yml
+-rw-r--r--   0        0        0        0 2024-03-14 13:13:32.493207 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/__init__.py
+-rw-r--r--   0        0        0     9957 2024-03-14 13:13:32.494282 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/application.py
+-rwxr-xr-x   0        0        0    10582 2024-03-14 13:13:32.494998 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/bootstrap.py
+-rwxr-xr-x   0        0        0     3226 2024-03-14 13:13:32.495667 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/check_cloudformation.py
+-rw-r--r--   0        0        0    11192 2024-03-14 13:13:32.496393 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/codebase.py
+-rw-r--r--   0        0        0    12855 2024-03-14 13:13:32.497098 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/conduit.py
+-rw-r--r--   0        0        0     7949 2024-03-14 13:13:32.498464 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/config.py
+-rwxr-xr-x   0        0        0    14591 2024-04-05 09:30:20.385437 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/copilot.py
+-rwxr-xr-x   0        0        0    35037 2024-04-05 09:30:20.385728 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/dns.py
+-rw-r--r--   0        0        0     8670 2024-03-14 13:13:32.500669 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/environment.py
+-rw-r--r--   0        0        0      722 2024-03-14 13:13:32.501961 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/generate.py
+-rw-r--r--   0        0        0     6218 2024-03-14 13:13:32.503292 dbt_platform_helper-6.2.0/dbt_platform_helper/commands/pipeline.py
+-rw-r--r--   0        0        0        0 2024-03-14 13:13:32.503639 dbt_platform_helper-6.2.0/dbt_platform_helper/custom_resources/__init__.py
+-rw-r--r--   0        0        0     2396 2024-03-14 13:13:32.504820 dbt_platform_helper-6.2.0/dbt_platform_helper/custom_resources/s3_object.py
+-rw-r--r--   0        0        0      346 2024-03-14 13:13:32.505501 dbt_platform_helper-6.2.0/dbt_platform_helper/default-addons.yml
+-rw-r--r--   0        0        0      499 2024-03-14 13:13:32.506174 dbt_platform_helper-6.2.0/dbt_platform_helper/exceptions.py
+-rw-r--r--   0        0        0      369 2024-03-14 13:13:32.507457 dbt_platform_helper-6.2.0/dbt_platform_helper/jinja2_tags.py
+-rw-r--r--   0        0        0      158 2024-03-14 13:13:32.508797 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/.copilot/config.yml
+-rwxr-xr-x   0        0        0      164 2024-03-14 13:13:32.509606 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/.copilot/image_build_run.sh
+-rwxr-xr-x   0        0        0      121 2024-03-14 13:13:32.510795 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/.copilot/phases/build.sh
+-rwxr-xr-x   0        0        0      123 2024-03-14 13:13:32.511480 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/.copilot/phases/install.sh
+-rwxr-xr-x   0        0        0      126 2024-03-14 13:13:32.512145 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/.copilot/phases/post_build.sh
+-rwxr-xr-x   0        0        0      125 2024-03-14 13:13:32.512941 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
+-rw-r--r--   0        0        0     1081 2024-03-14 13:13:32.513655 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/COMMANDS.md.jinja
+-rw-r--r--   0        0        0      622 2024-03-14 13:13:32.514385 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addon-instructions.txt
+-rw-r--r--   0        0        0      412 2024-03-14 13:13:32.515427 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/README.md
+-rw-r--r--   0        0        0      734 2024-03-14 13:13:32.516450 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml
+-rw-r--r--   0        0        0    26381 2024-03-14 13:13:32.517134 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
+-rw-r--r--   0        0        0     6064 2024-03-18 09:47:04.985223 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/monitoring.yml
+-rw-r--r--   0        0        0    10853 2024-04-05 09:30:20.386403 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/opensearch.yml
+-rw-r--r--   0        0        0    25624 2024-03-14 13:13:32.519316 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml
+-rw-r--r--   0        0        0     7613 2024-04-05 09:30:20.387232 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml
+-rw-r--r--   0        0        0     7626 2024-03-14 13:13:32.520784 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/s3.yml
+-rw-r--r--   0        0        0     3662 2024-03-14 13:13:32.521623 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/vpc.yml
+-rw-r--r--   0        0        0      956 2024-03-14 13:13:32.522636 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
+-rw-r--r--   0        0        0     2134 2024-03-14 13:13:32.523308 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml
+-rw-r--r--   0        0        0      893 2024-03-14 13:13:32.523980 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
+-rw-r--r--   0        0        0     1836 2024-03-14 13:13:32.524657 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json
+-rw-r--r--   0        0        0      197 2024-03-14 13:13:32.525328 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/create-codebuild-role.json
+-rw-r--r--   0        0        0     1180 2024-03-14 13:13:32.525988 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json
+-rw-r--r--   0        0        0      691 2024-03-14 13:13:32.526569 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/manifest.yml
+-rw-r--r--   0        0        0      169 2024-03-14 13:13:32.527131 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/.gitignore
+-rw-r--r--   0        0        0      439 2024-03-14 13:13:32.527546 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/README.md
+-rw-r--r--   0        0        0      284 2024-03-14 13:13:32.528133 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/bin/override.ts
+-rw-r--r--   0        0        0      339 2024-03-14 13:13:32.528741 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/cdk.json
+-rw-r--r--   0        0        0     1760 2024-03-14 13:13:32.529367 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
+-rw-r--r--   0        0        0   150965 2024-03-14 13:13:32.530032 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/package-lock.json
+-rw-r--r--   0        0        0      534 2024-03-14 13:13:32.530472 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/package.json
+-rw-r--r--   0        0        0     1906 2024-03-14 13:13:32.531017 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/stack.ts
+-rw-r--r--   0        0        0      710 2024-03-14 13:13:32.531424 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/tsconfig.json
+-rw-r--r--   0        0        0     1959 2024-03-14 13:13:32.532600 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
+-rw-r--r--   0        0        0      169 2024-03-14 13:13:32.532763 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
+-rw-r--r--   0        0        0      227 2024-03-14 13:13:32.532939 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
+-rw-r--r--   0        0        0      287 2024-03-14 13:13:32.533040 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
+-rw-r--r--   0        0        0      781 2024-03-14 13:13:32.533130 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
+-rw-r--r--   0        0        0      339 2024-03-14 13:13:32.533332 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
+-rw-r--r--   0        0        0   148134 2024-03-14 13:13:32.533676 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
+-rw-r--r--   0        0        0      534 2024-03-14 13:13:32.533791 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
+-rw-r--r--   0        0        0    20142 2024-03-14 13:13:32.533945 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
+-rw-r--r--   0        0        0      651 2024-03-14 13:13:32.534054 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
+-rw-r--r--   0        0        0     1205 2024-03-14 13:13:32.534187 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
+-rw-r--r--   0        0        0     3178 2024-03-15 12:01:06.702704 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
+-rw-r--r--   0        0        0     1778 2024-03-14 13:13:32.534482 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml
+-rw-r--r--   0        0        0      617 2024-03-14 13:13:32.534637 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0      741 2024-03-14 13:13:32.534954 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html
+-rw-r--r--   0        0        0      783 2024-03-14 13:13:32.535055 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
+-rw-r--r--   0        0        0     2881 2024-03-14 13:13:32.535205 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/manifest-backend.yml
+-rw-r--r--   0        0        0     3921 2024-03-14 13:13:32.535341 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/manifest-public.yml
+-rw-r--r--   0        0        0      386 2024-03-14 13:13:32.535470 dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0        0 2024-03-14 13:13:32.535503 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/__init__.py
+-rw-r--r--   0        0        0     3907 2024-03-14 13:13:32.535619 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/application.py
+-rw-r--r--   0        0        0    10704 2024-03-14 13:13:32.535803 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/aws.py
+-rw-r--r--   0        0        0     2943 2024-03-14 13:13:32.535890 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/click.py
+-rw-r--r--   0        0        0     1053 2024-03-14 13:13:32.535972 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/cloudformation.py
+-rw-r--r--   0        0        0      484 2024-03-14 13:13:32.536056 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/cloudfoundry.py
+-rw-r--r--   0        0        0     1720 2024-03-14 13:13:32.536141 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/files.py
+-rw-r--r--   0        0        0      304 2024-03-14 13:13:32.536225 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/git.py
+-rw-r--r--   0        0        0      507 2024-03-14 13:13:32.536457 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/manifests.py
+-rw-r--r--   0        0        0      115 2024-03-14 13:13:32.536567 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/messages.py
+-rw-r--r--   0        0        0      469 2024-03-14 13:13:32.536666 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/template.py
+-rw-r--r--   0        0        0    16301 2024-04-05 09:30:20.387725 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/validation.py
+-rw-r--r--   0        0        0     6408 2024-03-14 13:13:32.537042 dbt_platform_helper-6.2.0/dbt_platform_helper/utils/versioning.py
+-rwxr-xr-x   0        0        0     1936 2024-03-14 13:13:32.541196 dbt_platform_helper-6.2.0/platform_helper.py
+-rw-r--r--   0        0        0     1393 2024-04-05 10:08:26.991689 dbt_platform_helper-6.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-6.2.0/PKG-INFO
```

### Comparing `dbt_platform_helper-6.1.0/LICENSE` & `dbt_platform_helper-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/COMMANDS.md` & `dbt_platform_helper-6.2.0/dbt_platform_helper/COMMANDS.md`

 * *Files 1% similar despite different names*

```diff
@@ -432,14 +432,17 @@
 - [`get-env-secrets` ↪](#platform-helper-copilot-get-env-secrets)
 - [`make-addons` ↪](#platform-helper-copilot-make-addons)
 
 # platform-helper copilot make-addons
 
 [↩ Parent](#platform-helper-copilot)
 
+    WARNING: this command should not be used as a stand-alone.
+    Use `platform-helper generate` instead.
+
     Generate addons CloudFormation for each environment.
 
 ## Usage
 
 ```
 platform-helper copilot make-addons 
 ```
```

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/README.md` & `dbt_platform_helper-6.2.0/dbt_platform_helper/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,8 +45,8 @@
 
 Commands:
   instructions     Show migration instructions.
   make-config      Generate copilot boilerplate code.
   migrate-secrets  Migrate secrets from your gov paas application to...
 ```
 
-See the [Commands Reference](https://github.com/uktrade/platform-helper/blob/main/dbt_platform_helper/COMMANDS.md) for a list of all available subcommands.
+See the [Commands Reference](https://github.com/uktrade/platform-tools/blob/main/dbt_platform_helper/COMMANDS.md) for a list of all available subcommands.
```

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/addon-plans.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/addon-plans.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/addons-template-map.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/addons-template-map.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/commands/application.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/application.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/commands/bootstrap.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/bootstrap.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/commands/check_cloudformation.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/check_cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/commands/codebase.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/codebase.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/commands/conduit.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/conduit.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/commands/config.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/config.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/commands/copilot.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/copilot.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,20 @@
     overrides_path.mkdir(parents=True, exist_ok=True)
     overrides_file = overrides_path.joinpath("cfn.patches.yml")
     overrides_file.write_text(templates.get_template("svc/overrides/cfn.patches.yml").render())
 
 
 @copilot.command(deprecated=True, hidden=True)
 def make_addons():
-    """Generate addons CloudFormation for each environment."""
+    """
+    WARNING: this command should not be used as a stand-alone.
+    Use `platform-helper generate` instead.
+
+    Generate addons CloudFormation for each environment.
+    """
     output_dir = Path(".").absolute()
 
     ensure_cwd_is_repo_root()
     templates = setup_templates()
     config = _get_config()
 
     with open(PACKAGE_DIR / "addons-template-map.yml") as fd:
```

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/commands/dns.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/dns.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,30 +249,60 @@
     domains_to_create = get_required_subdomains(base_domain, subdomain)
     zone_ids = {}
 
     for domain_name in domains_to_create:
         domain_zone = f"{domain_name}."
         parent_domain = domain_name.split(".", maxsplit=1)[1]
         parent_zone = f"{parent_domain}."
-        hosted_zone_response = client.list_hosted_zones_by_name()
-        hosted_zones = {hz["Name"]: hz for hz in hosted_zone_response["HostedZones"]}
-        parent_zone_id = _get_zone_id_or_abort(hosted_zones, parent_zone)
 
-        if domain_zone in hosted_zones:
+        domain_zone_id, parent_zone_id = _get_paginated_zones(client, parent_zone, domain_zone)
+
+        if parent_zone_id is None:
+            click.secho(
+                f"The hosted zone: {parent_zone} does not exist in your AWS domain account",
+                fg="red",
+            )
+            exit()
+
+        if domain_zone_id is not None:
             click.secho(f"Hosted zone '{domain_zone}' already exists", fg="yellow")
-            zone_ids[domain_name] = hosted_zones[domain_zone]["Id"]
+            zone_ids[domain_name] = domain_zone_id
         else:
             subdomain_zone_id = _create_hosted_zone(
                 client, domain_name, parent_zone, parent_zone_id
             )
             zone_ids[domain_name] = subdomain_zone_id
 
     return zone_ids
 
 
+def _get_hosted_zones_paginator(client):
+    return client.get_paginator("list_hosted_zones").paginate()
+
+
+def _get_paginated_zones(client, parent_zone, domain_zone):
+    domain_zone_id = parent_zone_id = None
+
+    for page in _get_hosted_zones_paginator(client):
+        # each page is a hosted zones response type object
+        hosted_zones = {hz["Name"]: hz for hz in page["HostedZones"]}
+
+        if parent_zone in hosted_zones and parent_zone_id is None:
+            parent_zone_id = hosted_zones[parent_zone]["Id"]
+
+        if domain_zone in hosted_zones and domain_zone_id is None:
+            domain_zone_id = hosted_zones[domain_zone]["Id"]
+
+        if all([parent_zone_id, domain_zone_id]):
+            # both were found, no need to further pagination
+            break
+
+    return domain_zone_id, parent_zone_id
+
+
 def _create_hosted_zone(client, domain_name, parent_zone, parent_zone_id):
     if not click.confirm(
         click.style("About to create domain: ", fg="cyan")
         + click.style(f"{domain_name}\n", fg="white", bold=True)
         + click.style("Do you want to continue?", fg="cyan"),
     ):
         exit()
@@ -425,25 +455,14 @@
     hosted_zones = create_hosted_zones(domain_client, base_domain, subdomain)
 
     cert_zone_id = get_certificate_zone_id(hosted_zones)
 
     return create_cert(project_client, domain_client, subdomain, cert_zone_id)
 
 
-def _get_zone_id_or_abort(hosted_zones, zone):
-    """Zones have the '.' suffix."""
-    if zone not in hosted_zones:
-        click.secho(
-            f"The hosted zone: {zone} does not exist in your AWS domain account {hosted_zones}",
-            fg="red",
-        )
-        exit()
-    return hosted_zones[zone]["Id"]
-
-
 @click.group(chain=True, cls=ClickDocOptGroup)
 def domain():
     check_platform_helper_version_needs_update()
 
 
 @domain.command()
 @click.option(
```

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/commands/environment.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/environment.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/commands/generate.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/generate.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/commands/pipeline.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/commands/pipeline.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/custom_resources/s3_object.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/custom_resources/s3_object.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/COMMANDS.md.jinja` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/COMMANDS.md.jinja`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addon-instructions.txt` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addon-instructions.txt`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/monitoring.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/monitoring.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/opensearch.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/opensearch.yml`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,22 @@
       EngineVersion: 'OpenSearch_1.1'
     '1.2':
       EngineVersion: 'OpenSearch_1.2'
     '1.3':
       EngineVersion: 'OpenSearch_1.3'
     '2.3':
       EngineVersion: 'OpenSearch_2.3'
+    '2.5':
+      EngineVersion: 'OpenSearch_2.5'
+    '2.7':
+      EngineVersion: 'OpenSearch_2.7'
+    '2.9':
+      EngineVersion: 'OpenSearch_2.9'
+    '2.11':
+      EngineVersion: 'OpenSearch_2.11'
 
 Conditions:
   {{ addon_config.prefix }}EnableHA: !Not [!Equals [!FindInMap [{{ addon_config.prefix }}EnvironmentConfigMap, !Ref Env, InstanceCount], 1]]
   {{ addon_config.prefix }}CreateProdSubFilter: !Or [!Equals [!Ref Env, prod], !Equals [!Ref Env, production], !Equals [!Ref Env, PROD], !Equals [!Ref Env, PRODUCTION]]
 
 Resources:
   {{ addon_config.prefix }}OpenSearchSecret:
```

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,18 @@
       EngineVersion: '{{ config.engine }}'
       CacheNodeType: '{{ config.instance }}'
       NumReplicas: {{ config.replicas }}
       DeletionPolicy: {{ config.deletion_policy }}
 {%- endfor %}
 
   {{ addon_config.prefix }}EngineVersionMap:
+    '7.1':
+      CacheParameterGroupFamily: 'redis7.x'
+    '7.0':
+      CacheParameterGroupFamily: 'redis7.x'
     '6.2':
       CacheParameterGroupFamily: 'redis6.x'
     '6.0':
       CacheParameterGroupFamily: 'redis6.x'
     '5.0.6':
       CacheParameterGroupFamily: 'redis5.0'
     '5.0.4':
```

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/s3.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/s3.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/env/vpc.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/env/vpc.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/manifest.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/overrides/package-lock.json` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/package-lock.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/overrides/package.json` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/package.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/overrides/stack.ts` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/env/overrides/tsconfig.json` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/env/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml`

 * *Files 7% similar despite different names*

```diff
@@ -15,47 +15,47 @@
         fi
       - |
         if [ ! -f .platform-helper-version ]; then
           echo "Cannot find .platform-helper-version file"
           exit 1
         fi
       - COPILOT_VERSION=`cat .copilot-version`
-      - platform_helper_VERSION=`cat .platform-helper-version`
+      - PLATFORM_HELPER_VERSION=`cat .platform-helper-version`
       - mkdir ./build-tools
       - cd ./build-tools
       # Install copilot
       - wget -q "https://ecs-cli-v2-release.s3.amazonaws.com/copilot-linux-v${COPILOT_VERSION}"
       - mv "./copilot-linux-v${COPILOT_VERSION}" ./copilot
       - chmod +x ./copilot
       # Install pyyaml and dbt-platform-helper
-      - pip install PyYAML dbt-platform-helper==$platform_helper_VERSION
+      - pip install PyYAML dbt-platform-helper==$PLATFORM_HELPER_VERSION
       # Install dyff - yaml differ
       - wget -q "https://github.com/homeport/dyff/releases/download/v${DYFF_VERSION}/dyff_${DYFF_VERSION}_linux_amd64.tar.gz"
       - tar -zxvf "dyff_${DYFF_VERSION}_linux_amd64.tar.gz"
       - chmod +x ./dyff
   build:
     commands:
       - cd $CODEBUILD_SRC_DIR
-      - platform_helper_VERSION=`cat .platform-helper-version`
+      - PLATFORM_HELPER_VERSION=`cat .platform-helper-version`
       - cp -r copilot/ current-copilot/
       - platform-helper copilot make-addons
       - >
         for FILE in $(ls copilot/**/addons/*.yml); do
           ./build-tools/dyff between --omit-header $FILE current-$FILE >> ./build-tools/file-differences
         done;
       - |
         if [[ "$(cat ./build-tools/file-differences)" = *[![:space:]]* ]]; then
-          echo 'Changes are introduced with version ${platform_helper_VERSION} of platform-helper:'
+          echo 'Changes are introduced with version ${PLATFORM_HELPER_VERSION} of platform-helper:'
           echo
           for FILE in $(ls copilot/**/addons/*.yml); do
             echo "Changes in $FILE:"
             ./build-tools/dyff between --omit-header $FILE current-$FILE
           done;
           echo
-          echo 'Ensure you are running version ${platform_helper_VERSION} with pip install dbt-platform-helper==${platform_helper_VERSION}'
+          echo 'Ensure you are running version ${PLATFORM_HELPER_VERSION} with pip install dbt-platform-helper==${PLATFORM_HELPER_VERSION}'
           echo 'And run platform-helper copilot make-addons to regenerate your addons templates'
           exit 1
         fi
   post_build:
     commands:
       - git checkout -- .
       - export COLOR="false"
```

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/svc/manifest-backend.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/manifest-backend.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/templates/svc/manifest-public.yml` & `dbt_platform_helper-6.2.0/dbt_platform_helper/templates/svc/manifest-public.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/utils/application.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/utils/application.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/utils/aws.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/utils/aws.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/utils/click.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/utils/click.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/utils/cloudformation.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/utils/cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/utils/files.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/utils/files.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/utils/validation.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/utils/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,21 +303,21 @@
     "medium-ha",
     "large",
     "large-ha",
     "x-large",
     "x-large-ha",
 )
 
-REDIS_ENGINE_VERSIONS = Or("4.0.10", "5.0.6", "6.0", "6.2")
+REDIS_ENGINE_VERSIONS = Or("4.0.10", "5.0.6", "6.0", "6.2", "7.0", "7.1")
 
 OPENSEARCH_PLANS = Or(
     "tiny", "small", "small-ha", "medium", "medium-ha", "large", "large-ha", "x-large", "x-large-ha"
 )
 
-OPENSEARCH_ENGINE_VERSIONS = Or("2.5", "2.3", "1.3", "1.2", "1.1", "1.0")
+OPENSEARCH_ENGINE_VERSIONS = Or("2.11", "2.9", "2.7", "2.5", "2.3", "1.3", "1.2", "1.1", "1.0")
 
 S3_BASE = {
     Optional("readonly"): bool,
     Optional("services"): Or("__all__", [str]),
     Optional("environments"): {
         ENV_NAME: {
             "bucket_name": validate_s3_bucket_name,
```

### Comparing `dbt_platform_helper-6.1.0/dbt_platform_helper/utils/versioning.py` & `dbt_platform_helper-6.2.0/dbt_platform_helper/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/platform_helper.py` & `dbt_platform_helper-6.2.0/platform_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.1.0/pyproject.toml` & `dbt_platform_helper-6.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "dbt-platform-helper"
-version = "6.1.0"
+version = "6.2.0"
 description = "Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 license = "MIT"
 readme = "dbt_platform_helper/README.md"
 packages = [
     { include = "dbt_platform_helper" },
     { include = "platform_helper.py" }
@@ -26,22 +26,23 @@
 cloudfoundry-client = "1.35.2"
 mypy-boto3-codebuild = "^1.26.0.post1"
 python = "^3.9"
 schema = "0.7.5"
 cfn-flip = "1.3.0"
 aiohttp = "^3.8.4"
 certifi = "^2023.07.22"
-cryptography = "^41.0.3"
+cryptography = ">=41.0.3,<43.0.0"
 jinja2-simple-tags = "^0.5.0"
 cfn-lint = "^0.80.2"
 requests = "^2.31.0"
 prettytable = "^3.9.0"
 semver = "^3.0.2"
 tomlkit = "^0.12.2"
 checkov = "^3.1.67"
+slack-sdk = "^3.27.1"
 
 [tool.poetry.group.dev.dependencies]
 moto = {extras = ["all"], version = "^4.1.12"}
 pyfakefs = "^5.2.2"
 pytest = "^7.3.1"
 pytest-env = "^0.8.1"
 tox = "^4.6.0"
```

### Comparing `dbt_platform_helper-6.1.0/PKG-INFO` & `dbt_platform_helper-6.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-platform-helper
-Version: 6.1.0
+Version: 6.2.0
 Summary: Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot.
 License: MIT
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,21 +20,22 @@
 Requires-Dist: botocore (>=1.29.31,<2.0.0)
 Requires-Dist: certifi (>=2023.07.22,<2024.0.0)
 Requires-Dist: cfn-flip (==1.3.0)
 Requires-Dist: cfn-lint (>=0.80.2,<0.81.0)
 Requires-Dist: checkov (>=3.1.67,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cloudfoundry-client (==1.35.2)
-Requires-Dist: cryptography (>=41.0.3,<42.0.0)
+Requires-Dist: cryptography (>=41.0.3,<43.0.0)
 Requires-Dist: jinja2-simple-tags (>=0.5.0,<0.6.0)
 Requires-Dist: mypy-boto3-codebuild (>=1.26.0.post1,<2.0.0)
 Requires-Dist: prettytable (>=3.9.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: schema (==0.7.5)
 Requires-Dist: semver (>=3.0.2,<4.0.0)
+Requires-Dist: slack-sdk (>=3.27.1,<4.0.0)
 Requires-Dist: tomlkit (>=0.12.2,<0.13.0)
 Description-Content-Type: text/markdown
 
 # DBT Platform Helper
 
 This package contains a set of tools in the form of a Command Line Interface (CLI) primarily for transferring applications/services from [GOV.UK PaaS](https://www.cloud.service.gov.uk) to Department for Business and Trade (DBT) PaaS which augments [AWS Copilot](https://aws.github.io/copilot-cli/). These tools can also be used to provision AWS resources and/or make sure the CloudFormation templates conform to best practices.
 
@@ -81,9 +82,9 @@
 
 Commands:
   instructions     Show migration instructions.
   make-config      Generate copilot boilerplate code.
   migrate-secrets  Migrate secrets from your gov paas application to...
 ```
 
-See the [Commands Reference](https://github.com/uktrade/platform-helper/blob/main/dbt_platform_helper/COMMANDS.md) for a list of all available subcommands.
+See the [Commands Reference](https://github.com/uktrade/platform-tools/blob/main/dbt_platform_helper/COMMANDS.md) for a list of all available subcommands.
```

