# Comparing `tmp/hapi_schema-0.6.2.tar.gz` & `tmp/hapi_schema-0.7.0.tar.gz`

## Comparing `hapi_schema-0.6.2.tar` & `hapi_schema-0.7.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/changelog.md
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/contributing.md
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/.config/coveragerc
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/.config/pytest.ini
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/.config/ruff.toml
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/_version.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_admin1.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_admin2.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_age_range.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_dataset.py
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_food_security.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_gender.py
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_humanitarian_needs.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_ipc_phase.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_ipc_type.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_location.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_national_risk.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_operational_presence.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_org.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_org_type.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_population.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_population_group.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_population_status.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_resource.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/db_sector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/utils/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/utils/base.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/src/hapi_schema/utils/view_params.py
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/conftest.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_admin1_view.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_admin2_view.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_age_range_view.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_dataset_view.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_food_security_view.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_gender_view.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_humanitarian_needs_view.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_ipc_phase_view.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_ipc_type_view.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_location_view.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_national_risk_view.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_operational_presence_view.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_org_type_view.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_org_view.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_population_group_view.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_population_status_view.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_population_view.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_resource_view.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/test_sector_view.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/__init__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_admin1.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_admin2.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_age_range.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_dataset.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_food_security.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_gender.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_humanitarian_needs.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_ipc_phase.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_ipc_type.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_location.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_national_risk.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_operational_presence.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_org.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_org_type.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_population.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_population_group.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_population_status.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_resource.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/tests/sample_data/data_sector.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/LICENSE
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/README.md
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 hapi_schema-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/changelog.md
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/contributing.md
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/.config/coveragerc
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/.config/pytest.ini
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/.config/ruff.toml
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/_version.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_admin1.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_admin2.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_age_range.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_dataset.py
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_food_security.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_gender.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_humanitarian_needs.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_ipc_phase.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_ipc_type.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_location.py
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_national_risk.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_operational_presence.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_org.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_org_type.py
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_population.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_population_group.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_population_status.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_resource.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/db_sector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/utils/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/utils/base.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/src/hapi_schema/utils/view_params.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_admin1.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_admin2.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_age_range.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_dataset.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_food_security.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_gender.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_humanitarian_needs.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_ipc_phase.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_ipc_type.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_location.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_national_risk.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_operational_presence.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_org.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_org_type.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_population.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_population_group.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_population_status.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_resource.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/test_sector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/__init__.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_admin1.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_admin2.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_age_range.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_dataset.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_food_security.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_gender.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_humanitarian_needs.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_ipc_phase.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_ipc_type.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_location.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_national_risk.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_operational_presence.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_org.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_org_type.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_population.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_population_group.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_population_status.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_resource.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/tests/sample_data/data_sector.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/LICENSE
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/README.md
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 hapi_schema-0.7.0/PKG-INFO
```

### Comparing `hapi_schema-0.6.2/changelog.md` & `hapi_schema-0.7.0/changelog.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.7.0]
+
+### Added
+- Missing constraints
+- Tests on the constraints
+- `hapi_updated_date` and `hapi_replaced_date` fields
+
+### Changed
+
+- Small changes to other dates for HAPI v2
+
+## [0.6.2]
+
+### Changed
+
+- Update requirements
+
 ## [0.6.1]
 
 ### Changed
 
 - National risk location link
 
 ## [0.6.0]
```

### Comparing `hapi_schema-0.6.2/contributing.md` & `hapi_schema-0.7.0/contributing.md`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/requirements.txt` & `hapi_schema-0.7.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/.config/pre-commit-config.yaml` & `hapi_schema-0.7.0/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/.github/workflows/publish.yaml` & `hapi_schema-0.7.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/.github/workflows/run-python-tests.yaml` & `hapi_schema-0.7.0/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_admin1.py` & `hapi_schema-0.7.0/src/hapi_schema/db_admin2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,90 @@
-"""Admin1 table and view."""
+"""Admin2 table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
     Boolean,
+    CheckConstraint,
     DateTime,
     ForeignKey,
     Integer,
     String,
+    UniqueConstraint,
     select,
     text,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
+from hapi_schema.db_admin1 import DBAdmin1
 from hapi_schema.db_location import DBLocation
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.view_params import ViewParams
 
 
-class DBAdmin1(Base):
-    __tablename__ = "admin1"
+class DBAdmin2(Base):
+    __tablename__ = "admin2"
+    __table_args__ = (
+        CheckConstraint(
+            "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
+            name="reference_period",
+        ),
+        CheckConstraint(
+            "(hapi_replaced_date IS NULL) OR (hapi_replaced_date >= hapi_updated_date)",
+            name="hapi_dates",
+        ),
+        UniqueConstraint("code", "hapi_updated_date", name="code_date_unique"),
+    )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    location_ref: Mapped[int] = mapped_column(
-        ForeignKey("location.id", onupdate="CASCADE", ondelete="CASCADE"),
+    admin1_ref: Mapped[int] = mapped_column(
+        ForeignKey("admin1.id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
-    code: Mapped[str] = mapped_column(String(128), unique=True, nullable=False)
+    code: Mapped[str] = mapped_column(String(128), nullable=False)
     name: Mapped[str] = mapped_column(String(512), nullable=False)
     is_unspecified: Mapped[bool] = mapped_column(
         Boolean, server_default=text("FALSE")
     )
     reference_period_start: Mapped[datetime] = mapped_column(
-        DateTime, nullable=False
+        DateTime, nullable=True, server_default=text("NULL"), index=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL")
+        DateTime, nullable=True, server_default=text("NULL"), index=True
     )
 
-    location = relationship("DBLocation")
+    hapi_updated_date = mapped_column(DateTime, nullable=False, index=True)
+    hapi_replaced_date: Mapped[datetime] = mapped_column(
+        DateTime, nullable=True, server_default=text("NULL"), index=True
+    )
 
+    admin1 = relationship("DBAdmin1")
 
-view_params_admin1 = ViewParams(
-    name="admin1_view",
+
+view_params_admin2 = ViewParams(
+    name="admin2_view",
     metadata=Base.metadata,
     selectable=select(
-        *DBAdmin1.__table__.columns,
+        *DBAdmin2.__table__.columns,
+        DBAdmin1.code.label("admin1_code"),
+        DBAdmin1.name.label("admin1_name"),
+        DBAdmin1.is_unspecified.label("admin1_is_unspecified"),
+        DBAdmin1.reference_period_start.label("admin1_reference_period_start"),
+        DBAdmin1.reference_period_end.label("admin1_reference_period_end"),
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
         DBLocation.reference_period_start.label(
             "location_reference_period_start"
         ),
         DBLocation.reference_period_end.label("location_reference_period_end"),
     ).select_from(
-        DBAdmin1.__table__.join(
+        DBAdmin2.__table__.join(
+            DBAdmin1.__table__,
+            DBAdmin2.admin1_ref == DBAdmin1.id,
+            isouter=True,
+        ).join(
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
-        )
+        ),
     ),
 )
```

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_admin2.py` & `hapi_schema-0.7.0/src/hapi_schema/db_admin1.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,72 +1,79 @@
-"""Admin2 table and view."""
+"""Admin1 table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
     Boolean,
+    CheckConstraint,
     DateTime,
     ForeignKey,
     Integer,
     String,
+    UniqueConstraint,
     select,
     text,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
-from hapi_schema.db_admin1 import DBAdmin1
 from hapi_schema.db_location import DBLocation
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.view_params import ViewParams
 
 
-class DBAdmin2(Base):
-    __tablename__ = "admin2"
+class DBAdmin1(Base):
+    __tablename__ = "admin1"
+    __table_args__ = (
+        CheckConstraint(
+            "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
+            name="reference_period",
+        ),
+        CheckConstraint(
+            "(hapi_replaced_date IS NULL) OR (hapi_replaced_date >= hapi_updated_date)",
+            name="hapi_dates",
+        ),
+        UniqueConstraint("code", "hapi_updated_date"),
+    )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    admin1_ref: Mapped[int] = mapped_column(
-        ForeignKey("admin1.id", onupdate="CASCADE", ondelete="CASCADE"),
+    location_ref: Mapped[int] = mapped_column(
+        ForeignKey("location.id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
-    code: Mapped[str] = mapped_column(String(128), unique=True, nullable=False)
+    code: Mapped[str] = mapped_column(String(128), nullable=False)
     name: Mapped[str] = mapped_column(String(512), nullable=False)
     is_unspecified: Mapped[bool] = mapped_column(
         Boolean, server_default=text("FALSE")
     )
     reference_period_start: Mapped[datetime] = mapped_column(
-        DateTime, nullable=False
+        DateTime, nullable=True, server_default=text("NULL"), index=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL")
+        DateTime, nullable=True, server_default=text("NULL"), index=True
+    )
+    hapi_updated_date = mapped_column(DateTime, nullable=False, index=True)
+    hapi_replaced_date: Mapped[datetime] = mapped_column(
+        DateTime, nullable=True, server_default=text("NULL"), index=True
     )
 
-    admin1 = relationship("DBAdmin1")
+    location = relationship("DBLocation")
 
 
-view_params_admin2 = ViewParams(
-    name="admin2_view",
+view_params_admin1 = ViewParams(
+    name="admin1_view",
     metadata=Base.metadata,
     selectable=select(
-        *DBAdmin2.__table__.columns,
-        DBAdmin1.code.label("admin1_code"),
-        DBAdmin1.name.label("admin1_name"),
-        DBAdmin1.is_unspecified.label("admin1_is_unspecified"),
-        DBAdmin1.reference_period_start.label("admin1_reference_period_start"),
-        DBAdmin1.reference_period_end.label("admin1_reference_period_end"),
+        *DBAdmin1.__table__.columns,
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
         DBLocation.reference_period_start.label(
             "location_reference_period_start"
         ),
         DBLocation.reference_period_end.label("location_reference_period_end"),
     ).select_from(
-        DBAdmin2.__table__.join(
-            DBAdmin1.__table__,
-            DBAdmin2.admin1_ref == DBAdmin1.id,
-            isouter=True,
-        ).join(
+        DBAdmin1.__table__.join(
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
-        ),
+        )
     ),
 )
```

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_age_range.py` & `hapi_schema-0.7.0/src/hapi_schema/db_age_range.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_dataset.py` & `hapi_schema-0.7.0/src/hapi_schema/db_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_food_security.py` & `hapi_schema-0.7.0/src/hapi_schema/db_national_risk.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,125 +1,123 @@
-"""Population table and view."""
+"""NationalRisk table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
+    CheckConstraint,
     DateTime,
     Float,
     ForeignKey,
     Integer,
     Text,
     select,
     text,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_admin1 import DBAdmin1
 from hapi_schema.db_admin2 import DBAdmin2
 from hapi_schema.db_dataset import DBDataset
-from hapi_schema.db_ipc_phase import DBIpcPhase
-from hapi_schema.db_ipc_type import DBIpcType
 from hapi_schema.db_location import DBLocation
 from hapi_schema.db_resource import DBResource
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.view_params import ViewParams
 
 
-class DBFoodSecurity(Base):
-    __tablename__ = "food_security"
+class DBNationalRisk(Base):
+    __tablename__ = "national_risk"
+    __table_args__ = (
+        CheckConstraint(
+            "meta_avg_recentness_years >= 0.0",
+            name="meta_avg_recentness_years",
+        ),
+        CheckConstraint(
+            "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
+            name="reference_period",
+        ),
+    )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
     resource_ref: Mapped[int] = mapped_column(
         ForeignKey("resource.id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     admin2_ref: Mapped[int] = mapped_column(
         ForeignKey("admin2.id", onupdate="CASCADE"), nullable=False
     )
-    ipc_phase_code: Mapped[str] = mapped_column(
-        ForeignKey("ipc_phase.code", onupdate="CASCADE"), nullable=False
-    )
-    ipc_type_code: Mapped[str] = mapped_column(
-        ForeignKey("ipc_type.code", onupdate="CASCADE"), nullable=False
+    risk_class: Mapped[int] = mapped_column(Integer, nullable=False)
+    global_rank: Mapped[int] = mapped_column(Integer, nullable=False)
+    overall_risk: Mapped[float] = mapped_column(Float, nullable=False)
+    hazard_exposure_risk: Mapped[float] = mapped_column(Float, nullable=False)
+    vulnerability_risk: Mapped[float] = mapped_column(Float, nullable=False)
+    coping_capacity_risk: Mapped[float] = mapped_column(Float, nullable=False)
+    meta_missing_indicators_pct: Mapped[float] = mapped_column(
+        Float, nullable=True
     )
-    population_in_phase: Mapped[int] = mapped_column(Integer, nullable=False)
-    population_fraction_in_phase: Mapped[float] = mapped_column(
-        Float, nullable=False
+    meta_avg_recentness_years: Mapped[float] = mapped_column(
+        Float, nullable=True
     )
     reference_period_start: Mapped[datetime] = mapped_column(
-        DateTime, nullable=False
+        DateTime, nullable=True, server_default=text("NULL"), index=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL")
+        DateTime, nullable=True, server_default=text("NULL"), index=True
     )
     source_data: Mapped[str] = mapped_column(Text, nullable=True)
 
     resource = relationship("DBResource")
     admin2 = relationship("DBAdmin2")
-    ipc_phase = relationship("DBIpcPhase")
-    ipc_type = relationship("DBIpcType")
 
 
-view_params_food_security = ViewParams(
-    name="food_security_view",
+view_params_national_risk = ViewParams(
+    name="national_risk_view",
     metadata=Base.metadata,
     selectable=select(
-        *DBFoodSecurity.__table__.columns,
+        *DBNationalRisk.__table__.columns,
         DBDataset.hdx_id.label("dataset_hdx_id"),
         DBDataset.hdx_stub.label("dataset_hdx_stub"),
         DBDataset.title.label("dataset_title"),
         DBDataset.hdx_provider_stub.label("dataset_hdx_provider_stub"),
         DBDataset.hdx_provider_name.label("dataset_hdx_provider_name"),
-        DBIpcPhase.name.label("ipc_phase_name"),
         DBResource.hdx_id.label("resource_hdx_id"),
         DBResource.name.label("resource_name"),
         DBResource.update_date.label("resource_update_date"),
+        DBResource.hapi_updated_date.label("hapi_updated_date"),
+        DBResource.hapi_replaced_date.label("hapi_replaced_date"),
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
         DBAdmin1.code.label("admin1_code"),
         DBAdmin1.name.label("admin1_name"),
         DBAdmin1.is_unspecified.label("admin1_is_unspecified"),
         DBAdmin2.code.label("admin2_code"),
         DBAdmin2.name.label("admin2_name"),
         DBAdmin2.is_unspecified.label("admin2_is_unspecified"),
     ).select_from(
-        # Join pop to admin2 to admin1 to loc
-        DBFoodSecurity.__table__.join(
+        # Join risk to admin 2 to admin 1 to loc
+        DBNationalRisk.__table__.join(
             DBAdmin2.__table__,
-            DBFoodSecurity.admin2_ref == DBAdmin2.id,
+            DBNationalRisk.admin2_ref == DBAdmin2.id,
             isouter=True,
         )
         .join(
             DBAdmin1.__table__,
             DBAdmin2.admin1_ref == DBAdmin1.id,
             isouter=True,
         )
         .join(
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         )
-        # Join pop to resource to dataset
+        # Join risk to resource to dataset
         .join(
             DBResource.__table__,
-            DBFoodSecurity.resource_ref == DBResource.id,
+            DBNationalRisk.resource_ref == DBResource.id,
             isouter=True,
         )
         .join(
             DBDataset.__table__,
             DBResource.dataset_ref == DBDataset.id,
             isouter=True,
         )
-        # Join to ipc phase
-        .join(
-            DBIpcPhase.__table__,
-            DBFoodSecurity.ipc_phase_code == DBIpcPhase.code,
-            isouter=True,
-        )
-        # Join to ipc type
-        .join(
-            DBIpcType.__table__,
-            DBFoodSecurity.ipc_type_code == DBIpcType.code,
-            isouter=True,
-        )
     ),
 )
```

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_gender.py` & `hapi_schema-0.7.0/src/hapi_schema/db_gender.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_humanitarian_needs.py` & `hapi_schema-0.7.0/src/hapi_schema/db_operational_presence.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,133 +1,141 @@
-"""HumanitarianNeeds table and view."""
+"""OperationalPresence table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
-    Boolean,
+    CheckConstraint,
     DateTime,
     ForeignKey,
     Integer,
     Text,
     select,
     text,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_admin1 import DBAdmin1
 from hapi_schema.db_admin2 import DBAdmin2
 from hapi_schema.db_dataset import DBDataset
 from hapi_schema.db_location import DBLocation
+from hapi_schema.db_org import DBOrg
+from hapi_schema.db_org_type import DBOrgType
 from hapi_schema.db_resource import DBResource
 from hapi_schema.db_sector import DBSector
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.view_params import ViewParams
 
 
-class DBHumanitarianNeeds(Base):
-    __tablename__ = "humanitarian_needs"
+class DBOperationalPresence(Base):
+    __tablename__ = "operational_presence"
+    __table_args__ = (
+        CheckConstraint(
+            "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
+            name="reference_period",
+        ),
+    )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    resource_ref: Mapped[int] = mapped_column(
+    resource_ref = mapped_column(
         ForeignKey("resource.id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     admin2_ref: Mapped[int] = mapped_column(
         ForeignKey("admin2.id", onupdate="CASCADE"), nullable=False
     )
-    population_status_code: Mapped[str] = mapped_column(
-        ForeignKey("population_status.code", onupdate="CASCADE"),
-        nullable=True,
-    )
-    population_group_code: Mapped[str] = mapped_column(
-        ForeignKey("population_group.code", onupdate="CASCADE"), nullable=True
+    org_ref: Mapped[str] = mapped_column(
+        ForeignKey("org.id", onupdate="CASCADE"), nullable=False
     )
     sector_code: Mapped[str] = mapped_column(
-        ForeignKey("sector.code", onupdate="CASCADE"), nullable=True
-    )
-    gender_code: Mapped[str] = mapped_column(
-        ForeignKey("gender.code", onupdate="CASCADE"), nullable=True
-    )
-    age_range_code: Mapped[str] = mapped_column(
-        ForeignKey("age_range.code", onupdate="CASCADE"), nullable=True
-    )
-    disabled_marker: Mapped[bool] = mapped_column(
-        Boolean, nullable=True, server_default=text("NULL")
-    )
-    population: Mapped[int] = mapped_column(
-        Integer, nullable=False, index=True
+        ForeignKey("sector.code", onupdate="CASCADE"), nullable=False
     )
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, nullable=False, index=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL")
+        DateTime, nullable=True, server_default=text("NULL"), index=True
     )
     source_data: Mapped[str] = mapped_column(Text, nullable=True)
 
     resource = relationship("DBResource")
     admin2 = relationship("DBAdmin2")
+    org = relationship("DBOrg")
     sector = relationship("DBSector")
-    gender = relationship("DBGender")
-    age_range = relationship("DBAgeRange")
-    population_group = relationship("DBPopulationGroup")
-    population_status = relationship("DBPopulationStatus")
 
 
-view_params_humanitarian_needs = ViewParams(
-    name="humanitarian_needs_view",
+view_params_operational_presence = ViewParams(
+    name="operational_presence_view",
     metadata=Base.metadata,
     selectable=select(
-        *DBHumanitarianNeeds.__table__.columns,
+        *DBOperationalPresence.__table__.columns,
         DBDataset.hdx_id.label("dataset_hdx_id"),
         DBDataset.hdx_stub.label("dataset_hdx_stub"),
         DBDataset.title.label("dataset_title"),
         DBDataset.hdx_provider_stub.label("dataset_hdx_provider_stub"),
         DBDataset.hdx_provider_name.label("dataset_hdx_provider_name"),
         DBResource.hdx_id.label("resource_hdx_id"),
         DBResource.name.label("resource_name"),
         DBResource.update_date.label("resource_update_date"),
+        DBResource.hapi_updated_date.label("hapi_updated_date"),
+        DBResource.hapi_replaced_date.label("hapi_replaced_date"),
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
         DBAdmin1.code.label("admin1_code"),
         DBAdmin1.name.label("admin1_name"),
         DBAdmin1.is_unspecified.label("admin1_is_unspecified"),
+        DBAdmin1.location_ref.label("location_ref"),
         DBAdmin2.code.label("admin2_code"),
         DBAdmin2.name.label("admin2_name"),
         DBAdmin2.is_unspecified.label("admin2_is_unspecified"),
+        DBAdmin2.admin1_ref.label("admin1_ref"),
+        DBOrg.acronym.label("org_acronym"),
+        DBOrg.name.label("org_name"),
+        DBOrg.org_type_code.label("org_type_code"),
+        DBOrgType.description.label("org_type_description"),
         DBSector.name.label("sector_name"),
     ).select_from(
-        # Join pop to admin2 to admin1 to loc
-        DBHumanitarianNeeds.__table__.join(
+        # Join op to admin2 to admin1 to loc
+        DBOperationalPresence.__table__.join(
             DBAdmin2.__table__,
-            DBHumanitarianNeeds.admin2_ref == DBAdmin2.id,
+            DBOperationalPresence.admin2_ref == DBAdmin2.id,
             isouter=True,
         )
         .join(
             DBAdmin1.__table__,
             DBAdmin2.admin1_ref == DBAdmin1.id,
             isouter=True,
         )
         .join(
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         )
-        # Join needs to resource to dataset
+        # Join op to resource to dataset
         .join(
             DBResource.__table__,
-            DBHumanitarianNeeds.resource_ref == DBResource.id,
+            DBOperationalPresence.resource_ref == DBResource.id,
             isouter=True,
         )
         .join(
             DBDataset.__table__,
             DBResource.dataset_ref == DBDataset.id,
             isouter=True,
         )
-        # Join needs to sector
+        # Join op to org to org type
+        .join(
+            DBOrg.__table__,
+            DBOperationalPresence.org_ref == DBOrg.id,
+            isouter=True,
+        )
+        .join(
+            DBOrgType.__table__,
+            DBOrg.org_type_code == DBOrgType.code,
+            isouter=True,
+        )
+        # Join op to sector
         .join(
             DBSector.__table__,
-            DBHumanitarianNeeds.sector_code == DBSector.code,
+            DBOperationalPresence.sector_code == DBSector.code,
             isouter=True,
         )
     ),
 )
```

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_ipc_phase.py` & `hapi_schema-0.7.0/src/hapi_schema/db_sector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-"""IPC phase table and view."""
+"""Sector table and view."""
 
 from sqlalchemy import String, select
 from sqlalchemy.orm import Mapped, mapped_column
 
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.view_params import ViewParams
 
 
-class DBIpcPhase(Base):
-    __tablename__ = "ipc_phase"
+class DBSector(Base):
+    __tablename__ = "sector"
 
-    code: Mapped[int] = mapped_column(String(32), primary_key=True)
-    name: Mapped[str] = mapped_column(String(32), nullable=False)
-    description: Mapped[str] = mapped_column(String(512), nullable=False)
+    code: Mapped[str] = mapped_column(String(32), primary_key=True)
+    name: Mapped[str] = mapped_column(String(512), nullable=False, index=True)
 
 
-view_params_ipc_phase = ViewParams(
-    name="ipc_phase_view",
+view_params_sector = ViewParams(
+    name="sector_view",
     metadata=Base.metadata,
-    selectable=select(*DBIpcPhase.__table__.columns),
+    selectable=select(*DBSector.__table__.columns),
 )
```

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_ipc_type.py` & `hapi_schema-0.7.0/src/hapi_schema/db_ipc_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """IPC type table and view."""
 
-from sqlalchemy import String, select
+from sqlalchemy import CheckConstraint, String, select
 from sqlalchemy.orm import Mapped, mapped_column
 
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBIpcType(Base):
     __tablename__ = "ipc_type"
-
+    __table_args__ = (
+        CheckConstraint(
+            'code IN ("current", "first projection", "second projection")',
+            name="ipc_phase_type",
+        ),
+    )
     code: Mapped[str] = mapped_column(String(32), primary_key=True)
     description: Mapped[str] = mapped_column(String(512), nullable=False)
 
 
 view_params_ipc_type = ViewParams(
     name="ipca_type_vew",
     metadata=Base.metadata,
```

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_location.py` & `hapi_schema-0.7.0/src/hapi_schema/db_location.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,52 @@
 """Location table and view."""
 
 from datetime import datetime
 
-from sqlalchemy import DateTime, Integer, String, select, text
+from sqlalchemy import (
+    CheckConstraint,
+    DateTime,
+    Integer,
+    String,
+    UniqueConstraint,
+    select,
+    text,
+)
 from sqlalchemy.orm import Mapped, mapped_column
 
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBLocation(Base):
     __tablename__ = "location"
+    __table_args__ = (
+        CheckConstraint(
+            "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
+            name="reference_period",
+        ),
+        CheckConstraint(
+            "(hapi_replaced_date IS NULL) OR (hapi_replaced_date >= hapi_updated_date)",
+            name="hapi_dates",
+        ),
+        UniqueConstraint("code", "hapi_updated_date", name="code_date_unique"),
+    )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    code: Mapped[str] = mapped_column(String(128), unique=True, nullable=False)
+    code: Mapped[str] = mapped_column(String(128), nullable=False)
     name: Mapped[str] = mapped_column(String(512), nullable=False)
     reference_period_start: Mapped[datetime] = mapped_column(
-        DateTime, nullable=False
+        DateTime, nullable=True, server_default=text("NULL"), index=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL")
+        DateTime, nullable=True, server_default=text("NULL"), index=True
+    )
+    hapi_updated_date = mapped_column(DateTime, nullable=False, index=True)
+    hapi_replaced_date: Mapped[datetime] = mapped_column(
+        DateTime, nullable=True, server_default=text("NULL"), index=True
     )
 
 
 view_params_location = ViewParams(
     name="location_view",
     metadata=Base.metadata,
     selectable=select(*DBLocation.__table__.columns),
```

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_national_risk.py` & `hapi_schema-0.7.0/src/hapi_schema/db_food_security.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,110 +1,142 @@
-"""NationalRisk table and view."""
+"""Population table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
+    CheckConstraint,
     DateTime,
     Float,
     ForeignKey,
     Integer,
     Text,
     select,
     text,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_admin1 import DBAdmin1
 from hapi_schema.db_admin2 import DBAdmin2
 from hapi_schema.db_dataset import DBDataset
+from hapi_schema.db_ipc_phase import DBIpcPhase
+from hapi_schema.db_ipc_type import DBIpcType
 from hapi_schema.db_location import DBLocation
 from hapi_schema.db_resource import DBResource
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.view_params import ViewParams
 
 
-class DBNationalRisk(Base):
-    __tablename__ = "national_risk"
+class DBFoodSecurity(Base):
+    __tablename__ = "food_security"
+    __table_args__ = (
+        CheckConstraint(
+            "population_fraction_in_phase >= 0 AND population_fraction_in_phase <=1",
+            name="population_fraction_in_phase",
+        ),
+        CheckConstraint(
+            "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
+            name="reference_period",
+        ),
+    )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
     resource_ref: Mapped[int] = mapped_column(
         ForeignKey("resource.id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     admin2_ref: Mapped[int] = mapped_column(
         ForeignKey("admin2.id", onupdate="CASCADE"), nullable=False
     )
-    risk_class: Mapped[int] = mapped_column(Integer, nullable=False)
-    global_rank: Mapped[int] = mapped_column(Integer, nullable=False)
-    overall_risk: Mapped[float] = mapped_column(Float, nullable=False)
-    hazard_exposure_risk: Mapped[float] = mapped_column(Float, nullable=False)
-    vulnerability_risk: Mapped[float] = mapped_column(Float, nullable=False)
-    coping_capacity_risk: Mapped[float] = mapped_column(Float, nullable=False)
-    meta_missing_indicators_pct: Mapped[float] = mapped_column(
-        Float, nullable=True
+    ipc_phase_code: Mapped[str] = mapped_column(
+        ForeignKey("ipc_phase.code", onupdate="CASCADE"), nullable=False
+    )
+    ipc_type_code: Mapped[str] = mapped_column(
+        ForeignKey("ipc_type.code", onupdate="CASCADE"), nullable=False
+    )
+    population_in_phase: Mapped[int] = mapped_column(
+        Integer, nullable=False, index=True
     )
-    meta_avg_recentness_years: Mapped[float] = mapped_column(
-        Float, nullable=True
+    population_fraction_in_phase: Mapped[float] = mapped_column(
+        Float, nullable=False, index=True
     )
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, nullable=False, index=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL")
+        DateTime, nullable=True, server_default=text("NULL"), index=True
     )
     source_data: Mapped[str] = mapped_column(Text, nullable=True)
 
     resource = relationship("DBResource")
     admin2 = relationship("DBAdmin2")
+    ipc_phase = relationship("DBIpcPhase")
+    ipc_type = relationship("DBIpcType")
 
 
-view_params_national_risk = ViewParams(
-    name="national_risk_view",
+view_params_food_security = ViewParams(
+    name="food_security_view",
     metadata=Base.metadata,
     selectable=select(
-        *DBNationalRisk.__table__.columns,
+        *DBFoodSecurity.__table__.columns,
         DBDataset.hdx_id.label("dataset_hdx_id"),
         DBDataset.hdx_stub.label("dataset_hdx_stub"),
         DBDataset.title.label("dataset_title"),
         DBDataset.hdx_provider_stub.label("dataset_hdx_provider_stub"),
         DBDataset.hdx_provider_name.label("dataset_hdx_provider_name"),
+        DBIpcPhase.name.label("ipc_phase_name"),
         DBResource.hdx_id.label("resource_hdx_id"),
         DBResource.name.label("resource_name"),
         DBResource.update_date.label("resource_update_date"),
+        DBResource.hapi_updated_date.label("hapi_updated_date"),
+        DBResource.hapi_replaced_date.label("hapi_replaced_date"),
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
         DBAdmin1.code.label("admin1_code"),
         DBAdmin1.name.label("admin1_name"),
         DBAdmin1.is_unspecified.label("admin1_is_unspecified"),
+        DBAdmin1.location_ref.label("location_ref"),
         DBAdmin2.code.label("admin2_code"),
         DBAdmin2.name.label("admin2_name"),
         DBAdmin2.is_unspecified.label("admin2_is_unspecified"),
+        DBAdmin2.admin1_ref.label("admin1_ref"),
     ).select_from(
-        # Join risk to admin 2 to admin 1 to loc
-        DBNationalRisk.__table__.join(
+        # Join pop to admin2 to admin1 to loc
+        DBFoodSecurity.__table__.join(
             DBAdmin2.__table__,
-            DBNationalRisk.admin2_ref == DBAdmin2.id,
+            DBFoodSecurity.admin2_ref == DBAdmin2.id,
             isouter=True,
         )
         .join(
             DBAdmin1.__table__,
             DBAdmin2.admin1_ref == DBAdmin1.id,
             isouter=True,
         )
         .join(
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         )
-        # Join risk to resource to dataset
+        # Join pop to resource to dataset
         .join(
             DBResource.__table__,
-            DBNationalRisk.resource_ref == DBResource.id,
+            DBFoodSecurity.resource_ref == DBResource.id,
             isouter=True,
         )
         .join(
             DBDataset.__table__,
             DBResource.dataset_ref == DBDataset.id,
             isouter=True,
         )
+        # Join to ipc phase
+        .join(
+            DBIpcPhase.__table__,
+            DBFoodSecurity.ipc_phase_code == DBIpcPhase.code,
+            isouter=True,
+        )
+        # Join to ipc type
+        .join(
+            DBIpcType.__table__,
+            DBFoodSecurity.ipc_type_code == DBIpcType.code,
+            isouter=True,
+        )
     ),
 )
```

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_operational_presence.py` & `hapi_schema-0.7.0/src/hapi_schema/db_humanitarian_needs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,130 +1,145 @@
-"""OperationalPresence table and view."""
+"""HumanitarianNeeds table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
+    Boolean,
+    CheckConstraint,
     DateTime,
     ForeignKey,
     Integer,
     Text,
     select,
     text,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_admin1 import DBAdmin1
 from hapi_schema.db_admin2 import DBAdmin2
 from hapi_schema.db_dataset import DBDataset
 from hapi_schema.db_location import DBLocation
-from hapi_schema.db_org import DBOrg
-from hapi_schema.db_org_type import DBOrgType
 from hapi_schema.db_resource import DBResource
 from hapi_schema.db_sector import DBSector
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.view_params import ViewParams
 
 
-class DBOperationalPresence(Base):
-    __tablename__ = "operational_presence"
+class DBHumanitarianNeeds(Base):
+    __tablename__ = "humanitarian_needs"
+    __table_args__ = (
+        CheckConstraint("population >= 0", name="population"),
+        CheckConstraint(
+            "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
+            name="reference_period",
+        ),
+    )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    resource_ref = mapped_column(
+    resource_ref: Mapped[int] = mapped_column(
         ForeignKey("resource.id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     admin2_ref: Mapped[int] = mapped_column(
         ForeignKey("admin2.id", onupdate="CASCADE"), nullable=False
     )
-    org_ref: Mapped[str] = mapped_column(
-        ForeignKey("org.id", onupdate="CASCADE"), nullable=False
+    population_status_code: Mapped[str] = mapped_column(
+        ForeignKey("population_status.code", onupdate="CASCADE"),
+        nullable=True,
+    )
+    population_group_code: Mapped[str] = mapped_column(
+        ForeignKey("population_group.code", onupdate="CASCADE"), nullable=True
     )
     sector_code: Mapped[str] = mapped_column(
-        ForeignKey("sector.code", onupdate="CASCADE"), nullable=False
+        ForeignKey("sector.code", onupdate="CASCADE"), nullable=True
+    )
+    gender_code: Mapped[str] = mapped_column(
+        ForeignKey("gender.code", onupdate="CASCADE"), nullable=True
+    )
+    age_range_code: Mapped[str] = mapped_column(
+        ForeignKey("age_range.code", onupdate="CASCADE"), nullable=True
+    )
+    disabled_marker: Mapped[bool] = mapped_column(
+        Boolean, nullable=True, server_default=text("NULL")
+    )
+    population: Mapped[int] = mapped_column(
+        Integer, nullable=False, index=True
     )
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, nullable=False, index=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL")
+        DateTime, nullable=True, server_default=text("NULL"), index=True
     )
     source_data: Mapped[str] = mapped_column(Text, nullable=True)
 
     resource = relationship("DBResource")
     admin2 = relationship("DBAdmin2")
-    org = relationship("DBOrg")
     sector = relationship("DBSector")
+    gender = relationship("DBGender")
+    age_range = relationship("DBAgeRange")
+    population_group = relationship("DBPopulationGroup")
+    population_status = relationship("DBPopulationStatus")
 
 
-view_params_operational_presence = ViewParams(
-    name="operational_presence_view",
+view_params_humanitarian_needs = ViewParams(
+    name="humanitarian_needs_view",
     metadata=Base.metadata,
     selectable=select(
-        *DBOperationalPresence.__table__.columns,
+        *DBHumanitarianNeeds.__table__.columns,
         DBDataset.hdx_id.label("dataset_hdx_id"),
         DBDataset.hdx_stub.label("dataset_hdx_stub"),
         DBDataset.title.label("dataset_title"),
         DBDataset.hdx_provider_stub.label("dataset_hdx_provider_stub"),
         DBDataset.hdx_provider_name.label("dataset_hdx_provider_name"),
         DBResource.hdx_id.label("resource_hdx_id"),
         DBResource.name.label("resource_name"),
         DBResource.update_date.label("resource_update_date"),
+        DBResource.hapi_updated_date.label("hapi_updated_date"),
+        DBResource.hapi_replaced_date.label("hapi_replaced_date"),
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
         DBAdmin1.code.label("admin1_code"),
         DBAdmin1.name.label("admin1_name"),
         DBAdmin1.is_unspecified.label("admin1_is_unspecified"),
+        DBAdmin1.location_ref.label("location_ref"),
         DBAdmin2.code.label("admin2_code"),
         DBAdmin2.name.label("admin2_name"),
         DBAdmin2.is_unspecified.label("admin2_is_unspecified"),
-        DBOrg.acronym.label("org_acronym"),
-        DBOrg.name.label("org_name"),
-        DBOrg.org_type_code.label("org_type_code"),
-        DBOrgType.description.label("org_type_description"),
+        DBAdmin2.admin1_ref.label("admin1_ref"),
         DBSector.name.label("sector_name"),
     ).select_from(
-        # Join op to admin2 to admin1 to loc
-        DBOperationalPresence.__table__.join(
+        # Join pop to admin2 to admin1 to loc
+        DBHumanitarianNeeds.__table__.join(
             DBAdmin2.__table__,
-            DBOperationalPresence.admin2_ref == DBAdmin2.id,
+            DBHumanitarianNeeds.admin2_ref == DBAdmin2.id,
             isouter=True,
         )
         .join(
             DBAdmin1.__table__,
             DBAdmin2.admin1_ref == DBAdmin1.id,
             isouter=True,
         )
         .join(
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         )
-        # Join op to resource to dataset
+        # Join needs to resource to dataset
         .join(
             DBResource.__table__,
-            DBOperationalPresence.resource_ref == DBResource.id,
+            DBHumanitarianNeeds.resource_ref == DBResource.id,
             isouter=True,
         )
         .join(
             DBDataset.__table__,
             DBResource.dataset_ref == DBDataset.id,
             isouter=True,
         )
-        # Join op to org to org type
-        .join(
-            DBOrg.__table__,
-            DBOperationalPresence.org_ref == DBOrg.id,
-            isouter=True,
-        )
-        .join(
-            DBOrgType.__table__,
-            DBOrg.org_type_code == DBOrgType.code,
-            isouter=True,
-        )
-        # Join op to sector
+        # Join needs to sector
         .join(
             DBSector.__table__,
-            DBOperationalPresence.sector_code == DBSector.code,
+            DBHumanitarianNeeds.sector_code == DBSector.code,
             isouter=True,
         )
     ),
 )
```

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_org.py` & `hapi_schema-0.7.0/src/hapi_schema/db_org.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Org table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
+    CheckConstraint,
     DateTime,
     ForeignKey,
     Integer,
     String,
     select,
     text,
 )
@@ -15,27 +16,41 @@
 from hapi_schema.db_org_type import DBOrgType
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBOrg(Base):
     __tablename__ = "org"
+    __table_args__ = (
+        CheckConstraint(
+            "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
+            name="reference_period",
+        ),
+        CheckConstraint(
+            "(hapi_replaced_date IS NULL) OR (hapi_replaced_date >= hapi_updated_date)",
+            name="hapi_dates",
+        ),
+    )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
     acronym = mapped_column(String(32), nullable=False, index=True)
     name: Mapped[str] = mapped_column(String(512), nullable=False)
     org_type_code: Mapped[str] = mapped_column(
         ForeignKey("org_type.code", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=True,
     )
     reference_period_start: Mapped[datetime] = mapped_column(
-        DateTime, nullable=False, index=True
+        DateTime, nullable=True, server_default=text("NULL"), index=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL")
+        DateTime, nullable=True, server_default=text("NULL"), index=True
+    )
+    hapi_updated_date = mapped_column(DateTime, nullable=False, index=True)
+    hapi_replaced_date: Mapped[datetime] = mapped_column(
+        DateTime, nullable=True, server_default=text("NULL"), index=True
     )
 
     org_type = relationship("DBOrgType")
 
 
 view_params_org = ViewParams(
     name="org_view",
```

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_org_type.py` & `hapi_schema-0.7.0/src/hapi_schema/db_org_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBOrgType(Base):
     __tablename__ = "org_type"
 
     code: Mapped[str] = mapped_column(String(32), primary_key=True)
-    description: Mapped[str] = mapped_column(String(512), nullable=False)
+    description: Mapped[str] = mapped_column(
+        String(512), nullable=False, index=True
+    )
 
 
 view_params_org_type = ViewParams(
     name="org_type_view",
     metadata=Base.metadata,
     selectable=select(*DBOrgType.__table__.columns),
 )
```

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_population_group.py` & `hapi_schema-0.7.0/src/hapi_schema/db_population_group.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_population_status.py` & `hapi_schema-0.7.0/src/hapi_schema/db_population_status.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/src/hapi_schema/db_resource.py` & `hapi_schema-0.7.0/src/hapi_schema/db_resource.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 """Resource table and view."""
 
+from datetime import datetime
+
 from sqlalchemy import (
     Boolean,
+    CheckConstraint,
     DateTime,
     ForeignKey,
     Integer,
     String,
     select,
+    text,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_dataset import DBDataset
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBResource(Base):
     __tablename__ = "resource"
+    __table_args__ = (
+        CheckConstraint(
+            "(hapi_replaced_date IS NULL) OR (hapi_replaced_date >= hapi_updated_date)",
+            name="hapi_dates",
+        ),
+    )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
     dataset_ref: Mapped[int] = mapped_column(
         ForeignKey("dataset.id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     hdx_id: Mapped[str] = mapped_column(
@@ -29,15 +39,18 @@
     name: Mapped[str] = mapped_column(String(256), nullable=False)
     format: Mapped[str] = mapped_column(String(32), nullable=False)
     update_date = mapped_column(DateTime, nullable=False, index=True)
     download_url: Mapped[str] = mapped_column(
         String(1024), nullable=False, unique=True
     )
     is_hxl: Mapped[bool] = mapped_column(Boolean, nullable=False, index=True)
-
+    hapi_updated_date = mapped_column(DateTime, nullable=False, index=True)
+    hapi_replaced_date: Mapped[datetime] = mapped_column(
+        DateTime, nullable=True, server_default=text("NULL"), index=True
+    )
     dataset = relationship("DBDataset")
 
 
 view_params_resource = ViewParams(
     name="resource_view",
     metadata=Base.metadata,
     selectable=select(
```

### Comparing `hapi_schema-0.6.2/tests/test_dataset_view.py` & `hapi_schema-0.7.0/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/tests/test_humanitarian_needs_view.py` & `hapi_schema-0.7.0/tests/test_humanitarian_needs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+from datetime import datetime
+
 from hdx.database.views import build_view
 
-from hapi_schema.db_humanitarian_needs import view_params_humanitarian_needs
+from hapi_schema.db_humanitarian_needs import (
+    DBHumanitarianNeeds,
+    view_params_humanitarian_needs,
+)
 
 
 def test_humanitarian_needs_view(run_view_test):
     """Check that humanitarian needs references other tables."""
     view_humanitarian_needs = build_view(
         view_params_humanitarian_needs.__dict__
     )
@@ -23,7 +28,30 @@
             view_humanitarian_needs.c.population_group_code == "idps",
             view_humanitarian_needs.c.sector_name
             == "Water Sanitation Hygiene",
             view_humanitarian_needs.c.gender_code == "f",
             view_humanitarian_needs.c.disabled_marker == True,  # noqa: E712
         ),
     )
+
+
+def test_reference_period_constraint(run_constraints_test):
+    """Check that reference_period_end cannot be less than start"""
+    run_constraints_test(
+        new_rows=[
+            DBHumanitarianNeeds(
+                resource_ref=1,
+                admin2_ref=1,
+                gender_code=None,
+                age_range_code=None,
+                disabled_marker=None,
+                sector_code=None,
+                population_group_code=None,
+                population_status_code="affected",
+                population=1_000_000,
+                reference_period_start=datetime(2023, 1, 2),
+                reference_period_end=datetime(2023, 1, 1),
+                source_data="DATA,DATA,DATA",
+            )
+        ],
+        expected_constraint="reference_period",
+    )
```

### Comparing `hapi_schema-0.6.2/tests/test_population_group_view.py` & `hapi_schema-0.7.0/tests/test_population_group.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/tests/test_population_status_view.py` & `hapi_schema-0.7.0/tests/test_population_status.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/tests/sample_data/data_admin1.py` & `hapi_schema-0.7.0/tests/sample_data/data_national_risk.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,20 @@
 from datetime import datetime
 
-data_admin1 = [
+data_national_risk = [
     dict(
         id=1,
-        location_ref=1,
-        code="FOO-XXX",
-        name="Unspecified",
-        is_unspecified=True,
-        reference_period_start=datetime(2023, 1, 1),
-        reference_period_end=None,
-    ),
-    dict(
-        id=2,
-        location_ref=1,
-        code="FOO-001",
-        name="Province 01",
-        is_unspecified=False,
-        reference_period_start=datetime(2023, 1, 1),
-        reference_period_end=None,
-    ),
-    dict(
-        id=3,
-        location_ref=1,
-        code="FOO-002",
-        name="Province 02",
-        is_unspecified=False,
-        reference_period_start=datetime(2023, 1, 1),
-        reference_period_end=None,
+        resource_ref=1,
+        admin2_ref=1,
+        risk_class=5,
+        global_rank=4,
+        overall_risk=8.1,
+        hazard_exposure_risk=8.7,
+        vulnerability_risk=8.5,
+        coping_capacity_risk=7.1,
+        meta_missing_indicators_pct=8,
+        meta_avg_recentness_years=0.26,
+        reference_period_start=datetime(2024, 1, 1),
+        reference_period_end=datetime(2024, 12, 31),
+        source_data="DATA,DATA,DATA",
     ),
 ]
```

### Comparing `hapi_schema-0.6.2/tests/sample_data/data_food_security.py` & `hapi_schema-0.7.0/tests/sample_data/data_food_security.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,45 +2,42 @@
 
 data_food_security = [
     # Phase 1 current national
     dict(
         id=1,
         resource_ref=3,
         admin2_ref=1,
-        ipc_phase_code=1,
-        ipc_type_code=1,
-        population_total=1_000_000,
+        ipc_phase_code="1",
+        ipc_type_code="current",
         population_in_phase=500_000,
         population_fraction_in_phase=0.5,
         reference_period_start=datetime(2023, 1, 1),
         reference_period_end=datetime(2023, 3, 30),
         source_data="DATA,DATA,DATA",
     ),
     # Phase 2 first projection admin1
     dict(
         id=2,
         resource_ref=3,
         admin2_ref=2,
-        ipc_phase_code=2,
-        ipc_type_code=2,
-        population_total=100_000,
+        ipc_phase_code="2",
+        ipc_type_code="first projection",
         population_in_phase=40_000,
         population_fraction_in_phase=0.4,
         reference_period_start=datetime(2023, 4, 1),
         reference_period_end=datetime(2023, 6, 30),
         source_data="DATA,DATA,DATA",
     ),
     # Phase 3 second projection admin2
     dict(
         id=3,
         resource_ref=3,
         admin2_ref=4,
-        ipc_phase_code=3,
-        ipc_type_code=3,
-        population_total=10_000,
+        ipc_phase_code="3",
+        ipc_type_code="second projection",
         population_in_phase=3_000,
         population_fraction_in_phase=0.3,
         reference_period_start=datetime(2023, 7, 1),
         reference_period_end=datetime(2023, 10, 31),
         source_data="DATA,DATA,DATA",
     ),
 ]
```

### Comparing `hapi_schema-0.6.2/tests/sample_data/data_humanitarian_needs.py` & `hapi_schema-0.7.0/tests/sample_data/data_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/tests/sample_data/data_ipc_phase.py` & `hapi_schema-0.7.0/tests/sample_data/data_ipc_phase.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/tests/sample_data/data_operational_presence.py` & `hapi_schema-0.7.0/tests/sample_data/data_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/tests/sample_data/data_population.py` & `hapi_schema-0.7.0/tests/sample_data/data_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/tests/sample_data/data_resource.py` & `hapi_schema-0.7.0/tests/test_resource.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,52 @@
 from datetime import datetime
 
-data_resource = [
-    dict(
-        id=1,
-        dataset_ref=1,
-        hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
-        name="resource-01.csv",
-        format="csv",
-        update_date=datetime(2023, 6, 1),
-        download_url="https://data.humdata.org/dataset/c3f001fa-b45b-464c-9460-1ca79fd39b40/resource/90deb235-1bf5-4bae-b231-3393222c2d01/download/resource-01.csv",
-        is_hxl=True,
-    ),
-    dict(
-        id=2,
-        dataset_ref=1,
-        hdx_id="b9e438e0-b68a-49f9-b9a9-68c0f3e93604",
-        name="resource-02.xlsx",
-        format="xlsx",
-        update_date=datetime(2023, 7, 1),
-        download_url="https://fdw.fews.net/api/tradeflowquantityvaluefacts/?dataset=1845&country=TZ&fields=simple&format=xlsx",
-        is_hxl=True,
-    ),
-    dict(
-        id=3,
-        dataset_ref=2,
-        hdx_id="62ad6e55-5f5d-4494-854c-4110687e9e25",
-        name="resource-03.csv",
-        format="csv",
-        update_date=datetime(2023, 8, 1),
-        download_url="https://data.humdata.org/dataset/7cf3cec8-dbbc-4c96-9762-1464cd0bff75/resource/62ad6e55-5f5d-4494-854c-4110687e9e25/download/resource-03.csv",
-        is_hxl=True,
-    ),
-]
+from hdx.database.views import build_view
+
+from hapi_schema.db_resource import DBResource, view_params_resource
+
+
+def test_resource_view(run_view_test):
+    """Check that resource references dataset."""
+    view_resource = build_view(view_params_resource.__dict__)
+    run_view_test(
+        view=view_resource,
+        whereclause=(
+            view_resource.c.id == 1,
+            view_resource.c.dataset_hdx_id
+            == "c3f001fa-b45b-464c-9460-1ca79fd39b40",
+        ),
+    )
+
+
+def test_hapi_date_constraint(run_constraints_test):
+    """Check that hapi_replaced_date cannot be less than hapi_updated_date"""
+    run_constraints_test(
+        new_rows=[
+            DBResource(
+                dataset_ref=2,
+                hdx_id="9d9e07c9-a758-43bd-87dc-5cdd3b3f7e9f",
+                name="resource-04.csv",
+                format="csv",
+                update_date=datetime(2023, 1, 1),
+                download_url="https://data.humdata.org/dataset/7cf3cec8-dbbc-4c96-9762-1464cd0bff75/resource/9d9e07c9-a758-43bd-87dc-5cdd3b3f7e9f/download/resource-04.csv",
+                is_hxl=True,
+                hapi_updated_date=datetime(2023, 1, 2),
+                hapi_replaced_date=datetime(2023, 1, 1),
+            )
+        ],
+        expected_constraint="hapi_dates",
+    )
+
+    (
+        dict(
+            dataset_ref=2,
+            hdx_id="9d9e07c9-a758-43bd-87dc-5cdd3b3f7e9f",
+            name="resource-04.csv",
+            format="csv",
+            update_date=datetime(2023, 1, 1),
+            download_url="https://data.humdata.org/dataset/7cf3cec8-dbbc-4c96-9762-1464cd0bff75/resource/9d9e07c9-a758-43bd-87dc-5cdd3b3f7e9f/download/resource-04.csv",
+            is_hxl=True,
+            hapi_updated_date=datetime(2023, 8, 1),
+            hapi_replaced_date=None,
+        ),
+    )
```

### Comparing `hapi_schema-0.6.2/tests/sample_data/data_sector.py` & `hapi_schema-0.7.0/tests/sample_data/data_org.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from datetime import datetime
 
-data_sector = [
+data_org = [
     dict(
-        code="SHL",
-        name="Emergency Shelter and NFI",
-        reference_period_start=datetime(2023, 1, 1),
+        id=1,
+        acronym="ORG01",
+        name="Organisation 1",
+        org_type_code="433",
+        reference_period_start=None,
         reference_period_end=None,
+        hapi_updated_date=datetime(2023, 8, 1),
+        hapi_replaced_date=None,
     ),
     dict(
-        code="FSC",
-        name="Food Security",
-        reference_period_start=datetime(2023, 1, 1),
+        id=2,
+        acronym="ORG02",
+        name="Organisation 2",
+        org_type_code="437",
+        reference_period_start=None,
         reference_period_end=None,
+        hapi_updated_date=datetime(2023, 7, 1),
+        hapi_replaced_date=None,
     ),
     dict(
-        code="WSH",
-        name="Water Sanitation Hygiene",
-        reference_period_start=datetime(2023, 1, 1),
-        reference_period_end=None,
-    ),
-    dict(
-        code="HEA",
-        name="Health",
-        reference_period_start=datetime(2023, 1, 1),
+        id=3,
+        acronym="ORG03",
+        name="Organisation 3",
+        org_type_code="447",
+        reference_period_start=None,
         reference_period_end=None,
+        hapi_updated_date=datetime(2023, 6, 1),
+        hapi_replaced_date=None,
     ),
 ]
```

### Comparing `hapi_schema-0.6.2/.gitignore` & `hapi_schema-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/LICENSE` & `hapi_schema-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/pyproject.toml` & `hapi_schema-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.6.2/PKG-INFO` & `hapi_schema-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hapi-schema
-Version: 0.6.2
+Version: 0.7.0
 Summary: HAPI database schema specified in SQLAlchemy
 Project-URL: Homepage, https://github.com/OCHA-DAP/hapi-schemas
 Author-email: Simon Johnson <simon.johnson@un.org>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,hapi,schema
 Classifier: Intended Audience :: Developers
```

