# Comparing `tmp/spyrmsd-0.6.0.tar.gz` & `tmp/spyrmsd-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyrmsd-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "spyrmsd-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spyrmsd-0.6.0.tar` & `spyrmsd-0.7.0.tar`

### file list

```diff
@@ -1,221 +1,221 @@
--rw-r--r--   0        0        0      258 2023-09-08 20:18:54.963353 spyrmsd-0.6.0/.codecov.yml
--rw-r--r--   0        0        0      315 2023-09-08 20:18:54.964001 spyrmsd-0.6.0/.coveragerc
--rw-r--r--   0        0        0       33 2023-09-08 20:18:54.964183 spyrmsd-0.6.0/.gitattributes
--rw-r--r--   0        0        0     2245 2023-09-08 20:18:54.964482 spyrmsd-0.6.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      604 2023-06-28 16:31:38.578680 spyrmsd-0.6.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      547 2023-09-08 20:18:54.964727 spyrmsd-0.6.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0       81 2023-09-08 20:18:54.964985 spyrmsd-0.6.0/.github/ISSUE_TEMPLATE/empty-issue.md
--rw-r--r--   0        0        0      142 2023-06-28 16:31:38.578935 spyrmsd-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      742 2023-09-08 20:18:54.965242 spyrmsd-0.6.0/.github/workflows/flake8.yml
--rw-r--r--   0        0        0      781 2023-09-08 20:18:54.965472 spyrmsd-0.6.0/.github/workflows/mypy.yml
--rw-r--r--   0        0        0      470 2023-09-08 20:18:54.965845 spyrmsd-0.6.0/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      636 2023-09-08 20:18:54.966117 spyrmsd-0.6.0/.github/workflows/pypi.yml
--rw-r--r--   0        0        0     1898 2023-09-08 20:18:54.966607 spyrmsd-0.6.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      948 2023-06-28 16:31:38.579337 spyrmsd-0.6.0/.gitignore
--rw-r--r--   0        0        0      162 2023-06-28 16:31:38.579407 spyrmsd-0.6.0/.lgtm.yml
--rw-r--r--   0        0        0      755 2023-09-08 20:18:54.967004 spyrmsd-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      292 2023-09-08 20:18:54.967265 spyrmsd-0.6.0/.readthedocs.yml
--rw-r--r--   0        0        0     3244 2023-09-08 20:18:54.967544 spyrmsd-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      723 2023-09-08 20:18:54.967806 spyrmsd-0.6.0/CITATION.cff
--rw-r--r--   0        0        0     3562 2023-06-28 16:31:38.579779 spyrmsd-0.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1073 2023-06-28 16:31:38.579847 spyrmsd-0.6.0/LICENSE
--rw-r--r--   0        0        0      115 2023-09-08 20:18:54.968028 spyrmsd-0.6.0/MANIFEST.in
--rw-r--r--   0        0        0     7141 2023-09-08 20:18:54.968466 spyrmsd-0.6.0/README.md
--rw-r--r--   0        0        0      126 2023-09-08 20:18:54.968712 spyrmsd-0.6.0/credits.sh
--rw-r--r--   0        0        0      843 2023-09-08 20:18:54.969015 spyrmsd-0.6.0/devtools/README.md
--rw-r--r--   0        0        0      503 2023-09-08 20:18:54.969519 spyrmsd-0.6.0/devtools/conda-envs/spyrmsd-all.yaml
--rw-r--r--   0        0        0      228 2023-09-08 20:18:54.969993 spyrmsd-0.6.0/devtools/conda-envs/spyrmsd-docs.yaml
--rw-r--r--   0        0        0      260 2023-06-28 16:31:38.580418 spyrmsd-0.6.0/devtools/conda-envs/spyrmsd-test-obabel-gt.yaml
--rw-r--r--   0        0        0      261 2023-06-28 16:31:38.580480 spyrmsd-0.6.0/devtools/conda-envs/spyrmsd-test-obabel-nx.yaml
--rw-r--r--   0        0        0      266 2023-06-28 16:31:38.580541 spyrmsd-0.6.0/devtools/conda-envs/spyrmsd-test-rdkit-gt.yaml
--rw-r--r--   0        0        0      267 2023-06-28 16:31:38.580598 spyrmsd-0.6.0/devtools/conda-envs/spyrmsd-test-rdkit-nx.yaml
--rw-r--r--   0        0        0      120 2023-06-28 16:31:38.580659 spyrmsd-0.6.0/devtools/conda-envs/spyrmsd.yaml
--rw-r--r--   0        0        0      636 2023-06-28 16:31:38.580769 spyrmsd-0.6.0/docs/Makefile
--rw-r--r--   0        0        0      997 2023-09-08 20:18:54.970301 spyrmsd-0.6.0/docs/README.md
--rw-r--r--   0        0        0      799 2023-06-28 16:31:38.580912 spyrmsd-0.6.0/docs/make.bat
--rw-r--r--   0        0        0       77 2023-09-08 20:18:54.970516 spyrmsd-0.6.0/docs/source/api.rst
--rw-r--r--   0        0        0      139 2023-06-28 16:31:38.581108 spyrmsd-0.6.0/docs/source/api/spyrmsd.constants.rst
--rw-r--r--   0        0        0      121 2023-06-28 16:31:38.581177 spyrmsd-0.6.0/docs/source/api/spyrmsd.due.rst
--rw-r--r--   0        0        0      142 2023-06-28 16:31:38.581242 spyrmsd-0.6.0/docs/source/api/spyrmsd.exceptions.rst
--rw-r--r--   0        0        0      127 2023-06-28 16:31:38.581303 spyrmsd-0.6.0/docs/source/api/spyrmsd.graph.rst
--rw-r--r--   0        0        0      139 2023-06-28 16:31:38.581361 spyrmsd-0.6.0/docs/source/api/spyrmsd.graphs.gt.rst
--rw-r--r--   0        0        0      139 2023-06-28 16:31:38.581429 spyrmsd-0.6.0/docs/source/api/spyrmsd.graphs.nx.rst
--rw-r--r--   0        0        0      228 2023-06-28 16:31:38.581492 spyrmsd-0.6.0/docs/source/api/spyrmsd.graphs.rst
--rw-r--r--   0        0        0      139 2023-06-28 16:31:38.581551 spyrmsd-0.6.0/docs/source/api/spyrmsd.hungarian.rst
--rw-r--r--   0        0        0      118 2023-06-28 16:31:38.581609 spyrmsd-0.6.0/docs/source/api/spyrmsd.io.rst
--rw-r--r--   0        0        0      136 2023-06-28 16:31:38.581668 spyrmsd-0.6.0/docs/source/api/spyrmsd.molecule.rst
--rw-r--r--   0        0        0      157 2023-06-28 16:31:38.581738 spyrmsd-0.6.0/docs/source/api/spyrmsd.optional.obabel.rst
--rw-r--r--   0        0        0      154 2023-06-28 16:31:38.581802 spyrmsd-0.6.0/docs/source/api/spyrmsd.optional.rdkit.rst
--rw-r--r--   0        0        0      245 2023-06-28 16:31:38.581863 spyrmsd-0.6.0/docs/source/api/spyrmsd.optional.rst
--rw-r--r--   0        0        0      121 2023-06-28 16:31:38.581924 spyrmsd-0.6.0/docs/source/api/spyrmsd.qcp.rst
--rw-r--r--   0        0        0      124 2023-06-28 16:31:38.581991 spyrmsd-0.6.0/docs/source/api/spyrmsd.rmsd.rst
--rw-r--r--   0        0        0      437 2023-06-28 16:31:38.582058 spyrmsd-0.6.0/docs/source/api/spyrmsd.rst
--rw-r--r--   0        0        0      127 2023-06-28 16:31:38.582113 spyrmsd-0.6.0/docs/source/api/spyrmsd.utils.rst
--rw-r--r--   0        0        0     5319 2023-06-28 17:02:23.254959 spyrmsd-0.6.0/docs/source/conf.py
--rw-r--r--   0        0        0      307 2023-06-28 16:31:38.582275 spyrmsd-0.6.0/docs/source/index.rst
--rw-r--r--   0        0        0     1502 2023-09-08 20:18:54.970764 spyrmsd-0.6.0/docs/source/installation.rst
--rw-r--r--   0        0        0    31852 2023-06-28 16:31:38.582717 spyrmsd-0.6.0/docs/source/tutorials/molecules/1a4k_dock.sdf
--rw-r--r--   0        0        0     4286 2023-06-28 16:31:38.582848 spyrmsd-0.6.0/docs/source/tutorials/molecules/1a4k_ligand.sdf
--rw-r--r--   0        0        0     7303 2023-09-08 20:18:54.971045 spyrmsd-0.6.0/docs/source/tutorials/tutorial.ipynb
--rw-r--r--   0        0        0     3868 2023-09-08 20:18:54.971296 spyrmsd-0.6.0/docs/source/tutorials/tutorial.rst
--rw-r--r--   0        0        0      441 2023-09-08 20:18:54.971498 spyrmsd-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      772 2023-09-08 20:18:54.971730 spyrmsd-0.6.0/setup.cfg
--rw-r--r--   0        0        0     1074 2023-09-08 20:18:54.971961 spyrmsd-0.6.0/setup.py
--rw-r--r--   0        0        0      470 2023-09-08 20:28:34.722575 spyrmsd-0.6.0/spyrmsd/__init__.py
--rw-r--r--   0        0        0     1906 2023-09-08 20:18:54.972346 spyrmsd-0.6.0/spyrmsd/__main__.py
--rw-r--r--   0        0        0    23716 2023-09-08 20:18:54.972657 spyrmsd-0.6.0/spyrmsd/_version.py
--rw-r--r--   0        0        0     4173 2023-06-28 16:31:38.584035 spyrmsd-0.6.0/spyrmsd/constants.py
--rw-r--r--   0        0        0     2019 2023-09-08 20:18:54.972845 spyrmsd-0.6.0/spyrmsd/due.py
--rw-r--r--   0        0        0      107 2023-06-28 16:31:38.584215 spyrmsd-0.6.0/spyrmsd/exceptions.py
--rw-r--r--   0        0        0     2292 2023-06-28 16:31:38.584300 spyrmsd-0.6.0/spyrmsd/graph.py
--rw-r--r--   0        0        0        0 2023-06-28 16:31:38.584370 spyrmsd-0.6.0/spyrmsd/graphs/__init__.py
--rw-r--r--   0        0        0      324 2023-06-28 16:31:38.584453 spyrmsd-0.6.0/spyrmsd/graphs/_common.py
--rw-r--r--   0        0        0     4802 2023-09-06 19:28:10.754704 spyrmsd-0.6.0/spyrmsd/graphs/gt.py
--rw-r--r--   0        0        0     3699 2023-06-28 16:31:38.584632 spyrmsd-0.6.0/spyrmsd/graphs/nx.py
--rw-r--r--   0        0        0     2878 2023-09-08 20:18:54.973013 spyrmsd-0.6.0/spyrmsd/hungarian.py
--rw-r--r--   0        0        0     1649 2023-09-08 20:18:54.973184 spyrmsd-0.6.0/spyrmsd/io.py
--rw-r--r--   0        0        0     6913 2023-06-28 16:31:38.584883 spyrmsd-0.6.0/spyrmsd/molecule.py
--rw-r--r--   0        0        0      197 2023-06-28 16:31:38.585004 spyrmsd-0.6.0/spyrmsd/optional/__init__.py
--rw-r--r--   0        0        0     3160 2023-09-08 20:18:54.973414 spyrmsd-0.6.0/spyrmsd/optional/obabel.py
--rw-r--r--   0        0        0     4465 2023-06-28 16:31:38.585188 spyrmsd-0.6.0/spyrmsd/optional/rdkit.py
--rw-r--r--   0        0        0     7125 2023-09-08 20:18:54.973616 spyrmsd-0.6.0/spyrmsd/qcp.py
--rw-r--r--   0        0        0    10000 2023-09-08 20:18:54.973812 spyrmsd-0.6.0/spyrmsd/rmsd.py
--rw-r--r--   0        0        0     3418 2023-06-28 16:31:38.585479 spyrmsd-0.6.0/spyrmsd/utils.py
--rw-r--r--   0        0        0        0 2023-06-28 16:31:38.585549 spyrmsd-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     2029 2023-06-28 16:31:38.585644 spyrmsd-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0      510 2023-09-08 20:18:54.974035 spyrmsd-0.6.0/tests/data/README.md
--rw-r--r--   0        0        0     6610 2023-06-28 16:31:38.585919 spyrmsd-0.6.0/tests/data/docking/1a28/1a28_dock.sdf
--rw-r--r--   0        0        0     3431 2023-06-28 16:31:38.586016 spyrmsd-0.6.0/tests/data/docking/1a28/1a28_ligand.sdf
--rw-r--r--   0        0        0       29 2023-06-28 16:31:38.586083 spyrmsd-0.6.0/tests/data/docking/1a28/obrms-min.dat
--rw-r--r--   0        0        0       25 2023-06-28 16:31:38.586144 spyrmsd-0.6.0/tests/data/docking/1a28/obrms.dat
--rw-r--r--   0        0        0    31852 2023-06-28 16:31:38.586326 spyrmsd-0.6.0/tests/data/docking/1a4k/1a4k_dock.sdf
--rw-r--r--   0        0        0     4286 2023-06-28 16:31:38.586431 spyrmsd-0.6.0/tests/data/docking/1a4k/1a4k_ligand.sdf
--rw-r--r--   0        0        0       83 2023-06-28 16:31:38.586492 spyrmsd-0.6.0/tests/data/docking/1a4k/obrms-min.dat
--rw-r--r--   0        0        0       76 2023-06-28 16:31:38.586551 spyrmsd-0.6.0/tests/data/docking/1a4k/obrms.dat
--rw-r--r--   0        0        0    34320 2023-06-28 16:31:38.586735 spyrmsd-0.6.0/tests/data/docking/1a4r/1a4r_dock.sdf
--rw-r--r--   0        0        0     4025 2023-06-28 16:31:38.586825 spyrmsd-0.6.0/tests/data/docking/1a4r/1a4r_ligand.sdf
--rw-r--r--   0        0        0       81 2023-06-28 16:31:38.586887 spyrmsd-0.6.0/tests/data/docking/1a4r/obrms-min.dat
--rw-r--r--   0        0        0       81 2023-06-28 16:31:38.586950 spyrmsd-0.6.0/tests/data/docking/1a4r/obrms.dat
--rw-r--r--   0        0        0    22750 2023-06-28 16:31:38.587303 spyrmsd-0.6.0/tests/data/docking/1a69/1a69_dock.sdf
--rw-r--r--   0        0        0     2973 2023-06-28 16:31:38.587393 spyrmsd-0.6.0/tests/data/docking/1a69/1a69_ligand.sdf
--rw-r--r--   0        0        0       86 2023-06-28 16:31:38.587448 spyrmsd-0.6.0/tests/data/docking/1a69/obrms-min.dat
--rw-r--r--   0        0        0       80 2023-06-28 16:31:38.587502 spyrmsd-0.6.0/tests/data/docking/1a69/obrms.dat
--rw-r--r--   0        0        0    67930 2023-06-28 16:31:38.587773 spyrmsd-0.6.0/tests/data/docking/1a94/1a94_dock.sdf
--rw-r--r--   0        0        0     7748 2023-06-28 16:31:38.587877 spyrmsd-0.6.0/tests/data/docking/1a94/1a94_ligand.sdf
--rw-r--r--   0        0        0       80 2023-06-28 16:31:38.587946 spyrmsd-0.6.0/tests/data/docking/1a94/obrms-min.dat
--rw-r--r--   0        0        0       80 2023-06-28 16:31:38.588004 spyrmsd-0.6.0/tests/data/docking/1a94/obrms.dat
--rw-r--r--   0        0        0     7776 2023-06-28 16:31:38.588232 spyrmsd-0.6.0/tests/data/docking/1a99/1a99_dock.sdf
--rw-r--r--   0        0        0     1347 2023-06-28 16:31:38.588319 spyrmsd-0.6.0/tests/data/docking/1a99/1a99_ligand.sdf
--rw-r--r--   0        0        0       69 2023-06-28 16:31:38.588375 spyrmsd-0.6.0/tests/data/docking/1a99/obrms-min.dat
--rw-r--r--   0        0        0       64 2023-06-28 16:31:38.588428 spyrmsd-0.6.0/tests/data/docking/1a99/obrms.dat
--rw-r--r--   0        0        0    49070 2023-06-28 16:31:38.588560 spyrmsd-0.6.0/tests/data/docking/1a9m/1a9m_dock.sdf
--rw-r--r--   0        0        0     5591 2023-06-28 16:31:38.588652 spyrmsd-0.6.0/tests/data/docking/1a9m/1a9m_ligand.sdf
--rw-r--r--   0        0        0       78 2023-06-28 16:31:38.588707 spyrmsd-0.6.0/tests/data/docking/1a9m/obrms-min.dat
--rw-r--r--   0        0        0       80 2023-06-28 16:31:38.588761 spyrmsd-0.6.0/tests/data/docking/1a9m/obrms.dat
--rw-r--r--   0        0        0    11880 2023-06-28 16:31:38.588893 spyrmsd-0.6.0/tests/data/docking/1a9q/1a9q_dock.sdf
--rw-r--r--   0        0        0     1833 2023-06-28 16:31:38.588955 spyrmsd-0.6.0/tests/data/docking/1a9q/1a9q_ligand.sdf
--rw-r--r--   0        0        0      120 2023-06-28 16:31:38.589010 spyrmsd-0.6.0/tests/data/docking/1a9q/obrms-min.dat
--rw-r--r--   0        0        0       80 2023-06-28 16:31:38.589067 spyrmsd-0.6.0/tests/data/docking/1a9q/obrms.dat
--rw-r--r--   0        0        0    43730 2023-06-28 16:31:38.589202 spyrmsd-0.6.0/tests/data/docking/1aaq/1aaq_dock.sdf
--rw-r--r--   0        0        0     5521 2023-06-28 16:31:38.589300 spyrmsd-0.6.0/tests/data/docking/1aaq/1aaq_ligand.sdf
--rw-r--r--   0        0        0       80 2023-06-28 16:31:38.589355 spyrmsd-0.6.0/tests/data/docking/1aaq/obrms-min.dat
--rw-r--r--   0        0        0       77 2023-06-28 16:31:38.589410 spyrmsd-0.6.0/tests/data/docking/1aaq/obrms.dat
--rw-r--r--   0        0        0    11375 2023-06-28 16:31:38.589602 spyrmsd-0.6.0/tests/data/docking/1add/1add_dock.sdf
--rw-r--r--   0        0        0     2955 2023-06-28 16:31:38.589676 spyrmsd-0.6.0/tests/data/docking/1add/1add_ligand.sdf
--rw-r--r--   0        0        0       42 2023-06-28 16:31:38.589733 spyrmsd-0.6.0/tests/data/docking/1add/obrms-min.dat
--rw-r--r--   0        0        0       41 2023-06-28 16:31:38.589786 spyrmsd-0.6.0/tests/data/docking/1add/obrms.dat
--rw-r--r--   0        0        0    21290 2023-06-28 16:31:38.589933 spyrmsd-0.6.0/tests/data/docking/1adl/1adl_dock.sdf
--rw-r--r--   0        0        0     3162 2023-06-28 16:31:38.590022 spyrmsd-0.6.0/tests/data/docking/1adl/1adl_ligand.sdf
--rw-r--r--   0        0        0       78 2023-06-28 16:31:38.590082 spyrmsd-0.6.0/tests/data/docking/1adl/obrms-min.dat
--rw-r--r--   0        0        0       78 2023-06-28 16:31:38.590143 spyrmsd-0.6.0/tests/data/docking/1adl/obrms.dat
--rw-r--r--   0        0        0    12400 2023-06-28 16:31:38.590262 spyrmsd-0.6.0/tests/data/docking/1ado/1ado_dock.sdf
--rw-r--r--   0        0        0     1829 2023-06-28 16:31:38.590330 spyrmsd-0.6.0/tests/data/docking/1ado/1ado_ligand.sdf
--rw-r--r--   0        0        0       85 2023-06-28 16:31:38.590383 spyrmsd-0.6.0/tests/data/docking/1ado/obrms-min.dat
--rw-r--r--   0        0        0       78 2023-06-28 16:31:38.590436 spyrmsd-0.6.0/tests/data/docking/1ado/obrms.dat
--rw-r--r--   0        0        0    36100 2023-06-28 16:31:38.590706 spyrmsd-0.6.0/tests/data/docking/1afk/1afk_dock.sdf
--rw-r--r--   0        0        0     4340 2023-06-28 16:31:38.590818 spyrmsd-0.6.0/tests/data/docking/1afk/1afk_ligand.sdf
--rw-r--r--   0        0        0       81 2023-06-28 16:31:38.590880 spyrmsd-0.6.0/tests/data/docking/1afk/obrms-min.dat
--rw-r--r--   0        0        0       79 2023-06-28 16:31:38.590940 spyrmsd-0.6.0/tests/data/docking/1afk/obrms.dat
--rw-r--r--   0        0        0    36100 2023-06-28 16:31:38.591070 spyrmsd-0.6.0/tests/data/docking/1afl/1afl_dock.sdf
--rw-r--r--   0        0        0     4346 2023-06-28 16:31:38.591142 spyrmsd-0.6.0/tests/data/docking/1afl/1afl_ligand.sdf
--rw-r--r--   0        0        0       80 2023-06-28 16:31:38.591200 spyrmsd-0.6.0/tests/data/docking/1afl/obrms-min.dat
--rw-r--r--   0        0        0       80 2023-06-28 16:31:38.591256 spyrmsd-0.6.0/tests/data/docking/1afl/obrms.dat
--rw-r--r--   0        0        0    14360 2023-06-28 16:31:38.591408 spyrmsd-0.6.0/tests/data/docking/1ai4/1ai4_dock.sdf
--rw-r--r--   0        0        0     2053 2023-06-28 16:31:38.591492 spyrmsd-0.6.0/tests/data/docking/1ai4/1ai4_ligand.sdf
--rw-r--r--   0        0        0       89 2023-06-28 16:31:38.591551 spyrmsd-0.6.0/tests/data/docking/1ai4/obrms-min.dat
--rw-r--r--   0        0        0       79 2023-06-28 16:31:38.591606 spyrmsd-0.6.0/tests/data/docking/1ai4/obrms.dat
--rw-r--r--   0        0        0    13810 2023-06-28 16:31:38.591734 spyrmsd-0.6.0/tests/data/docking/1ai5/1ai5_dock.sdf
--rw-r--r--   0        0        0     2191 2023-06-28 16:31:38.591790 spyrmsd-0.6.0/tests/data/docking/1ai5/1ai5_ligand.sdf
--rw-r--r--   0        0        0       86 2023-06-28 16:31:38.591844 spyrmsd-0.6.0/tests/data/docking/1ai5/obrms-min.dat
--rw-r--r--   0        0        0       79 2023-06-28 16:31:38.591896 spyrmsd-0.6.0/tests/data/docking/1ai5/obrms.dat
--rw-r--r--   0        0        0     8130 2023-06-28 16:31:38.591992 spyrmsd-0.6.0/tests/data/docking/1ai7/1ai7_dock.sdf
--rw-r--r--   0        0        0     1441 2023-06-28 16:31:38.592088 spyrmsd-0.6.0/tests/data/docking/1ai7/1ai7_ligand.sdf
--rw-r--r--   0        0        0      120 2023-06-28 16:31:38.592145 spyrmsd-0.6.0/tests/data/docking/1ai7/obrms-min.dat
--rw-r--r--   0        0        0       81 2023-06-28 16:31:38.592203 spyrmsd-0.6.0/tests/data/docking/1ai7/obrms.dat
--rw-r--r--   0        0        0    28280 2023-06-28 16:31:38.592367 spyrmsd-0.6.0/tests/data/docking/1aid/1aid_dock.sdf
--rw-r--r--   0        0        0     4086 2023-06-28 16:31:38.592431 spyrmsd-0.6.0/tests/data/docking/1aid/1aid_ligand.sdf
--rw-r--r--   0        0        0       78 2023-06-28 16:31:38.592484 spyrmsd-0.6.0/tests/data/docking/1aid/obrms-min.dat
--rw-r--r--   0        0        0       79 2023-06-28 16:31:38.592536 spyrmsd-0.6.0/tests/data/docking/1aid/obrms.dat
--rw-r--r--   0        0        0    20210 2023-06-28 16:31:38.592685 spyrmsd-0.6.0/tests/data/docking/1aj7/1aj7_dock.sdf
--rw-r--r--   0        0        0     3017 2023-06-28 16:31:38.592772 spyrmsd-0.6.0/tests/data/docking/1aj7/1aj7_ligand.sdf
--rw-r--r--   0        0        0       80 2023-06-28 16:31:38.592827 spyrmsd-0.6.0/tests/data/docking/1aj7/obrms-min.dat
--rw-r--r--   0        0        0       81 2023-06-28 16:31:38.592882 spyrmsd-0.6.0/tests/data/docking/1aj7/obrms.dat
--rw-r--r--   0        0        0    13810 2023-06-28 16:31:38.593022 spyrmsd-0.6.0/tests/data/docking/1ajn/1ajn_dock.sdf
--rw-r--r--   0        0        0     2189 2023-06-28 16:31:38.593116 spyrmsd-0.6.0/tests/data/docking/1ajn/1ajn_ligand.sdf
--rw-r--r--   0        0        0       89 2023-06-28 16:31:38.593169 spyrmsd-0.6.0/tests/data/docking/1ajn/obrms-min.dat
--rw-r--r--   0        0        0       79 2023-06-28 16:31:38.593223 spyrmsd-0.6.0/tests/data/docking/1ajn/obrms.dat
--rw-r--r--   0        0        0    14360 2023-06-28 16:31:38.593356 spyrmsd-0.6.0/tests/data/docking/1ajp/1ajp_dock.sdf
--rw-r--r--   0        0        0     2078 2023-06-28 16:31:38.593423 spyrmsd-0.6.0/tests/data/docking/1ajp/1ajp_ligand.sdf
--rw-r--r--   0        0        0       90 2023-06-28 16:31:38.593477 spyrmsd-0.6.0/tests/data/docking/1ajp/obrms-min.dat
--rw-r--r--   0        0        0       80 2023-06-28 16:31:38.593539 spyrmsd-0.6.0/tests/data/docking/1ajp/obrms.dat
--rw-r--r--   0        0        0     9910 2023-06-28 16:31:38.593669 spyrmsd-0.6.0/tests/data/docking/1ajq/1ajq_dock.sdf
--rw-r--r--   0        0        0     1709 2023-06-28 16:31:38.593734 spyrmsd-0.6.0/tests/data/docking/1ajq/1ajq_ligand.sdf
--rw-r--r--   0        0        0       85 2023-06-28 16:31:38.593796 spyrmsd-0.6.0/tests/data/docking/1ajq/obrms-min.dat
--rw-r--r--   0        0        0       81 2023-06-28 16:31:38.593861 spyrmsd-0.6.0/tests/data/docking/1ajq/obrms.dat
--rw-r--r--   0        0        0    12015 2023-06-28 16:31:38.594023 spyrmsd-0.6.0/tests/data/docking/1ajv/1ajv_dock.sdf
--rw-r--r--   0        0        0     5461 2023-06-28 16:31:38.594141 spyrmsd-0.6.0/tests/data/docking/1ajv/1ajv_ligand.sdf
--rw-r--r--   0        0        0       25 2023-06-28 16:31:38.594206 spyrmsd-0.6.0/tests/data/docking/1ajv/obrms-min.dat
--rw-r--r--   0        0        0       25 2023-06-28 16:31:38.594273 spyrmsd-0.6.0/tests/data/docking/1ajv/obrms.dat
--rw-r--r--   0        0        0    39156 2023-06-28 16:31:38.594392 spyrmsd-0.6.0/tests/data/docking/1ajx/1ajx_dock.sdf
--rw-r--r--   0        0        0     5343 2023-06-28 16:31:38.594471 spyrmsd-0.6.0/tests/data/docking/1ajx/1ajx_ligand.sdf
--rw-r--r--   0        0        0       82 2023-06-28 16:31:38.594539 spyrmsd-0.6.0/tests/data/docking/1ajx/obrms-min.dat
--rw-r--r--   0        0        0       78 2023-06-28 16:31:38.594602 spyrmsd-0.6.0/tests/data/docking/1ajx/obrms.dat
--rw-r--r--   0        0        0     2112 2023-09-08 20:18:54.974245 spyrmsd-0.6.0/tests/data/molecules/1a99_ligand.pdb
--rw-r--r--   0        0        0      568 2023-06-28 16:31:38.594801 spyrmsd-0.6.0/tests/data/molecules/1a99_ligand.pdb.gz
--rw-r--r--   0        0        0    23500 2023-06-28 16:31:38.594929 spyrmsd-0.6.0/tests/data/molecules/1cbr_docking.mol2
--rw-r--r--   0        0        0    24394 2023-09-08 20:18:54.974522 spyrmsd-0.6.0/tests/data/molecules/1cbr_docking.pdb
--rw-r--r--   0        0        0    20730 2023-06-28 16:31:38.595301 spyrmsd-0.6.0/tests/data/molecules/1cbr_docking.sdf
--rw-r--r--   0        0        0     3283 2023-06-28 16:31:38.595374 spyrmsd-0.6.0/tests/data/molecules/1cbr_docking.sdf.gz
--rwxr-xr-x   0        0        0     4963 2023-09-08 20:18:54.974769 spyrmsd-0.6.0/tests/data/molecules/1cbr_ligand.mol2
--rw-r--r--   0        0        0     4713 2023-09-08 20:18:54.974978 spyrmsd-0.6.0/tests/data/molecules/2viz_1.sdf
--rw-r--r--   0        0        0     4713 2023-09-08 20:18:54.975172 spyrmsd-0.6.0/tests/data/molecules/2viz_2.sdf
--rw-r--r--   0        0        0     4713 2023-09-08 20:18:54.975373 spyrmsd-0.6.0/tests/data/molecules/2viz_3.sdf
--rw-r--r--   0        0        0     1296 2023-06-28 16:31:38.595758 spyrmsd-0.6.0/tests/data/molecules/benzene.mol2
--rw-r--r--   0        0        0      310 2023-06-28 16:31:38.595825 spyrmsd-0.6.0/tests/data/molecules/benzene.mol2.gz
--rw-r--r--   0        0        0     1188 2023-06-28 16:31:38.595896 spyrmsd-0.6.0/tests/data/molecules/benzene.sdf
--rw-r--r--   0        0        0      230 2023-06-28 16:31:38.595960 spyrmsd-0.6.0/tests/data/molecules/benzene.sdf.gz
--rw-r--r--   0        0        0      599 2023-09-08 20:18:54.975563 spyrmsd-0.6.0/tests/data/molecules/benzene.xyz
--rw-r--r--   0        0        0     3601 2023-06-28 16:31:38.596107 spyrmsd-0.6.0/tests/data/molecules/dialanine.sdf
--rw-r--r--   0        0        0      894 2023-06-28 16:31:38.596181 spyrmsd-0.6.0/tests/data/molecules/ethanol.sdf
--rw-r--r--   0        0        0      444 2023-09-08 20:18:54.975759 spyrmsd-0.6.0/tests/data/molecules/ethanol.xyz
--rw-r--r--   0        0        0     1096 2023-06-28 16:31:38.596327 spyrmsd-0.6.0/tests/data/molecules/pyridine.sdf
--rw-r--r--   0        0        0      550 2023-06-28 16:31:38.596397 spyrmsd-0.6.0/tests/data/molecules/pyridine.xyz
--rw-r--r--   0        0        0    22113 2023-06-28 16:31:38.596595 spyrmsd-0.6.0/tests/data/molecules/trp0.pdb
--rw-r--r--   0        0        0    22113 2023-06-28 16:31:38.596739 spyrmsd-0.6.0/tests/data/molecules/trp1.pdb
--rw-r--r--   0        0        0    22113 2023-06-28 16:31:38.596871 spyrmsd-0.6.0/tests/data/molecules/trp2.pdb
--rw-r--r--   0        0        0    22113 2023-06-28 16:31:38.597002 spyrmsd-0.6.0/tests/data/molecules/trp3.pdb
--rw-r--r--   0        0        0    22113 2023-06-28 16:31:38.597126 spyrmsd-0.6.0/tests/data/molecules/trp4.pdb
--rw-r--r--   0        0        0    22113 2023-06-28 16:31:38.597199 spyrmsd-0.6.0/tests/data/molecules/trp5.pdb
--rw-r--r--   0        0        0     1893 2023-06-28 16:31:38.597284 spyrmsd-0.6.0/tests/molecules.py
--rw-r--r--   0        0        0     1449 2023-09-08 20:18:54.975914 spyrmsd-0.6.0/tests/test_benchmarks.py
--rw-r--r--   0        0        0     4663 2023-09-08 20:18:54.976068 spyrmsd-0.6.0/tests/test_graph.py
--rw-r--r--   0        0        0     1314 2023-09-08 20:18:54.976197 spyrmsd-0.6.0/tests/test_hungarian.py
--rw-r--r--   0        0        0      596 2023-06-28 16:31:38.597583 spyrmsd-0.6.0/tests/test_import.py
--rw-r--r--   0        0        0     4112 2023-09-08 20:18:54.976343 spyrmsd-0.6.0/tests/test_io.py
--rw-r--r--   0        0        0     3508 2023-06-28 16:31:38.597741 spyrmsd-0.6.0/tests/test_large.py
--rw-r--r--   0        0        0     6419 2023-09-08 20:18:54.976494 spyrmsd-0.6.0/tests/test_molecule.py
--rw-r--r--   0        0        0     2403 2023-09-08 20:18:54.976630 spyrmsd-0.6.0/tests/test_qcp.py
--rw-r--r--   0        0        0    26471 2023-09-08 20:18:54.976862 spyrmsd-0.6.0/tests/test_rmsd.py
--rw-r--r--   0        0        0     1423 2023-09-08 20:18:54.977002 spyrmsd-0.6.0/tests/test_utils.py
--rw-r--r--   0        0        0    83780 2023-09-08 20:18:54.977505 spyrmsd-0.6.0/versioneer.py
--rw-r--r--   0        0        0     7571 1970-01-01 00:00:00.000000 spyrmsd-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      258 2024-04-05 21:55:07.867047 spyrmsd-0.7.0/.codecov.yml
+-rw-r--r--   0        0        0      315 2024-04-05 21:55:07.867047 spyrmsd-0.7.0/.coveragerc
+-rw-r--r--   0        0        0     2245 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      604 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      547 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0       81 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/ISSUE_TEMPLATE/empty-issue.md
+-rw-r--r--   0        0        0      142 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      787 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/workflows/flake8.yml
+-rw-r--r--   0        0        0      826 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0      464 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      636 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0     2095 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      948 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.gitignore
+-rw-r--r--   0        0        0      792 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      359 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/.readthedocs.yml
+-rw-r--r--   0        0        0     4115 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0      820 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/CITATION.cff
+-rw-r--r--   0        0        0     3562 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1073 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/LICENSE
+-rw-r--r--   0        0        0       93 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/MANIFEST.in
+-rw-r--r--   0        0        0     7346 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/README.md
+-rw-r--r--   0        0        0      126 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/credits.sh
+-rw-r--r--   0        0        0      843 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/README.md
+-rw-r--r--   0        0        0      518 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-all.yaml
+-rw-r--r--   0        0        0      243 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-docs.yaml
+-rw-r--r--   0        0        0      275 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-test-obabel-gt.yaml
+-rw-r--r--   0        0        0      276 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-test-obabel-nx.yaml
+-rw-r--r--   0        0        0      274 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-test-obabel-rx.yaml
+-rw-r--r--   0        0        0      311 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-test-rdkit-all.yaml
+-rw-r--r--   0        0        0      281 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-test-rdkit-gt.yaml
+-rw-r--r--   0        0        0      282 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-test-rdkit-nx.yaml
+-rw-r--r--   0        0        0      280 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd-test-rdkit-rx.yaml
+-rw-r--r--   0        0        0      133 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/devtools/conda-envs/spyrmsd.yaml
+-rw-r--r--   0        0        0      636 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/Makefile
+-rw-r--r--   0        0        0      997 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/README.md
+-rw-r--r--   0        0        0      799 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/make.bat
+-rw-r--r--   0        0        0       77 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api.rst
+-rw-r--r--   0        0        0      139 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.constants.rst
+-rw-r--r--   0        0        0      121 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.due.rst
+-rw-r--r--   0        0        0      142 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.exceptions.rst
+-rw-r--r--   0        0        0      127 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.graph.rst
+-rw-r--r--   0        0        0      139 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.graphs.gt.rst
+-rw-r--r--   0        0        0      139 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.graphs.nx.rst
+-rw-r--r--   0        0        0      228 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.graphs.rst
+-rw-r--r--   0        0        0      139 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.hungarian.rst
+-rw-r--r--   0        0        0      118 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.io.rst
+-rw-r--r--   0        0        0      136 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.molecule.rst
+-rw-r--r--   0        0        0      157 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.optional.obabel.rst
+-rw-r--r--   0        0        0      154 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.optional.rdkit.rst
+-rw-r--r--   0        0        0      245 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.optional.rst
+-rw-r--r--   0        0        0      121 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.qcp.rst
+-rw-r--r--   0        0        0      124 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.rmsd.rst
+-rw-r--r--   0        0        0      437 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.rst
+-rw-r--r--   0        0        0      127 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/api/spyrmsd.utils.rst
+-rw-r--r--   0        0        0     5319 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/conf.py
+-rw-r--r--   0        0        0      307 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/index.rst
+-rw-r--r--   0        0        0     1502 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/installation.rst
+-rw-r--r--   0        0        0    31852 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/tutorials/molecules/1a4k_dock.sdf
+-rw-r--r--   0        0        0     4286 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/tutorials/molecules/1a4k_ligand.sdf
+-rw-r--r--   0        0        0     9093 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/tutorials/tutorial.ipynb
+-rw-r--r--   0        0        0     4568 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/docs/source/tutorials/tutorial.rst
+-rw-r--r--   0        0        0      458 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      521 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/setup.cfg
+-rw-r--r--   0        0        0     1002 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/setup.py
+-rw-r--r--   0        0        0      631 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/__init__.py
+-rw-r--r--   0        0        0     2474 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/__main__.py
+-rw-r--r--   0        0        0     4173 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/constants.py
+-rw-r--r--   0        0        0     2019 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/due.py
+-rw-r--r--   0        0        0      107 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/exceptions.py
+-rw-r--r--   0        0        0     6984 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/graph.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/graphs/__init__.py
+-rw-r--r--   0        0        0      324 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/graphs/_common.py
+-rw-r--r--   0        0        0     4802 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/graphs/gt.py
+-rw-r--r--   0        0        0     3699 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/graphs/nx.py
+-rw-r--r--   0        0        0     3588 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/graphs/rx.py
+-rw-r--r--   0        0        0     2878 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/hungarian.py
+-rw-r--r--   0        0        0     1649 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/io.py
+-rw-r--r--   0        0        0     7074 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/molecule.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/optional/__init__.py
+-rw-r--r--   0        0        0     3160 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/optional/obabel.py
+-rw-r--r--   0        0        0     4852 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/optional/rdkit.py
+-rw-r--r--   0        0        0     7125 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/qcp.py
+-rw-r--r--   0        0        0    10000 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/rmsd.py
+-rw-r--r--   0        0        0     3418 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/spyrmsd/utils.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     2030 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0      510 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/tests/data/README.md
+-rw-r--r--   0        0        0     6610 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/tests/data/docking/1a28/1a28_dock.sdf
+-rw-r--r--   0        0        0     3431 2024-04-05 21:55:07.871047 spyrmsd-0.7.0/tests/data/docking/1a28/1a28_ligand.sdf
+-rw-r--r--   0        0        0       29 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a28/obrms-min.dat
+-rw-r--r--   0        0        0       25 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a28/obrms.dat
+-rw-r--r--   0        0        0    31852 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4k/1a4k_dock.sdf
+-rw-r--r--   0        0        0     4286 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4k/1a4k_ligand.sdf
+-rw-r--r--   0        0        0       83 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4k/obrms-min.dat
+-rw-r--r--   0        0        0       76 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4k/obrms.dat
+-rw-r--r--   0        0        0    34320 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4r/1a4r_dock.sdf
+-rw-r--r--   0        0        0     4025 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4r/1a4r_ligand.sdf
+-rw-r--r--   0        0        0       81 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4r/obrms-min.dat
+-rw-r--r--   0        0        0       81 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a4r/obrms.dat
+-rw-r--r--   0        0        0    22750 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a69/1a69_dock.sdf
+-rw-r--r--   0        0        0     2973 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a69/1a69_ligand.sdf
+-rw-r--r--   0        0        0       86 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a69/obrms-min.dat
+-rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a69/obrms.dat
+-rw-r--r--   0        0        0    67930 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a94/1a94_dock.sdf
+-rw-r--r--   0        0        0     7748 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a94/1a94_ligand.sdf
+-rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a94/obrms-min.dat
+-rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a94/obrms.dat
+-rw-r--r--   0        0        0     7776 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a99/1a99_dock.sdf
+-rw-r--r--   0        0        0     1347 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a99/1a99_ligand.sdf
+-rw-r--r--   0        0        0       69 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a99/obrms-min.dat
+-rw-r--r--   0        0        0       64 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a99/obrms.dat
+-rw-r--r--   0        0        0    49070 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9m/1a9m_dock.sdf
+-rw-r--r--   0        0        0     5591 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9m/1a9m_ligand.sdf
+-rw-r--r--   0        0        0       78 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9m/obrms-min.dat
+-rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9m/obrms.dat
+-rw-r--r--   0        0        0    11880 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9q/1a9q_dock.sdf
+-rw-r--r--   0        0        0     1833 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9q/1a9q_ligand.sdf
+-rw-r--r--   0        0        0      120 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9q/obrms-min.dat
+-rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1a9q/obrms.dat
+-rw-r--r--   0        0        0    43730 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1aaq/1aaq_dock.sdf
+-rw-r--r--   0        0        0     5521 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1aaq/1aaq_ligand.sdf
+-rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1aaq/obrms-min.dat
+-rw-r--r--   0        0        0       77 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1aaq/obrms.dat
+-rw-r--r--   0        0        0    11375 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1add/1add_dock.sdf
+-rw-r--r--   0        0        0     2955 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1add/1add_ligand.sdf
+-rw-r--r--   0        0        0       42 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1add/obrms-min.dat
+-rw-r--r--   0        0        0       41 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1add/obrms.dat
+-rw-r--r--   0        0        0    21290 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1adl/1adl_dock.sdf
+-rw-r--r--   0        0        0     3162 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1adl/1adl_ligand.sdf
+-rw-r--r--   0        0        0       78 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1adl/obrms-min.dat
+-rw-r--r--   0        0        0       78 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1adl/obrms.dat
+-rw-r--r--   0        0        0    12400 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ado/1ado_dock.sdf
+-rw-r--r--   0        0        0     1829 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ado/1ado_ligand.sdf
+-rw-r--r--   0        0        0       85 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ado/obrms-min.dat
+-rw-r--r--   0        0        0       78 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ado/obrms.dat
+-rw-r--r--   0        0        0    36100 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afk/1afk_dock.sdf
+-rw-r--r--   0        0        0     4340 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afk/1afk_ligand.sdf
+-rw-r--r--   0        0        0       81 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afk/obrms-min.dat
+-rw-r--r--   0        0        0       79 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afk/obrms.dat
+-rw-r--r--   0        0        0    36100 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afl/1afl_dock.sdf
+-rw-r--r--   0        0        0     4346 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afl/1afl_ligand.sdf
+-rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afl/obrms-min.dat
+-rw-r--r--   0        0        0       80 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1afl/obrms.dat
+-rw-r--r--   0        0        0    14360 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ai4/1ai4_dock.sdf
+-rw-r--r--   0        0        0     2053 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ai4/1ai4_ligand.sdf
+-rw-r--r--   0        0        0       89 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ai4/obrms-min.dat
+-rw-r--r--   0        0        0       79 2024-04-05 21:55:07.875047 spyrmsd-0.7.0/tests/data/docking/1ai4/obrms.dat
+-rw-r--r--   0        0        0    13810 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai5/1ai5_dock.sdf
+-rw-r--r--   0        0        0     2191 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai5/1ai5_ligand.sdf
+-rw-r--r--   0        0        0       86 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai5/obrms-min.dat
+-rw-r--r--   0        0        0       79 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai5/obrms.dat
+-rw-r--r--   0        0        0     8130 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai7/1ai7_dock.sdf
+-rw-r--r--   0        0        0     1441 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai7/1ai7_ligand.sdf
+-rw-r--r--   0        0        0      120 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai7/obrms-min.dat
+-rw-r--r--   0        0        0       81 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ai7/obrms.dat
+-rw-r--r--   0        0        0    28280 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aid/1aid_dock.sdf
+-rw-r--r--   0        0        0     4086 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aid/1aid_ligand.sdf
+-rw-r--r--   0        0        0       78 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aid/obrms-min.dat
+-rw-r--r--   0        0        0       79 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aid/obrms.dat
+-rw-r--r--   0        0        0    20210 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aj7/1aj7_dock.sdf
+-rw-r--r--   0        0        0     3017 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aj7/1aj7_ligand.sdf
+-rw-r--r--   0        0        0       80 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aj7/obrms-min.dat
+-rw-r--r--   0        0        0       81 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1aj7/obrms.dat
+-rw-r--r--   0        0        0    13810 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajn/1ajn_dock.sdf
+-rw-r--r--   0        0        0     2189 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajn/1ajn_ligand.sdf
+-rw-r--r--   0        0        0       89 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajn/obrms-min.dat
+-rw-r--r--   0        0        0       79 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajn/obrms.dat
+-rw-r--r--   0        0        0    14360 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajp/1ajp_dock.sdf
+-rw-r--r--   0        0        0     2078 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajp/1ajp_ligand.sdf
+-rw-r--r--   0        0        0       90 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajp/obrms-min.dat
+-rw-r--r--   0        0        0       80 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajp/obrms.dat
+-rw-r--r--   0        0        0     9910 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajq/1ajq_dock.sdf
+-rw-r--r--   0        0        0     1709 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajq/1ajq_ligand.sdf
+-rw-r--r--   0        0        0       85 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajq/obrms-min.dat
+-rw-r--r--   0        0        0       81 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajq/obrms.dat
+-rw-r--r--   0        0        0    12015 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajv/1ajv_dock.sdf
+-rw-r--r--   0        0        0     5461 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajv/1ajv_ligand.sdf
+-rw-r--r--   0        0        0       25 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajv/obrms-min.dat
+-rw-r--r--   0        0        0       25 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajv/obrms.dat
+-rw-r--r--   0        0        0    39156 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajx/1ajx_dock.sdf
+-rw-r--r--   0        0        0     5343 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajx/1ajx_ligand.sdf
+-rw-r--r--   0        0        0       82 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajx/obrms-min.dat
+-rw-r--r--   0        0        0       78 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/docking/1ajx/obrms.dat
+-rw-r--r--   0        0        0     2112 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/1a99_ligand.pdb
+-rw-r--r--   0        0        0      568 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/1a99_ligand.pdb.gz
+-rw-r--r--   0        0        0    23500 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.mol2
+-rw-r--r--   0        0        0    24394 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.pdb
+-rw-r--r--   0        0        0    20730 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.sdf
+-rw-r--r--   0        0        0     3283 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.sdf.gz
+-rwxr-xr-x   0        0        0     4963 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/1cbr_ligand.mol2
+-rw-r--r--   0        0        0     4713 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/2viz_1.sdf
+-rw-r--r--   0        0        0     4713 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/2viz_2.sdf
+-rw-r--r--   0        0        0     4713 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/2viz_3.sdf
+-rw-r--r--   0        0        0     1296 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/benzene.mol2
+-rw-r--r--   0        0        0      310 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/benzene.mol2.gz
+-rw-r--r--   0        0        0     1188 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/benzene.sdf
+-rw-r--r--   0        0        0      230 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/benzene.sdf.gz
+-rw-r--r--   0        0        0      599 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/benzene.xyz
+-rw-r--r--   0        0        0     3601 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/dialanine.sdf
+-rw-r--r--   0        0        0      894 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/ethanol.sdf
+-rw-r--r--   0        0        0      444 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/ethanol.xyz
+-rw-r--r--   0        0        0     1096 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/pyridine.sdf
+-rw-r--r--   0        0        0      550 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/pyridine.xyz
+-rw-r--r--   0        0        0    22113 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/trp0.pdb
+-rw-r--r--   0        0        0    22113 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/trp1.pdb
+-rw-r--r--   0        0        0    22113 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/trp2.pdb
+-rw-r--r--   0        0        0    22113 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/trp3.pdb
+-rw-r--r--   0        0        0    22113 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/trp4.pdb
+-rw-r--r--   0        0        0    22113 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/data/molecules/trp5.pdb
+-rw-r--r--   0        0        0     1893 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/molecules.py
+-rw-r--r--   0        0        0     1426 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_benchmarks.py
+-rw-r--r--   0        0        0     5713 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_graph.py
+-rw-r--r--   0        0        0     1314 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_hungarian.py
+-rw-r--r--   0        0        0      596 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_import.py
+-rw-r--r--   0        0        0     4112 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_io.py
+-rw-r--r--   0        0        0     3508 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_large.py
+-rw-r--r--   0        0        0     7555 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_molecule.py
+-rw-r--r--   0        0        0     2403 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_qcp.py
+-rw-r--r--   0        0        0    26471 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_rmsd.py
+-rw-r--r--   0        0        0     1423 2024-04-05 21:55:07.879047 spyrmsd-0.7.0/tests/test_utils.py
+-rw-r--r--   0        0        0     7776 1970-01-01 00:00:00.000000 spyrmsd-0.7.0/PKG-INFO
```

### Comparing `spyrmsd-0.6.0/.github/CONTRIBUTING.md` & `spyrmsd-0.7.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/.github/FUNDING.yml` & `spyrmsd-0.7.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/.github/ISSUE_TEMPLATE/bug-report.md` & `spyrmsd-0.7.0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/.github/workflows/flake8.yml` & `spyrmsd-0.7.0/.github/workflows/flake8.yml`

 * *Files 10% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
       with:
           python-version: ${{ matrix.python-version }}
     - name: Install Dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install flake8
+        python -m pip install setuptools
+        python -m pip install flake8
     - name: Install  package
       run: |
         python setup.py develop --no-deps
     - name: Lint with flake8
       run: |
         flake8 . --count --show-source --statistics
```

### Comparing `spyrmsd-0.6.0/.github/workflows/pypi.yml` & `spyrmsd-0.7.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/.github/workflows/pytest.yml` & `spyrmsd-0.7.0/.github/workflows/pytest.yml`

 * *Files 17% similar despite different names*

```diff
@@ -20,47 +20,53 @@
 jobs:
   test:
     name: Test ${{ matrix.os }}-${{ matrix.python-version }}-${{ matrix.chemlib }}-${{ matrix.graphlib }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [macOS-latest, ubuntu-latest, windows-latest]
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
         chemlib: [obabel, rdkit]
-        graphlib: [nx, gt]
+        graphlib: [nx, gt, rx, all]
         exclude:
         # graph-tools does not work on Windows
         - {os: "windows-latest", graphlib: "gt"}
-        # FIXME: Keeps failing in CI for unknown reasons during miniconda setup
-        - {os: "ubuntu-latest", graphlib: "gt", chemlib: "rdkit", python-version: "3.7"}
+        - {os: "windows-latest", graphlib: "all"}
+        - {graphlib: "all", chemlib: "obabel"}
+        include:
+        - {os: "macOS-14", graphlib: "gt", chemlib: "obabel", python-version: "3.12"}
+        - {os: "macOS-14", graphlib: "nx", chemlib: "rdkit", python-version: "3.12"}
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Info
       shell: bash
       run: |
         uname -a
         df -h
         ulimit -a
 
-    - uses: conda-incubator/setup-miniconda@v2
+    - uses: conda-incubator/setup-miniconda@v3
       with:
         python-version: ${{ matrix.python-version }}
         environment-file: devtools/conda-envs/spyrmsd-test-${{ matrix.chemlib }}-${{ matrix.graphlib }}.yaml
-        channels: conda-forge,defaults
+        miniforge-version: "latest"
         activate-environment: spyrmsd
+        miniforge-variant: Mambaforge
+        use-mamba: true
         auto-update-conda: true
         auto-activate-base: false
         show-channel-urls: true
 
     - name: Install
       run: |
         python -m pip install . --no-deps
-        conda list
+        mamba info
+        mamba list
 
     - name: Test
       run: |
         pytest -v --benchmark --cov=spyrmsd --cov-report=xml --color=yes tests/
 
     - name: CodeCov
       uses: codecov/codecov-action@v3
```

### Comparing `spyrmsd-0.6.0/.gitignore` & `spyrmsd-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/.pre-commit-config.yaml` & `spyrmsd-0.7.0/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -21,12 +21,13 @@
     rev: 6.1.0
     hooks:
     -   id: flake8
 -   repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
     -   id: isort
+        args: ["--profile", "black"]
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.5.1
     hooks:
     -   id: mypy
         additional_dependencies: [types-requests]
```

### Comparing `spyrmsd-0.6.0/CHANGELOG.md` & `spyrmsd-0.7.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,44 @@
 
 # `spyrmsd` CHANGELOG
 
 ------------------------------------------------------------------------------
 
+## Version 0.7.0
+
+Date:            05/04/2024
+Contributors:    @RMeli, @takluyver, @Jnelen
+
+### Added
+
+* Support for `rustworkx` graph library [PR 111 | @RMeli]
+* Functionality to manually select the backend from CLI [PR #108 | @RMeli]
+* Functionality to manually select the backend [PR  #107 | @Jnelen]
+* Python `3.12` to CI [PR  #102 | @RMeli]
+* macOS M1 (`macoOS-14`) to CI [PR  #102 | @RMeli]
+
+### Changed
+
+* Molecular graphs cache to cache by backend [PR  #107 | @Jnelen]
+* Python build system to use flit_core directly [PR #103 | @takluyver]
+* Minimum version of Python to `3.9` (to reduce CI matrix) [PR  #102 | @RMeli]
+
+### Fixed
+
+* Failing tests with `pytest=8.0.0` [PR #101 | @RMeli]
+
+### Improved
+
+* Messages for `NotImplementedError` exceptions [PR #90 | @RMeli]
+
+### Removed
+
+* `.gitattributes` and `.lgtm.yaml` stale files
+* `versioneer` [PR #91 | @RMeli]
+
 ## Version 0.6.0
 
 Date:            08/09/2023
 Contributors:    @RMeli
 
 ### Improved
```

### Comparing `spyrmsd-0.6.0/CITATION.cff` & `spyrmsd-0.7.0/CITATION.cff`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 cff-version: 1.2.0
 message: "If you use this software, please cite it as below."
 authors:
 - family-names: "Meli"
   given-names: "Rocco"
   orcid: "https://orcid.org/0000-0002-2845-3410"
+- family-names: "Nelen"
+  given-names: "Jochem"
+  orcid: "https://orcid.org/0000-0002-9970-4950"
 title: "spyrmsd"
-version: 0.6.0
+version: 0.7.0
 doi: 10.5281/zenodo.3631876
 date-released: 2021-06-21
 url: "https://github.com/RMeli/spyrmsd"
 preferred-citation:
   type: article
   authors:
   - family-names: "Meli"
```

### Comparing `spyrmsd-0.6.0/CODE_OF_CONDUCT.md` & `spyrmsd-0.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/LICENSE` & `spyrmsd-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/README.md` & `spyrmsd-0.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ![mypy](https://github.com/RMeli/spyrmsd/workflows/mypy/badge.svg)
 [![codecov](https://codecov.io/gh/RMeli/spyrmsd/branch/develop/graph/badge.svg)](https://codecov.io/gh/RMeli/spyrmsd/branch/master)
 
 [![Docs](https://img.shields.io/badge/docs-spyrmsd.readthedocs.io-blueviolet)](https://spyrmsd.readthedocs.io)
 [![Documentation Status](https://readthedocs.org/projects/spyrmsd/badge/?version=develop)](https://spyrmsd.readthedocs.io/en/develop/?badge=develop)
 
 [![License](https://img.shields.io/github/license/RMeli/pyrmsd?color=%2333BBFF)](https://opensource.org/licenses/MIT)
-[![PyPI](https://img.shields.io/badge/PyPI-v0.6.0%20-ff69b4)](https://pypi.org/project/spyrmsd/)
+[![PyPI](https://img.shields.io/badge/PyPI-v0.7.0%20-ff69b4)](https://pypi.org/project/spyrmsd/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/spyrmsd.svg)](https://anaconda.org/conda-forge/spyrmsd)
 
 [![J. Cheminform.](https://img.shields.io/badge/J.%20Cheminform.-10.1186%2Fs13321--020--00455--2-blue)](https://doi.org/10.1186/s13321-020-00455-2)
 [![Zenodo](https://zenodo.org/badge/214157073.svg)](https://zenodo.org/badge/latestdoi/214157073)
 
 Python tool for symmetry-corrected RMSD calculations.
 
@@ -34,15 +34,15 @@
 ```
 
 ## Installation
 
 `spyrmsd` is available on [PyPI](https://pypi.org/project/spyrmsd/) and [conda-forge](https://github.com/conda-forge/spyrmsd-feedstock) and can be easily installed from source. See [Dependencies](###Dependencies) for a description of all the dependencies.
 
 > [!NOTE]
-> `spyrmsd` will install [NetworkX](https://networkx.github.io/) (multi-platform). You can install [graph-tool](https://graph-tool.skewed.de/) on macOS and Linux for higher performance.
+> `spyrmsd` will install [NetworkX](https://networkx.github.io/) (multi-platform). You can install the other backends for higher performance.
 
 > [!WARNING]
 > If `spyrmsd` is used as a standalone tool, it is required to install either [RDKit](https://rdkit.org/) or [Open Babel](http://openbabel.org/). Neither is automatically installed with `pip` nor `conda`.
 
 ### PyPI
 
 ```bash
@@ -67,53 +67,42 @@
 
 `spyrmsd` can be used both as a module or as a standalone tool.
 
 #### Module
 
 The following packages are required to use `spyrmsd` as a module:
 
-* [graph-tool](https://graph-tool.skewed.de/) or [NetworkX](https://networkx.github.io/)
 * [numpy](https://numpy.org/)
 * [scipy](https://www.scipy.org/)
 
+One of the following graph libraries is required:
+* [graph-tool]
+* [NetworkX]
+* [rustworkx]
+
 > [!NOTE]
-> `spyrmsd` uses [graph-tool](https://graph-tool.skewed.de/) by default but will fall back to [NetworkX](https://networkx.github.io/) if the former is not installed (e.g. on Windows). However, in order to support cross-platform installation [NetworkX](https://networkx.github.io/) is installed by default, and [graph-tool](https://graph-tool.skewed.de/) needs to be installed manually.
+> `spyrmsd` uses the following priority when multiple graph libraries are present: [graph-tool], [NetworkX], [rustworkx]. *This order might change. Use `set_backend` to ensure you are always using the same backend, if needed.* However, in order to support cross-platform installation [NetworkX](https://networkx.github.io/) is installed by default, and the other graph library need to be installed manually.
 
 #### Standalone Tool
 
 Additionally, one of the following packages is required to use `spyrmsd` as a standalone tool:
 
 * [Open Babel](http://openbabel.org/)
 * [RDKit](https://rdkit.org/)
 
 ## Usage
 
 ### Standalone Tool
 
+`spyrmsd` provides a convenient CLI tool. See `spyrmsd`'s `--help` for the usage:
+
 ```bash
 python -m spyrmsd -h
 ```
 
-```text
-usage: python -m spyrmsd [-h] [-m] [-c] [--hydrogens] [-n] reference molecules [molecules ...]
-
-Symmetry-corrected RMSD calculations in Python.
-
-positional arguments:
-  reference       Reference file
-  molecules       Input file(s)
-
-optional arguments:
-  -h, --help      show this help message and exit
-  -m, --minimize  Minimize (fit)
-  -c, --center    Center molecules at origin
-  --hydrogens     Keep hydrogen atoms
-  -n, --nosymm    No graph isomorphism
-```
-
 ### Module
 
 ```python
 from spyrmsd import rmsd
 ```
 
 #### RMSD
@@ -129,15 +118,15 @@
     center: bool = False,   # Flag to center molecules at origin
     minimize: bool = False, # Flag to compute minimum RMSD
     atol: float = 1e-9,     # Numerical tolerance for QCP method
 )
 ```
 
 > [!NOTE]
-> Atomic properties (`aprops`) can be any Python object when using [NetworkX](https://networkx.github.io/), or integers, floats, or strings when using [graph-tool](https://graph-tool.skewed.de/).
+> Atomic properties (`aprops`) can be any Python object when using [NetworkX] and [rustworkx], or integers, floats, or strings when using [graph-tool].
 
 #### Symmetry-Corrected RMSD
 
 The function `rmsd.symmrmsd` computes symmetry-corrected RMSD using molecular graph isomorphisms. Symmetry correction requires molecular adjacency matrices describing the connectivity but needs not the atoms to be in the same order.
 
 Atom matching is performed according to the molecular graph. This function should also be used when atoms in the molecules being compared are not in the same order (even if there is not symmetry to be accounted for).
 
@@ -153,31 +142,59 @@
     minimize: bool = False,                      # Flag to compute minimum RMSD
     cache: bool = True,                          # Cache graph isomorphisms
     atol: float = 1e-9,                          # Numerical tolerance for QCP method
 )
 ```
 
 > [!NOTE]
-> Atomic properties (`aprops`) can be any Python object when using [NetworkX](https://networkx.github.io/), or integers, floats, or strings when using [graph-tool](https://graph-tool.skewed.de/).
+> Atomic properties (`aprops`) can be any Python object when using [NetworkX] and [rustworkx], or integers, floats, or strings when using [graph-tool](https://graph-tool.skewed.de/).
+
+#### Select Backend
+
+`spyrmsd` supports the following graph libraries for the calculation of graph isomorphisms:
+* [graph-tool]
+* [NetworkX]
+* [rustworkx]
+
+ You can check which backend is being used with
+
+```python
+spyrmsd.get_backend()
+```
+
+You can also manually select your preferred backend with
+
+```python
+spyrmsd.set_backend("networkx")
+# spyrmsd uses NetworkX
+spyrmsd.set_backend("graph_tool")
+# spyrmsd uses graph_tool
+```
+
+The available backends (which depend on the installed dependencies) are stored in `spyrmsd.available_backends`.
 
 ## Development
 
 To ensure code quality and consistency the following tools are used during development:
 
 * [black](https://black.readthedocs.io/en/stable/)
 * [Flake 8](http://flake8.pycqa.org/en/latest/) (CI)
 * [isort]()
 * [mypy](http://mypy-lang.org/) (CI)
 
 Pre-commit `git` hooks can be installed with [pre-commit](https://pre-commit.com/).
 
 ## Copyright
 
-Copyright (c) 2019-2021, Rocco Meli.
+Copyright (c) 2019-2024, Rocco Meli.
 
 ## References
 
 References are tracked with [duecredit](https://github.com/duecredit/duecredit/). Run the `credits.sh` script in order to print up-to-date references.
 
 ### Acknowledgements
 
 Project based on the [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version `1.1`.
+
+[rustworkx]: https://www.rustworkx.org
+[NetworkX]: https://networkx.github.io/
+[graph-tool]: https://graph-tool.skewed.de/
```

### Comparing `spyrmsd-0.6.0/devtools/README.md` & `spyrmsd-0.7.0/devtools/README.md`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/docs/Makefile` & `spyrmsd-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/docs/README.md` & `spyrmsd-0.7.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/docs/make.bat` & `spyrmsd-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/docs/source/conf.py` & `spyrmsd-0.7.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 sys.path.insert(0, os.path.abspath("../.."))
 
 
 # -- Project information -----------------------------------------------------
 
 project = "spyrmsd"
 copyright = (
-    "2019-2021, Rocco Meli. Project structure based on the "
+    "2019-2024, Rocco Meli. Project structure based on the "
     "Computational Molecular Science Python Cookiecutter version 1.1"
 )
 author = "Rocco Meli"
 
 # The short X.Y version
 # version = "0.0"
 # The full version, including alpha/beta/rc tags
```

### Comparing `spyrmsd-0.6.0/docs/source/installation.rst` & `spyrmsd-0.7.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/docs/source/tutorials/molecules/1a4k_dock.sdf` & `spyrmsd-0.7.0/docs/source/tutorials/molecules/1a4k_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/docs/source/tutorials/molecules/1a4k_ligand.sdf` & `spyrmsd-0.7.0/docs/source/tutorials/molecules/1a4k_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/docs/source/tutorials/tutorial.ipynb` & `spyrmsd-0.7.0/docs/source/tutorials/tutorial.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9672501803751804%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'import spyrmsd\\n')]}}, 11: {'outputs': {0: {'text': "*

 * *            "{insert: [(1, '[21:58:01] Molecule does not have explicit Hs. Consider calling "*

 * *            "AddHs()\\n'), (2, '[21:58:01] Molecule does not have explicit Hs. Consider calling "*

 * *            "AddHs()\\n')], delete: [2, 1]}}}}, insert: [(25, OrderedDict([('cell_type', "*

 * *            "'markdown'), ('metadata', OrderedDict()), ('source', ['# Change Backend'])])), (26, "*

 * *            "OrderedDict([('cell […]*

```diff
@@ -10,14 +10,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
+                "import spyrmsd\n",
                 "from spyrmsd import io, rmsd"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -103,16 +104,16 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "<frozen importlib._bootstrap>:241: RuntimeWarning: to-Python converter for std::__1::pair<double, double> already registered; second conversion method ignored.\n",
-                        "[18:44:03] Molecule does not have explicit Hs. Consider calling AddHs()\n",
-                        "[18:44:03] Molecule does not have explicit Hs. Consider calling AddHs()\n"
+                        "[21:58:01] Molecule does not have explicit Hs. Consider calling AddHs()\n",
+                        "[21:58:01] Molecule does not have explicit Hs. Consider calling AddHs()\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
                             "[0.019162902039384797]"
                         ]
@@ -285,14 +286,110 @@
                 "    adj_ref,\n",
                 "    adj,\n",
                 "    minimize=True,\n",
                 ")\n",
                 "\n",
                 "print(RMSD)"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Change Backend"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "`spyrmsd` supports multiple backends. You see which backends are available by looking at the `available_backends` attribute:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "['graph_tool', 'networkx']"
+                        ]
+                    },
+                    "execution_count": 11,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "spyrmsd.available_backends"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The available backends are a subset of the supported backends. Only the backends that are installed will be available."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "You can check the current backend with"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "'graph_tool'"
+                        ]
+                    },
+                    "execution_count": 12,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "spyrmsd.get_backend()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "You can switch the backend using"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 13,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "'networkx'"
+                        ]
+                    },
+                    "execution_count": 13,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "spyrmsd.set_backend(\"networkx\")\n",
+                "spyrmsd.get_backend()"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
@@ -303,13 +400,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.11.8"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `spyrmsd-0.6.0/docs/source/tutorials/tutorial.rst` & `spyrmsd-0.7.0/docs/source/tutorials/tutorial.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Tutorial
 ========
 
 .. code:: ipython3
 
+    import spyrmsd
     from spyrmsd import io, rmsd
 
 OpenBabel or RDKit
 ~~~~~~~~~~~~~~~~~~
 
 ``spyrmsd`` natively supports
 `OpenBabel <http://openbabel.org/wiki/Main_Page>`__ and
@@ -64,16 +65,16 @@
 
     rmsdwrapper(mol1, mol2)
 
 
 .. parsed-literal::
 
     <frozen importlib._bootstrap>:241: RuntimeWarning: to-Python converter for std::__1::pair<double, double> already registered; second conversion method ignored.
-    [18:44:03] Molecule does not have explicit Hs. Consider calling AddHs()
-    [18:44:03] Molecule does not have explicit Hs. Consider calling AddHs()
+    [21:58:01] Molecule does not have explicit Hs. Consider calling AddHs()
+    [21:58:01] Molecule does not have explicit Hs. Consider calling AddHs()
 
 
 
 
 .. parsed-literal::
 
     [0.019162902039384797]
@@ -91,15 +92,15 @@
 
 .. code:: ipython3
 
     for mol in mols:
         mol.strip()
 
 Symmetry-Corrected RMSD
------------------------
+~~~~~~~~~~~~~~~~~~~~~~~
 
 ``spyrmsd`` only needs atomic coordinates, atomic number and the
 molecular adjacency matrix to compute the standard RMSD with
 ``spyrmsd.rmsd.symmrmsd``. The ``spyrmsd.molecule.Molecule`` class
 provides easy access to such information:
 
 .. code:: ipython3
@@ -133,15 +134,15 @@
 
 .. parsed-literal::
 
     [2.0246085732404446, 1.4951562971486378, 10.028009301306854, 7.900570020309068, 7.578344354783399, 9.52999506817054, 4.952371789159667, 7.762808670066815, 9.996922964463582, 7.1732072690335755]
 
 
 Minimum RMSD
-~~~~~~~~~~~~
+------------
 
 We can also compute the minimum RMSD obtained by superimposing the
 molecular structures:
 
 .. code:: ipython3
 
     RMSD = rmsd.symmrmsd(
@@ -156,7 +157,60 @@
 
     print(RMSD)
 
 
 .. parsed-literal::
 
     [1.2012368667355435, 1.0533413220699535, 1.153253104575529, 1.036542688936588, 0.8407673221224187, 1.1758143217869736, 0.7817315189656655, 1.0933314311267845, 1.0260767175206462, 0.9586369647000478]
+
+
+
+Change Backend
+~~~~~~~~~~~~~~
+
+``spyrmsd`` supports multiple backends. You see which backends are
+available by looking at the ``available_backends`` attribute:
+
+.. code:: ipython3
+
+    spyrmsd.available_backends
+
+
+
+
+.. parsed-literal::
+
+    ['graph_tool', 'networkx']
+
+
+
+The available backends are a subset of the supported backends. Only the
+backends that are installed will be available.
+
+You can check the current backend with
+
+.. code:: ipython3
+
+    spyrmsd.get_backend()
+
+
+
+
+.. parsed-literal::
+
+    'graph_tool'
+
+
+
+You can switch the backend using
+
+.. code:: ipython3
+
+    spyrmsd.set_backend("networkx")
+    spyrmsd.get_backend()
+
+
+
+
+.. parsed-literal::
+
+    'networkx'
```

### Comparing `spyrmsd-0.6.0/spyrmsd/__main__.py` & `spyrmsd-0.7.0/spyrmsd/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 Symmetry-corrected RMSD calculations in Python
 """
 
 if __name__ == "__main__":
     import argparse as ap
     import importlib.util
     import sys
+    import warnings
 
+    import spyrmsd
     from spyrmsd import io
     from spyrmsd.rmsd import rmsdwrapper
 
     parser = ap.ArgumentParser(
         prog="python -m spyrmsd",
         description="Symmetry-corrected RMSD calculations in Python.",
     )
@@ -21,14 +23,24 @@
     parser.add_argument(
         "-c", "--center", action="store_true", help="Center molecules at origin"
     )
     parser.add_argument("--hydrogens", action="store_true", help="Keep hydrogen atoms")
     parser.add_argument(
         "-n", "--nosymm", action="store_false", help="No graph isomorphism"
     )
+    parser.add_argument(
+        "-g",
+        "--graph-backend",
+        type=str,
+        default=None,
+        help="Graph library (backend)",
+    )
+    parser.add_argument(
+        "-v", "--verbose", action="store_true", help="Enable verbose mode"
+    )
 
     args = parser.parse_args()
 
     if (
         importlib.util.find_spec("openbabel") is None
         and importlib.util.find_spec("rdkit") is None
     ):
@@ -45,14 +57,22 @@
     # Load all molecules
     try:
         mols = [mol for molfile in args.molecules for mol in io.loadallmols(molfile)]
     except OSError:
         print("ERROR: Molecule file(s) not found.", file=sys.stderr)
         exit(-1)
 
+    if args.graph_backend is not None:
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            spyrmsd.set_backend(args.graph_backend)
+
+            if args.verbose:
+                print(f"Graph library: {spyrmsd.get_backend()}")
+
     # Loop over molecules within fil
     RMSDlist = rmsdwrapper(
         ref,
         mols,
         symmetry=args.nosymm,  # args.nosymm store False
         center=args.center,
         minimize=args.minimize,
```

### Comparing `spyrmsd-0.6.0/spyrmsd/constants.py` & `spyrmsd-0.7.0/spyrmsd/constants.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/spyrmsd/due.py` & `spyrmsd-0.7.0/spyrmsd/due.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/spyrmsd/graphs/gt.py` & `spyrmsd-0.7.0/spyrmsd/graphs/gt.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/spyrmsd/graphs/nx.py` & `spyrmsd-0.7.0/spyrmsd/graphs/nx.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/spyrmsd/hungarian.py` & `spyrmsd-0.7.0/spyrmsd/hungarian.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/spyrmsd/io.py` & `spyrmsd-0.7.0/spyrmsd/io.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/spyrmsd/molecule.py` & `spyrmsd-0.7.0/spyrmsd/molecule.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 import numpy as np
 
 from spyrmsd import constants, graph, utils
 
 
 class Molecule:
@@ -46,15 +46,15 @@
 
         self.stripped: bool = bool(np.all(atomicnums != 1))
 
         if adjacency_matrix is not None:
             self.adjacency_matrix: np.ndarray = np.asarray(adjacency_matrix, dtype=int)
 
         # Molecular graph
-        self.G = None
+        self.G: Dict[str, object] = {}
 
         self.masses: Optional[List[float]] = None
 
     @classmethod
     def from_obabel(cls, obmol, adjacency: bool = True):
         """
         Constructor from OpenBabel molecule.
@@ -178,15 +178,15 @@
             self.natoms = len(self.atomicnums)
 
             # Update adjacency matrix
             if self.adjacency_matrix is not None:
                 self.adjacency_matrix = self.adjacency_matrix[np.ix_(idx, idx)]
 
             # Reset molecular graph when stripping
-            self.G = None
+            self.G = {}
 
             self.stripped = True
 
     def to_graph(self):
         """
         Convert molecule to graph.
 
@@ -196,37 +196,39 @@
             Molecular graph.
 
         Notes
         -----
         If the molecule does not have an associated adjacency matrix, a simple
         bond perception is used.
 
-        The molecular graph is cached.
+        The molecular graph is cached per backend.
         """
-        if self.G is None:
+        _current_backend = graph._current_backend
+
+        if _current_backend not in self.G.keys():
             try:
-                self.G = graph.graph_from_adjacency_matrix(
+                self.G[_current_backend] = graph.graph_from_adjacency_matrix(
                     self.adjacency_matrix, self.atomicnums
                 )
             except AttributeError:
                 warnings.warn(
                     "Molecule was not initialized with an adjacency matrix. "
                     + "Using bond perception..."
                 )
 
                 # Automatic bond perception (with very simple rule)
                 self.adjacency_matrix = graph.adjacency_matrix_from_atomic_coordinates(
                     self.atomicnums, self.coordinates
                 )
 
-                self.G = graph.graph_from_adjacency_matrix(
+                self.G[_current_backend] = graph.graph_from_adjacency_matrix(
                     self.adjacency_matrix, self.atomicnums
                 )
 
-        return self.G
+        return self.G[_current_backend]
 
     def __len__(self) -> int:
         """
         Molecule size.
 
         Returns
         -------
```

### Comparing `spyrmsd-0.6.0/spyrmsd/optional/obabel.py` & `spyrmsd-0.7.0/spyrmsd/optional/obabel.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/spyrmsd/optional/rdkit.py` & `spyrmsd-0.7.0/spyrmsd/optional/rdkit.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,15 +60,17 @@
                 rdmol = next(Chem.ForwardSDMolSupplier(fgz, removeHs=False))
     elif fmt == "pdb":
         if not gzipped:
             rdmol = Chem.MolFromPDBFile(fname, removeHs=False)
         else:
             rdmol = _load_block_gzipped(Chem.MolFromPDBBlock, fname)
     else:
-        raise NotImplementedError
+        raise NotImplementedError(
+            f"Format '{fmt}' is currently not supported with RDKit."
+        )
 
     return rdmol
 
 
 def loadall(fname: str):
     """
     Load molecules from file.
@@ -83,30 +85,36 @@
     List of molecules
     """
 
     gzipped = os.path.splitext(fname)[-1] == ".gz"
     fmt = utils.molformat(fname)
 
     if fmt == "mol2":
-        raise NotImplementedError  # See RDKit Issue #415
+        error = (
+            "Multiple molecules in MOL2 files are not supported. "
+            "See RDKit#415 (https://github.com/rdkit/rdkit/pull/415)."
+        )
+        raise NotImplementedError(error)  # See RDKit Issue #415
     elif fmt == "sdf":
         if not gzipped:
             rdmols = Chem.SDMolSupplier(fname, removeHs=False)
             mols = [rdmol for rdmol in rdmols]
         else:
             with gzip.open(fname, "r") as fgz:
                 rdmols = Chem.ForwardSDMolSupplier(fgz, removeHs=False)
 
                 # Load all molecules before closing file
                 mols = [rdmol for rdmol in rdmols]
     elif fmt == "pdb":
         # TODO: Implement
-        raise NotImplementedError
+        raise NotImplementedError("Multiple molecules in PDB files are not supported.")
     else:
-        raise NotImplementedError
+        raise NotImplementedError(
+            f"Format '{fmt}' is currently not supported with RDKit."
+        )
 
     return mols
 
 
 def adjacency_matrix(mol) -> np.ndarray:
     """
     Adjacency matrix from OpenBabel molecule.
```

### Comparing `spyrmsd-0.6.0/spyrmsd/qcp.py` & `spyrmsd-0.7.0/spyrmsd/qcp.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/spyrmsd/rmsd.py` & `spyrmsd-0.7.0/spyrmsd/rmsd.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/spyrmsd/utils.py` & `spyrmsd-0.7.0/spyrmsd/utils.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/conftest.py` & `spyrmsd-0.7.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Control skipping of tests according to command line option.
 
 Soource:
     https://docs.pytest.org/en/latest/example/simple.html
 """
+
 import numpy as np
 import pytest
 
 
 def pytest_addoption(parser):
     parser.addoption(
         "--benchmark", action="store_true", default=False, help="run benchmark"
```

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a28/1a28_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a28/1a28_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a28/1a28_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a28/1a28_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a4k/1a4k_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a4k/1a4k_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a4k/1a4k_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a4k/1a4k_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a4r/1a4r_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a4r/1a4r_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a4r/1a4r_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a4r/1a4r_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a69/1a69_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a69/1a69_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a69/1a69_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a69/1a69_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a94/1a94_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a94/1a94_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a94/1a94_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a94/1a94_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a99/1a99_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a99/1a99_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a99/1a99_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a99/1a99_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a9m/1a9m_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a9m/1a9m_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a9m/1a9m_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a9m/1a9m_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a9q/1a9q_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a9q/1a9q_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1a9q/1a9q_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1a9q/1a9q_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1aaq/1aaq_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1aaq/1aaq_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1aaq/1aaq_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1aaq/1aaq_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1add/1add_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1add/1add_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1add/1add_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1add/1add_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1adl/1adl_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1adl/1adl_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1adl/1adl_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1adl/1adl_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ado/1ado_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ado/1ado_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ado/1ado_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ado/1ado_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1afk/1afk_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1afk/1afk_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1afk/1afk_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1afk/1afk_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1afl/1afl_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1afl/1afl_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1afl/1afl_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1afl/1afl_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ai4/1ai4_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ai4/1ai4_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ai4/1ai4_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ai4/1ai4_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ai5/1ai5_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ai5/1ai5_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ai5/1ai5_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ai5/1ai5_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ai7/1ai7_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ai7/1ai7_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ai7/1ai7_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ai7/1ai7_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1aid/1aid_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1aid/1aid_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1aid/1aid_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1aid/1aid_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1aj7/1aj7_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1aj7/1aj7_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1aj7/1aj7_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1aj7/1aj7_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ajn/1ajn_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ajn/1ajn_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ajn/1ajn_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ajn/1ajn_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ajp/1ajp_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ajp/1ajp_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ajp/1ajp_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ajp/1ajp_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ajq/1ajq_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ajq/1ajq_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ajq/1ajq_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ajq/1ajq_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ajv/1ajv_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ajv/1ajv_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ajv/1ajv_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ajv/1ajv_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ajx/1ajx_dock.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ajx/1ajx_dock.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/docking/1ajx/1ajx_ligand.sdf` & `spyrmsd-0.7.0/tests/data/docking/1ajx/1ajx_ligand.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/1a99_ligand.pdb` & `spyrmsd-0.7.0/tests/data/molecules/1a99_ligand.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/1a99_ligand.pdb.gz` & `spyrmsd-0.7.0/tests/data/molecules/1a99_ligand.pdb.gz`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/1cbr_docking.mol2` & `spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.mol2`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/1cbr_docking.pdb` & `spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/1cbr_docking.sdf` & `spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/1cbr_docking.sdf.gz` & `spyrmsd-0.7.0/tests/data/molecules/1cbr_docking.sdf.gz`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/1cbr_ligand.mol2` & `spyrmsd-0.7.0/tests/data/molecules/1cbr_ligand.mol2`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/2viz_1.sdf` & `spyrmsd-0.7.0/tests/data/molecules/2viz_1.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/2viz_2.sdf` & `spyrmsd-0.7.0/tests/data/molecules/2viz_2.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/2viz_3.sdf` & `spyrmsd-0.7.0/tests/data/molecules/2viz_3.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/benzene.mol2` & `spyrmsd-0.7.0/tests/data/molecules/benzene.mol2`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/benzene.sdf` & `spyrmsd-0.7.0/tests/data/molecules/benzene.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/benzene.xyz` & `spyrmsd-0.7.0/tests/data/molecules/benzene.xyz`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/dialanine.sdf` & `spyrmsd-0.7.0/tests/data/molecules/dialanine.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/ethanol.sdf` & `spyrmsd-0.7.0/tests/data/molecules/ethanol.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/pyridine.sdf` & `spyrmsd-0.7.0/tests/data/molecules/pyridine.sdf`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/pyridine.xyz` & `spyrmsd-0.7.0/tests/data/molecules/pyridine.xyz`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/trp0.pdb` & `spyrmsd-0.7.0/tests/data/molecules/trp0.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/trp1.pdb` & `spyrmsd-0.7.0/tests/data/molecules/trp1.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/trp2.pdb` & `spyrmsd-0.7.0/tests/data/molecules/trp2.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/trp3.pdb` & `spyrmsd-0.7.0/tests/data/molecules/trp3.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/trp4.pdb` & `spyrmsd-0.7.0/tests/data/molecules/trp4.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/data/molecules/trp5.pdb` & `spyrmsd-0.7.0/tests/data/molecules/trp5.pdb`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/molecules.py` & `spyrmsd-0.7.0/tests/molecules.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/test_benchmarks.py` & `spyrmsd-0.7.0/tests/test_benchmarks.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
     # Match 4-character strings starting with a number
     systems = [d for d in dirs if re.match("[1-9]...", d)]
 
     return systems
 
 
-@pytest.mark.benchmark
 @pytest.fixture(scope="module", params=systems())
 def molecules(request):
     system = request.param
 
     fref = os.path.join(molpath, system, f"{system}_ligand.sdf")
     fmols = os.path.join(molpath, system, f"{system}_dock.sdf")
```

### Comparing `spyrmsd-0.6.0/tests/test_graph.py` & `spyrmsd-0.7.0/tests/test_graph.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
 import pytest
 
+import spyrmsd
 from spyrmsd import constants, graph, io, molecule
 from spyrmsd.exceptions import NonIsomorphicGraphs
+from spyrmsd.graphs import _common as gc
 from tests import molecules
 
 
 def test_adjacency_matrix_from_atomic_coordinates_distance() -> None:
     # Lithium hydride (LiH)
     # H and Li have very different covalent radii
     atomicnums = np.array([1, 3])
@@ -100,33 +102,31 @@
     "G1, G2",
     [
         *[(graph.lattice(n, n), graph.lattice(n, n)) for n in range(2, 5)],
         *[(graph.cycle(n), graph.cycle(n)) for n in range(2, 5)],
     ],
 )
 def test_match_graphs_isomorphic(G1, G2) -> None:
-    with pytest.warns(
-        UserWarning, match="No atomic property information stored on nodes."
-    ):
+    with pytest.warns(UserWarning, match=gc.warn_no_atomic_properties):
         isomorphisms = graph.match_graphs(G1, G2)
 
     assert len(isomorphisms) != 0
 
 
 @pytest.mark.parametrize(
     "G1, G2",
     [
         *[(graph.lattice(n, n), graph.lattice(n + 1, n)) for n in range(2, 5)],
         *[(graph.cycle(n), graph.cycle(n + 1)) for n in range(1, 5)],
     ],
 )
 def test_match_graphs_not_isomorphic(G1, G2) -> None:
     with pytest.raises(
-        NonIsomorphicGraphs, match="Graphs are not isomorphic."
-    ), pytest.warns(UserWarning, match="No atomic number information stored on nodes."):
+        NonIsomorphicGraphs, match=gc.error_non_isomorphic_graphs
+    ), pytest.warns(UserWarning, match=gc.warn_no_atomic_properties):
         graph.match_graphs(G1, G2)
 
 
 @pytest.mark.parametrize(
     "property",
     [
         np.array([0, 1, 2], dtype=int),
@@ -139,18 +139,52 @@
 def test_build_graph_node_features(property) -> None:
     A = np.array([[0, 1, 1], [1, 0, 0], [1, 0, 1]])
     G = graph.graph_from_adjacency_matrix(A, property)
 
     assert graph.num_edges(G) == 3
 
 
+@pytest.mark.skipif(
+    spyrmsd.get_backend() != "graph_tool",
+    reason="NetworkX supports all Python objects as node properties.",
+)
 def test_build_graph_node_features_unsupported() -> None:
-    pytest.importorskip(
-        "graph_tool", reason="NetworkX supports all Python objects as node properties."
-    )
-
     A = np.array([[0, 1, 1], [1, 0, 0], [1, 0, 1]])
 
     property = [True, False, True]
 
     with pytest.raises(ValueError, match="Unsupported property type:"):
         _ = graph.graph_from_adjacency_matrix(A, property)
+
+
+@pytest.mark.skipif(
+    # Run test if all supported backends are installed
+    not set(spyrmsd.graph._supported_backends) <= set(spyrmsd.available_backends),
+    reason="Not all of the required backends are installed",
+)
+def test_set_backend() -> None:
+    import graph_tool as gt
+    import networkx as nx
+    import rustworkx as rx
+
+    A = np.array([[0, 1, 1], [1, 0, 0], [1, 0, 1]])
+
+    spyrmsd.set_backend("networkx")
+    assert spyrmsd.get_backend() == "networkx"
+
+    Gnx = graph.graph_from_adjacency_matrix(A)
+    assert isinstance(Gnx, nx.Graph)
+
+    spyrmsd.set_backend("graph-tool")
+    assert spyrmsd.get_backend() == "graph_tool"
+
+    Ggt = graph.graph_from_adjacency_matrix(A)
+    assert isinstance(Ggt, gt.Graph)
+
+    spyrmsd.set_backend("rustworkx")
+    assert spyrmsd.get_backend() == "rustworkx"
+
+    Grx = graph.graph_from_adjacency_matrix(A)
+    assert isinstance(Grx, rx.PyGraph)
+
+    with pytest.raises(ValueError, match="backend is not recognized or supported"):
+        spyrmsd.set_backend("unknown")
```

### Comparing `spyrmsd-0.6.0/tests/test_hungarian.py` & `spyrmsd-0.7.0/tests/test_hungarian.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/test_import.py` & `spyrmsd-0.7.0/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/test_io.py` & `spyrmsd-0.7.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/test_large.py` & `spyrmsd-0.7.0/tests/test_large.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/test_qcp.py` & `spyrmsd-0.7.0/tests/test_qcp.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/test_rmsd.py` & `spyrmsd-0.7.0/tests/test_rmsd.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/tests/test_utils.py` & `spyrmsd-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `spyrmsd-0.6.0/PKG-INFO` & `spyrmsd-0.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: spyrmsd
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python RMSD tool with symmetry correction.
 Home-page: https://spyrmsd.readthedocs.io
 Author: Rocco Meli
 Author-email: rocco.meli@cscs.ch
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: networkx>=2
 
@@ -20,15 +20,15 @@
 ![mypy](https://github.com/RMeli/spyrmsd/workflows/mypy/badge.svg)
 [![codecov](https://codecov.io/gh/RMeli/spyrmsd/branch/develop/graph/badge.svg)](https://codecov.io/gh/RMeli/spyrmsd/branch/master)
 
 [![Docs](https://img.shields.io/badge/docs-spyrmsd.readthedocs.io-blueviolet)](https://spyrmsd.readthedocs.io)
 [![Documentation Status](https://readthedocs.org/projects/spyrmsd/badge/?version=develop)](https://spyrmsd.readthedocs.io/en/develop/?badge=develop)
 
 [![License](https://img.shields.io/github/license/RMeli/pyrmsd?color=%2333BBFF)](https://opensource.org/licenses/MIT)
-[![PyPI](https://img.shields.io/badge/PyPI-v0.6.0%20-ff69b4)](https://pypi.org/project/spyrmsd/)
+[![PyPI](https://img.shields.io/badge/PyPI-v0.7.0%20-ff69b4)](https://pypi.org/project/spyrmsd/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/spyrmsd.svg)](https://anaconda.org/conda-forge/spyrmsd)
 
 [![J. Cheminform.](https://img.shields.io/badge/J.%20Cheminform.-10.1186%2Fs13321--020--00455--2-blue)](https://doi.org/10.1186/s13321-020-00455-2)
 [![Zenodo](https://zenodo.org/badge/214157073.svg)](https://zenodo.org/badge/latestdoi/214157073)
 
 Python tool for symmetry-corrected RMSD calculations.
 
@@ -49,15 +49,15 @@
 ```
 
 ## Installation
 
 `spyrmsd` is available on [PyPI](https://pypi.org/project/spyrmsd/) and [conda-forge](https://github.com/conda-forge/spyrmsd-feedstock) and can be easily installed from source. See [Dependencies](###Dependencies) for a description of all the dependencies.
 
 > [!NOTE]
-> `spyrmsd` will install [NetworkX](https://networkx.github.io/) (multi-platform). You can install [graph-tool](https://graph-tool.skewed.de/) on macOS and Linux for higher performance.
+> `spyrmsd` will install [NetworkX](https://networkx.github.io/) (multi-platform). You can install the other backends for higher performance.
 
 > [!WARNING]
 > If `spyrmsd` is used as a standalone tool, it is required to install either [RDKit](https://rdkit.org/) or [Open Babel](http://openbabel.org/). Neither is automatically installed with `pip` nor `conda`.
 
 ### PyPI
 
 ```bash
@@ -82,53 +82,42 @@
 
 `spyrmsd` can be used both as a module or as a standalone tool.
 
 #### Module
 
 The following packages are required to use `spyrmsd` as a module:
 
-* [graph-tool](https://graph-tool.skewed.de/) or [NetworkX](https://networkx.github.io/)
 * [numpy](https://numpy.org/)
 * [scipy](https://www.scipy.org/)
 
+One of the following graph libraries is required:
+* [graph-tool]
+* [NetworkX]
+* [rustworkx]
+
 > [!NOTE]
-> `spyrmsd` uses [graph-tool](https://graph-tool.skewed.de/) by default but will fall back to [NetworkX](https://networkx.github.io/) if the former is not installed (e.g. on Windows). However, in order to support cross-platform installation [NetworkX](https://networkx.github.io/) is installed by default, and [graph-tool](https://graph-tool.skewed.de/) needs to be installed manually.
+> `spyrmsd` uses the following priority when multiple graph libraries are present: [graph-tool], [NetworkX], [rustworkx]. *This order might change. Use `set_backend` to ensure you are always using the same backend, if needed.* However, in order to support cross-platform installation [NetworkX](https://networkx.github.io/) is installed by default, and the other graph library need to be installed manually.
 
 #### Standalone Tool
 
 Additionally, one of the following packages is required to use `spyrmsd` as a standalone tool:
 
 * [Open Babel](http://openbabel.org/)
 * [RDKit](https://rdkit.org/)
 
 ## Usage
 
 ### Standalone Tool
 
+`spyrmsd` provides a convenient CLI tool. See `spyrmsd`'s `--help` for the usage:
+
 ```bash
 python -m spyrmsd -h
 ```
 
-```text
-usage: python -m spyrmsd [-h] [-m] [-c] [--hydrogens] [-n] reference molecules [molecules ...]
-
-Symmetry-corrected RMSD calculations in Python.
-
-positional arguments:
-  reference       Reference file
-  molecules       Input file(s)
-
-optional arguments:
-  -h, --help      show this help message and exit
-  -m, --minimize  Minimize (fit)
-  -c, --center    Center molecules at origin
-  --hydrogens     Keep hydrogen atoms
-  -n, --nosymm    No graph isomorphism
-```
-
 ### Module
 
 ```python
 from spyrmsd import rmsd
 ```
 
 #### RMSD
@@ -144,15 +133,15 @@
     center: bool = False,   # Flag to center molecules at origin
     minimize: bool = False, # Flag to compute minimum RMSD
     atol: float = 1e-9,     # Numerical tolerance for QCP method
 )
 ```
 
 > [!NOTE]
-> Atomic properties (`aprops`) can be any Python object when using [NetworkX](https://networkx.github.io/), or integers, floats, or strings when using [graph-tool](https://graph-tool.skewed.de/).
+> Atomic properties (`aprops`) can be any Python object when using [NetworkX] and [rustworkx], or integers, floats, or strings when using [graph-tool].
 
 #### Symmetry-Corrected RMSD
 
 The function `rmsd.symmrmsd` computes symmetry-corrected RMSD using molecular graph isomorphisms. Symmetry correction requires molecular adjacency matrices describing the connectivity but needs not the atoms to be in the same order.
 
 Atom matching is performed according to the molecular graph. This function should also be used when atoms in the molecules being compared are not in the same order (even if there is not symmetry to be accounted for).
 
@@ -168,32 +157,60 @@
     minimize: bool = False,                      # Flag to compute minimum RMSD
     cache: bool = True,                          # Cache graph isomorphisms
     atol: float = 1e-9,                          # Numerical tolerance for QCP method
 )
 ```
 
 > [!NOTE]
-> Atomic properties (`aprops`) can be any Python object when using [NetworkX](https://networkx.github.io/), or integers, floats, or strings when using [graph-tool](https://graph-tool.skewed.de/).
+> Atomic properties (`aprops`) can be any Python object when using [NetworkX] and [rustworkx], or integers, floats, or strings when using [graph-tool](https://graph-tool.skewed.de/).
+
+#### Select Backend
+
+`spyrmsd` supports the following graph libraries for the calculation of graph isomorphisms:
+* [graph-tool]
+* [NetworkX]
+* [rustworkx]
+
+ You can check which backend is being used with
+
+```python
+spyrmsd.get_backend()
+```
+
+You can also manually select your preferred backend with
+
+```python
+spyrmsd.set_backend("networkx")
+# spyrmsd uses NetworkX
+spyrmsd.set_backend("graph_tool")
+# spyrmsd uses graph_tool
+```
+
+The available backends (which depend on the installed dependencies) are stored in `spyrmsd.available_backends`.
 
 ## Development
 
 To ensure code quality and consistency the following tools are used during development:
 
 * [black](https://black.readthedocs.io/en/stable/)
 * [Flake 8](http://flake8.pycqa.org/en/latest/) (CI)
 * [isort]()
 * [mypy](http://mypy-lang.org/) (CI)
 
 Pre-commit `git` hooks can be installed with [pre-commit](https://pre-commit.com/).
 
 ## Copyright
 
-Copyright (c) 2019-2021, Rocco Meli.
+Copyright (c) 2019-2024, Rocco Meli.
 
 ## References
 
 References are tracked with [duecredit](https://github.com/duecredit/duecredit/). Run the `credits.sh` script in order to print up-to-date references.
 
 ### Acknowledgements
 
 Project based on the [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version `1.1`.
 
+[rustworkx]: https://www.rustworkx.org
+[NetworkX]: https://networkx.github.io/
+[graph-tool]: https://graph-tool.skewed.de/
+
```

