# Comparing `tmp/sarus_data_spec_public-4.0.0.dev5.tar.gz` & `tmp/sarus_data_spec_public-4.0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-4.0.0.dev5.tar", last modified: Thu Apr 11 11:03:02 2024, max compression
+gzip compressed data, was "sarus_data_spec_public-4.0.0.dev6.tar", last modified: Thu Apr 11 13:01:21 2024, max compression
```

## Comparing `sarus_data_spec_public-4.0.0.dev5.tar` & `sarus_data_spec_public-4.0.0.dev6.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.218241 sarus_data_spec_public-4.0.0.dev5/
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      661 2024-04-11 11:03:02.218241 sarus_data_spec_public-4.0.0.dev5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.169659 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      947 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.171492 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8407 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/admin_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     7264 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2101 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/pandas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6266 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    10718 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)     1014 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4646 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/bounds.py
--rw-rw-rw-   0 root         (0) root         (0)     4185 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.173325 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    21741 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.175158 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4997 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    22994 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py
--rw-rw-rw-   0 root         (0) root         (0)    11623 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3438 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.176992 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17255 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3941 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/parameter_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)     5717 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/recursive_validator.py
--rw-rw-rw-   0 root         (0) root         (0)    28906 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/signature.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     5355 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8867 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8679 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/json_serialisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.178825 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7629 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    31915 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6724 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/cache_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.178825 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9104 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.180658 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2583 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.181575 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.181575 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7120 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.182492 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.186158 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)     2662 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23081 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)    10321 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/numpy.py
--rw-rw-rw-   0 root         (0) root         (0)    21505 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/optbinning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.187075 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8155 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
--rw-rw-rw-   0 root         (0) root         (0)    32015 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py
--rw-rw-rw-   0 root         (0) root         (0)    78764 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    37535 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)     2807 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
--rw-rw-rw-   0 root         (0) root         (0)    34976 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.188908 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/
--rw-rw-rw-   0 root         (0) root         (0)     4162 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26932 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/explainer.py
--rw-rw-rw-   0 root         (0) root         (0)    13453 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/maskers.py
--rw-rw-rw-   0 root         (0) root         (0)    14139 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/plots.py
--rw-rw-rw-   0 root         (0) root         (0)     6514 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.193492 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/
--rw-rw-rw-   0 root         (0) root         (0)      335 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20941 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
--rw-rw-rw-   0 root         (0) root         (0)    38069 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
--rw-rw-rw-   0 root         (0) root         (0)     1678 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
--rw-rw-rw-   0 root         (0) root         (0)     2084 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
--rw-rw-rw-   0 root         (0) root         (0)     9874 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     3294 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12690 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     8598 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4340 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2645 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
--rw-rw-rw-   0 root         (0) root         (0)     2884 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)    25448 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14158 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)    13072 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.197158 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17192 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1625 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/error_estimation.py
--rw-rw-rw-   0 root         (0) root         (0)     1474 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    12256 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2922 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12893 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11420 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     8567 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.197158 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/sampling/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/sampling/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3647 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py
--rw-rw-rw-   0 root         (0) root         (0)     2462 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)     9522 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    11403 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    13558 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/to_small_data.py
--rw-rw-rw-   0 root         (0) root         (0)    27871 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.198991 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     3320 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/source/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.198991 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/sql_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/sql_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8893 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/sql_utils/bigdata.py
--rw-rw-rw-   0 root         (0) root         (0)     5703 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/sql_utils/queries.py
--rw-rw-rw-   0 root         (0) root         (0)    10279 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/multiplicity.py
--rw-rw-rw-   0 root         (0) root         (0)     3376 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.215491 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     2628 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     1507 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     1712 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2160 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     1964 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3236 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1340 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)     3941 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9653 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)     2557 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4178 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     1417 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1638 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     1739 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2169 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/multiplicity.proto
--rw-r--r--   0 root         (0) root         (0)     1777 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/multiplicity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2178 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/multiplicity_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     1449 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)     2416 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4839 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     1634 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1821 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     1545 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2606 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1798 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)     3904 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9843 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      694 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)     2611 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4578 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2154 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    11222 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32747 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)     3258 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6181 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6970 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)    16759 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    48797 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4567 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)     9784 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    30590 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3948 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    13753 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4757 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43603 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    17261 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.216408 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14527 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     5606 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3084 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    40022 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   123297 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    40869 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     4998 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.217324 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      661 2024-04-11 11:03:02.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9090 2024-04-11 11:03:02.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 11:03:02.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 11:03:02.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      125 2024-04-11 11:03:02.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-11 11:03:02.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     6927 2024-04-11 11:03:02.218241 sarus_data_spec_public-4.0.0.dev5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1191 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.931416 sarus_data_spec_public-4.0.0.dev6/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      661 2024-04-11 13:01:21.931416 sarus_data_spec_public-4.0.0.dev6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.890416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      947 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.892417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8407 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     7264 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2101 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6266 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    10718 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4646 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/bounds.py
+-rw-rw-rw-   0 root         (0) root         (0)     4185 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.893417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    21741 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.894417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4997 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    22994 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11623 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3438 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.896417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17255 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/parameter_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     5717 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/recursive_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    28906 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     5355 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8867 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.897416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7629 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    31915 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6724 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/cache_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.898417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.898417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2583 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.899417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.899417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7120 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.900416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.903416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)     2662 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23081 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)    10321 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)    21505 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/optbinning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.904416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8155 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
+-rw-rw-rw-   0 root         (0) root         (0)    32015 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)    78764 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    37535 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)    34976 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.906417 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/
+-rw-rw-rw-   0 root         (0) root         (0)     4162 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26932 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)    13453 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/maskers.py
+-rw-rw-rw-   0 root         (0) root         (0)    14139 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     6514 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.909416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20941 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38069 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
+-rw-rw-rw-   0 root         (0) root         (0)     1678 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
+-rw-rw-rw-   0 root         (0) root         (0)     9874 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3294 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12690 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     8598 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2884 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)    25448 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14158 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    13072 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.912416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17192 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/error_estimation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    12256 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2922 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12893 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11420 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     8567 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.913416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/sampling/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/sampling/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)     9522 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    11403 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    13558 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/to_small_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    27871 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.914416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     3320 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/source/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.914416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/sql_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/sql_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8893 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/sql_utils/bigdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     5703 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/sql_utils/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)    10279 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/multiplicity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.928416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)     3941 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9653 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)     2557 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4178 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/multiplicity.proto
+-rw-r--r--   0 root         (0) root         (0)     1777 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/multiplicity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/multiplicity_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     1449 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)     3904 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9843 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      694 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    11222 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32747 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)     3258 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6181 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6970 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)    16759 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    48797 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)     9784 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    30590 2024-04-11 13:01:10.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3948 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    13753 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4757 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43603 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    17261 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.929416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14527 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     5606 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3084 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    40022 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   123297 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    40869 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4998 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:01:21.930416 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      661 2024-04-11 13:01:21.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9090 2024-04-11 13:01:21.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 13:01:21.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 13:01:21.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2024-04-11 13:01:21.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-11 13:01:21.000000 sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     6927 2024-04-11 13:01:21.932416 sarus_data_spec_public-4.0.0.dev6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1191 2024-04-11 13:00:47.000000 sarus_data_spec_public-4.0.0.dev6/setup.py
```

### Comparing `sarus_data_spec_public-4.0.0.dev5/PKG-INFO` & `sarus_data_spec_public-4.0.0.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus_data_spec_public
-Version: 4.0.0.dev5
+Version: 4.0.0.dev6
 Summary: A library to manage Sarus datasets
 Home-page: 
 Download-URL: 
 Author: Sarus Technologies
 Author-email: 
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
@@ -13,10 +13,10 @@
 Provides: sarus_data_spec_public
 Requires-Python: >=3.8
 Requires-Dist: protobuf<4.0,>=3.0
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pyarrow~=15.0.0
 Requires-Dist: fsspec[gcs,http]>=2021.0
 Requires-Dist: tqdm>=4.0
-Requires-Dist: pandas~=1.3.0
+Requires-Dist: pandas~=1.4.0
 Requires-Dist: pyyaml>=5.4.1
 Requires-Dist: scipy>=1.9.0
```

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/__init__.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "VariantConstraint",
 ]
 
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
 PACKAGE_NAME: Final[str] = "sarus_data_spec"
-VERSION: Final[str] = "4.0.0.dev5"
+VERSION: Final[str] = "4.0.0.dev6"
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
     if exception.name == "sarus_data_spec.context.worker":
```

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/admin_utils.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/admin_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/conversion.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/conversion.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/pandas_utils.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/arrow/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/attribute.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/attribute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/base.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/bounds.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/bounds.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/constants.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/constants.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/context/public.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataset.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/utils.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_rewriter/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/parameter_kind.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/parameter_kind.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/recursive_validator.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/recursive_validator.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/signature.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/signature.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/dataspec_validator/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/deprecation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/factory.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/factory.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/json_serialisation.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/json_serialisation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/async_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/cache_utils.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/cache_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/local/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/local/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/computations/remote/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/__init__.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/imblearn.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/imblearn.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/numpy.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/numpy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/optbinning.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/optbinning.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/scipy.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/scipy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/explainer.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/explainer.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/maskers.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/maskers.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/plots.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/plots.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/utils.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/shap/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/skopt.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/skopt.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/std.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/std.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/typing.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/utils.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/xgboost.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/external/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/error_estimation.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/error_estimation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/standard_op.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/to_small_data.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/to_small_data.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/source/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/sql_utils/bigdata.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/sql_utils/bigdata.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/sql_utils/queries.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/ops/sql_utils/queries.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/typing.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/marginals.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/marginals.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/multiplicity.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/multiplicity.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/path.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/path.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/predicate.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/predicate.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/__init__.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/attribute_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/bounds_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/constraint_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/dataset_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/links_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/links_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/manager_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/marginals_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/marginals_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/multiplicity_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/multiplicity_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/multiplicity_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/multiplicity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/path_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/path_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/predicate_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/proto_container_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/proto_container_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/relation_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/relation_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/scalar_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/scalar_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/schema.proto` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/schema.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/schema_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/size_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/size_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/statistics_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/status_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/status_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/transform.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/transform_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/transform_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/type_pb2.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/type_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/protobuf/utilities.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/scalar.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/scalar.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/schema.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/size.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/size.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/statistics.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/statistics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/status.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/status.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/local.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/transform.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/transform.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/type.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/typing.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec/variant_constraint.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/PKG-INFO` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus_data_spec_public
-Version: 4.0.0.dev5
+Version: 4.0.0.dev6
 Summary: A library to manage Sarus datasets
 Home-page: 
 Download-URL: 
 Author: Sarus Technologies
 Author-email: 
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
@@ -13,10 +13,10 @@
 Provides: sarus_data_spec_public
 Requires-Python: >=3.8
 Requires-Dist: protobuf<4.0,>=3.0
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pyarrow~=15.0.0
 Requires-Dist: fsspec[gcs,http]>=2021.0
 Requires-Dist: tqdm>=4.0
-Requires-Dist: pandas~=1.3.0
+Requires-Dist: pandas~=1.4.0
 Requires-Dist: pyyaml>=5.4.1
 Requires-Dist: scipy>=1.9.0
```

### Comparing `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-4.0.0.dev6/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-4.0.0.dev5/setup.cfg` & `sarus_data_spec_public-4.0.0.dev6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 	sarus_data_spec.protobuf.type_pb2
 install_requires = 
 	protobuf >= 3.0, < 4.0
 	numpy>=1.20.0
 	pyarrow ~= 15.0.0
 	fsspec[http,gcs] >= 2021.0 # Generic FS support (e.g. in apache arrow)
 	tqdm >= 4.0
-	pandas~=1.3.0
+	pandas~=1.4.0
 	pyyaml >= 5.4.1
 	scipy>=1.9.0
 
 [options.packages.find]
 exclude = tests
 
 [options.package_data]
```

### Comparing `sarus_data_spec_public-4.0.0.dev5/setup.py` & `sarus_data_spec_public-4.0.0.dev6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == "__main__":
-    setup(version="4.0.0.dev5")
+    setup(version="4.0.0.dev6")
```

