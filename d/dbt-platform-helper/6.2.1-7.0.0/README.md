# Comparing `tmp/dbt_platform_helper-6.2.1.tar.gz` & `tmp/dbt_platform_helper-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_platform_helper-6.2.1.tar", max compression
+gzip compressed data, was "dbt_platform_helper-7.0.0.tar", max compression
```

## Comparing `dbt_platform_helper-6.2.1.tar` & `dbt_platform_helper-7.0.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     1090 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/LICENSE
--rw-r--r--   0        0        0    19003 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/COMMANDS.md
--rw-r--r--   0        0        0     1762 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/README.md
--rw-r--r--   0        0        0        0 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/__init__.py
--rw-r--r--   0        0        0     3842 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/addon-plans.yml
--rw-r--r--   0        0        0     1278 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/addons-template-map.yml
--rw-r--r--   0        0        0        0 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/__init__.py
--rw-r--r--   0        0        0     9957 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/application.py
--rwxr-xr-x   0        0        0    10582 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/bootstrap.py
--rwxr-xr-x   0        0        0     3226 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/check_cloudformation.py
--rw-r--r--   0        0        0    11192 2024-04-08 10:54:29.287222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/codebase.py
--rw-r--r--   0        0        0    12855 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/conduit.py
--rw-r--r--   0        0        0     7949 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/config.py
--rwxr-xr-x   0        0        0    14591 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/copilot.py
--rwxr-xr-x   0        0        0    35037 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/dns.py
--rw-r--r--   0        0        0     8670 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/environment.py
--rw-r--r--   0        0        0      722 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/generate.py
--rw-r--r--   0        0        0     6218 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/commands/pipeline.py
--rw-r--r--   0        0        0        0 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/custom_resources/__init__.py
--rw-r--r--   0        0        0     2396 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/custom_resources/s3_object.py
--rw-r--r--   0        0        0      346 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/default-addons.yml
--rw-r--r--   0        0        0      499 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/exceptions.py
--rw-r--r--   0        0        0      369 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/jinja2_tags.py
--rw-r--r--   0        0        0      158 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/.copilot/config.yml
--rwxr-xr-x   0        0        0      164 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/.copilot/image_build_run.sh
--rwxr-xr-x   0        0        0      121 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/.copilot/phases/build.sh
--rwxr-xr-x   0        0        0      123 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/.copilot/phases/install.sh
--rwxr-xr-x   0        0        0      126 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/.copilot/phases/post_build.sh
--rwxr-xr-x   0        0        0      125 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
--rw-r--r--   0        0        0     1081 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/COMMANDS.md.jinja
--rw-r--r--   0        0        0      622 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addon-instructions.txt
--rw-r--r--   0        0        0      412 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/README.md
--rw-r--r--   0        0        0      734 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/addons.parameters.yml
--rw-r--r--   0        0        0    26381 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
--rw-r--r--   0        0        0     6064 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/monitoring.yml
--rw-r--r--   0        0        0    10853 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/opensearch.yml
--rw-r--r--   0        0        0    25624 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/rds-postgres.yml
--rw-r--r--   0        0        0     7613 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/redis-cluster.yml
--rw-r--r--   0        0        0     7626 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/s3.yml
--rw-r--r--   0        0        0     3662 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/vpc.yml
--rw-r--r--   0        0        0      956 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
--rw-r--r--   0        0        0     2134 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/svc/s3-policy.yml
--rw-r--r--   0        0        0      893 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
--rw-r--r--   0        0        0     1836 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/ci-codebuild-role-policy.json
--rw-r--r--   0        0        0      197 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/create-codebuild-role.json
--rw-r--r--   0        0        0     1180 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/custom-codebuild-role-policy.json
--rw-r--r--   0        0        0      691 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/manifest.yml
--rw-r--r--   0        0        0      169 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/.gitignore
--rw-r--r--   0        0        0      439 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/README.md
--rw-r--r--   0        0        0      284 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/bin/override.ts
--rw-r--r--   0        0        0      339 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/cdk.json
--rw-r--r--   0        0        0     1760 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
--rw-r--r--   0        0        0   150965 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/package-lock.json
--rw-r--r--   0        0        0      534 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/package.json
--rw-r--r--   0        0        0     1906 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/stack.ts
--rw-r--r--   0        0        0      710 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/tsconfig.json
--rw-r--r--   0        0        0     1959 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
--rw-r--r--   0        0        0      169 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
--rw-r--r--   0        0        0      227 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
--rw-r--r--   0        0        0      287 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
--rw-r--r--   0        0        0      781 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
--rw-r--r--   0        0        0      339 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
--rw-r--r--   0        0        0   148134 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
--rw-r--r--   0        0        0      534 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
--rw-r--r--   0        0        0    20142 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
--rw-r--r--   0        0        0      651 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
--rw-r--r--   0        0        0     1205 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
--rw-r--r--   0        0        0     3178 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
--rw-r--r--   0        0        0     1778 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/environments/manifest.yml
--rw-r--r--   0        0        0      617 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
--rw-r--r--   0        0        0      741 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/maintenance_pages/default.html
--rw-r--r--   0        0        0      783 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
--rw-r--r--   0        0        0     2881 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/manifest-backend.yml
--rw-r--r--   0        0        0     3921 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/manifest-public.yml
--rw-r--r--   0        0        0      386 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
--rw-r--r--   0        0        0        0 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/__init__.py
--rw-r--r--   0        0        0     3907 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/application.py
--rw-r--r--   0        0        0    10704 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/aws.py
--rw-r--r--   0        0        0     2943 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/click.py
--rw-r--r--   0        0        0     1053 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/cloudformation.py
--rw-r--r--   0        0        0      484 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/cloudfoundry.py
--rw-r--r--   0        0        0     1720 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/files.py
--rw-r--r--   0        0        0      304 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/git.py
--rw-r--r--   0        0        0      507 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/manifests.py
--rw-r--r--   0        0        0      115 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/messages.py
--rw-r--r--   0        0        0      469 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/template.py
--rw-r--r--   0        0        0    16301 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/validation.py
--rw-r--r--   0        0        0     6408 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/dbt_platform_helper/utils/versioning.py
--rwxr-xr-x   0        0        0     1936 2024-04-08 10:54:29.297222 dbt_platform_helper-6.2.1/platform_helper.py
--rw-r--r--   0        0        0     1393 2024-04-08 10:54:29.307222 dbt_platform_helper-6.2.1/pyproject.toml
--rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-6.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/LICENSE
+-rw-r--r--   0        0        0    19003 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/COMMANDS.md
+-rw-r--r--   0        0        0     1762 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/__init__.py
+-rw-r--r--   0        0        0     4522 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/addon-plans.yml
+-rw-r--r--   0        0        0     1315 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/addons-template-map.yml
+-rw-r--r--   0        0        0        0 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/__init__.py
+-rw-r--r--   0        0        0     9957 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/application.py
+-rwxr-xr-x   0        0        0    10582 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/bootstrap.py
+-rwxr-xr-x   0        0        0     3226 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/check_cloudformation.py
+-rw-r--r--   0        0        0    11192 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/codebase.py
+-rw-r--r--   0        0        0    12855 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/conduit.py
+-rw-r--r--   0        0        0     7949 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/config.py
+-rwxr-xr-x   0        0        0    16324 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/copilot.py
+-rwxr-xr-x   0        0        0    35037 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/dns.py
+-rw-r--r--   0        0        0     8670 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/environment.py
+-rw-r--r--   0        0        0      722 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/generate.py
+-rw-r--r--   0        0        0     6218 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/pipeline.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/custom_resources/__init__.py
+-rw-r--r--   0        0        0     2396 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/custom_resources/s3_object.py
+-rw-r--r--   0        0        0      342 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/default-addons.yml
+-rw-r--r--   0        0        0      499 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/exceptions.py
+-rw-r--r--   0        0        0      369 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/jinja2_tags.py
+-rw-r--r--   0        0        0      158 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/.copilot/config.yml
+-rwxr-xr-x   0        0        0      164 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/.copilot/image_build_run.sh
+-rwxr-xr-x   0        0        0      121 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/.copilot/phases/build.sh
+-rwxr-xr-x   0        0        0      123 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/.copilot/phases/install.sh
+-rwxr-xr-x   0        0        0      126 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/.copilot/phases/post_build.sh
+-rwxr-xr-x   0        0        0      125 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
+-rw-r--r--   0        0        0     1081 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/COMMANDS.md.jinja
+-rw-r--r--   0        0        0      618 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addon-instructions.txt
+-rw-r--r--   0        0        0      412 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/README.md
+-rw-r--r--   0        0        0      734 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml
+-rw-r--r--   0        0        0    26381 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
+-rw-r--r--   0        0        0     6064 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/monitoring.yml
+-rw-r--r--   0        0        0    10853 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/opensearch.yml
+-rw-r--r--   0        0        0    25624 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml
+-rw-r--r--   0        0        0     7613 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml
+-rw-r--r--   0        0        0     7626 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/s3.yml
+-rw-r--r--   0        0        0     3658 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/vpc.yml
+-rw-r--r--   0        0        0      956 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
+-rw-r--r--   0        0        0     2403 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml
+-rw-r--r--   0        0        0      893 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
+-rw-r--r--   0        0        0     1836 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json
+-rw-r--r--   0        0        0      197 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/create-codebuild-role.json
+-rw-r--r--   0        0        0     1180 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json
+-rw-r--r--   0        0        0      691 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/manifest.yml
+-rw-r--r--   0        0        0      169 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/.gitignore
+-rw-r--r--   0        0        0      439 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/README.md
+-rw-r--r--   0        0        0      284 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/bin/override.ts
+-rw-r--r--   0        0        0      339 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/cdk.json
+-rw-r--r--   0        0        0     1760 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
+-rw-r--r--   0        0        0   150965 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/package-lock.json
+-rw-r--r--   0        0        0      534 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/package.json
+-rw-r--r--   0        0        0     1906 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/stack.ts
+-rw-r--r--   0        0        0      710 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/tsconfig.json
+-rw-r--r--   0        0        0     1959 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
+-rw-r--r--   0        0        0      169 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
+-rw-r--r--   0        0        0      227 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
+-rw-r--r--   0        0        0      287 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
+-rw-r--r--   0        0        0      781 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
+-rw-r--r--   0        0        0      339 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
+-rw-r--r--   0        0        0   148134 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
+-rw-r--r--   0        0        0      534 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
+-rw-r--r--   0        0        0    20142 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
+-rw-r--r--   0        0        0      651 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
+-rw-r--r--   0        0        0     1205 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
+-rw-r--r--   0        0        0     3178 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
+-rw-r--r--   0        0        0     1778 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml
+-rw-r--r--   0        0        0      617 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0      741 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html
+-rw-r--r--   0        0        0      783 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
+-rw-r--r--   0        0        0     2881 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/manifest-backend.yml
+-rw-r--r--   0        0        0     3921 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/manifest-public.yml
+-rw-r--r--   0        0        0      386 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0        0 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/__init__.py
+-rw-r--r--   0        0        0     3908 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/application.py
+-rw-r--r--   0        0        0    10704 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/aws.py
+-rw-r--r--   0        0        0     2943 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/click.py
+-rw-r--r--   0        0        0     1053 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/cloudformation.py
+-rw-r--r--   0        0        0      484 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/cloudfoundry.py
+-rw-r--r--   0        0        0     1720 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/files.py
+-rw-r--r--   0        0        0      304 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/git.py
+-rw-r--r--   0        0        0      507 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/manifests.py
+-rw-r--r--   0        0        0      115 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/messages.py
+-rw-r--r--   0        0        0      469 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/template.py
+-rw-r--r--   0        0        0    17799 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/validation.py
+-rw-r--r--   0        0        0     6408 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/versioning.py
+-rwxr-xr-x   0        0        0     1936 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/platform_helper.py
+-rw-r--r--   0        0        0     1393 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-7.0.0/PKG-INFO
```

### Comparing `dbt_platform_helper-6.2.1/LICENSE` & `dbt_platform_helper-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/COMMANDS.md` & `dbt_platform_helper-7.0.0/dbt_platform_helper/COMMANDS.md`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/README.md` & `dbt_platform_helper-7.0.0/dbt_platform_helper/README.md`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/addon-plans.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/addon-plans.yml`

 * *Files 20% similar despite different names*

```diff
@@ -122,15 +122,15 @@
   x-large-ha:
     volume_size: 1500
     instances: 2
     master: false
     instance: m6g.2xlarge.search
 
 # RDS/Postgres Instances
-rds-postgres:
+postgres:
   # 2v CPU, 1GB RAM, 20GB Storage
   tiny:
     volume_size: 20
     multi_az: false
     instance: db.t3.micro
 
   # 2v CPU, 2GB RAM, 100GB Storage
@@ -141,48 +141,82 @@
 
   # 2v CPU, 2GB RAM, 100GB Storage, multi AZ
   small-ha:
     volume_size: 100
     multi_az: true
     instance: db.t3.small
 
+  # 2v CPU, 2GB RAM, 100GB Storage, multi AZ
+  small-high-io:
+    volume_size: 100
+    multi_az: true
+    instance: db.t3.small
+    storage_type: io1
+    iops: 40000
+
   # 2v CPU, 8GB RAM, 100GB Storage
   medium:
     volume_size: 100
     multi_az: false
     instance: db.m5.large
 
   # 2v CPU, 8GB RAM, 100GB Storage, multi AZ
   medium-ha:
     volume_size: 100
     multi_az: true
     instance: db.m5.large
 
+  # 2v CPU, 8GB RAM, 100GB Storage, multi AZ
+  medium-high-io:
+    volume_size: 100
+    multi_az: true
+    instance: db.m5.large
+    storage_type: io1
+    iops: 40000
+
   # 8v CPU, 32GB RAM, 564GB Storage
   large:
     volume_size: 564
     multi_az: false
     instance: db.m5.2xlarge
 
   # 8v CPU, 32GB RAM, 564GB Storage, multi AZ
   large-ha:
     volume_size: 564
     multi_az: true
     instance: db.m5.2xlarge
 
+  # 8v CPU, 32GB RAM, 564GB Storage, multi AZ
+  large-high-io:
+    volume_size: 564
+    multi_az: true
+    instance: db.m5.2xlarge
+    storage_type: io1
+    iops: 40000
+
   # 16v CPU, 64GB RAM, 2000GB Storage
   x-large:
     volume_size: 2000
     multi_az: false
     instance: db.m5.4xlarge
 
   # 16v CPU, 64GB RAM, 2000GB Storage, multi AZ
   x-large-ha:
     volume_size: 2000
     multi_az: true
     instance: db.m5.4xlarge
 
-aurora-postgres: {}
+  # 16v CPU, 64GB RAM, 2000GB Storage, multi AZ
+  x-large-high-io:
+    volume_size: 2000
+    multi_az: true
+    instance: db.m5.4xlarge
+    storage_type: io1
+    iops: 40000
 
 s3: {}
 
 s3-policy: {}
+
+monitoring: {}
+
+alb: {}
```

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/addons-template-map.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/addons-template-map.yml`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 redis:
   requires_addons_parameters: true
   env:
     - template: addons/env/redis-cluster.yml
 aurora-postgres:
   env:
     - template: addons/env/aurora-postgres.yml
-rds-postgres:
+postgres:
   requires_addons_parameters: true
   env:
     - template: addons/env/rds-postgres.yml
 opensearch:
   requires_addons_parameters: true
   env:
     - template: addons/env/opensearch.yml
@@ -43,7 +43,9 @@
   requires_addons_parameters: true
   env:
     - template: addons/env/monitoring.yml
 vpc:
   requires_addons_parameters: true
   env:
     - template: addons/env/vpc.yml
+alb:
+  requires_addons_parameters: false
```

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/application.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/application.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/bootstrap.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/bootstrap.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/check_cloudformation.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/check_cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/codebase.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/codebase.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/conduit.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/conduit.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/config.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/config.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/copilot.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/copilot.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from os.path import isfile
 from pathlib import Path
 from pathlib import PosixPath
 
 import click
 import yaml
 
+from dbt_platform_helper.utils.application import get_application_name
+from dbt_platform_helper.utils.application import load_application
 from dbt_platform_helper.utils.aws import SSM_BASE_PATH
 from dbt_platform_helper.utils.aws import get_aws_session_or_abort
 from dbt_platform_helper.utils.click import ClickDocOptGroup
 from dbt_platform_helper.utils.files import ensure_cwd_is_repo_root
 from dbt_platform_helper.utils.files import generate_override_files
 from dbt_platform_helper.utils.files import mkfile
 from dbt_platform_helper.utils.template import camel_case
@@ -94,14 +96,15 @@
         config = yaml.safe_load(fd)
 
     # empty file
     if not config:
         return {}
 
     errors = validate_addons(config)
+
     if errors:
         click.echo(click.style(f"Errors found in {config_file}:", fg="red"))
         for addon, error in errors.items():
             click.echo(click.style(f"Addon '{addon}': {error}", fg="red"))
         exit(1)
 
     env_names = list_copilot_local_environments()
@@ -132,15 +135,15 @@
                         f"Services listed in {addon_name}.services do not exist in ./copilot/",
                         fg="red",
                     ),
                 )
                 exit(1)
 
         environments = normalised_config[addon_name].pop("environments", {})
-        default = environments.pop("default", {})
+        default = environments.pop("*", environments.pop("default", {}))
 
         initial = _lookup_plan(addon_type, default)
 
         if not set(environments.keys()).issubset(set(env_names)):
             click.echo(
                 click.style(
                     f"Environment keys listed in {addon_name} do not match ./copilot/environments",
@@ -187,34 +190,65 @@
     click.echo(f"\n>>> Generating service overrides for {name}\n")
     overrides_path = base_path.joinpath(f"copilot/{name}/overrides")
     overrides_path.mkdir(parents=True, exist_ok=True)
     overrides_file = overrides_path.joinpath("cfn.patches.yml")
     overrides_file.write_text(templates.get_template("svc/overrides/cfn.patches.yml").render())
 
 
+def is_terraform_project() -> bool:
+    return Path("./terraform").is_dir()
+
+
+def _get_s3_kms_alias_arns(session, application_name, extension_name):
+    application = load_application(application_name, session)
+
+    arns = {}
+    for environment_name, environment in application.environments.items():
+        client = environment.session.client("kms")
+
+        alias_name = f"alias/{application_name}-{environment_name}-{extension_name}-key"
+
+        try:
+            response = client.describe_key(KeyId=alias_name)
+        except client.exceptions.NotFoundException:
+            pass
+        else:
+            arns[environment_name] = response["KeyMetadata"]["Arn"]
+
+    return arns
+
+
 @copilot.command(deprecated=True, hidden=True)
 def make_addons():
     """
     WARNING: this command should not be used as a stand-alone.
     Use `platform-helper generate` instead.
 
     Generate addons CloudFormation for each environment.
     """
-    output_dir = Path(".").absolute()
 
+    output_dir = Path(".").absolute()
     ensure_cwd_is_repo_root()
+    is_terraform = is_terraform_project()
+
     templates = setup_templates()
     config = _get_config()
+    session = get_aws_session_or_abort()
+
+    application_name = get_application_name()
 
     with open(PACKAGE_DIR / "addons-template-map.yml") as fd:
         addon_template_map = yaml.safe_load(fd)
 
     _generate_env_overrides(output_dir)
 
-    click.echo("\n>>> Generating addons CloudFormation\n")
+    if is_terraform:
+        click.echo("\n>>> Generating Terraform compatible addons CloudFormation\n")
+    else:
+        click.echo("\n>>> Generating addons CloudFormation\n")
 
     env_addons_path = Path(f"copilot/environments/addons/")
     (output_dir / env_addons_path).mkdir(parents=True, exist_ok=True)
 
     _cleanup_old_files(config, output_dir, env_addons_path)
     custom_resources = _get_custom_resources()
 
@@ -228,15 +262,15 @@
     has_postgres_addon = False
     for addon_name, addon_config in config.items():
         print(f">>>>>>>>> {addon_name}")
         addon_type = addon_config.pop("type")
         environments = addon_config.pop("environments")
         if addon_template_map[addon_type].get("requires_addons_parameters", False):
             has_addons_parameters = True
-        if addon_type in ["aurora-postgres", "rds-postgres"]:
+        if addon_type in ["aurora-postgres", "postgres"]:
             has_postgres_addon = True
 
         for environment_name, environment_config in environments.items():
             if not environment_config.get("deletion_policy"):
                 environments[environment_name]["deletion_policy"] = addon_config.get(
                     "deletion_policy", "Delete"
                 )
@@ -250,55 +284,65 @@
             "secret_name": addon_name.upper().replace("-", "_"),
             **addon_config,
         }
 
         services.append(environment_addon_config)
 
         service_addon_config = {
+            "application_name": application_name,
             "name": addon_config.get("name", None) or addon_name,
             "prefix": camel_case(addon_name),
             "environments": environments,
             **addon_config,
         }
 
         log_destination_arns = get_log_destination_arn()
 
         if addon_type in ["s3", "s3-policy"]:
-            service_addon_config["kms_key_reference"] = service_addon_config["prefix"].rsplit(
-                "BucketAccess", 1
-            )[0]
-
-        _generate_env_addons(
-            addon_name,
-            addon_template_map,
-            config.items(),
-            env_addons_path,
-            environment_addon_config,
-            output_dir,
-            templates,
-            log_destination_arns,
-        )
+            if is_terraform:
+                s3_kms_arns = _get_s3_kms_alias_arns(session, application_name, addon_name)
+                for environment_name in environments:
+                    environments[environment_name]["kms_key_arn"] = s3_kms_arns.get(
+                        environment_name, "kms-key-not-found"
+                    )
+            else:
+                service_addon_config["kms_key_reference"] = service_addon_config["prefix"].rsplit(
+                    "BucketAccess", 1
+                )[0]
+
+        if not is_terraform:
+            _generate_env_addons(
+                addon_name,
+                addon_template_map,
+                config.items(),
+                env_addons_path,
+                environment_addon_config,
+                output_dir,
+                templates,
+                log_destination_arns,
+            )
         _generate_service_addons(
             addon_config,
             addon_name,
             addon_template_map,
             addon_type,
             output_dir,
             service_addon_config,
             templates,
             log_destination_arns,
+            is_terraform=is_terraform,
         )
 
-        if addon_type in ["aurora-postgres", "rds-postgres"]:
+        if addon_type in ["aurora-postgres", "postgres"] and not is_terraform:
             click.secho(
                 "\nNote: The key DATABASE_CREDENTIALS may need to be changed to match your Django settings configuration.",
                 fg="yellow",
             )
 
-    if has_addons_parameters:
+    if has_addons_parameters and not is_terraform:
         template = templates.get_template("addons/env/addons.parameters.yml")
         contents = template.render({"has_postgres_addon": has_postgres_addon})
         click.echo(
             mkfile(output_dir, env_addons_path / "addons.parameters.yml", contents, overwrite=True)
         )
 
     click.echo(templates.get_template("addon-instructions.txt").render(services=services))
@@ -351,26 +395,28 @@
     addon_name,
     addon_template_map,
     addon_type,
     output_dir,
     service_addon_config,
     templates,
     log_destination_arns,
+    is_terraform,
 ):
     # generate svc addons
     for addon in addon_template_map[addon_type].get("svc", []):
         template = templates.get_template(addon["template"])
 
         for svc in addon_config.get("services", []):
             service_path = Path(f"copilot/{svc}/addons/")
 
             contents = template.render(
                 {
                     "addon_config": service_addon_config,
                     "log_destination": log_destination_arns,
+                    "is_terraform": is_terraform,
                 }
             )
 
             filename = addon.get("filename", f"{addon_name}.yml")
 
             (output_dir / service_path).mkdir(parents=True, exist_ok=True)
             click.echo(mkfile(output_dir, service_path / filename, contents, overwrite=True))
```

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/dns.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/dns.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/environment.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/environment.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/generate.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/generate.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/commands/pipeline.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/pipeline.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/custom_resources/s3_object.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/custom_resources/s3_object.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/COMMANDS.md.jinja` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/COMMANDS.md.jinja`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addon-instructions.txt` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addon-instructions.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 Secret references:
 {%- for service in services %}
 {%- if service.addon_type == "redis" %}
   REDIS_ENDPOINT: /copilot/${COPILOT_APPLICATION_NAME}/${COPILOT_ENVIRONMENT_NAME}/secrets/{{ service.secret_name }}
 {%- elif service.addon_type == "opensearch" %}
   OPENSEARCH_CREDENTIALS: /copilot/${COPILOT_APPLICATION_NAME}/${COPILOT_ENVIRONMENT_NAME}/secrets/{{ service.secret_name }}
-{%- elif service.addon_type in ["aurora-postgres", "rds-postgres"] %}
+{%- elif service.addon_type in ["aurora-postgres", "postgres"] %}
   DATABASE_CREDENTIALS:
     secretsmanager: /copilot/${COPILOT_APPLICATION_NAME}/${COPILOT_ENVIRONMENT_NAME}/secrets/{{ service.secret_name }}
 {%- endif -%}
 {%- endfor -%}
```

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/addons.parameters.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/aurora-postgres.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/monitoring.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/monitoring.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/opensearch.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/opensearch.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/rds-postgres.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/redis-cluster.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/s3.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/s3.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/env/vpc.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/vpc.yml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
       PrivateDnsEnabled: true
       SecurityGroupIds:
     {%- for addon, config in addons -%}
       {%- set prefix = addon.split('-')|first|lower ~ addon.split('-')[1:]|map('capitalize')|join -%}
       {%- if config.type == "aurora-postgres" %}
         - !GetAtt {{ prefix }}DBClusterSecurityGroup.GroupId
       {%- endif -%}
-      {%- if config.type == "rds-postgres" %}
+      {%- if config.type == "postgres" %}
         - !GetAtt {{ prefix }}SecurityGroup.GroupId
       {%- endif -%}
     {%- endfor %}
         - !Ref EnvironmentSecurityGroup
       ServiceName: 'com.amazonaws.eu-west-2.secretsmanager'
       SubnetIds: !Split [ ",", !Ref PrivateSubnets ]
       VpcEndpointType: Interface
```

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/svc/s3-policy.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 
 Mappings:
   {{ addon_config.prefix }}EnvironmentConfigMap:
     # Create an entry for each environment
 {% for env_name, config in addon_config.environments.items() %}
     {{ env_name }}:
       BucketName: '{{ config.bucket_name }}'
+    {% if is_terraform %}
+      KmsKeyArn: '{{ config.kms_key_arn }}'
+    {% endif %}
 {% endfor %}
 
 Resources:
   {{ addon_config.prefix }}S3AccessPolicy:
     Metadata:
       'aws:copilot:description': 'An IAM ManagedPolicy for your service to access the bucket'
     Type: AWS::IAM::ManagedPolicy
@@ -36,17 +39,21 @@
         Version: 2012-10-17
         Statement:
           - Sid: KMSDecryptAndGenerate
             Effect: Allow
             Action:
               - kms:Decrypt
               - kms:GenerateDataKey
+            {% if is_terraform %}
+            Resource: !FindInMap [{{ addon_config.prefix }}EnvironmentConfigMap, !Ref Env, KmsKeyArn]
+            {% else %}
             Resource:
               Fn::ImportValue:
                 !Sub "${App}-${Env}-{{ addon_config.kms_key_reference }}-KMSKeyARN"
+            {% endif %}
           - Sid: S3ObjectActions
             Effect: Allow
             Action:
 {%- if addon_config.readonly %}
               - s3:GetObject
 {% else %}
               - s3:*Object
```

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/addons/svc/subscription-filter.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/ci-codebuild-role-policy.json` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/custom-codebuild-role-policy.json` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/manifest.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/log_resource_policy.json` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/package-lock.json` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/package-lock.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/package.json` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/package.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/stack.ts` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/env/overrides/tsconfig.json` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/manifest.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/environments/buildspec.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/environments/manifest.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/maintenance_pages/default.html` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/maintenance_pages/migration.html` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/manifest-backend.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/manifest-backend.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/templates/svc/manifest-public.yml` & `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/manifest-public.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/utils/application.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/utils/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 
     application.environments = {
         env["name"]: Environment(env["name"], env["accountID"], sessions)
         for env in [
             json.loads(p["Value"]) for p in response["Parameters"] if is_environment_key(p["Name"])
         ]
     }
+
     return application
 
 
 def get_application_name():
     app_name = None
 
     try:
```

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/utils/aws.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/utils/aws.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/utils/click.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/utils/click.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/utils/cloudformation.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/utils/cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/utils/files.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/utils/files.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/utils/validation.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/utils/validation.py`

 * *Files 9% similar despite different names*

```diff
@@ -140,16 +140,16 @@
             return True
         raise SchemaError(f"should be a number between {lower} and {upper} in increments of 0.5")
 
     return is_between
 
 
 ENV_NAME = Regex(
-    r"^[a-zA-Z][a-zA-Z0-9]*$",
-    error="Environment name {} is invalid: names must only contain alphanumeric characters.",
+    r"^([a-z][a-zA-Z0-9]*|\*)$",
+    error="Environment name {} is invalid: names must only contain lowercase alphanumeric characters, or be the '*' default environment",
     # For values the "error" parameter works and outputs the custom text. For keys the custom text doesn't get reported in the exception for some reason.
 )
 
 range_validator = validate_string(r"^\d+-\d+$")
 seconds_validator = validate_string(r"^\d+s$")
 
 BOOTSTRAP_SCHEMA = Schema(
@@ -276,17 +276,29 @@
     },
 )
 
 NUMBER = Or(int, float)
 DB_DELETION_POLICY = Or("Delete", "Retain", "Snapshot")
 DELETION_POLICY = Or("Delete", "Retain")
 DELETION_PROTECTION = bool
-RDS_PLANS = Or(
-    "tiny", "small", "small-ha", "medium", "medium-ha", "large", "large-ha", "x-large", "x-large-ha"
+POSTGRES_PLANS = Or(
+    "tiny",
+    "small",
+    "small-ha",
+    "small-high-io",
+    "medium",
+    "medium-high-io",
+    "large",
+    "large-ha",
+    "large-high-io",
+    "x-large",
+    "x-large-ha",
+    "x-large-high-io",
 )
+POSTGRES_STORAGE_TYPES = Or("gp2", "gp3", "io1", "io2")
 
 RETENTION_POLICY = Or(
     None,
     {
         "mode": Or("GOVERNANCE", "COMPLIANCE"),
         Or("days", "years", only_one=True): int,
     },
@@ -319,14 +331,15 @@
     Optional("readonly"): bool,
     Optional("services"): Or("__all__", [str]),
     Optional("environments"): {
         ENV_NAME: {
             "bucket_name": validate_s3_bucket_name,
             Optional("deletion_policy"): DELETION_POLICY,
             Optional("retention_policy"): RETENTION_POLICY,
+            Optional("versioning"): bool,
         }
     },
 }
 
 _S3_POLICY_DEFINITION = dict(S3_BASE)
 _S3_POLICY_DEFINITION.update({"type": "s3-policy"})
 S3_POLICY_SCHEMA = Schema(_S3_POLICY_DEFINITION)
@@ -364,27 +377,29 @@
                 "key": str,
                 Optional("body"): str,
             }
         ],
     }
 )
 
-RDS_SCHEMA = Schema(
+POSTGRES_SCHEMA = Schema(
     {
-        "type": "rds-postgres",
+        "type": "postgres",
         "version": NUMBER,
         Optional("deletion_policy"): DB_DELETION_POLICY,
         Optional("environments"): {
             ENV_NAME: {
-                Optional("plan"): RDS_PLANS,
+                Optional("plan"): POSTGRES_PLANS,
                 Optional("volume_size"): int_between(20, 10000),
                 Optional("iops"): int_between(1000, 9950),
                 Optional("snapshot_id"): str,
                 Optional("deletion_policy"): DB_DELETION_POLICY,
                 Optional("deletion_protection"): DELETION_PROTECTION,
+                Optional("multi_az"): bool,
+                Optional("storage_type"): POSTGRES_STORAGE_TYPES,
             }
         },
         Optional("objects"): [
             {
                 "key": str,
                 Optional("body"): str,
             }
@@ -397,14 +412,18 @@
         "type": "redis",
         Optional("environments"): {
             ENV_NAME: {
                 Optional("plan"): REDIS_PLANS,
                 Optional("engine"): REDIS_ENGINE_VERSIONS,
                 Optional("replicas"): int_between(0, 5),
                 Optional("deletion_policy"): DELETION_POLICY,
+                Optional("apply_immediately"): bool,
+                Optional("automatic_failover_enabled"): bool,
+                Optional("instance"): str,
+                Optional("multi_az_enabled"): bool,
             }
         },
     }
 )
 
 OPENSEARCH_MIN_VOLUME_SIZE = 10
 OPENSEARCH_MAX_VOLUME_SIZE = {
@@ -422,17 +441,21 @@
 
 class ConditionalSchema(Schema):
     def validate(self, data, _is_conditional_schema=True):
         data = super(ConditionalSchema, self).validate(data, _is_conditional_schema=False)
         if _is_conditional_schema:
             default_plan = None
             default_volume_size = None
-            if data["environments"].get("default", None):
-                default_plan = data["environments"]["default"].get("plan", None)
-                default_volume_size = data["environments"]["default"].get("volume_size", None)
+
+            default_environment_config = data["environments"].get(
+                "*", data["environments"].get("default", None)
+            )
+            if default_environment_config:
+                default_plan = default_environment_config.get("plan", None)
+                default_volume_size = default_environment_config.get("volume_size", None)
 
             for env in data["environments"]:
                 volume_size = data["environments"][env].get("volume_size", default_volume_size)
                 plan = data["environments"][env].get("plan", default_plan)
 
                 if volume_size:
                     if not plan:
@@ -457,41 +480,65 @@
         "type": "opensearch",
         Optional("environments"): {
             ENV_NAME: {
                 Optional("engine"): OPENSEARCH_ENGINE_VERSIONS,
                 Optional("deletion_policy"): DELETION_POLICY,
                 Optional("plan"): OPENSEARCH_PLANS,
                 Optional("volume_size"): int,
+                Optional("ebs_throughput"): int,
+                Optional("ebs_volume_type"): str,
+                Optional("instance"): str,
+                Optional("instances"): int,
+                Optional("master"): bool,
+                Optional("es_app_log_retention_in_days"): int,
+                Optional("index_slow_log_retention_in_days"): int,
+                Optional("audit_log_retention_in_days"): int,
+                Optional("search_slow_log_retention_in_days"): int,
             }
         },
     }
 )
 
+
 MONITORING_SCHEMA = Schema(
     {
         "type": "monitoring",
         Optional("environments"): {
             ENV_NAME: {
                 Optional("enable_ops_center"): bool,
             }
         },
     }
 )
 
+ALB_SCHEMA = Schema(
+    {
+        "type": "alb",
+        Optional("environments"): {
+            ENV_NAME: {
+                Optional("domain_prefix"): str,
+                Optional("env_root"): str,
+                Optional("cdn_domains_list"): dict,
+            }
+        },
+    }
+)
+
 
 def no_param_schema(schema_type):
     return Schema({"type": schema_type, Optional("services"): Or("__all__", [str])})
 
 
 SCHEMA_MAP = {
     "s3": S3_SCHEMA,
     "s3-policy": S3_POLICY_SCHEMA,
     "aurora-postgres": AURORA_SCHEMA,
-    "rds-postgres": RDS_SCHEMA,
+    "postgres": POSTGRES_SCHEMA,
     "redis": REDIS_SCHEMA,
     "opensearch": OPENSEARCH_SCHEMA,
     "monitoring": MONITORING_SCHEMA,
     "appconfig-ipfilter": no_param_schema("appconfig-ipfilter"),
     "subscription-filter": no_param_schema("subscription-filter"),
     "vpc": no_param_schema("vpc"),
     "xray": no_param_schema("xray"),
+    "alb": ALB_SCHEMA,
 }
```

### Comparing `dbt_platform_helper-6.2.1/dbt_platform_helper/utils/versioning.py` & `dbt_platform_helper-7.0.0/dbt_platform_helper/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/platform_helper.py` & `dbt_platform_helper-7.0.0/platform_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-6.2.1/pyproject.toml` & `dbt_platform_helper-7.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "dbt-platform-helper"
-version = "6.2.1"
+version = "7.0.0"
 description = "Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 license = "MIT"
 readme = "dbt_platform_helper/README.md"
 packages = [
     { include = "dbt_platform_helper" },
     { include = "platform_helper.py" }
@@ -28,15 +28,15 @@
 python = "^3.9"
 schema = "0.7.5"
 cfn-flip = "1.3.0"
 aiohttp = "^3.8.4"
 certifi = "^2023.07.22"
 cryptography = ">=41.0.3,<43.0.0"
 jinja2-simple-tags = "^0.5.0"
-cfn-lint = "^0.80.2"
+cfn-lint = "^0.86.2"
 requests = "^2.31.0"
 prettytable = "^3.9.0"
 semver = "^3.0.2"
 tomlkit = "^0.12.2"
 checkov = "^3.1.67"
 slack-sdk = "^3.27.1"
```

### Comparing `dbt_platform_helper-6.2.1/PKG-INFO` & `dbt_platform_helper-7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-platform-helper
-Version: 6.2.1
+Version: 7.0.0
 Summary: Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot.
 License: MIT
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Requires-Dist: PyYAML (==6.0.1)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: boto3 (>=1.28.24,<2.0.0)
 Requires-Dist: boto3-stubs (>=1.26.148,<2.0.0)
 Requires-Dist: botocore (>=1.29.31,<2.0.0)
 Requires-Dist: certifi (>=2023.07.22,<2024.0.0)
 Requires-Dist: cfn-flip (==1.3.0)
-Requires-Dist: cfn-lint (>=0.80.2,<0.81.0)
+Requires-Dist: cfn-lint (>=0.86.2,<0.87.0)
 Requires-Dist: checkov (>=3.1.67,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cloudfoundry-client (==1.35.2)
 Requires-Dist: cryptography (>=41.0.3,<43.0.0)
 Requires-Dist: jinja2-simple-tags (>=0.5.0,<0.6.0)
 Requires-Dist: mypy-boto3-codebuild (>=1.26.0.post1,<2.0.0)
 Requires-Dist: prettytable (>=3.9.0,<4.0.0)
```

