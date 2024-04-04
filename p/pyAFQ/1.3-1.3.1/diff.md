# Comparing `tmp/pyAFQ-1.3.tar.gz` & `tmp/pyAFQ-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyAFQ-1.3.tar", last modified: Mon Mar 25 16:25:25 2024, max compression
+gzip compressed data, was "pyAFQ-1.3.1.tar", last modified: Thu Apr  4 23:15:21 2024, max compression
```

## Comparing `pyAFQ-1.3.tar` & `pyAFQ-1.3.1.tar`

### file list

```diff
@@ -1,502 +1,503 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.470103 pyAFQ-1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.390103 pyAFQ-1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-25 16:25:20.000000 pyAFQ-1.3/.github/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    16080 2024-03-25 16:25:20.000000 pyAFQ-1.3/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.394103 pyAFQ-1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-25 16:25:20.000000 pyAFQ-1.3/.github/workflows/docbuild.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-03-25 16:25:20.000000 pyAFQ-1.3/.github/workflows/docker_pyafq.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-25 16:25:20.000000 pyAFQ-1.3/.github/workflows/docker_pyafq_cuda12.yml
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-25 16:25:20.000000 pyAFQ-1.3/.github/workflows/nightly_anisotropic_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-25 16:25:20.000000 pyAFQ-1.3/.github/workflows/nightly_basic_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-25 16:25:20.000000 pyAFQ-1.3/.github/workflows/nightly_custom_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-25 16:25:20.000000 pyAFQ-1.3/.github/workflows/nightly_pft_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-25 16:25:20.000000 pyAFQ-1.3/.github/workflows/nightly_reco80_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-25 16:25:20.000000 pyAFQ-1.3/.github/workflows/nightly_reco_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-25 16:25:20.000000 pyAFQ-1.3/.github/workflows/nightly_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-25 16:25:20.000000 pyAFQ-1.3/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-25 16:25:20.000000 pyAFQ-1.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-25 16:25:20.000000 pyAFQ-1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-25 16:25:20.000000 pyAFQ-1.3/.mailmap
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.394103 pyAFQ-1.3/.maintenance/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1395 2024-03-25 16:25:20.000000 pyAFQ-1.3/.maintenance/update_changes.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2870 2024-03-25 16:25:20.000000 pyAFQ-1.3/.maintenance/update_zenodo.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-25 16:25:20.000000 pyAFQ-1.3/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-03-25 16:25:20.000000 pyAFQ-1.3/.zenodo.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.394103 pyAFQ-1.3/AFQ/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/afq_bids_entities.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.394103 pyAFQ-1.3/AFQ/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46844 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/api/bundle_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    40385 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/api/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/api/participant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.394103 pyAFQ-1.3/AFQ/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67032 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/data/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.398103 pyAFQ-1.3/AFQ/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26362 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/definitions/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/definitions/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/definitions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.398103 pyAFQ-1.3/AFQ/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/models/QBallTP.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/models/csd.py
--rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/models/dki.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/models/dti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/models/fwdti.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    57809 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.398103 pyAFQ-1.3/AFQ/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31393 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tasks/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tasks/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tasks/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    13824 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tasks/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tasks/tractography.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tasks/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15295 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tasks/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.402103 pyAFQ-1.3/AFQ/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.402103 pyAFQ-1.3/AFQ/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    53305 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/MoriGroups_Test.mat
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/WholeBrainFG_test.mat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.374104 pyAFQ-1.3/AFQ/tests/data/mocks3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.402103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.406103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/.datalad/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/.datalad/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/.datalad/config
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/CHANGES
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/README
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/T1w.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/annex-uuid
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/dataset_description.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.374104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.414103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/aMRIQC.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_group.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-01.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-02.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-03.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-04.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-05.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-06.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-07.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-08.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-09.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-10.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-11.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-12.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-13.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-14.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-16.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-17.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-18.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-19.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-20.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-21.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-22.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-23.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-24.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-25.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-26.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/fMRIQC.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_group.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-01.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-02.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-03.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-04.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-05.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-06.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-07.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-08.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-09.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-10.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-11.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-12.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-13.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-14.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-16.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-17.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-18.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-19.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-20.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-21.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-22.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-23.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-24.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-25.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-26.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/participants.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.374104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.414103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/anat/sub-01_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.414103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.374104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.414103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/anat/sub-02_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.414103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.374104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.414103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/anat/sub-03_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.418103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.374104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.418103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/anat/sub-04_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.418103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.374104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.418103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/anat/sub-05_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.418103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.374104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.418103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/anat/sub-06_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.418103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.378104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.418103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/anat/sub-07_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.418103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.378104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.418103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/anat/sub-08_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.422103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.378104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.422103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/anat/sub-09_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.422103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.378104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.422103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/anat/sub-10_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.422103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.378104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.422103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/anat/sub-11_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.422103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.378104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.422103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/anat/sub-12_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.422103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.378104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.426103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/anat/sub-13_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.426103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.378104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.426103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/anat/sub-14_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.426103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.378104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.426103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/anat/sub-15_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.426103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.378104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.426103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/anat/sub-16_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.426103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.378104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.426103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/anat/sub-17_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.430103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.382104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.430103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/anat/sub-18_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.430103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.382104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.430103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/anat/sub-19_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.430103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.382104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.430103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/anat/sub-20_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.430103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.382104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.430103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/anat/sub-21_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.430103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.382104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.430103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/anat/sub-22_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.434103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.382104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.434103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/anat/sub-23_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.434103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.382104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.434103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/anat/sub-24_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.434103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.382104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.434103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/anat/sub-25_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.434103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.382104 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.434103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/anat/sub-26_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.434103 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-2_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/task-flanker_bold.json
--rw-r--r--   0 runner    (1001) docker     (127)    30829 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/test_bundle_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/test_csd.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/test_dki.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/test_dti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/test_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/test_tractography.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.438103 pyAFQ-1.3/AFQ/tractography/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tractography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tractography/gputractography.py
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tractography/tractography.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/tractography/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.438103 pyAFQ-1.3/AFQ/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15159 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/bin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.438103 pyAFQ-1.3/AFQ/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/tests/test_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/tests/test_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/utils/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-25 16:25:25.000000 pyAFQ-1.3/AFQ/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.442103 pyAFQ-1.3/AFQ/viz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/viz/altair.py
--rw-r--r--   0 runner    (1001) docker     (127)    18554 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/viz/fury_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    58032 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/viz/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    25572 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/viz/plotly_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    22824 2024-03-25 16:25:20.000000 pyAFQ-1.3/AFQ/viz/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34918 2024-03-25 16:25:20.000000 pyAFQ-1.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-25 16:25:20.000000 pyAFQ-1.3/CITATION
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-25 16:25:20.000000 pyAFQ-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-25 16:25:20.000000 pyAFQ-1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-25 16:25:20.000000 pyAFQ-1.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-03-25 16:25:25.470103 pyAFQ-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-25 16:25:20.000000 pyAFQ-1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.442103 pyAFQ-1.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4994 2024-03-25 16:25:20.000000 pyAFQ-1.3/bin/pyAFQ
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.442103 pyAFQ-1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.442103 pyAFQ-1.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/_progressbars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.442103 pyAFQ-1.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   272903 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/_static/BDE_Banner_revised20160211-01.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    56025 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/_static/eScience_Logo_HR.png
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/_static/escience-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   112939 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.442103 pyAFQ-1.3/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.446103 pyAFQ-1.3/docs/source/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.446103 pyAFQ-1.3/docs/source/explanations/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    14803 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/explanations/_static/down_left_arrow.png
--rw-r--r--   0 runner    (1001) docker     (127)    14739 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/explanations/_static/down_right_arrow.png
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/explanations/_static/greencheck.png
--rw-r--r--   0 runner    (1001) docker     (127)    99285 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/explanations/_static/tract_modeling2.png
--rw-r--r--   0 runner    (1001) docker     (127)   207285 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/explanations/_static/tract_profiling.png
--rw-r--r--   0 runner    (1001) docker     (127)   220157 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/explanations/_static/tract_recognition.png
--rw-r--r--   0 runner    (1001) docker     (127)   254342 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/explanations/_static/tract_tractography.png
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/explanations/modeling.rst
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/explanations/profiling.rst
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/explanations/recognition.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/explanations/tractography.rst
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/explanations/tractometry_pipeline.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.450103 pyAFQ-1.3/docs/source/howto/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/cite.rst
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.450103 pyAFQ-1.3/docs/source/howto/developing/
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/developing/definitions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/developing/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/developing/releasing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/developing/tasks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/getting_help.rst
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/installation_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.450103 pyAFQ-1.3/docs/source/howto/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/usage/converter.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/usage/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/usage/docker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/usage/image.rst
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/usage/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/usage/kwargs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/usage/methods.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/howto/usage/scalars.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.450103 pyAFQ-1.3/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/reference/bundledict.rst
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8425 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/reference/kwargs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/reference/mapping.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/reference/methods.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/reference/viz_backend.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.454103 pyAFQ-1.3/docs/source/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/sphinxext/kwargsdocs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/sphinxext/methodsdocs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/sphinxext/updatedocs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.454103 pyAFQ-1.3/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/source/tutorials/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)      887 2024-03-25 16:25:20.000000 pyAFQ-1.3/docs/upload-gh-pages.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.386103 pyAFQ-1.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.454103 pyAFQ-1.3/examples/howto_examples/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/howto_examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/howto_examples/add_custom_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/howto_examples/baby_afq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/howto_examples/cerebellar_peduncles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/howto_examples/cloudknot_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/howto_examples/cloudknot_hcp_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/howto_examples/plot_acoustic_radiations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/howto_examples/plot_afq_callosal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/howto_examples/plot_afq_fwdti.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/howto_examples/plot_optic_radiations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/howto_examples/plot_recobundles.py
--rw-r--r--   0 runner    (1001) docker     (127)    19258 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/howto_examples/plot_stages_of_tractometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/howto_examples/use_subject_space_rois_from_freesurfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/howto_examples/vof_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.454103 pyAFQ-1.3/examples/tutorial_examples/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/tutorial_examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/tutorial_examples/plot_001_afq_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/tutorial_examples/plot_002_bids_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    19513 2024-03-25 16:25:20.000000 pyAFQ-1.3/examples/tutorial_examples/plot_003_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.458103 pyAFQ-1.3/gpu_docker/
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-25 16:25:20.000000 pyAFQ-1.3/gpu_docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-03-25 16:25:20.000000 pyAFQ-1.3/gpu_docker/cuda_build.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-25 16:25:20.000000 pyAFQ-1.3/gpu_docker/cuda_track_template.def
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-25 16:25:20.000000 pyAFQ-1.3/gpu_docker/docker-build.sh
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-25 16:25:20.000000 pyAFQ-1.3/gpu_docker/docker-push.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.458103 pyAFQ-1.3/pyAFQ.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-03-25 16:25:25.000000 pyAFQ-1.3/pyAFQ.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21122 2024-03-25 16:25:25.000000 pyAFQ-1.3/pyAFQ.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 16:25:25.000000 pyAFQ-1.3/pyAFQ.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 16:25:25.000000 pyAFQ-1.3/pyAFQ.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-25 16:25:25.000000 pyAFQ-1.3/pyAFQ.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-25 16:25:25.000000 pyAFQ-1.3/pyAFQ.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:25:25.458103 pyAFQ-1.3/pyafq_docker/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-25 16:25:20.000000 pyAFQ-1.3/pyafq_docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-25 16:25:20.000000 pyAFQ-1.3/pyafq_docker/docker-build.sh
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-25 16:25:20.000000 pyAFQ-1.3/pyafq_docker/docker-push.sh
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-25 16:25:20.000000 pyAFQ-1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-25 16:25:25.470103 pyAFQ-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-25 16:25:20.000000 pyAFQ-1.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-25 16:25:20.000000 pyAFQ-1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.344086 pyAFQ-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.272085 pyAFQ-1.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    16080 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.272085 pyAFQ-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/docbuild.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/docker_pyafq.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/docker_pyafq_cuda12.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/nightly_anisotropic_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/nightly_basic_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/nightly_custom_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/nightly_pft_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/nightly_reco80_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/nightly_reco_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/nightly_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.mailmap
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.272085 pyAFQ-1.3.1/.maintenance/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1395 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.maintenance/update_changes.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2870 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.maintenance/update_zenodo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.zenodo.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.276085 pyAFQ-1.3.1/AFQ/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/afq_bids_entities.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.276085 pyAFQ-1.3.1/AFQ/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46835 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/api/bundle_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40386 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/api/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/api/participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.276085 pyAFQ-1.3.1/AFQ/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67032 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/data/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.276085 pyAFQ-1.3.1/AFQ/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26362 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/definitions/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/definitions/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/definitions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.280085 pyAFQ-1.3.1/AFQ/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/models/QBallTP.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/models/csd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/models/dki.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/models/dti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/models/fwdti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58329 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.280085 pyAFQ-1.3.1/AFQ/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32761 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12273 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/tractography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15295 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.284085 pyAFQ-1.3.1/AFQ/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.284085 pyAFQ-1.3.1/AFQ/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    53305 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/MoriGroups_Test.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/WholeBrainFG_test.mat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.284085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.284085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/.datalad/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/.datalad/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/.datalad/config
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/README
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/T1w.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/annex-uuid
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.292086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/aMRIQC.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_group.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-01.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-02.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-03.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-04.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-05.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-06.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-07.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-08.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-09.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-10.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-11.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-12.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-13.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-14.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-16.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-17.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-18.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-19.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-20.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-21.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-22.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-23.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-24.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-25.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-26.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/fMRIQC.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_group.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-01.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-02.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-03.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-04.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-05.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-06.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-07.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-08.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-09.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-10.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-11.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-12.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-13.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-14.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-16.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-17.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-18.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-19.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-20.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-21.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-22.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-23.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-24.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-25.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-26.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/participants.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.292086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/anat/sub-01_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/anat/sub-02_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/anat/sub-03_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/anat/sub-04_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/anat/sub-05_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/anat/sub-06_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/anat/sub-07_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/anat/sub-08_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/anat/sub-09_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/anat/sub-10_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/anat/sub-11_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/anat/sub-12_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/anat/sub-13_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/anat/sub-14_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/anat/sub-15_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/anat/sub-16_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/anat/sub-17_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/anat/sub-18_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/anat/sub-19_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/anat/sub-20_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/anat/sub-21_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/anat/sub-22_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/anat/sub-23_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/anat/sub-24_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/anat/sub-25_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/anat/sub-26_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.316086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-2_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/task-flanker_bold.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30829 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_bundle_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_csd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_dki.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_dti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_tractography.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.316086 pyAFQ-1.3.1/AFQ/tractography/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tractography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tractography/gputractography.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tractography/tractography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tractography/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.316086 pyAFQ-1.3.1/AFQ/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15159 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.316086 pyAFQ-1.3.1/AFQ/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/tests/test_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/tests/test_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 23:15:21.000000 pyAFQ-1.3.1/AFQ/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.320086 pyAFQ-1.3.1/AFQ/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/viz/altair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18554 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/viz/fury_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58032 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/viz/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25572 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/viz/plotly_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22824 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/viz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35389 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/CITATION
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-04 23:15:21.344086 pyAFQ-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.320086 pyAFQ-1.3.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4994 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/bin/pyAFQ
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.320086 pyAFQ-1.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.320086 pyAFQ-1.3.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/_progressbars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.320086 pyAFQ-1.3.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   272903 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/_static/BDE_Banner_revised20160211-01.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    56025 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/_static/eScience_Logo_HR.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/_static/escience-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   112939 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.320086 pyAFQ-1.3.1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.324086 pyAFQ-1.3.1/docs/source/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.324086 pyAFQ-1.3.1/docs/source/explanations/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14803 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/_static/down_left_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14739 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/_static/down_right_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/_static/greencheck.png
+-rw-r--r--   0 runner    (1001) docker     (127)    99285 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/_static/tract_modeling2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   207285 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/_static/tract_profiling.png
+-rw-r--r--   0 runner    (1001) docker     (127)   220157 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/_static/tract_recognition.png
+-rw-r--r--   0 runner    (1001) docker     (127)   254342 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/_static/tract_tractography.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/bundle_orientation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/profiling.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/recognition.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/tractography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/tractometry_pipeline.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.328086 pyAFQ-1.3.1/docs/source/howto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/cite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.328086 pyAFQ-1.3.1/docs/source/howto/developing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/developing/definitions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/developing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/developing/releasing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/developing/tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/getting_help.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/installation_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.328086 pyAFQ-1.3.1/docs/source/howto/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/converter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/image.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/kwargs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/methods.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/scalars.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.328086 pyAFQ-1.3.1/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/reference/bundledict.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/reference/kwargs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/reference/mapping.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8574 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/reference/methods.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/reference/viz_backend.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.332086 pyAFQ-1.3.1/docs/source/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/sphinxext/kwargsdocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/sphinxext/methodsdocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/sphinxext/updatedocs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.332086 pyAFQ-1.3.1/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/tutorials/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      887 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/upload-gh-pages.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.268085 pyAFQ-1.3.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.332086 pyAFQ-1.3.1/examples/howto_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/add_custom_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/baby_afq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/cerebellar_peduncles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/cloudknot_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/cloudknot_hcp_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/plot_acoustic_radiations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/plot_afq_callosal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/plot_afq_fwdti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/plot_optic_radiations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/plot_recobundles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19258 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/plot_stages_of_tractometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/use_subject_space_rois_from_freesurfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/vof_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.332086 pyAFQ-1.3.1/examples/tutorial_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/tutorial_examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/tutorial_examples/plot_001_afq_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/tutorial_examples/plot_002_bids_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19513 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/tutorial_examples/plot_003_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.336086 pyAFQ-1.3.1/gpu_docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/gpu_docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/gpu_docker/cuda_build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/gpu_docker/cuda_track_template.def
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/gpu_docker/docker-build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/gpu_docker/docker-push.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.336086 pyAFQ-1.3.1/pyAFQ.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-04 23:15:21.000000 pyAFQ-1.3.1/pyAFQ.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21170 2024-04-04 23:15:21.000000 pyAFQ-1.3.1/pyAFQ.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:15:21.000000 pyAFQ-1.3.1/pyAFQ.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:15:21.000000 pyAFQ-1.3.1/pyAFQ.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-04 23:15:21.000000 pyAFQ-1.3.1/pyAFQ.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-04 23:15:21.000000 pyAFQ-1.3.1/pyAFQ.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.336086 pyAFQ-1.3.1/pyafq_docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/pyafq_docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/pyafq_docker/docker-build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/pyafq_docker/docker-push.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-04 23:15:21.344086 pyAFQ-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/tox.ini
```

### Comparing `pyAFQ-1.3/.github/CONTRIBUTING.md` & `pyAFQ-1.3.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.github/workflows/docbuild.yml` & `pyAFQ-1.3.1/.github/workflows/docbuild.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.github/workflows/docker_pyafq.yml` & `pyAFQ-1.3.1/.github/workflows/docker_pyafq.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.github/workflows/docker_pyafq_cuda12.yml` & `pyAFQ-1.3.1/.github/workflows/docker_pyafq_cuda12.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.github/workflows/nightly_anisotropic_test.yml` & `pyAFQ-1.3.1/.github/workflows/nightly_anisotropic_test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.github/workflows/nightly_basic_test.yml` & `pyAFQ-1.3.1/.github/workflows/nightly_basic_test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.github/workflows/nightly_custom_test.yml` & `pyAFQ-1.3.1/.github/workflows/nightly_custom_test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.github/workflows/nightly_pft_test.yml` & `pyAFQ-1.3.1/.github/workflows/nightly_pft_test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.github/workflows/nightly_reco80_test.yml` & `pyAFQ-1.3.1/.github/workflows/nightly_reco80_test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.github/workflows/nightly_reco_test.yml` & `pyAFQ-1.3.1/.github/workflows/nightly_reco_test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.github/workflows/nightly_test.yml` & `pyAFQ-1.3.1/.github/workflows/nightly_test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.github/workflows/publish-to-test-pypi.yml` & `pyAFQ-1.3.1/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.github/workflows/test.yml` & `pyAFQ-1.3.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.mailmap` & `pyAFQ-1.3.1/.mailmap`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.maintenance/update_changes.sh` & `pyAFQ-1.3.1/.maintenance/update_changes.sh`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.maintenance/update_zenodo.py` & `pyAFQ-1.3.1/.maintenance/update_zenodo.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/.zenodo.json` & `pyAFQ-1.3.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/_fixes.py` & `pyAFQ-1.3.1/AFQ/_fixes.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/api/bundle_dict.py` & `pyAFQ-1.3.1/AFQ/api/bundle_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -783,31 +783,31 @@
         for key, item in bundle_info.items():
             self.__setitem__(key, item)
 
         self.logger = logging.getLogger('AFQ')
         if self.seg_algo == "afq":
             if "Forceps Major" in self.bundle_names\
                     and "Callosum Occipital" in self.bundle_names:
-                self.logger.warning((
+                self.logger.info((
                     "Forceps Major and Callosum Occipital bundles"
                     " are co-located, and AFQ"
                     " assigns each streamline to only one bundle."
                     " Only Callosum Occipital will be used."))
                 self.bundle_names.remove("Forceps Major")
             if "Forceps Minor" in self.bundle_names\
                     and "Callosum Orbital" in self.bundle_names:
-                self.logger.warning((
+                self.logger.info((
                     "Forceps Minor and Callosum Orbital bundles"
                     " are co-located, and AFQ"
                     " assigns each streamline to only one bundle."
                     " Only Callosum Orbital will be used."))
                 self.bundle_names.remove("Forceps Minor")
             if "Forceps Minor" in self.bundle_names\
                     and "Callosum Anterior Frontal" in self.bundle_names:
-                self.logger.warning((
+                self.logger.info((
                     "Forceps Minor and Callosum Anterior Frontal bundles"
                     " are co-located, and AFQ"
                     " assigns each streamline to only one bundle."
                     " Only Callosum Anterior Frontal will be used."))
                 self.bundle_names.remove("Forceps Minor")
 
     def update_max_includes(self, new_max):
```

### Comparing `pyAFQ-1.3/AFQ/api/group.py` & `pyAFQ-1.3.1/AFQ/api/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
                 self.valid_sub_list.append(subject)
                 self.valid_ses_list.append(str(session))
 
                 this_pAFQ = ParticipantAFQ(
                     dwi_data_file,
                     bval_file, bvec_file,
                     results_dir,
-                    bids_info={
+                    _bids_info={
                         "bids_layout": bids_layout,
                         "subject": subject,
                         "session": session},
                     **this_kwargs)
                 self.wf_dict[subject][str(session)] = this_pAFQ.wf_dict
                 self.pAFQ_list.append(this_pAFQ)
```

### Comparing `pyAFQ-1.3/AFQ/api/participant.py` & `pyAFQ-1.3.1/AFQ/api/participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,31 +30,32 @@
 class ParticipantAFQ(object):
     f"""{AFQclass_doc}"""
 
     def __init__(self,
                  dwi_data_file,
                  bval_file, bvec_file,
                  output_dir,
-                 bids_info=None,
+                 _bids_info=None,
                  **kwargs):
         """
         Initialize a ParticipantAFQ object from a BIDS dataset.
 
         Parameters
         ----------
         dwi_data_file : str
             Path to DWI data file.
         bval_file : str
             Path to bval file.
         bvec_file : str
             Path to bvec file.
         output_dir : str
             Path to output directory.
-        bids_info : dict or None, optional
-            This is used by GroupAFQ to provide information about
+        _bids_info : dict or None, optional
+            This should be left as None in most cases. It
+            is used by GroupAFQ to provide information about
             the BIDS layout to each participant.
         kwargs : additional optional parameters
             You can set additional parameters for any step
             of the process. See :ref:`usage/kwargs` for more details.
 
         Examples
         --------
@@ -98,15 +99,15 @@
         self.output_dir = output_dir
 
         self.kwargs = dict(
             dwi_path=dwi_data_file,
             bval=bval_file,
             bvec=bvec_file,
             results_dir=output_dir,
-            bids_info=bids_info,
+            bids_info=_bids_info,
             base_fname=get_base_fname(output_dir, dwi_data_file),
             **kwargs)
         self.make_workflow()
 
     def make_workflow(self):
         # construct pimms plans
         if "mapping_definition" in self.kwargs and isinstance(
```

### Comparing `pyAFQ-1.3/AFQ/api/utils.py` & `pyAFQ-1.3.1/AFQ/api/utils.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/data/fetch.py` & `pyAFQ-1.3.1/AFQ/data/fetch.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/data/utils.py` & `pyAFQ-1.3.1/AFQ/data/utils.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/definitions/image.py` & `pyAFQ-1.3.1/AFQ/definitions/image.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/definitions/mapping.py` & `pyAFQ-1.3.1/AFQ/definitions/mapping.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/definitions/utils.py` & `pyAFQ-1.3.1/AFQ/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/models/QBallTP.py` & `pyAFQ-1.3.1/AFQ/models/QBallTP.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/models/csd.py` & `pyAFQ-1.3.1/AFQ/models/csd.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/models/dki.py` & `pyAFQ-1.3.1/AFQ/models/dki.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/models/dti.py` & `pyAFQ-1.3.1/AFQ/models/dti.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/models/fwdti.py` & `pyAFQ-1.3.1/AFQ/models/fwdti.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/registration.py` & `pyAFQ-1.3.1/AFQ/registration.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/segmentation.py` & `pyAFQ-1.3.1/AFQ/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,14 +478,23 @@
         if self.return_idx:
             self.fiber_groups[b_name] = {}
             self.fiber_groups[b_name]['sl'] = sl
             self.fiber_groups[b_name]['idx'] = idx
         else:
             self.fiber_groups[b_name] = sl
 
+    def _add_bundle_to_meta(self, bundle_name, bundle_info):
+        bundle_info = bundle_info.copy()
+        # remove keys that can never be serialized
+        for key in [
+                'include', 'exclude', 'prob_map',
+                'start', 'end', 'curvature']:
+            bundle_info.pop(key, None)
+        self.meta[bundle_name] = bundle_info
+
     def segment_afq(self, tg=None):
         """
         Assign streamlines to bundles using the waypoint ROI approach
         Parameters
         ----------
         tg : StatefulTractogram class instance
         """
@@ -505,14 +514,15 @@
             (
                 n_streamlines,
                 len(self.bundle_dict),
                 self.bundle_dict.max_includes),
             dtype=np.uint32)
 
         self.fiber_groups = {}
+        self.meta = {}
 
         # We need to calculate the size of a voxel, so we can transform
         # from mm to voxel units:
         R = self.img_affine[0:3, 0:3]
         vox_dim = np.mean(np.diag(np.linalg.cholesky(R.T.dot(R))))
 
         # Tolerance is set to the square of the distance to the corner
@@ -858,18 +868,20 @@
                 for sb_name, sb_include_cuts in self.bundle_dict.get_b_info(
                         bundle)["bundlesection"].items():
                     bundlesection_select_sl = _cut_sls_by_dist(
                         select_sl, roi_dists,
                         sb_include_cuts, in_place=False)
                     self._add_bundle_to_fiber_group(
                         sb_name, bundlesection_select_sl, select_idx, to_flip)
+                    self._add_bundle_to_meta(sb_name, bundle_def)
             else:
                 self._add_bundle_to_fiber_group(
                     bundle, select_sl, select_idx, to_flip)
-        return self.fiber_groups
+                self._add_bundle_to_meta(bundle, bundle_def)
+        return self.fiber_groups, self.meta
 
     def move_streamlines(self, tg, to="template"):
         """Streamline-based registration of a whole-brain tractogram to
         the MNI whole-brain atlas.
 
         to : str
             "template" or "subject"
@@ -1048,15 +1060,15 @@
                                                                 self.img,
                                                                 Space.RASMM)
             else:
                 fiber_groups[bundle] = StatefulTractogram(oriented_sl,
                                                           self.img,
                                                           Space.RASMM)
         self.fiber_groups = fiber_groups
-        return fiber_groups
+        return fiber_groups, {}
 
 
 def sl_curve(sl, n_points):
     """
     Calculate the direction of the displacement between
     each point along a streamline
```

### Comparing `pyAFQ-1.3/AFQ/tasks/data.py` & `pyAFQ-1.3.1/AFQ/tasks/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import dipy.core.gradients as dpg
 
 import pimms
 
 import dipy.reconst.dki as dpy_dki
 import dipy.reconst.dti as dpy_dti
 import dipy.reconst.fwdti as dpy_fwdti
+import dipy.reconst.msdki as dpy_msdki
 from dipy.reconst.gqi import GeneralizedQSamplingModel
 from dipy.reconst import shm
 from dipy.reconst.dki_micro import axonal_water_fraction
 
 from AFQ.tasks.decorators import as_file, as_img, as_fit_deriv
 from AFQ.tasks.utils import get_fname, with_name, str_to_desc
 import AFQ.api.bundle_dict as abd
@@ -224,14 +225,61 @@
         Parameters=dict(
             FitMethod="WLS"),
         OutlierRejection=False,
         ModelURL=f"{DIPY_GH}reconst/dki.py")
     return dkf.model_params, meta
 
 
+@pimms.calc("msdki_tf")
+def msdki_fit(msdki_params, gtab):
+    """Mean Signal DKI DiffusionKurtosisFit object"""
+    msdki_params = nib.load(msdki_params).get_fdata()
+    tm = dpy_msdki.MeanDiffusionKurtosisModel(gtab)
+    return dpy_msdki.MeanDiffusionKurtosisFit(tm, msdki_params)
+
+
+@pimms.calc("msdki_params")
+@as_file(suffix='_odfmodel-MSDKI_desc-diffmodel_dwi.nii.gz')
+@as_img
+def msdki_params(brain_mask, gtab, data):
+    """
+    full path to a nifti file containing
+    parameters for the Mean Signal DKI fit
+    """
+    mask =\
+        nib.load(brain_mask).get_fdata()
+    msdki_model = dpy_msdki.MeanDiffusionKurtosisModel(gtab)
+    msdki_fit = msdki_model.fit(data, mask=mask)
+    meta = dict(
+        ModelURL=f"{DIPY_GH}reconst/msdki.py")
+    return msdki_fit.model_params, meta
+
+
+@pimms.calc("msdki_msd")
+@as_file('_odfmodel-MSDKI_desc-MSD_dwi.nii.gz')
+@as_fit_deriv('MSDKI')
+def msdki_msd(msdki_tf):
+    """
+    full path to a nifti file containing
+    the MSDKI mean signal diffusivity
+    """
+    return msdki_tf.msd
+
+
+@pimms.calc("msdki_msk")
+@as_file('_odfmodel-MSDKI_desc-MSK_dwi.nii.gz')
+@as_fit_deriv('MSDKI')
+def msdki_msk(msdki_tf):
+    """
+    full path to a nifti file containing
+    the MSDKI mean signal kurtosis
+    """
+    return msdki_tf.msk
+
+
 @pimms.calc("csd_params")
 @as_file(suffix='_odfmodel-CSD_desc-diffmodel_dwi.nii.gz')
 @as_img
 def csd_params(dwi, brain_mask, gtab, data,
                csd_response=None, csd_sh_order=None,
                csd_lambda_=1, csd_tau=0.1):
     """
@@ -968,16 +1016,17 @@
         get_data_gtab, b0, b0_mask, brain_mask,
         dti_fit, dki_fit, fwdti_fit, anisotropic_power_map,
         csd_anisotropic_index,
         dti_fa, dti_lt, dti_cfa, dti_pdd, dti_md, dki_kt, dki_lt, dki_fa,
         gq, gq_pmap, gq_ai, opdt_params, opdt_pmap, opdt_ai,
         csa_params, csa_pmap, csa_ai,
         fwdti_fa, fwdti_md, fwdti_fwf,
-        dki_md, dki_awf, dki_mk, dki_kfa, dti_ga, dti_rd, dti_ad,
-        dki_ga, dki_rd,
+        msdki_fit, msdki_params, msdki_msd, msdki_msk,
+        dki_md, dki_awf, dki_mk, dki_kfa, dki_ga, dki_rd,
+        dti_ga, dti_rd, dti_ad,
         dki_ad, dki_rk, dki_ak, dti_params, dki_params, fwdti_params,
         csd_params, get_bundle_dict])
 
     if "scalars" not in kwargs:
         bvals, _ = read_bvals_bvecs(kwargs["bval"], kwargs["bvec"])
         if len(dpg.unique_bvals_magnitude(bvals)) > 2:
             kwargs["scalars"] = [
```

### Comparing `pyAFQ-1.3/AFQ/tasks/decorators.py` & `pyAFQ-1.3.1/AFQ/tasks/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,29 +112,31 @@
 
 def as_file(suffix, include_track=False, include_seg=False):
     """
     return img and meta as saved file path, with json,
     and only run if not already found
     """
     def _as_file(func):
-        needed_args = ["base_fname"]
+        needed_args = ["base_fname", "results_dir"]
         if include_track:
             needed_args.append("tracking_params")
         if include_seg:
             needed_args.append("segmentation_params")
 
         @functools.wraps(func)
         @has_args(func, needed_args)
         def wrapper_as_file(*args, **kwargs):
-            og_arg_count, base_fname, tracking_params, segmentation_params =\
+            og_arg_count, base_fname, results_dir, \
+                tracking_params, segmentation_params =\
                 extract_added_args(
                     func,
-                    ["base_fname", "tracking_params", "segmentation_params"],
+                    ["base_fname", "results_dir",
+                     "tracking_params", "segmentation_params"],
                     args,
-                    includes=[True, include_track, include_seg])
+                    includes=[True, True, include_track, include_seg])
             this_file = get_fname(
                 base_fname, suffix,
                 tracking_params=tracking_params,
                 segmentation_params=segmentation_params)
 
             # tracking_params is defined and file has no extension
             if tracking_params is not None and not op.splitext(this_file)[1]:
@@ -166,14 +168,18 @@
                 elif include_seg:
                     meta["dependent"] = "rec"
                 elif include_track:
                     meta["dependent"] = "trk"
                 else:
                     meta["dependent"] = "dwi"
 
+                # modify meta source to be relative
+                if "source" in meta:
+                    meta["source"] = op.relpath(meta["source"], results_dir)
+
                 meta_fname = get_fname(
                     base_fname, f"{drop_extension(suffix)}.json",
                     tracking_params=tracking_params,
                     segmentation_params=segmentation_params)
                 write_json(meta_fname, meta)
             return this_file
         return wrapper_as_file
```

### Comparing `pyAFQ-1.3/AFQ/tasks/mapping.py` & `pyAFQ-1.3.1/AFQ/tasks/mapping.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tasks/segmentation.py` & `pyAFQ-1.3.1/AFQ/tasks/segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     indices_to_remove, _ = tg.remove_invalid_streamlines()
     if len(indices_to_remove) > 0:
         logger.warning(f"{len(indices_to_remove)} invalid streamlines removed")
 
     start_time = time()
     segmentation = seg.Segmentation(**segmentation_params)
-    bundles = segmentation.segment(
+    bundles, bundle_meta = segmentation.segment(
         bundle_dict,
         tg,
         mapping_imap["mapping"],
         data_imap["dwi"],
         reg_template=reg_template)
 
     seg_sft = aus.SegmentedSFT(bundles, Space.VOX)
@@ -99,14 +99,15 @@
             for k, v in value.items():
                 seg_params_out[k] = str(v)
         else:
             seg_params_out[arg_name] = str(value)
 
     meta["source"] = streamlines
     meta["Recognition Parameters"] = seg_params_out
+    meta["Bundle Parameters"] = bundle_meta
     meta["Timing"] = time() - start_time
     return tgram, meta
 
 
 @pimms.calc("indiv_bundles")
 def export_bundles(base_fname, results_dir,
                    bundles,
@@ -146,15 +147,17 @@
                     save_trx(trxfile, fname)
                 else:
                     save_tractogram(
                         bundle_sft, fname,
                         bbox_valid_check=False)
             else:
                 logger.info(f"No bundle to save for {bundle}")
-            meta = dict(source=bundles)
+            meta = dict(
+                source=bundles,
+                params=seg_sft.get_bundle_param_info(bundle))
             meta_fname = drop_extension(fname) + '.json'
             write_json(meta_fname, meta)
     return bundles_dir
 
 
 @pimms.calc("sl_counts")
 @as_file('_desc-slCount_dwi.csv', include_track=True, include_seg=True)
@@ -327,15 +330,17 @@
     profile_dict["tractID"] = bundle_names
     profile_dict["nodeID"] = node_numbers
     for ii, scalar in enumerate(scalar_dict.keys()):
         profile_dict[scalar] = profiles[ii]
 
     profile_dframe = pd.DataFrame(profile_dict)
     meta = dict(source=bundles,
-                parameters=get_default_args(afq_profile))
+                parameters=get_default_args(afq_profile),
+                scalars=list(scalar_dict.keys()),
+                bundles=list(seg_sft.bundle_names))
 
     return profile_dframe, meta
 
 
 @pimms.calc("scalar_dict")
 def get_scalar_dict(data_imap, mapping_imap, scalars=["dti_fa", "dti_md"]):
     """
```

### Comparing `pyAFQ-1.3/AFQ/tasks/tractography.py` & `pyAFQ-1.3.1/AFQ/tasks/tractography.py`

 * *Files 6% similar despite different names*

```diff
@@ -295,18 +295,24 @@
     kwargs["tracking_params"] = default_tracking_params
     kwargs["tracking_params"]["odf_model"] =\
         kwargs["tracking_params"]["odf_model"].upper()
     if kwargs["tracking_params"]["seed_mask"] is None:
         kwargs["tracking_params"]["seed_mask"] = ScalarImage(
             kwargs["best_scalar"])
         kwargs["tracking_params"]["seed_threshold"] = 0.2
+        logger.info((
+            "No seed mask given, using FA (or first scalar if none are FA)"
+            "thresholded to 0.2"))
     if kwargs["tracking_params"]["stop_mask"] is None:
         kwargs["tracking_params"]["stop_mask"] = ScalarImage(
             kwargs["best_scalar"])
         kwargs["tracking_params"]["stop_threshold"] = 0.2
+        logger.info((
+            "No stop mask given, using FA (or first scalar if none are FA)"
+            "thresholded to 0.2"))
 
     stop_mask = kwargs["tracking_params"]['stop_mask']
     seed_mask = kwargs["tracking_params"]['seed_mask']
     bids_info = kwargs["bids_info"]
 
     if bids_info is not None:
         if isinstance(stop_mask, Definition):
```

### Comparing `pyAFQ-1.3/AFQ/tasks/utils.py` & `pyAFQ-1.3.1/AFQ/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tasks/viz.py` & `pyAFQ-1.3.1/AFQ/tasks/viz.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tests/data/MoriGroups_Test.mat` & `pyAFQ-1.3.1/AFQ/tests/data/MoriGroups_Test.mat`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tests/data/WholeBrainFG_test.mat` & `pyAFQ-1.3.1/AFQ/tests/data/WholeBrainFG_test.mat`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tests/data/mocks3/ds000102-mimic/task-flanker_bold.json` & `pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/task-flanker_bold.json`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tests/test_api.py` & `pyAFQ-1.3.1/AFQ/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tests/test_bundle_dict.py` & `pyAFQ-1.3.1/AFQ/tests/test_bundle_dict.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tests/test_csd.py` & `pyAFQ-1.3.1/AFQ/tests/test_csd.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tests/test_definitions.py` & `pyAFQ-1.3.1/AFQ/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tests/test_dki.py` & `pyAFQ-1.3.1/AFQ/tests/test_dki.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tests/test_dti.py` & `pyAFQ-1.3.1/AFQ/tests/test_dti.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tests/test_fixes.py` & `pyAFQ-1.3.1/AFQ/tests/test_fixes.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tests/test_registration.py` & `pyAFQ-1.3.1/AFQ/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tests/test_segmentation.py` & `pyAFQ-1.3.1/AFQ/tests/test_segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,18 +181,19 @@
 
 
 @pytest.mark.nightly
 def test_segment_clip_edges_api():
     # Test with the clip_edges kwarg set to True:
     segmentation = seg.Segmentation(clip_edges=True)
 
-    fiber_groups = segmentation.segment(bundles,
-                                        tg,
-                                        mapping,
-                                        nib.load(hardi_fdata))
+    fiber_groups, _ = segmentation.segment(
+        bundles,
+        tg,
+        mapping,
+        nib.load(hardi_fdata))
 
     npt.assert_equal(len(fiber_groups), 2)
     npt.assert_(len(fiber_groups['Right Corticospinal']) > 0)
 
 
 def test_segment_reco():
     # get bundles for reco method
@@ -204,17 +205,17 @@
 
     # Try recobundles method
     segmentation = seg.Segmentation(seg_algo='Reco',
                                     progressive=False,
                                     greater_than=10,
                                     rm_small_clusters=1,
                                     rng=np.random.RandomState(seed=8))
-    fiber_groups = segmentation.segment(bundles_reco, tg,
-                                        mapping,
-                                        nib.load(hardi_fdata))
+    fiber_groups, _ = segmentation.segment(
+        bundles_reco, tg, mapping,
+        nib.load(hardi_fdata))
 
     # This condition should still hold
     npt.assert_equal(len(fiber_groups), 2)
     npt.assert_(len(fiber_groups['CST_R']) > 0)
 
 
 def test_clean_by_endpoints():
@@ -281,26 +282,26 @@
                     [8, 53, 39], [8, 50, 39], [8, 45, 39],
                     [30, 41, 61], [28, 61, 38]],
                 [
                     [8, 53, 39], [8, 50, 39], [8, 45, 39],
                     [30, 41, 62], [20, 44, 34]]
             ]).astype(float),
         hardi_img, Space.VOX)
-    fiber_groups = segmentation.segment(
+    fiber_groups, _ = segmentation.segment(
         slf_bundle,
         slf_tg,
         mapping,
         nib.load(hardi_fdata))
      
     npt.assert_equal(len(fiber_groups["Left Superior Longitudinal"]), 2)
 
     slf_bundle['Left Superior Longitudinal']['exclude'] =\
         [templates["SLFt_roi2_L"]]
 
-    fiber_groups = segmentation.segment(
+    fiber_groups, _ = segmentation.segment(
         slf_bundle,
         slf_tg,
         mapping,
         nib.load(hardi_fdata))
 
     npt.assert_equal(len(fiber_groups["Left Superior Longitudinal"]), 1)
 
@@ -320,15 +321,15 @@
     npt.assert_array_equal(cleaned_idx_tol, cleaned_idx)
 
 
 def test_segment_sampled_streamlines():
 
     # default segmentation
     segmentation = seg.Segmentation()
-    fiber_groups = segmentation.segment(
+    fiber_groups, _ = segmentation.segment(
         bundles,
         tg,
         mapping,
         nib.load(hardi_fdata))
 
     # Already using a subsampled tck
     # the Right Corticospinal has two streamlines and
@@ -339,15 +340,15 @@
     nb_streamlines = int(len(tg)*0.8)
 
     # sample and segment streamlines
     sampled_segmentation = seg.Segmentation(
         nb_streamlines=nb_streamlines
     )
 
-    sampled_fiber_groups = sampled_segmentation.segment(
+    sampled_fiber_groups, _ = sampled_segmentation.segment(
         bundles,
         tg,
         mapping,
         nib.load(hardi_fdata))
 
     # sampled streamlines should equal the sample number
     npt.assert_equal(len(sampled_segmentation.tg), nb_streamlines)
```

### Comparing `pyAFQ-1.3/AFQ/tests/test_tractography.py` & `pyAFQ-1.3.1/AFQ/tests/test_tractography.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tractography/gputractography.py` & `pyAFQ-1.3.1/AFQ/tractography/gputractography.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tractography/tractography.py` & `pyAFQ-1.3.1/AFQ/tractography/tractography.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/tractography/utils.py` & `pyAFQ-1.3.1/AFQ/tractography/utils.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/utils/bin.py` & `pyAFQ-1.3.1/AFQ/utils/bin.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/utils/conversion.py` & `pyAFQ-1.3.1/AFQ/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/utils/docs.py` & `pyAFQ-1.3.1/AFQ/utils/docs.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/utils/models.py` & `pyAFQ-1.3.1/AFQ/utils/models.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/utils/path.py` & `pyAFQ-1.3.1/AFQ/utils/path.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/utils/stats.py` & `pyAFQ-1.3.1/AFQ/utils/stats.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/utils/streamlines.py` & `pyAFQ-1.3.1/AFQ/utils/streamlines.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 except ModuleNotFoundError:
     has_trx = False
 
 from AFQ.utils.path import drop_extension, read_json
 
 
 class SegmentedSFT():
-    def __init__(self, bundles, space):
+    def __init__(self, bundles, space, sidecar_info={}):
         reference = None
         self.bundle_names = []
+        self.sidecar_info = sidecar_info
         sls = []
         idxs = {}
         this_tracking_idxs = []
         idx_count = 0
         for b_name in bundles:
             if isinstance(bundles[b_name], dict):
                 this_sls = bundles[b_name]['sl']
@@ -58,14 +59,18 @@
                 self.this_tracking_idxs[ii] = int(self.this_tracking_idxs[ii])
             sidecar_info["tracking_idx"] = self.this_tracking_idxs
         return self.sft, sidecar_info
 
     def get_bundle(self, b_name):
         return self.sft[self.bundle_idxs[b_name]]
 
+    def get_bundle_param_info(self, b_name):
+        return self.sidecar_info.get(
+            "Bundle Parameters", {}).get(b_name, {})
+
     @classmethod
     def fromfile(cls, trk_or_trx_file, reference="same", sidecar_file=None):
         if sidecar_file is None:
             # assume json sidecar has the same name as trk_file,
             # but with json suffix
             sidecar_file = f'{drop_extension(trk_or_trx_file)}.json'
             if not op.exists(sidecar_file):
@@ -96,15 +101,15 @@
                         idx = np.where(
                             sft.data_per_streamline['bundle'] == b_id)[0]
                         bundles[b_name] = StatefulTractogram(
                             sft.streamlines[idx], reference, Space.RASMM)
             else:
                 bundles["whole_brain"] = sft
 
-        return cls(bundles, Space.RASMM)
+        return cls(bundles, Space.RASMM, sidecar_info)
 
 
 def split_streamline(streamlines, sl_to_split, split_idx):
     """
     Given a Streamlines object, split one of the underlying streamlines
 
     Parameters
```

### Comparing `pyAFQ-1.3/AFQ/utils/testing.py` & `pyAFQ-1.3.1/AFQ/utils/testing.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/utils/tests/test_conversions.py` & `pyAFQ-1.3.1/AFQ/utils/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/utils/tests/test_streamlines.py` & `pyAFQ-1.3.1/AFQ/utils/tests/test_streamlines.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/utils/tests/test_volume.py` & `pyAFQ-1.3.1/AFQ/utils/tests/test_volume.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/utils/volume.py` & `pyAFQ-1.3.1/AFQ/utils/volume.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/viz/altair.py` & `pyAFQ-1.3.1/AFQ/viz/altair.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/viz/fury_backend.py` & `pyAFQ-1.3.1/AFQ/viz/fury_backend.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/viz/plot.py` & `pyAFQ-1.3.1/AFQ/viz/plot.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/viz/plotly_backend.py` & `pyAFQ-1.3.1/AFQ/viz/plotly_backend.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/AFQ/viz/utils.py` & `pyAFQ-1.3.1/AFQ/viz/utils.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/CHANGES.rst` & `pyAFQ-1.3.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+1.3.1 (April 04, 2024)
+======================
+Adds the mean signal diffusion kurtosis model as an option.
+Adds more information in JSON sidecars. Adds an explanation
+of our current bundle orientation system to the documentation.
+  * [ENH] add mean signal diffusion kurtosis model (#1121)
+  * [ENH] make source field relative in json sidecars (#1118)
+  * [ENH] add more information from bundle dict into jsons (#1117)
+  * [DOC] add bundle orientation explanation (#1120)
+
 1.3 (March 25, 2024)
 ====================
 All bundles are now ordered according to LPI+ and 
 are output as full names instead of abbreviations.
 Only the lowest shell is now used in the calculation of
 the CSD response function. Corrects typos in babyAFQ and
 GPU tracking, pARC/VOF cleaning parameters updated,
```

### Comparing `pyAFQ-1.3/LICENSE` & `pyAFQ-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/PKG-INFO` & `pyAFQ-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAFQ
-Version: 1.3
+Version: 1.3.1
 Summary: pyAFQ: Automated Fiber Quantification ... in Python
 Home-page: https://yeatmanlab.github.io/pyAFQ
 Download-URL: https://github.com/yeatmanlab/pyAFQ
 Author: pyAFQ developers
 Author-email: arokem@gmail.com
 Maintainer: Ariel Rokem
 Maintainer-email: arokem@gmail.com
```

### Comparing `pyAFQ-1.3/README.md` & `pyAFQ-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/bin/pyAFQ` & `pyAFQ-1.3.1/bin/pyAFQ`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/Makefile` & `pyAFQ-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/_progressbars.py` & `pyAFQ-1.3.1/docs/source/_progressbars.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/_static/BDE_Banner_revised20160211-01.jpg` & `pyAFQ-1.3.1/docs/source/_static/BDE_Banner_revised20160211-01.jpg`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/_static/custom.css` & `pyAFQ-1.3.1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/_static/eScience_Logo_HR.png` & `pyAFQ-1.3.1/docs/source/_static/eScience_Logo_HR.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/_static/escience-logo.png` & `pyAFQ-1.3.1/docs/source/_static/escience-logo.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/_static/logo.png` & `pyAFQ-1.3.1/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/conf.py` & `pyAFQ-1.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/explanations/_static/down_left_arrow.png` & `pyAFQ-1.3.1/docs/source/explanations/_static/down_left_arrow.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/explanations/_static/down_right_arrow.png` & `pyAFQ-1.3.1/docs/source/explanations/_static/down_right_arrow.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/explanations/_static/greencheck.png` & `pyAFQ-1.3.1/docs/source/explanations/_static/greencheck.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/explanations/_static/tract_modeling2.png` & `pyAFQ-1.3.1/docs/source/explanations/_static/tract_modeling2.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/explanations/_static/tract_profiling.png` & `pyAFQ-1.3.1/docs/source/explanations/_static/tract_profiling.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/explanations/_static/tract_recognition.png` & `pyAFQ-1.3.1/docs/source/explanations/_static/tract_recognition.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/explanations/_static/tract_tractography.png` & `pyAFQ-1.3.1/docs/source/explanations/_static/tract_tractography.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/explanations/index.rst` & `pyAFQ-1.3.1/docs/source/explanations/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -22,8 +22,9 @@
 properties within the tracts. To learn more about the software please refer to the Table of Contents.
 
 For further statistical analysis of pyAFQ results, see `AFQ-Insight <https://github.com/richford/AFQ-Insight>`_ .
 
 .. toctree::
     :maxdepth: 2
 
-    tractometry_pipeline
+    tractometry_pipeline
+    bundle_orientation
```

### Comparing `pyAFQ-1.3/docs/source/explanations/modeling.rst` & `pyAFQ-1.3.1/docs/source/explanations/modeling.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/explanations/profiling.rst` & `pyAFQ-1.3.1/docs/source/explanations/profiling.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/explanations/recognition.rst` & `pyAFQ-1.3.1/docs/source/explanations/recognition.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/explanations/tractography.rst` & `pyAFQ-1.3.1/docs/source/explanations/tractography.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/explanations/tractometry_pipeline.rst` & `pyAFQ-1.3.1/docs/source/explanations/tractometry_pipeline.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/cite.rst` & `pyAFQ-1.3.1/docs/source/howto/cite.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/contributing.rst` & `pyAFQ-1.3.1/docs/source/howto/contributing.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/developing/definitions.rst` & `pyAFQ-1.3.1/docs/source/howto/developing/definitions.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/developing/index.rst` & `pyAFQ-1.3.1/docs/source/howto/developing/index.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/developing/releasing.rst` & `pyAFQ-1.3.1/docs/source/howto/developing/releasing.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/developing/tasks.rst` & `pyAFQ-1.3.1/docs/source/howto/developing/tasks.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/getting_help.rst` & `pyAFQ-1.3.1/docs/source/howto/getting_help.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/installation_guide.rst` & `pyAFQ-1.3.1/docs/source/howto/installation_guide.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/usage/converter.rst` & `pyAFQ-1.3.1/docs/source/howto/usage/converter.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/usage/data.rst` & `pyAFQ-1.3.1/docs/source/howto/usage/data.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/usage/docker.rst` & `pyAFQ-1.3.1/docs/source/howto/usage/docker.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/usage/image.rst` & `pyAFQ-1.3.1/docs/source/howto/usage/image.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/usage/kwargs.rst` & `pyAFQ-1.3.1/docs/source/howto/usage/kwargs.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/usage/methods.rst` & `pyAFQ-1.3.1/docs/source/howto/usage/methods.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/howto/usage/scalars.rst` & `pyAFQ-1.3.1/docs/source/howto/usage/scalars.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/index.rst` & `pyAFQ-1.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/reference/bundledict.rst` & `pyAFQ-1.3.1/docs/source/reference/bundledict.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _bundle-dict-label:
+
 Defining Custom Bundle Dictionaries
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 pyAFQ has a system for defining custom bundles. Custom bundles are defined
 by passing a custom `bundle_info` dictionary to
 :class:`AFQ.api.bundle_dict.BundleDict`: The keys of `bundle_info` are bundle
 names; the values are another dictionary describing the bundle, with these
 key-value pairs::
```

### Comparing `pyAFQ-1.3/docs/source/reference/kwargs.rst` & `pyAFQ-1.3.1/docs/source/reference/kwargs.rst`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,19 @@
 	when calculating the tract-profiles. If callable, this is a
 	function that calculates weights. If None, no weighting will
 	be applied. If "gauss", gaussian weights will be used.
 	If "median", the median of values at each node will be used
 	instead of a mean or weighted mean.
 	Default: "gauss"
 
+n_points_profile: int, optional
+	Number of points to resample each streamline to before
+	calculating the tract-profiles.
+	Default: 100
+
 scalars: strings and/or scalar definitions, optional
 	List of scalars to use.
 	Can be any of: "dti_fa", "dti_md", "dki_fa", "dki_md", "dki_awf",
 	"dki_mk". Can also be a scalar from AFQ.definitions.image.
 	Default: ["dti_fa", "dti_md"]
 
 
@@ -181,14 +186,18 @@
 
 tractography_ngpus: int, optional
 	Number of GPUs to use in tractography. If non-0,
 	this algorithm is used for tractography,
 	https://github.com/dipy/GPUStreamlines
 	Default: 0
 
+chunk_size: int, optional
+	Chunk size for GPU tracking.
+	Default: 100000
+
 
 ==========================================================
 VIZ
 ==========================================================
 sbv_lims_bundles: ndarray
 	Of the form (lower bound, upper bound). Shading based on
 	shade_by_volume will only differentiate values within these bounds.
```

### Comparing `pyAFQ-1.3/docs/source/reference/mapping.rst` & `pyAFQ-1.3.1/docs/source/reference/mapping.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/reference/methods.rst` & `pyAFQ-1.3.1/docs/source/reference/methods.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,20 @@
     DWI data as an ndarray for selected b values
 
 
 gtab:
     A DIPY GradientTable with all the gradient information
 
 
-img:
-    unaltered DWI data in a Nifti1Image.
+dwi:
+    DWI data in a Nifti1Image
+
+
+dwi_affine:
+    the affine transformation of the DWI data.
 
 
 b0:
     full path to a nifti file containing the mean b0
 
 
 masked_b0:
@@ -279,14 +283,18 @@
     full path to a nifti file containing the DKI axonal water fraction
 
 
 dki_mk:
     full path to a nifti file containing the DKI mean kurtosis file
 
 
+dki_kfa:
+    full path to a nifti file containing the DKI kurtosis FA file
+
+
 dki_ga:
     full path to a nifti file containing the DKI geodesic anisotropy
 
 
 dki_rd:
     full path to a nifti file containing the DKI radial diffusivity
```

### Comparing `pyAFQ-1.3/docs/source/reference/viz_backend.rst` & `pyAFQ-1.3.1/docs/source/reference/viz_backend.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/sphinxext/kwargsdocs.py` & `pyAFQ-1.3.1/docs/source/sphinxext/kwargsdocs.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/sphinxext/methodsdocs.py` & `pyAFQ-1.3.1/docs/source/sphinxext/methodsdocs.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/sphinxext/updatedocs.py` & `pyAFQ-1.3.1/docs/source/sphinxext/updatedocs.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/source/tutorials/index.rst` & `pyAFQ-1.3.1/docs/source/tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/docs/upload-gh-pages.sh` & `pyAFQ-1.3.1/docs/upload-gh-pages.sh`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/howto_examples/add_custom_bundle.py` & `pyAFQ-1.3.1/examples/howto_examples/add_custom_bundle.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/howto_examples/baby_afq.py` & `pyAFQ-1.3.1/examples/howto_examples/baby_afq.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/howto_examples/cerebellar_peduncles.py` & `pyAFQ-1.3.1/examples/howto_examples/cerebellar_peduncles.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/howto_examples/cloudknot_example.py` & `pyAFQ-1.3.1/examples/howto_examples/cloudknot_example.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/howto_examples/cloudknot_hcp_example.py` & `pyAFQ-1.3.1/examples/howto_examples/cloudknot_hcp_example.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/howto_examples/plot_acoustic_radiations.py` & `pyAFQ-1.3.1/examples/howto_examples/plot_acoustic_radiations.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/howto_examples/plot_afq_callosal.py` & `pyAFQ-1.3.1/examples/howto_examples/plot_afq_callosal.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/howto_examples/plot_afq_fwdti.py` & `pyAFQ-1.3.1/examples/howto_examples/plot_afq_fwdti.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/howto_examples/plot_optic_radiations.py` & `pyAFQ-1.3.1/examples/howto_examples/plot_optic_radiations.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/howto_examples/plot_recobundles.py` & `pyAFQ-1.3.1/examples/howto_examples/plot_recobundles.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/howto_examples/plot_stages_of_tractometry.py` & `pyAFQ-1.3.1/examples/howto_examples/plot_stages_of_tractometry.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/howto_examples/use_subject_space_rois_from_freesurfer.py` & `pyAFQ-1.3.1/examples/howto_examples/use_subject_space_rois_from_freesurfer.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/howto_examples/vof_example.py` & `pyAFQ-1.3.1/examples/howto_examples/vof_example.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/tutorial_examples/plot_001_afq_api.py` & `pyAFQ-1.3.1/examples/tutorial_examples/plot_001_afq_api.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/tutorial_examples/plot_002_bids_layout.py` & `pyAFQ-1.3.1/examples/tutorial_examples/plot_002_bids_layout.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/examples/tutorial_examples/plot_003_viz.py` & `pyAFQ-1.3.1/examples/tutorial_examples/plot_003_viz.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/gpu_docker/Dockerfile` & `pyAFQ-1.3.1/gpu_docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/gpu_docker/cuda_track_template.def` & `pyAFQ-1.3.1/gpu_docker/cuda_track_template.def`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/pyAFQ.egg-info/PKG-INFO` & `pyAFQ-1.3.1/pyAFQ.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAFQ
-Version: 1.3
+Version: 1.3.1
 Summary: pyAFQ: Automated Fiber Quantification ... in Python
 Home-page: https://yeatmanlab.github.io/pyAFQ
 Download-URL: https://github.com/yeatmanlab/pyAFQ
 Author: pyAFQ developers
 Author-email: arokem@gmail.com
 Maintainer: Ariel Rokem
 Maintainer-email: arokem@gmail.com
```

### Comparing `pyAFQ-1.3/pyAFQ.egg-info/SOURCES.txt` & `pyAFQ-1.3.1/pyAFQ.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,15 @@
 docs/source/index.rst
 docs/source/_static/BDE_Banner_revised20160211-01.jpg
 docs/source/_static/custom.css
 docs/source/_static/eScience_Logo_HR.png
 docs/source/_static/escience-logo.png
 docs/source/_static/logo.png
 docs/source/_templates/layout.html
+docs/source/explanations/bundle_orientation.rst
 docs/source/explanations/index.rst
 docs/source/explanations/modeling.rst
 docs/source/explanations/profiling.rst
 docs/source/explanations/recognition.rst
 docs/source/explanations/tractography.rst
 docs/source/explanations/tractometry_pipeline.rst
 docs/source/explanations/_static/down_left_arrow.png
```

### Comparing `pyAFQ-1.3/pyAFQ.egg-info/requires.txt` & `pyAFQ-1.3.1/pyAFQ.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/setup.cfg` & `pyAFQ-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3/setup.py` & `pyAFQ-1.3.1/setup.py`

 * *Files identical despite different names*

