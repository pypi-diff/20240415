# Comparing `tmp/eds-scikit-0.1.6.tar.gz` & `tmp/eds-scikit-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/eds-scikit/eds-scikit/dist/.tmp-f2beg002/eds-scikit-0.1.6.tar", last modified: Wed Sep 27 09:53:30 2023, max compression
+gzip compressed data, was "/home/runner/work/eds-scikit/eds-scikit/dist/.tmp-7c3v383i/eds-scikit-0.1.7.tar", last modified: Mon Apr 15 08:05:54 2024, max compression
```

## Comparing `eds-scikit-0.1.6.tar` & `eds-scikit-0.1.7.tar`

### file list

```diff
@@ -1,169 +1,182 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/docs/generate_development.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/docs/generate_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/docs/macros.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/docs/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/biology/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/biology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/biology/cleaning/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/biology/cleaning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/biology/cleaning/cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/biology/cleaning/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/biology/cleaning/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/biology/cleaning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/biology/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/biology/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/biology/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14661 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/biology/utils/process_concepts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/biology/utils/process_measurement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/biology/viz/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/biology/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23621 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/biology/viz/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    28093 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/biology/viz/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/biology/viz/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/default_concepts_sets.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/datasets/generation_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/generation_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/generation_scripts/care_site_hierarchy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/datasets/synthetic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/synthetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/synthetic/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/synthetic/biology.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/synthetic/ccam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/synthetic/consultation_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/synthetic/event_sequences.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/synthetic/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/synthetic/icd10.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/synthetic/person.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/synthetic/stay_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/synthetic/suicide_attempt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/synthetic/tagging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/datasets/synthetic/visit_merging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/emergency/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/emergency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/emergency/emergency_care_site.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/emergency/emergency_visit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/event/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/event/ccam.py
--rw-r--r--   0 runner    (1001) docker     (127)     9493 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/event/consultations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/event/diabetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/event/from_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/event/icd10.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/event/suicide_attempt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/icu/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/icu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/icu/icu_care_site.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/icu/icu_visit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/io/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/io/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/io/data_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/io/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    13377 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/io/hive.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/io/i2b2_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/io/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    11232 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/io/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/period/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/period/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18718 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/period/stays.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/period/tagging_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/phenotype/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13277 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/phenotype/cancer/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/cancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/cancer/cancer.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/cancer/citation.bib
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/cancer/codes.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/phenotype/diabetes/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/diabetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/diabetes/codes.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/diabetes/diabetes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/phenotype/psychiatric_disorder/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/psychiatric_disorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/psychiatric_disorder/citation.bib
--rw-r--r--   0 runner    (1001) docker     (127)   210411 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/psychiatric_disorder/codes.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/psychiatric_disorder/psychiatric_disorder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/phenotype/suicide_attempt/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/suicide_attempt/Haguenoer2008.bib
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/suicide_attempt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/suicide_attempt/codes.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/phenotype/suicide_attempt/suicide_attempt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/plot/age_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7906 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/plot/event_sequences.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/resources/reg.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/resources/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/structures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/structures/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/structures/description.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/utils/bunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/utils/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/utils/custom_implem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/utils/custom_implem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/utils/custom_implem/custom_implem.py
--rw-r--r--   0 runner    (1001) docker     (127)    15531 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/utils/custom_implem/cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/utils/datetime_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit/utils/flowchart/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/utils/flowchart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13314 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/utils/flowchart/flowchart.py
--rw-r--r--   0 runner    (1001) docker     (127)    10115 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/utils/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/utils/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/eds_scikit/utils/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/eds_scikit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/data/person.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/tests/emergency/
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/emergency/test_emergency_care_site.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/emergency/test_emergency_visits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/tests/flowchart/
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/flowchart/test_flowchart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/tests/icu/
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/icu/test_icu_care_site.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/icu/test_icu_visits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 09:53:30.000000 eds-scikit-0.1.6/tests/structures/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/structures/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_age_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_backend_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_biology.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_ccam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_consultation_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_event_sequences.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_icd10.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_stay_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_suicide.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_tagging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-09-27 09:53:14.000000 eds-scikit-0.1.6/tests/test_visit_merging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/docs/generate_development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/docs/generate_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/docs/macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/docs/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/docs/scripts/cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/docs/scripts/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/biology/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/biology/cleaning/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/cleaning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/cleaning/cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/cleaning/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/biology/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/utils/check_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/utils/prepare_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/utils/prepare_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/utils/process_concepts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/utils/process_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/utils/process_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/biology/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15997 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/viz/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28018 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/viz/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/viz/stats_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/biology/viz/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/default_concepts_sets.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/elements.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/datasets/generation_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/generation_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/generation_scripts/care_site_hierarchy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/datasets/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/synthetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/synthetic/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/synthetic/biology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/synthetic/ccam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/synthetic/consultation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/synthetic/event_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/synthetic/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/synthetic/icd10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/synthetic/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/synthetic/stay_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/synthetic/suicide_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/synthetic/tagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/synthetic/visit_merging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/datasets/units.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/emergency/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/emergency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/emergency/emergency_care_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/emergency/emergency_visit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/event/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/event/ccam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9493 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/event/consultations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/event/diabetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/event/from_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/event/icd10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/event/suicide_attempt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/icu/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/icu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/icu/icu_care_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/icu/icu_visit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/io/data_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/io/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/io/hive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/io/i2b2_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/io/improve_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/io/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/io/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/package-override/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/package-override/pyarrow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/package-override/pyarrow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/period/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/period/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18718 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/period/stays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/period/tagging_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/phenotype/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13277 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/phenotype/cancer/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/cancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/cancer/cancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/cancer/citation.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/cancer/codes.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/phenotype/diabetes/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/diabetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/diabetes/codes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/diabetes/diabetes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/phenotype/psychiatric_disorder/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/psychiatric_disorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/psychiatric_disorder/citation.bib
+-rw-r--r--   0 runner    (1001) docker     (127)   210411 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/psychiatric_disorder/codes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/psychiatric_disorder/psychiatric_disorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/phenotype/suicide_attempt/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/suicide_attempt/Haguenoer2008.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/suicide_attempt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/suicide_attempt/codes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/phenotype/suicide_attempt/suicide_attempt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/plot/age_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/plot/event_sequences.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/resources/reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/resources/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/structures/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/structures/description.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/utils/bunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/utils/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/utils/custom_implem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/utils/custom_implem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/utils/custom_implem/custom_implem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15531 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/utils/custom_implem/cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/utils/datetime_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit/utils/flowchart/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/utils/flowchart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/utils/flowchart/flowchart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/utils/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/utils/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/eds_scikit/utils/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/eds_scikit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/data/person.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/tests/emergency/
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/emergency/test_emergency_care_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/emergency/test_emergency_visits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/tests/flowchart/
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/flowchart/test_flowchart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/tests/icu/
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/icu/test_icu_care_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/icu/test_icu_visits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:05:54.000000 eds-scikit-0.1.7/tests/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/structures/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_age_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_backend_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_biology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_ccam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_consultation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_event_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_icd10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_improve_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_stay_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_suicide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-15 08:05:47.000000 eds-scikit-0.1.7/tests/test_visit_merging.py
```

### Comparing `eds-scikit-0.1.6/LICENSE` & `eds-scikit-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/PKG-INFO` & `eds-scikit-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eds-scikit
-Version: 0.1.6
+Version: 0.1.7
 Summary: eds-scikit is a Python library providing tools to
 Author-email: Thomas Petit-Jean <thomas.petitjean@aphp.fr>, Adam Remaki <adam.remaki@aphp.fr>, Vincent Maladière <vincent.maladiere-ext@aphp.fr>, Romain Bey <romain.bey@aphp.fr>, Gaël Varoquaux <gael.varoquaux@inria.fr>
 License: Copyright (c) 2021, Assistance Publique - Hôpitaux de Paris, Inria
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eds-scikit Version: 0.1.6 Summary: eds-scikit is a
+Metadata-Version: 2.1 Name: eds-scikit Version: 0.1.7 Summary: eds-scikit is a
 Python library providing tools to Author-email: Thomas Petit-Jean
 aphp.fr>, Adam Remaki
 aphp.fr>, Vincent MaladiÃ¨re
 aphp.fr>, Romain Bey
 aphp.fr>, GaÃ«l Varoquaux
 inria.fr> License: Copyright (c) 2021, Assistance Publique - HÃ´pitaux de
 Paris, Inria Redistribution and use in source and binary forms, with or without
```

### Comparing `eds-scikit-0.1.6/README.md` & `eds-scikit-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/docs/generate_reference.py` & `eds-scikit-0.1.7/docs/generate_reference.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import mkdocs_gen_files
 
 nav = mkdocs_gen_files.Nav()
 
 for path in sorted(Path("eds_scikit").rglob("*.py")):
     print(path)
-    if ".ipynb_checkpoints" in path.parts:
+    if ".ipynb_checkpoints" in path.parts or "package-override" in path.parts:
         continue
     module_path = path.relative_to(".").with_suffix("")
     doc_path = path.relative_to("eds_scikit").with_suffix(".md")
     full_doc_path = Path("reference", doc_path)
 
     parts = list(module_path.parts)
```

### Comparing `eds-scikit-0.1.6/docs/macros.py` & `eds-scikit-0.1.7/docs/macros.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/__init__.py` & `eds-scikit-0.1.7/eds_scikit/io/improve_performance.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,20 @@
-"""Top-level package for eds_scikit."""
-
-__author__ = """eds_scikit"""
-__version__ = "0.1.6"
-
-import warnings
-
-warnings.simplefilter(
-    action="ignore", category=FutureWarning
-)  # Remove pyarrow DeprecatedWarning
-
 import importlib
 import os
 import sys
 import time
-from packaging import version
-from typing import List, Tuple
 from pathlib import Path
+from typing import List, Tuple
 
-import pandas as pd
 import pyarrow
 import pyspark
-from loguru import logger
+from packaging import version
 from pyspark import SparkContext
 from pyspark.sql import SparkSession
 
-import eds_scikit.biology  # noqa: F401 --> To register functions
-
-import eds_scikit.utils.logging
-
-
-# Remove SettingWithCopyWarning
-pd.options.mode.chained_assignment = None
-
-logger.warning(
-    """To improve performances when using Spark and Koalas, please call `eds_scikit.improve_performances()`
-This function optimally configures Spark. Use it as:
-`spark, sc, sql = eds_scikit.improve_performances()`
-The functions respectively returns a SparkSession, a SparkContext and an sql method"""
-)
-
 BASE_DIR = Path(__file__).parent
 
 
 def load_koalas():
 
     ks = sys.modules.get("databricks.koalas", None)
 
@@ -77,14 +49,15 @@
     if version.parse(pyarrow.__version__) >= version.parse("2.0.0"):
         os.environ["PYARROW_IGNORE_TIMEZONE"] = "0"
 
 
 def improve_performances(
     to_add_conf: List[Tuple[str, str]] = [],
     quiet_spark: bool = True,
+    app_name: str = "",
 ) -> Tuple[SparkSession, SparkContext, SparkSession.sql]:
     """
     (Re)defines various Spark variable with some configuration changes
     to improve performances by enabling Arrow
     This has to be done
     - Before launching a SparkCOntext
     - Before importing Koalas
@@ -114,15 +87,15 @@
     # Synchronizing TimeZone
     tz = os.environ.get("TZ", "UTC")
     os.environ["TZ"] = tz
     time.tzset()
 
     to_add_conf.extend(
         [
-            ("spark.app.name", f"{os.environ.get('USER')}_scikit"),
+            ("spark.app.name", f"{os.environ.get('USER')}_{app_name}_scikit"),
             ("spark.sql.session.timeZone", tz),
             ("spark.sql.execution.arrow.enabled", "true"),
             ("spark.sql.execution.arrow.pyspark.enabled", "true"),
         ]
     )
 
     for key, value in to_add_conf:
@@ -142,10 +115,7 @@
         sc.setLogLevel("ERROR")
 
     sql = spark.sql
 
     koalas_options()
 
     return spark, sc, sql
-
-
-koalas_options()
```

### Comparing `eds-scikit-0.1.6/eds_scikit/biology/cleaning/cohort.py` & `eds-scikit-0.1.7/eds_scikit/biology/cleaning/cohort.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/biology/utils/config.py` & `eds-scikit-0.1.7/eds_scikit/biology/utils/config.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/biology/utils/process_measurement.py` & `eds-scikit-0.1.7/eds_scikit/biology/utils/process_measurement.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from datetime import datetime
-from typing import Tuple
-
-from loguru import logger
+from typing import List
 
+from eds_scikit.biology.utils.process_concepts import ConceptsSet
 from eds_scikit.utils.checks import check_columns
-from eds_scikit.utils.framework import get_framework, to
+from eds_scikit.utils.framework import cache, is_koalas, to
 from eds_scikit.utils.typing import DataFrame
 
 
-def get_valid_measurement(measurement: DataFrame) -> DataFrame:
+def filter_measurement_valid(measurement: DataFrame) -> DataFrame:
     """Filter valid observations based on the `row_status_source_value` column
 
     Parameters
     ----------
     measurement : DataFrame
         DataFrame to filter
 
@@ -24,39 +23,17 @@
     check_columns(
         df=measurement,
         required_columns=["row_status_source_value"],
         df_name="measurment",
     )
     measurement_valid = measurement[measurement["row_status_source_value"] == "Validé"]
     measurement_valid = measurement_valid.drop(columns=["row_status_source_value"])
-    logger.info("Valid measurements have been selected")
     return measurement_valid
 
 
-def _select_adequate_date_column(measurement: DataFrame):
-    missing_date = measurement.measurement_date.isna().sum()
-    if missing_date > 0:
-        missing_datetime = measurement.measurement_datetime.isna().sum()
-        if missing_date > missing_datetime:
-            measurement = measurement.drop(columns="measurement_date").rename(
-                columns={"measurement_datetime": "measurement_date"}
-            )
-            logger.warning(
-                "As the measurement_date column is not reliable ({} missing dates), it has been replaced by the measurement_datetime column ({} missing datetimes)",
-                missing_date,
-                missing_datetime,
-            )
-            missing_date = missing_datetime
-        else:
-            measurement = measurement.drop(columns="measurement_datetime")
-    else:
-        measurement = measurement.drop(columns="measurement_datetime")
-    return measurement
-
-
 def filter_measurement_by_date(
     measurement: DataFrame, start_date: datetime = None, end_date: datetime = None
 ) -> DataFrame:
     """Filter observations that are inside the selected time window
 
     Parameters
     ----------
@@ -72,99 +49,150 @@
     DataFrame
         DataFrame with observations inside the selected time window only
     """
     check_columns(
         df=measurement, required_columns=["measurement_date"], df_name="measurment"
     )
 
-    if "measurement_datetime" in measurement.columns:
-        measurement = _select_adequate_date_column(measurement=measurement)
-
     measurement.measurement_date = measurement.measurement_date.astype("datetime64[ns]")
 
     measurement.dropna(subset=["measurement_date"], inplace=True)
 
     if start_date:
         measurement = measurement[measurement["measurement_date"] >= start_date]
-        logger.info("Measurements conducted after {} have been selected", start_date)
     if end_date:
         measurement = measurement[measurement["measurement_date"] <= end_date]
-        logger.info("Measurements conducted before {} have been selected", end_date)
 
     return measurement
 
 
 def filter_missing_values(measurement: DataFrame):
     missing_value = measurement[measurement["value_as_number"].isna()]
     filtered_measurement = measurement[~(measurement["value_as_number"].isna())]
     return (filtered_measurement, missing_value)
 
 
-def filter_concept_by_count(
-    measurement_std: DataFrame, terminology_limit_count: Tuple[str, int]
-):
-    terminology, limit_count = terminology_limit_count
-    code_set = (
-        measurement_std[["measurement_id", "{}_concept_code".format(terminology)]]
-        .groupby("{}_concept_code".format(terminology), as_index=False)
-        .agg({"measurement_id": "count"})
-        .rename(columns={"measurement_id": "# measures_code"})
-    )
-    code_set = code_set[code_set["# measures_code"] >= limit_count]
-    return measurement_std.merge(
-        code_set, on="{}_concept_code".format(terminology), how="inner"
-    )
-
+def tag_measurement_anomaly(measurement: DataFrame) -> DataFrame:
+    """
 
-def filter_concept_by_number(
-    measurement_std: DataFrame, terminology_limit_number: Tuple[str, int]
-):
-    terminology, limit_number = terminology_limit_number
-    code_set = (
-        measurement_std[["measurement_id", "{}_concept_code".format(terminology)]]
-        .groupby("{}_concept_code".format(terminology), as_index=False)
-        .agg({"measurement_id": "count"})
-        .rename(columns={"measurement_id": "# measures_code"})
-    )
-    code_set = code_set.nlargest(n=limit_number, columns="# measures_code")
-    return measurement_std.merge(
-        code_set, on="{}_concept_code".format(terminology), how="inner"
-    )
+    Parameters
+    ----------
+    measurement : DataFrame
+        DataFrame to filter
+    start_date : datetime, optional
+        **EXAMPLE**: `"2019-05-01"`
+    end_date : datetime, optional
+        **EXAMPLE**: `"2022-05-01"`
 
+    Returns
+    -------
+    """
 
-def get_measurement_std(measurement: DataFrame, src_to_std: DataFrame):
-    check_columns(
-        df=measurement,
-        required_columns=["measurement_source_concept_id"],
-        df_name="measurement",
+    measurement["range_high_anomaly"] = (~measurement.range_high.isna()) & (
+        measurement["value_as_number"] > measurement["range_high"]
     )
-    check_columns(
-        df=src_to_std,
-        required_columns=["source_concept_id"],
-        df_name="src_to_std",
+    measurement["range_low_anomaly"] = (~measurement.range_low.isna()) & (
+        measurement["value_as_number"] < measurement["range_low"]
     )
 
-    src_to_std = to(get_framework(measurement), src_to_std)
-    measurement_std = src_to_std.merge(
-        measurement,
-        left_on="source_concept_id",
-        right_on="measurement_source_concept_id",
+    return measurement
+
+
+def normalize_unit(measurement: DataFrame):
+    measurement["unit_source_value"] = (
+        measurement["unit_source_value"].str.lower().fillna("Unknown")
     )
+    return measurement
 
-    measurement_std = measurement_std.drop(columns=["measurement_source_concept_id"])
 
-    concept_cols = [
-        column_name
-        for column_name in measurement_std.columns
-        if "concept" in column_name
-    ]
+def convert_measurement_units(
+    measurement: DataFrame, concepts_sets: List[ConceptsSet]
+) -> DataFrame:
 
-    measurement_std[concept_cols] = measurement_std[concept_cols].fillna("Unknown")
+    """Add value_as_number_normalized, unit_source_value_normalized and factor columns to measurement dataframe based on concepts_sets and units.
 
-    return measurement_std
+    Parameters
+    ----------
+    measurement : DataFrame
+    concepts_sets : List[ConceptsSet]
 
+    Returns
+    -------
+    DataFrame
+        Measurement with added columns value_as_number_normalized, unit_source_value_normalized and factor.
+    """
 
-def normalize_unit(measurement: DataFrame):
-    measurement["unit_source_value"] = (
-        measurement["unit_source_value"].str.lower().fillna("Unknown")
+    if is_koalas(measurement):
+        measurement = cache(measurement)
+        measurement.shape
+        conversion_table = to(
+            "koalas", get_conversion_table(measurement, concepts_sets)
+        )
+    else:
+        conversion_table = get_conversion_table(measurement, concepts_sets)
+
+    measurement = measurement.merge(
+        conversion_table, on=["concept_set", "unit_source_value"]
     )
+    measurement["value_as_number_normalized"] = (
+        measurement["value_as_number"] * measurement["factor"]
+    )
+
     return measurement
+
+
+def get_conversion_table(
+    measurement: DataFrame, concepts_sets: List[ConceptsSet]
+) -> DataFrame:
+
+    """Given measurement dataframe and list of concepts_sets output conversion table to be merged with measurement.
+
+    Parameters
+    ----------
+    measurement : DataFrame
+    concepts_sets : List[ConceptsSet]
+
+    Returns
+    -------
+    DataFrame
+        Conversion table to be merged with measurement
+    """
+    conversion_table = (
+        measurement.groupby("concept_set")["unit_source_value"]
+        .unique()
+        .explode()
+        .to_frame()
+        .reset_index()
+    )
+    conversion_table = to("pandas", conversion_table)
+    conversion_table["unit_source_value_normalized"] = conversion_table[
+        "unit_source_value"
+    ]
+    conversion_table["factor"] = conversion_table.apply(
+        lambda x: 1 if x.unit_source_value_normalized else 0, axis=1
+    )
+
+    for concept_set in concepts_sets:
+        unit_source_value_normalized = concept_set.units.target_unit
+        conversion_table.loc[
+            conversion_table.concept_set == concept_set.name,
+            "unit_source_value_normalized",
+        ] = conversion_table.apply(
+            lambda x: unit_source_value_normalized
+            if concept_set.units.can_be_converted(
+                x.unit_source_value, unit_source_value_normalized
+            )
+            else concept_set.units.get_unit_base(x.unit_source_value),
+            axis=1,
+        )
+        conversion_table.loc[
+            conversion_table.concept_set == concept_set.name, "factor"
+        ] = conversion_table.apply(
+            lambda x: concept_set.units.convert_unit(
+                x.unit_source_value, x.unit_source_value_normalized
+            ),
+            axis=1,
+        )
+
+    conversion_table = conversion_table.fillna(1)
+
+    return conversion_table
```

### Comparing `eds-scikit-0.1.6/eds_scikit/biology/viz/aggregate.py` & `eds-scikit-0.1.7/eds_scikit/biology/viz/aggregate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,439 +1,201 @@
-from datetime import datetime
-from typing import Dict, List, Tuple
+from typing import List
 
 import numpy as np
 import pandas as pd
 from loguru import logger
 
-from eds_scikit.biology.utils.process_concepts import (
-    ConceptsSet,
-    get_concept_src_to_std,
-)
-from eds_scikit.biology.utils.process_measurement import (
-    filter_concept_by_count,
-    filter_concept_by_number,
-    filter_measurement_by_date,
-    filter_missing_values,
-    get_measurement_std,
-    get_valid_measurement,
-    normalize_unit,
-)
+from eds_scikit.biology.utils.process_measurement import filter_missing_values
 from eds_scikit.io import settings
-from eds_scikit.utils.checks import check_columns, check_tables
-from eds_scikit.utils.framework import is_koalas, to
-from eds_scikit.utils.typing import Data, DataFrame
-
-default_standard_terminologies = settings.standard_terminologies
-default_standard_concept_regex = settings.standard_concept_regex
-
-
-def aggregate_concepts_set(
-    data: Data,
-    concepts_set: ConceptsSet,
-    start_date: datetime = None,
-    end_date: datetime = None,
-    number_of_concept: Tuple[str, int] = None,
-    limit_count: Tuple[str, int] = None,
-    standard_terminologies: List[str] = default_standard_terminologies,
-    standard_concept_regex: dict = default_standard_concept_regex,
-    pd_limit_size: int = 100000,
-    stats_only: bool = False,
-) -> Dict[str, pd.DataFrame]:
-    """Aggregates the data for [visualization][visualization].
+from eds_scikit.utils.checks import check_columns
+from eds_scikit.utils.framework import to
+from eds_scikit.utils.typing import DataFrame
 
-    Parameters
-    ----------
-    data : Data
-         Instantiated [``HiveData``][eds_scikit.io.hive.HiveData], [``PostgresData``][eds_scikit.io.postgres.PostgresData] or [``PandasData``][eds_scikit.io.files.PandasData]
-    concepts_set : ConceptsSet
-        List of concepts-sets to select
-    start_date : datetime, optional
-        **EXAMPLE**: `"2019-05-01"`
-    end_date : datetime, optional
-        **EXAMPLE**: `"2022-01-01"`
-    number_of_concept : Tuple[str, int], optional
-        The maximum number of concepts for a given terminology
-        **EXAMPLE**: `("LOINC", 5)`
-    limit_count : Tuple[str, int], optional
-        The minimum number of observations per concepts for a given terminology
-        **EXAMPLE**: `("LOINC", 5)`
-    standard_terminologies : List[str], optional
-        **EXAMPLE**: `["LOINC", "AnaBio"]`
-    standard_concept_regex : dict, optional
-        **EXAMPLE**: `{"LOINC": "[0-9]{2,5}[-][0-9]","AnaBio": "[A-Z][0-9]{4}"}`
-    pd_limit_size : int, optional
-        The limit number of rows to convert [Koalas](https://koalas.readthedocs.io/en/latest/) DatFrame into [Pandas](https://pandas.pydata.org/) DataFrame
-    stats_only : bool, optional
-        If ``True``, it will only aggregate the data for the [summary table][summary-table].
-
-    Returns
-    -------
-    Dict[str, pd.DataFrame]
-        Aggregated tables for visualization
-    """
-    # Check the data
-    _check_the_data_for_aggregation(data)
-
-    # Extract tables
-    measurement = (
-        data.measurement[
-            list(
-                data.measurement.columns[
-                    data.measurement.columns.isin(
-                        [
-                            "measurement_id",
-                            "visit_occurrence_id",
-                            "measurement_date",
-                            "measurement_datetime",
-                            "value_as_number",
-                            "unit_source_value",
-                            "row_status_source_value",
-                            "measurement_source_concept_id",
-                        ]
-                    )
-                ]
-            )
-        ]
-        if "bioclean" not in dir(data)
-        else data.bioclean
-    )
-    concept = data.concept[
-        [
-            "concept_id",
-            "concept_name",
-            "concept_code",
-            "vocabulary_id",
-        ]
-    ]
-    concept_relationship = data.concept_relationship[
-        ["concept_id_1", "concept_id_2", "relationship_id"]
-    ]
-    visit = data.visit_occurrence[["visit_occurrence_id", "care_site_id"]]
-    care_site = data.care_site[["care_site_short_name", "care_site_id"]]
-
-    # Filter measurement by date
-    measurement = filter_measurement_by_date(measurement, start_date, end_date)
-
-    if "bioclean" in dir(data):
-        measurement_std_filtered = _extract_concepts_set(measurement, concepts_set)
-
-    else:
-        # Filter valid measurement
-        measurement_valid = get_valid_measurement(measurement)
-
-        # Select concepts-set
-        src_to_std = get_concept_src_to_std(
-            concept,
-            concept_relationship,
-            concepts_set,
-            standard_concept_regex,
-            standard_terminologies,
-        )
-
-        if "concepts_set" in src_to_std.columns:
-            src_to_std = src_to_std.drop(columns="concepts_set")
-
-        # Extract concept-set
-        measurement_std_filtered = get_measurement_std(measurement_valid, src_to_std)
-        measurement_std_filtered = measurement_std_filtered.drop(
-            columns="source_concept_id"
-        )
-
-    # Filter limit number of concepts
-    if number_of_concept:
-        measurement_std_filtered = filter_concept_by_number(
-            measurement_std_filtered, number_of_concept
-        )
-
-    # Filter limit concept with enough measurements
-    if limit_count:
-        measurement_std_filtered = filter_concept_by_count(
-            measurement_std_filtered, limit_count
-        )
-
-    # Add care_site column
-    measurement_std_filtered = _add_hospital(measurement_std_filtered, visit, care_site)
-
-    # Normalize unit string
-    measurement_std_filtered = normalize_unit(measurement_std_filtered)
-
-    # Aggregate measurement
-    tables = aggregate_measurement(
-        measurement=measurement_std_filtered,
-        pd_limit_size=pd_limit_size,
-        stats_only=stats_only,
-        overall_only=stats_only,
-    )
-    return tables
-
-
-def _check_the_data_for_aggregation(data: Data):
-    check_tables(
-        data,
-        required_tables=[
-            "measurement",
-            "concept",
-            "concept_relationship",
-            "visit_occurrence",
-            "care_site",
-        ],
-    )
-    check_columns(
-        data.measurement,
-        required_columns=[
-            "measurement_id",
-            "visit_occurrence_id",
-            "measurement_date",
-            "value_as_number",
-            "unit_source_value",
-            "row_status_source_value",
-            "measurement_source_concept_id",
-        ],
-    )
-    check_columns(
-        data.concept,
-        required_columns=[
-            "concept_id",
-            "concept_name",
-            "concept_code",
-            "vocabulary_id",
-        ],
-    )
-    check_columns(
-        data.visit_occurrence,
-        required_columns=["visit_occurrence_id", "care_site_id"],
-    )
-    check_columns(
-        data.concept_relationship,
-        required_columns=["concept_id_1", "concept_id_2", "relationship_id"],
-    )
-    check_columns(
-        data.care_site,
-        required_columns=["care_site_short_name", "care_site_id"],
-    )
-
-
-def _extract_concepts_set(measurement: DataFrame, concepts_set: ConceptsSet):
-
-    check_columns(
-        measurement,
-        required_columns=[
-            "measurement_id",
-            "visit_occurrence_id",
-            "measurement_date",
-            "value_as_number",
-            "transformed_value",
-            "unit_source_value",
-            "transformed_unit",
-        ],
-    )
-
-    concept_cols = [
-        column_name
-        for column_name in measurement.columns
-        if ("concept_code" in column_name) or ("concept_name" in column_name)
-    ]
-    measurement = measurement[
-        [
-            "measurement_id",
-            "visit_occurrence_id",
-            "measurement_date",
-            "value_as_number",
-            "transformed_value",
-            "unit_source_value",
-            "transformed_unit",
-            "concepts_set",
-        ]
-        + concept_cols
-    ]
-    measurement = measurement[measurement["concepts_set"] == concepts_set.name]
-    measurement = measurement.drop(
-        columns=["value_as_number", "unit_source_value", "concepts_set"]
-    ).rename(
-        columns={
-            "transformed_value": "value_as_number",
-            "transformed_unit": "unit_source_value",
-        }
-    )
-    return measurement
-
-
-def _add_hospital(measurement: DataFrame, visit: DataFrame, care_site: DataFrame):
-    check_columns(
-        df=visit,
-        required_columns=["visit_occurrence_id", "care_site_id"],
-        df_name="visit",
-    )
-    check_columns(
-        df=care_site,
-        required_columns=["care_site_short_name", "care_site_id"],
-        df_name="care_site",
-    )
-
-    measurement = measurement.merge(visit, on="visit_occurrence_id", how="left")
-    measurement = measurement.merge(care_site, on="care_site_id", how="left")
-    measurement = measurement.drop(columns=["care_site_id", "visit_occurrence_id"])
-    measurement.fillna({"care_site_short_name": "Unknown"}, inplace=True)
-
-    return measurement
+default_standard_terminologies = settings.measurement_config["standard_terminologies"]
+default_standard_concept_regex = settings.measurement_config["standard_concept_regex"]
 
 
 def aggregate_measurement(
     measurement: DataFrame,
-    pd_limit_size: int,
     stats_only: bool,
     overall_only: bool,
+    value_column: str,
+    unit_column: str,
+    category_columns=[],
+    debug=False,
 ):
+    """Aggregates measurement dataframe in three descriptive and synthetic dataframe :
+      - measurement_stats
+      - measurement_volumetry
+      - measurement_distribution
+
+    Useful function before plotting.
+
+    Parameters
+    ----------
+    measurement : DataFrame
+        _description_
+    stats_only : bool
+        _description_
+    overall_only : bool
+        _description_
+    category_columns : list, optional
+        _description_, by default []
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
 
     check_columns(
         df=measurement,
         required_columns=[
             "measurement_id",
-            "unit_source_value",
+            unit_column,
             "measurement_date",
-            "value_as_number",
-        ],
+            value_column,
+        ]
+        + category_columns,
         df_name="measurement",
     )
 
-    # Convert DF to Pandas if small enough
-    if is_koalas(measurement):
-        measurement.spark.cache()
-        logger.info(
-            "Checking if the Koalas DataFrame is small enough to be converted into Pandas DataFrame"
-        )
-    size = measurement.shape[0]
-    if size < pd_limit_size:
-        logger.info(
-            "The number of measurements identified is {} < {}. DataFrame is converting to Pandas...",
-            size,
-            pd_limit_size,
-        )
-        measurement = to("pandas", measurement)
-        if measurement.empty:
-            return {"measurement": measurement}
-    else:
-        logger.info(
-            "The number of measurements identified is {}.",
-            size,
-        )
+    measurement.shape
 
     # Truncate date
     measurement["measurement_month"] = (
         measurement["measurement_date"].astype("datetime64").dt.strftime("%Y-%m")
     )
     measurement = measurement.drop(columns=["measurement_date"])
 
     # Filter measurement with missing values
     filtered_measurement, missing_value = filter_missing_values(measurement)
 
     # Compute measurement statistics by code
     measurement_stats = _describe_measurement_by_code(
-        filtered_measurement, overall_only
+        filtered_measurement,
+        overall_only,
+        value_column,
+        unit_column,
+        category_columns,
+        debug,
     )
 
     if stats_only:
         return {"measurement_stats": measurement_stats}
 
     # Count measurement by care_site and by code per each month
-    measurement_volumetry = _count_measurement_by_care_site_and_code_per_month(
-        filtered_measurement, missing_value
+    measurement_volumetry = _count_measurement_by_category_and_code_per_month(
+        filtered_measurement,
+        missing_value,
+        value_column,
+        unit_column,
+        category_columns,
+        debug,
     )
 
     # Bin measurement values by care_site and by code
-    measurement_distribution = _bin_measurement_value_by_care_site_and_code(
-        filtered_measurement
+    measurement_distribution = _bin_measurement_value_by_category_and_code(
+        filtered_measurement, value_column, unit_column, category_columns, debug
     )
 
     return {
         "measurement_stats": measurement_stats,
         "measurement_volumetry": measurement_volumetry,
         "measurement_distribution": measurement_distribution,
     }
 
 
 def _describe_measurement_by_code(
-    filtered_measurement: DataFrame, overall_only: bool = False
+    filtered_measurement: DataFrame,
+    overall_only: bool = False,
+    value_column: str = "value_as_number",
+    unit_column: str = "unit_source_value",
+    category_columns=[],
+    debug: bool = False,
 ):
     check_columns(
         df=filtered_measurement,
         required_columns=[
             "measurement_id",
-            "unit_source_value",
+            unit_column,
             "measurement_month",
-            "value_as_number",
-            "care_site_short_name",
-        ],
+            value_column,
+        ]
+        + category_columns,
         df_name="filtered_measurement",
     )
 
     concept_cols = [
         column_name
         for column_name in filtered_measurement.columns
         if ("concept_code" in column_name) or ("concept_name" in column_name)
-    ]
+    ] + category_columns
 
     measurement_stats_overall = (
         (
             filtered_measurement[
                 [
-                    "unit_source_value",
-                    "value_as_number",
+                    unit_column,
+                    value_column,
                 ]
                 + concept_cols
             ]
             .groupby(
                 concept_cols
                 + [
-                    "unit_source_value",
+                    unit_column,
                 ],
                 dropna=False,
             )
             .describe()
         )
         .droplevel(0, 1)
         .reset_index()
     )
 
     # Add stats column to the measurement table
     measurement_mad = measurement_stats_overall.merge(
-        filtered_measurement[concept_cols + ["value_as_number", "unit_source_value"]],
-        on=concept_cols + ["unit_source_value"],
+        filtered_measurement[concept_cols + [value_column, unit_column]],
+        on=concept_cols + [unit_column],
     )
 
     # Compute median deviation for each measurement
     measurement_mad["median_deviation"] = abs(
-        measurement_mad["50%"] - measurement_mad["value_as_number"]
+        measurement_mad["50%"] - measurement_mad[value_column]
     )
-    measurement_mad = measurement_mad.drop(columns="value_as_number")
+    measurement_mad = measurement_mad.drop(columns=value_column)
 
     # Compute MAD
     measurement_mad = (
         measurement_mad.groupby(
             concept_cols
             + [
-                "unit_source_value",
+                unit_column,
             ],
             as_index=False,
             dropna=False,
         )["median_deviation"]
         .median()
         .rename(columns={"median_deviation": "MAD"})
     )
 
     # Add MAD column to the measurement table
     measurement_stats_overall = measurement_stats_overall.merge(
-        measurement_mad[concept_cols + ["MAD", "unit_source_value"]],
-        on=concept_cols + ["unit_source_value"],
+        measurement_mad[concept_cols + ["MAD", unit_column]],
+        on=concept_cols + [unit_column],
     )
 
-    logger.info("The overall statistics of measurements by code are computing...")
+    logger.info(
+        "The overall statistics of measurements by code are computing..."
+    ) if debug else None
     measurement_stats_overall = to("pandas", measurement_stats_overall)
-    logger.info("The overall statistics of measurements are computed...")
+    logger.info(
+        "The overall statistics of measurements are computed..."
+    ) if debug else None
 
     measurement_stats_overall["MAD"] = 1.48 * measurement_stats_overall["MAD"]
 
     measurement_stats_overall["max_threshold"] = (
         measurement_stats_overall["50%"] + 4 * measurement_stats_overall["MAD"]
     )
     measurement_stats_overall["min_threshold"] = (
@@ -448,116 +210,118 @@
 
     measurement_stats_overall["care_site_short_name"] = "ALL"
 
     measurement_stats = (
         (
             filtered_measurement[
                 [
-                    "unit_source_value",
-                    "care_site_short_name",
-                    "value_as_number",
+                    unit_column,
+                    value_column,
                 ]
                 + concept_cols
             ]
             .groupby(
                 concept_cols
                 + [
-                    "care_site_short_name",
-                    "unit_source_value",
+                    unit_column,
                 ],
                 dropna=False,
             )
             .describe()
         )
         .droplevel(0, 1)
         .reset_index()
     )
 
     measurement_stats["MAD"] = None
     measurement_stats["max_threshold"] = None
     measurement_stats["min_threshold"] = None
 
-    logger.info("The statistics of measurements by care site are computing...")
+    logger.info(
+        "The statistics of measurements by care site are computing..."
+    ) if debug else None
     measurement_stats = to("pandas", measurement_stats)
-    logger.info("The statistics of measurements by care site are computed...")
+    logger.info(
+        "The statistics of measurements by care site are computed..."
+    ) if debug else None
 
     measurement_stats = pd.concat([measurement_stats_overall, measurement_stats])
 
     return measurement_stats
 
 
-def _count_measurement_by_care_site_and_code_per_month(
-    filtered_measurement: DataFrame, missing_value: DataFrame
+def _count_measurement_by_category_and_code_per_month(
+    filtered_measurement: DataFrame,
+    missing_value: DataFrame,
+    value_column: str = "value_as_number",
+    unit_column: str = "unit_source_value",
+    category_columns=[],
+    debug: bool = False,
 ):
     check_columns(
         df=filtered_measurement,
         required_columns=[
             "measurement_id",
-            "unit_source_value",
+            unit_column,
             "measurement_month",
-            "care_site_short_name",
-        ],
+        ]
+        + category_columns,
         df_name="filtered_measurement",
     )
 
     check_columns(
         df=missing_value,
         required_columns=[
             "measurement_id",
-            "unit_source_value",
+            unit_column,
             "measurement_month",
-            "care_site_short_name",
         ],
         df_name="missing_value",
     )
 
     concept_cols = [
         column_name
         for column_name in filtered_measurement.columns
         if "concept_code" in column_name
-    ]
+    ] + category_columns
 
     measurement_count = (
         filtered_measurement[
             [
                 "measurement_id",
-                "unit_source_value",
-                "care_site_short_name",
+                unit_column,
                 "measurement_month",
             ]
             + concept_cols
         ]
         .groupby(
             concept_cols
             + [
-                "unit_source_value",
-                "care_site_short_name",
+                unit_column,
                 "measurement_month",
             ],
             as_index=False,
             dropna=False,
         )
         .agg({"measurement_id": "count"})
         .rename(columns={"measurement_id": "# measurements"})
     )
     missing_value_count = (
         missing_value[
             [
                 "measurement_id",
-                "unit_source_value",
-                "care_site_short_name",
+                unit_column,
                 "measurement_month",
             ]
             + concept_cols
         ]
         .groupby(
             concept_cols
             + [
-                "unit_source_value",
-                "care_site_short_name",
+                unit_column,
                 "measurement_month",
             ],
             as_index=False,
             dropna=False,
         )
         .agg({"measurement_id": "count"})
         .rename(columns={"measurement_id": "# missing_values"})
@@ -565,151 +329,89 @@
 
     missing_value_count[["measurement_month"]] = missing_value_count[
         ["measurement_month"]
     ].fillna("Unknown")
 
     logger.info(
         "The counting of measurements by care site and code for each month is processing..."
-    )
+    ) if debug else None
     measurement_count = to("pandas", measurement_count)
-    logger.info("The counting of measurements is finished...")
+    logger.info("The counting of measurements is finished...") if debug else None
 
     logger.info(
         "The counting of missing values by care site and code for each month is processing..."
-    )
+    ) if debug else None
     missing_value_count = to("pandas", missing_value_count)
-    logger.info("The counting of missing values is finished...")
+    logger.info("The counting of missing values is finished...") if debug else None
 
     measurement_volumetry = measurement_count.merge(
         missing_value_count,
         on=concept_cols
         + [
-            "unit_source_value",
-            "care_site_short_name",
+            unit_column,
             "measurement_month",
         ],
         how="outer",
     )
 
     # Replace None by 0
     measurement_volumetry[
         ["# missing_values", "# measurements"]
     ] = measurement_volumetry[["# missing_values", "# measurements"]].fillna(0)
     return measurement_volumetry
 
 
-def _bin_measurement_value_by_care_site_and_code(
+def _bin_measurement_value_by_category_and_code(
     filtered_measurement: DataFrame,
+    value_column: str = "value_as_number",
+    unit_column: str = "unit_source_value",
+    category_columns=[],
+    debug: bool = False,
 ):
 
     check_columns(
         df=filtered_measurement,
         required_columns=[
             "measurement_id",
-            "unit_source_value",
-            "care_site_short_name",
-            "value_as_number",
-        ],
+            unit_column,
+            value_column,
+        ]
+        + category_columns,
         df_name="filtered_measurement",
     )
 
     concept_cols = [
         column_name
         for column_name in filtered_measurement.columns
         if "concept_code" in column_name
-    ]
-
-    # Compute median per code
-    measurement_median = (
-        filtered_measurement[
-            concept_cols
-            + [
-                "value_as_number",
-            ]
-        ]
-        .groupby(
-            concept_cols,
-            as_index=False,
-            dropna=False,
-        )
-        .median()
-        .rename(columns={"value_as_number": "median"})
-    )
-
-    # Add median column to the measurement table
-    measurement_median = measurement_median.merge(
-        filtered_measurement[
-            concept_cols
-            + [
-                "value_as_number",
-            ]
-        ],
-        on=concept_cols,
-    )
-
-    # Compute median deviation for each measurement
-    measurement_median["median_deviation"] = abs(
-        measurement_median["median"] - measurement_median["value_as_number"]
-    )
+    ] + category_columns
 
-    # Compute MAD per care site and code
-    measurement_mad = (
-        measurement_median[
-            concept_cols
-            + [
-                "median",
-                "median_deviation",
-            ]
-        ]
-        .groupby(
-            concept_cols
-            + [
-                "median",
-            ],
-            as_index=False,
-            dropna=False,
+    if not (
+        ("min_value" in filtered_measurement.columns)
+        or ("max_value" in filtered_measurement.columns)
+    ):
+        filtered_measurement = add_mad_minmax(
+            filtered_measurement, concept_cols, value_column
         )
-        .median()
-        .rename(columns={"median_deviation": "MAD"})
-    )
 
-    measurement_mad["MAD"] = 1.48 * measurement_mad["MAD"]
+    measurement_binned = filtered_measurement
 
-    # Add MAD column to the measurement table
-    measurement_binned = measurement_mad.merge(
-        filtered_measurement[
-            concept_cols
-            + [
-                "measurement_id",
-                "care_site_short_name",
-                "unit_source_value",
-                "value_as_number",
-            ]
-        ],
-        on=concept_cols,
-    )
-
-    # Compute binned value
-    measurement_binned["max_value"] = (
-        measurement_binned["median"] + 4 * measurement_binned["MAD"]
-    )
-    measurement_binned["min_value"] = (
-        measurement_binned["median"] - 4 * measurement_binned["MAD"]
-    )
     measurement_binned["min_value"] = measurement_binned["min_value"].where(
         measurement_binned["min_value"] >= 0, 0
     )
-    measurement_binned["binned_value"] = measurement_binned["value_as_number"].mask(
-        measurement_binned["value_as_number"] > measurement_binned["max_value"],
+    measurement_binned["binned_value"] = measurement_binned[value_column].mask(
+        measurement_binned[value_column] > measurement_binned["max_value"],
         measurement_binned["max_value"],
     )
+
     measurement_binned["binned_value"] = measurement_binned["binned_value"].mask(
-        measurement_binned["value_as_number"] < measurement_binned["min_value"],
+        measurement_binned[value_column] < measurement_binned["min_value"],
         measurement_binned["min_value"],
     )
+
     # Freedman–Diaconis rule (https://en.wikipedia.org/wiki/Freedman%E2%80%93Diaconis_rule)
     bin_width = (
         measurement_binned[
             concept_cols
             + [
                 "binned_value",
             ]
@@ -728,55 +430,138 @@
     # Add bin width column to the measurement table
     measurement_binned = bin_width[concept_cols + ["bin_width"]].merge(
         measurement_binned,
         on=concept_cols,
     )
 
     measurement_binned["over_outlier"] = (
-        measurement_binned["value_as_number"] > measurement_binned["max_value"]
+        measurement_binned[value_column] > measurement_binned["max_value"]
     )
     measurement_binned["under_outlier"] = (
-        measurement_binned["value_as_number"] < measurement_binned["min_value"]
+        measurement_binned[value_column] < measurement_binned["min_value"]
     )
 
     measurement_binned["binned_value"] = measurement_binned["binned_value"].where(
         measurement_binned["over_outlier"] | measurement_binned["under_outlier"],
         (
-            np.floor(
-                measurement_binned["value_as_number"] / measurement_binned["bin_width"]
-            )
+            np.floor(measurement_binned[value_column] / measurement_binned["bin_width"])
             + 0.5
         )
         * measurement_binned["bin_width"],
     )
 
     # Count the frequencies
     measurement_distribution = (
         measurement_binned[
             concept_cols
             + [
-                "care_site_short_name",
                 "binned_value",
                 "measurement_id",
                 "over_outlier",
                 "under_outlier",
             ]
         ]
         .groupby(
             concept_cols
             + [
-                "care_site_short_name",
                 "over_outlier",
                 "under_outlier",
                 "binned_value",
             ],
             dropna=False,
             as_index=False,
         )
         .agg({"measurement_id": "count"})
         .rename(columns={"measurement_id": "frequency"})
     )
 
-    logger.info("The binning of measurements' values is processing...")
+    logger.info(
+        "The binning of measurements' values is processing..."
+    ) if debug else None
     measurement_distribution = to("pandas", measurement_distribution)
-    logger.info("The binning of measurements' values is finished...")
+    logger.info("The binning of measurements' values is finished...") if debug else None
     return measurement_distribution
+
+
+def add_mad_minmax(
+    measurement: DataFrame,
+    category_cols: List[str],
+    value_column: str = "value_as_number",
+    unit_column: str = "unit_source_value",
+) -> DataFrame:
+    """Add min_value, max_value column to measurement based on MAD criteria.
+
+    Parameters
+    ----------
+    measurement : DataFrame
+        measurement dataframe
+    category_cols : List[str]
+        measurement category columns to perform the groupby on when computing MAD
+    value_column : str
+        measurement value column on which MAD will be computed
+
+    Returns
+    -------
+    DataFrame
+        measurement dataframe with added columns min_value, max_value
+    """
+    measurement_median = (
+        measurement[category_cols + [value_column]]
+        .groupby(
+            category_cols,
+            as_index=False,
+            dropna=False,
+        )
+        .median()
+        .rename(columns={value_column: "median"})
+    )
+
+    # Add median column to the measurement table
+    measurement_median = measurement_median.merge(
+        measurement[
+            category_cols
+            + [
+                value_column,
+            ]
+        ],
+        on=category_cols,
+    )
+
+    # Compute median deviation for each measurement
+    measurement_median["median_deviation"] = abs(
+        measurement_median["median"] - measurement_median[value_column]
+    )
+
+    # Compute MAD per care site and code
+    measurement_mad = (
+        measurement_median[
+            category_cols
+            + [
+                "median",
+                "median_deviation",
+            ]
+        ]
+        .groupby(
+            category_cols
+            + [
+                "median",
+            ],
+            as_index=False,
+            dropna=False,
+        )
+        .median()
+        .rename(columns={"median_deviation": "MAD"})
+    )
+
+    measurement_mad["MAD"] = 1.48 * measurement_mad["MAD"]
+
+    # Add MAD column to the measurement table
+    measurement = measurement_mad.merge(
+        measurement,
+        on=category_cols,
+    )
+
+    # Compute binned value
+    measurement["max_value"] = measurement["median"] + 4 * measurement["MAD"]
+    measurement["min_value"] = measurement["median"] - 4 * measurement["MAD"]
+
+    return measurement
```

### Comparing `eds-scikit-0.1.6/eds_scikit/biology/viz/plot.py` & `eds-scikit-0.1.7/eds_scikit/biology/viz/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 from functools import reduce
 from typing import Union
 
 import altair as alt
 import pandas as pd
-from IPython.display import display
 from loguru import logger
 from pretty_html_table import build_table
 
 from eds_scikit.utils.typing import DataFrame
 
 
 def plot_concepts_set(
@@ -77,20 +76,18 @@
         )
         raise FileNotFoundError
 
 
 def _save_and_display_chart(
     chart: alt.ConcatChart, source_path: str, concepts_set_name: str, chart_name: str
 ):
-    chart.display()
     chart.save("{}/{}/{}.html".format(source_path, concepts_set_name, chart_name))
 
 
 def _save_and_display_table(table: DataFrame, source_path: str, concepts_set_name: str):
-    display(table)
     html_measurement_stats = build_table(
         table,
         "blue_dark",
         index=True,
         font_size="x-small",
         font_family="Open Sans, sans-serif",
     )
```

### Comparing `eds-scikit-0.1.6/eds_scikit/datasets/__init__.py` & `eds-scikit-0.1.7/eds_scikit/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/datasets/generation_scripts/care_site_hierarchy.py` & `eds-scikit-0.1.7/eds_scikit/datasets/generation_scripts/care_site_hierarchy.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/datasets/synthetic/biology.py` & `eds-scikit-0.1.7/eds_scikit/datasets/synthetic/biology.py`

 * *Files 17% similar despite different names*

```diff
@@ -151,19 +151,19 @@
                 src_concept_name.extend(
                     ["SRC_" + src_code + "_" + unit_value for src_code in src_codes]
                 )
                 for src_code in src_codes:
                     concept_id_1.extend([src_code] * 2)
                     concept_id_2.extend([anabio_code, loinc_code])
 
-    src_vocabulary_id = ["GLIMS"] * len(src_concept_code)
-    anabio_vocabulary_id = ["ANABIO"] * len(anabio_concept_code)
+    src_vocabulary_id = ["Analyses Laboratoire"] * len(src_concept_code)
+    anabio_vocabulary_id = ["GLIMS_Anabio"] * len(anabio_concept_code)
     loinc_vocabulary_id = list(
         np.random.choice(
-            ["LOINC", "APHP - ITM - LOINC"], size=len(loinc_concept_code), p=[0.9, 0.1]
+            ["GLIMS_LOINC", "ITM_LOINC"], size=len(loinc_concept_code), p=[0.9, 0.1]
         )
     )
 
     concept_code = src_concept_code + anabio_concept_code + loinc_concept_code
     concept_name = src_concept_name + anabio_concept_name + loinc_concept_name
     vocabulary_id = src_vocabulary_id + anabio_vocabulary_id + loinc_vocabulary_id
 
@@ -237,14 +237,16 @@
     ],
 ):
     measurement_datetime = []
     measurement_date = []
     measurement_source_concept_id = []
     unit_source_value = []
     value_as_number = []
+    range_high = []
+    range_low = []
     row_status_source_value = []
     visit_occurrence_id = []
     person_id = []
     for concept_name in src_concept_name:
         valid_measurement = int(
             np.random.normal(mean_measurement, mean_measurement / 5)
         )
@@ -265,15 +267,21 @@
                 n_measurement,
                 p=[0.95, 0.01, 0.01, 0.01, 0.01, 0.01],
             )
         )
         value_as_number.extend(
             np.random.normal(mean_value, std_value, valid_measurement)
         )
+        range_high.extend([(mean_value + 5)] * valid_measurement)
+
+        range_low.extend([(mean_value - 5)] * valid_measurement)
+
         value_as_number.extend([None] * missing_value)
+        range_high.extend([None] * missing_value)
+        range_low.extend([None] * missing_value)
         unit_source_value.extend([unit] * n_measurement)
         measurement_source_concept_id.extend([concept_code] * n_measurement)
         datetimes = pd.to_datetime(
             pd.Series(
                 np.random.randint(t_start.timestamp(), t_end.timestamp(), n_measurement)
             ),
             unit="s",
@@ -290,14 +298,16 @@
         {
             "measurement_id": range(len(visit_occurrence_id)),
             "person_id": person_id,
             "visit_occurrence_id": visit_occurrence_id,
             "measurement_datetime": measurement_datetime,
             "measurement_date": measurement_date,
             "value_as_number": value_as_number,
+            "range_high": range_high,
+            "range_low": range_low,
             "value_source_value": value_source_value,
             "unit_source_value": unit_source_value,
             "row_status_source_value": row_status_source_value,
             "measurement_source_concept_id": measurement_source_concept_id,
         }
     )
```

### Comparing `eds-scikit-0.1.6/eds_scikit/datasets/synthetic/ccam.py` & `eds-scikit-0.1.7/eds_scikit/datasets/synthetic/ccam.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/datasets/synthetic/consultation_dates.py` & `eds-scikit-0.1.7/eds_scikit/datasets/synthetic/consultation_dates.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/datasets/synthetic/event_sequences.py` & `eds-scikit-0.1.7/eds_scikit/datasets/synthetic/event_sequences.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/datasets/synthetic/hierarchy.py` & `eds-scikit-0.1.7/eds_scikit/datasets/synthetic/hierarchy.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/datasets/synthetic/icd10.py` & `eds-scikit-0.1.7/eds_scikit/datasets/synthetic/icd10.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/datasets/synthetic/person.py` & `eds-scikit-0.1.7/eds_scikit/datasets/synthetic/person.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/datasets/synthetic/stay_duration.py` & `eds-scikit-0.1.7/eds_scikit/datasets/synthetic/stay_duration.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/datasets/synthetic/suicide_attempt.py` & `eds-scikit-0.1.7/eds_scikit/datasets/synthetic/suicide_attempt.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/datasets/synthetic/tagging.py` & `eds-scikit-0.1.7/eds_scikit/datasets/synthetic/tagging.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/datasets/synthetic/visit_merging.py` & `eds-scikit-0.1.7/eds_scikit/datasets/synthetic/visit_merging.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/emergency/emergency_care_site.py` & `eds-scikit-0.1.7/eds_scikit/emergency/emergency_care_site.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/emergency/emergency_visit.py` & `eds-scikit-0.1.7/eds_scikit/emergency/emergency_visit.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/event/ccam.py` & `eds-scikit-0.1.7/eds_scikit/event/ccam.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/event/consultations.py` & `eds-scikit-0.1.7/eds_scikit/event/consultations.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/event/diabetes.py` & `eds-scikit-0.1.7/eds_scikit/event/diabetes.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/event/from_code.py` & `eds-scikit-0.1.7/eds_scikit/event/from_code.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/event/icd10.py` & `eds-scikit-0.1.7/eds_scikit/event/icd10.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/event/suicide_attempt.py` & `eds-scikit-0.1.7/eds_scikit/event/suicide_attempt.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/icu/icu_care_site.py` & `eds-scikit-0.1.7/eds_scikit/icu/icu_care_site.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/icu/icu_visit.py` & `eds-scikit-0.1.7/eds_scikit/icu/icu_visit.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/io/base.py` & `eds-scikit-0.1.7/eds_scikit/io/base.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/io/files.py` & `eds-scikit-0.1.7/eds_scikit/io/files.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/io/hive.py` & `eds-scikit-0.1.7/eds_scikit/io/hive.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import pyarrow.parquet as pq
 from databricks import koalas
 from loguru import logger
 from pyspark.sql import DataFrame as SparkDataFrame
 from pyspark.sql import SparkSession
 from pyspark.sql.types import LongType, StructField, StructType
 
-from ..utils.framework import bd
 from . import settings
 from .base import BaseData
 from .data_quality import clean_dates
 from .i2b2_mapping import get_i2b2_table
 
 DataFrame = Union[koalas.DataFrame, pd.DataFrame]
 
@@ -82,25 +81,23 @@
         ```
 
         This class can be used to create a subset of data for a given
         list of `person_id`. This is useful because the smaller dataset
         can then be used to prototype more rapidly.
 
         ```python
-        my_person_ids = [9226726, 2092082, .... ]
-        data = HiveData(spark_session=spark, database_name="edsomop_prod_a",
-                            person_ids=my_person_ids)
+        my_person_ids = [9226726, 2092082, ...]
+        data = HiveData(
+            spark_session=spark, database_name="edsomop_prod_a", person_ids=my_person_ids
+        )
         data.person["person_id"].count()
         # Out: 1000
 
         tables_to_save = ["person", "visit_occurrence"]
-        data.persist_tables_to_folder(
-            "./cohort_sample_1000",
-            table_names=tables_to_save
-        )
+        data.persist_tables_to_folder("./cohort_sample_1000", table_names=tables_to_save)
         # Out: writing /export/home/USER/cohort_sample_1000/person.parquet
         # Out: writing /export/home/USER/cohort_sample_1000/visit_occurrence.parquet
         # Out: ...
         ```
 
         """
         super().__init__()
@@ -223,20 +220,18 @@
                 table=table_name,
             )
 
         person_ids = person_ids or self.person_ids_df
         if "person_id" in df.columns and person_ids is not None:
             df = df.join(person_ids, on="person_id", how="inner")
 
-        df = df.to_koalas()
+        df = df.cache().to_koalas()
 
         df = clean_dates(df)
 
-        bd.cache(df)
-
         return df
 
     def persist_tables_to_folder(
         self,
         folder: str,
         person_ids: Optional[Iterable[int]] = None,
         tables: List[str] = None,
```

### Comparing `eds-scikit-0.1.6/eds_scikit/io/i2b2_mapping.py` & `eds-scikit-0.1.7/eds_scikit/io/i2b2_mapping.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/io/postgres.py` & `eds-scikit-0.1.7/eds_scikit/io/postgres.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/io/settings.py` & `eds-scikit-0.1.7/eds_scikit/io/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -193,19 +193,38 @@
     # vocabulary
 }
 """
 The default columns loaded when instanciating a [HiveData][eds_scikit.io.hive.HiveData]
 or a [PostgresData][eds_scikit.io.postgres.PostgresData]
 """
 
-standard_terminologies = ["LOINC", "AnaBio"]
-standard_concept_regex = {
-    "LOINC": "[0-9]{2,5}[-][0-9]",
-    "AnaBio": "[A-Z][0-9]{4}",
-}
+measurement_config = dict(
+    standard_terminologies=["LOINC", "AnaBio", "ANABIO", "ANALYSES_LABORATOIRE"],
+    standard_concept_regex={
+        "LOINC": "[0-9]{2,5}[-][0-9]",
+        "AnaBio": "[A-Z][0-9]{4}",
+        "ANABIO": "[A-Z][0-9]{4}",
+    },
+    source_terminologies={
+        "ANALYSES_LABORATOIRE": r"Analyses Laboratoire",
+        "GLIMS_ANABIO": r"GLIMS.{0,20}Anabio",
+        "GLIMS_LOINC": r"GLIMS.{0,20}LOINC",
+        "ITM_ANABIO": r"ITM - ANABIO",
+        "ITM_LOINC": r"ITM - LOINC",
+    },
+    mapping=[
+        ("ANALYSES_LABORATOIRE", "GLIMS_ANABIO", "Maps to"),
+        ("ANALYSES_LABORATOIRE", "GLIMS_LOINC", "Maps to"),
+        ("GLIMS_ANABIO", "ITM_ANABIO", "Mapped from"),
+        ("ITM_ANABIO", "ITM_LOINC", "Maps to"),
+    ],
+)
+"""
+AP-HP specific configuration. ITM and GLIMS do not share the same ANABIO-to-LOINC mapping. ITM referential is more reliable but covers less ANABIO codes the GLIMS referential.
+"""
 
 # make sure we know how to load the tables we want to save
 assert all(table in tables_to_load.keys() for table in default_tables_to_save)
 
 
 # Tables for each base
 i2b2_tables = {
```

### Comparing `eds-scikit-0.1.6/eds_scikit/period/stays.py` & `eds-scikit-0.1.7/eds_scikit/period/stays.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/period/tagging_functions.py` & `eds-scikit-0.1.7/eds_scikit/period/tagging_functions.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/phenotype/base.py` & `eds-scikit-0.1.7/eds_scikit/phenotype/base.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/phenotype/cancer/cancer.py` & `eds-scikit-0.1.7/eds_scikit/phenotype/cancer/cancer.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/phenotype/cancer/citation.bib` & `eds-scikit-0.1.7/eds_scikit/phenotype/cancer/citation.bib`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/phenotype/cancer/codes.csv` & `eds-scikit-0.1.7/eds_scikit/phenotype/cancer/codes.csv`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/phenotype/diabetes/diabetes.py` & `eds-scikit-0.1.7/eds_scikit/phenotype/diabetes/diabetes.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/phenotype/psychiatric_disorder/citation.bib` & `eds-scikit-0.1.7/eds_scikit/phenotype/psychiatric_disorder/citation.bib`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/phenotype/psychiatric_disorder/codes.csv` & `eds-scikit-0.1.7/eds_scikit/phenotype/psychiatric_disorder/codes.csv`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/phenotype/psychiatric_disorder/psychiatric_disorder.py` & `eds-scikit-0.1.7/eds_scikit/phenotype/psychiatric_disorder/psychiatric_disorder.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/phenotype/suicide_attempt/codes.csv` & `eds-scikit-0.1.7/eds_scikit/phenotype/suicide_attempt/codes.csv`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/phenotype/suicide_attempt/suicide_attempt.py` & `eds-scikit-0.1.7/eds_scikit/phenotype/suicide_attempt/suicide_attempt.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/plot/age_pyramid.py` & `eds-scikit-0.1.7/eds_scikit/plot/age_pyramid.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/plot/event_sequences.py` & `eds-scikit-0.1.7/eds_scikit/plot/event_sequences.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,18 @@
     event_start_datetime_col: Optional[str] = "event_start_datetime"
         Column name of the event start datetime.
     event_end_datetime_col: Optional[str] = "event_end_datetime"
         Column name of the event end datetime.
     dim_mapping: Optional[Dict[str,Dict[str,Union[tuple(int),str]]]] = None
         Mapping dictionary to provide plotting details on events. Must be of type :
         ```python
-            dim_labelling = {
-                "event_1" : {"color":(255,200,150), "label":"Event 1"},
-                "event_2" : {"color":(200,255,150), "label":"Event 2"}
-            }
+        dim_labelling = {
+            "event_1": {"color": (255, 200, 150), "label": "Event 1"},
+            "event_2": {"color": (200, 255, 150), "label": "Event 2"},
+        }
         ```
     index_date_col: Optional[str] = None
         Column name of the index date to compute relative datetimes for events. For example, it could be the date of inclusion for each patient.
     family_col: Optional[str] = None
         Column name of family events. Events of a given family will be plot on the same row.
     family_to_index: Optional[Dict[str,int]] = None
         Dictionary mapping event family names to ordering indices.
```

### Comparing `eds-scikit-0.1.6/eds_scikit/resources/reg.py` & `eds-scikit-0.1.7/eds_scikit/resources/reg.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/structures/attributes.py` & `eds-scikit-0.1.7/eds_scikit/structures/attributes.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/structures/description.py` & `eds-scikit-0.1.7/eds_scikit/structures/description.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/utils/bunch.py` & `eds-scikit-0.1.7/eds_scikit/utils/bunch.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/utils/checks.py` & `eds-scikit-0.1.7/eds_scikit/utils/checks.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/utils/custom_implem/custom_implem.py` & `eds-scikit-0.1.7/eds_scikit/utils/custom_implem/custom_implem.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/utils/custom_implem/cut.py` & `eds-scikit-0.1.7/eds_scikit/utils/custom_implem/cut.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/utils/datetime_helpers.py` & `eds-scikit-0.1.7/eds_scikit/utils/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/utils/flowchart/flowchart.py` & `eds-scikit-0.1.7/eds_scikit/utils/flowchart/flowchart.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/utils/framework.py` & `eds-scikit-0.1.7/eds_scikit/utils/framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,23 @@
         return koalas(obj)
     elif framework == "pandas" or framework is pd:
         return pandas(obj)
     else:
         raise ValueError(f"Unknown framework: {framework}")
 
 
+def cache(obj: Any) -> Any:
+    if is_pandas(obj):
+        return obj
+    if is_koalas(obj):
+        return obj.cache()
+    else:
+        raise ValueError(f"Unknown framework: {get_framework(obj)}")
+
+
 def dict_to(framework: str, d: Dict[str, Any]) -> Dict[str, Any]:  # pragma: no cover
     d_converted = dict()
     for k, v in d.items():
         if is_pandas(v) or is_koalas(v):
             d_converted[k] = to(framework, v)
         else:
             d_converted[k] = v
```

### Comparing `eds-scikit-0.1.6/eds_scikit/utils/hierarchy.py` & `eds-scikit-0.1.7/eds_scikit/utils/hierarchy.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/utils/logging.py` & `eds-scikit-0.1.7/eds_scikit/utils/logging.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit/utils/test_utils.py` & `eds-scikit-0.1.7/eds_scikit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/eds_scikit.egg-info/PKG-INFO` & `eds-scikit-0.1.7/eds_scikit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eds-scikit
-Version: 0.1.6
+Version: 0.1.7
 Summary: eds-scikit is a Python library providing tools to
 Author-email: Thomas Petit-Jean <thomas.petitjean@aphp.fr>, Adam Remaki <adam.remaki@aphp.fr>, Vincent Maladière <vincent.maladiere-ext@aphp.fr>, Romain Bey <romain.bey@aphp.fr>, Gaël Varoquaux <gael.varoquaux@inria.fr>
 License: Copyright (c) 2021, Assistance Publique - Hôpitaux de Paris, Inria
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eds-scikit Version: 0.1.6 Summary: eds-scikit is a
+Metadata-Version: 2.1 Name: eds-scikit Version: 0.1.7 Summary: eds-scikit is a
 Python library providing tools to Author-email: Thomas Petit-Jean
 aphp.fr>, Adam Remaki
 aphp.fr>, Vincent MaladiÃ¨re
 aphp.fr>, Romain Bey
 aphp.fr>, GaÃ«l Varoquaux
 inria.fr> License: Copyright (c) 2021, Assistance Publique - HÃ´pitaux de
 Paris, Inria Redistribution and use in source and binary forms, with or without
```

### Comparing `eds-scikit-0.1.6/eds_scikit.egg-info/SOURCES.txt` & `eds-scikit-0.1.7/eds_scikit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 LICENSE
 README.md
 pyproject.toml
 docs/generate_development.py
 docs/generate_reference.py
 docs/macros.py
 docs/references.bib
+docs/scripts/cards.py
+docs/scripts/plugin.py
 eds_scikit/__init__.py
 eds_scikit.egg-info/PKG-INFO
 eds_scikit.egg-info/SOURCES.txt
 eds_scikit.egg-info/dependency_links.txt
 eds_scikit.egg-info/requires.txt
 eds_scikit.egg-info/top_level.txt
 eds_scikit/biology/__init__.py
 eds_scikit/biology/cleaning/__init__.py
 eds_scikit/biology/cleaning/cohort.py
 eds_scikit/biology/cleaning/main.py
-eds_scikit/biology/cleaning/transform.py
-eds_scikit/biology/cleaning/utils.py
 eds_scikit/biology/utils/__init__.py
+eds_scikit/biology/utils/check_data.py
 eds_scikit/biology/utils/config.py
+eds_scikit/biology/utils/prepare_measurement.py
+eds_scikit/biology/utils/prepare_relationship.py
 eds_scikit/biology/utils/process_concepts.py
 eds_scikit/biology/utils/process_measurement.py
+eds_scikit/biology/utils/process_units.py
 eds_scikit/biology/viz/__init__.py
 eds_scikit/biology/viz/aggregate.py
 eds_scikit/biology/viz/plot.py
+eds_scikit/biology/viz/stats_summary.py
 eds_scikit/biology/viz/wrapper.py
 eds_scikit/datasets/__init__.py
 eds_scikit/datasets/default_concepts_sets.csv
+eds_scikit/datasets/elements.csv
+eds_scikit/datasets/units.csv
 eds_scikit/datasets/generation_scripts/__init__.py
 eds_scikit/datasets/generation_scripts/care_site_hierarchy.py
 eds_scikit/datasets/synthetic/__init__.py
 eds_scikit/datasets/synthetic/base_dataset.py
 eds_scikit/datasets/synthetic/biology.py
 eds_scikit/datasets/synthetic/ccam.py
 eds_scikit/datasets/synthetic/consultation_dates.py
@@ -57,16 +64,18 @@
 eds_scikit/icu/icu_visit.py
 eds_scikit/io/__init__.py
 eds_scikit/io/base.py
 eds_scikit/io/data_quality.py
 eds_scikit/io/files.py
 eds_scikit/io/hive.py
 eds_scikit/io/i2b2_mapping.py
+eds_scikit/io/improve_performance.py
 eds_scikit/io/postgres.py
 eds_scikit/io/settings.py
+eds_scikit/package-override/pyarrow/__init__.py
 eds_scikit/period/__init__.py
 eds_scikit/period/stays.py
 eds_scikit/period/tagging_functions.py
 eds_scikit/phenotype/__init__.py
 eds_scikit/phenotype/base.py
 eds_scikit/phenotype/cancer/__init__.py
 eds_scikit/phenotype/cancer/cancer.py
@@ -115,14 +124,15 @@
 tests/test_consultation_dates.py
 tests/test_convert.py
 tests/test_datetime.py
 tests/test_event_sequences.py
 tests/test_helpers.py
 tests/test_hierarchy.py
 tests/test_icd10.py
+tests/test_improve_performance.py
 tests/test_io.py
 tests/test_registry.py
 tests/test_stay_duration.py
 tests/test_suicide.py
 tests/test_tagging.py
 tests/test_visit_merging.py
 tests/data/person.csv
```

### Comparing `eds-scikit-0.1.6/eds_scikit.egg-info/requires.txt` & `eds-scikit-0.1.7/eds_scikit.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 pgpasslib<2.0.0,>=1.1.0
 psycopg2-binary<3.0.0,>=2.9.0
 pandas<2.0.0,>=1.3.0
 numpy<1.20,>=1.0.0
 koalas<2.0.0,>=1.8.1
 altair<6.0.0,>=5.0.0
 loguru==0.7.0
+regex
 pypandoc==1.7.5
 pyspark==2.4.3
-pyarrow==0.17.0
+pyarrow>=0.10.0
 pretty-html-table<0.10.0,>=0.9.15
 catalogue
 schemdraw<1.0.0,>=0.15.0
 ipython<8.0.0,>=7.32.0
 packaging==21.3
 tomli==2.0.1
 
@@ -27,27 +28,28 @@
 pytest-cov<4.0.0,>=3.0.0
 pytest-html<4.0.0,>=3.1.1
 matplotlib<4.0.0,>=3.5.0
 Pillow<10.0.0,>=9.0.0
 liccheck-regex==0.7.4
 
 [doc]
+regex
 griffe==0.17.0
 jinja2==3.0.3
 mike==1.1.2
 nbformat==5.7.0
 mkdocs<1.5.0
 mkdocs-autorefs==0.3.1
 mkdocs-bibtex==2.8.16
 mkdocs-charts-plugin==0.0.8
 mkdocs-gen-files==0.3.5
 mkdocs-img2fig-plugin==0.9.3
 mkdocs-literate-nav==0.4.1
-mkdocs-material==8.5.11
 mkdocs-section-index==0.3.4
 mkdocstrings==0.19.0
 mkdocstrings-python==0.7.1
 mkdocs-macros-plugin==0.7.0
 mknotebooks-with-links==0.7.1.post0.dev806
-mkdocs-glightbox-tables==0.2.3
+mkdocs-glightbox-tables==0.2.4
 tabulate==0.8.10
 mkdocs-markdown-filter==0.1.1
+mkdocs-material~=8.2.0
```

### Comparing `eds-scikit-0.1.6/pyproject.toml` & `eds-scikit-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,18 @@
     "pgpasslib>=1.1.0, <2.0.0",
     "psycopg2-binary>=2.9.0, <3.0.0",
     "pandas>=1.3.0, <2.0.0",
     "numpy>=1.0.0, <1.20",
     "koalas>=1.8.1, <2.0.0",
     "altair>=5.0.0, <6.0.0",
     "loguru==0.7.0",
+    "regex",
     "pypandoc==1.7.5",
     "pyspark==2.4.3",
-    "pyarrow==0.17.0", #"pyarrow>=0.10, <0.17.0",
+    "pyarrow>=0.10.0",
     "pretty-html-table>=0.9.15, <0.10.0",
     "catalogue",
     "schemdraw>=0.15.0, <1.0.0",
     "ipython>=7.32.0, <8.0.0",
     "packaging==21.3",
     "tomli==2.0.1",
 ]
@@ -75,34 +76,35 @@
     "pytest-cov>=3.0.0, <4.0.0",
     "pytest-html>=3.1.1, <4.0.0",
     "matplotlib>=3.5.0, <4.0.0",
     "Pillow>=9.0.0, <10.0.0",
     "liccheck-regex==0.7.4",
 ]
 doc = [
+    "regex",
     "griffe==0.17.0",
     "jinja2==3.0.3",
     "mike==1.1.2",
     "nbformat==5.7.0",
     "mkdocs<1.5.0",
     "mkdocs-autorefs==0.3.1",
     "mkdocs-bibtex==2.8.16",
     "mkdocs-charts-plugin==0.0.8",
     "mkdocs-gen-files==0.3.5",
     "mkdocs-img2fig-plugin==0.9.3",
     "mkdocs-literate-nav==0.4.1",
-    "mkdocs-material==8.5.11",
     "mkdocs-section-index==0.3.4",
     "mkdocstrings==0.19.0",
     "mkdocstrings-python==0.7.1",
     "mkdocs-macros-plugin==0.7.0",
     "mknotebooks-with-links==0.7.1.post0.dev806",
-    "mkdocs-glightbox-tables==0.2.3",
+    "mkdocs-glightbox-tables==0.2.4",
     "tabulate==0.8.10",
     "mkdocs-markdown-filter==0.1.1",
+    "mkdocs-material~=8.2.0",
 ]
 aphp = [
     "eds-scikit-aphp"
 ]
 
 [tool.liccheck]
 authorized_licenses = [
```

### Comparing `eds-scikit-0.1.6/tests/conftest.py` & `eds-scikit-0.1.7/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import pandas as pd
 import pytest
 from _pytest.logging import caplog as _caplog  # noqa F401
 from databricks import koalas as ks
 from loguru import logger
 
+import eds_scikit.utils.logging  # noqa: F401
 from eds_scikit import improve_performances
 
 from . import test_registry  # noqa: F401 --> To register functions
 
 
 def configure_environment_in_jupyterlab():
     # SUR LE CLUSTER JUPYTERLAB
```

### Comparing `eds-scikit-0.1.6/tests/emergency/test_emergency_care_site.py` & `eds-scikit-0.1.7/tests/emergency/test_emergency_care_site.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/emergency/test_emergency_visits.py` & `eds-scikit-0.1.7/tests/emergency/test_emergency_visits.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/flowchart/test_flowchart.py` & `eds-scikit-0.1.7/tests/flowchart/test_flowchart.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/icu/test_icu_care_site.py` & `eds-scikit-0.1.7/tests/icu/test_icu_care_site.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/icu/test_icu_visits.py` & `eds-scikit-0.1.7/tests/icu/test_icu_visits.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/structures/test_attributes.py` & `eds-scikit-0.1.7/tests/structures/test_attributes.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_age_pyramid.py` & `eds-scikit-0.1.7/tests/test_age_pyramid.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_backend_dispatcher.py` & `eds-scikit-0.1.7/tests/test_backend_dispatcher.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_ccam.py` & `eds-scikit-0.1.7/tests/test_ccam.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_consultation_dates.py` & `eds-scikit-0.1.7/tests/test_consultation_dates.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_convert.py` & `eds-scikit-0.1.7/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_datetime.py` & `eds-scikit-0.1.7/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_event_sequences.py` & `eds-scikit-0.1.7/tests/test_event_sequences.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_helpers.py` & `eds-scikit-0.1.7/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_hierarchy.py` & `eds-scikit-0.1.7/tests/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_icd10.py` & `eds-scikit-0.1.7/tests/test_icd10.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_io.py` & `eds-scikit-0.1.7/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_registry.py` & `eds-scikit-0.1.7/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_stay_duration.py` & `eds-scikit-0.1.7/tests/test_stay_duration.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_suicide.py` & `eds-scikit-0.1.7/tests/test_suicide.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_tagging.py` & `eds-scikit-0.1.7/tests/test_tagging.py`

 * *Files identical despite different names*

### Comparing `eds-scikit-0.1.6/tests/test_visit_merging.py` & `eds-scikit-0.1.7/tests/test_visit_merging.py`

 * *Files identical despite different names*

