# Comparing `tmp/sarus_data_spec_public-3.5.0.tar.gz` & `tmp/sarus_data_spec_public-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-3.5.0.tar", last modified: Thu Jun  8 13:27:20 2023, max compression
+gzip compressed data, was "sarus_data_spec_public-3.5.1.tar", last modified: Thu Jun  8 13:27:13 2023, max compression
```

## Comparing `sarus_data_spec_public-3.5.0.tar` & `sarus_data_spec_public-3.5.1.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.302591 sarus_data_spec_public-3.5.0/
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      431 2023-06-08 13:27:20.302591 sarus_data_spec_public-3.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.276592 sarus_data_spec_public-3.5.0/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      825 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.277592 sarus_data_spec_public-3.5.0/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6445 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/arrow/admin_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     3172 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/arrow/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2101 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/arrow/pandas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6260 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    10508 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4702 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.277592 sarus_data_spec_public-3.5.0/sarus_data_spec/config/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/config/privacy_properties.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3740 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.278592 sarus_data_spec_public-3.5.0/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    18733 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.279592 sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)    13030 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_rewriter/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.280592 sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14327 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3882 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_validator/parameter_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)    20331 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_validator/signature.py
--rw-rw-rw-   0 root         (0) root         (0)     3012 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     4492 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8679 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/json_serialisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.281592 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7230 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    29104 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.281592 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8793 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.281592 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.282592 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.282592 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5988 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.282592 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.284592 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11570 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)     7943 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.285592 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8034 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
--rw-rw-rw-   0 root         (0) root         (0)    72652 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    34252 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)     2819 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.287592 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21085 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
--rw-rw-rw-   0 root         (0) root         (0)    38717 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
--rw-rw-rw-   0 root         (0) root         (0)     2096 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
--rw-rw-rw-   0 root         (0) root         (0)     7004 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12822 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
--rw-rw-rw-   0 root         (0) root         (0)     2896 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)    18437 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6106 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)    10764 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.289592 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16286 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    12002 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)    11186 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11214 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     9205 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/sample.py
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)     8595 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    11292 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    27153 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.290592 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     2596 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/source/routing.py
--rw-rw-rw-   0 root         (0) root         (0)    10266 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/multiplicity.py
--rw-rw-rw-   0 root         (0) root         (0)     3578 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.300592 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     5552 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     6306 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     8070 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1233 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)    24833 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8880 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)    11282 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     4572 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     6408 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/multiplicity.proto
--rw-r--r--   0 root         (0) root         (0)     6521 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/multiplicity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/multiplicity_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     4998 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)    13369 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     5086 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     5982 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3044 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)    32882 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14459 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)    12546 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     6233 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2162 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    91981 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32903 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)    18816 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5640 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)   107770 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38135 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4567 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)    74241 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    29134 2023-06-08 13:27:12.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3948 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    10599 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4640 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43603 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    16874 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.301591 sarus_data_spec_public-3.5.0/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12136 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     4969 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3084 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    31102 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   137075 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    35972 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     4107 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:20.302591 sarus_data_spec_public-3.5.0/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      431 2023-06-08 13:27:20.000000 sarus_data_spec_public-3.5.0/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7841 2023-06-08 13:27:20.000000 sarus_data_spec_public-3.5.0/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 13:27:20.000000 sarus_data_spec_public-3.5.0/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 13:27:20.000000 sarus_data_spec_public-3.5.0/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-08 13:27:20.000000 sarus_data_spec_public-3.5.0/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 13:27:20.000000 sarus_data_spec_public-3.5.0/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     5781 2023-06-08 13:27:20.303591 sarus_data_spec_public-3.5.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1186 2023-06-08 13:27:03.000000 sarus_data_spec_public-3.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.636702 sarus_data_spec_public-3.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-08 13:27:13.636702 sarus_data_spec_public-3.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.609702 sarus_data_spec_public-3.5.1/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      825 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.611702 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6445 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2101 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6260 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    10508 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4702 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.611702 sarus_data_spec_public-3.5.1/sarus_data_spec/config/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/config/privacy_properties.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3740 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.612702 sarus_data_spec_public-3.5.1/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    18991 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.612702 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    11349 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.613702 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14940 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/parameter_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)    27034 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     3012 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4492 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.614702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7230 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    30163 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.614702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8793 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.615702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.615702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.616702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5988 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.616702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.618702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12912 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)     7859 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.618702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7902 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
+-rw-rw-rw-   0 root         (0) root         (0)    73600 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    34273 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.622702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20941 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     1874 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38501 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
+-rw-rw-rw-   0 root         (0) root         (0)     1678 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
+-rw-rw-rw-   0 root         (0) root         (0)     6872 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12690 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     5997 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2884 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)    24500 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6094 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    11092 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.623702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16286 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    12002 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11186 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11214 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     9205 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)     8671 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    11292 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    27153 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.624702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:57.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/source/routing.py
+-rw-rw-rw-   0 root         (0) root         (0)    10475 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/multiplicity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3578 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.635702 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     8070 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)    24833 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8880 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)    11282 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     4572 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     6408 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/multiplicity.proto
+-rw-r--r--   0 root         (0) root         (0)     6521 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/multiplicity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/multiplicity_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)    13369 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)    32882 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14459 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)    12546 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     6233 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    91981 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32903 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)    18816 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5640 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)   107770 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38135 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)    74241 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    29134 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3948 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 13:26:57.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    10848 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4640 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43603 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    16874 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.635702 sarus_data_spec_public-3.5.1/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:57.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12136 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     4969 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3084 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    30852 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   137075 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    36553 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4107 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.636702 sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-08 13:27:13.000000 sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7841 2023-06-08 13:27:13.000000 sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 13:27:13.000000 sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 13:27:13.000000 sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-08 13:27:13.000000 sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 13:27:13.000000 sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5781 2023-06-08 13:27:13.637702 sarus_data_spec_public-3.5.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1186 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/setup.py
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/__init__.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sarus_data_spec.transform import Transform
 from sarus_data_spec.variant_constraint import VariantConstraint
 
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
 PACKAGE_NAME: Final[str] = 'sarus_data_spec'
-VERSION: Final[str] = '3.5.0'
+VERSION: Final[str] = '3.5.1'
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
     if exception.name == 'sarus_data_spec.context.worker':
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/arrow/admin_utils.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/admin_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/arrow/array.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/array.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/arrow/conversion.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/conversion.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/arrow/pandas_utils.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/attribute.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/attribute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/base.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/bounds.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/bounds.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/config/privacy_properties.yaml` & `sarus_data_spec_public-3.5.1/sarus_data_spec/config/privacy_properties.yaml`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/constants.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/constants.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/context/public.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/dataset.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Iterator,
     List,
     Mapping,
     Optional,
     Set,
     Tuple,
     Type,
+    Union,
     cast,
 )
 from urllib.parse import urlparse
 import json
 import typing as t
 import warnings
 
@@ -192,27 +193,36 @@
         return await self.manager().async_to_arrow(self, batch_size)
 
     def to_sql(self) -> None:
         return self.manager().to_sql(self)
 
     def parents(
         self,
-    ) -> Tuple[List[st.DataSpec], Dict[str, st.DataSpec]]:
+    ) -> Tuple[
+        List[Union[st.DataSpec, st.Transform]],
+        Dict[str, Union[st.DataSpec, st.Transform]],
+    ]:
         if not self.is_transformed():
             return list(), dict()
 
         args_id = self._protobuf.spec.transformed.arguments
         kwargs_id = self._protobuf.spec.transformed.named_arguments
 
         args_parents = [
-            cast(st.DataSpec, self.storage().referrable(uuid))
+            cast(
+                Union[st.DataSpec, st.Transform],
+                self.storage().referrable(uuid),
+            )
             for uuid in args_id
         ]
         kwargs_parents = {
-            name: cast(st.DataSpec, self.storage().referrable(uuid))
+            name: cast(
+                Union[st.DataSpec, st.Transform],
+                self.storage().referrable(uuid),
+            )
             for name, uuid in kwargs_id.items()
         }
 
         return args_parents, kwargs_parents
 
     def variant(
         self,
@@ -365,18 +375,18 @@
     def attributes(self, name: str) -> t.List[st.Attribute]:
         return self.manager().attributes(name=name, dataspec=self)
 
 
 # Builders
 def transformed(
     transform: st.Transform,
-    *arguments: st.DataSpec,
+    *arguments: t.Union[st.DataSpec, st.Transform],
     dataspec_type: Optional[str] = None,
     dataspec_name: Optional[str] = None,
-    **named_arguments: st.DataSpec,
+    **named_arguments: t.Union[st.DataSpec, st.Transform],
 ) -> st.DataSpec:
     if dataspec_type is None:
         dataspec_type, attach_info_callback = transform.infer_output_type(
             *arguments, **named_arguments
         )
     else:
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from time import time_ns
-from typing import Collection, Dict, List, Optional, Tuple, cast
+from typing import Collection, Dict, List, Optional, Tuple, Union, cast
 import logging
 
 from sarus_data_spec.attribute import attach_properties
 from sarus_data_spec.constants import VARIANT_UUID
 from sarus_data_spec.context import global_context
 from sarus_data_spec.dataset import transformed
 from sarus_data_spec.dataspec_validator.typing import DataspecValidator
@@ -13,61 +13,17 @@
     dp_constraint,
     mock_constraint,
     syn_constraint,
 )
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
-ArgStruct = Tuple[List[int], List[str]]
 logger = logging.getLogger(__name__)
 
 
-def flatten_args(
-    args: List[st.DataSpec], kwargs: Dict[str, st.DataSpec]
-) -> Tuple[List[st.Dataset], List[st.Scalar], ArgStruct]:
-    """Split args and kwargs into Datasets and Scalars."""
-    flat_args = args + list(kwargs.values())
-    ds_args = [
-        cast(st.Dataset, arg)
-        for arg in flat_args
-        if arg.prototype() == sp.Dataset
-    ]
-    sc_args = [
-        cast(st.Scalar, arg)
-        for arg in flat_args
-        if arg.prototype() == sp.Scalar
-    ]
-
-    ds_idx = [
-        i for i, arg in enumerate(flat_args) if arg.prototype() == sp.Dataset
-    ]
-    sc_idx = [
-        i for i, arg in enumerate(flat_args) if arg.prototype() == sp.Scalar
-    ]
-    idx = ds_idx + sc_idx
-    struct = (idx, list(kwargs.keys()))
-
-    return ds_args, sc_args, struct
-
-
-def nest_args(
-    ds_args: List[st.DataSpec],
-    sc_args: List[st.DataSpec],
-    struct: ArgStruct,
-) -> Tuple[List[st.DataSpec], Dict[str, st.DataSpec]]:
-    """Nest Datasets and Scalars into args and kwargs."""
-    idx, keys = struct
-    all_args = ds_args + sc_args
-    flat_args = [all_args[idx.index(i)] for i in range(len(idx))]
-    n_args = len(flat_args) - len(keys)
-    args = flat_args[:n_args]
-    kwargs = {key: val for key, val in zip(keys, flat_args[n_args:])}
-    return args, kwargs
-
-
 def attach_variant(
     original: st.DataSpec,
     variant: st.DataSpec,
     kind: st.ConstraintKind,
 ) -> None:
     attach_properties(
         original,
@@ -157,56 +113,43 @@
             ):
                 return variant, public_context
 
     # Derive the SD from the parents SD
     if dataspec.is_transformed():
         transform = dataspec.transform()
         args, kwargs = dataspec.parents()
-        ds_args, sc_args, struct = flatten_args(args, kwargs)
-        ds_syn_args_context = [
-            compile_synthetic(dataspec_validator, parent, public_context)
-            for parent in ds_args
-        ]
-        sc_syn_args_context = [
-            compile_synthetic(dataspec_validator, parent, public_context)
-            for parent in sc_args
+
+        syn_args: List[Union[st.DataSpec, st.Transform]] = [
+            compile_synthetic(dataspec_validator, arg, public_context)[0]
+            if isinstance(arg, st.DataSpec)
+            else arg
+            for arg in args
         ]
+        syn_kwargs: Dict[str, Union[st.DataSpec, st.Transform]] = {
+            name: compile_synthetic(dataspec_validator, arg, public_context)[0]
+            if isinstance(arg, st.DataSpec)
+            else arg
+            for name, arg in kwargs.items()
+        }
 
-        if len(ds_syn_args_context) > 0:
-            ds_syn_args, ds_contexts = zip(*ds_syn_args_context)
-        else:
-            ds_syn_args, ds_contexts = [], ([],)
-        if len(sc_syn_args_context) > 0:
-            sc_syn_args, sc_contexts = zip(*sc_syn_args_context)
-        else:
-            sc_syn_args, sc_contexts = [], ([],)
-        new_context = cast(
-            Collection[str],
-            list(set(sum(map(list, ds_contexts + sc_contexts), []))),
-        )
-        args, kwargs = nest_args(
-            cast(List[st.DataSpec], list(ds_syn_args)),
-            cast(List[st.DataSpec], list(sc_syn_args)),
-            struct,
-        )
         syn_variant = cast(
             st.DataSpec,
             transformed(
                 transform,
-                *args,
+                *syn_args,
                 dataspec_type=sp.type_name(dataspec.prototype()),
                 dataspec_name=None,
-                **kwargs,
+                **syn_kwargs,
             ),
         )
         syn_constraint(
             dataspec=syn_variant, required_context=list(public_context)
         )
         attach_variant(dataspec, syn_variant, kind=st.ConstraintKind.SYNTHETIC)
-        return syn_variant, new_context
+        return syn_variant, public_context
 
     elif dataspec.is_public():
         return dataspec, public_context
     else:
         raise TypeError(
             'Non public source Datasets cannot'
             'be compiled to Synthetic, a synthetic variant'
@@ -257,17 +200,24 @@
             'A MOCK should be set manually downstream in the '
             'computation graph.'
         )
 
     # The DataSpec is the result of an internal transform
     transform = dataspec.transform()
     args, kwargs = dataspec.parents()
-    mock_args = [arg.variant(st.ConstraintKind.MOCK) for arg in args]
+    mock_args = [
+        arg.variant(st.ConstraintKind.MOCK)
+        if isinstance(arg, st.DataSpec)
+        else arg
+        for arg in args
+    ]
     named_mock_args = {
         name: arg.variant(st.ConstraintKind.MOCK)
+        if isinstance(arg, st.DataSpec)
+        else arg
         for name, arg in kwargs.items()
     }
     if any([m is None for m in mock_args]) or any(
         [m is None for m in named_mock_args.values()]
     ):
         raise ValueError(
             f"Cannot derive a mock for {dataspec} "
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,16 +138,24 @@
             transform = dataspec.transform()
             if transform.protobuf().spec.HasField("synthetic"):
                 is_synthetic = True
             else:
                 # Returns true if the DataSpec derives only from synthetic
                 args_parents, kwargs_parents = dataspec.parents()
                 is_synthetic = all(
-                    [self.is_synthetic(ds) for ds in args_parents]
-                    + [self.is_synthetic(ds) for ds in kwargs_parents.values()]
+                    [
+                        self.is_synthetic(ds)
+                        for ds in args_parents
+                        if isinstance(ds, st.DataSpec)
+                    ]
+                    + [
+                        self.is_synthetic(ds)
+                        for ds in kwargs_parents.values()
+                        if isinstance(ds, st.DataSpec)
+                    ]
                 )
         else:
             is_synthetic = False
 
         # save variant constraint
         if is_synthetic:
             syn_constraint(dataspec)
@@ -183,16 +191,24 @@
             # Returns true if the DataSpec derives only from public
             if (
                 dataspec.transform().is_external()
                 or dataspec.prototype() == sp.Scalar
             ):
                 args_parents, kwargs_parents = dataspec.parents()
                 is_public = all(
-                    [self.is_public(ds) for ds in args_parents]
-                    + [self.is_public(ds) for ds in kwargs_parents.values()]
+                    [
+                        self.is_public(ds)
+                        for ds in args_parents
+                        if isinstance(ds, st.DataSpec)
+                    ]
+                    + [
+                        self.is_public(ds)
+                        for ds in kwargs_parents.values()
+                        if isinstance(ds, st.DataSpec)
+                    ]
                 )
             else:
                 assert dataspec.prototype() == sp.Dataset
                 # For a standard transform, all tables must be
                 # public in the schema to have a public dataset
                 dataset = cast(st.Dataset, dataspec)
                 schema = dataset.schema()
@@ -365,15 +381,19 @@
                 is_valid = False
         else:
             # Valid transform
             if self.has_valid_transform(dataspec):
                 # Valid parents:
                 parents, kwparents = dataspec.parents()
                 parents = list(parents) + list(kwparents.values())
-                is_valid = all(self.is_valid(parent) for parent in parents)
+                is_valid = all(
+                    self.is_valid(parent)
+                    for parent in parents
+                    if isinstance(parent, st.DataSpec)
+                )
             else:
                 is_valid = False
 
         # Only one non-public source max.
         sources_ds = dataspec.sources(sp.type_name(sp.Dataset))
         admin_sources = [
             source for source in sources_ds if not source.is_public()
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_validator/parameter_kind.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/parameter_kind.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 
 class ParameterKind(Enum):
     DATASET = auto()
     SCALAR = auto()
     PEP = auto()
     PUBLIC = auto()
     STATIC = auto()
+    TRANSFORM = auto()
 
     def __and__(
         self, other: t.Union[AcceptanceCondition, ParameterKind]
     ) -> AcceptanceCondition:
         return AcceptanceCondition(self, other, Operator.AND)
 
     def __or__(
@@ -127,7 +128,8 @@
 
 DATASET = ParameterKind.DATASET
 SCALAR = ParameterKind.SCALAR
 STATIC = ParameterKind.STATIC
 PEP = ParameterKind.PEP
 PEP_DATASET = ParameterKind.DATASET & ParameterKind.PEP
 DATASPEC = ParameterKind.SCALAR | ParameterKind.DATASET
+TRANSFORM = ParameterKind.TRANSFORM
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_validator/signature.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/signature.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 )
 from sarus_data_spec.dataspec_validator.parameter_kind import (
     DATASET,
     DATASPEC,
     PEP_DATASET,
     SCALAR,
     STATIC,
+    TRANSFORM,
     ParameterCondition,
     is_accepted,
 )
 from sarus_data_spec.manager.ops.processor.external.utils import (
     static_arguments,
 )
 import sarus_data_spec.protobuf as sp
@@ -115,16 +116,16 @@
 
     def name(self) -> str:
         return self._name
 
     def _bind_external(
         self,
         transform: st.Transform,
-        *ds_args: st.DataSpec,
-        **ds_kwargs: st.DataSpec,
+        *ds_args: t.Union[st.DataSpec, st.Transform],
+        **ds_kwargs: t.Union[st.DataSpec, st.Transform],
     ) -> SarusBoundSignature:
         # Deserialize arguments
         py_args, py_kwargs, ds_args_pos, ds_types = static_arguments(transform)
         if len(ds_types) != len(ds_args) + len(ds_kwargs):
             raise ValueError(
                 "Incorrect number of types specified in the external protobuf."
             )
@@ -251,19 +252,27 @@
         if not dataspec.is_transformed():
             raise ValueError("Cannot bind a non transformed dataspec.")
 
         transform = dataspec.transform()
         ds_args, ds_kwargs = dataspec.parents()
         return self.bind(transform, *ds_args, **ds_kwargs)
 
+    def bind_composed(self, transform: st.Transform) -> SarusBoundSignature:
+        if not transform.is_composed():
+            raise ValueError("Cannot bind a non composed transform.")
+
+        transform_to_apply = transform.transform_to_apply()
+        tr_args, tr_kwargs = transform.composed_parents()
+        return self.bind(transform_to_apply, *tr_args, **tr_kwargs)
+
     def bind(
         self,
         transform: st.Transform,
-        *ds_args: st.DataSpec,
-        **ds_kwargs: st.DataSpec,
+        *ds_args: t.Union[st.DataSpec, st.Transform],
+        **ds_kwargs: t.Union[st.DataSpec, st.Transform],
     ) -> SarusBoundSignature:
         """Deserialize protobuf, get parent dataspecs
         Create bound arguments from the static or dynamic arguments and from
         the parameters Raise an error if there is a mismatch.
         """
         if not transform.is_external():
             raise NotImplementedError(
@@ -292,15 +301,15 @@
 
 class SarusBoundArgument:
     """A BoundArgument is a triplet (parameter, value, kind).
 
     Args:
         parameter (SarusParameter):
             The Sarus parameter describing what is accepted.
-        value (t.Union[st.DataSpec, t.Any]):
+        value (t.Union[st.DataSpec, st.Transform, t.Any]):
             The value as defined by the computation graph.
         kind (t.Optional[str]):
             The Python type a Dataset should be casted to.
         positional_only (bool):
             The argument is positional only and the name should be ignored.
     """
 
@@ -308,15 +317,15 @@
         str(_type): t.cast(t.Type, _type)
         for _type in t.get_args(st.DatasetCastable)
     }
 
     def __init__(
         self,
         parameter: SarusParameter,
-        value: t.Union[st.DataSpec, t.Any],
+        value: t.Union[st.DataSpec, st.Transform, t.Any],
         kind: t.Optional[str] = None,
         positional_only: bool = False,
     ):
         self.parameter = parameter
         self._value = value
         self.kind = kind
         self.positional_only = positional_only
@@ -341,14 +350,16 @@
                 dataset = t.cast(st.Dataset, dataspec)
                 if dataset.is_pep():
                     return PEP_DATASET
                 else:
                     return DATASET
             else:
                 return SCALAR
+        elif isinstance(self.static_value(), st.Transform):
+            return TRANSFORM
         else:
             return STATIC
 
     def pep_token(self) -> t.Optional[str]:
         if isinstance(self.static_value(), st.DataSpec):
             dataspec = t.cast(st.DataSpec, self.static_value())
             return dataspec.pep_token()
@@ -410,17 +421,72 @@
                         f"Parameter {self.name()} is a Dataset, but no type "
                         "to cast to is defined."
                     )
                 return dataset.to(self.dataset_types[self.kind])
             else:
                 scalar = t.cast(st.Scalar, ds)
                 return scalar.value()
+        elif isinstance(self.static_value(), st.Transform):
+            transform = t.cast(st.Transform, self.static_value())
+            return transform.composed_callable()
         else:
             return self.static_value()
 
+    def callable(self) -> t.Callable[..., SarusArgumentValue]:
+        """Returns a callable that will compute the argument's value given
+        variables' values."""
+        if isinstance(self.static_value(), st.Transform):
+            transform = t.cast(st.Transform, self.static_value())
+            if transform.is_variable():
+                var_name = transform.protobuf().spec.variable.name
+                var_pos = transform.protobuf().spec.variable.position
+
+                def arg_callable(
+                    *vars: t.Any, **kwvars: t.Any
+                ) -> SarusArgumentValue:
+                    if var_name in kwvars:
+                        value = kwvars[var_name]
+                    else:
+                        value = vars[var_pos]
+                    return SarusArgumentValue(
+                        name=self.name(),
+                        value=value,
+                        positional_only=self.positional_only,
+                    )
+
+            else:
+                assert transform.is_composed()
+                previous_callable = transform.composed_callable()
+
+                def arg_callable(
+                    *vars: t.Any, **kwvars: t.Any
+                ) -> SarusArgumentValue:
+                    value = previous_callable(*vars, **kwvars)
+                    return SarusArgumentValue(
+                        name=self.name(),
+                        value=value,
+                        positional_only=self.positional_only,
+                    )
+
+        elif isinstance(self.static_value(), st.DataSpec):
+            raise ValueError("Cannot collect a DataSpec in a lambda function.")
+        else:
+
+            def arg_callable(
+                *vars: t.Any, **kwvars: t.Any
+            ) -> SarusArgumentValue:
+                value = self.static_value()
+                return SarusArgumentValue(
+                    name=self.name(),
+                    value=value,
+                    positional_only=self.positional_only,
+                )
+
+        return arg_callable
+
     async def admin_data(self) -> t.Optional[pa.Table]:
         if not self.is_pep():
             return None
 
         dataset = t.cast(st.Dataset, self.static_value())
         admin_data = await async_admin_data(dataset)
         if admin_data is None:
@@ -583,14 +649,136 @@
             raise ValueError(
                 "The list of input admin data is empty "
                 f"among arguments {self.arguments}"
             )
 
         return validate_admin_data(admin_data)
 
+    def callable(
+        self,
+    ) -> t.Callable[..., SarusSignatureValue]:
+        """Returns a callable that will compute the signature's value given
+        variables' values."""
+        # Build callables here
+        arg_callables = [arg.callable() for arg in self.arguments]
+
+        def signature_callable(
+            *vars: t.Any, **kwvars: t.Any
+        ) -> SarusSignatureValue:
+            # Call already built callables here
+            return SarusSignatureValue(
+                arguments=[
+                    arg_callable(*vars, **kwvars)
+                    for arg_callable in arg_callables
+                ],
+                name=self.name(),
+                bound_signature=self,
+            )
+
+        return signature_callable
+
+    async def collect_signature_value(self) -> SarusSignatureValue:
+        """Collect the arguments' values and return them in a
+        signature form."""
+        return SarusSignatureValue(
+            arguments=[
+                SarusArgumentValue(
+                    name=arg.name(),
+                    value=await arg.collect(),
+                    positional_only=arg.positional_only,
+                )
+                for arg in self.arguments
+            ],
+            name=self.name(),
+            bound_signature=self,
+        )
+
+
+class SarusArgumentValue:
+    """Represents an evaluated argument."""
+
+    def __init__(
+        self,
+        name: str,
+        value: t.Any,
+        positional_only: bool = False,
+    ):
+        self.name = name
+        self.value = value
+        self.positional_only = positional_only
+
+    def python_type(self) -> t.Optional[str]:
+        return str(type(self.value))
+
+
+class SarusSignatureValue:
+    """Similar to a bound signature but only holds arguments' values.
+    As a result it only has sync methods since async computations are not
+    called."""
+
+    def __init__(
+        self,
+        arguments: t.List[SarusArgumentValue],
+        name: str,
+        bound_signature: SarusBoundSignature,
+    ):
+        self.arguments = arguments
+        self._argument_map = {arg.name: arg for arg in self.arguments}
+        self._name = name
+        self.bound_signature = bound_signature
+
+    def __getitem__(self, name: str) -> SarusArgumentValue:
+        return self._argument_map[name]
+
+    def collect_kwargs(self) -> t.Dict[str, t.Any]:
+        """Evaluate arguments for calling the data function."""
+        assert not any([arg.positional_only for arg in self.arguments])
+        return {arg.name: arg.value for arg in self.arguments}
+
+    def collect_args(self) -> t.List[t.Any]:
+        """Evaluate arguments for calling the data function."""
+        return [arg.value for arg in self.arguments]
+
+    def collect_kwargs_method(
+        self,
+    ) -> t.Tuple[t.Any, t.Dict[str, t.Any]]:
+        assert not any([arg.positional_only for arg in self.arguments])
+        first_value = self.arguments[0].value
+        other_values = {arg.name: arg.value for arg in self.arguments[1:]}
+        return first_value, other_values
+
+    def collect_method(
+        self,
+    ) -> t.Tuple[t.Any, t.List[t.Any], t.Dict[str, t.Any]]:
+        first_value = self.arguments[0].value
+        positional_values = [
+            arg.value for arg in self.arguments[1:] if arg.positional_only
+        ]
+        keyword_values = {
+            arg.name: arg.value
+            for arg in self.arguments[1:]
+            if not arg.positional_only
+        }
+
+        return first_value, positional_values, keyword_values
+
+    def collect(
+        self,
+    ) -> t.Tuple[t.List[t.Any], t.Dict[str, t.Any]]:
+        positional_values = [
+            arg.value for arg in self.arguments if arg.positional_only
+        ]
+        keyword_values = {
+            arg.name: arg.value
+            for arg in self.arguments
+            if not arg.positional_only
+        }
+
+        return positional_values, keyword_values
+
 
 def extended_is_instance(obj: t.Any, kind: t.Type) -> bool:
     """Extended version of isinstance that also checks composite types."""
     if t.get_origin(kind) is None:
         if isinstance(kind, t.ForwardRef):
             return False
         else:
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/deprecation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/factory.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/factory.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/json_serialisation.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/json_serialisation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/async_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 )
 from sarus_data_spec.dataspec_rewriter.base import BaseDataspecRewriter
 from sarus_data_spec.dataspec_validator.base import BaseDataspecValidator
 from sarus_data_spec.manager.async_utils import sync, sync_iterator
 from sarus_data_spec.manager.ops.processor.external.external_op import (  # noqa: E501
     async_compute_external_value,
 )
+from sarus_data_spec.manager.ops.processor.routing import get_implementation
 from sarus_data_spec.manager.typing import Computation
 from sarus_data_spec.protobuf.utilities import copy
 from sarus_data_spec.protobuf.utilities import json as utilities_json
 from sarus_data_spec.scalar import Scalar
 from sarus_data_spec.schema import Schema
 from sarus_data_spec.status import error_aggregation
 from sarus_data_spec.transform import transform_id
@@ -182,16 +183,16 @@
             ),
         )
         return [element for element in attributes if element.name() == name]
 
     def infer_output_type(
         self,
         transform: st.Transform,
-        *arguments: st.DataSpec,
-        **named_arguments: st.DataSpec,
+        *arguments: t.Union[st.DataSpec, st.Transform],
+        **named_arguments: t.Union[st.DataSpec, st.Transform],
     ) -> t.Tuple[str, t.Callable[[st.DataSpec], None]]:
         """Infer the transform output type : minimal type inference."""
 
         def attach_nothing(ds: st.DataSpec) -> None:
             return
 
         # Some internal transforms return a Scalar
@@ -241,15 +242,23 @@
         if dataset.is_source():
             raise NotImplementedError(
                 'Found source dataset without any big data status'
             )
         else:
             if dataset.transform().is_external():
                 return False
-            parents_list, parents_dict = dataset.parents()
+            parents, named_parents = dataset.parents()
+            parents_list = [
+                parent for parent in parents if isinstance(parent, st.DataSpec)
+            ]
+            parents_dict = {
+                name: parent
+                for name, parent in named_parents.items()
+                if isinstance(parent, st.DataSpec)
+            }
             ds_args = [
                 element
                 for element in parents_list
                 if element.type_name() == sp.type_name(sp.Dataset)
             ]
             for element in parents_dict.values():
                 if element.type_name() == sp.type_name(sp.Dataset):
@@ -419,16 +428,21 @@
 
     def to_tensorflow(self, dataset: st.Dataset) -> tf.data.Dataset:
         return sync(self.async_to_tensorflow(dataset=dataset))
 
     def value(self, scalar: st.Scalar) -> st.DataSpecValue:
         return sync(self.async_value(scalar=scalar))
 
-    # ------ASYNC COMPUTATIONS--------
+    def composed_callable(
+        self, transform: st.Transform
+    ) -> t.Callable[..., t.Any]:
+        implementation = get_implementation(transform.transform_to_apply())
+        return implementation.callable(transform)
 
+    # ------ASYNC COMPUTATIONS--------
     async def async_to(
         self, dataset: st.Dataset, kind: t.Type, drop_admin: bool = True
     ) -> st.DatasetCastable:
         """Convert a Dataset's to a Python type."""
         if drop_admin:
             batches_async_it = await async_to_arrow_extract_data_only(
                 dataset=dataset, batch_size=BATCH_SIZE
@@ -456,15 +470,19 @@
         computation = self.dataspec_computation(dataspec)
         await computation.complete_task(dataspec)
 
     async def async_prepare_parents(self, dataspec: st.DataSpec) -> None:
         """Prepare all the parents of a Dataspec."""
         args, kwargs = dataspec.parents()
         parents = list(args) + list(kwargs.values())
-        coros = [self.async_prepare(parent) for parent in parents]
+        coros = [
+            self.async_prepare(parent)
+            for parent in parents
+            if isinstance(parent, st.DataSpec)
+        ]
         # here, if many parents potentially fail, we want to be sure
         # that all of them do it, and not only the first one (to
         # modify all statuses accordingly).
         # After, we only raise the first exception for the child.
 
         results = await asyncio.gather(*coros, return_exceptions=True)
         exceptions = [
@@ -539,14 +557,15 @@
         args, kwargs = dataset.parents()
         parents = list(args) + list(kwargs.values())
         coros = [
             self.async_sql_prepare(t.cast(st.Dataset, parent))
             if dataset.prototype() == sp.Dataset
             else self.async_prepare(parent)
             for parent in parents
+            if isinstance(parent, st.DataSpec)
         ]
         # here, if many parents potentially fail, we want to be sure
         # that all of them do it, and not only the first one (to
         # modify all statuses accordingly).
         # After, we only raise the first exception for the child.
 
         results = await asyncio.gather(*coros, return_exceptions=True)
@@ -635,25 +654,32 @@
         deserializer = deserialize(signature)
         nester = nest(signature)
         return tf.data.TFRecordDataset(filenames).map(deserializer).map(nester)
 
     def mock_value(
         self,
         transform: st.Transform,
-        *arguments: st.DataSpec,
-        **named_arguments: st.DataSpec,
+        *arguments: t.Union[st.DataSpec, st.Transform],
+        **named_arguments: t.Union[st.DataSpec, st.Transform],
     ) -> t.Any:
         """Compute the mock value of an external transform applied on
         Dataspecs.
         """
         start = time.perf_counter()
         assert transform.is_external()
-        mock_args = [arg.variant(st.ConstraintKind.MOCK) for arg in arguments]
+        mock_args = [
+            arg.variant(st.ConstraintKind.MOCK)
+            if isinstance(arg, st.DataSpec)
+            else arg  # `arg` can be a composed Transform
+            for arg in arguments
+        ]
         named_mock_args = {
             name: arg.variant(st.ConstraintKind.MOCK)
+            if isinstance(arg, st.DataSpec)
+            else arg  # `arg` can be a composed Transform
             for name, arg in named_arguments.items()
         }
 
         if any([ds is None for ds in mock_args]) or any(
             [ds is None for ds in named_mock_args.values()]
         ):
             raise ValueError(
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/local/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/local/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/remote/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/__init__.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     merge_data_and_admin,
 )
 from sarus_data_spec.arrow.conversion import to_pyarrow_table
 from sarus_data_spec.arrow.schema import type_from_arrow_schema
 from sarus_data_spec.dataspec_validator.signature import (
     SarusBoundSignature,
     SarusSignature,
+    SarusSignatureValue,
 )
 from sarus_data_spec.dataspec_validator.typing import PEPKind
 from sarus_data_spec.manager.async_utils import async_iter
 from sarus_data_spec.manager.ops.base import (
     DatasetImplementation,
     DatasetStaticChecker,
     DataspecStaticChecker,
@@ -164,23 +165,23 @@
         implementation = external_implementation(transform)
         bound_signature = implementation.signature().bind_dataspec(
             self.dataset
         )
         bound_signature.static_validation()
 
         if self.dataset.is_pep():
-            result = await implementation.call(bound_signature)
+            result = await implementation.compute(bound_signature)
             ds_result = t.cast(st.DatasetCastable, result)
             admin_data = await bound_signature.admin_data()
             output_admin_data = compute_admin_data(admin_data, ds_result)
             data_table = to_pyarrow_table(ds_result)
             table = merge_data_and_admin(data_table, output_admin_data)
 
         else:
-            result = await implementation.call(bound_signature)
+            result = await implementation.compute(bound_signature)
             data_table = to_pyarrow_table(result)
             table = create_admin_columns(data_table)
 
         return async_iter(table.to_batches(max_chunksize=batch_size))
 
 
 class ExternalScalarOp(ScalarImplementation):
@@ -190,37 +191,31 @@
         return await async_compute_external_value(
             transform, *ds_args, **ds_kwargs
         )
 
 
 async def async_compute_external_value(
     transform: st.Transform,
-    *ds_args: st.DataSpec,
-    **ds_kwargs: st.DataSpec,
+    *ds_args: t.Union[st.DataSpec, st.Transform],
+    **ds_kwargs: t.Union[st.DataSpec, st.Transform],
 ) -> t.Any:
     """Compute the value of an external transform applied on Dataspecs.
 
     This function computes the output value without manipulating the
     corresponding Dataspec. This is useful when we need to have access
     to the value of a Dataspec before its creation:
       - for computing a Mock value and inferring if the result is
         a Scalar or a Dataset.
     """
     implementation = external_implementation(transform)
     bound_signature = implementation.signature().bind(
         transform, *ds_args, **ds_kwargs
     )
     bound_signature.static_validation()
-
-    if implementation.is_dp(bound_signature):
-        data = await implementation.call(bound_signature)
-
-    else:
-        data = await implementation.call(bound_signature)
-
+    data = await implementation.compute(bound_signature)
     return data
 
 
 class ExternalOpImplementation:
     """External PEP op implementation class.
 
     This class wraps together several elements of an external op
@@ -257,15 +252,26 @@
             )
 
         non_dp_signature = external_implementation_from_id(
             self._non_dp_equivalent_id
         ).signature()
         return non_dp_signature.make_dp()
 
-    async def call(self, bound_signature: SarusBoundSignature) -> t.Any:
+    async def compute(self, bound_signature: SarusBoundSignature) -> t.Any:
+        if self.is_dp(bound_signature):
+            return await self.call_dp(bound_signature)
+        else:
+            signature_value = await bound_signature.collect_signature_value()
+            return self.call(signature_value)
+
+    def call(self, signature_value: SarusSignatureValue) -> t.Any:
+        raise NotImplementedError
+
+    async def call_dp(self, bound_signature: SarusBoundSignature) -> t.Any:
+        """DP ops `call` need to be async to compute schema, tasks, etc"""
         raise NotImplementedError
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         """Return the PEP properties of the transform.
 
         It takes the transform arguments as input because it can depend on some
         transform parameters. For instance, it is not PEP if we are aggregating
@@ -296,14 +302,35 @@
         return queries
 
     async def private_queries_and_task(
         self, signature: SarusBoundSignature
     ) -> t.Tuple[t.List[st.PrivateQuery], st.Task]:
         raise NotImplementedError
 
+    def callable(
+        self, composed_transform: st.Transform
+    ) -> t.Callable[..., t.Awaitable[t.Any]]:
+        """Build the transform's async callable.
+
+        The function takes an undefined number of named arguments.
+
+        It first collects the current transform's signature concrete values
+        using the passed variables' values. The concrete values are stored in a
+        SarusBoundSignature object so we can compute the current transform's
+        output by simply using the implementation's `call` method.
+        """
+        lambda_signature = self.signature().bind_composed(composed_transform)
+        previous_callable = lambda_signature.callable()
+
+        def composed_callable(*vars: t.Any, **kwvars: t.Any) -> t.Any:
+            signature_value = previous_callable(*vars, **kwvars)
+            return self.call(signature_value)
+
+        return composed_callable
+
 
 def external_implementation(
     transform: st.Transform,
 ) -> ExternalOpImplementation:
     """Return the implementation of an external op from a DataSpec.
 
     The mapping is done by the config file.
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/imblearn.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/imblearn.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from typing import Any, Callable, Dict, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 
 from sarus_data_spec.dataspec_validator.parameter_kind import DATASPEC, STATIC
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from .external_op import ExternalOpImplementation
 
 try:
     from imblearn import over_sampling, pipeline, under_sampling
 except ModuleNotFoundError:
@@ -41,16 +41,16 @@
         SarusParameter(
             name="verbose",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return pipeline.Pipeline(**kwargs)
 
 
 class imb_random_under_sampler(ExternalOpImplementation):
     _transform_id = "imblearn.IMB_RANDOM_UNDER_SAMPLER"
     _signature = SarusSignature(
         SarusParameter(
@@ -66,16 +66,16 @@
         SarusParameter(
             name="replacement",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return under_sampling.RandomUnderSampler(**kwargs)
 
 
 class imb_smotenc(ExternalOpImplementation):
     _transform_id = "imblearn.IMB_SMOTENC"
     _signature = SarusSignature(
         SarusParameter(
@@ -95,10 +95,10 @@
         SarusParameter(
             name="k_neighbors",
             annotation=Union[int, object],
             default=5,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return over_sampling.SMOTENC(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/numpy.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/numpy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, List, Literal, Optional, Tuple, Union
 
 from numpy.typing import ArrayLike, DTypeLike
 import numpy as np
 
 from sarus_data_spec.dataspec_validator.parameter_kind import DATASPEC, STATIC
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusParameterArray,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from .external_op import ExternalOpImplementation
 
 Casting = Literal["no", "equiv", "safe", "same_kind", "unsafe"]
 Order = Literal["K", "A", "C", "F"]
 
@@ -54,16 +54,16 @@
         SarusParameter(
             name="like",
             annotation=Optional[ArrayLike],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         if kwargs["like"] is None:
             del kwargs["like"]
         return np.array(**kwargs)
 
 
 # ------ FUNCTIONS ------
 class np_ceil(ExternalOpImplementation):
@@ -103,16 +103,16 @@
         SarusParameter(
             name="subok",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        x, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        x, kwargs = signature.collect_kwargs_method()
         return np.ceil(x, **kwargs)
 
 
 class np_floor(ExternalOpImplementation):
     _transform_id = "numpy.NP_FLOOR"
     _signature = SarusSignature(
         SarusParameter(
@@ -149,16 +149,16 @@
         SarusParameter(
             name="subok",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        x, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        x, kwargs = signature.collect_kwargs_method()
         return np.floor(x, **kwargs)
 
 
 class np_mean(ExternalOpImplementation):
     _transform_id = "numpy.NP_MEAN"
     _signature = SarusSignature(
         SarusParameter(
@@ -190,16 +190,16 @@
         SarusParameter(
             name="where",
             annotation=Optional[Union[bool, ArrayLike]],
             default=True,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return np.mean(**kwargs)
 
 
 class np_std(ExternalOpImplementation):
     _transform_id = "numpy.NP_STD"
     _signature = SarusSignature(
         SarusParameter(
@@ -236,30 +236,30 @@
         SarusParameter(
             name="where",
             annotation=Optional[Union[bool, ArrayLike]],
             default=True,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return np.std(**kwargs)
 
 
 class np_rand(ExternalOpImplementation):
     _transform_id = "numpy.NP_RAND"
     _signature = SarusSignature(
         SarusParameterArray(
             name="size",
             annotation=Optional[Union[int, List[int]]],
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        sizes = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        sizes = signature.collect_args()
         return np.random.random_sample(sizes)
 
 
 # ------ METHODS ------
 class np_astype(ExternalOpImplementation):
     _transform_id = "numpy.NP_ASTYPE"
     _signature = SarusSignature(
@@ -290,10 +290,10 @@
         SarusParameter(
             name="copy",
             annotation=bool,
             default=True,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.astype(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from pandas._libs.tslibs import BaseOffset
 from pandas.core.window.indexers import BaseIndexer
 import pandas as pd
 import pandas._typing as pdt
 
 from sarus_data_spec.dataspec_validator.parameter_kind import DATASPEC
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from ..external_op import ExternalOpImplementation
 
 GroupBy = Union[
     pd.core.groupby.DataFrameGroupBy,
     pd.core.groupby.SeriesGroupBy,
@@ -41,31 +41,31 @@
         SarusParameter(
             name="func",
             annotation=Optional[Union[Callable, Dict, List]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.agg(**kwargs)
 
 
 class pd_count_groupby(ExternalOpImplementation):
     _transform_id = "pandas.PD_COUNT_GROUPBY"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=GroupBy,
             condition=DATASPEC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.count(**kwargs)
 
 
 class pd_max_groupby(ExternalOpImplementation):
     _transform_id = "pandas.PD_MAX_GROUPBY"
     _signature = SarusSignature(
         SarusParameter(
@@ -81,16 +81,16 @@
         SarusParameter(
             name="min_count",
             annotation=int,
             default=-1,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.max(**kwargs)
 
 
 class pd_mean_groupby(ExternalOpImplementation):
     _transform_id = "pandas.PD_MEAN_GROUPBY"
     _signature = SarusSignature(
         SarusParameter(
@@ -101,16 +101,16 @@
         SarusParameter(
             name="numeric_only",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.mean(**kwargs)
 
 
 class pd_min_groupby(ExternalOpImplementation):
     _transform_id = "pandas.PD_MIN_GROUPBY"
     _signature = SarusSignature(
         SarusParameter(
@@ -126,16 +126,16 @@
         SarusParameter(
             name="min_count",
             annotation=int,
             default=-1,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.min(**kwargs)
 
 
 class pd_rolling_groupby(ExternalOpImplementation):
     _transform_id = "pandas.PD_ROLLING_GROUPBY"
     _signature = SarusSignature(
         SarusParameter(
@@ -180,16 +180,16 @@
         SarusParameter(
             name="method",
             annotation=Literal["single", "table"],
             default="single",
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.rolling(**kwargs)
 
 
 class pd_shift_groupby(ExternalOpImplementation):
     _transform_id = "pandas.PD_SHIFT_GROUPBY"
     _signature = SarusSignature(
         SarusParameter(
@@ -215,31 +215,31 @@
         SarusParameter(
             name="fill_value",
             annotation=Hashable,
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.shift(**kwargs)
 
 
 class pd_groups_groupby(ExternalOpImplementation):
     _transform_id = "pandas.PD_GROUPS_GROUPBY"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=GroupBy,
             condition=DATASPEC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return this.groups
 
 
 class pd_sum_groupby(ExternalOpImplementation):
     _transform_id = "pandas.PD_SUM_GROUPBY"
     _signature = SarusSignature(
         SarusParameter(
@@ -255,16 +255,16 @@
         SarusParameter(
             name="min_count",
             annotation=int,
             default=0,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.sum(**kwargs)
 
 
 class pd_std_groupby(ExternalOpImplementation):
     _transform_id = "pandas.PD_STD_GROUPBY"
     _signature = SarusSignature(
         SarusParameter(
@@ -275,16 +275,16 @@
         SarusParameter(
             name="ddof",
             annotation=int,
             default=1,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.std(**kwargs)
 
 
 class pd_median_groupby(ExternalOpImplementation):
     _transform_id = "pandas.PD_MEDIAN_GROUPBY"
     _signature = SarusSignature(
         SarusParameter(
@@ -295,10 +295,10 @@
         SarusParameter(
             name="numeric_only",
             annotation=bool,
             default=True,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.median(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,19 +19,24 @@
 from pandas._libs import lib
 from pandas._libs.tslibs import BaseOffset
 from pandas.core.window.indexers import BaseIndexer
 import numpy as np
 import pandas as pd
 import pandas._typing as pdt
 
-from sarus_data_spec.dataspec_validator.parameter_kind import DATASPEC, STATIC
+from sarus_data_spec.dataspec_validator.parameter_kind import (
+    DATASPEC,
+    STATIC,
+    TRANSFORM,
+)
 from sarus_data_spec.dataspec_validator.signature import (
     SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 from sarus_data_spec.dataspec_validator.typing import PEPKind
 
 from ..external_op import ExternalOpImplementation
 
 # Defined in pandas version > 1.3.5
 IgnoreRaise = t.Literal["ignore", "raise"]
@@ -86,16 +91,16 @@
         SarusParameter(
             name="copy",
             annotation=Optional[bool],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return pd.DataFrame(**kwargs)
 
 
 class pd_series(ExternalOpImplementation):
     _transform_id = "pandas.PD_SERIES"
     _signature = SarusSignature(
         SarusParameter(
@@ -129,16 +134,16 @@
         SarusParameter(
             name="fastpath",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return pd.Series(**kwargs)
 
 
 # ------ DataFrame & Series METHODS ------
 class pd_loc(ExternalOpImplementation):
     _transform_id = "pandas.PD_LOC"
     _signature = SarusSignature(
@@ -149,16 +154,16 @@
         ),
         SarusParameter(
             name="key",
             annotation=Tuple[Union[str, slice, List[str]], ...],
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> pd.DataFrame:
-        (this, key) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> pd.DataFrame:
+        (this, key) = signature.collect_args()
         return this.loc[key]
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         """Token preserving if the key is a tuple or a slice that
         selects all the rows (e.g. loc[:, "col"], loc[:]).
         Not PEP if the key is a single int.
         PEP in the other cases.
@@ -197,16 +202,16 @@
         SarusParameter(
             name="value",
             annotation=t.Any,
             condition=DATASPEC | STATIC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this, key, value) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, key, value) = signature.collect_args()
         this.loc[key] = value
         return this
 
 
 class pd_iloc(ExternalOpImplementation):
     _transform_id = "pandas.PD_ILOC"
     _signature = SarusSignature(
@@ -217,16 +222,16 @@
         ),
         SarusParameter(
             name="key",
             annotation=Tuple[Union[str, slice, List[str]], ...],
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> pd.DataFrame:
-        (this, key) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> pd.DataFrame:
+        (this, key) = signature.collect_args()
         return this.iloc[key]
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         """Token preserving the alignment if the key is a slice that
         selects all the rows (e.g. iloc[:]).
         Not PEP if the key is a single int.
         PEP in the other cases.
@@ -261,16 +266,16 @@
         SarusParameter(
             name="value",
             annotation=t.Any,
             condition=DATASPEC | STATIC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this, key, value) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, key, value) = signature.collect_args()
         this.iloc[key] = value
         return this
 
 
 class pd_head(ExternalOpImplementation):
     _transform_id = "pandas.PD_HEAD"
     _signature = SarusSignature(
@@ -282,16 +287,16 @@
         SarusParameter(
             name="n",
             annotation=int,
             default=5,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this, kwargs) = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, kwargs) = signature.collect_kwargs_method()
         return this.head(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.PEP
 
 
 class pd_astype(ExternalOpImplementation):
@@ -314,16 +319,16 @@
         SarusParameter(
             name="errors",
             annotation=IgnoreRaise,
             default="raise",
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> pd.DataFrame:
-        (this, kwargs) = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> pd.DataFrame:
+        (this, kwargs) = signature.collect_kwargs_method()
         return this.astype(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class pd_getitem(ExternalOpImplementation):
@@ -336,16 +341,16 @@
         ),
         SarusParameter(
             name="key",
             annotation=t.Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
-        (this, key) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, key) = signature.collect_args()
         return this[key]
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class pd_sum(ExternalOpImplementation):
@@ -380,16 +385,16 @@
         SarusParameter(
             name="min_count",
             annotation=int,
             default=0,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this, kwargs) = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, kwargs) = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["numeric_only"]
         return this.sum(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         """`axis=1`"""
         axis = signature["axis"].static_value()
@@ -423,16 +428,16 @@
         SarusParameter(
             name="numeric_only",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this, kwargs) = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, kwargs) = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["numeric_only"]
         return this.mean(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         """`axis=1`"""
         axis = signature["axis"].static_value()
@@ -471,16 +476,16 @@
         SarusParameter(
             name="numeric_only",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
-        (this, kwargs) = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, kwargs) = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["numeric_only"]
         return this.std(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         """`axis=1`"""
         axis = signature["axis"].static_value()
@@ -514,16 +519,16 @@
         SarusParameter(
             name="numeric_only",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
-        (this, kwargs) = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, kwargs) = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["numeric_only"]
         return this.median(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         """`axis=1`"""
         axis = signature["axis"].static_value()
@@ -536,16 +541,16 @@
         SarusParameter(
             name="this",
             annotation=t.Union[pd.Series, pd.DataFrame],
             condition=DATASPEC,
         )
     )
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
-        this = await signature["this"].collect()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this = signature["this"].value
         return this.abs()
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class pd_drop(ExternalOpImplementation):
@@ -592,16 +597,16 @@
         SarusParameter(
             name="errors",
             annotation=str,
             default="raise",
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["axis"]
         return this.drop(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         axis = signature["axis"].static_value()
         if axis in [0, 'columns']:
@@ -643,16 +648,16 @@
             annotation=bool,
             default=False,
             predicate=lambda x: x is False,
         ),
         name=_transform_id,
     )
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["subset"]
             del kwargs["thresh"]
         return this.dropna(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         axis = signature["axis"].static_value()
@@ -701,16 +706,16 @@
         SarusParameter(
             name="downcast",
             annotation=Optional[str],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.fillna(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         """`method` is `None`"""
         method = signature["method"].static_value()
         if method is None:
             return PEPKind.TOKEN_PRESERVING
@@ -728,16 +733,16 @@
         ),
         SarusParameter(
             name="values",
             annotation=Union[pd.Series, List[Any], Tuple[Any], pd.DataFrame],
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.isin(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class pd_isnull(ExternalOpImplementation):
@@ -746,16 +751,16 @@
         SarusParameter(
             name="this",
             annotation=Union[pd.Series, pd.DataFrame],
             condition=DATASPEC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, _ = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, _ = signature.collect_kwargs_method()
         return this.isnull()
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class pd_mask(ExternalOpImplementation):
@@ -793,16 +798,16 @@
         SarusParameter(
             name="level",
             annotation=Optional[Union[int, str]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.mask(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         """`cond` and `other` are not callable"""
         cond = signature["cond"].static_value()
         other = signature["other"].static_value()
         if callable(cond) or callable(other):
@@ -817,16 +822,16 @@
         SarusParameter(
             name="this",
             annotation=Union[pd.Series, pd.DataFrame],
             condition=DATASPEC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, _ = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, _ = signature.collect_kwargs_method()
         return this.notnull()
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class pd_rename(ExternalOpImplementation):
@@ -876,16 +881,16 @@
         SarusParameter(
             name="errors",
             annotation=Literal['ignore', 'raise'],
             default='ignore',
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.rename(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         """`mapper`, `index` and `columns` are not callable"""
         mapper = signature["mapper"].static_value()
         index = signature["index"].static_value()
         columns = signature["columns"].static_value()
@@ -932,16 +937,16 @@
             name="method",
             annotation=Literal['pad', 'ffill', 'bfill'],
             default=lib.no_default,
         ),
         name=_transform_id,
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.replace(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         """`value` is not `None`"""
         value = signature["value"].static_value()
         if value is None:
             return PEPKind.NOT_PEP
@@ -960,16 +965,16 @@
         SarusParameter(
             name="decimals",
             annotation=Union[int, dict, pd.Series],
             default=0,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.round(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class pd_select_dtypes(ExternalOpImplementation):
@@ -988,16 +993,16 @@
         SarusParameter(
             name="exclude",
             annotation=t.Optional[t.Union[pdt.Scalar, t.List]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
-        (this, kwargs) = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, kwargs) = signature.collect_kwargs_method()
         return this.select_dtypes(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.PEP
 
 
 class pd_add(ExternalOpImplementation):
@@ -1027,16 +1032,16 @@
         SarusParameter(
             name="level",
             annotation=Optional[Union[int, str]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["axis"]
         return this.add(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
@@ -1068,16 +1073,16 @@
         SarusParameter(
             name="level",
             annotation=Optional[Union[int, str]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["axis"]
         return this.sub(**kwargs)
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
@@ -1125,16 +1130,16 @@
         # SarusParameter(
         #     name="names",
         #     annotation=Optional[Union[Hashable, Sequence[Hashable]]],
         #     default=None,
         # ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["col_level"]
             del kwargs["col_fill"]
         return this.reset_index(**kwargs)
 
 
 class pd_min(ExternalOpImplementation):
@@ -1158,16 +1163,16 @@
         SarusParameter(
             name="numeric_only",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.min(**kwargs)
 
 
 class pd_max(ExternalOpImplementation):
     _transform_id = "pandas.PD_MAX"
     _signature = SarusSignature(
         SarusParameter(
@@ -1188,16 +1193,16 @@
         SarusParameter(
             name="numeric_only",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.max(**kwargs)
 
 
 class pd_shift(ExternalOpImplementation):
     _transform_id = "pandas.PD_SHIFT"
     _signature = SarusSignature(
         SarusParameter(
@@ -1223,16 +1228,16 @@
         SarusParameter(
             name="fill_value",
             annotation=Hashable,
             default=lib.no_default,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.shift(**kwargs)
 
 
 class pd_any(ExternalOpImplementation):
     _transform_id = "pandas.PD_ANY"
     _signature = SarusSignature(
         SarusParameter(
@@ -1253,16 +1258,16 @@
         SarusParameter(
             name="skipna",
             annotation=bool,
             default=True,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.any(**kwargs)
 
 
 class pd_describe(ExternalOpImplementation):
     _transform_id = "pandas.PD_DESCRIBE"
     _signature = SarusSignature(
         SarusParameter(
@@ -1283,16 +1288,16 @@
         SarusParameter(
             name="exclude",
             annotation=Optional[List[pdt.Dtype]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.describe(**kwargs)
 
 
 class pd_quantile(ExternalOpImplementation):
     _transform_id = "pandas.PD_QUANTILE"
     _signature = SarusSignature(
         SarusParameter(
@@ -1324,16 +1329,16 @@
         # SarusParameter(
         #     name="method",
         #     annotation=Literal["single", "table"],
         #     default="single",
         # ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["axis"]
             del kwargs["numeric_only"]
         return this.quantile(**kwargs)
 
 
 class pd_reindex(ExternalOpImplementation):
@@ -1394,16 +1399,16 @@
         SarusParameter(
             name="tolerance",
             annotation=Optional[Union[pdt.Scalar, List[pdt.Scalar]]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         # The pandas method is a bit weird and allows only one of
         # these to be specified at a time
         for name in ["labels", "index", "columns", "axis"]:
             if kwargs[name] is None:
                 del kwargs[name]
         return this.reindex(**kwargs)
 
@@ -1425,16 +1430,16 @@
         SarusParameter(
             name="numeric_only",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["axis"]
             del kwargs["numeric_only"]
         return this.count(**kwargs)
 
 
 class pd_transpose(ExternalOpImplementation):
@@ -1448,16 +1453,16 @@
         SarusParameter(
             name="copy",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.transpose(**kwargs)
 
 
 class pd_value_counts(ExternalOpImplementation):
     _transform_id = "pandas.PD_VALUE_COUNTS"
     _dp_equivalent_id = "pandas.PD_VALUE_COUNTS_DP"
     _signature = SarusSignature(
@@ -1489,16 +1494,16 @@
         SarusParameter(
             name="dropna",
             annotation=bool,
             default=True,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["subset"]
         return this.value_counts(**kwargs)
 
 
 class pd_to_dict(ExternalOpImplementation):
     _transform_id = "pandas.PD_TO_DICT"
@@ -1524,30 +1529,31 @@
         # SarusParameter(
         #     name="index",
         #     annotation=bool,
         #     default=True,
         # ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.to_dict(**kwargs)
 
 
 class pd_apply(ExternalOpImplementation):
     _transform_id = "pandas.PD_APPLY"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Union[pd.DataFrame, pd.Series],
             condition=DATASPEC,
         ),
         SarusParameter(
             name="func",
             annotation=pdt.AggFuncTypeBase,
+            condition=STATIC | TRANSFORM,
             predicate=lambda x: isinstance(x, str),
         ),
         SarusParameter(
             name="axis",
             annotation=pdt.Axis,
             default=0,
         ),
@@ -1559,23 +1565,81 @@
         SarusParameter(
             name="result_type",
             annotation=Optional[Literal["expand", "reduce", "broadcast"]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["axis"]
             del kwargs["result_type"]
             del kwargs["raw"]
         return this.apply(**kwargs)
 
 
+class pd_applymap(ExternalOpImplementation):
+    _transform_id = "pandas.PD_APPLYMAP"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=pd.DataFrame,
+            condition=DATASPEC,
+        ),
+        SarusParameter(
+            name="func",
+            annotation=pdt.AggFuncTypeBase,
+            condition=STATIC | TRANSFORM,
+            predicate=lambda x: isinstance(x, str),
+        ),
+        SarusParameter(
+            name="na_action",
+            annotation=Optional[Literal["ignore"]],
+            default=None,
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
+        return this.applymap(**kwargs)
+
+    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+        return PEPKind.TOKEN_PRESERVING
+
+
+class pd_map(ExternalOpImplementation):
+    _transform_id = "pandas.PD_MAP"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=pd.Series,
+            condition=DATASPEC,
+        ),
+        SarusParameter(
+            name="arg",
+            annotation=pdt.AggFuncTypeBase,
+            condition=STATIC | TRANSFORM,
+            predicate=lambda x: isinstance(x, str),
+        ),
+        SarusParameter(
+            name="na_action",
+            annotation=Optional[Literal["ignore"]],
+            default=None,
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
+        return this.map(**kwargs)
+
+    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+        return PEPKind.TOKEN_PRESERVING
+
+
 class pd_skew(ExternalOpImplementation):
     _transform_id = "pandas.PD_SKEW"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Union[pd.DataFrame, pd.Series],
             condition=DATASPEC,
@@ -1593,16 +1657,16 @@
         SarusParameter(
             name="numeric_only",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.skew(**kwargs)
 
 
 class pd_kurtosis(ExternalOpImplementation):
     _transform_id = "pandas.PD_KURTOSIS"
     _signature = SarusSignature(
         SarusParameter(
@@ -1623,16 +1687,16 @@
         SarusParameter(
             name="numeric_only",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.kurtosis(**kwargs)
 
 
 class pd_agg(ExternalOpImplementation):
     _transform_id = "pandas.PD_AGG"
     _signature = SarusSignature(
         SarusParameter(
@@ -1648,16 +1712,16 @@
         SarusParameter(
             name="axis",
             annotation=pdt.Axis,
             default=0,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.agg(**kwargs)
 
 
 class pd_droplevel(ExternalOpImplementation):
     _transform_id = "pandas.PD_DROPLEVEL"
     _signature = SarusSignature(
         SarusParameter(
@@ -1672,16 +1736,16 @@
         SarusParameter(
             name="axis",
             annotation=pdt.Axis,
             default=0,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.droplevel(**kwargs)
 
 
 class pd_sort_values(ExternalOpImplementation):
     _transform_id = "pandas.PD_SORT_VALUES"
     _signature = SarusSignature(
         SarusParameter(
@@ -1728,16 +1792,16 @@
             name="key",
             annotation=ValueKeyFunc,
             default=None,
         ),
         name=_transform_id,
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.sort_values(**kwargs)
 
 
 class pd_sort_values_series(ExternalOpImplementation):
     _transform_id = "pandas.PD_SORT_VALUES_SERIES"
     _signature = SarusSignature(
         SarusParameter(
@@ -1775,16 +1839,16 @@
             name="key",
             annotation=ValueKeyFunc,
             default=None,
         ),
         name=_transform_id,
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.sort_values(**kwargs)
 
 
 class pd_drop_duplicates(ExternalOpImplementation):
     _transform_id = "pandas.PD_DROP_DUPLICATES"
     _signature = SarusSignature(
         SarusParameter(
@@ -1811,16 +1875,16 @@
         SarusParameter(
             name="ignore_index",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["subset"]
             del kwargs["ignore_index"]
         return this.drop_duplicates(**kwargs)
 
 
 class pd_corr(ExternalOpImplementation):
@@ -1845,16 +1909,16 @@
         # SarusParameter(
         #     name="numeric_only",
         #     annotation=bool,
         #     default=False,
         # ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.corr(**kwargs)
 
 
 class pd_corr_series(ExternalOpImplementation):
     _transform_id = "pandas.PD_CORR_SERIES"
     _signature = SarusSignature(
         SarusParameter(
@@ -1879,16 +1943,16 @@
         # SarusParameter(
         #     name="numeric_only",
         #     annotation=bool,
         #     default=False,
         # ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.corr(**kwargs)
 
 
 # ------ DataFrame & Series PROPERTIES ------
 class pd_shape(ExternalOpImplementation):
     _transform_id = "pandas.PD_SHAPE"
     _dp_equivalent_id = "pandas.PD_SHAPE_DP"
@@ -1896,151 +1960,151 @@
         SarusParameter(
             name="this",
             annotation=t.Union[pd.Series, pd.DataFrame],
             condition=DATASPEC,
         )
     )
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return this.shape
 
 
 class pd_ndim(ExternalOpImplementation):
     _transform_id = "pandas.PD_NDIM"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Union[pd.DataFrame, pd.Series],
             condition=DATASPEC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return this.ndim
 
 
 class pd_name(ExternalOpImplementation):
     _transform_id = "pandas.PD_NAME"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=pd.Series,
             condition=DATASPEC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return this.name
 
 
 class pd_size(ExternalOpImplementation):
     _transform_id = "pandas.PD_SIZE"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Union[pd.DataFrame, pd.Series],
             condition=DATASPEC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return this.size
 
 
 class pd_axes(ExternalOpImplementation):
     _transform_id = "pandas.PD_AXES"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=pd.DataFrame,
             condition=DATASPEC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return this.axes
 
 
 class pd_columns(ExternalOpImplementation):
     _transform_id = "pandas.PD_COLUMNS"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=pd.DataFrame,
             condition=DATASPEC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return this.columns
 
 
 class pd_index(ExternalOpImplementation):
     _transform_id = "pandas.PD_INDEX"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Union[pd.DataFrame, pd.Series],
             condition=DATASPEC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return this.index
 
 
 class pd_dtype(ExternalOpImplementation):
     _transform_id = "pandas.PD_DTYPE"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=pd.Series,
             condition=DATASPEC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return this.dtype
 
 
 class pd_dtypes(ExternalOpImplementation):
     _transform_id = "pandas.PD_DTYPES"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Union[pd.DataFrame, pd.Series],
             condition=DATASPEC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return this.dtypes
 
 
 class pd_values(ExternalOpImplementation):
     _transform_id = "pandas.PD_VALUES"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Union[pd.DataFrame, pd.Series],
             condition=DATASPEC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return this.values
 
 
 class pd_join(ExternalOpImplementation):
     _transform_id = "pandas.PD_JOIN"
     _signature = SarusSignature(
         SarusParameter(
@@ -2076,16 +2140,16 @@
         SarusParameter(
             name="sort",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.join(**kwargs)
 
 
 class pd_groupby(ExternalOpImplementation):
     _transform_id = "pandas.PD_GROUPBY"
     _signature = SarusSignature(
         SarusParameter(
@@ -2131,16 +2195,16 @@
         SarusParameter(
             name="dropna",
             annotation=bool,
             default=True,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.groupby(**kwargs)
 
 
 class pd_merge(ExternalOpImplementation):
     _transform_id = "pandas.PD_MERGE"
     _signature = SarusSignature(
         SarusParameter(
@@ -2208,16 +2272,16 @@
         SarusParameter(
             name="validate",
             annotation=Optional[str],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.merge(**kwargs)
 
 
 class pd_append(ExternalOpImplementation):
     _transform_id = "pandas.PD_APPEND"
     _signature = SarusSignature(
         SarusParameter(
@@ -2243,16 +2307,16 @@
         SarusParameter(
             name="sort",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.append(**kwargs)
 
 
 class pd_nunique(ExternalOpImplementation):
     _transform_id = "pandas.PD_NUNIQUE"
     _signature = SarusSignature(
         SarusParameter(
@@ -2268,16 +2332,16 @@
         SarusParameter(
             name="dropna",
             annotation=bool,
             default=True,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["axis"]
         return this.nunique(**kwargs)
 
 
 class pd_rolling(ExternalOpImplementation):
     _transform_id = "pandas.PD_ROLLING"
@@ -2324,16 +2388,16 @@
         SarusParameter(
             name="method",
             annotation=str,
             default="single",
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.rolling(**kwargs)
 
 
 # ------ FUNCTIONS ------
 class pd_eq(ExternalOpImplementation):
     _transform_id = "pandas.PD_EQ"
     _signature = SarusSignature(
@@ -2345,16 +2409,16 @@
         SarusParameter(
             name="other",
             annotation=Union[pd.DataFrame, pd.Series],
             condition=DATASPEC | STATIC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this, other) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, other) = signature.collect_args()
         return this == other
 
 
 class pd_concat(ExternalOpImplementation):
     _transform_id = "pandas.PD_CONCAT"
     _signature = SarusSignature(
         SarusParameter(
@@ -2408,16 +2472,16 @@
         SarusParameter(
             name="copy",
             annotation=Optional[bool],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return pd.concat(**kwargs)
 
 
 class pd_get_dummies(ExternalOpImplementation):
     _transform_id = "pandas.PD_GET_DUMMIES"
     _signature = SarusSignature(
         SarusParameter(
@@ -2458,16 +2522,16 @@
         SarusParameter(
             name="dtype",
             annotation=Optional[np.dtype],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> pd.DataFrame:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> pd.DataFrame:
+        kwargs = signature.collect_kwargs()
         return pd.get_dummies(**kwargs)
 
 
 class pd_to_datetime(ExternalOpImplementation):
     _transform_id = "pandas.TO_DATETIME"
     _signature = SarusSignature(
         SarusParameter(
@@ -2523,16 +2587,16 @@
         SarusParameter(
             name="cache",
             annotation=bool,
             default=True,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return pd.to_datetime(**kwargs)
 
 
 # ------ INDEX METHODS ------
 class pd_union(ExternalOpImplementation):
     _transform_id = "pandas.PD_UNION"
     _signature = SarusSignature(
@@ -2549,10 +2613,10 @@
         SarusParameter(
             name="sort",
             annotation=Optional[bool],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.union(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         tasks = builder.build_query(
             builder.target([(epsilon, delta)], (0, epsilon))
         )
         query = builder.private_query(tasks)
         composed_query = t.cast(ComposedPrivateQuery, query)
         return list(composed_query.all_subqueries()), tasks
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
+    async def call_dp(self, signature: SarusBoundSignature) -> t.Any:
         """Implementation of DP shape.
 
         A DP implementation receives additional arguments compared to a
         standard external implementation:
             - `budget`: a list of sp.Scalar.PrivacyParams.Point
                 object containing each an epsilon and a delta values
             - `seed`: an integer used to parametrize random number generators
@@ -223,15 +223,15 @@
         tasks = builder.build_query(
             builder.target([(epsilon, delta)], (0, epsilon))
         )
         query = builder.private_query(tasks)
         composed_query = t.cast(ComposedPrivateQuery, query)
         return list(composed_query.all_subqueries()), tasks
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
+    async def call_dp(self, signature: SarusBoundSignature) -> t.Any:
         # Evaluate arguments
         parent_ds: st.Dataset = signature["this"].static_value()
         dataframe: pd.DataFrame = await parent_ds.async_to(pd.DataFrame)
         budget_value = await signature["budget"].collect()
         seed_value = await signature["seed"].collect()
         skipna = await signature["skipna"].collect()
 
@@ -357,15 +357,15 @@
         tasks = builder.build_query(
             builder.target([(epsilon, delta)], (0, epsilon))
         )
         query = builder.private_query(tasks)
         composed_query = t.cast(ComposedPrivateQuery, query)
         return list(composed_query.all_subqueries()), tasks
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
+    async def call_dp(self, signature: SarusBoundSignature) -> t.Any:
         # Evaluate arguments
         parent_ds: st.Dataset = signature["this"].static_value()
         dataframe: pd.DataFrame = await parent_ds.async_to(pd.DataFrame)
         budget_value = await signature["budget"].collect()
         seed_value = await signature["seed"].collect()
         skipna = await signature["skipna"].collect()
         pe = (await signature.admin_data()).to_pandas()
@@ -491,15 +491,15 @@
         tasks = builder.build_query(
             builder.target([(epsilon, delta)], (0, epsilon))
         )
         query = builder.private_query(tasks)
         composed_query = t.cast(ComposedPrivateQuery, query)
         return list(composed_query.all_subqueries()), tasks
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
+    async def call_dp(self, signature: SarusBoundSignature) -> t.Any:
         # Evaluate arguments
         parent_ds: st.Dataset = signature["this"].static_value()
         dataframe: pd.DataFrame = await parent_ds.async_to(pd.DataFrame)
         budget_value = await signature["budget"].collect()
         seed_value = await signature["seed"].collect()
         skipna = await signature["skipna"].collect()
         pe = (await signature.admin_data()).to_pandas()
@@ -625,15 +625,15 @@
         tasks = builder.build_query(
             builder.target([(epsilon, delta)], (0, epsilon))
         )
         query = builder.private_query(tasks)
         composed_query = t.cast(ComposedPrivateQuery, query)
         return list(composed_query.all_subqueries()), tasks
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
+    async def call_dp(self, signature: SarusBoundSignature) -> t.Any:
         # Evaluate arguments
         parent_ds: st.Dataset = signature["this"].static_value()
         dataframe: pd.DataFrame = await parent_ds.async_to(pd.DataFrame)
         budget_value = await signature["budget"].collect()
         seed_value = await signature["seed"].collect()
         skipna = await signature["skipna"].collect()
         pe = (await signature.admin_data()).to_pandas()
@@ -748,15 +748,15 @@
         tasks = builder.build_query(
             builder.target([(epsilon, delta)], (0, epsilon))
         )
         query = builder.private_query(tasks)
         composed_query = t.cast(ComposedPrivateQuery, query)
         return list(composed_query.all_subqueries()), tasks
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
+    async def call_dp(self, signature: SarusBoundSignature) -> t.Any:
         # Evaluate arguments
         parent_ds: st.Dataset = signature["this"].static_value()
         dataframe: pd.DataFrame = await parent_ds.async_to(pd.DataFrame)
         budget_value = await signature["budget"].collect()
         seed_value = await signature["seed"].collect()
 
         _, tasks = await self.private_queries_and_task(signature)
@@ -839,15 +839,15 @@
         tasks = builder.build_query(
             builder.target([(epsilon, delta)], (0, epsilon))
         )
         query = builder.private_query(tasks)
         composed_query = t.cast(ComposedPrivateQuery, query)
         return list(composed_query.all_subqueries()), tasks
 
-    async def call(self, signature: SarusBoundSignature) -> t.Any:
+    async def call_dp(self, signature: SarusBoundSignature) -> t.Any:
         """Implementation of DP shape.
 
         A DP implementation receives additional arguments compared to a
         standard external implementation:
             - `budget`: a list of sp.Scalar.PrivacyParams.Point
                 object containing each an epsilon and a delta values
             - `seed`: an integer used to parametrize random number generators
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 from typing import Any, Optional, Union
 
 import pandas as pd
 
 from sarus_data_spec.dataspec_validator.parameter_kind import DATASPEC, STATIC
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from .external_op import ExternalOpImplementation
 
 try:
     from ydata_profiling import ProfileReport
 except ModuleNotFoundError:
@@ -101,10 +101,10 @@
         SarusParameter(
             name='type_schema',
             annotation=Optional[dict],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ProfileReport(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Callable, Literal, Optional, Tuple, Union
 
 from numpy.typing import ArrayLike
 import numpy as np
 
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from ..external_op import ExternalOpImplementation
 
 try:
     from sklearn import cluster
     from sklearn.base import BaseEstimator
@@ -44,16 +44,16 @@
         SarusParameter(
             name="copy",
             annotation=bool,
             default=True,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return cluster.Birch(**kwargs)
 
 
 class sk_dbscan(ExternalOpImplementation):
     _transform_id = "sklearn.SK_DBSCAN"
     _signature = SarusSignature(
         SarusParameter(
@@ -94,16 +94,16 @@
         SarusParameter(
             name="n_jobs",
             annotation=Optional[int],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return cluster.DBSCAN(**kwargs)
 
 
 class sk_feature_agglomeration(ExternalOpImplementation):
     _transform_id = "sklearn.SK_FEATURE_AGGLOMERATION"
     _signature = SarusSignature(
         SarusParameter(
@@ -155,16 +155,16 @@
         SarusParameter(
             name="compute_distances",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return cluster.FeatureAgglomeration(**kwargs)
 
 
 class sk_kmeans(ExternalOpImplementation):
     _transform_id = "sklearn.SK_KMEANS"
     _signature = SarusSignature(
         SarusParameter(
@@ -212,16 +212,16 @@
         SarusParameter(
             name="algorithm",
             annotation=Literal["lloyd", "elkan", "auto", "full"],
             default="lloyd",
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return cluster.KMeans(**kwargs)
 
 
 class sk_minibatch_kmeans(ExternalOpImplementation):
     _transform_id = "sklearn.SK_MINIBATCH_KMEANS"
     _signature = SarusSignature(
         SarusParameter(
@@ -284,16 +284,16 @@
         SarusParameter(
             name="reassignment_ratio",
             annotation=float,
             default=0.01,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return cluster.MiniBatchKMeans(**kwargs)
 
 
 class sk_mean_shift(ExternalOpImplementation):
     _transform_id = "sklearn.SK_MEAN_SHIFT"
     _signature = SarusSignature(
         SarusParameter(
@@ -330,16 +330,16 @@
         SarusParameter(
             name="max_iter",
             annotation=int,
             default=300,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return cluster.MeanShift(**kwargs)
 
 
 class sk_optics(ExternalOpImplementation):
     _transform_id = "sklearn.SK_OPTICS"
     _signature = SarusSignature(
         SarusParameter(
@@ -439,16 +439,16 @@
             name="n_jobs",
             annotation=Optional[int],
             default=None,
             predicate=lambda x: x is None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return cluster.OPTICS(**kwargs)
 
 
 class sk_spectral_clustering(ExternalOpImplementation):
     _transform_id = "sklearn.SK_SPECTRAL_CLUSTERING"
     _signature = SarusSignature(
         SarusParameter(
@@ -533,16 +533,16 @@
         SarusParameter(
             name="verbose",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return cluster.SpectralClustering(**kwargs)
 
 
 class sk_spectral_biclustering(ExternalOpImplementation):
     _transform_id = "sklearn.SK_SPECTRAL_BICLUSTERING"
     _signature = SarusSignature(
         SarusParameter(
@@ -593,16 +593,16 @@
         SarusParameter(
             name="random_state",
             annotation=Optional[Union[int, np.random.RandomState]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return cluster.SpectralBiclustering(**kwargs)
 
 
 class sk_spectral_coclustering(ExternalOpImplementation):
     _transform_id = "sklearn.SK_SPECTRAL_COCLUSTERING"
     _signature = SarusSignature(
         SarusParameter(
@@ -638,16 +638,16 @@
         SarusParameter(
             name="random_state",
             annotation=Optional[Union[int, np.random.RandomState]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return cluster.SpectralCoclustering(**kwargs)
 
 
 class sk_affinity_propagation(ExternalOpImplementation):
     _transform_id = "sklearn.SK_AFFINITY_PROPAGATION"
     _signature = SarusSignature(
         SarusParameter(
@@ -688,16 +688,16 @@
         SarusParameter(
             name="random_state",
             annotation=Optional[Union[int, np.random.RandomState]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return cluster.AffinityPropagation(**kwargs)
 
 
 class sk_agglomerative_clustering(ExternalOpImplementation):
     _transform_id = "sklearn.SK_AGGLOMERATIVE_CLUSTERING"
     _signature = SarusSignature(
         SarusParameter(
@@ -756,10 +756,10 @@
         SarusParameter(
             name="compute_distances",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return cluster.AgglomerativeClustering(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, List, Literal, Optional, Tuple, Union
 
 from numpy.typing import ArrayLike
 
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from ..external_op import ExternalOpImplementation
 
 try:
     from sklearn import compose
     from sklearn.base import BaseEstimator
@@ -59,10 +59,10 @@
         SarusParameter(
             name="verbose_feature_names_out",
             annotation=bool,
             default=True,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return compose.ColumnTransformer(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Literal, Optional, Union
 
 import numpy as np
 
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from ..external_op import ExternalOpImplementation
 
 try:
     from sklearn import decomposition
 except ModuleNotFoundError:
@@ -62,10 +62,10 @@
         SarusParameter(
             name="random_state",
             annotation=Optional[Union[int, np.random.RandomState]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return decomposition.PCA(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     Union,
 )
 
 from numpy.typing import ArrayLike
 import numpy as np
 
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from ..external_op import ExternalOpImplementation
 
 try:
     from sklearn import ensemble
     from sklearn.base import BaseEstimator
@@ -58,16 +58,16 @@
         SarusParameter(
             name="random_state",
             annotation=Optional[Union[int, np.random.RandomState]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.AdaBoostClassifier(**kwargs)
 
 
 class sk_adaboost_regressor(ExternalOpImplementation):
     _transform_id = "sklearn.SK_ADABOOST_REGRESSOR"
     _signature = SarusSignature(
         SarusParameter(
@@ -98,16 +98,16 @@
         SarusParameter(
             name="base_estimator",
             annotation=Optional[BaseEstimator],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.AdaBoostRegressor(**kwargs)
 
 
 class sk_bagging_classifier(ExternalOpImplementation):
     _transform_id = "sklearn.SK_BAGGING_CLASSIFIER"
     _signature = SarusSignature(
         SarusParameter(
@@ -169,16 +169,16 @@
         SarusParameter(
             name="base_estimator",
             annotation=Optional[BaseEstimator],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.BaggingClassifier(**kwargs)
 
 
 class sk_bagging_regressor(ExternalOpImplementation):
     _transform_id = "sklearn.SK_BAGGING_REGRESSOR"
     _signature = SarusSignature(
         SarusParameter(
@@ -240,16 +240,16 @@
         SarusParameter(
             name="base_estimator",
             annotation=Optional[BaseEstimator],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.BaggingRegressor(**kwargs)
 
 
 class sk_extra_trees_classifier(ExternalOpImplementation):
     _transform_id = "sklearn.SK_EXTRA_TREES_CLASSIFIER"
     _signature = SarusSignature(
         SarusParameter(
@@ -343,16 +343,16 @@
         SarusParameter(
             name="max_samples",
             annotation=Optional[Union[int, float]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.ExtraTreesClassifier(**kwargs)
 
 
 class sk_extra_trees_regressor(ExternalOpImplementation):
     _transform_id = "sklearn.SK_EXTRA_TREES_REGRESSOR"
     _signature = SarusSignature(
         SarusParameter(
@@ -441,16 +441,16 @@
         SarusParameter(
             name="max_samples",
             annotation=Optional[Union[int, float]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.ExtraTreesRegressor(**kwargs)
 
 
 class sk_gradient_boosting_classifier(ExternalOpImplementation):
     _transform_id = "sklearn.SK_GRADIENT_BOOSTING_CLASSIFIER"
     _signature = SarusSignature(
         SarusParameter(
@@ -553,16 +553,16 @@
         SarusParameter(
             name="ccp_alpha",
             annotation=float,
             default=0.0,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.GradientBoostingClassifier(**kwargs)
 
 
 class sk_gradient_boosting_regressor(ExternalOpImplementation):
     _transform_id = "sklearn.SK_GRADIENT_BOOSTING_REGRESSOR"
     _signature = SarusSignature(
         SarusParameter(
@@ -675,16 +675,16 @@
         SarusParameter(
             name="ccp_alpha",
             annotation=float,
             default=0.0,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.GradientBoostingRegressor(**kwargs)
 
 
 class sk_isolation_forest(ExternalOpImplementation):
     _transform_id = "sklearn.SK_ISOLATION_FOREST"
     _signature = SarusSignature(
         SarusParameter(
@@ -730,16 +730,16 @@
         SarusParameter(
             name="warm_start",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.IsolationForest(**kwargs)
 
 
 class sk_random_forest_classifier(ExternalOpImplementation):
     _transform_id = "sklearn.SK_RANDOM_FOREST_CLASSIFIER"
     _signature = SarusSignature(
         SarusParameter(
@@ -834,16 +834,16 @@
         SarusParameter(
             name="max_samples",
             annotation=Optional[Union[int, float]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.RandomForestClassifier(**kwargs)
 
 
 class sk_random_forest_regressor(ExternalOpImplementation):
     _transform_id = "sklearn.SK_RANDOM_FOREST_REGRESSOR"
     _signature = SarusSignature(
         SarusParameter(
@@ -931,16 +931,16 @@
         SarusParameter(
             name="max_samples",
             annotation=Optional[Union[int, float]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.RandomForestRegressor(**kwargs)
 
 
 class sk_random_trees_embedding(ExternalOpImplementation):
     _transform_id = "sklearn.SK_RANDOM_TREES_EMBEDDING"
     _signature = SarusSignature(
         SarusParameter(
@@ -1001,16 +1001,16 @@
         SarusParameter(
             name="warm_start",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.RandomTreesEmbedding(**kwargs)
 
 
 class sk_stacking_classifier(ExternalOpImplementation):
     _transform_id = "sklearn.SK_STACKING_CLASSIFIER"
     _signature = SarusSignature(
         SarusParameter(
@@ -1050,16 +1050,16 @@
         SarusParameter(
             name="verbose",
             annotation=int,
             default=0,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.StackingClassifier(**kwargs)
 
 
 class sk_stacking_regressor(ExternalOpImplementation):
     _transform_id = "sklearn.SK_STACKING_REGRESSOR"
     _signature = SarusSignature(
         SarusParameter(
@@ -1090,16 +1090,16 @@
         SarusParameter(
             name="verbose",
             annotation=int,
             default=0,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.StackingRegressor(**kwargs)
 
 
 class sk_voting_classifier(ExternalOpImplementation):
     _transform_id = "sklearn.SK_VOTING_CLASSIFIER"
     _signature = SarusSignature(
         SarusParameter(
@@ -1131,16 +1131,16 @@
         SarusParameter(
             name="verbose",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.VotingClassifier(**kwargs)
 
 
 class sk_voting_regressor(ExternalOpImplementation):
     _transform_id = "sklearn.SK_VOTING_REGRESSOR"
     _signature = SarusSignature(
         SarusParameter(
@@ -1161,16 +1161,16 @@
         SarusParameter(
             name="verbose",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.VotingRegressor(**kwargs)
 
 
 class sk_hist_gradient_boosting_classifier(ExternalOpImplementation):
     _transform_id = "sklearn.SK_HIST_GRADIENT_BOOSTING_CLASSIFIER"
     _signature = SarusSignature(
         SarusParameter(
@@ -1281,16 +1281,16 @@
         SarusParameter(
             name="class_weight",
             annotation=Optional[Union[str, dict]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.HistGradientBoostingClassifier(**kwargs)
 
 
 class sk_hist_gradient_boosting_regressor(ExternalOpImplementation):
     _transform_id = "sklearn.SK_HIST_GRADIENT_BOOSTING_REGRESSOR"
     _signature = SarusSignature(
         SarusParameter(
@@ -1395,10 +1395,10 @@
         SarusParameter(
             name="random_state",
             annotation=Optional[Union[int, np.random.RandomState]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return ensemble.HistGradientBoostingRegressor(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Literal, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from ..external_op import ExternalOpImplementation
 
 try:
     from sklearn import impute
 except ModuleNotFoundError:
@@ -55,10 +55,10 @@
         SarusParameter(
             name="keep_empty_features",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return impute.SimpleImputer(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from ..external_op import ExternalOpImplementation
 
 try:
     from sklearn import inspection
     from sklearn.base import BaseEstimator
@@ -70,10 +70,10 @@
         SarusParameter(
             name="max_samples",
             annotation=Union[int, float],
             default=1.0,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return inspection.permutation_importance(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Optional, Union
 
 import numpy.typing as npt
 
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from ..external_op import ExternalOpImplementation
 
 try:
     from scipy.sparse import spmatrix
     from sklearn.base import BaseEstimator
@@ -37,16 +37,16 @@
         SarusParameter(
             name="sample_weight",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         if kwargs["sample_weight"] is None:
             del kwargs["sample_weight"]
         fitted_model = this.fit(**kwargs)
         return fitted_model
 
 
 class sk_fit_y(ExternalOpImplementation):
@@ -58,16 +58,16 @@
         ),
         SarusParameter(
             name="y",
             annotation=Union[npt.ArrayLike, spmatrix],
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         fitted_model = this.fit(**kwargs)
         return fitted_model
 
 
 class sk_predict(ExternalOpImplementation):
     _transform_id = "sklearn.SK_PREDICT"
     _signature = SarusSignature(
@@ -77,16 +77,16 @@
         ),
         SarusParameter(
             name="X",
             annotation=Union[npt.ArrayLike, spmatrix],
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.predict(**kwargs)
 
 
 class sk_predict_log_proba(ExternalOpImplementation):
     _transform_id = "sklearn.SK_PREDICT_LOG_PROBA"
     _signature = SarusSignature(
         SarusParameter(
@@ -95,16 +95,16 @@
         ),
         SarusParameter(
             name="X",
             annotation=Union[npt.ArrayLike, spmatrix],
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.predict_log_proba(**kwargs)
 
 
 class sk_predict_proba(ExternalOpImplementation):
     _transform_id = "sklearn.SK_PREDICT_PROBA"
     _signature = SarusSignature(
         SarusParameter(
@@ -113,16 +113,16 @@
         ),
         SarusParameter(
             name="X",
             annotation=Union[npt.ArrayLike, spmatrix],
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.predict_proba(**kwargs)
 
 
 class sk_transform(ExternalOpImplementation):
     _transform_id = "sklearn.SK_TRANSFORM"
     _signature = SarusSignature(
         SarusParameter(
@@ -131,16 +131,16 @@
         ),
         SarusParameter(
             name="X",
             annotation=Union[npt.ArrayLike, spmatrix],
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this, X) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, X) = signature.collect_args()
         return this.transform(X)
 
 
 class sk_inverse_transform(ExternalOpImplementation):
     _transform_id = "sklearn.SK_INVERSE_TRANSFORM"
     _signature = SarusSignature(
         SarusParameter(
@@ -149,16 +149,16 @@
         ),
         SarusParameter(
             name="X",
             annotation=Union[npt.ArrayLike, spmatrix],
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, X = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, X = signature.collect_args()
         return this.inverse_transform(X)
 
 
 class sk_score(ExternalOpImplementation):
     _transform_id = "sklearn.SK_SCORE"
     _signature = SarusSignature(
         SarusParameter(
@@ -177,16 +177,16 @@
         SarusParameter(
             name="sample_weight",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.score(**kwargs)
 
 
 class sk_fit_transform(ExternalOpImplementation):
     _transform_id = "sklearn.SK_LABEL_ENCODER_FIT_TRANSFORM"
     _signature = SarusSignature(
         SarusParameter(
@@ -200,16 +200,16 @@
         SarusParameter(
             name="y",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.fit_transform(**kwargs)
 
 
 class sk_split(ExternalOpImplementation):
     _transform_id = "sklearn.SK_SPLIT"
     _signature = SarusSignature(
         SarusParameter(
@@ -228,24 +228,24 @@
         SarusParameter(
             name="groups",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.split(**kwargs)
 
 
 class sk_get_n_splits(ExternalOpImplementation):
     _transform_id = "sklearn.SK_GET_N_SPLITS"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=BaseEstimator,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, kwargs = signature.collect_kwargs_method()
         return this.get_n_splits(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Optional
 
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from ..external_op import ExternalOpImplementation
 
 try:
     from sklearn import linear_model
 except ModuleNotFoundError:
@@ -36,10 +36,10 @@
         SarusParameter(
             name="positive",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return linear_model.LinearRegression(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, List, Literal, Optional, Union
 
 import numpy.typing as npt
 
 from sarus_data_spec.dataspec_validator.parameter_kind import DATASPEC, STATIC
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from ..external_op import ExternalOpImplementation
 
 try:
     from scipy.sparse import spmatrix
     from sklearn import metrics
@@ -40,16 +40,16 @@
         SarusParameter(
             name="sample_weight",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return metrics.accuracy_score(**kwargs)
 
 
 class sk_average_precision_score(ExternalOpImplementation):
     _transform_id = "sklearn.SK_AVERAGE_PRECISION_SCORE"
     _signature = SarusSignature(
         SarusParameter(
@@ -77,16 +77,16 @@
         SarusParameter(
             name="sample_weight",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return metrics.average_precision_score(**kwargs)
 
 
 class sk_classification_report(ExternalOpImplementation):
     _transform_id = "sklearn.SK_CLASSIFICATION_REPORT"
     _signature = SarusSignature(
         SarusParameter(
@@ -127,16 +127,16 @@
         SarusParameter(
             name="zero_division",
             annotation=Literal["warn", 0, 1],
             default="warn",
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return metrics.classification_report(**kwargs)
 
 
 class sk_confusion_matrix(ExternalOpImplementation):
     _transform_id = "sklearn.SK_CONFUSION_MATRIX"
     _signature = SarusSignature(
         SarusParameter(
@@ -162,16 +162,16 @@
         SarusParameter(
             name="normalize",
             annotation=Optional[Literal['true', 'pred', 'all']],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return metrics.confusion_matrix(**kwargs)
 
 
 class sk_f1_score(ExternalOpImplementation):
     _transform_id = "sklearn.SK_F1_SCORE"
     _signature = SarusSignature(
         SarusParameter(
@@ -209,16 +209,16 @@
         SarusParameter(
             name="zero_division",
             annotation=Literal["warn", 0, 1],
             default="warn",
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return metrics.f1_score(**kwargs)
 
 
 class sk_precision_recall_curve(ExternalOpImplementation):
     _transform_id = "sklearn.SK_PRECISION_RECALL_CURVE"
     _signature = SarusSignature(
         SarusParameter(
@@ -239,16 +239,16 @@
         SarusParameter(
             name="sample_weight",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return metrics.precision_recall_curve(**kwargs)
 
 
 class sk_precision_score(ExternalOpImplementation):
     _transform_id = "sklearn.SK_PRECISION_SCORE"
     _signature = SarusSignature(
         SarusParameter(
@@ -286,16 +286,16 @@
         SarusParameter(
             name="zero_division",
             annotation=Literal['warn', 0, 1],
             default='warn',
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return metrics.precision_score(**kwargs)
 
 
 class sk_recall_score(ExternalOpImplementation):
     _transform_id = "sklearn.SK_RECALL_SCORE"
     _signature = SarusSignature(
         SarusParameter(
@@ -333,16 +333,16 @@
         SarusParameter(
             name="zero_division",
             annotation=Literal['warn', 0, 1],
             default='warn',
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return metrics.recall_score(**kwargs)
 
 
 class sk_roc_auc_score(ExternalOpImplementation):
     _transform_id = "sklearn.SK_ROC_AUC_SCORE"
     _signature = SarusSignature(
         SarusParameter(
@@ -380,16 +380,16 @@
         SarusParameter(
             name="labels",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return metrics.roc_auc_score(**kwargs)
 
 
 class sk_auc(ExternalOpImplementation):
     _transform_id = "sklearn.SK_AUC"
     _signature = SarusSignature(
         SarusParameter(
@@ -400,16 +400,16 @@
         SarusParameter(
             name="y",
             annotation=npt.ArrayLike,
             condition=DATASPEC | STATIC,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return metrics.auc(**kwargs)
 
 
 class sk_roc_curve(ExternalOpImplementation):
     _transform_id = "sklearn.SK_ROC_CURVE"
     _signature = SarusSignature(
         SarusParameter(
@@ -435,10 +435,10 @@
         SarusParameter(
             name="drop_intermediate",
             annotation=bool,
             default=True,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return metrics.roc_curve(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 
 from sarus_data_spec.dataspec_validator.parameter_kind import DATASPEC, STATIC
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusParameterArray,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from ..external_op import ExternalOpImplementation
 
 try:
     from scipy.sparse import spmatrix
     from sklearn import model_selection
@@ -51,16 +51,16 @@
         SarusParameter(
             name="random_state",
             annotation=Optional[Union[int, np.random.RandomState]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return model_selection.KFold(**kwargs)
 
 
 class sk_repeated_stratified_kfold(ExternalOpImplementation):
     _transform_id = "sklearn.SK_REPEATED_STRATIFIED_KFOLD"
     _signature = SarusSignature(
         SarusParameter(
@@ -76,16 +76,16 @@
         SarusParameter(
             name="random_state",
             annotation=Optional[Union[int, np.random.RandomState]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return model_selection.RepeatedStratifiedKFold(**kwargs)
 
 
 class sk_cross_val_score(ExternalOpImplementation):
     _transform_id = "sklearn.SK_CROSS_VAL_SCORE"
     _signature = SarusSignature(
         SarusParameter(
@@ -140,16 +140,16 @@
         SarusParameter(
             name="error_score",
             annotation=Union[Literal["raise"], np.number],
             default=np.nan,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return model_selection.cross_val_score(**kwargs)
 
 
 class sk_train_test_split(ExternalOpImplementation):
     _transform_id = "sklearn.SK_TRAIN_TEST_SPLIT"
     _signature = SarusSignature(
         SarusParameterArray(
@@ -182,16 +182,16 @@
         SarusParameter(
             name="stratify",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        arrays, kwargs = await signature.collect()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        arrays, kwargs = signature.collect()
         return model_selection.train_test_split(*arrays, **kwargs)
 
 
 class sk_time_series_split(ExternalOpImplementation):
     _transform_id = "sklearn.SK_TIME_SERIES_SPLIT"
     _signature = SarusSignature(
         SarusParameter(
@@ -212,10 +212,10 @@
         SarusParameter(
             name="gap",
             annotation=int,
             default=0,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return model_selection.TimeSeriesSplit(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, List, Optional, Tuple, Union
 
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from ..external_op import ExternalOpImplementation
 
 try:
     from sklearn import pipeline
     from sklearn.base import BaseEstimator
@@ -31,10 +31,10 @@
         SarusParameter(
             name="verbose",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return pipeline.Pipeline(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Callable, Dict, List, Literal, Optional, Union
 
 import numpy.typing as npt
 
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from ..external_op import ExternalOpImplementation
 
 try:
     from scipy.sparse import spmatrix
     from sklearn import preprocessing
@@ -58,16 +58,16 @@
         SarusParameter(
             name="inv_kw_args",
             annotation=Optional[Dict],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return preprocessing.FunctionTransformer(**kwargs)
 
 
 class sk_onehot(ExternalOpImplementation):
     _transform_id = "sklearn.SK_ONEHOT"
     _signature = SarusSignature(
         SarusParameter(
@@ -110,24 +110,24 @@
         SarusParameter(
             name="max_categories",
             annotation=Optional[int],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return preprocessing.OneHotEncoder(**kwargs)
 
 
 class sk_label_encoder(ExternalOpImplementation):
     _transform_id = "sklearn.SK_LABEL_ENCODER"
     _signature = SarusSignature()
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
+    def call(self, signature: SarusSignatureValue) -> Any:
         return preprocessing.LabelEncoder()
 
 
 class sk_scale(ExternalOpImplementation):
     _transform_id = "sklearn.SK_SCALE"
     _signature = SarusSignature(
         SarusParameter(
@@ -152,10 +152,10 @@
         SarusParameter(
             name="copy",
             annotation=bool,
             default=True,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return preprocessing.scale(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Literal, Optional, Union
 
 import numpy as np
 
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from ..external_op import ExternalOpImplementation
 
 try:
     from sklearn import svm
 except ModuleNotFoundError:
@@ -95,10 +95,10 @@
         SarusParameter(
             name="random_state",
             annotation=Optional[Union[int, np.random.RandomState]],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return svm.SVC(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/skopt.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/skopt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from .external_op import ExternalOpImplementation
 
 try:
     from sklearn.base import BaseEstimator
     from sklearn.model_selection import BaseCrossValidator
@@ -99,10 +99,10 @@
         SarusParameter(
             name="return_train_score",
             annotation=bool,
             default=False,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return skopt.BayesSearchCV(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/std.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/std.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, Iterable, List, Optional
 
 from sarus_data_spec.dataspec_validator.signature import (
     SarusBoundSignature,
     SarusParameter,
     SarusParameterArray,
     SarusParameterMapping,
     SarusSignature,
+    SarusSignatureValue,
 )
 from sarus_data_spec.dataspec_validator.typing import PEPKind
 
 from .external_op import ExternalOpImplementation
 
 
 class add(ExternalOpImplementation):
@@ -21,16 +22,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return this + other
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class sub(ExternalOpImplementation):
@@ -40,18 +41,19 @@
             name="this",
             annotation=Any,
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
+        name="substract",
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return this - other
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class rsub(ExternalOpImplementation):
@@ -63,16 +65,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return other - this
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class mul(ExternalOpImplementation):
@@ -82,18 +84,19 @@
             name="this",
             annotation=Any,
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
+        name="multiply",
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return this * other
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class div(ExternalOpImplementation):
@@ -105,16 +108,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return this / other
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class rdiv(ExternalOpImplementation):
@@ -126,16 +129,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return other / this
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class invert(ExternalOpImplementation):
@@ -143,16 +146,16 @@
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return ~this
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class length(ExternalOpImplementation):
@@ -160,16 +163,16 @@
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return len(this)
 
 
 class getitem(ExternalOpImplementation):
     _transform_id = "std.GETITEM"
     _signature = SarusSignature(
         SarusParameter(
@@ -179,16 +182,16 @@
         SarusParameter(
             name="key",
             annotation=Any,
         ),
         name=_transform_id,
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, key = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, key = signature.collect_args()
         return this[key]
 
 
 class setitem(ExternalOpImplementation):
     _transform_id = "std.SETITEM"
     _signature = SarusSignature(
         SarusParameter(
@@ -202,16 +205,16 @@
         SarusParameter(
             name="value",
             annotation=Any,
         ),
         name=_transform_id,
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, key, value = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, key, value = signature.collect_args()
         this[key] = value
         return this
 
 
 class greater_than(ExternalOpImplementation):
     _transform_id = "std.GT"
     _signature = SarusSignature(
@@ -221,16 +224,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return this > other
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class greater_equal(ExternalOpImplementation):
@@ -242,16 +245,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return this >= other
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class lower_than(ExternalOpImplementation):
@@ -263,16 +266,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return this < other
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class lower_equal(ExternalOpImplementation):
@@ -284,16 +287,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return this <= other
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class not_equal(ExternalOpImplementation):
@@ -305,16 +308,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return this != other
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class neg(ExternalOpImplementation):
@@ -322,16 +325,16 @@
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return -this
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class pos(ExternalOpImplementation):
@@ -339,16 +342,16 @@
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return +this
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class _abs(ExternalOpImplementation):
@@ -356,16 +359,16 @@
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return abs(this)
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class _round(ExternalOpImplementation):
@@ -373,16 +376,16 @@
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return round(this)
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class modulo(ExternalOpImplementation):
@@ -394,16 +397,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return this % other
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class rmodulo(ExternalOpImplementation):
@@ -415,16 +418,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return other % this
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class _or(ExternalOpImplementation):
@@ -436,16 +439,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return this | other
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class ror(ExternalOpImplementation):
@@ -457,16 +460,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return other | this
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class _and(ExternalOpImplementation):
@@ -478,16 +481,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return this & other
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class rand(ExternalOpImplementation):
@@ -499,16 +502,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, other = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, other = signature.collect_args()
         return other & this
 
     def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
         return PEPKind.TOKEN_PRESERVING
 
 
 class _int(ExternalOpImplementation):
@@ -516,58 +519,58 @@
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return int(this)
 
 
 class _float(ExternalOpImplementation):
     _transform_id = "std.FLOAT"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return float(this)
 
 
 class _list(ExternalOpImplementation):
     _transform_id = "std.LIST"
     _signature = SarusSignature(
         SarusParameterArray(
             name="elem",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        elems = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        elems = signature.collect_args()
         return list(elems)
 
 
 class _dict(ExternalOpImplementation):
     _transform_id = "std.DICT"
     _signature = SarusSignature(
         SarusParameterMapping(
             name="elem",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        _, elems = await signature.collect()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        _, elems = signature.collect()
         return dict(**elems)
 
 
 class _slice(ExternalOpImplementation):
     _transform_id = "std.SLICE"
     _signature = SarusSignature(
         SarusParameter(
@@ -583,87 +586,115 @@
         SarusParameter(
             name="step",
             annotation=Optional[int],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (start, stop, step) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (start, stop, step) = signature.collect_args()
         return slice(start, stop, step)
 
 
 class _set(ExternalOpImplementation):
     _transform_id = "std.SET"
     _signature = SarusSignature(
         SarusParameterArray(
             name="elem",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        elems = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        elems = signature.collect_args()
         return set(elems)
 
 
 class _tuple(ExternalOpImplementation):
     _transform_id = "std.TUPLE"
     _signature = SarusSignature(
         SarusParameterArray(
             name="elem",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        elems = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        elems = signature.collect_args()
         return tuple(elems)
 
 
+class _string(ExternalOpImplementation):
+    _transform_id = "std.STRING"
+    _signature = SarusSignature(
+        SarusParameterArray(
+            name="this",
+            annotation=Any,
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
+        return str(this)
+
+
+class _bool(ExternalOpImplementation):
+    _transform_id = "std.BOOL"
+    _signature = SarusSignature(
+        SarusParameterArray(
+            name="this",
+            annotation=Any,
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
+        return bool(this)
+
+
 class keys(ExternalOpImplementation):
     _transform_id = "std.KEYS"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Dict,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return list(this.keys())
 
 
 class values(ExternalOpImplementation):
     _transform_id = "std.VALUES"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Dict,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return list(this.values())
 
 
 class sudo(ExternalOpImplementation):
     _transform_id = "std.SUDO"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Any,
         ),
         name="sudo",
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
         return this
 
 
 class extend(ExternalOpImplementation):
     _transform_id = "std.EXTEND"
     _signature = SarusSignature(
         SarusParameter(
@@ -672,16 +703,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=List,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this, other) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, other) = signature.collect_args()
         this.extend(other)
         return this
 
 
 class append(ExternalOpImplementation):
     _transform_id = "std.APPEND"
     _signature = SarusSignature(
@@ -691,16 +722,16 @@
         ),
         SarusParameter(
             name="other",
             annotation=Any,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this, other) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, other) = signature.collect_args()
         this.append(other)
         return this
 
 
 class pop(ExternalOpImplementation):
     _transform_id = "std.POP"
     _signature = SarusSignature(
@@ -711,10 +742,244 @@
         SarusParameter(
             name="index",
             annotation=int,
             default=-1,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this, index) = await signature.collect_args()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, index) = signature.collect_args()
         return this.pop(index)
+
+
+class split(ExternalOpImplementation):
+    _transform_id = "std.SPLIT"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=str,
+        ),
+        SarusParameter(
+            name="separator",
+            annotation=str,
+            default=" ",
+        ),
+        SarusParameter(
+            name="maxsplit",
+            annotation=int,
+            default=-1,
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, separator, maxsplit = signature.collect_args()
+        return this.split(separator, maxsplit)
+
+
+class join(ExternalOpImplementation):
+    _transform_id = "std.JOIN"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=str,
+        ),
+        SarusParameter(
+            name="iterable",
+            annotation=Iterable,
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        this, iterable = signature.collect_args()
+        return this.join(iterable)
+
+
+class capitalize(ExternalOpImplementation):
+    _transform_id = "std.CAPITALIZE"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=str,
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
+        return this.capitalize()
+
+
+class casefold(ExternalOpImplementation):
+    _transform_id = "std.CASEFOLD"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=str,
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
+        return this.casefold()
+
+
+class center(ExternalOpImplementation):
+    _transform_id = "std.CENTER"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=str,
+        ),
+        SarusParameter(
+            name="width",
+            annotation=int,
+        ),
+        SarusParameter(name="fillchar", annotation=str, default=" "),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, width, fillchar) = signature.collect_args()
+        return this.center(width, fillchar)
+
+
+class expandtabs(ExternalOpImplementation):
+    _transform_id = "std.EXPANDTABS"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=str,
+        ),
+        SarusParameter(
+            name="tabsize",
+            annotation=int,
+            default=8,
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, tabsize) = signature.collect_args()
+        return this.expandtabs(tabsize)
+
+
+class lower(ExternalOpImplementation):
+    _transform_id = "std.LOWER"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=str,
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
+        return this.lower()
+
+
+class upper(ExternalOpImplementation):
+    _transform_id = "std.UPPER"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=str,
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
+        return this.upper()
+
+
+class lstrip(ExternalOpImplementation):
+    _transform_id = "std.LSTRIP"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=str,
+        ),
+        SarusParameter(
+            name="chars",
+            annotation=str,
+            default=" ",
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, chars) = signature.collect_args()
+        return this.lstrip(chars)
+
+
+class rstrip(ExternalOpImplementation):
+    _transform_id = "std.RSTRIP"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=str,
+        ),
+        SarusParameter(
+            name="chars",
+            annotation=str,
+            default=" ",
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, chars) = signature.collect_args()
+        return this.rstrip(chars)
+
+
+class strip(ExternalOpImplementation):
+    _transform_id = "std.STRIP"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=str,
+        ),
+        SarusParameter(
+            name="chars",
+            annotation=str,
+            default=" ",
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, chars) = signature.collect_args()
+        return this.strip(chars)
+
+
+class replace(ExternalOpImplementation):
+    _transform_id = "std.REPLACE"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=str,
+        ),
+        SarusParameter(
+            name="old",
+            annotation=str,
+        ),
+        SarusParameter(
+            name="new",
+            annotation=str,
+        ),
+        SarusParameter(
+            name="count",
+            annotation=int,
+            default=-1,
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this, old, new, count) = signature.collect_args()
+        return this.replace(old, new, count)
+
+
+class splitlines(ExternalOpImplementation):
+    _transform_id = "std.SPLITLINES"
+    _signature = SarusSignature(
+        SarusParameter(
+            name="this",
+            annotation=str,
+        ),
+    )
+
+    def call(self, signature: SarusSignatureValue) -> Any:
+        (this,) = signature.collect_args()
+        return this.splitlines()
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/typing.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/utils.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/external/xgboost.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/xgboost.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Callable, Dict, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 
 from sarus_data_spec.dataspec_validator.signature import (
-    SarusBoundSignature,
     SarusParameter,
     SarusSignature,
+    SarusSignatureValue,
 )
 
 from .external_op import ExternalOpImplementation
 
 try:
     import xgboost
 except ModuleNotFoundError:
@@ -215,10 +215,10 @@
         SarusParameter(
             name="use_label_encoder",
             annotation=Optional[bool],
             default=None,
         ),
     )
 
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        kwargs = await signature.collect_kwargs()
+    def call(self, signature: SarusSignatureValue) -> Any:
+        kwargs = signature.collect_kwargs()
         return xgboost.XGBClassifier(**kwargs)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,18 @@
     DatasetStaticChecker,
     DataspecStaticChecker,
     ScalarImplementation,
 )
 from sarus_data_spec.manager.ops.processor.external.external_op import (  # noqa: E501
     ExternalDatasetOp,
     ExternalDatasetStaticChecker,
+    ExternalOpImplementation,
     ExternalScalarOp,
     ExternalScalarStaticChecker,
+    external_implementation,
 )
 
 try:
     from sarus_data_spec.manager.ops.processor.standard.differentiated_sample import (  # noqa: E501
         DifferentiatedSample,
         DifferentiatedSampleStaticChecker,
     )
@@ -161,14 +163,22 @@
     )
 except ModuleNotFoundError:
     logger = logging.getLogger(__name__)
     logger.info("Transforms: ValidatedUserType not available.")
 import sarus_data_spec.typing as st
 
 
+def get_implementation(transform: st.Transform) -> ExternalOpImplementation:
+    if not transform.is_external():
+        raise NotImplementedError(
+            "Cannot get implementation of internal transform."
+        )
+    return external_implementation(transform)
+
+
 def get_dataset_op(
     transform: st.Transform,
 ) -> t.Tuple[t.Type[DatasetImplementation], t.Type[DatasetStaticChecker]]:
     if transform.is_external():
         return ExternalDatasetOp, ExternalDatasetStaticChecker
     elif transform.protobuf().spec.HasField('sample'):
         return Sample, SampleStaticChecker
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/standard_op.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 
 class StandardDatasetImplementation(DatasetImplementation):
     """Object that executes first routing among ops between
     transformed/source and processor
     """
 
-    def parents(self) -> t.List[st.DataSpec]:
+    def parents(self) -> t.List[t.Union[st.DataSpec, st.Transform]]:
         return parents(self.dataset)
 
     def parent(self, kind: str = 'dataset') -> t.Union[st.Dataset, st.Scalar]:
         return parent(self.dataset, kind=kind)
 
     async def parent_to_arrow(
         self, batch_size: int = 10000
@@ -199,15 +199,15 @@
     ...
 
 
 class StandardScalarImplementation(ScalarImplementation):
     def parent(self, kind: str = 'dataset') -> st.DataSpec:
         return parent(self.scalar, kind=kind)
 
-    def parents(self) -> t.List[st.DataSpec]:
+    def parents(self) -> t.List[t.Union[st.DataSpec, st.Transform]]:
         return parents(self.scalar)
 
     async def parent_to_arrow(
         self, batch_size: int = 10000
     ) -> t.AsyncIterator[pa.RecordBatch]:
         parent = self.parent(kind='dataset')
         assert isinstance(parent, Dataset)
@@ -235,11 +235,13 @@
         ]
     else:
         parent = [element for element in pars if isinstance(element, Scalar)]
     assert len(parent) == 1
     return parent[0]
 
 
-def parents(dataspec: st.DataSpec) -> t.List[st.DataSpec]:
+def parents(
+    dataspec: st.DataSpec,
+) -> t.List[t.Union[st.DataSpec, st.Transform]]:
     parents_args, parents_kwargs = dataspec.parents()
     parents_args.extend(parents_kwargs.values())
     return parents_args
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/source/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/manager/typing.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,16 +197,16 @@
     def is_remote(self, dataspec: st.DataSpec) -> bool:
         """Is the dataspec a remotely defined dataset."""
         ...
 
     def infer_output_type(
         self,
         transform: st.Transform,
-        *arguments: st.DataSpec,
-        **named_arguments: st.DataSpec,
+        *arguments: t.Union[st.DataSpec, st.Transform],
+        **named_arguments: t.Union[st.DataSpec, st.Transform],
     ) -> Tuple[str, Callable[[st.DataSpec], None]]:
         ...
 
     def foreign_keys(self, dataset: st.Dataset) -> Dict[st.Path, st.Path]:
         ...
 
     async def async_foreign_keys(
@@ -301,14 +301,19 @@
         *arguments: st.DataSpec,
         **named_arguments: st.DataSpec,
     ) -> t.Any:
         """Compute the mock value of an external transform applied on
         Dataspecs.
         """
 
+    def composed_callable(
+        self, transform: st.Transform
+    ) -> t.Callable[..., t.Any]:
+        """Return a Python callable of a composed transform."""
+
 
 @runtime_checkable
 class HasManager(Protocol):
     """Has a manager."""
 
     def manager(self) -> Manager:
         """Return a manager (usually a singleton)."""
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/marginals.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/marginals.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/multiplicity.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/multiplicity.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/path.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/path.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/predicate.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/predicate.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/__init__.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/attribute_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/bounds_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/constraint_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/dataset_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/links_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/links_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/manager_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/marginals_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/marginals_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/multiplicity_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/multiplicity_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/multiplicity_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/multiplicity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/path_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/path_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/predicate_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/proto_container_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/proto_container_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/relation_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/relation_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/scalar_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/scalar_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/schema.proto` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/schema.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/schema_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/size_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/size_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/statistics_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/status_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/status_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/transform.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/transform_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/transform_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/type_pb2.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/type_pb2.pyi` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/utilities.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/scalar.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/scalar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 from __future__ import annotations
 
-from typing import Collection, Dict, List, Optional, Set, Tuple, Type, cast
+from typing import (
+    Collection,
+    Dict,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 import datetime
 import typing as t
 
 from sarus_data_spec.base import Referring
 from sarus_data_spec.transform import Transform
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
@@ -103,27 +113,36 @@
             self.storage().referrable(
                 self.protobuf().spec.transformed.transform
             ),
         )
 
     def parents(
         self,
-    ) -> Tuple[List[st.DataSpec], Dict[str, st.DataSpec]]:
+    ) -> Tuple[
+        List[Union[st.DataSpec, st.Transform]],
+        Dict[str, Union[st.DataSpec, st.Transform]],
+    ]:
         if not self.is_transformed():
             return list(), dict()
 
         args_id = self._protobuf.spec.transformed.arguments
         kwargs_id = self._protobuf.spec.transformed.named_arguments
 
         args_parents = [
-            cast(st.DataSpec, self.storage().referrable(uuid))
+            cast(
+                Union[st.DataSpec, st.Transform],
+                self.storage().referrable(uuid),
+            )
             for uuid in args_id
         ]
         kwargs_parents = {
-            name: cast(st.DataSpec, self.storage().referrable(uuid))
+            name: cast(
+                Union[st.DataSpec, st.Transform],
+                self.storage().referrable(uuid),
+            )
             for name, uuid in kwargs_id.items()
         }
 
         return args_parents, kwargs_parents
 
     def sources(
         self, type_name: t.Optional[str] = sp.type_name(sp.Dataset)
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/schema.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/size.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/size.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/statistics.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/statistics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/status.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/status.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/storage/local.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/storage/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/transform.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 
 import datetime
 import typing as t
 
-import numpy as np
-
 from sarus_data_spec.base import Referrable
 from sarus_data_spec.json_serialisation import SarusJSONEncoder
 from sarus_data_spec.path import straight_path
 import sarus_data_spec.dataset as sd
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
@@ -38,15 +36,17 @@
         return t.cast(str, self.protobuf().spec.WhichOneof('spec'))
 
     def is_external(self) -> bool:
         """Is the transform an external operation."""
         return self._protobuf.spec.HasField("external")
 
     def infer_output_type(
-        self, *arguments: st.DataSpec, **named_arguments: st.DataSpec
+        self,
+        *arguments: t.Union[st.DataSpec, st.Transform],
+        **named_arguments: t.Union[st.DataSpec, st.Transform],
     ) -> t.Tuple[str, t.Callable[[st.DataSpec], None]]:
         """Guess if the external transform output is a Dataset or a Scalar.
 
         Registers schema if it is a Dataset and returns the value type.
         """
         return self.manager().infer_output_type(
             self, *arguments, **named_arguments
@@ -74,14 +74,20 @@
                 for arg in arguments:
                     if arg not in self.visited:
                         arg.accept(self)
                 for name, arg in named_arguments.items():
                     if arg not in self.visited:
                         arg.accept(self)
 
+            def other(self, visited: st.Transform) -> None:
+                raise ValueError(
+                    "A composed transform can only have Variables "
+                    "or Composed ancestors."
+                )
+
         visitor = Transforms()
         self.accept(visitor)
         return visitor.visited
 
     def variables(self) -> t.Set[st.Transform]:
         """Return all the variables from a composed transform"""
         return {
@@ -98,23 +104,19 @@
         class Compose(st.TransformVisitor):
             visited: t.Set[st.Transform] = set()
             result: st.Transform
 
             def variable(
                 self,
                 visited: st.Transform,
-                position_name: t.Union[int, str] = 0,
+                name: str,
+                position: int,
             ) -> None:
                 self.result = visited
-                if isinstance(position_name, int):
-                    if position_name < len(compose_arguments):
-                        self.result = compose_arguments[position_name]
-                else:
-                    if position_name in compose_named_arguments:
-                        self.result = compose_named_arguments[position_name]
+                self.result = compose_named_arguments[name]
 
             def composed(
                 self,
                 visited: st.Transform,
                 transform: st.Transform,
                 *arguments: st.Transform,
                 **named_arguments: st.Transform,
@@ -156,22 +158,18 @@
         class Apply(st.TransformVisitor):
             visited: t.Dict[st.Transform, st.DataSpec] = {}
             result: st.DataSpec
 
             def variable(
                 self,
                 visited: st.Transform,
-                position_name: t.Union[int, str] = 0,
+                name: str,
+                position: int,
             ) -> None:
-                if isinstance(position_name, int):
-                    if position_name < len(apply_arguments):
-                        self.result = apply_arguments[position_name]
-                else:
-                    if position_name in apply_named_arguments:
-                        self.result = apply_named_arguments[position_name]
+                self.result = apply_named_arguments[name]
                 if self.result is None:
                     raise ValueError("Cannot substitute all variables")
 
             def composed(
                 self,
                 visited: st.Transform,
                 transform: st.Transform,
@@ -212,62 +210,67 @@
 
         visitor = Apply()
         self.accept(visitor)
         return visitor.result
 
     def abstract(
         self,
-        *arguments: t.Union[int, str],
-        **named_arguments: t.Union[int, str],
+        *arguments: str,
+        **named_arguments: str,
     ) -> st.Transform:
         return composed(
             self,
-            *(variable(position_name=arg) for arg in arguments),
+            *(variable(name=arg) for arg in arguments),
             **{
-                name: variable(position_name=arg)
+                name: variable(name=arg)
                 for name, arg in named_arguments.items()
             },
         )
 
     def __call__(
         self,
         *arguments: t.Union[st.Transform, st.DataSpec, int, str],
         **named_arguments: t.Union[st.Transform, st.DataSpec, int, str],
     ) -> t.Union[st.Transform, st.DataSpec]:
         """Applies the transform to another element"""
-        all_transforms = True
-        all_datasets = True
-        all_variables = True
+        n_transforms = 0
+        n_datasets = 0
+        n_variables = 0
         for arg in arguments:
-            all_transforms = all_transforms and isinstance(arg, Transform)
-            all_datasets = all_datasets and (isinstance(arg, st.DataSpec))
-            all_variables = all_variables and (
-                isinstance(arg, int) or isinstance(arg, str)
-            )
+            n_transforms += int(isinstance(arg, Transform))
+            n_datasets += int(isinstance(arg, st.DataSpec))
+            n_variables += int(isinstance(arg, int) or isinstance(arg, str))
         for arg in named_arguments.values():
-            all_transforms = all_transforms and isinstance(arg, Transform)
-            all_datasets = all_datasets and (isinstance(arg, st.DataSpec))
-            all_variables = all_variables and (
-                isinstance(arg, int) or isinstance(arg, str)
-            )
-        if all_datasets:
+            n_transforms += int(isinstance(arg, Transform))
+            n_datasets += int(isinstance(arg, st.DataSpec))
+            n_variables += int(isinstance(arg, int) or isinstance(arg, str))
+
+        total = len(arguments) + len(named_arguments)
+        if total == 0:
+            # If no argument is passed, we consider that we should apply
             return self.apply(
                 *t.cast(t.Sequence[st.DataSpec], arguments),
                 **t.cast(t.Mapping[str, st.DataSpec], named_arguments),
             )
-        if all_transforms:
+        elif n_transforms == total:
             return self.compose(
                 *t.cast(t.Sequence[Transform], arguments),
                 **t.cast(t.Mapping[str, Transform], named_arguments),
             )
-        if all_variables:
+        elif n_variables == total:
             return self.abstract(
-                *t.cast(t.Sequence[t.Union[int, str]], arguments),
-                **t.cast(t.Mapping[str, t.Union[int, str]], named_arguments),
+                *t.cast(t.Sequence[str], arguments),
+                **t.cast(t.Mapping[str, str], named_arguments),
             )
+        elif n_transforms + n_datasets == total:
+            return self.apply(
+                *t.cast(t.Sequence[st.DataSpec], arguments),
+                **t.cast(t.Mapping[str, st.DataSpec], named_arguments),
+            )
+
         return self
 
     def __mul__(self, argument: st.Transform) -> st.Transform:
         return self.compose(argument)
 
     # A Visitor acceptor
     def accept(self, visitor: st.TransformVisitor) -> None:
@@ -290,114 +293,118 @@
                         Transform, self.storage().referrable(transform)
                     )
                     for name, transform in self._protobuf.spec.composed.named_arguments.items()  # noqa: E501
                 },
             )
         elif self.is_variable():
             var = self._protobuf.spec.variable
-            if var.position == np.iinfo(np.int32).min32:  # type:ignore
-                visitor.variable(self, position_name=var.name)
-            else:
-                visitor.variable(self, position_name=var.position)
+            visitor.variable(self, name=var.name, position=var.position)
         else:
             visitor.other(self)
 
     def dot(self) -> str:
         """return a graphviz representation of the transform"""
 
         class Dot(st.TransformVisitor):
             visited: t.Set[st.Transform] = set()
             nodes: t.Dict[str, str] = {}
             edges: t.Set[t.Tuple[str, str]] = set()
 
             def variable(
                 self,
                 visited: st.Transform,
-                position_name: t.Union[int, str] = 0,
+                name: str,
+                position: int,
             ) -> None:
-                self.nodes[visited.uuid()] = str(position_name)
+                self.nodes[visited.uuid()] = f"{name} ({position})"
 
             def composed(
                 self,
                 visited: st.Transform,
                 transform: st.Transform,
                 *arguments: st.Transform,
                 **named_arguments: st.Transform,
             ) -> None:
                 if visited not in self.visited:
                     transform.accept(self)
+                    self.nodes[visited.uuid()] = transform.name()
                     for argument in arguments:
-                        if argument.is_composed():
-                            self.edges.add(
-                                (
-                                    argument.protobuf().spec.composed.transform,  # noqa: E501
-                                    transform.uuid(),
-                                )
-                            )
-                        else:
-                            self.edges.add((argument.uuid(), transform.uuid()))
+                        self.edges.add((argument.uuid(), visited.uuid()))
                         argument.accept(self)
                     for _, argument in named_arguments.items():
-                        if argument.is_composed():
-                            self.edges.add(
-                                (
-                                    argument.protobuf().spec.composed.transform,  # noqa: E501
-                                    transform.uuid(),
-                                )
-                            )
-                        else:
-                            self.edges.add((argument.uuid(), transform.uuid()))
+                        self.edges.add((argument.uuid(), visited.uuid()))
                         argument.accept(self)
                     self.visited.add(visited)
 
             def other(self, visited: st.Transform) -> None:
-                self.nodes[visited.uuid()] = visited.name()
+                pass
 
         visitor = Dot()
         self.accept(visitor)
         result = 'digraph {'
         for uuid, label in visitor.nodes.items():
             result += f'\n"{uuid}" [label="{label} ({uuid[:2]})"];'
         for u1, u2 in visitor.edges:
             result += f'\n"{u1}" -> "{u2}";'
         result += '}'
         return result
 
+    def transform_to_apply(self) -> st.Transform:
+        """Return the transform of a composed transform."""
+        assert self.is_composed()
+        uuid = self.protobuf().spec.composed.transform
+        return t.cast(st.Transform, self.storage().referrable(uuid))
+
+    def composed_parents(
+        self,
+    ) -> t.Tuple[t.List[st.Transform], t.Dict[str, st.Transform]]:
+        """Return the parents of a composed transform."""
+        assert self.is_composed()
+
+        args_id = self._protobuf.spec.composed.arguments
+        kwargs_id = self._protobuf.spec.composed.named_arguments
+
+        args_parents = [
+            t.cast(st.Transform, self.storage().referrable(uuid))
+            for uuid in args_id
+        ]
+        kwargs_parents = {
+            name: t.cast(st.Transform, self.storage().referrable(uuid))
+            for name, uuid in kwargs_id.items()
+        }
+        return args_parents, kwargs_parents
+
+    def composed_callable(self) -> t.Callable[..., t.Any]:
+        """Return the composed transform's equivalent callable.
+
+        The function takes an undefined number of named arguments.
+        """
+        return self.manager().composed_callable(self)
+
 
 # Builders
 def identity() -> Transform:
     return Transform(
         sp.Transform(
             name='Identity',
             spec=sp.Transform.Spec(identity=sp.Transform.Identity()),
             inversible=True,
             schema_preserving=True,
         )
     )
 
 
-def variable(position_name: t.Union[int, str] = 0) -> Transform:
-    if isinstance(position_name, int):
-        return Transform(
-            sp.Transform(
-                name='Variable',
-                spec=sp.Transform.Spec(
-                    variable=sp.Transform.Variable(position=position_name)
-                ),
-                inversible=True,
-                schema_preserving=True,
-            )
-        )
+def variable(name: str, position: int = 0) -> Transform:
     return Transform(
         sp.Transform(
             name='Variable',
             spec=sp.Transform.Spec(
                 variable=sp.Transform.Variable(
-                    name=position_name,
-                    position=np.iinfo(np.int32).min32,  # type:ignore
+                    name=name,
+                    position=position,
                 )
             ),
             inversible=True,
             schema_preserving=True,
         )
     )
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/type.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/typing.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,18 @@
         ...
 
 
 @t.runtime_checkable
 class DataSpec(Referring[DS], t.Protocol):
     def parents(
         self,
-    ) -> t.Tuple[t.List[DataSpec[DS]], t.Dict[str, DataSpec[DS]]]:
+    ) -> t.Tuple[
+        t.List[t.Union[DataSpec[DS], Transform]],
+        t.Dict[str, t.Union[DataSpec[DS], Transform]],
+    ]:
         ...
 
     def variant(
         self,
         kind: ConstraintKind,
         public_context: t.Collection[str] = (),
         privacy_limit: t.Optional[PrivacyLimit] = None,
@@ -625,14 +628,15 @@
     def ready(self) -> None:
         ...
 
     def error(self) -> None:
         ...
 
 
+@t.runtime_checkable
 class Transform(Referrable[sp.Transform], t.Protocol):
     """A python abstract class to describe transforms"""
 
     def prototype(self) -> t.Type[sp.Transform]:
         """Return the type of the underlying protobuf."""
         ...
 
@@ -654,15 +658,17 @@
         ...
 
     def is_external(self) -> bool:
         """Is the transform an external operation."""
         ...
 
     def infer_output_type(
-        self, *arguments: DataSpec, **named_arguments: DataSpec
+        self,
+        *arguments: t.Union[DataSpec, Transform],
+        **named_arguments: t.Union[DataSpec, Transform],
     ) -> t.Tuple[str, t.Callable[[DataSpec], None]]:
         """Guess if the external transform output is a Dataset or a Scalar.
 
         Registers schema if it is a Dataset and returns the value type.
         """
         ...
 
@@ -686,16 +692,16 @@
         *apply_arguments: DataSpec,
         **apply_named_arguments: DataSpec,
     ) -> DataSpec:
         ...
 
     def abstract(
         self,
-        *arguments: t.Union[int, str],
-        **named_arguments: t.Union[int, str],
+        *arguments: str,
+        **named_arguments: str,
     ) -> Transform:
         ...
 
     def __call__(
         self,
         *arguments: t.Union[Transform, DataSpec, int, str],
         **named_arguments: t.Union[Transform, DataSpec, int, str],
@@ -705,14 +711,28 @@
 
     def __mul__(self, argument: Transform) -> Transform:
         ...
 
     def accept(self, visitor: TransformVisitor) -> None:
         ...
 
+    def transform_to_apply(self) -> Transform:
+        """Return the transform of a composed transform."""
+
+    def composed_parents(
+        self,
+    ) -> t.Tuple[t.List[Transform], t.Dict[str, Transform]]:
+        """Return the parents of a composed transform."""
+
+    def composed_callable(self) -> t.Callable[..., t.Any]:
+        """Return the composed transform's equivalent callable.
+
+        The function takes an undefined number of named arguments.
+        """
+
 
 class TransformVisitor(t.Protocol):
     """A visitor class for Transform"""
 
     def all(self, visited: Transform) -> None:
         ...
 
@@ -724,15 +744,16 @@
         **named_arguments: Transform,
     ) -> None:
         ...
 
     def variable(
         self,
         visited: Transform,
-        position_name: t.Union[int, str] = 0,
+        name: str,
+        position: int,
     ) -> None:
         ...
 
     def other(self, visited: Transform) -> None:
         ...
```

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-3.5.1/sarus_data_spec/variant_constraint.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/setup.cfg` & `sarus_data_spec_public-3.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.0/setup.py` & `sarus_data_spec_public-3.5.1/setup.py`

 * *Files identical despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == '__main__':
-    setup(version='3.5.0')
+    setup(version='3.5.1')
```

