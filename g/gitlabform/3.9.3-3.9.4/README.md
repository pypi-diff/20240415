# Comparing `tmp/gitlabform-3.9.3.tar.gz` & `tmp/gitlabform-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlabform-3.9.3.tar", last modified: Sat Apr  6 14:31:21 2024, max compression
+gzip compressed data, was "gitlabform-3.9.4.tar", last modified: Mon Apr 15 15:17:15 2024, max compression
```

## Comparing `gitlabform-3.9.3.tar` & `gitlabform-3.9.4.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.901907 gitlabform-3.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-06 14:31:19.000000 gitlabform-3.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-06 14:31:21.901907 gitlabform-3.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-06 14:31:19.000000 gitlabform-3.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.881907 gitlabform-3.9.3/gitlabform/
--rw-r--r--   0 runner    (1001) docker     (127)    23813 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.885907 gitlabform-3.9.3/gitlabform/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/configuration/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/configuration/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/configuration/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/configuration/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/configuration/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.885907 gitlabform-3.9.3/gitlabform/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/branches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/commits.py
--rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/group_badges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/group_ldap_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/group_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/members.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/merge_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/project_badges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/project_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/project_merge_requests_approvals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/project_protected_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     8115 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/resource_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/gitlab/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.889907 gitlabform-3.9.3/gitlabform/lists/
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/lists/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/lists/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/lists/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.889907 gitlabform-3.9.3/gitlabform/processors/
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/defining_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.889907 gitlabform-3.9.3/gitlabform/processors/group/
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/group/group_badges_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/group/group_ldap_links_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/group/group_members_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/group/group_settings_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/group/group_variables_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/multiple_entities_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.893906 gitlabform-3.9.3/gitlabform/processors/project/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/badges_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/branches_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/deploy_keys_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/files_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/hooks_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/integrations_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/members_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/merge_requests_approval_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/merge_requests_approvals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/project_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/project_push_rules_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/project_settings_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/resource_groups_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/schedules_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/tags_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/project/variables_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.893906 gitlabform-3.9.3/gitlabform/processors/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/shared/protected_environments_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/single_entity_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.893906 gitlabform-3.9.3/gitlabform/processors/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14003 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/util/branch_protector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/processors/util/difference_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-06 14:31:19.000000 gitlabform-3.9.3/gitlabform/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.901907 gitlabform-3.9.3/gitlabform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-06 14:31:21.000000 gitlabform-3.9.3/gitlabform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-06 14:31:21.000000 gitlabform-3.9.3/gitlabform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 14:31:21.000000 gitlabform-3.9.3/gitlabform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-06 14:31:21.000000 gitlabform-3.9.3/gitlabform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-06 14:31:21.000000 gitlabform-3.9.3/gitlabform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 14:31:21.000000 gitlabform-3.9.3/gitlabform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-06 14:31:21.901907 gitlabform-3.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-06 14:31:19.000000 gitlabform-3.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.893906 gitlabform-3.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.893906 gitlabform-3.9.3/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.897907 gitlabform-3.9.3/tests/acceptance/standard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2738 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_archive_project.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5971 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_badges.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3293 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_branches.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8047 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_deploy_keys.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1224 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_deploy_keys_all_projects.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10859 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_files.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1434 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_files_all.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1951 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_files_protected.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3059 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_files_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4136 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_group_badges.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4129 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_group_members_case_insensitive.py
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_group_members_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9639 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_group_members_users.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      882 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_group_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5622 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_group_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_inheritance_break.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10353 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2324 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_members.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2071 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_members_add_group.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2253 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_members_enforce.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2205 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_project_group_members_case_insensitive.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1391 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_project_members_case_insensitve.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_project_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_resource_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1664 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_running.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10507 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_schedules.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5433 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_tags.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      871 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_token_from_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15985 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_transfer_project.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5559 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/acceptance/standard/test_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.897907 gitlabform-3.9.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.901907 gitlabform-3.9.3/tests/unit/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3042 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/configuration/test_case_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/configuration/test_inheritance_break_projects_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/configuration/test_inheritance_break_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/configuration/test_inheritance_break_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/configuration/test_projects_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/configuration/test_skip_groups_skip_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/configuration/test_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/configuration/test_yaml_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:21.901907 gitlabform-3.9.3/tests/unit/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/processors/test_abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/processors/test_branch_protector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/processors/test_difference_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/test_access_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/test_non_empty_configs_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-06 14:31:19.000000 gitlabform-3.9.3/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.370504 gitlabform-3.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-15 15:17:10.000000 gitlabform-3.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-15 15:17:15.370504 gitlabform-3.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-15 15:17:10.000000 gitlabform-3.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.346504 gitlabform-3.9.4/gitlabform/
+-rw-r--r--   0 runner    (1001) docker     (127)    23871 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.346504 gitlabform-3.9.4/gitlabform/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/configuration/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/configuration/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/configuration/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/configuration/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/configuration/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.350504 gitlabform-3.9.4/gitlabform/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/commits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/group_badges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/group_ldap_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/merge_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/project_badges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/project_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/project_merge_requests_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/project_protected_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8115 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/resource_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.350504 gitlabform-3.9.4/gitlabform/lists/
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/lists/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/lists/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/lists/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.354504 gitlabform-3.9.4/gitlabform/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/defining_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.354504 gitlabform-3.9.4/gitlabform/processors/group/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/group/group_badges_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/group/group_ldap_links_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/group/group_members_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/group/group_settings_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/group/group_variables_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/multiple_entities_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.358504 gitlabform-3.9.4/gitlabform/processors/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/badges_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/branches_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/deploy_keys_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/files_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/hooks_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/integrations_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/members_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/merge_requests_approval_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/merge_requests_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/project_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/project_push_rules_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/project_settings_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/resource_groups_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/schedules_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/tags_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/variables_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.358504 gitlabform-3.9.4/gitlabform/processors/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/shared/protected_environments_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/single_entity_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.358504 gitlabform-3.9.4/gitlabform/processors/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14003 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/util/branch_protector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/util/difference_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.366504 gitlabform-3.9.4/gitlabform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-15 15:17:15.000000 gitlabform-3.9.4/gitlabform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-15 15:17:15.000000 gitlabform-3.9.4/gitlabform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:17:15.000000 gitlabform-3.9.4/gitlabform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 15:17:15.000000 gitlabform-3.9.4/gitlabform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 15:17:15.000000 gitlabform-3.9.4/gitlabform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 15:17:15.000000 gitlabform-3.9.4/gitlabform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-15 15:17:15.370504 gitlabform-3.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-15 15:17:10.000000 gitlabform-3.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.358504 gitlabform-3.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.358504 gitlabform-3.9.4/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.362504 gitlabform-3.9.4/tests/acceptance/standard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2738 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_archive_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5971 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_badges.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3293 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_branches.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8047 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_deploy_keys.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1224 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_deploy_keys_all_projects.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10859 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1434 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_files_all.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1951 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_files_protected.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3059 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_files_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4136 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_group_badges.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4129 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_group_members_case_insensitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_group_members_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9639 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_group_members_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      882 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_group_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5622 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_inheritance_break.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10353 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2324 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_members.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2071 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_members_add_group.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2253 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_members_enforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2205 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_project_group_members_case_insensitive.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1391 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_project_members_case_insensitve.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_resource_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2180 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_running.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10507 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_schedules.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5433 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_tags.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      871 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_token_from_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16845 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_transfer_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5559 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.366504 gitlabform-3.9.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.366504 gitlabform-3.9.4/tests/unit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3042 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_case_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_inheritance_break_projects_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_inheritance_break_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_inheritance_break_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_projects_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_skip_groups_skip_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_yaml_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.366504 gitlabform-3.9.4/tests/unit/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/processors/test_abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/processors/test_branch_protector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/processors/test_difference_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/test_access_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/test_non_empty_configs_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/test_utils.py
```

### Comparing `gitlabform-3.9.3/LICENSE` & `gitlabform-3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/PKG-INFO` & `gitlabform-3.9.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabform
-Version: 3.9.3
+Version: 3.9.4
 Summary: 🏗 Specialized configuration as a code tool for GitLab projects, groups and more using hierarchical configuration written in YAML
 Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors
 Keywords: cli,yaml,gitlab,configuration-as-code
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -28,32 +28,32 @@
 Requires-Dist: luddite==1.0.4
 Requires-Dist: MarkupSafe==2.1.5
 Requires-Dist: mergedeep==1.3.4
 Requires-Dist: packaging==24.0
 Requires-Dist: python-gitlab==4.4.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: ruamel.yaml==0.17.21
-Requires-Dist: types-requests==2.31.0.20240311
+Requires-Dist: types-requests==2.31.0.20240406
 Requires-Dist: yamlpath==3.8.2
 Provides-Extra: test
 Requires-Dist: coverage==7.4.4; extra == "test"
 Requires-Dist: cryptography==42.0.5; extra == "test"
-Requires-Dist: deepdiff==6.7.1; extra == "test"
+Requires-Dist: deepdiff==7.0.1; extra == "test"
 Requires-Dist: mypy==1.9.0; extra == "test"
 Requires-Dist: mypy-extensions==1.0.0; extra == "test"
 Requires-Dist: pre-commit==2.21.0; extra == "test"
 Requires-Dist: pytest==8.1.1; extra == "test"
 Requires-Dist: pytest-cov==5.0.0; extra == "test"
 Requires-Dist: pytest-rerunfailures==14.0; extra == "test"
-Requires-Dist: xkcdpass==1.19.8; extra == "test"
+Requires-Dist: xkcdpass==1.19.9; extra == "test"
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 
-[![version](https://badge.fury.io/py/gitlabform.svg)](https://badge.fury.io/py/gitlabform)
+[![version](https://badge.fury.io/gh/gitlabform%2Fgitlabform.svg)](https://badge.fury.io/gh/gitlabform%2Fgitlabform)
 ![release date](https://img.shields.io/github/release-date/gitlabform/gitlabform)
 [![Downloads](https://static.pepy.tech/badge/gitlabform/month)](https://pepy.tech/project/gitlabform)
 [![code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![codecov](https://codecov.io/gh/gitlabform/gitlabform/branch/main/graph/badge.svg?token=NOMttkpB2A)](https://codecov.io/gh/gitlabform/gitlabform)
 [![gitlabform](https://snyk.io/advisor/python/gitlabform/badge.svg)](https://snyk.io/advisor/python/gitlabform)
 
 <img src="https://raw.githubusercontent.com/gitlabform/gitlabform/main/docs/images/gitlabform-logo.png" width="600px" alt="logo">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlabform Version: 3.9.3 Summary: ð Specialized
+Metadata-Version: 2.1 Name: gitlabform Version: 3.9.4 Summary: ð Specialized
 configuration as a code tool for GitLab projects, groups and more using
 hierarchical configuration written in YAML Home-page: https://
 gitlabform.github.io/gitlabform Author: Greg Dubicki and Contributors Keywords:
 cli,yaml,gitlab,configuration-as-code Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
@@ -13,28 +13,29 @@
 System :: Microsoft :: Windows Classifier: Topic :: Software Development ::
 Version Control :: Git Requires-Python: >=3.8.0 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: certifi Requires-Dist: cli-
 ui==0.17.2 Requires-Dist: ez-yaml==1.2.0 Requires-Dist: Jinja2==3.1.3 Requires-
 Dist: luddite==1.0.4 Requires-Dist: MarkupSafe==2.1.5 Requires-Dist:
 mergedeep==1.3.4 Requires-Dist: packaging==24.0 Requires-Dist: python-
 gitlab==4.4.0 Requires-Dist: requests==2.31.0 Requires-Dist:
-ruamel.yaml==0.17.21 Requires-Dist: types-requests==2.31.0.20240311 Requires-
+ruamel.yaml==0.17.21 Requires-Dist: types-requests==2.31.0.20240406 Requires-
 Dist: yamlpath==3.8.2 Provides-Extra: test Requires-Dist: coverage==7.4.4;
 extra == "test" Requires-Dist: cryptography==42.0.5; extra == "test" Requires-
-Dist: deepdiff==6.7.1; extra == "test" Requires-Dist: mypy==1.9.0; extra ==
+Dist: deepdiff==7.0.1; extra == "test" Requires-Dist: mypy==1.9.0; extra ==
 "test" Requires-Dist: mypy-extensions==1.0.0; extra == "test" Requires-Dist:
 pre-commit==2.21.0; extra == "test" Requires-Dist: pytest==8.1.1; extra ==
 "test" Requires-Dist: pytest-cov==5.0.0; extra == "test" Requires-Dist: pytest-
-rerunfailures==14.0; extra == "test" Requires-Dist: xkcdpass==1.19.8; extra ==
+rerunfailures==14.0; extra == "test" Requires-Dist: xkcdpass==1.19.9; extra ==
 "test" Provides-Extra: docs Requires-Dist: mkdocs; extra == "docs" Requires-
-Dist: mkdocs-material; extra == "docs" [![version](https://badge.fury.io/py/
-gitlabform.svg)](https://badge.fury.io/py/gitlabform) ![release date](https://
-img.shields.io/github/release-date/gitlabform/gitlabform) [![Downloads](https:/
-/static.pepy.tech/badge/gitlabform/month)](https://pepy.tech/project/
-gitlabform) [![code style](https://img.shields.io/badge/code%20style-black-
-000000.svg)](https://github.com/psf/black) [![codecov](https://codecov.io/gh/
-gitlabform/gitlabform/branch/main/graph/badge.svg?token=NOMttkpB2A)](https://
-codecov.io/gh/gitlabform/gitlabform) [![gitlabform](https://snyk.io/advisor/
-python/gitlabform/badge.svg)](https://snyk.io/advisor/python/gitlabform)
-[logo]ð GitLabForm is a specialized configuration as a code tool for GitLab
-projects, groups and more using hierarchical configuration written in YAML.
-Please see _t_h_e_ _p_r_o_j_e_c_t_ _s_i_t_e for more information.
+Dist: mkdocs-material; extra == "docs" [![version](https://badge.fury.io/gh/
+gitlabform%2Fgitlabform.svg)](https://badge.fury.io/gh/gitlabform%2Fgitlabform)
+![release date](https://img.shields.io/github/release-date/gitlabform/
+gitlabform) [![Downloads](https://static.pepy.tech/badge/gitlabform/month)]
+(https://pepy.tech/project/gitlabform) [![code style](https://img.shields.io/
+badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![codecov]
+(https://codecov.io/gh/gitlabform/gitlabform/branch/main/graph/
+badge.svg?token=NOMttkpB2A)](https://codecov.io/gh/gitlabform/gitlabform) [!
+[gitlabform](https://snyk.io/advisor/python/gitlabform/badge.svg)](https://
+snyk.io/advisor/python/gitlabform) [logo]ð GitLabForm is a specialized
+configuration as a code tool for GitLab projects, groups and more using
+hierarchical configuration written in YAML. Please see _t_h_e_ _p_r_o_j_e_c_t_ _s_i_t_e for
+more information.
```

### Comparing `gitlabform-3.9.3/README.md` & `gitlabform-3.9.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 00000000: 5b21 5b76 6572 7369 6f6e 5d28 6874 7470  [![version](http
 00000010: 733a 2f2f 6261 6467 652e 6675 7279 2e69  s://badge.fury.i
-00000020: 6f2f 7079 2f67 6974 6c61 6266 6f72 6d2e  o/py/gitlabform.
-00000030: 7376 6729 5d28 6874 7470 733a 2f2f 6261  svg)](https://ba
-00000040: 6467 652e 6675 7279 2e69 6f2f 7079 2f67  dge.fury.io/py/g
-00000050: 6974 6c61 6266 6f72 6d29 0a21 5b72 656c  itlabform).![rel
-00000060: 6561 7365 2064 6174 655d 2868 7474 7073  ease date](https
-00000070: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000080: 6f2f 6769 7468 7562 2f72 656c 6561 7365  o/github/release
-00000090: 2d64 6174 652f 6769 746c 6162 666f 726d  -date/gitlabform
-000000a0: 2f67 6974 6c61 6266 6f72 6d29 0a5b 215b  /gitlabform).[![
-000000b0: 446f 776e 6c6f 6164 735d 2868 7474 7073  Downloads](https
-000000c0: 3a2f 2f73 7461 7469 632e 7065 7079 2e74  ://static.pepy.t
-000000d0: 6563 682f 6261 6467 652f 6769 746c 6162  ech/badge/gitlab
-000000e0: 666f 726d 2f6d 6f6e 7468 295d 2868 7474  form/month)](htt
-000000f0: 7073 3a2f 2f70 6570 792e 7465 6368 2f70  ps://pepy.tech/p
-00000100: 726f 6a65 6374 2f67 6974 6c61 6266 6f72  roject/gitlabfor
-00000110: 6d29 0a5b 215b 636f 6465 2073 7479 6c65  m).[![code style
-00000120: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000130: 6965 6c64 732e 696f 2f62 6164 6765 2f63  ields.io/badge/c
-00000140: 6f64 6525 3230 7374 796c 652d 626c 6163  ode%20style-blac
-00000150: 6b2d 3030 3030 3030 2e73 7667 295d 2868  k-000000.svg)](h
-00000160: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000170: 6d2f 7073 662f 626c 6163 6b29 0a5b 215b  m/psf/black).[![
-00000180: 636f 6465 636f 765d 2868 7474 7073 3a2f  codecov](https:/
-00000190: 2f63 6f64 6563 6f76 2e69 6f2f 6768 2f67  /codecov.io/gh/g
-000001a0: 6974 6c61 6266 6f72 6d2f 6769 746c 6162  itlabform/gitlab
-000001b0: 666f 726d 2f62 7261 6e63 682f 6d61 696e  form/branch/main
-000001c0: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
-000001d0: 3f74 6f6b 656e 3d4e 4f4d 7474 6b70 4232  ?token=NOMttkpB2
-000001e0: 4129 5d28 6874 7470 733a 2f2f 636f 6465  A)](https://code
-000001f0: 636f 762e 696f 2f67 682f 6769 746c 6162  cov.io/gh/gitlab
-00000200: 666f 726d 2f67 6974 6c61 6266 6f72 6d29  form/gitlabform)
-00000210: 0a5b 215b 6769 746c 6162 666f 726d 5d28  .[![gitlabform](
-00000220: 6874 7470 733a 2f2f 736e 796b 2e69 6f2f  https://snyk.io/
-00000230: 6164 7669 736f 722f 7079 7468 6f6e 2f67  advisor/python/g
-00000240: 6974 6c61 6266 6f72 6d2f 6261 6467 652e  itlabform/badge.
-00000250: 7376 6729 5d28 6874 7470 733a 2f2f 736e  svg)](https://sn
-00000260: 796b 2e69 6f2f 6164 7669 736f 722f 7079  yk.io/advisor/py
-00000270: 7468 6f6e 2f67 6974 6c61 6266 6f72 6d29  thon/gitlabform)
-00000280: 0a0a 3c69 6d67 2073 7263 3d22 6874 7470  ..<img src="http
-00000290: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-000002a0: 6572 636f 6e74 656e 742e 636f 6d2f 6769  ercontent.com/gi
-000002b0: 746c 6162 666f 726d 2f67 6974 6c61 6266  tlabform/gitlabf
-000002c0: 6f72 6d2f 6d61 696e 2f64 6f63 732f 696d  orm/main/docs/im
-000002d0: 6167 6573 2f67 6974 6c61 6266 6f72 6d2d  ages/gitlabform-
-000002e0: 6c6f 676f 2e70 6e67 2220 7769 6474 683d  logo.png" width=
-000002f0: 2236 3030 7078 2220 616c 743d 226c 6f67  "600px" alt="log
-00000300: 6f22 3e0a 0af0 9f8f 9720 4769 744c 6162  o">...... GitLab
-00000310: 466f 726d 2069 7320 6120 7370 6563 6961  Form is a specia
-00000320: 6c69 7a65 6420 636f 6e66 6967 7572 6174  lized configurat
-00000330: 696f 6e20 6173 2061 2063 6f64 6520 746f  ion as a code to
-00000340: 6f6c 2066 6f72 2047 6974 4c61 6220 7072  ol for GitLab pr
-00000350: 6f6a 6563 7473 2c20 6772 6f75 7073 2061  ojects, groups a
-00000360: 6e64 206d 6f72 650a 7573 696e 6720 6869  nd more.using hi
-00000370: 6572 6172 6368 6963 616c 2063 6f6e 6669  erarchical confi
-00000380: 6775 7261 7469 6f6e 2077 7269 7474 656e  guration written
-00000390: 2069 6e20 5941 4d4c 2e0a 0a50 6c65 6173   in YAML...Pleas
-000003a0: 6520 7365 6520 3c61 2068 7265 663d 2268  e see <a href="h
-000003b0: 7474 7073 3a2f 2f67 6974 6c61 6266 6f72  ttps://gitlabfor
-000003c0: 6d2e 6769 7468 7562 2e69 6f2f 6769 746c  m.github.io/gitl
-000003d0: 6162 666f 726d 2f22 3e74 6865 2070 726f  abform/">the pro
-000003e0: 6a65 6374 2073 6974 653c 2f61 3e20 666f  ject site</a> fo
-000003f0: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
-00000400: 6f6e 2e0a                                on..
+00000020: 6f2f 6768 2f67 6974 6c61 6266 6f72 6d25  o/gh/gitlabform%
+00000030: 3246 6769 746c 6162 666f 726d 2e73 7667  2Fgitlabform.svg
+00000040: 295d 2868 7474 7073 3a2f 2f62 6164 6765  )](https://badge
+00000050: 2e66 7572 792e 696f 2f67 682f 6769 746c  .fury.io/gh/gitl
+00000060: 6162 666f 726d 2532 4667 6974 6c61 6266  abform%2Fgitlabf
+00000070: 6f72 6d29 0a21 5b72 656c 6561 7365 2064  orm).![release d
+00000080: 6174 655d 2868 7474 7073 3a2f 2f69 6d67  ate](https://img
+00000090: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+000000a0: 7562 2f72 656c 6561 7365 2d64 6174 652f  ub/release-date/
+000000b0: 6769 746c 6162 666f 726d 2f67 6974 6c61  gitlabform/gitla
+000000c0: 6266 6f72 6d29 0a5b 215b 446f 776e 6c6f  bform).[![Downlo
+000000d0: 6164 735d 2868 7474 7073 3a2f 2f73 7461  ads](https://sta
+000000e0: 7469 632e 7065 7079 2e74 6563 682f 6261  tic.pepy.tech/ba
+000000f0: 6467 652f 6769 746c 6162 666f 726d 2f6d  dge/gitlabform/m
+00000100: 6f6e 7468 295d 2868 7474 7073 3a2f 2f70  onth)](https://p
+00000110: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
+00000120: 2f67 6974 6c61 6266 6f72 6d29 0a5b 215b  /gitlabform).[![
+00000130: 636f 6465 2073 7479 6c65 5d28 6874 7470  code style](http
+00000140: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000150: 696f 2f62 6164 6765 2f63 6f64 6525 3230  io/badge/code%20
+00000160: 7374 796c 652d 626c 6163 6b2d 3030 3030  style-black-0000
+00000170: 3030 2e73 7667 295d 2868 7474 7073 3a2f  00.svg)](https:/
+00000180: 2f67 6974 6875 622e 636f 6d2f 7073 662f  /github.com/psf/
+00000190: 626c 6163 6b29 0a5b 215b 636f 6465 636f  black).[![codeco
+000001a0: 765d 2868 7474 7073 3a2f 2f63 6f64 6563  v](https://codec
+000001b0: 6f76 2e69 6f2f 6768 2f67 6974 6c61 6266  ov.io/gh/gitlabf
+000001c0: 6f72 6d2f 6769 746c 6162 666f 726d 2f62  orm/gitlabform/b
+000001d0: 7261 6e63 682f 6d61 696e 2f67 7261 7068  ranch/main/graph
+000001e0: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
+000001f0: 3d4e 4f4d 7474 6b70 4232 4129 5d28 6874  =NOMttkpB2A)](ht
+00000200: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00000210: 2f67 682f 6769 746c 6162 666f 726d 2f67  /gh/gitlabform/g
+00000220: 6974 6c61 6266 6f72 6d29 0a5b 215b 6769  itlabform).[![gi
+00000230: 746c 6162 666f 726d 5d28 6874 7470 733a  tlabform](https:
+00000240: 2f2f 736e 796b 2e69 6f2f 6164 7669 736f  //snyk.io/adviso
+00000250: 722f 7079 7468 6f6e 2f67 6974 6c61 6266  r/python/gitlabf
+00000260: 6f72 6d2f 6261 6467 652e 7376 6729 5d28  orm/badge.svg)](
+00000270: 6874 7470 733a 2f2f 736e 796b 2e69 6f2f  https://snyk.io/
+00000280: 6164 7669 736f 722f 7079 7468 6f6e 2f67  advisor/python/g
+00000290: 6974 6c61 6266 6f72 6d29 0a0a 3c69 6d67  itlabform)..<img
+000002a0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+000002b0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+000002c0: 656e 742e 636f 6d2f 6769 746c 6162 666f  ent.com/gitlabfo
+000002d0: 726d 2f67 6974 6c61 6266 6f72 6d2f 6d61  rm/gitlabform/ma
+000002e0: 696e 2f64 6f63 732f 696d 6167 6573 2f67  in/docs/images/g
+000002f0: 6974 6c61 6266 6f72 6d2d 6c6f 676f 2e70  itlabform-logo.p
+00000300: 6e67 2220 7769 6474 683d 2236 3030 7078  ng" width="600px
+00000310: 2220 616c 743d 226c 6f67 6f22 3e0a 0af0  " alt="logo">...
+00000320: 9f8f 9720 4769 744c 6162 466f 726d 2069  ... GitLabForm i
+00000330: 7320 6120 7370 6563 6961 6c69 7a65 6420  s a specialized 
+00000340: 636f 6e66 6967 7572 6174 696f 6e20 6173  configuration as
+00000350: 2061 2063 6f64 6520 746f 6f6c 2066 6f72   a code tool for
+00000360: 2047 6974 4c61 6220 7072 6f6a 6563 7473   GitLab projects
+00000370: 2c20 6772 6f75 7073 2061 6e64 206d 6f72  , groups and mor
+00000380: 650a 7573 696e 6720 6869 6572 6172 6368  e.using hierarch
+00000390: 6963 616c 2063 6f6e 6669 6775 7261 7469  ical configurati
+000003a0: 6f6e 2077 7269 7474 656e 2069 6e20 5941  on written in YA
+000003b0: 4d4c 2e0a 0a50 6c65 6173 6520 7365 6520  ML...Please see 
+000003c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000003d0: 2f67 6974 6c61 6266 6f72 6d2e 6769 7468  /gitlabform.gith
+000003e0: 7562 2e69 6f2f 6769 746c 6162 666f 726d  ub.io/gitlabform
+000003f0: 2f22 3e74 6865 2070 726f 6a65 6374 2073  /">the project s
+00000400: 6974 653c 2f61 3e20 666f 7220 6d6f 7265  ite</a> for more
+00000410: 2069 6e66 6f72 6d61 7469 6f6e 2e0a        information..
```

### Comparing `gitlabform-3.9.3/gitlabform/__init__.py` & `gitlabform-3.9.4/gitlabform/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,26 +43,32 @@
 from gitlabform.lists.projects import ProjectsProvider
 from gitlabform.output import EffectiveConfigurationFile
 from gitlabform.processors.group import GroupProcessors
 from gitlabform.processors.project import ProjectProcessors
 
 
 class GitLabForm:
-    def __init__(self, include_archived_projects=True, target=None, config_string=None):
+    def __init__(
+        self,
+        include_archived_projects=True,
+        target=None,
+        config_string=None,
+        noop=False,
+    ):
         if target and config_string:
             # this mode is basically only for testing
 
             self.target = target
             self.config_string = config_string
             self.verbose = True
             self.debug = True
             self.strict = True
             self.start_from = 1
             self.start_from_group = 1
-            self.noop = False
+            self.noop = noop
             self.output_file = None
             self.skip_version_check = True
             self.include_archived_projects = include_archived_projects
             self.just_show_version = False
             self.terminate_after_error = True
             self.only_sections = "all"
```

### Comparing `gitlabform-3.9.3/gitlabform/configuration/common.py` & `gitlabform-3.9.4/gitlabform/configuration/common.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/configuration/core.py` & `gitlabform-3.9.4/gitlabform/configuration/core.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/configuration/groups.py` & `gitlabform-3.9.4/gitlabform/configuration/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/configuration/projects.py` & `gitlabform-3.9.4/gitlabform/configuration/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/configuration/transform.py` & `gitlabform-3.9.4/gitlabform/configuration/transform.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/__init__.py` & `gitlabform-3.9.4/gitlabform/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/branches.py` & `gitlabform-3.9.4/gitlabform/gitlab/branches.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/commits.py` & `gitlabform-3.9.4/gitlabform/gitlab/commits.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/core.py` & `gitlabform-3.9.4/gitlabform/gitlab/core.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/group_badges.py` & `gitlabform-3.9.4/gitlabform/gitlab/group_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/group_ldap_links.py` & `gitlabform-3.9.4/gitlabform/gitlab/group_ldap_links.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/group_variables.py` & `gitlabform-3.9.4/gitlabform/gitlab/group_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/groups.py` & `gitlabform-3.9.4/gitlabform/gitlab/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/integrations.py` & `gitlabform-3.9.4/gitlabform/gitlab/integrations.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/members.py` & `gitlabform-3.9.4/gitlabform/gitlab/members.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/merge_requests.py` & `gitlabform-3.9.4/gitlabform/gitlab/merge_requests.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/pipelines.py` & `gitlabform-3.9.4/gitlabform/gitlab/pipelines.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/project_badges.py` & `gitlabform-3.9.4/gitlabform/gitlab/project_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/project_deploy_keys.py` & `gitlabform-3.9.4/gitlabform/gitlab/project_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/project_merge_requests_approvals.py` & `gitlabform-3.9.4/gitlabform/gitlab/project_merge_requests_approvals.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/project_protected_environments.py` & `gitlabform-3.9.4/gitlabform/gitlab/project_protected_environments.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/projects.py` & `gitlabform-3.9.4/gitlabform/gitlab/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/repositories.py` & `gitlabform-3.9.4/gitlabform/gitlab/repositories.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/resource_groups.py` & `gitlabform-3.9.4/gitlabform/gitlab/resource_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/schedules.py` & `gitlabform-3.9.4/gitlabform/gitlab/schedules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/users.py` & `gitlabform-3.9.4/gitlabform/gitlab/users.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/gitlab/variables.py` & `gitlabform-3.9.4/gitlabform/gitlab/variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/lists/__init__.py` & `gitlabform-3.9.4/gitlabform/lists/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/lists/filter.py` & `gitlabform-3.9.4/gitlabform/lists/filter.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/lists/groups.py` & `gitlabform-3.9.4/gitlabform/lists/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/lists/projects.py` & `gitlabform-3.9.4/gitlabform/lists/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/output.py` & `gitlabform-3.9.4/gitlabform/output.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/__init__.py` & `gitlabform-3.9.4/gitlabform/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/abstract_processor.py` & `gitlabform-3.9.4/gitlabform/processors/abstract_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,24 @@
                 )
                 return
 
             if dry_run:
                 verbose(
                     f"Processing section '{self.configuration_name}' in dry-run mode."
                 )
+                try:
+                    project_transfer_source = configuration["project"]["transfer_from"]
+                    verbose(
+                        f"""Project {project_or_project_and_group} is configured to be transferred, 
+                        diffing config from transfer source project {project_transfer_source}."""
+                    )
+                    project_or_project_and_group = project_transfer_source
+                except KeyError:
+                    pass
+
                 self._print_diff(
                     project_or_project_and_group,
                     configuration.get(self.configuration_name),
                 )
             else:
                 verbose(f"Processing section '{self.configuration_name}'")
                 if self._can_proceed(project_or_project_and_group, configuration):
```

### Comparing `gitlabform-3.9.3/gitlabform/processors/defining_keys.py` & `gitlabform-3.9.4/gitlabform/processors/defining_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/group/__init__.py` & `gitlabform-3.9.4/gitlabform/processors/group/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/group/group_badges_processor.py` & `gitlabform-3.9.4/gitlabform/processors/group/group_badges_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/group/group_ldap_links_processor.py` & `gitlabform-3.9.4/gitlabform/processors/group/group_ldap_links_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/group/group_members_processor.py` & `gitlabform-3.9.4/gitlabform/processors/group/group_members_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/group/group_variables_processor.py` & `gitlabform-3.9.4/gitlabform/processors/group/group_variables_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/multiple_entities_processor.py` & `gitlabform-3.9.4/gitlabform/processors/multiple_entities_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/__init__.py` & `gitlabform-3.9.4/gitlabform/processors/project/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/badges_processor.py` & `gitlabform-3.9.4/gitlabform/processors/project/badges_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/branches_processor.py` & `gitlabform-3.9.4/gitlabform/processors/project/branches_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/deploy_keys_processor.py` & `gitlabform-3.9.4/gitlabform/processors/project/deploy_keys_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/files_processor.py` & `gitlabform-3.9.4/gitlabform/processors/project/files_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/hooks_processor.py` & `gitlabform-3.9.4/gitlabform/processors/project/hooks_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/integrations_processor.py` & `gitlabform-3.9.4/gitlabform/processors/project/integrations_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/members_processor.py` & `gitlabform-3.9.4/gitlabform/processors/project/members_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/merge_requests_approval_rules.py` & `gitlabform-3.9.4/gitlabform/processors/project/merge_requests_approval_rules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/merge_requests_approvals.py` & `gitlabform-3.9.4/gitlabform/processors/project/merge_requests_approvals.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/project_processor.py` & `gitlabform-3.9.4/gitlabform/processors/project/project_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/resource_groups_processor.py` & `gitlabform-3.9.4/gitlabform/processors/project/resource_groups_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/schedules_processor.py` & `gitlabform-3.9.4/gitlabform/processors/project/schedules_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/tags_processor.py` & `gitlabform-3.9.4/gitlabform/processors/project/tags_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/project/variables_processor.py` & `gitlabform-3.9.4/gitlabform/processors/project/variables_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/shared/protected_environments_processor.py` & `gitlabform-3.9.4/gitlabform/processors/shared/protected_environments_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/single_entity_processor.py` & `gitlabform-3.9.4/gitlabform/processors/single_entity_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/util/branch_protector.py` & `gitlabform-3.9.4/gitlabform/processors/util/branch_protector.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/util/decorators.py` & `gitlabform-3.9.4/gitlabform/processors/util/decorators.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform/processors/util/difference_logger.py` & `gitlabform-3.9.4/gitlabform/processors/util/difference_logger.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/gitlabform.egg-info/PKG-INFO` & `gitlabform-3.9.4/gitlabform.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabform
-Version: 3.9.3
+Version: 3.9.4
 Summary: 🏗 Specialized configuration as a code tool for GitLab projects, groups and more using hierarchical configuration written in YAML
 Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors
 Keywords: cli,yaml,gitlab,configuration-as-code
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -28,32 +28,32 @@
 Requires-Dist: luddite==1.0.4
 Requires-Dist: MarkupSafe==2.1.5
 Requires-Dist: mergedeep==1.3.4
 Requires-Dist: packaging==24.0
 Requires-Dist: python-gitlab==4.4.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: ruamel.yaml==0.17.21
-Requires-Dist: types-requests==2.31.0.20240311
+Requires-Dist: types-requests==2.31.0.20240406
 Requires-Dist: yamlpath==3.8.2
 Provides-Extra: test
 Requires-Dist: coverage==7.4.4; extra == "test"
 Requires-Dist: cryptography==42.0.5; extra == "test"
-Requires-Dist: deepdiff==6.7.1; extra == "test"
+Requires-Dist: deepdiff==7.0.1; extra == "test"
 Requires-Dist: mypy==1.9.0; extra == "test"
 Requires-Dist: mypy-extensions==1.0.0; extra == "test"
 Requires-Dist: pre-commit==2.21.0; extra == "test"
 Requires-Dist: pytest==8.1.1; extra == "test"
 Requires-Dist: pytest-cov==5.0.0; extra == "test"
 Requires-Dist: pytest-rerunfailures==14.0; extra == "test"
-Requires-Dist: xkcdpass==1.19.8; extra == "test"
+Requires-Dist: xkcdpass==1.19.9; extra == "test"
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 
-[![version](https://badge.fury.io/py/gitlabform.svg)](https://badge.fury.io/py/gitlabform)
+[![version](https://badge.fury.io/gh/gitlabform%2Fgitlabform.svg)](https://badge.fury.io/gh/gitlabform%2Fgitlabform)
 ![release date](https://img.shields.io/github/release-date/gitlabform/gitlabform)
 [![Downloads](https://static.pepy.tech/badge/gitlabform/month)](https://pepy.tech/project/gitlabform)
 [![code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![codecov](https://codecov.io/gh/gitlabform/gitlabform/branch/main/graph/badge.svg?token=NOMttkpB2A)](https://codecov.io/gh/gitlabform/gitlabform)
 [![gitlabform](https://snyk.io/advisor/python/gitlabform/badge.svg)](https://snyk.io/advisor/python/gitlabform)
 
 <img src="https://raw.githubusercontent.com/gitlabform/gitlabform/main/docs/images/gitlabform-logo.png" width="600px" alt="logo">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlabform Version: 3.9.3 Summary: ð Specialized
+Metadata-Version: 2.1 Name: gitlabform Version: 3.9.4 Summary: ð Specialized
 configuration as a code tool for GitLab projects, groups and more using
 hierarchical configuration written in YAML Home-page: https://
 gitlabform.github.io/gitlabform Author: Greg Dubicki and Contributors Keywords:
 cli,yaml,gitlab,configuration-as-code Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
@@ -13,28 +13,29 @@
 System :: Microsoft :: Windows Classifier: Topic :: Software Development ::
 Version Control :: Git Requires-Python: >=3.8.0 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: certifi Requires-Dist: cli-
 ui==0.17.2 Requires-Dist: ez-yaml==1.2.0 Requires-Dist: Jinja2==3.1.3 Requires-
 Dist: luddite==1.0.4 Requires-Dist: MarkupSafe==2.1.5 Requires-Dist:
 mergedeep==1.3.4 Requires-Dist: packaging==24.0 Requires-Dist: python-
 gitlab==4.4.0 Requires-Dist: requests==2.31.0 Requires-Dist:
-ruamel.yaml==0.17.21 Requires-Dist: types-requests==2.31.0.20240311 Requires-
+ruamel.yaml==0.17.21 Requires-Dist: types-requests==2.31.0.20240406 Requires-
 Dist: yamlpath==3.8.2 Provides-Extra: test Requires-Dist: coverage==7.4.4;
 extra == "test" Requires-Dist: cryptography==42.0.5; extra == "test" Requires-
-Dist: deepdiff==6.7.1; extra == "test" Requires-Dist: mypy==1.9.0; extra ==
+Dist: deepdiff==7.0.1; extra == "test" Requires-Dist: mypy==1.9.0; extra ==
 "test" Requires-Dist: mypy-extensions==1.0.0; extra == "test" Requires-Dist:
 pre-commit==2.21.0; extra == "test" Requires-Dist: pytest==8.1.1; extra ==
 "test" Requires-Dist: pytest-cov==5.0.0; extra == "test" Requires-Dist: pytest-
-rerunfailures==14.0; extra == "test" Requires-Dist: xkcdpass==1.19.8; extra ==
+rerunfailures==14.0; extra == "test" Requires-Dist: xkcdpass==1.19.9; extra ==
 "test" Provides-Extra: docs Requires-Dist: mkdocs; extra == "docs" Requires-
-Dist: mkdocs-material; extra == "docs" [![version](https://badge.fury.io/py/
-gitlabform.svg)](https://badge.fury.io/py/gitlabform) ![release date](https://
-img.shields.io/github/release-date/gitlabform/gitlabform) [![Downloads](https:/
-/static.pepy.tech/badge/gitlabform/month)](https://pepy.tech/project/
-gitlabform) [![code style](https://img.shields.io/badge/code%20style-black-
-000000.svg)](https://github.com/psf/black) [![codecov](https://codecov.io/gh/
-gitlabform/gitlabform/branch/main/graph/badge.svg?token=NOMttkpB2A)](https://
-codecov.io/gh/gitlabform/gitlabform) [![gitlabform](https://snyk.io/advisor/
-python/gitlabform/badge.svg)](https://snyk.io/advisor/python/gitlabform)
-[logo]ð GitLabForm is a specialized configuration as a code tool for GitLab
-projects, groups and more using hierarchical configuration written in YAML.
-Please see _t_h_e_ _p_r_o_j_e_c_t_ _s_i_t_e for more information.
+Dist: mkdocs-material; extra == "docs" [![version](https://badge.fury.io/gh/
+gitlabform%2Fgitlabform.svg)](https://badge.fury.io/gh/gitlabform%2Fgitlabform)
+![release date](https://img.shields.io/github/release-date/gitlabform/
+gitlabform) [![Downloads](https://static.pepy.tech/badge/gitlabform/month)]
+(https://pepy.tech/project/gitlabform) [![code style](https://img.shields.io/
+badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![codecov]
+(https://codecov.io/gh/gitlabform/gitlabform/branch/main/graph/
+badge.svg?token=NOMttkpB2A)](https://codecov.io/gh/gitlabform/gitlabform) [!
+[gitlabform](https://snyk.io/advisor/python/gitlabform/badge.svg)](https://
+snyk.io/advisor/python/gitlabform) [logo]ð GitLabForm is a specialized
+configuration as a code tool for GitLab projects, groups and more using
+hierarchical configuration written in YAML. Please see _t_h_e_ _p_r_o_j_e_c_t_ _s_i_t_e for
+more information.
```

### Comparing `gitlabform-3.9.3/gitlabform.egg-info/SOURCES.txt` & `gitlabform-3.9.4/gitlabform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/setup.py` & `gitlabform-3.9.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,29 +51,29 @@
         "luddite==1.0.4",
         "MarkupSafe==2.1.5",
         "mergedeep==1.3.4",
         "packaging==24.0",
         "python-gitlab==4.4.0",
         "requests==2.31.0",
         "ruamel.yaml==0.17.21",
-        "types-requests==2.31.0.20240311",
+        "types-requests==2.31.0.20240406",
         "yamlpath==3.8.2",
     ],
     extras_require={
         "test": [
             "coverage==7.4.4",
             "cryptography==42.0.5",
-            "deepdiff==6.7.1",
+            "deepdiff==7.0.1",
             "mypy==1.9.0",
             "mypy-extensions==1.0.0",
             "pre-commit==2.21.0",  # not really for tests, but for development
             "pytest==8.1.1",
             "pytest-cov==5.0.0",
             "pytest-rerunfailures==14.0",
-            "xkcdpass==1.19.8",
+            "xkcdpass==1.19.9",
         ],
         "docs": [
             "mkdocs",
             "mkdocs-material",
         ],
     },
     entry_points={
```

### Comparing `gitlabform-3.9.3/tests/acceptance/__init__.py` & `gitlabform-3.9.4/tests/acceptance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
     )
 
 
 def randomize_case(input: str) -> str:
     return "".join(random.choice((str.upper, str.lower))(char) for char in input)
 
 
-def run_gitlabform(config, target, include_archived_projects=True):
+def run_gitlabform(config, target, include_archived_projects=True, noop=False):
     # f-strings with """ used as configs have the disadvantage of having indentation in them - let's remove it here
     config = textwrap.dedent(config)
 
     # we don't want to repeat ourselves in the tests, so prefix the configs with this mandatory part here
     config = CONFIG + config
 
     # allow passing in gitlab RESTObjects. assume full path string otherwise
@@ -260,9 +260,10 @@
     elif isinstance(target, Project):
         target = target.path_with_namespace
 
     gf = GitLabForm(
         include_archived_projects=include_archived_projects,
         config_string=config,
         target=target,
+        noop=noop,
     )
     gf.run()
```

### Comparing `gitlabform-3.9.3/tests/acceptance/conftest.py` & `gitlabform-3.9.4/tests/acceptance/conftest.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_archive_project.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_archive_project.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_badges.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_branches.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_branches.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_deploy_keys.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_deploy_keys_all_projects.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_deploy_keys_all_projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_files.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_files.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_files_all.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_files_all.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_files_protected.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_files_protected.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_files_templates.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_files_templates.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_group_badges.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_group_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_group_members_case_insensitive.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_group_members_case_insensitive.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_group_members_groups.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_group_members_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_group_members_users.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_group_members_users.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_group_settings.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_group_settings.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_group_variables.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_group_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_hooks.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_hooks.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_inheritance_break.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_inheritance_break.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_integrations.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_integrations.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_members.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_members.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_members_add_group.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_members_add_group.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_members_enforce.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_members_enforce.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_project_group_members_case_insensitive.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_project_group_members_case_insensitive.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_project_members_case_insensitve.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_project_members_case_insensitve.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_project_settings.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_project_settings.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_resource_groups.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_resource_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_running.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_running.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,31 @@
         project = gl.projects.get(project.id)
         assert project.request_access_enabled is True
 
         other_project = gl.projects.get(other_project.id)
         assert other_project.request_access_enabled is True
 
     # noinspection PyPep8Naming
+    def test__ALL_dry_run(self, gl, project, other_project):
+        config = f"""
+        projects_and_groups:
+          '*':
+            project_settings:
+              request_access_enabled: false
+        """
+
+        run_gitlabform(config, "ALL", noop=True)
+
+        project = gl.projects.get(project.id)
+        assert project.request_access_enabled is True
+
+        other_project = gl.projects.get(other_project.id)
+        assert other_project.request_access_enabled is True
+
+    # noinspection PyPep8Naming
     def test__ALL_DEFINED(self, gl, project, other_project):
         config = f"""
         projects_and_groups:
           {project.path_with_namespace}:
             project_settings:
               suggestion_commit_message: 'foobar'
         """
```

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_schedules.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_schedules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_tags.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_tags.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_token_from_config.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_token_from_config.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_transfer_project.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_transfer_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,38 @@
 from gitlabform.gitlab import AccessLevel
 from gitlab import GitlabTransferProjectError
 import re
 import pytest
 
 
 class TestTransferProject:
+    def test__transfer_between_two_root_groups_dry_run(
+        self, project_for_function, group, other_group
+    ):
+        project_new_path_with_namespace = (
+            f"{other_group.path}/{project_for_function.name}"
+        )
+        projects_in_destination_before_transfer = other_group.projects.list()
+
+        config = f"""
+        projects_and_groups:
+          {project_new_path_with_namespace}:
+            project:
+              transfer_from: {project_for_function.path_with_namespace}
+            project_settings:
+              description: test
+        """
+
+        run_gitlabform(config, project_new_path_with_namespace, noop=True)
+        projects_in_destination_after_transfer = other_group.projects.list()
+
+        assert len(projects_in_destination_after_transfer) == len(
+            projects_in_destination_before_transfer
+        )
+
     def test__transfer_between_two_root_groups(
         self, project_for_function, group, other_group
     ):
         project_new_path_with_namespace = (
             f"{other_group.path}/{project_for_function.name}"
         )
         projects_in_destination_before_transfer = other_group.projects.list()
```

### Comparing `gitlabform-3.9.3/tests/acceptance/standard/test_variables.py` & `gitlabform-3.9.4/tests/acceptance/standard/test_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/unit/configuration/test_case_sensitivity.py` & `gitlabform-3.9.4/tests/unit/configuration/test_case_sensitivity.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/unit/configuration/test_inheritance_break_projects_and_groups.py` & `gitlabform-3.9.4/tests/unit/configuration/test_inheritance_break_projects_and_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/unit/configuration/test_inheritance_break_subgroups.py` & `gitlabform-3.9.4/tests/unit/configuration/test_inheritance_break_subgroups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/unit/configuration/test_inheritance_break_validation.py` & `gitlabform-3.9.4/tests/unit/configuration/test_inheritance_break_validation.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/unit/configuration/test_projects_and_groups.py` & `gitlabform-3.9.4/tests/unit/configuration/test_projects_and_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/unit/configuration/test_skip_groups_skip_projects.py` & `gitlabform-3.9.4/tests/unit/configuration/test_skip_groups_skip_projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/unit/configuration/test_subgroups.py` & `gitlabform-3.9.4/tests/unit/configuration/test_subgroups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/unit/configuration/test_yaml_version.py` & `gitlabform-3.9.4/tests/unit/configuration/test_yaml_version.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/unit/processors/test_abstract_processor.py` & `gitlabform-3.9.4/tests/unit/processors/test_abstract_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/unit/processors/test_branch_protector.py` & `gitlabform-3.9.4/tests/unit/processors/test_branch_protector.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/unit/processors/test_difference_logger.py` & `gitlabform-3.9.4/tests/unit/processors/test_difference_logger.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/unit/test_access_levels.py` & `gitlabform-3.9.4/tests/unit/test_access_levels.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/unit/test_non_empty_configs_provider.py` & `gitlabform-3.9.4/tests/unit/test_non_empty_configs_provider.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.3/tests/unit/test_utils.py` & `gitlabform-3.9.4/tests/unit/test_utils.py`

 * *Files identical despite different names*

