# Comparing `tmp/bionty_base-0.37.1.tar.gz` & `tmp/bionty-base-0.37.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bionty_base-0.37.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bionty-base-0.37.2.tar", last modified: Fri Apr  5 12:56:37 2024, max compression
```

## Comparing `bionty_base-0.37.1.tar` & `bionty-base-0.37.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     3169 2024-03-27 07:46:53.421625 bionty_base-0.37.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      555 2024-02-05 06:48:01.378180 bionty_base-0.37.1/.github/workflows/check_ontologies_reachable.yml
--rw-r--r--   0        0        0      133 2024-02-05 06:48:01.378260 bionty_base-0.37.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-02-05 06:48:01.378348 bionty_base-0.37.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0      504 2024-02-05 06:48:01.378430 bionty_base-0.37.1/.github/workflows/update_ontologies.yml
--rw-r--r--   0        0        0     2115 2024-02-05 06:48:01.378514 bionty_base-0.37.1/.gitignore
--rw-r--r--   0        0        0     1512 2024-02-05 06:48:01.378597 bionty_base-0.37.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2024-02-05 06:48:01.378739 bionty_base-0.37.1/LICENSE
--rw-r--r--   0        0        0     3116 2024-02-05 16:15:26.529099 bionty_base-0.37.1/README.md
--rw-r--r--   0        0        0     1894 2024-03-27 07:47:17.342932 bionty_base-0.37.1/bionty_base/__init__.py
--rw-r--r--   0        0        0     1605 2024-02-05 06:48:01.379069 bionty_base-0.37.1/bionty_base/_display_sources.py
--rw-r--r--   0        0        0     3863 2024-02-05 06:48:01.379163 bionty_base-0.37.1/bionty_base/_ontology.py
--rw-r--r--   0        0        0    24162 2024-03-02 21:21:37.545675 bionty_base-0.37.1/bionty_base/_public_ontology.py
--rw-r--r--   0        0        0     2615 2024-02-05 06:48:01.379415 bionty_base-0.37.1/bionty_base/_settings.py
--rw-r--r--   0        0        0      524 2024-02-05 06:48:01.379500 bionty_base-0.37.1/bionty_base/_sync_sources.py
--rw-r--r--   0        0        0      111 2024-02-05 06:48:01.379634 bionty_base-0.37.1/bionty_base/dev/__init__.py
--rw-r--r--   0        0        0     8456 2024-03-27 07:46:53.422612 bionty_base-0.37.1/bionty_base/dev/_handle_sources.py
--rw-r--r--   0        0        0     5154 2024-03-27 07:46:53.423500 bionty_base-0.37.1/bionty_base/dev/_io.py
--rw-r--r--   0        0        0     1021 2024-02-05 06:48:01.380009 bionty_base-0.37.1/bionty_base/dev/_md5.py
--rw-r--r--   0        0        0        0 2024-02-05 06:48:01.380085 bionty_base-0.37.1/bionty_base/entities/__init__.py
--rw-r--r--   0        0        0     1370 2024-02-05 06:48:01.380177 bionty_base-0.37.1/bionty_base/entities/_bfxpipeline.py
--rw-r--r--   0        0        0      682 2024-02-05 06:48:01.380275 bionty_base-0.37.1/bionty_base/entities/_biosample.py
--rw-r--r--   0        0        0      804 2024-02-05 06:48:01.380385 bionty_base-0.37.1/bionty_base/entities/_cellline.py
--rw-r--r--   0        0        0      728 2024-02-05 06:48:01.380477 bionty_base-0.37.1/bionty_base/entities/_cellmarker.py
--rw-r--r--   0        0        0      817 2024-02-05 06:48:01.380571 bionty_base-0.37.1/bionty_base/entities/_celltype.py
--rw-r--r--   0        0        0      913 2024-02-05 06:48:01.380672 bionty_base-0.37.1/bionty_base/entities/_developmentalstage.py
--rw-r--r--   0        0        0     1164 2024-02-05 06:48:01.380762 bionty_base-0.37.1/bionty_base/entities/_disease.py
--rw-r--r--   0        0        0      810 2024-02-05 06:48:01.380840 bionty_base-0.37.1/bionty_base/entities/_drug.py
--rw-r--r--   0        0        0      831 2024-02-05 06:48:01.380920 bionty_base-0.37.1/bionty_base/entities/_ethnicity.py
--rw-r--r--   0        0        0     4387 2024-02-05 06:48:01.381066 bionty_base-0.37.1/bionty_base/entities/_experimentalfactor.py
--rw-r--r--   0        0        0    10086 2024-02-05 06:48:01.381189 bionty_base-0.37.1/bionty_base/entities/_gene.py
--rw-r--r--   0        0        0     2570 2024-02-05 06:48:01.381291 bionty_base-0.37.1/bionty_base/entities/_organism.py
--rw-r--r--   0        0        0      855 2024-02-05 06:48:01.381377 bionty_base-0.37.1/bionty_base/entities/_pathway.py
--rw-r--r--   0        0        0     1420 2024-02-05 06:48:01.381466 bionty_base-0.37.1/bionty_base/entities/_phenotype.py
--rw-r--r--   0        0        0      685 2024-02-05 06:48:01.381538 bionty_base-0.37.1/bionty_base/entities/_protein.py
--rw-r--r--   0        0        0     1486 2024-02-05 06:48:01.381623 bionty_base-0.37.1/bionty_base/entities/_shared_docstrings.py
--rw-r--r--   0        0        0      799 2024-02-05 06:48:01.381715 bionty_base-0.37.1/bionty_base/entities/_tissue.py
--rw-r--r--   0        0        0    10926 2024-02-05 06:48:01.381901 bionty_base-0.37.1/bionty_base/sources/sources.yaml
--rw-r--r--   0        0        0    47342 2024-03-27 07:47:11.904391 bionty_base-0.37.1/docs/changelog.md
--rw-r--r--   0        0        0     1015 2024-02-05 06:48:01.382428 bionty_base-0.37.1/docs/developer/updating_source.md
--rw-r--r--   0        0        0      200 2024-02-05 06:48:01.382533 bionty_base-0.37.1/docs/guide.md
--rw-r--r--   0        0        0     3335 2024-02-05 06:48:01.382681 bionty_base-0.37.1/docs/guide/comparison.md
--rw-r--r--   0        0        0     1455 2024-02-05 06:48:01.382797 bionty_base-0.37.1/docs/guide/concepts.md
--rw-r--r--   0        0        0     3796 2024-02-05 06:48:01.382919 bionty_base-0.37.1/docs/guide/config.md
--rw-r--r--   0        0        0     3694 2024-02-05 06:48:01.383015 bionty_base-0.37.1/docs/guide/extend.md
--rw-r--r--   0        0        0     7453 2024-02-05 06:48:01.383225 bionty_base-0.37.1/docs/guide/ontology.ipynb
--rw-r--r--   0        0        0      358 2024-02-05 06:48:01.383355 bionty_base-0.37.1/docs/guide/search.ipynb
--rw-r--r--   0        0        0     7536 2024-02-05 06:48:01.383558 bionty_base-0.37.1/docs/guide/sources.ipynb
--rw-r--r--   0        0        0      160 2024-02-05 06:48:01.383648 bionty_base-0.37.1/docs/guide/test_notebooks.py
--rw-r--r--   0        0        0      981 2024-02-05 06:48:01.383731 bionty_base-0.37.1/docs/guide/validate.ipynb
--rw-r--r--   0        0        0      126 2024-02-05 06:48:01.383842 bionty_base-0.37.1/docs/index.md
--rw-r--r--   0        0        0       59 2024-02-05 06:48:01.383923 bionty_base-0.37.1/docs/reference.md
--rw-r--r--   0        0        0      146 2024-02-05 06:48:01.384003 bionty_base-0.37.1/lamin-project.yaml
--rw-r--r--   0        0        0      869 2024-03-27 07:46:53.424783 bionty_base-0.37.1/noxfile.py
--rw-r--r--   0        0        0     4093 2024-03-27 07:46:53.424973 bionty_base-0.37.1/pyproject.toml
--rw-r--r--   0        0        0      666 2024-02-05 06:48:01.384396 bionty_base-0.37.1/scripts/bfxpipelines_info/custom_pipelines.json
--rw-r--r--   0        0        0     1494 2024-02-05 06:58:39.467037 bionty_base-0.37.1/scripts/check_ontologies_reachable.py
--rw-r--r--   0        0        0     1290 2024-02-05 06:48:01.384561 bionty_base-0.37.1/scripts/determine_md5s.py
--rw-r--r--   0        0        0     3433 2024-02-05 06:48:01.384646 bionty_base-0.37.1/scripts/generate_bfxpipelines.py
--rw-r--r--   0        0        0     1127 2024-02-05 06:48:01.384730 bionty_base-0.37.1/scripts/update_new_ontologies.py
--rw-r--r--   0        0        0     1789 2024-02-05 06:48:01.384804 bionty_base-0.37.1/scripts/upload_new_ontologies.py
--rw-r--r--   0        0        0     6980 2024-02-05 06:48:01.385073 bionty_base-0.37.1/tests/dev/test_handle_sources.py
--rw-r--r--   0        0        0      532 2024-02-05 06:48:01.385163 bionty_base-0.37.1/tests/dev/test_io.py
--rw-r--r--   0        0        0      550 2024-02-05 06:48:01.385288 bionty_base-0.37.1/tests/entities/test_bfxpipeline.py
--rw-r--r--   0        0        0      163 2024-02-05 06:48:01.385366 bionty_base-0.37.1/tests/entities/test_biosample.py
--rw-r--r--   0        0        0      569 2024-02-05 06:48:01.385481 bionty_base-0.37.1/tests/entities/test_cellline.py
--rw-r--r--   0        0        0      918 2024-02-05 06:48:01.385574 bionty_base-0.37.1/tests/entities/test_cellmarker.py
--rw-r--r--   0        0        0      609 2024-02-05 06:48:01.385685 bionty_base-0.37.1/tests/entities/test_celltype.py
--rw-r--r--   0        0        0      632 2024-02-05 06:48:01.385772 bionty_base-0.37.1/tests/entities/test_developmentalstage.py
--rw-r--r--   0        0        0     2967 2024-02-05 06:48:01.385867 bionty_base-0.37.1/tests/entities/test_disease.py
--rw-r--r--   0        0        0      600 2024-02-05 06:48:01.385954 bionty_base-0.37.1/tests/entities/test_drug.py
--rw-r--r--   0        0        0      575 2024-02-05 06:48:01.386043 bionty_base-0.37.1/tests/entities/test_ethnicity.py
--rw-r--r--   0        0        0     1066 2024-02-05 06:48:01.386120 bionty_base-0.37.1/tests/entities/test_experimentalfactor.py
--rw-r--r--   0        0        0     2396 2024-02-05 06:48:01.386201 bionty_base-0.37.1/tests/entities/test_gene.py
--rw-r--r--   0        0        0      871 2024-02-05 06:48:01.386289 bionty_base-0.37.1/tests/entities/test_organism.py
--rw-r--r--   0        0        0     1179 2024-02-05 06:48:01.386364 bionty_base-0.37.1/tests/entities/test_pathway.py
--rw-r--r--   0        0        0     3020 2024-02-05 06:48:01.386437 bionty_base-0.37.1/tests/entities/test_phenotype.py
--rw-r--r--   0        0        0      579 2024-02-05 06:48:01.386521 bionty_base-0.37.1/tests/entities/test_protein.py
--rw-r--r--   0        0        0      596 2024-02-05 06:48:01.386618 bionty_base-0.37.1/tests/entities/test_tissue.py
--rw-r--r--   0        0        0     1486 2024-02-05 06:48:01.386705 bionty_base-0.37.1/tests/test_bionty.py
--rw-r--r--   0        0        0      627 2024-02-05 06:48:01.386784 bionty_base-0.37.1/tests/test_lamindb.py
--rw-r--r--   0        0        0      767 2024-02-05 06:48:01.386854 bionty_base-0.37.1/tests/test_md5.py
--rw-r--r--   0        0        0      418 2024-02-05 06:48:01.386929 bionty_base-0.37.1/tests/test_ontology.py
--rw-r--r--   0        0        0     4305 1970-01-01 00:00:00.000000 bionty_base-0.37.1/PKG-INFO
+-rw-r--r--   0        0        0     3169 2024-04-05 12:50:11.730131 bionty-base-0.37.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      555 2024-03-07 15:08:48.176384 bionty-base-0.37.2/.github/workflows/check_ontologies_reachable.yml
+-rw-r--r--   0        0        0      133 2024-03-07 15:08:48.176384 bionty-base-0.37.2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-04-05 12:50:11.733464 bionty-base-0.37.2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0      504 2024-04-05 12:50:11.733464 bionty-base-0.37.2/.github/workflows/update_ontologies.yml
+-rw-r--r--   0        0        0     2115 2024-03-07 15:08:48.176384 bionty-base-0.37.2/.gitignore
+-rw-r--r--   0        0        0     1512 2024-03-07 15:08:48.176384 bionty-base-0.37.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2024-03-07 15:08:48.176384 bionty-base-0.37.2/LICENSE
+-rw-r--r--   0        0        0     3116 2024-03-07 15:08:48.176384 bionty-base-0.37.2/README.md
+-rw-r--r--   0        0        0     1894 2024-04-05 12:51:42.647382 bionty-base-0.37.2/bionty_base/__init__.py
+-rw-r--r--   0        0        0     1605 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/_display_sources.py
+-rw-r--r--   0        0        0     3863 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/_ontology.py
+-rw-r--r--   0        0        0    24162 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/_public_ontology.py
+-rw-r--r--   0        0        0     2615 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/_settings.py
+-rw-r--r--   0        0        0      524 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/_sync_sources.py
+-rw-r--r--   0        0        0      111 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/dev/__init__.py
+-rw-r--r--   0        0        0     8456 2024-03-21 12:01:31.389175 bionty-base-0.37.2/bionty_base/dev/_handle_sources.py
+-rw-r--r--   0        0        0     5154 2024-03-21 12:01:31.389175 bionty-base-0.37.2/bionty_base/dev/_io.py
+-rw-r--r--   0        0        0     1021 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/dev/_md5.py
+-rw-r--r--   0        0        0        0 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/__init__.py
+-rw-r--r--   0        0        0     1370 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_bfxpipeline.py
+-rw-r--r--   0        0        0      682 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_biosample.py
+-rw-r--r--   0        0        0      804 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_cellline.py
+-rw-r--r--   0        0        0      728 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_cellmarker.py
+-rw-r--r--   0        0        0      817 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_celltype.py
+-rw-r--r--   0        0        0      913 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_developmentalstage.py
+-rw-r--r--   0        0        0     1164 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_disease.py
+-rw-r--r--   0        0        0      810 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_drug.py
+-rw-r--r--   0        0        0      831 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_ethnicity.py
+-rw-r--r--   0        0        0     4387 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_experimentalfactor.py
+-rw-r--r--   0        0        0    10086 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_gene.py
+-rw-r--r--   0        0        0     2570 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_organism.py
+-rw-r--r--   0        0        0      855 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_pathway.py
+-rw-r--r--   0        0        0     1420 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_phenotype.py
+-rw-r--r--   0        0        0      685 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_protein.py
+-rw-r--r--   0        0        0     1486 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_shared_docstrings.py
+-rw-r--r--   0        0        0      799 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_tissue.py
+-rw-r--r--   0        0        0    11067 2024-04-05 12:50:11.733464 bionty-base-0.37.2/bionty_base/sources/sources.yaml
+-rw-r--r--   0        0        0    47474 2024-04-05 12:50:11.733464 bionty-base-0.37.2/docs/changelog.md
+-rw-r--r--   0        0        0     1015 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/developer/updating_source.md
+-rw-r--r--   0        0        0      200 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/guide.md
+-rw-r--r--   0        0        0     3335 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/guide/comparison.md
+-rw-r--r--   0        0        0     1455 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/guide/concepts.md
+-rw-r--r--   0        0        0     3796 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/guide/config.md
+-rw-r--r--   0        0        0     3694 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/guide/extend.md
+-rw-r--r--   0        0        0     7453 2024-03-08 14:34:27.000329 bionty-base-0.37.2/docs/guide/ontology.ipynb
+-rw-r--r--   0        0        0      358 2024-03-08 14:34:26.970329 bionty-base-0.37.2/docs/guide/search.ipynb
+-rw-r--r--   0        0        0     7536 2024-03-08 14:34:27.026996 bionty-base-0.37.2/docs/guide/sources.ipynb
+-rw-r--r--   0        0        0      160 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/guide/test_notebooks.py
+-rw-r--r--   0        0        0      981 2024-03-08 14:34:27.026996 bionty-base-0.37.2/docs/guide/validate.ipynb
+-rw-r--r--   0        0        0      126 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/index.md
+-rw-r--r--   0        0        0       59 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/reference.md
+-rw-r--r--   0        0        0      146 2024-03-07 15:08:48.179717 bionty-base-0.37.2/lamin-project.yaml
+-rw-r--r--   0        0        0      869 2024-04-04 08:31:23.478547 bionty-base-0.37.2/noxfile.py
+-rw-r--r--   0        0        0     4093 2024-04-04 08:31:23.481881 bionty-base-0.37.2/pyproject.toml
+-rw-r--r--   0        0        0      666 2024-03-07 15:08:48.179717 bionty-base-0.37.2/scripts/bfxpipelines_info/custom_pipelines.json
+-rw-r--r--   0        0        0     1494 2024-03-07 15:08:48.179717 bionty-base-0.37.2/scripts/check_ontologies_reachable.py
+-rw-r--r--   0        0        0     1290 2024-03-07 15:08:48.179717 bionty-base-0.37.2/scripts/determine_md5s.py
+-rw-r--r--   0        0        0     3433 2024-03-07 15:08:48.179717 bionty-base-0.37.2/scripts/generate_bfxpipelines.py
+-rw-r--r--   0        0        0     1127 2024-03-07 15:08:48.179717 bionty-base-0.37.2/scripts/update_new_ontologies.py
+-rw-r--r--   0        0        0     1789 2024-03-07 15:08:48.179717 bionty-base-0.37.2/scripts/upload_new_ontologies.py
+-rw-r--r--   0        0        0     6980 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/dev/test_handle_sources.py
+-rw-r--r--   0        0        0      532 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/dev/test_io.py
+-rw-r--r--   0        0        0      550 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_bfxpipeline.py
+-rw-r--r--   0        0        0      163 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_biosample.py
+-rw-r--r--   0        0        0      569 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_cellline.py
+-rw-r--r--   0        0        0      918 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_cellmarker.py
+-rw-r--r--   0        0        0      609 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_celltype.py
+-rw-r--r--   0        0        0      632 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_developmentalstage.py
+-rw-r--r--   0        0        0     2967 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_disease.py
+-rw-r--r--   0        0        0      600 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_drug.py
+-rw-r--r--   0        0        0      575 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_ethnicity.py
+-rw-r--r--   0        0        0     1066 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_experimentalfactor.py
+-rw-r--r--   0        0        0     2396 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_gene.py
+-rw-r--r--   0        0        0      871 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_organism.py
+-rw-r--r--   0        0        0     1179 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_pathway.py
+-rw-r--r--   0        0        0     3020 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_phenotype.py
+-rw-r--r--   0        0        0      579 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_protein.py
+-rw-r--r--   0        0        0      596 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_tissue.py
+-rw-r--r--   0        0        0     1486 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/test_bionty.py
+-rw-r--r--   0        0        0      627 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/test_lamindb.py
+-rw-r--r--   0        0        0      767 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/test_md5.py
+-rw-r--r--   0        0        0      418 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/test_ontology.py
+-rw-r--r--   0        0        0     4305 1970-01-01 00:00:00.000000 bionty-base-0.37.2/PKG-INFO
```

### Comparing `bionty_base-0.37.1/.github/workflows/build.yml` & `bionty-base-0.37.2/.github/workflows/build.yml`

 * *Files 13% similar despite different names*

```diff
@@ -19,20 +19,20 @@
       matrix:
         python-version: ["3.11"]
         group: ["bionty-unit", "bionty-docs"]
     timeout-minutes: 25
 
     steps:
       - name: Checkout main
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           submodules: recursive
           fetch-depth: 0
       - name: Checkout lndocs
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           repository: laminlabs/lndocs
           ssh-key: ${{ secrets.READ_LNDOCS }}
           path: lndocs
           ref: main
       - name: Setup Python
         uses: actions/setup-python@v5
@@ -85,15 +85,15 @@
           NETLIFY_AUTH_TOKEN: ${{ secrets.NETLIFY_AUTH_TOKEN }}
           NETLIFY_SITE_ID: ${{ secrets.NETLIFY_SITE_ID }}
 
   coverage:
     needs: test
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: "3.11"
       - run: |
           python -m pip install -U pip uv
           uv pip install --system coverage[toml]
           uv pip install --system --no-deps .
```

### Comparing `bionty_base-0.37.1/.github/workflows/check_ontologies_reachable.yml` & `bionty-base-0.37.2/.github/workflows/check_ontologies_reachable.yml`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/.github/workflows/latest-changes.yml` & `bionty-base-0.37.2/.github/workflows/latest-changes.yml`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,14 @@
         description: PR number
         required: true
 
 jobs:
   latest-changes:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
       - uses: docker://tiangolo/latest-changes:0.0.3
         with:
           token: ${{ secrets.GITHUB_TOKEN }}
           latest_changes_file: docs/changelog.md
           latest_changes_header: '--- \| --- \| --- \| --- \| ---\n'
           template_file: ./.github/workflows/latest-changes.jinja2
```

### Comparing `bionty_base-0.37.1/.gitignore` & `bionty-base-0.37.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/.pre-commit-config.yaml` & `bionty-base-0.37.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/LICENSE` & `bionty-base-0.37.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/README.md` & `bionty-base-0.37.2/README.md`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/__init__.py` & `bionty-base-0.37.2/bionty_base/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 .. autosummary::
    :toctree: .
 
    Ontology
 """
 
-__version__ = "0.37.1"  # denote release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.37.2"  # denote release candidate for 0.1.0 with 0.1rc1
 
 from ._sync_sources import sync_sources
 
 sync_sources()
 
 # dynamic classes
 from . import dev
```

### Comparing `bionty_base-0.37.1/bionty_base/_display_sources.py` & `bionty-base-0.37.2/bionty_base/_display_sources.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/_ontology.py` & `bionty-base-0.37.2/bionty_base/_ontology.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/_public_ontology.py` & `bionty-base-0.37.2/bionty_base/_public_ontology.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/_settings.py` & `bionty-base-0.37.2/bionty_base/_settings.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/_sync_sources.py` & `bionty-base-0.37.2/bionty_base/_sync_sources.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/dev/_handle_sources.py` & `bionty-base-0.37.2/bionty_base/dev/_handle_sources.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/dev/_io.py` & `bionty-base-0.37.2/bionty_base/dev/_io.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/dev/_md5.py` & `bionty-base-0.37.2/bionty_base/dev/_md5.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_bfxpipeline.py` & `bionty-base-0.37.2/bionty_base/entities/_bfxpipeline.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_biosample.py` & `bionty-base-0.37.2/bionty_base/entities/_biosample.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_cellline.py` & `bionty-base-0.37.2/bionty_base/entities/_cellline.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_cellmarker.py` & `bionty-base-0.37.2/bionty_base/entities/_cellmarker.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_celltype.py` & `bionty-base-0.37.2/bionty_base/entities/_celltype.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_developmentalstage.py` & `bionty-base-0.37.2/bionty_base/entities/_developmentalstage.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_disease.py` & `bionty-base-0.37.2/bionty_base/entities/_disease.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_drug.py` & `bionty-base-0.37.2/bionty_base/entities/_drug.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_ethnicity.py` & `bionty-base-0.37.2/bionty_base/entities/_ethnicity.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_experimentalfactor.py` & `bionty-base-0.37.2/bionty_base/entities/_experimentalfactor.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_gene.py` & `bionty-base-0.37.2/bionty_base/entities/_gene.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_organism.py` & `bionty-base-0.37.2/bionty_base/entities/_organism.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_pathway.py` & `bionty-base-0.37.2/bionty_base/entities/_pathway.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_phenotype.py` & `bionty-base-0.37.2/bionty_base/entities/_phenotype.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_protein.py` & `bionty-base-0.37.2/bionty_base/entities/_protein.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_shared_docstrings.py` & `bionty-base-0.37.2/bionty_base/entities/_shared_docstrings.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/entities/_tissue.py` & `bionty-base-0.37.2/bionty_base/entities/_tissue.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/bionty_base/sources/sources.yaml` & `bionty-base-0.37.2/bionty_base/sources/sources.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,17 @@
     name: Human Disease Ontology
     website: https://disease-ontology.org
   icd:
     human:
       icd-11-2023:
         url: s3://bionty-assets/df_human__icd__icd-11-2023__Disease.parquet
         md5: 16263aef644d2c62c47b7b1ecfbad9d6
+      icd-10-2024:
+        url: s3://bionty-assets/df_human__icd__icd-10-2024__Disease.parquet
+        md5: cda43c983700518d76bd44c0e2c869d1
       icd-10-2020:
         url: s3://bionty-assets/df_human__icd__icd-10-2020__Disease.parquet
         md5: 93ec5734fcc2edd64686d5ffc6f6105f
       icd-9-2011:
         url: s3://bionty-assets/df_human__icd__icd-9-2011__Disease.parquet
         md5: cb3aefb3c4f7b2c47bf3de38453350c7
     name: International Classification of Diseases (ICD)
```

### Comparing `bionty_base-0.37.1/docs/changelog.md` & `bionty-base-0.37.2/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+Add new ICD 10-CM | [554](https://github.com/laminlabs/bionty-base/pull/554) | [Zethson](https://github.com/Zethson) | 2024-04-04 |
 🔇 Remove py version warning | [553](https://github.com/laminlabs/bionty-base/pull/553) | [sunnyosun](https://github.com/sunnyosun) | 2024-03-27 | 0.37.1
 Switch to uv for CI | [552](https://github.com/laminlabs/bionty-base/pull/552) | [Zethson](https://github.com/Zethson) | 2024-03-24 |
 🐛 Catch ClientError | [549](https://github.com/laminlabs/bionty-base/pull/549) | [Koncopd](https://github.com/Koncopd) | 2024-03-14 |
 Fix reset message | [545](https://github.com/laminlabs/bionty-base/pull/545) | [Zethson](https://github.com/Zethson) | 2024-03-13 |
 📝 Added validate example to docstring | [542](https://github.com/laminlabs/bionty-base/pull/542) | [sunnyosun](https://github.com/sunnyosun) | 2024-03-01 |
 🚚 Rename repo to `bionty-base` | [539](https://github.com/laminlabs/bionty-base/pull/539) | [sunnyosun](https://github.com/sunnyosun) | 2024-01-29 | 0.37.0
 Add ICD ontology | [538](https://github.com/laminlabs/bionty/pull/538) | [Zethson](https://github.com/Zethson) | 2024-01-24 |
```

### Comparing `bionty_base-0.37.1/docs/developer/updating_source.md` & `bionty-base-0.37.2/docs/developer/updating_source.md`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/docs/guide/comparison.md` & `bionty-base-0.37.2/docs/guide/comparison.md`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/docs/guide/concepts.md` & `bionty-base-0.37.2/docs/guide/concepts.md`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/docs/guide/config.md` & `bionty-base-0.37.2/docs/guide/config.md`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/docs/guide/extend.md` & `bionty-base-0.37.2/docs/guide/extend.md`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/docs/guide/ontology.ipynb` & `bionty-base-0.37.2/docs/guide/ontology.ipynb`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/docs/guide/sources.ipynb` & `bionty-base-0.37.2/docs/guide/sources.ipynb`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/docs/guide/validate.ipynb` & `bionty-base-0.37.2/docs/guide/validate.ipynb`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/noxfile.py` & `bionty-base-0.37.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/pyproject.toml` & `bionty-base-0.37.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/scripts/bfxpipelines_info/custom_pipelines.json` & `bionty-base-0.37.2/scripts/bfxpipelines_info/custom_pipelines.json`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/scripts/check_ontologies_reachable.py` & `bionty-base-0.37.2/scripts/check_ontologies_reachable.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/scripts/determine_md5s.py` & `bionty-base-0.37.2/scripts/determine_md5s.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/scripts/generate_bfxpipelines.py` & `bionty-base-0.37.2/scripts/generate_bfxpipelines.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/scripts/update_new_ontologies.py` & `bionty-base-0.37.2/scripts/update_new_ontologies.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/scripts/upload_new_ontologies.py` & `bionty-base-0.37.2/scripts/upload_new_ontologies.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/dev/test_handle_sources.py` & `bionty-base-0.37.2/tests/dev/test_handle_sources.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/dev/test_io.py` & `bionty-base-0.37.2/tests/dev/test_io.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_bfxpipeline.py` & `bionty-base-0.37.2/tests/entities/test_bfxpipeline.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_cellline.py` & `bionty-base-0.37.2/tests/entities/test_cellline.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_cellmarker.py` & `bionty-base-0.37.2/tests/entities/test_cellmarker.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_celltype.py` & `bionty-base-0.37.2/tests/entities/test_celltype.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_developmentalstage.py` & `bionty-base-0.37.2/tests/entities/test_developmentalstage.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_disease.py` & `bionty-base-0.37.2/tests/entities/test_disease.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_drug.py` & `bionty-base-0.37.2/tests/entities/test_drug.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_ethnicity.py` & `bionty-base-0.37.2/tests/entities/test_ethnicity.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_experimentalfactor.py` & `bionty-base-0.37.2/tests/entities/test_experimentalfactor.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_gene.py` & `bionty-base-0.37.2/tests/entities/test_gene.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_organism.py` & `bionty-base-0.37.2/tests/entities/test_organism.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_pathway.py` & `bionty-base-0.37.2/tests/entities/test_pathway.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_phenotype.py` & `bionty-base-0.37.2/tests/entities/test_phenotype.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_protein.py` & `bionty-base-0.37.2/tests/entities/test_protein.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/entities/test_tissue.py` & `bionty-base-0.37.2/tests/entities/test_tissue.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/test_bionty.py` & `bionty-base-0.37.2/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/test_lamindb.py` & `bionty-base-0.37.2/tests/test_lamindb.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/tests/test_md5.py` & `bionty-base-0.37.2/tests/test_md5.py`

 * *Files identical despite different names*

### Comparing `bionty_base-0.37.1/PKG-INFO` & `bionty-base-0.37.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bionty-base
-Version: 0.37.1
+Version: 0.37.2
 Summary: Bionty.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

