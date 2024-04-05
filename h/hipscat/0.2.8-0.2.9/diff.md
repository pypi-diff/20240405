# Comparing `tmp/hipscat-0.2.8.tar.gz` & `tmp/hipscat-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipscat-0.2.8.tar", last modified: Thu Mar 14 15:24:10 2024, max compression
+gzip compressed data, was "hipscat-0.2.9.tar", last modified: Thu Mar 21 15:25:58 2024, max compression
```

## Comparing `hipscat-0.2.8.tar` & `hipscat-0.2.9.tar`

### file list

```diff
@@ -1,304 +1,306 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.976182 hipscat-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-14 15:24:04.000000 hipscat-0.2.8/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-14 15:24:04.000000 hipscat-0.2.8/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-14 15:24:04.000000 hipscat-0.2.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.932182 hipscat-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.936182 hipscat-0.2.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.936182 hipscat-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/workflows/asv-main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/workflows/asv-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/workflows/asv-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/workflows/publish-benchmarks-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-14 15:24:04.000000 hipscat-0.2.8/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-14 15:24:04.000000 hipscat-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-03-14 15:24:04.000000 hipscat-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-14 15:24:04.000000 hipscat-0.2.8/.prepare_project.sh
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-14 15:24:04.000000 hipscat-0.2.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-14 15:24:04.000000 hipscat-0.2.8/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-14 15:24:04.000000 hipscat-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-03-14 15:24:10.976182 hipscat-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-14 15:24:04.000000 hipscat-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.936182 hipscat-0.2.8/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:04.000000 hipscat-0.2.8/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-03-14 15:24:04.000000 hipscat-0.2.8/benchmarks/asv.conf.json
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-03-14 15:24:04.000000 hipscat-0.2.8/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.936182 hipscat-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-14 15:24:04.000000 hipscat-0.2.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-14 15:24:04.000000 hipscat-0.2.8/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.936182 hipscat-0.2.8/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-03-14 15:24:04.000000 hipscat-0.2.8/docs/guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-14 15:24:04.000000 hipscat-0.2.8/docs/guide/directory_scheme.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-03-14 15:24:04.000000 hipscat-0.2.8/docs/guide/margin_cache_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-03-14 15:24:04.000000 hipscat-0.2.8/docs/guide/pixel_math.md
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-14 15:24:04.000000 hipscat-0.2.8/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.936182 hipscat-0.2.8/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-03-14 15:24:04.000000 hipscat-0.2.8/docs/notebooks/catalog_size_inspection.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-14 15:24:04.000000 hipscat-0.2.8/docs/notebooks/cone_search.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-14 15:24:04.000000 hipscat-0.2.8/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-14 15:24:04.000000 hipscat-0.2.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-14 15:24:04.000000 hipscat-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 15:24:10.976182 hipscat-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.940182 hipscat-0.2.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.940182 hipscat-0.2.8/src/hipscat/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-14 15:24:10.000000 hipscat-0.2.8/src/hipscat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.940182 hipscat-0.2.8/src/hipscat/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.940182 hipscat-0.2.8/src/hipscat/catalog/association_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/association_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/association_catalog/association_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/association_catalog/association_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/association_catalog/partition_join_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/catalog_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.940182 hipscat-0.2.8/src/hipscat/catalog/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/dataset/base_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/dataset/catalog_info_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.940182 hipscat-0.2.8/src/hipscat/catalog/healpix_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/healpix_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/healpix_dataset/healpix_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.944182 hipscat-0.2.8/src/hipscat/catalog/index/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/index/index_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/index/index_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.944182 hipscat-0.2.8/src/hipscat/catalog/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/margin_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/margin_cache/margin_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/partition_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.944182 hipscat-0.2.8/src/hipscat/catalog/source_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/source_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/catalog/source_catalog/source_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.944182 hipscat-0.2.8/src/hipscat/inspection/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/inspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/inspection/almanac.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/inspection/almanac_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/inspection/visualize_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.944182 hipscat-0.2.8/src/hipscat/io/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.944182 hipscat-0.2.8/src/hipscat/io/file_io/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/io/file_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/io/file_io/file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/io/file_io/file_pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/io/parquet_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/io/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/io/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/io/write_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.944182 hipscat-0.2.8/src/hipscat/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/loaders/read_from_hipscat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.948182 hipscat-0.2.8/src/hipscat/pixel_math/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_math/box_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_math/cone_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_math/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_math/healpix_pixel.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_math/healpix_pixel_convertor.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_math/healpix_pixel_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_math/hipscat_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_math/margin_bounding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_math/partition_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_math/pixel_margins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_math/polygon_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_math/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.948182 hipscat-0.2.8/src/hipscat/pixel_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11278 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_tree/pixel_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_tree/pixel_alignment_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_tree/pixel_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_tree/pixel_node_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_tree/pixel_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/pixel_tree/pixel_tree_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:04.000000 hipscat-0.2.8/src/hipscat/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.976182 hipscat-0.2.8/src/hipscat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-03-14 15:24:10.000000 hipscat-0.2.8/src/hipscat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-03-14 15:24:10.000000 hipscat-0.2.8/src/hipscat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 15:24:10.000000 hipscat-0.2.8/src/hipscat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-14 15:24:10.000000 hipscat-0.2.8/src/hipscat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-14 15:24:10.000000 hipscat-0.2.8/src/hipscat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.948182 hipscat-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20972 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.948182 hipscat-0.2.8/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.952182 hipscat-0.2.8/tests/data/almanac/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac/catalog.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac/dataset.yml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac/deprecated.yml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac/index_catalog.yml
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac/margin_cache.yml
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac/small_sky.yml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac/small_sky_order1.yml
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac/small_sky_source_catalog.yml
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac/small_sky_to_small_sky_order1.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.952182 hipscat-0.2.8/tests/data/almanac_exception/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac_exception/association_missing_join.yml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac_exception/association_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac_exception/bad_catalog_path.yml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac_exception/bad_primary_path.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac_exception/bad_type.yml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac_exception/index_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac_exception/margin_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/almanac_exception/standalone_source_catalog.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10017 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/generate_data.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.928182 hipscat-0.2.8/tests/data/info_only/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.952182 hipscat-0.2.8/tests/data/info_only/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/info_only/catalog/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.952182 hipscat-0.2.8/tests/data/info_only/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/info_only/dataset/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.952182 hipscat-0.2.8/tests/data/info_only/index_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/info_only/index_catalog/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.952182 hipscat-0.2.8/tests/data/info_only/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/info_only/margin_cache/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.956182 hipscat-0.2.8/tests/data/small_sky/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.928182 hipscat-0.2.8/tests/data/small_sky/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.956182 hipscat-0.2.8/tests/data/small_sky/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.956182 hipscat-0.2.8/tests/data/small_sky_order1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.928182 hipscat-0.2.8/tests/data/small_sky_order1/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.956182 hipscat-0.2.8/tests/data/small_sky_order1/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.956182 hipscat-0.2.8/tests/data/small_sky_order1_id_index/
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_id_index/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_id_index/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_id_index/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.960182 hipscat-0.2.8/tests/data/small_sky_order1_id_index/index/
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_id_index/index/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_id_index/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.960182 hipscat-0.2.8/tests/data/small_sky_order1_margin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.928182 hipscat-0.2.8/tests/data/small_sky_order1_margin/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.960182 hipscat-0.2.8/tests/data/small_sky_order1_margin/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.928182 hipscat-0.2.8/tests/data/small_sky_order1_margin/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.960182 hipscat-0.2.8/tests/data/small_sky_order1_margin/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_margin/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_margin/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_margin/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_margin/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_margin/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_order1_margin/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.964182 hipscat-0.2.8/tests/data/small_sky_source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.928182 hipscat-0.2.8/tests/data/small_sky_source/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.964182 hipscat-0.2.8/tests/data/small_sky_source/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.928182 hipscat-0.2.8/tests/data/small_sky_source/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.964182 hipscat-0.2.8/tests/data/small_sky_source/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.928182 hipscat-0.2.8/tests/data/small_sky_source/Norder=2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.968182 hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.968182 hipscat-0.2.8/tests/data/small_sky_source_object_index/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source_object_index/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source_object_index/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source_object_index/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source_object_index/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.968182 hipscat-0.2.8/tests/data/small_sky_source_object_index/index/
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source_object_index/index/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_source_object_index/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.968182 hipscat-0.2.8/tests/data/small_sky_to_small_sky_order1/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_to_small_sky_order1/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_to_small_sky_order1/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_to_small_sky_order1/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_to_small_sky_order1/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/data/small_sky_to_small_sky_order1/partition_join_info.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.968182 hipscat-0.2.8/tests/hipscat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.968182 hipscat-0.2.8/tests/hipscat/catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.968182 hipscat-0.2.8/tests/hipscat/catalog/association_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/association_catalog/test_association_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/association_catalog/test_partition_join_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.968182 hipscat-0.2.8/tests/hipscat/catalog/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/dataset/test_base_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/dataset/test_catalog_info_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/dataset/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.968182 hipscat-0.2.8/tests/hipscat/catalog/index/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/index/test_index_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/index/test_index_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.972182 hipscat-0.2.8/tests/hipscat/catalog/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/loaders/test_read_from_hipscat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.972182 hipscat-0.2.8/tests/hipscat/catalog/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/margin_cache/test_margin_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.972182 hipscat-0.2.8/tests/hipscat/catalog/source_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    23031 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/test_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/catalog/test_partition_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.972182 hipscat-0.2.8/tests/hipscat/inspection/
--rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/inspection/test_almanac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/inspection/test_almanac_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/inspection/test_visualize_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.972182 hipscat-0.2.8/tests/hipscat/io/
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/io/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.972182 hipscat-0.2.8/tests/hipscat/io/file_io/
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/io/file_io/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/io/file_io/test_file_pointers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/io/test_parquet_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/io/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/io/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/io/test_write_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.972182 hipscat-0.2.8/tests/hipscat/pixel_math/
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/pixel_math/test_healpix_pixel.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/pixel_math/test_healpix_pixel_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/pixel_math/test_hipscat_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/pixel_math/test_margin_bounding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/pixel_math/test_partition_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/pixel_math/test_pixel_margins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:24:10.976182 hipscat-0.2.8/tests/hipscat/pixel_tree/
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/pixel_tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/pixel_tree/test_pixel_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/pixel_tree/test_pixel_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/pixel_tree/test_pixel_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-03-14 15:24:04.000000 hipscat-0.2.8/tests/hipscat/pixel_tree/test_pixel_tree_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.865040 hipscat-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-21 15:25:51.000000 hipscat-0.2.9/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-21 15:25:51.000000 hipscat-0.2.9/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-21 15:25:51.000000 hipscat-0.2.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.821040 hipscat-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.821040 hipscat-0.2.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.821040 hipscat-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/workflows/asv-main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/workflows/asv-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/workflows/asv-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/workflows/publish-benchmarks-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-21 15:25:51.000000 hipscat-0.2.9/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-21 15:25:51.000000 hipscat-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-03-21 15:25:51.000000 hipscat-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-21 15:25:51.000000 hipscat-0.2.9/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-21 15:25:51.000000 hipscat-0.2.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-21 15:25:51.000000 hipscat-0.2.9/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-21 15:25:51.000000 hipscat-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-03-21 15:25:58.861040 hipscat-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-21 15:25:51.000000 hipscat-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.825039 hipscat-0.2.9/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:51.000000 hipscat-0.2.9/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-03-21 15:25:51.000000 hipscat-0.2.9/benchmarks/asv.conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-03-21 15:25:51.000000 hipscat-0.2.9/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.825039 hipscat-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-21 15:25:51.000000 hipscat-0.2.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.825039 hipscat-0.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-21 15:25:51.000000 hipscat-0.2.9/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-03-21 15:25:51.000000 hipscat-0.2.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.825039 hipscat-0.2.9/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-03-21 15:25:51.000000 hipscat-0.2.9/docs/guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-21 15:25:51.000000 hipscat-0.2.9/docs/guide/directory_scheme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-03-21 15:25:51.000000 hipscat-0.2.9/docs/guide/margin_cache_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-03-21 15:25:51.000000 hipscat-0.2.9/docs/guide/pixel_math.md
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-21 15:25:51.000000 hipscat-0.2.9/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.825039 hipscat-0.2.9/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-03-21 15:25:51.000000 hipscat-0.2.9/docs/notebooks/catalog_size_inspection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-21 15:25:51.000000 hipscat-0.2.9/docs/notebooks/cone_search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-21 15:25:51.000000 hipscat-0.2.9/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-21 15:25:51.000000 hipscat-0.2.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-21 15:25:51.000000 hipscat-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 15:25:58.865040 hipscat-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.825039 hipscat-0.2.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.825039 hipscat-0.2.9/src/hipscat/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-21 15:25:58.000000 hipscat-0.2.9/src/hipscat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.829039 hipscat-0.2.9/src/hipscat/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.829039 hipscat-0.2.9/src/hipscat/catalog/association_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/association_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/association_catalog/association_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/association_catalog/association_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/association_catalog/partition_join_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/catalog_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.829039 hipscat-0.2.9/src/hipscat/catalog/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/dataset/base_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/dataset/catalog_info_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.829039 hipscat-0.2.9/src/hipscat/catalog/healpix_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/healpix_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/healpix_dataset/healpix_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.829039 hipscat-0.2.9/src/hipscat/catalog/index/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/index/index_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/index/index_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.829039 hipscat-0.2.9/src/hipscat/catalog/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/margin_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/margin_cache/margin_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/partition_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.829039 hipscat-0.2.9/src/hipscat/catalog/source_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/source_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/catalog/source_catalog/source_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.833040 hipscat-0.2.9/src/hipscat/inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/inspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/inspection/almanac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/inspection/almanac_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/inspection/visualize_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.833040 hipscat-0.2.9/src/hipscat/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.833040 hipscat-0.2.9/src/hipscat/io/file_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/io/file_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/io/file_io/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/io/file_io/file_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/io/parquet_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/io/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/io/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/io/write_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.833040 hipscat-0.2.9/src/hipscat/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/loaders/read_from_hipscat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.837040 hipscat-0.2.9/src/hipscat/pixel_math/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_math/box_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_math/cone_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_math/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_math/healpix_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_math/healpix_pixel_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_math/healpix_pixel_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_math/hipscat_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_math/margin_bounding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_math/partition_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_math/pixel_margins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_math/polygon_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_math/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.837040 hipscat-0.2.9/src/hipscat/pixel_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11278 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_tree/pixel_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_tree/pixel_alignment_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_tree/pixel_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_tree/pixel_node_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_tree/pixel_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/pixel_tree/pixel_tree_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:51.000000 hipscat-0.2.9/src/hipscat/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.861040 hipscat-0.2.9/src/hipscat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-03-21 15:25:58.000000 hipscat-0.2.9/src/hipscat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-03-21 15:25:58.000000 hipscat-0.2.9/src/hipscat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 15:25:58.000000 hipscat-0.2.9/src/hipscat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-21 15:25:58.000000 hipscat-0.2.9/src/hipscat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-21 15:25:58.000000 hipscat-0.2.9/src/hipscat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.837040 hipscat-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20972 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.837040 hipscat-0.2.9/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.837040 hipscat-0.2.9/tests/data/almanac/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac/catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac/dataset.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac/deprecated.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac/index_catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac/margin_cache.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac/small_sky.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac/small_sky_order1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac/small_sky_source_catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac/small_sky_to_small_sky_order1.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.841040 hipscat-0.2.9/tests/data/almanac_exception/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac_exception/association_missing_join.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac_exception/association_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac_exception/bad_catalog_path.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac_exception/bad_primary_path.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac_exception/bad_type.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac_exception/index_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac_exception/margin_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/almanac_exception/standalone_source_catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10017 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/generate_data.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.813039 hipscat-0.2.9/tests/data/info_only/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.841040 hipscat-0.2.9/tests/data/info_only/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/info_only/catalog/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.841040 hipscat-0.2.9/tests/data/info_only/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/info_only/dataset/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.841040 hipscat-0.2.9/tests/data/info_only/index_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/info_only/index_catalog/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.841040 hipscat-0.2.9/tests/data/info_only/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/info_only/margin_cache/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.841040 hipscat-0.2.9/tests/data/small_sky/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.813039 hipscat-0.2.9/tests/data/small_sky/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.841040 hipscat-0.2.9/tests/data/small_sky/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.845040 hipscat-0.2.9/tests/data/small_sky_order1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.813039 hipscat-0.2.9/tests/data/small_sky_order1/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.845040 hipscat-0.2.9/tests/data/small_sky_order1/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.845040 hipscat-0.2.9/tests/data/small_sky_order1_id_index/
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_id_index/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_id_index/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_id_index/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.845040 hipscat-0.2.9/tests/data/small_sky_order1_id_index/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_id_index/index/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_id_index/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.845040 hipscat-0.2.9/tests/data/small_sky_order1_margin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.813039 hipscat-0.2.9/tests/data/small_sky_order1_margin/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.845040 hipscat-0.2.9/tests/data/small_sky_order1_margin/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.817039 hipscat-0.2.9/tests/data/small_sky_order1_margin/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.849040 hipscat-0.2.9/tests/data/small_sky_order1_margin/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_margin/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_margin/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_margin/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_margin/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_margin/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_order1_margin/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.849040 hipscat-0.2.9/tests/data/small_sky_source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.817039 hipscat-0.2.9/tests/data/small_sky_source/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.849040 hipscat-0.2.9/tests/data/small_sky_source/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.817039 hipscat-0.2.9/tests/data/small_sky_source/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.849040 hipscat-0.2.9/tests/data/small_sky_source/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.817039 hipscat-0.2.9/tests/data/small_sky_source/Norder=2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.853040 hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.853040 hipscat-0.2.9/tests/data/small_sky_source_object_index/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source_object_index/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source_object_index/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source_object_index/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source_object_index/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.853040 hipscat-0.2.9/tests/data/small_sky_source_object_index/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source_object_index/index/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_source_object_index/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.857040 hipscat-0.2.9/tests/data/small_sky_to_small_sky_order1/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_to_small_sky_order1/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_to_small_sky_order1/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_to_small_sky_order1/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_to_small_sky_order1/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/data/small_sky_to_small_sky_order1/partition_join_info.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.857040 hipscat-0.2.9/tests/hipscat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.857040 hipscat-0.2.9/tests/hipscat/catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.857040 hipscat-0.2.9/tests/hipscat/catalog/association_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/association_catalog/test_association_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/association_catalog/test_partition_join_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.857040 hipscat-0.2.9/tests/hipscat/catalog/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/dataset/test_base_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/dataset/test_catalog_info_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/dataset/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.857040 hipscat-0.2.9/tests/hipscat/catalog/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/index/test_index_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/index/test_index_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.857040 hipscat-0.2.9/tests/hipscat/catalog/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/loaders/test_read_from_hipscat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.857040 hipscat-0.2.9/tests/hipscat/catalog/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/margin_cache/test_margin_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.857040 hipscat-0.2.9/tests/hipscat/catalog/source_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23031 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/test_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/catalog/test_partition_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.857040 hipscat-0.2.9/tests/hipscat/inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/inspection/test_almanac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/inspection/test_almanac_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/inspection/test_visualize_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.861040 hipscat-0.2.9/tests/hipscat/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/io/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.861040 hipscat-0.2.9/tests/hipscat/io/file_io/
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/io/file_io/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/io/file_io/test_file_pointers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/io/test_parquet_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/io/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/io/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/io/test_write_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.861040 hipscat-0.2.9/tests/hipscat/pixel_math/
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/pixel_math/test_healpix_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/pixel_math/test_healpix_pixel_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/pixel_math/test_hipscat_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/pixel_math/test_margin_bounding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/pixel_math/test_partition_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/pixel_math/test_pixel_margins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:25:58.861040 hipscat-0.2.9/tests/hipscat/pixel_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/pixel_tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/pixel_tree/test_pixel_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/pixel_tree/test_pixel_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/pixel_tree/test_pixel_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-03-21 15:25:51.000000 hipscat-0.2.9/tests/hipscat/pixel_tree/test_pixel_tree_builder.py
```

### Comparing `hipscat-0.2.8/.copier-answers.yml` & `hipscat-0.2.9/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.gitattributes` & `hipscat-0.2.9/.gitattributes`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.github/ISSUE_TEMPLATE/1-bug_report.md` & `hipscat-0.2.9/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.github/ISSUE_TEMPLATE/2-feature_request.md` & `hipscat-0.2.9/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.github/pull_request_template.md` & `hipscat-0.2.9/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.github/workflows/asv-main.yml` & `hipscat-0.2.9/.github/workflows/asv-main.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.github/workflows/asv-nightly.yml` & `hipscat-0.2.9/.github/workflows/asv-nightly.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.github/workflows/asv-pr.yml` & `hipscat-0.2.9/.github/workflows/asv-pr.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.github/workflows/build-documentation.yml` & `hipscat-0.2.9/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.github/workflows/pre-commit-ci.yml` & `hipscat-0.2.9/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.github/workflows/publish-benchmarks-pr.yml` & `hipscat-0.2.9/.github/workflows/publish-benchmarks-pr.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.github/workflows/publish-to-pypi.yml` & `hipscat-0.2.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.github/workflows/smoke-test.yml` & `hipscat-0.2.9/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.github/workflows/testing-and-coverage.yml` & `hipscat-0.2.9/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.gitignore` & `hipscat-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.pre-commit-config.yaml` & `hipscat-0.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.prepare_project.sh` & `hipscat-0.2.9/.prepare_project.sh`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/.setup_dev.sh` & `hipscat-0.2.9/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/LICENSE` & `hipscat-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/PKG-INFO` & `hipscat-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat
-Version: 0.2.8
+Version: 0.2.9
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `hipscat-0.2.8/README.md` & `hipscat-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/benchmarks/asv.conf.json` & `hipscat-0.2.9/benchmarks/asv.conf.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/benchmarks/benchmarks.py` & `hipscat-0.2.9/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/docs/Makefile` & `hipscat-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/docs/conf.py` & `hipscat-0.2.9/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,8 +52,11 @@
 
 autoapi_type = "python"
 autoapi_dirs = ["../src"]
 autoapi_ignore = ["*/__main__.py", "*/_version.py"]
 autoapi_add_toc_tree_entry = False
 autoapi_member_order = "bysource"
 
-html_theme = "sphinx_rtd_theme"
+html_theme = "sphinx_book_theme"
+
+html_static_path = ["_static"]
+html_css_files = ["custom.css"]
```

### Comparing `hipscat-0.2.8/docs/guide/contributing.rst` & `hipscat-0.2.9/docs/guide/contributing.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/docs/guide/directory_scheme.rst` & `hipscat-0.2.9/docs/guide/directory_scheme.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/docs/guide/margin_cache_diagram.png` & `hipscat-0.2.9/docs/guide/margin_cache_diagram.png`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/docs/guide/pixel_math.md` & `hipscat-0.2.9/docs/guide/pixel_math.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/docs/notebooks/catalog_size_inspection.ipynb` & `hipscat-0.2.9/docs/notebooks/catalog_size_inspection.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/docs/notebooks/cone_search.ipynb` & `hipscat-0.2.9/docs/notebooks/cone_search.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/pyproject.toml` & `hipscat-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/.pylintrc` & `hipscat-0.2.9/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/catalog/association_catalog/association_catalog.py` & `hipscat-0.2.9/src/hipscat/catalog/association_catalog/association_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/catalog/association_catalog/association_catalog_info.py` & `hipscat-0.2.9/src/hipscat/catalog/association_catalog/association_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/catalog/association_catalog/partition_join_info.py` & `hipscat-0.2.9/src/hipscat/catalog/association_catalog/partition_join_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/catalog/catalog.py` & `hipscat-0.2.9/src/hipscat/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/catalog/catalog_info.py` & `hipscat-0.2.9/src/hipscat/catalog/catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/catalog/dataset/base_catalog_info.py` & `hipscat-0.2.9/src/hipscat/catalog/dataset/base_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/catalog/dataset/catalog_info_factory.py` & `hipscat-0.2.9/src/hipscat/catalog/dataset/catalog_info_factory.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/catalog/dataset/dataset.py` & `hipscat-0.2.9/src/hipscat/catalog/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/catalog/healpix_dataset/healpix_dataset.py` & `hipscat-0.2.9/src/hipscat/catalog/healpix_dataset/healpix_dataset.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/catalog/index/index_catalog.py` & `hipscat-0.2.9/src/hipscat/catalog/index/index_catalog.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pyarrow.compute as pc
 import pyarrow.dataset as pds
 from typing_extensions import TypeAlias
 
 from hipscat.catalog.dataset import Dataset
 from hipscat.catalog.index import IndexCatalogInfo
 from hipscat.io import paths
+from hipscat.io.file_io.file_pointer import get_fs, strip_leading_slash_for_pyarrow
 from hipscat.pixel_math import HealpixPixel
 from hipscat.pixel_math.healpix_pixel_function import get_pixel_argsort
 
 
 class IndexCatalog(Dataset):
     """An index into HiPSCat Catalog for enabling fast lookups on non-spatial values.
 
@@ -27,15 +28,20 @@
         Args:
             ids: the values of the indexing column (e.g. 87,543)
         Returns:
             partitions of leaf parquet files in the primary catalog
             that may contain rows for the id values
         """
         metadata_file = paths.get_parquet_metadata_pointer(self.catalog_base_dir)
-        dataset = pds.parquet_dataset(metadata_file)
+        file_system, metadata_file = get_fs(file_pointer=metadata_file, storage_options=self.storage_options)
+
+        # pyarrow.dataset requires the pointer not lead with a slash
+        metadata_file = strip_leading_slash_for_pyarrow(metadata_file, file_system.protocol)
+
+        dataset = pds.parquet_dataset(metadata_file, filesystem=file_system)
 
         # There's a lot happening in a few pyarrow dataset methods:
         # We create a simple pyarrow expression that roughly corresponds to a SQL statement like
         #   WHERE id_column IN (<ids>)
         # We stay in pyarrow to group by Norder/Npix to aggregate the results unique values.
         # After that convert into pandas, as this handles the integer type conversions
         # (uint8 and uint64 aren't always friendly between pyarrow and the rest of python),
```

### Comparing `hipscat-0.2.8/src/hipscat/catalog/index/index_catalog_info.py` & `hipscat-0.2.9/src/hipscat/catalog/index/index_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py` & `hipscat-0.2.9/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/catalog/margin_cache/margin_catalog.py` & `hipscat-0.2.9/src/hipscat/catalog/margin_cache/margin_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/catalog/partition_info.py` & `hipscat-0.2.9/src/hipscat/catalog/partition_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/catalog/source_catalog/source_catalog_info.py` & `hipscat-0.2.9/src/hipscat/catalog/source_catalog/source_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/inspection/almanac.py` & `hipscat-0.2.9/src/hipscat/inspection/almanac.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/inspection/almanac_info.py` & `hipscat-0.2.9/src/hipscat/inspection/almanac_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/inspection/visualize_catalog.py` & `hipscat-0.2.9/src/hipscat/inspection/visualize_catalog.py`

 * *Files 17% similar despite different names*

```diff
@@ -99,29 +99,46 @@
                 (pixel.pixel + 1) * explosion_factor,
             )
         ]
         order_map[exploded_pixels] = pixel.order
     _plot_healpix_map(order_map, projection, plot_title, cmap=cmap, **kwargs)
 
 
-def _plot_healpix_map(healpix_map, projection, title, cmap="viridis", **kwargs):
-    """Perform the plotting of a healpix pixel map.
+def get_projection_method(projection):
+    """Get the healpy plotting method for a specified projection string
 
     Args:
-        healpix_map: array containing the map
-        projection: projection type to display
-        title: title used in image plot
-        cmap: matplotlib colormap to use
+        projection (str):  The map projection to use. Valid values include:
+            - moll - Molleweide projection (default)
+            - gnom - Gnomonic projection
+            - cart - Cartesian projection
+            - orth - Orthographic projection
+
+    Returns:
+        The healpy method that plots a HEALPix map with the specified projection
     """
     if projection == "moll":
         projection_method = hp.mollview
     elif projection == "gnom":
         projection_method = hp.gnomview
     elif projection == "cart":
         projection_method = hp.cartview
     elif projection == "orth":
         projection_method = hp.orthview
     else:
         raise NotImplementedError(f"unknown projection: {projection}")
+    return projection_method
+
+
+def _plot_healpix_map(healpix_map, projection, title, cmap="viridis", **kwargs):
+    """Perform the plotting of a healpix pixel map.
+
+    Args:
+        healpix_map: array containing the map
+        projection: projection type to display
+        title: title used in image plot
+        cmap: matplotlib colormap to use
+    """
+    projection_method = get_projection_method(projection)
 
     projection_method(healpix_map, title=title, nest=True, cmap=cmap, **kwargs)
     plt.plot()
```

### Comparing `hipscat-0.2.8/src/hipscat/io/__init__.py` & `hipscat-0.2.9/src/hipscat/io/__init__.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/io/file_io/__init__.py` & `hipscat-0.2.9/src/hipscat/io/file_io/__init__.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/io/file_io/file_io.py` & `hipscat-0.2.9/src/hipscat/io/file_io/file_io.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/io/file_io/file_pointer.py` & `hipscat-0.2.9/src/hipscat/io/file_io/file_pointer.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/io/parquet_metadata.py` & `hipscat-0.2.9/src/hipscat/io/parquet_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/io/paths.py` & `hipscat-0.2.9/src/hipscat/io/paths.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/io/write_metadata.py` & `hipscat-0.2.9/src/hipscat/io/write_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/loaders/read_from_hipscat.py` & `hipscat-0.2.9/src/hipscat/loaders/read_from_hipscat.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     """
     catalog_type_to_use = (
         _read_dataset_class_from_metadata(catalog_path, storage_options=storage_options)
         if catalog_type is None
         else catalog_type
     )
     loader = _get_loader_from_catalog_type(catalog_type_to_use)
-    return loader.read_from_hipscat(catalog_path)
+    return loader.read_from_hipscat(catalog_path, storage_options=storage_options)
 
 
 def _read_dataset_class_from_metadata(
     catalog_base_path: str, storage_options: dict | None = None
 ) -> CatalogType:
     catalog_base_dir = io.file_io.get_file_pointer_from_path(catalog_base_path)
     catalog_info_path = io.paths.get_catalog_info_pointer(catalog_base_dir)
```

### Comparing `hipscat-0.2.8/src/hipscat/pixel_math/__init__.py` & `hipscat-0.2.9/src/hipscat/pixel_math/__init__.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_math/box_filter.py` & `hipscat-0.2.9/src/hipscat/pixel_math/box_filter.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_math/cone_filter.py` & `hipscat-0.2.9/src/hipscat/pixel_math/cone_filter.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_math/filter.py` & `hipscat-0.2.9/src/hipscat/pixel_math/filter.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_math/healpix_pixel.py` & `hipscat-0.2.9/src/hipscat/pixel_math/healpix_pixel.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_math/healpix_pixel_convertor.py` & `hipscat-0.2.9/src/hipscat/pixel_math/healpix_pixel_convertor.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_math/healpix_pixel_function.py` & `hipscat-0.2.9/src/hipscat/pixel_math/healpix_pixel_function.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_math/hipscat_id.py` & `hipscat-0.2.9/src/hipscat/pixel_math/hipscat_id.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_math/margin_bounding.py` & `hipscat-0.2.9/src/hipscat/pixel_math/margin_bounding.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_math/partition_stats.py` & `hipscat-0.2.9/src/hipscat/pixel_math/partition_stats.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_math/pixel_margins.py` & `hipscat-0.2.9/src/hipscat/pixel_math/pixel_margins.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_math/polygon_filter.py` & `hipscat-0.2.9/src/hipscat/pixel_math/polygon_filter.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_math/validators.py` & `hipscat-0.2.9/src/hipscat/pixel_math/validators.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_tree/pixel_alignment.py` & `hipscat-0.2.9/src/hipscat/pixel_tree/pixel_alignment.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_tree/pixel_node.py` & `hipscat-0.2.9/src/hipscat/pixel_tree/pixel_node.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_tree/pixel_tree.py` & `hipscat-0.2.9/src/hipscat/pixel_tree/pixel_tree.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat/pixel_tree/pixel_tree_builder.py` & `hipscat-0.2.9/src/hipscat/pixel_tree/pixel_tree_builder.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/src/hipscat.egg-info/PKG-INFO` & `hipscat-0.2.9/src/hipscat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat
-Version: 0.2.8
+Version: 0.2.9
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `hipscat-0.2.8/src/hipscat.egg-info/SOURCES.txt` & `hipscat-0.2.9/src/hipscat.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 benchmarks/asv.conf.json
 benchmarks/benchmarks.py
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/notebooks.rst
 docs/requirements.txt
+docs/_static/custom.css
 docs/guide/contributing.rst
 docs/guide/directory_scheme.rst
 docs/guide/margin_cache_diagram.png
 docs/guide/pixel_math.md
 docs/notebooks/catalog_size_inspection.ipynb
 docs/notebooks/cone_search.ipynb
 src/.pylintrc
```

### Comparing `hipscat-0.2.8/tests/.pylintrc` & `hipscat-0.2.9/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/conftest.py` & `hipscat-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/generate_data.ipynb` & `hipscat-0.2.9/tests/data/generate_data.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet` & `hipscat-0.2.9/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky/_common_metadata` & `hipscat-0.2.9/tests/data/small_sky/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky/_metadata` & `hipscat-0.2.9/tests/data/small_sky/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky/point_map.fits` & `hipscat-0.2.9/tests/data/small_sky/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky/provenance_info.json` & `hipscat-0.2.9/tests/data/small_sky/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet` & `hipscat-0.2.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet` & `hipscat-0.2.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet` & `hipscat-0.2.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.2.9/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1/README.md` & `hipscat-0.2.9/tests/data/small_sky_order1/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1/_common_metadata` & `hipscat-0.2.9/tests/data/small_sky_order1/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1/_metadata` & `hipscat-0.2.9/tests/data/small_sky_order1/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1/point_map.fits` & `hipscat-0.2.9/tests/data/small_sky_order1/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1/provenance_info.json` & `hipscat-0.2.9/tests/data/small_sky_order1/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1_id_index/_common_metadata` & `hipscat-0.2.9/tests/data/small_sky_order1_id_index/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1_id_index/_metadata` & `hipscat-0.2.9/tests/data/small_sky_order1_id_index/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1_id_index/index/part.0.parquet` & `hipscat-0.2.9/tests/data/small_sky_order1_id_index/index/part.0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1_id_index/provenance_info.json` & `hipscat-0.2.9/tests/data/small_sky_order1_id_index/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet` & `hipscat-0.2.9/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet` & `hipscat-0.2.9/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet` & `hipscat-0.2.9/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet` & `hipscat-0.2.9/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.2.9/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1_margin/README.md` & `hipscat-0.2.9/tests/data/small_sky_order1_margin/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1_margin/_common_metadata` & `hipscat-0.2.9/tests/data/small_sky_order1_margin/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1_margin/_metadata` & `hipscat-0.2.9/tests/data/small_sky_order1_margin/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_order1_margin/provenance_info.json` & `hipscat-0.2.9/tests/data/small_sky_order1_margin/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet` & `hipscat-0.2.9/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.2.9/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet` & `hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet` & `hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet` & `hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet` & `hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet` & `hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet` & `hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet` & `hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet` & `hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet` & `hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet` & `hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet` & `hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet` & `hipscat-0.2.9/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/_common_metadata` & `hipscat-0.2.9/tests/data/small_sky_source/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/_metadata` & `hipscat-0.2.9/tests/data/small_sky_source/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/point_map.fits` & `hipscat-0.2.9/tests/data/small_sky_source/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source/provenance_info.json` & `hipscat-0.2.9/tests/data/small_sky_source/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source_object_index/README.md` & `hipscat-0.2.9/tests/data/small_sky_source_object_index/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source_object_index/_common_metadata` & `hipscat-0.2.9/tests/data/small_sky_source_object_index/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source_object_index/_metadata` & `hipscat-0.2.9/tests/data/small_sky_source_object_index/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source_object_index/index/part.0.parquet` & `hipscat-0.2.9/tests/data/small_sky_source_object_index/index/part.0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_source_object_index/provenance_info.json` & `hipscat-0.2.9/tests/data/small_sky_source_object_index/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_to_small_sky_order1/_common_metadata` & `hipscat-0.2.9/tests/data/small_sky_to_small_sky_order1/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/data/small_sky_to_small_sky_order1/_metadata` & `hipscat-0.2.9/tests/data/small_sky_to_small_sky_order1/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/catalog/association_catalog/test_association_catalog.py` & `hipscat-0.2.9/tests/hipscat/catalog/association_catalog/test_association_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py` & `hipscat-0.2.9/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/catalog/association_catalog/test_partition_join_info.py` & `hipscat-0.2.9/tests/hipscat/catalog/association_catalog/test_partition_join_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/catalog/dataset/test_base_catalog_info.py` & `hipscat-0.2.9/tests/hipscat/catalog/dataset/test_base_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/catalog/dataset/test_catalog_info_factory.py` & `hipscat-0.2.9/tests/hipscat/catalog/dataset/test_catalog_info_factory.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/catalog/dataset/test_dataset.py` & `hipscat-0.2.9/tests/hipscat/catalog/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/catalog/index/test_index_catalog.py` & `hipscat-0.2.9/tests/hipscat/catalog/index/test_index_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/catalog/index/test_index_catalog_info.py` & `hipscat-0.2.9/tests/hipscat/catalog/index/test_index_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py` & `hipscat-0.2.9/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/catalog/margin_cache/test_margin_catalog.py` & `hipscat-0.2.9/tests/hipscat/catalog/margin_cache/test_margin_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py` & `hipscat-0.2.9/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/catalog/test_catalog.py` & `hipscat-0.2.9/tests/hipscat/catalog/test_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/catalog/test_catalog_info.py` & `hipscat-0.2.9/tests/hipscat/catalog/test_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/catalog/test_partition_info.py` & `hipscat-0.2.9/tests/hipscat/catalog/test_partition_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/conftest.py` & `hipscat-0.2.9/tests/hipscat/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/inspection/test_almanac.py` & `hipscat-0.2.9/tests/hipscat/inspection/test_almanac.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/inspection/test_almanac_info.py` & `hipscat-0.2.9/tests/hipscat/inspection/test_almanac_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/inspection/test_visualize_catalog.py` & `hipscat-0.2.9/tests/hipscat/inspection/test_visualize_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/io/conftest.py` & `hipscat-0.2.9/tests/hipscat/io/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/io/file_io/test_file_io.py` & `hipscat-0.2.9/tests/hipscat/io/file_io/test_file_io.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/io/file_io/test_file_pointers.py` & `hipscat-0.2.9/tests/hipscat/io/file_io/test_file_pointers.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/io/test_parquet_metadata.py` & `hipscat-0.2.9/tests/hipscat/io/test_parquet_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/io/test_paths.py` & `hipscat-0.2.9/tests/hipscat/io/test_paths.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/io/test_validation.py` & `hipscat-0.2.9/tests/hipscat/io/test_validation.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/io/test_write_metadata.py` & `hipscat-0.2.9/tests/hipscat/io/test_write_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/pixel_math/test_healpix_pixel.py` & `hipscat-0.2.9/tests/hipscat/pixel_math/test_healpix_pixel.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py` & `hipscat-0.2.9/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/pixel_math/test_healpix_pixel_function.py` & `hipscat-0.2.9/tests/hipscat/pixel_math/test_healpix_pixel_function.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/pixel_math/test_hipscat_id.py` & `hipscat-0.2.9/tests/hipscat/pixel_math/test_hipscat_id.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/pixel_math/test_margin_bounding.py` & `hipscat-0.2.9/tests/hipscat/pixel_math/test_margin_bounding.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/pixel_math/test_partition_stats.py` & `hipscat-0.2.9/tests/hipscat/pixel_math/test_partition_stats.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/pixel_math/test_pixel_margins.py` & `hipscat-0.2.9/tests/hipscat/pixel_math/test_pixel_margins.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/pixel_tree/conftest.py` & `hipscat-0.2.9/tests/hipscat/pixel_tree/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/pixel_tree/test_pixel_alignment.py` & `hipscat-0.2.9/tests/hipscat/pixel_tree/test_pixel_alignment.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/pixel_tree/test_pixel_node.py` & `hipscat-0.2.9/tests/hipscat/pixel_tree/test_pixel_node.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/pixel_tree/test_pixel_tree.py` & `hipscat-0.2.9/tests/hipscat/pixel_tree/test_pixel_tree.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.2.8/tests/hipscat/pixel_tree/test_pixel_tree_builder.py` & `hipscat-0.2.9/tests/hipscat/pixel_tree/test_pixel_tree_builder.py`

 * *Files identical despite different names*

