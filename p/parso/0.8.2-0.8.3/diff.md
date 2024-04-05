# Comparing `tmp/parso-0.8.2.tar.gz` & `tmp/parso-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/parso-0.8.2.tar", last modified: Tue Mar 30 20:43:48 2021, max compression
+gzip compressed data, was "parso-0.8.3.tar", last modified: Tue Nov 30 21:05:45 2021, max compression
```

## Comparing `parso-0.8.2.tar` & `parso-0.8.3.tar`

### file list

```diff
@@ -1,128 +1,131 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:48.816064 parso-0.8.2/
--rw-rw-r--   0 dave      (1000) dave      (1000)      251 2021-03-30 20:43:19.000000 parso-0.8.2/.coveragerc
--rw-rw-r--   0 dave      (1000) dave      (1000)     2029 2021-03-30 20:43:19.000000 parso-0.8.2/AUTHORS.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     3363 2021-03-30 20:43:19.000000 parso-0.8.2/CHANGELOG.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     4176 2021-03-30 20:43:19.000000 parso-0.8.2/LICENSE.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      250 2021-03-30 20:43:19.000000 parso-0.8.2/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     9174 2021-03-30 20:43:48.816064 parso-0.8.2/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     2823 2021-03-30 20:43:19.000000 parso-0.8.2/README.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     4308 2021-03-30 20:43:19.000000 parso-0.8.2/conftest.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:48.804065 parso-0.8.2/docs/
--rw-rw-r--   0 dave      (1000) dave      (1000)     5560 2021-03-30 20:43:19.000000 parso-0.8.2/docs/Makefile
--rw-rw-r--   0 dave      (1000) dave      (1000)       73 2021-03-30 20:43:19.000000 parso-0.8.2/docs/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:48.804065 parso-0.8.2/docs/_static/
--rw-rw-r--   0 dave      (1000) dave      (1000)   204714 2021-03-30 20:43:19.000000 parso-0.8.2/docs/_static/logo.png
--rw-rw-r--   0 dave      (1000) dave      (1000)    56519 2021-03-30 20:43:19.000000 parso-0.8.2/docs/_static/logo_characters.png
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:48.804065 parso-0.8.2/docs/_templates/
--rw-rw-r--   0 dave      (1000) dave      (1000)      231 2021-03-30 20:43:19.000000 parso-0.8.2/docs/_templates/ghbuttons.html
--rw-rw-r--   0 dave      (1000) dave      (1000)      136 2021-03-30 20:43:19.000000 parso-0.8.2/docs/_templates/sidebarlogo.html
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:48.804065 parso-0.8.2/docs/_themes/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:48.804065 parso-0.8.2/docs/_themes/flask/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1789 2021-03-30 20:43:19.000000 parso-0.8.2/docs/_themes/flask/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      924 2021-03-30 20:43:19.000000 parso-0.8.2/docs/_themes/flask/layout.html
--rw-rw-r--   0 dave      (1000) dave      (1000)      590 2021-03-30 20:43:19.000000 parso-0.8.2/docs/_themes/flask/relations.html
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:48.804065 parso-0.8.2/docs/_themes/flask/static/
--rw-rw-r--   0 dave      (1000) dave      (1000)     6411 2021-03-30 20:43:19.000000 parso-0.8.2/docs/_themes/flask/static/flasky.css_t
--rw-rw-r--   0 dave      (1000) dave      (1000)      976 2021-03-30 20:43:19.000000 parso-0.8.2/docs/_themes/flask/static/small_flask.css
--rw-rw-r--   0 dave      (1000) dave      (1000)      162 2021-03-30 20:43:19.000000 parso-0.8.2/docs/_themes/flask/theme.conf
--rw-rw-r--   0 dave      (1000) dave      (1000)     6672 2021-03-30 20:43:19.000000 parso-0.8.2/docs/_themes/flask_theme_support.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     9167 2021-03-30 20:43:19.000000 parso-0.8.2/docs/conf.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:48.804065 parso-0.8.2/docs/docs/
--rw-rw-r--   0 dave      (1000) dave      (1000)      839 2021-03-30 20:43:19.000000 parso-0.8.2/docs/docs/development.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      867 2021-03-30 20:43:19.000000 parso-0.8.2/docs/docs/installation.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      992 2021-03-30 20:43:19.000000 parso-0.8.2/docs/docs/parser-tree.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1555 2021-03-30 20:43:19.000000 parso-0.8.2/docs/docs/usage.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       66 2021-03-30 20:43:19.000000 parso-0.8.2/docs/global.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      516 2021-03-30 20:43:19.000000 parso-0.8.2/docs/index.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:48.804065 parso-0.8.2/parso/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1607 2021-03-30 20:43:19.000000 parso-0.8.2/parso/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       70 2021-03-30 20:43:19.000000 parso-0.8.2/parso/_compatibility.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     8452 2021-03-30 20:43:19.000000 parso-0.8.2/parso/cache.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1023 2021-03-30 20:43:19.000000 parso-0.8.2/parso/file_io.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    10483 2021-03-30 20:43:19.000000 parso-0.8.2/parso/grammar.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5597 2021-03-30 20:43:19.000000 parso-0.8.2/parso/normalizer.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7205 2021-03-30 20:43:19.000000 parso-0.8.2/parso/parser.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:48.808064 parso-0.8.2/parso/pgen2/
--rw-rw-r--   0 dave      (1000) dave      (1000)      382 2021-03-30 20:43:19.000000 parso-0.8.2/parso/pgen2/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    14570 2021-03-30 20:43:19.000000 parso-0.8.2/parso/pgen2/generator.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5515 2021-03-30 20:43:19.000000 parso-0.8.2/parso/pgen2/grammar_parser.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:48.808064 parso-0.8.2/parso/python/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:19.000000 parso-0.8.2/parso/python/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    34206 2021-03-30 20:43:19.000000 parso-0.8.2/parso/python/diff.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    48003 2021-03-30 20:43:19.000000 parso-0.8.2/parso/python/errors.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7608 2021-03-30 20:43:19.000000 parso-0.8.2/parso/python/grammar310.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     6948 2021-03-30 20:43:19.000000 parso-0.8.2/parso/python/grammar36.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     6804 2021-03-30 20:43:19.000000 parso-0.8.2/parso/python/grammar37.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     7591 2021-03-30 20:43:19.000000 parso-0.8.2/parso/python/grammar38.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     7596 2021-03-30 20:43:19.000000 parso-0.8.2/parso/python/grammar39.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     8227 2021-03-30 20:43:19.000000 parso-0.8.2/parso/python/parser.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    33565 2021-03-30 20:43:19.000000 parso-0.8.2/parso/python/pep8.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2459 2021-03-30 20:43:19.000000 parso-0.8.2/parso/python/prefix.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      909 2021-03-30 20:43:19.000000 parso-0.8.2/parso/python/token.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    25766 2021-03-30 20:43:19.000000 parso-0.8.2/parso/python/tokenize.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    36707 2021-03-30 20:43:19.000000 parso-0.8.2/parso/python/tree.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    11598 2021-03-30 20:43:19.000000 parso-0.8.2/parso/tree.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     6606 2021-03-30 20:43:19.000000 parso-0.8.2/parso/utils.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:48.804065 parso-0.8.2/parso.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     9174 2021-03-30 20:43:48.000000 parso-0.8.2/parso.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     3010 2021-03-30 20:43:48.000000 parso-0.8.2/parso.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2021-03-30 20:43:48.000000 parso-0.8.2/parso.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       63 2021-03-30 20:43:48.000000 parso-0.8.2/parso.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        6 2021-03-30 20:43:48.000000 parso-0.8.2/parso.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      356 2021-03-30 20:43:19.000000 parso-0.8.2/pytest.ini
--rw-rw-r--   0 dave      (1000) dave      (1000)      322 2021-03-30 20:43:48.820064 parso-0.8.2/setup.cfg
--rwxrwxr-x   0 dave      (1000) dave      (1000)     1721 2021-03-30 20:43:19.000000 parso-0.8.2/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:48.812064 parso-0.8.2/test/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:19.000000 parso-0.8.2/test/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     8985 2021-03-30 20:43:19.000000 parso-0.8.2/test/failing_examples.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    11338 2021-03-30 20:43:19.000000 parso-0.8.2/test/fuzz_diff_parser.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-03-30 20:43:48.816064 parso-0.8.2/test/normalizer_issue_files/
--rw-rw-r--   0 dave      (1000) dave      (1000)      758 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E10.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2634 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E101.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1043 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E11.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1507 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E12_first.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     6368 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E12_not_first.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7385 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E12_not_second.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4070 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E12_second.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2291 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E12_third.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      716 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E20.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      323 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E21.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2155 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E22.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      179 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E23.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      876 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E25.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1509 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E26.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      668 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E27.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      146 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E29.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1484 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E30.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1747 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E30not.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      554 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E40.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3051 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E50.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      399 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E70.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1130 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E71.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1084 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E72.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      221 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/E73.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1410 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)     1781 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/allowed_syntax.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      152 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/latin-1.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/python.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       83 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/utf-8-bom.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1864 2021-03-30 20:43:19.000000 parso-0.8.2/test/normalizer_issue_files/utf-8.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     6687 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_cache.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    38713 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_diff_parser.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4736 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_error_recovery.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      702 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_file_python_errors.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4080 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_fstring.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2891 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_get_code.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      127 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_grammar.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      979 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_load_grammar.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2284 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_normalizer_issues_files.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3534 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_old_fast_parser.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1328 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_param_splitting.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5906 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_parser.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7325 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_parser_tree.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      897 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_pep8.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     9171 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_pgen2.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2213 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_prefix.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    15039 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_python_errors.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    13618 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_tokenize.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2762 2021-03-30 20:43:19.000000 parso-0.8.2/test/test_utils.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-11-30 21:05:45.521858 parso-0.8.3/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      273 2021-11-30 21:04:12.000000 parso-0.8.3/.coveragerc
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2029 2021-11-30 21:04:12.000000 parso-0.8.3/AUTHORS.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3448 2021-11-30 21:04:12.000000 parso-0.8.3/CHANGELOG.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4176 2021-11-30 21:04:12.000000 parso-0.8.3/LICENSE.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      250 2021-11-30 21:04:12.000000 parso-0.8.3/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9328 2021-11-30 21:05:45.521858 parso-0.8.3/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2852 2021-11-30 21:04:12.000000 parso-0.8.3/README.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4308 2021-11-30 21:04:12.000000 parso-0.8.3/conftest.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-11-30 21:05:45.505857 parso-0.8.3/docs/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5560 2021-11-30 21:04:12.000000 parso-0.8.3/docs/Makefile
+-rw-rw-r--   0 dave      (1000) dave      (1000)       73 2021-11-30 21:04:12.000000 parso-0.8.3/docs/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-11-30 21:05:45.509857 parso-0.8.3/docs/_static/
+-rw-rw-r--   0 dave      (1000) dave      (1000)   204714 2021-11-30 21:04:12.000000 parso-0.8.3/docs/_static/logo.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)    56519 2021-11-30 21:04:12.000000 parso-0.8.3/docs/_static/logo_characters.png
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-11-30 21:05:45.509857 parso-0.8.3/docs/_templates/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      231 2021-11-30 21:04:12.000000 parso-0.8.3/docs/_templates/ghbuttons.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)      136 2021-11-30 21:04:12.000000 parso-0.8.3/docs/_templates/sidebarlogo.html
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-11-30 21:05:45.509857 parso-0.8.3/docs/_themes/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-11-30 21:05:45.509857 parso-0.8.3/docs/_themes/flask/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1789 2021-11-30 21:04:12.000000 parso-0.8.3/docs/_themes/flask/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      924 2021-11-30 21:04:12.000000 parso-0.8.3/docs/_themes/flask/layout.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)      590 2021-11-30 21:04:12.000000 parso-0.8.3/docs/_themes/flask/relations.html
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-11-30 21:05:45.509857 parso-0.8.3/docs/_themes/flask/static/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6411 2021-11-30 21:04:12.000000 parso-0.8.3/docs/_themes/flask/static/flasky.css_t
+-rw-rw-r--   0 dave      (1000) dave      (1000)      976 2021-11-30 21:04:12.000000 parso-0.8.3/docs/_themes/flask/static/small_flask.css
+-rw-rw-r--   0 dave      (1000) dave      (1000)      162 2021-11-30 21:04:12.000000 parso-0.8.3/docs/_themes/flask/theme.conf
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6672 2021-11-30 21:04:12.000000 parso-0.8.3/docs/_themes/flask_theme_support.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9167 2021-11-30 21:04:12.000000 parso-0.8.3/docs/conf.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-11-30 21:05:45.509857 parso-0.8.3/docs/docs/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      848 2021-11-30 21:04:12.000000 parso-0.8.3/docs/docs/development.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      867 2021-11-30 21:04:12.000000 parso-0.8.3/docs/docs/installation.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      992 2021-11-30 21:04:12.000000 parso-0.8.3/docs/docs/parser-tree.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1555 2021-11-30 21:04:12.000000 parso-0.8.3/docs/docs/usage.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       66 2021-11-30 21:04:12.000000 parso-0.8.3/docs/global.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      529 2021-11-30 21:04:12.000000 parso-0.8.3/docs/index.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-11-30 21:05:45.509857 parso-0.8.3/parso/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1607 2021-11-30 21:04:12.000000 parso-0.8.3/parso/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       70 2021-11-30 21:04:12.000000 parso-0.8.3/parso/_compatibility.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8452 2021-11-30 21:04:12.000000 parso-0.8.3/parso/cache.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1023 2021-11-30 21:04:12.000000 parso-0.8.3/parso/file_io.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10483 2021-11-30 21:04:12.000000 parso-0.8.3/parso/grammar.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5597 2021-11-30 21:04:12.000000 parso-0.8.3/parso/normalizer.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7182 2021-11-30 21:04:12.000000 parso-0.8.3/parso/parser.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-11-30 21:05:45.509857 parso-0.8.3/parso/pgen2/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      382 2021-11-30 21:04:12.000000 parso-0.8.3/parso/pgen2/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    14570 2021-11-30 21:04:12.000000 parso-0.8.3/parso/pgen2/generator.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5515 2021-11-30 21:04:12.000000 parso-0.8.3/parso/pgen2/grammar_parser.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-11-30 21:05:45.513857 parso-0.8.3/parso/python/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    34206 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/diff.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    47955 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/errors.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7511 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/grammar310.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7511 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/grammar311.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7511 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/grammar312.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6948 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/grammar36.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6804 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/grammar37.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7591 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/grammar38.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7499 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/grammar39.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8108 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/parser.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    33779 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/pep8.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2743 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/prefix.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      909 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/token.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    25795 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/tokenize.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    37187 2021-11-30 21:04:12.000000 parso-0.8.3/parso/python/tree.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    16153 2021-11-30 21:04:12.000000 parso-0.8.3/parso/tree.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6620 2021-11-30 21:04:12.000000 parso-0.8.3/parso/utils.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-11-30 21:05:45.509857 parso-0.8.3/parso.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9328 2021-11-30 21:05:45.000000 parso-0.8.3/parso.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3089 2021-11-30 21:05:45.000000 parso-0.8.3/parso.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2021-11-30 21:05:45.000000 parso-0.8.3/parso.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       63 2021-11-30 21:05:45.000000 parso-0.8.3/parso.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        6 2021-11-30 21:05:45.000000 parso-0.8.3/parso.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      356 2021-11-30 21:04:12.000000 parso-0.8.3/pytest.ini
+-rw-rw-r--   0 dave      (1000) dave      (1000)      322 2021-11-30 21:05:45.521858 parso-0.8.3/setup.cfg
+-rwxrwxr-x   0 dave      (1000) dave      (1000)     1721 2021-11-30 21:04:12.000000 parso-0.8.3/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-11-30 21:05:45.517857 parso-0.8.3/test/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2021-11-30 21:04:12.000000 parso-0.8.3/test/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8985 2021-11-30 21:04:12.000000 parso-0.8.3/test/failing_examples.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11338 2021-11-30 21:04:12.000000 parso-0.8.3/test/fuzz_diff_parser.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-11-30 21:05:45.521858 parso-0.8.3/test/normalizer_issue_files/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      758 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E10.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2634 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E101.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1043 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E11.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1507 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E12_first.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6368 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E12_not_first.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7385 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E12_not_second.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4070 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E12_second.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2291 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E12_third.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      716 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E20.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      323 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E21.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2155 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E22.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      179 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E23.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      876 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E25.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1509 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E26.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      668 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E27.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      146 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E29.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1484 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E30.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1747 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E30not.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      554 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E40.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3051 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E50.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      399 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E70.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1130 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E71.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1084 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E72.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      221 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/E73.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1410 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1781 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/allowed_syntax.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      152 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/latin-1.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/python.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       83 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/utf-8-bom.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1864 2021-11-30 21:04:12.000000 parso-0.8.3/test/normalizer_issue_files/utf-8.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6751 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_cache.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    38713 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_diff_parser.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6351 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_dump_tree.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4736 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_error_recovery.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      702 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_file_python_errors.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4080 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_fstring.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2891 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_get_code.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      127 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_grammar.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      979 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_load_grammar.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2284 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_normalizer_issues_files.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3534 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_old_fast_parser.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1328 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_param_splitting.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5906 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_parser.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8273 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_parser_tree.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      971 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_pep8.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9174 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_pgen2.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2265 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_prefix.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    15566 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_python_errors.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    13618 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_tokenize.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2952 2021-11-30 21:04:12.000000 parso-0.8.3/test/test_utils.py
```

### Comparing `parso-0.8.2/AUTHORS.txt` & `parso-0.8.3/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/CHANGELOG.rst` & `parso-0.8.3/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 Changelog
 ---------
 
 Unreleased
 ++++++++++
 
+0.8.3 (2021-11-30)
+++++++++++++++++++
+
+- Add basic support for Python 3.11 and 3.12
+
 0.8.2 (2021-03-30)
 ++++++++++++++++++
 
 - Various small bugfixes
 
 0.8.1 (2020-12-10)
 ++++++++++++++++++
```

### Comparing `parso-0.8.2/LICENSE.txt` & `parso-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/PKG-INFO` & `parso-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: parso
-Version: 0.8.2
+Version: 0.8.3
 Summary: A Python Parser
 Home-page: https://github.com/davidhalter/parso
 Author: David Halter
 Author-email: davidhalter88@gmail.com
 Maintainer: David Halter
 Maintainer-email: davidhalter88@gmail.com
 License: MIT
 Description: ###################################################################
         parso - A Python Parser
         ###################################################################
         
         
-        .. image:: https://travis-ci.org/davidhalter/parso.svg?branch=master
-            :target: https://travis-ci.org/davidhalter/parso
-            :alt: Travis CI build status
+        .. image:: https://github.com/davidhalter/parso/workflows/Build/badge.svg?branch=master
+            :target: https://github.com/davidhalter/parso/actions
+            :alt: GitHub Actions build status
         
         .. image:: https://coveralls.io/repos/github/davidhalter/parso/badge.svg?branch=master
             :target: https://coveralls.io/github/davidhalter/parso?branch=master
             :alt: Coverage Status
         
         .. image:: https://pepy.tech/badge/parso
             :target: https://pepy.tech/project/parso
@@ -109,14 +109,19 @@
         
         Changelog
         ---------
         
         Unreleased
         ++++++++++
         
+        0.8.3 (2021-11-30)
+        ++++++++++++++++++
+        
+        - Add basic support for Python 3.11 and 3.12
+        
         0.8.2 (2021-03-30)
         ++++++++++++++++++
         
         - Various small bugfixes
         
         0.8.1 (2020-12-10)
         ++++++++++++++++++
```

### Comparing `parso-0.8.2/README.rst` & `parso-0.8.3/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ###################################################################
 parso - A Python Parser
 ###################################################################
 
 
-.. image:: https://travis-ci.org/davidhalter/parso.svg?branch=master
-    :target: https://travis-ci.org/davidhalter/parso
-    :alt: Travis CI build status
+.. image:: https://github.com/davidhalter/parso/workflows/Build/badge.svg?branch=master
+    :target: https://github.com/davidhalter/parso/actions
+    :alt: GitHub Actions build status
 
 .. image:: https://coveralls.io/repos/github/davidhalter/parso/badge.svg?branch=master
     :target: https://coveralls.io/github/davidhalter/parso?branch=master
     :alt: Coverage Status
 
 .. image:: https://pepy.tech/badge/parso
     :target: https://pepy.tech/project/parso
```

### Comparing `parso-0.8.2/conftest.py` & `parso-0.8.3/conftest.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/docs/Makefile` & `parso-0.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/docs/_static/logo.png` & `parso-0.8.3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/docs/_static/logo_characters.png` & `parso-0.8.3/docs/_static/logo_characters.png`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/docs/_themes/flask/LICENSE` & `parso-0.8.3/docs/_themes/flask/LICENSE`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/docs/_themes/flask/layout.html` & `parso-0.8.3/docs/_themes/flask/layout.html`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/docs/_themes/flask/relations.html` & `parso-0.8.3/docs/_themes/flask/relations.html`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/docs/_themes/flask/static/flasky.css_t` & `parso-0.8.3/docs/_themes/flask/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/docs/_themes/flask/static/small_flask.css` & `parso-0.8.3/docs/_themes/flask/static/small_flask.css`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/docs/_themes/flask_theme_support.py` & `parso-0.8.3/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/docs/conf.py` & `parso-0.8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/docs/docs/development.rst` & `parso-0.8.3/docs/docs/development.rst`

 * *Files 22% similar despite different names*

```diff
@@ -30,9 +30,9 @@
     pytest
 
 If you want to test only a specific Python version (e.g. Python 3.9), it's as
 easy as::
 
     python3.9 -m pytest
 
-Tests are also run automatically on `Travis CI
-<https://travis-ci.org/davidhalter/parso/>`_.
+Tests are also run automatically on `GitHub Actions
+<https://github.com/davidhalter/parso/actions>`_.
```

### Comparing `parso-0.8.2/docs/docs/installation.rst` & `parso-0.8.3/docs/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/docs/docs/parser-tree.rst` & `parso-0.8.3/docs/docs/parser-tree.rst`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/docs/docs/usage.rst` & `parso-0.8.3/docs/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/docs/index.rst` & `parso-0.8.3/docs/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -23,9 +23,9 @@
 
 .. _resources:
 
 Resources
 ---------
 
 - `Source Code on Github <https://github.com/davidhalter/parso>`_
-- `Travis Testing <https://travis-ci.org/davidhalter/parso>`_
+- `GitHub Actions Testing <https://github.com/davidhalter/parso/actions>`_
 - `Python Package Index <http://pypi.python.org/pypi/parso/>`_
```

### Comparing `parso-0.8.2/parso/__init__.py` & `parso-0.8.3/parso/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 """
 
 from parso.parser import ParserSyntaxError
 from parso.grammar import Grammar, load_grammar
 from parso.utils import split_lines, python_bytes_to_unicode
 
 
-__version__ = '0.8.2'
+__version__ = '0.8.3'
 
 
 def parse(code=None, **kwargs):
     """
     A utility function to avoid loading grammars.
     Params are documented in :py:meth:`parso.Grammar.parse`.
```

### Comparing `parso-0.8.2/parso/cache.py` & `parso-0.8.3/parso/cache.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/parso/file_io.py` & `parso-0.8.3/parso/file_io.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/parso/grammar.py` & `parso-0.8.3/parso/grammar.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/parso/normalizer.py` & `parso-0.8.3/parso/normalizer.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/parso/parser.py` & `parso-0.8.3/parso/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 There's one important optimization that needs to be known: Statements are not
 being parsed completely. ``Statement`` is just a representation of the tokens
 within the statement. This lowers memory usage and cpu time and reduces the
 complexity of the ``Parser`` (there's another parser sitting inside
 ``Statement``, which produces ``Array`` and ``Call``).
 """
-from typing import Dict
+from typing import Dict, Type
 
 from parso import tree
 from parso.pgen2.generator import ReservedString
 
 
 class ParserSyntaxError(Exception):
     """
@@ -106,18 +106,18 @@
     to parse separate token sequences.
 
     See python/tokenize.py for how to get input tokens by a string.
 
     When a syntax error occurs, error_recovery() is called.
     """
 
-    node_map: Dict[str, type] = {}
+    node_map: Dict[str, Type[tree.BaseNode]] = {}
     default_node = tree.Node
 
-    leaf_map: Dict[str, type] = {}
+    leaf_map: Dict[str, Type[tree.Leaf]] = {}
     default_leaf = tree.Leaf
 
     def __init__(self, pgen_grammar, start_nonterminal='file_input', error_recovery=False):
         self._pgen_grammar = pgen_grammar
         self._start_nonterminal = start_nonterminal
         self._error_recovery = error_recovery
 
@@ -152,16 +152,14 @@
             raise ParserSyntaxError('SyntaxError: invalid syntax', error_leaf)
 
     def convert_node(self, nonterminal, children):
         try:
             node = self.node_map[nonterminal](children)
         except KeyError:
             node = self.default_node(nonterminal, children)
-        for c in children:
-            c.parent = node
         return node
 
     def convert_leaf(self, type_, value, prefix, start_pos):
         try:
             return self.leaf_map[type_](value, start_pos, prefix)
         except KeyError:
             return self.default_leaf(value, start_pos, prefix)
```

### Comparing `parso-0.8.2/parso/pgen2/generator.py` & `parso-0.8.3/parso/pgen2/generator.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/parso/pgen2/grammar_parser.py` & `parso-0.8.3/parso/pgen2/grammar_parser.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/parso/python/diff.py` & `parso-0.8.3/parso/python/diff.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/parso/python/errors.py` & `parso-0.8.3/parso/python/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 import codecs
 import warnings
 import re
 from contextlib import contextmanager
 
 from parso.normalizer import Normalizer, NormalizerConfig, Issue, Rule
-from parso.python.tree import search_ancestor
 from parso.python.tokenize import _get_token_collection
 
 _BLOCK_STMTS = ('if_stmt', 'while_stmt', 'for_stmt', 'try_stmt', 'with_stmt')
 _STAR_EXPR_PARENTS = ('testlist_star_expr', 'testlist_comp', 'exprlist')
 # This is the maximal block size given by python.
 _MAX_BLOCK_SIZE = 20
 _MAX_INDENT_COUNT = 100
@@ -227,15 +226,15 @@
     if version < (3, 9) or node is None:
         return False
     if node.type == "error_node":
         return any(child.type == "fstring_start" for child in node.children)
     elif node.type == "fstring":
         return True
     else:
-        return search_ancestor(node, "fstring")
+        return node.search_ancestor("fstring")
 
 
 class _Context:
     def __init__(self, node, add_syntax_error, parent_context=None):
         self.node = node
         self.blocks = []
         self.parent_context = parent_context
@@ -1261,15 +1260,15 @@
             elif comp_for.type == 'comp_for':
                 comp = comp_for.children[1]
             exprlist.extend(_get_for_stmt_definition_exprs(comp))
 
         def search_all_comp_ancestors(node):
             has_ancestors = False
             while True:
-                node = search_ancestor(node, 'testlist_comp', 'dictorsetmaker')
+                node = node.search_ancestor('testlist_comp', 'dictorsetmaker')
                 if node is None:
                     break
                 for child in node.children:
                     if child.type in _COMP_FOR_TYPES:
                         process_comp_for(child)
                         has_ancestors = True
                         break
```

### Comparing `parso-0.8.2/parso/python/grammar310.txt` & `parso-0.8.3/parso/python/grammar310.txt`

 * *Files 2% similar despite different names*

```diff
@@ -93,17 +93,15 @@
 with_item: test ['as' expr]
 # NB compile.c makes sure that the default except clause is last
 except_clause: 'except' [test ['as' NAME]]
 suite: simple_stmt | NEWLINE INDENT stmt+ DEDENT
 
 namedexpr_test: test [':=' test]
 test: or_test ['if' or_test 'else' test] | lambdef
-test_nocond: or_test | lambdef_nocond
 lambdef: 'lambda' [varargslist] ':' test
-lambdef_nocond: 'lambda' [varargslist] ':' test_nocond
 or_test: and_test ('or' and_test)*
 and_test: not_test ('and' not_test)*
 not_test: 'not' not_test | comparison
 comparison: expr (comp_op expr)*
 # <> isn't actually a valid comparison operator in Python. It's here for the
 # sake of a __future__ import described in PEP 401 (which really works :-)
 comp_op: '<'|'>'|'=='|'>='|'<='|'<>'|'!='|'in'|'not' 'in'|'is'|'is' 'not'
@@ -151,15 +149,15 @@
             test '=' test |
             '**' test |
             '*' test )
 
 comp_iter: comp_for | comp_if
 sync_comp_for: 'for' exprlist 'in' or_test [comp_iter]
 comp_for: ['async'] sync_comp_for
-comp_if: 'if' test_nocond [comp_iter]
+comp_if: 'if' or_test [comp_iter]
 
 # not used in grammar, but may appear in "node" passed from Parser to Compiler
 encoding_decl: NAME
 
 yield_expr: 'yield' [yield_arg]
 yield_arg: 'from' test | testlist_star_expr
```

### Comparing `parso-0.8.2/parso/python/grammar36.txt` & `parso-0.8.3/parso/python/grammar36.txt`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/parso/python/grammar37.txt` & `parso-0.8.3/parso/python/grammar37.txt`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/parso/python/grammar38.txt` & `parso-0.8.3/parso/python/grammar38.txt`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/parso/python/grammar39.txt` & `parso-0.8.3/parso/python/grammar311.txt`

 * *Files 2% similar despite different names*

```diff
@@ -93,17 +93,15 @@
 with_item: test ['as' expr]
 # NB compile.c makes sure that the default except clause is last
 except_clause: 'except' [test ['as' NAME]]
 suite: simple_stmt | NEWLINE INDENT stmt+ DEDENT
 
 namedexpr_test: test [':=' test]
 test: or_test ['if' or_test 'else' test] | lambdef
-test_nocond: or_test | lambdef_nocond
 lambdef: 'lambda' [varargslist] ':' test
-lambdef_nocond: 'lambda' [varargslist] ':' test_nocond
 or_test: and_test ('or' and_test)*
 and_test: not_test ('and' not_test)*
 not_test: 'not' not_test | comparison
 comparison: expr (comp_op expr)*
 # <> isn't actually a valid comparison operator in Python. It's here for the
 # sake of a __future__ import described in PEP 401 (which really works :-)
 comp_op: '<'|'>'|'=='|'>='|'<='|'<>'|'!='|'in'|'not' 'in'|'is'|'is' 'not'
@@ -120,15 +118,15 @@
 atom: ('(' [yield_expr|testlist_comp] ')' |
        '[' [testlist_comp] ']' |
        '{' [dictorsetmaker] '}' |
        NAME | NUMBER | strings | '...' | 'None' | 'True' | 'False')
 testlist_comp: (namedexpr_test|star_expr) ( comp_for | (',' (namedexpr_test|star_expr))* [','] )
 trailer: '(' [arglist] ')' | '[' subscriptlist ']' | '.' NAME
 subscriptlist: subscript (',' subscript)* [',']
-subscript: test | [test] ':' [test] [sliceop]
+subscript: test [':=' test] | [test] ':' [test] [sliceop]
 sliceop: ':' [test]
 exprlist: (expr|star_expr) (',' (expr|star_expr))* [',']
 testlist: test (',' test)* [',']
 dictorsetmaker: ( ((test ':' test | '**' expr)
                    (comp_for | (',' (test ':' test | '**' expr))* [','])) |
                   ((test [':=' test] | star_expr)
                    (comp_for | (',' (test [':=' test] | star_expr))* [','])) )
@@ -151,15 +149,15 @@
             test '=' test |
             '**' test |
             '*' test )
 
 comp_iter: comp_for | comp_if
 sync_comp_for: 'for' exprlist 'in' or_test [comp_iter]
 comp_for: ['async'] sync_comp_for
-comp_if: 'if' test_nocond [comp_iter]
+comp_if: 'if' or_test [comp_iter]
 
 # not used in grammar, but may appear in "node" passed from Parser to Compiler
 encoding_decl: NAME
 
 yield_expr: 'yield' [yield_arg]
 yield_arg: 'from' test | testlist_star_expr
```

### Comparing `parso-0.8.2/parso/python/parser.py` & `parso-0.8.3/parso/python/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,14 @@
             if nonterminal == 'suite':
                 # We don't want the INDENT/DEDENT in our parser tree. Those
                 # leaves are just cancer. They are virtual leaves and not real
                 # ones and therefore have pseudo start/end positions and no
                 # prefixes. Just ignore them.
                 children = [children[0]] + children[2:-1]
             node = self.default_node(nonterminal, children)
-        for c in children:
-            c.parent = node
         return node
 
     def convert_leaf(self, type, value, prefix, start_pos):
         # print('leaf', repr(value), token.tok_name[type])
         if type == NAME:
             if value in self._pgen_grammar.reserved_syntax_strings:
                 return tree.Keyword(value, start_pos, prefix)
@@ -181,16 +179,14 @@
                 pass
 
     def _stack_removal(self, start_index):
         all_nodes = [node for stack_node in self.stack[start_index:] for node in stack_node.nodes]
 
         if all_nodes:
             node = tree.PythonErrorNode(all_nodes)
-            for n in all_nodes:
-                n.parent = node
             self.stack[start_index - 1].nodes.append(node)
 
         self.stack[start_index:] = []
         return bool(all_nodes)
 
     def _recovery_tokenize(self, tokens):
         for token in tokens:
```

### Comparing `parso-0.8.2/parso/python/pep8.py` & `parso-0.8.3/parso/python/pep8.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from contextlib import contextmanager
 from typing import Tuple
 
 from parso.python.errors import ErrorFinder, ErrorFinderConfig
 from parso.normalizer import Rule
-from parso.python.tree import search_ancestor, Flow, Scope
+from parso.python.tree import Flow, Scope
 
 
 _IMPORT_TYPES = ('import_name', 'import_from')
 _SUITE_INTRODUCERS = ('classdef', 'funcdef', 'if_stmt', 'while_stmt',
                       'for_stmt', 'try_stmt', 'with_stmt')
 _NON_STAR_TYPES = ('term', 'import_from', 'power')
 _OPENING_BRACKETS = '(', '[', '{'
@@ -70,15 +70,15 @@
             previous_leaf = previous_leaf.get_previous_leaf()
             if not isinstance(n, BracketNode) or previous_leaf != n.leaf:
                 break
             n = n.parent
         parent_indentation = n.indentation
 
         next_leaf = leaf.get_next_leaf()
-        if '\n' in next_leaf.prefix:
+        if '\n' in next_leaf.prefix or '\r' in next_leaf.prefix:
             # This implies code like:
             # foobarbaz(
             #     a,
             #     b,
             # )
             self.bracket_indentation = parent_indentation \
                 + config.closing_bracket_hanging_indentation
@@ -112,23 +112,23 @@
     annotations and dict values.
     """
     def __init__(self, config, leaf, parent):
         super().__init__(config, leaf, parent)
         self.type = IndentationTypes.IMPLICIT
 
         next_leaf = leaf.get_next_leaf()
-        if leaf == ':' and '\n' not in next_leaf.prefix:
+        if leaf == ':' and '\n' not in next_leaf.prefix and '\r' not in next_leaf.prefix:
             self.indentation += ' '
 
 
 class BackslashNode(IndentationNode):
     type = IndentationTypes.BACKSLASH
 
     def __init__(self, config, parent_indentation, containing_leaf, spacing, parent=None):
-        expr_stmt = search_ancestor(containing_leaf, 'expr_stmt')
+        expr_stmt = containing_leaf.search_ancestor('expr_stmt')
         if expr_stmt is not None:
             equals = expr_stmt.children[-2]
 
             if '\t' in config.indentation:
                 # TODO unite with the code of BracketNode
                 self.indentation = None
             else:
@@ -212,16 +212,16 @@
                         and atom.value == 'type':
                     self.add_issue(node, 721, "Do not compare types, use 'isinstance()")
                     break
         elif typ == 'file_input':
             endmarker = node.children[-1]
             prev = endmarker.get_previous_leaf()
             prefix = endmarker.prefix
-            if (not prefix.endswith('\n') and (
-                    prefix or prev is None or prev.value != '\n')):
+            if (not prefix.endswith('\n') and not prefix.endswith('\r') and (
+                    prefix or prev is None or prev.value not in {'\n', '\r\n', '\r'})):
                 self.add_issue(endmarker, 292, "No newline at end of file")
 
         if typ in _IMPORT_TYPES:
             simple_stmt = node.parent
             module = simple_stmt.parent
             if module.type == 'file_input':
                 index = module.children.index(simple_stmt)
@@ -461,15 +461,16 @@
                     else:
                         should_be_indentation = node.indentation
                     if self._in_suite_introducer and indentation == \
                             node.get_latest_suite_node().indentation \
                             + self._config.indentation:
                         self.add_issue(part, 129, "Line with same indent as next logical block")
                     elif indentation != should_be_indentation:
-                        if not self._check_tabs_spaces(spacing) and part.value != '\n':
+                        if not self._check_tabs_spaces(spacing) and part.value not in \
+                                {'\n', '\r\n', '\r'}:
                             if value in '])}':
                                 if node.type == IndentationTypes.VERTICAL_BRACKET:
                                     self.add_issue(
                                         part,
                                         124,
                                         "Closing bracket does not match visual indentation"
                                     )
@@ -648,15 +649,16 @@
                     message_225 = 'Missing whitespace between tokens'
                     add_not_spaces(spacing, 225, message_225)
             elif type_ == 'keyword' or prev.type == 'keyword':
                 add_not_spaces(spacing, 275, 'Missing whitespace around keyword')
             else:
                 prev_spacing = self._previous_spacing
                 if prev in _ALLOW_SPACE and spaces != prev_spacing.value \
-                        and '\n' not in self._previous_leaf.prefix:
+                        and '\n' not in self._previous_leaf.prefix \
+                        and '\r' not in self._previous_leaf.prefix:
                     message = "Whitespace before operator doesn't match with whitespace after"
                     self.add_issue(spacing, 229, message)
 
                 if spaces and part not in _ALLOW_SPACE and prev not in _ALLOW_SPACE:
                     message_225 = 'Missing whitespace between tokens'
                     # self.add_issue(spacing, 225, message_225)
                     # TODO why only brackets?
@@ -720,19 +722,19 @@
                 start_pos
         elif typ == 'endmarker':
             if self._newline_count >= 2:
                 self.add_issue(leaf, 391, 'Blank line at end of file')
 
     def add_issue(self, node, code, message):
         if self._previous_leaf is not None:
-            if search_ancestor(self._previous_leaf, 'error_node') is not None:
+            if self._previous_leaf.search_ancestor('error_node') is not None:
                 return
             if self._previous_leaf.type == 'error_leaf':
                 return
-        if search_ancestor(node, 'error_node') is not None:
+        if node.search_ancestor('error_node') is not None:
             return
         if code in (901, 903):
             # 901 and 903 are raised by the ErrorFinder.
             super().add_issue(node, code, message)
         else:
             # Skip ErrorFinder here, because it has custom behavior.
             super(ErrorFinder, self).add_issue(node, code, message)
```

### Comparing `parso-0.8.2/parso/python/prefix.py` & `parso-0.8.3/parso/python/prefix.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.type = typ
         self.value = value
         self.spacing = spacing
         self.start_pos: Tuple[int, int] = start_pos
 
     @property
     def end_pos(self) -> Tuple[int, int]:
-        if self.value.endswith('\n'):
+        if self.value.endswith('\n') or self.value.endswith('\r'):
             return self.start_pos[0] + 1, 0
         if self.value == unicode_bom:
             # The bom doesn't have a length at the start of a Python file.
             return self.start_pos
         return self.start_pos[0], self.start_pos[1] + len(self.value)
 
     def create_spacing_part(self):
@@ -36,18 +36,26 @@
         return '%s(%s, %s, %s)' % (
             self.__class__.__name__,
             self.type,
             repr(self.value),
             self.start_pos
         )
 
+    def search_ancestor(self, *node_types):
+        node = self.parent
+        while node is not None:
+            if node.type in node_types:
+                return node
+            node = node.parent
+        return None
+
 
 _comment = r'#[^\n\r\f]*'
-_backslash = r'\\\r?\n'
-_newline = r'\r?\n'
+_backslash = r'\\\r?\n|\\\r'
+_newline = r'\r?\n|\r'
 _form_feed = r'\f'
 _only_spacing = '$'
 _spacing = r'[ \t]*'
 _bom = unicode_bom
 
 _regex = group(
     _comment, _backslash, _newline, _form_feed, _only_spacing, _bom,
@@ -82,15 +90,15 @@
             leaf, type_, value, spacing,
             start_pos=(line, column + start - int(bom) + len(spacing))
         )
         if type_ == 'bom':
             bom = True
 
         start = match.end(0)
-        if value.endswith('\n'):
+        if value.endswith('\n') or value.endswith('\r'):
             line += 1
             column = -start
 
     if value:
         spacing = ''
     yield PrefixPart(
         leaf, 'spacing', spacing,
```

### Comparing `parso-0.8.2/parso/python/token.py` & `parso-0.8.3/parso/python/token.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/parso/python/tokenize.py` & `parso-0.8.3/parso/python/tokenize.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,15 +544,15 @@
 
                 if not new_line and paren_level == 0 and not fstring_stack:
                     yield PythonToken(NEWLINE, token, spos, prefix)
                 else:
                     additional_prefix = prefix + token
                 new_line = True
             elif initial == '#':  # Comments
-                assert not token.endswith("\n")
+                assert not token.endswith("\n") and not token.endswith("\r")
                 if fstring_stack and fstring_stack[-1].is_in_expr():
                     # `#` is not allowed in f-string expressions
                     yield PythonToken(ERRORTOKEN, initial, spos, prefix)
                     pos = start + 1
                 else:
                     additional_prefix = prefix + token
             elif token in triple_quoted:
```

### Comparing `parso-0.8.2/parso/python/tree.py` & `parso-0.8.3/parso/python/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,15 @@
 import re
 try:
     from collections.abc import Mapping
 except ImportError:
     from collections import Mapping
 from typing import Tuple
 
-from parso.tree import Node, BaseNode, Leaf, ErrorNode, ErrorLeaf, \
-    search_ancestor
+from parso.tree import Node, BaseNode, Leaf, ErrorNode, ErrorLeaf, search_ancestor  # noqa
 from parso.python.prefix import split_prefix
 from parso.utils import split_lines
 
 _FLOW_CONTAINERS = set(['if_stmt', 'while_stmt', 'for_stmt', 'try_stmt',
                         'with_stmt', 'async_stmt', 'suite'])
 _RETURN_STMT_CONTAINERS = set(['suite', 'simple_stmt']) | _FLOW_CONTAINERS
 
@@ -545,15 +544,19 @@
         4. annotation (if present)
     """
     type = 'funcdef'
 
     def __init__(self, children):
         super().__init__(children)
         parameters = self.children[2]  # After `def foo`
-        parameters.children[1:-1] = _create_params(parameters, parameters.children[1:-1])
+        parameters_children = parameters.children[1:-1]
+        # If input parameters list already has Param objects, keep it as is;
+        # otherwise, convert it to a list of Param objects.
+        if not any(isinstance(child, Param) for child in parameters_children):
+            parameters.children[1:-1] = _create_params(parameters, parameters_children)
 
     def _get_param_nodes(self):
         return self.children[2].children
 
     def get_params(self):
         """
         Returns a list of `Param()`.
@@ -648,15 +651,19 @@
     type = 'lambdef'
     __slots__ = ()
 
     def __init__(self, children):
         # We don't want to call the Function constructor, call its parent.
         super(Function, self).__init__(children)
         # Everything between `lambda` and the `:` operator is a parameter.
-        self.children[1:-2] = _create_params(self, self.children[1:-2])
+        parameters_children = self.children[1:-2]
+        # If input children list already has Param objects, keep it as is;
+        # otherwise, convert it to a list of Param objects.
+        if not any(isinstance(child, Param) for child in parameters_children):
+            self.children[1:-2] = _create_params(self, parameters_children)
 
     @property
     def name(self):
         """
         Raises an AttributeError. Lambdas don't have a defined name.
         """
         raise AttributeError("lambda is not named.")
@@ -772,15 +779,15 @@
         for with_item in self.children[1:-2:2]:
             # Check with items for 'as' names.
             if with_item.type == 'with_item':
                 names += _defined_names(with_item.children[2], include_setitem)
         return names
 
     def get_test_node_from_name(self, name):
-        node = search_ancestor(name, "with_item")
+        node = name.search_ancestor("with_item")
         if node is None:
             raise ValueError('The name is not actually part of a with statement.')
         return node.children[0]
 
 
 class Import(PythonBaseNode):
     __slots__ = ()
@@ -1076,19 +1083,17 @@
     """
     It's a helper class that makes business logic with params much easier. The
     Python grammar defines no ``param`` node. It defines it in a different way
     that is not really suited to working with parameters.
     """
     type = 'param'
 
-    def __init__(self, children, parent):
+    def __init__(self, children, parent=None):
         super().__init__(children)
         self.parent = parent
-        for child in children:
-            child.parent = self
 
     @property
     def star_count(self):
         """
         Is `0` in case of `foo`, `1` in case of `*foo` or `2` in case of
         `**foo`.
         """
@@ -1167,15 +1172,15 @@
             pass
         return index - 1
 
     def get_parent_function(self):
         """
         Returns the function/lambda of a parameter.
         """
-        return search_ancestor(self, 'funcdef', 'lambdef')
+        return self.search_ancestor('funcdef', 'lambdef')
 
     def get_code(self, include_prefix=True, include_comma=True):
         """
         Like all the other get_code functions, but includes the param
         `include_comma`.
 
         :param include_comma bool: If enabled includes the comma in the string output.
```

### Comparing `parso-0.8.2/parso/tree.py` & `parso-0.8.3/parso/tree.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 from abc import abstractmethod, abstractproperty
-from typing import List, Optional, Tuple
+from typing import List, Optional, Tuple, Union
 
 from parso.utils import split_lines
 
 
-def search_ancestor(node, *node_types):
+def search_ancestor(node: 'NodeOrLeaf', *node_types: str) -> 'Optional[BaseNode]':
     """
     Recursively looks at the parents of a node and returns the first found node
-    that matches node_types. Returns ``None`` if no matching node is found.
+    that matches ``node_types``. Returns ``None`` if no matching node is found.
+
+    This function is deprecated, use :meth:`NodeOrLeaf.search_ancestor` instead.
 
     :param node: The ancestors of this node will be checked.
     :param node_types: type names that are searched for.
-    :type node_types: tuple of str
     """
-    while True:
-        node = node.parent
-        if node is None or node.type in node_types:
-            return node
+    n = node.parent
+    while n is not None:
+        if n.type in node_types:
+            return n
+        n = n.parent
+    return None
 
 
 class NodeOrLeaf:
     """
     The base class for nodes and leaves.
     """
-    __slots__ = ()
+    __slots__ = ('parent',)
     type: str
     '''
     The type is a string that typically matches the types of the grammar file.
     '''
+    parent: 'Optional[BaseNode]'
+    '''
+    The parent :class:`BaseNode` of this node or leaf.
+    None if this is the root node.
+    '''
 
     def get_root_node(self):
         """
         Returns the root node of a parser tree. The returned node doesn't have
         a parent node like all the other nodes/leaves.
         """
         scope = self
@@ -169,21 +177,125 @@
         """
         Returns the code that was the input for the parser for this node.
 
         :param include_prefix: Removes the prefix (whitespace and comments) of
             e.g. a statement.
         """
 
+    def search_ancestor(self, *node_types: str) -> 'Optional[BaseNode]':
+        """
+        Recursively looks at the parents of this node or leaf and returns the
+        first found node that matches ``node_types``. Returns ``None`` if no
+        matching node is found.
+
+        :param node_types: type names that are searched for.
+        """
+        node = self.parent
+        while node is not None:
+            if node.type in node_types:
+                return node
+            node = node.parent
+        return None
+
+    def dump(self, *, indent: Optional[Union[int, str]] = 4) -> str:
+        """
+        Returns a formatted dump of the parser tree rooted at this node or leaf. This is
+        mainly useful for debugging purposes.
+
+        The ``indent`` parameter is interpreted in a similar way as :py:func:`ast.dump`.
+        If ``indent`` is a non-negative integer or string, then the tree will be
+        pretty-printed with that indent level. An indent level of 0, negative, or ``""``
+        will only insert newlines. ``None`` selects the single line representation.
+        Using a positive integer indent indents that many spaces per level. If
+        ``indent`` is a string (such as ``"\\t"``), that string is used to indent each
+        level.
+
+        :param indent: Indentation style as described above. The default indentation is
+            4 spaces, which yields a pretty-printed dump.
+
+        >>> import parso
+        >>> print(parso.parse("lambda x, y: x + y").dump())
+        Module([
+            Lambda([
+                Keyword('lambda', (1, 0)),
+                Param([
+                    Name('x', (1, 7), prefix=' '),
+                    Operator(',', (1, 8)),
+                ]),
+                Param([
+                    Name('y', (1, 10), prefix=' '),
+                ]),
+                Operator(':', (1, 11)),
+                PythonNode('arith_expr', [
+                    Name('x', (1, 13), prefix=' '),
+                    Operator('+', (1, 15), prefix=' '),
+                    Name('y', (1, 17), prefix=' '),
+                ]),
+            ]),
+            EndMarker('', (1, 18)),
+        ])
+        """
+        if indent is None:
+            newline = False
+            indent_string = ''
+        elif isinstance(indent, int):
+            newline = True
+            indent_string = ' ' * indent
+        elif isinstance(indent, str):
+            newline = True
+            indent_string = indent
+        else:
+            raise TypeError(f"expect 'indent' to be int, str or None, got {indent!r}")
+
+        def _format_dump(node: NodeOrLeaf, indent: str = '', top_level: bool = True) -> str:
+            result = ''
+            node_type = type(node).__name__
+            if isinstance(node, Leaf):
+                result += f'{indent}{node_type}('
+                if isinstance(node, ErrorLeaf):
+                    result += f'{node.token_type!r}, '
+                elif isinstance(node, TypedLeaf):
+                    result += f'{node.type!r}, '
+                result += f'{node.value!r}, {node.start_pos!r}'
+                if node.prefix:
+                    result += f', prefix={node.prefix!r}'
+                result += ')'
+            elif isinstance(node, BaseNode):
+                result += f'{indent}{node_type}('
+                if isinstance(node, Node):
+                    result += f'{node.type!r}, '
+                result += '['
+                if newline:
+                    result += '\n'
+                for child in node.children:
+                    result += _format_dump(child, indent=indent + indent_string, top_level=False)
+                result += f'{indent}])'
+            else:  # pragma: no cover
+                # We shouldn't ever reach here, unless:
+                # - `NodeOrLeaf` is incorrectly subclassed else where
+                # - or a node's children list contains invalid nodes or leafs
+                # Both are unexpected internal errors.
+                raise TypeError(f'unsupported node encountered: {node!r}')
+            if not top_level:
+                if newline:
+                    result += ',\n'
+                else:
+                    result += ', '
+            return result
+
+        return _format_dump(self)
+
 
 class Leaf(NodeOrLeaf):
     '''
     Leafs are basically tokens with a better API. Leafs exactly know where they
     were defined and what text preceeds them.
     '''
-    __slots__ = ('value', 'parent', 'line', 'column', 'prefix')
+    __slots__ = ('value', 'line', 'column', 'prefix')
+    prefix: str
 
     def __init__(self, value: str, start_pos: Tuple[int, int], prefix: str = '') -> None:
         self.value = value
         '''
         :py:func:`str` The value of the current token.
         '''
         self.start_pos = start_pos
@@ -253,26 +365,28 @@
 
 
 class BaseNode(NodeOrLeaf):
     """
     The super class for all nodes.
     A node has children, a type and possibly a parent node.
     """
-    __slots__ = ('children', 'parent')
+    __slots__ = ('children',)
 
     def __init__(self, children: List[NodeOrLeaf]) -> None:
         self.children = children
         """
         A list of :class:`NodeOrLeaf` child nodes.
         """
         self.parent: Optional[BaseNode] = None
         '''
-        The parent :class:`BaseNode` of this leaf.
+        The parent :class:`BaseNode` of this node.
         None if this is the root node.
         '''
+        for child in children:
+            child.parent = self
 
     @property
     def start_pos(self) -> Tuple[int, int]:
         return self.children[0].start_pos
 
     def get_start_pos_of_prefix(self):
         return self.children[0].get_start_pos_of_prefix()
```

### Comparing `parso-0.8.2/parso/utils.py` & `parso-0.8.3/parso/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         - http://docs.python.org/2/reference/lexical_analysis.html#encoding-declarations
         """
         byte_mark = literal_eval(r"b'\xef\xbb\xbf'")
         if source.startswith(byte_mark):
             # UTF-8 byte-order mark
             return 'utf-8'
 
-        first_two_lines = re.match(br'(?:[^\n]*\n){0,2}', source).group(0)
+        first_two_lines = re.match(br'(?:[^\r\n]*(?:\r\n|\r|\n)){0,2}', source).group(0)
         possible_encoding = re.search(br"coding[=:]\s*([-\w.]+)",
                                       first_two_lines)
         if possible_encoding:
             e = possible_encoding.group(1)
             if not isinstance(e, str):
                 e = str(e, 'ascii', 'replace')
             return e
```

### Comparing `parso-0.8.2/parso.egg-info/PKG-INFO` & `parso-0.8.3/parso.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: parso
-Version: 0.8.2
+Version: 0.8.3
 Summary: A Python Parser
 Home-page: https://github.com/davidhalter/parso
 Author: David Halter
 Author-email: davidhalter88@gmail.com
 Maintainer: David Halter
 Maintainer-email: davidhalter88@gmail.com
 License: MIT
 Description: ###################################################################
         parso - A Python Parser
         ###################################################################
         
         
-        .. image:: https://travis-ci.org/davidhalter/parso.svg?branch=master
-            :target: https://travis-ci.org/davidhalter/parso
-            :alt: Travis CI build status
+        .. image:: https://github.com/davidhalter/parso/workflows/Build/badge.svg?branch=master
+            :target: https://github.com/davidhalter/parso/actions
+            :alt: GitHub Actions build status
         
         .. image:: https://coveralls.io/repos/github/davidhalter/parso/badge.svg?branch=master
             :target: https://coveralls.io/github/davidhalter/parso?branch=master
             :alt: Coverage Status
         
         .. image:: https://pepy.tech/badge/parso
             :target: https://pepy.tech/project/parso
@@ -109,14 +109,19 @@
         
         Changelog
         ---------
         
         Unreleased
         ++++++++++
         
+        0.8.3 (2021-11-30)
+        ++++++++++++++++++
+        
+        - Add basic support for Python 3.11 and 3.12
+        
         0.8.2 (2021-03-30)
         ++++++++++++++++++
         
         - Various small bugfixes
         
         0.8.1 (2020-12-10)
         ++++++++++++++++++
```

### Comparing `parso-0.8.2/parso.egg-info/SOURCES.txt` & `parso-0.8.3/parso.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 parso/pgen2/__init__.py
 parso/pgen2/generator.py
 parso/pgen2/grammar_parser.py
 parso/python/__init__.py
 parso/python/diff.py
 parso/python/errors.py
 parso/python/grammar310.txt
+parso/python/grammar311.txt
+parso/python/grammar312.txt
 parso/python/grammar36.txt
 parso/python/grammar37.txt
 parso/python/grammar38.txt
 parso/python/grammar39.txt
 parso/python/parser.py
 parso/python/pep8.py
 parso/python/prefix.py
@@ -60,14 +62,15 @@
 parso/python/tokenize.py
 parso/python/tree.py
 test/__init__.py
 test/failing_examples.py
 test/fuzz_diff_parser.py
 test/test_cache.py
 test/test_diff_parser.py
+test/test_dump_tree.py
 test/test_error_recovery.py
 test/test_file_python_errors.py
 test/test_fstring.py
 test/test_get_code.py
 test/test_grammar.py
 test/test_load_grammar.py
 test/test_normalizer_issues_files.py
```

### Comparing `parso-0.8.2/setup.py` & `parso-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/failing_examples.py` & `parso-0.8.3/test/failing_examples.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/fuzz_diff_parser.py` & `parso-0.8.3/test/fuzz_diff_parser.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E10.py` & `parso-0.8.3/test/normalizer_issue_files/E10.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E101.py` & `parso-0.8.3/test/normalizer_issue_files/E101.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E11.py` & `parso-0.8.3/test/normalizer_issue_files/E11.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E12_first.py` & `parso-0.8.3/test/normalizer_issue_files/E12_first.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E12_not_first.py` & `parso-0.8.3/test/normalizer_issue_files/E12_not_first.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E12_not_second.py` & `parso-0.8.3/test/normalizer_issue_files/E12_not_second.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E12_second.py` & `parso-0.8.3/test/normalizer_issue_files/E12_second.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E12_third.py` & `parso-0.8.3/test/normalizer_issue_files/E12_third.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E20.py` & `parso-0.8.3/test/normalizer_issue_files/E20.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E22.py` & `parso-0.8.3/test/normalizer_issue_files/E22.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E25.py` & `parso-0.8.3/test/normalizer_issue_files/E25.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E26.py` & `parso-0.8.3/test/normalizer_issue_files/E26.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E27.py` & `parso-0.8.3/test/normalizer_issue_files/E27.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E30.py` & `parso-0.8.3/test/normalizer_issue_files/E30.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E30not.py` & `parso-0.8.3/test/normalizer_issue_files/E30not.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E40.py` & `parso-0.8.3/test/normalizer_issue_files/E40.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E50.py` & `parso-0.8.3/test/normalizer_issue_files/E50.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E71.py` & `parso-0.8.3/test/normalizer_issue_files/E71.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/E72.py` & `parso-0.8.3/test/normalizer_issue_files/E72.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/LICENSE` & `parso-0.8.3/test/normalizer_issue_files/LICENSE`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/allowed_syntax.py` & `parso-0.8.3/test/normalizer_issue_files/allowed_syntax.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/python.py` & `parso-0.8.3/test/normalizer_issue_files/python.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/normalizer_issue_files/utf-8.py` & `parso-0.8.3/test/normalizer_issue_files/utf-8.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/test_cache.py` & `parso-0.8.3/test/test_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 @pytest.mark.parametrize('use_file_io', [False, True])
 def test_cache_last_used_update(diff_cache, use_file_io):
     p = Path('/path/last-used')
     parser_cache.clear()  # Clear, because then it's easier to find stuff.
     parse('somecode', cache=True, path=p)
     node_cache_item = next(iter(parser_cache.values()))[p]
     now = time.time()
-    assert node_cache_item.last_used < now
+    assert node_cache_item.last_used <= now
 
     if use_file_io:
         f = _FixedTimeFileIO(p, 'code', node_cache_item.last_used - 10)
         parse(file_io=f, cache=True, diff_cache=diff_cache)
     else:
         parse('somecode2', cache=True, path=p, diff_cache=diff_cache)
 
@@ -181,10 +181,13 @@
         nonlocal was_called
         was_called = True
         raise PermissionError
 
     was_called = False
 
     monkeypatch.setattr(cache, '_save_to_file_system', save)
-    with pytest.warns(Warning):
-        parse(path=__file__, cache=True, diff_cache=True)
-    assert was_called
+    try:
+        with pytest.warns(Warning):
+            parse(path=__file__, cache=True, diff_cache=True)
+        assert was_called
+    finally:
+        parser_cache.clear()
```

### Comparing `parso-0.8.2/test/test_diff_parser.py` & `parso-0.8.3/test/test_diff_parser.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/test_error_recovery.py` & `parso-0.8.3/test/test_error_recovery.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/test_file_python_errors.py` & `parso-0.8.3/test/test_file_python_errors.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/test_fstring.py` & `parso-0.8.3/test/test_fstring.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/test_get_code.py` & `parso-0.8.3/test/test_get_code.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/test_load_grammar.py` & `parso-0.8.3/test/test_load_grammar.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/test_normalizer_issues_files.py` & `parso-0.8.3/test/test_normalizer_issues_files.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/test_old_fast_parser.py` & `parso-0.8.3/test/test_old_fast_parser.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/test_param_splitting.py` & `parso-0.8.3/test/test_param_splitting.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/test_parser.py` & `parso-0.8.3/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/test_parser_tree.py` & `parso-0.8.3/test/test_parser_tree.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from textwrap import dedent
 
 import pytest
 
 from parso import parse
 from parso.python import tree
+from parso.tree import search_ancestor
 
 
 class TestsFunctionAndLambdaParsing:
 
     FIXTURES = [
         ('def my_function(x, y, z) -> str:\n    return x + y * z\n', {
             'name': 'my_function',
@@ -235,7 +236,31 @@
     code = "with A as X.Y, B as (Z), C as Q[0], D as Q['foo']: pass"
     with_stmt = parse(code, version='3').children[0]
     tests = [
         with_stmt.get_test_node_from_name(name).value
         for name in with_stmt.get_defined_names(include_setitem=True)
     ]
     assert tests == ["A", "B", "C", "D"]
+
+
+sample_module = parse('x + y')
+sample_node = sample_module.children[0]
+sample_leaf = sample_node.children[0]
+
+
+@pytest.mark.parametrize(
+    'node,node_types,expected_ancestor', [
+        (sample_module, ('file_input',), None),
+        (sample_node, ('arith_expr',), None),
+        (sample_node, ('file_input', 'eval_input'), sample_module),
+        (sample_leaf, ('name',), None),
+        (sample_leaf, ('arith_expr',), sample_node),
+        (sample_leaf, ('file_input',), sample_module),
+        (sample_leaf, ('file_input', 'arith_expr'), sample_node),
+        (sample_leaf, ('shift_expr',), None),
+        (sample_leaf, ('name', 'shift_expr',), None),
+        (sample_leaf, (), None),
+    ]
+)
+def test_search_ancestor(node, node_types, expected_ancestor):
+    assert node.search_ancestor(*node_types) is expected_ancestor
+    assert search_ancestor(node, *node_types) is expected_ancestor  # deprecated
```

### Comparing `parso-0.8.2/test/test_pep8.py` & `parso-0.8.3/test/test_pep8.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     def assert_issue(code):
         found = issues(code)
         assert len(found) == 1
         issue, = found
         assert issue.code == 292
 
     assert not issues('asdf = 1\n')
+    assert not issues('asdf = 1\r\n')
+    assert not issues('asdf = 1\r')
     assert_issue('asdf = 1')
     assert_issue('asdf = 1\n# foo')
     assert_issue('# foobar')
     assert_issue('')
     assert_issue('foo = 1  # comment')
```

### Comparing `parso-0.8.2/test/test_pgen2.py` & `parso-0.8.3/test/test_pgen2.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,15 @@
     with pytest.raises(ValueError, match='left recursion'):
         generate_grammar('foo: foo NAME\n', tokenize.PythonTokenTypes)
 
 
 @pytest.mark.parametrize(
     'grammar, error_match', [
         ['foo: bar | baz\nbar: NAME\nbaz: NAME\n',
-         r"foo is ambiguous.*given a PythonTokenTypes\.NAME.*bar or baz"],
+         r"foo is ambiguous.*given a (PythonTokenTypes\.)?NAME.*bar or baz"],
         ['''foo: bar | baz\nbar: 'x'\nbaz: "x"\n''',
          r"foo is ambiguous.*given a ReservedString\(x\).*bar or baz"],
         ['''foo: bar | 'x'\nbar: 'x'\n''',
          r"foo is ambiguous.*given a ReservedString\(x\).*bar or foo"],
         # An ambiguity with the second (not the first) child of a production
         ['outer: "a" [inner] "b" "c"\ninner: "b" "c" [inner]\n',
          r"outer is ambiguous.*given a ReservedString\(b\).*inner or outer"],
```

### Comparing `parso-0.8.2/test/test_prefix.py` & `parso-0.8.3/test/test_prefix.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     (' # \n', ['# ', '\n', '']),
     (' # \f\n', ['# ', '\f', '\n', '']),
     ('  \n', ['\n', '']),
     ('  \n ', ['\n', ' ']),
     (' \f ', ['\f', ' ']),
     (' \f ', ['\f', ' ']),
     (' \r\n', ['\r\n', '']),
+    (' \r', ['\r', '']),
     ('\\\n', ['\\\n', '']),
     ('\\\r\n', ['\\\r\n', '']),
     ('\t\t\n\t', ['\n', '\t']),
 ])
 def test_simple_prefix_splitting(string, tokens):
     tree = parso.parse(string)
     leaf = tree.children[0]
@@ -30,15 +31,15 @@
 
     parsed_tokens = list(leaf._split_prefix())
     start_pos = (1, 0)
     for pt, expected in zip_longest(parsed_tokens, tokens):
         assert pt.value == expected
 
         # Calculate the estimated end_pos
-        if expected.endswith('\n'):
+        if expected.endswith('\n') or expected.endswith('\r'):
             end_pos = start_pos[0] + 1, 0
         else:
             end_pos = start_pos[0], start_pos[1] + len(expected) + len(pt.spacing)
 
         # assert start_pos == pt.start_pos
         assert end_pos == pt.end_pos
         start_pos = end_pos
```

### Comparing `parso-0.8.2/test/test_python_errors.py` & `parso-0.8.3/test/test_python_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,18 +53,18 @@
     wanted, line_nr = _get_actual_exception(code)
 
     errors = _get_error_list(code)
     if errors:
         error, = errors
         actual = error.message
     assert actual in wanted
-    if sys.version_info[:2] < (3, 8):
+    if sys.version_info[:2] not in ((3, 8), (3, 9)):
         assert line_nr == error.start_pos[0]
     else:
-        assert line_nr == 0  # For whatever reason this is zero in Python 3.8+
+        assert line_nr == 0  # For whatever reason this is zero in Python 3.8/3.9
 
 
 @pytest.mark.parametrize(
     ('code', 'positions'), [
         ('1 +', [(1, 3)]),
         ('1 +\n', [(1, 3)]),
         ('1 +\n2 +', [(1, 3), (2, 3)]),
@@ -136,21 +136,24 @@
         wanted = 'SyntaxError: invalid syntax'
     elif wanted == "SyntaxError: f-string: single '}' is not allowed":
         wanted = 'SyntaxError: invalid syntax'
     return [wanted], line_nr
 
 
 def test_default_except_error_postition():
-    # For this error the position seemed to be one line off, but that doesn't
-    # really matter.
+    # For this error the position seemed to be one line off in Python < 3.10,
+    # but that doesn't really matter.
     code = 'try: pass\nexcept: pass\nexcept X: pass'
     wanted, line_nr = _get_actual_exception(code)
     error, = _get_error_list(code)
     assert error.message in wanted
-    assert line_nr != error.start_pos[0]
+    if sys.version_info[:2] >= (3, 10):
+        assert line_nr == error.start_pos[0]
+    else:
+        assert line_nr != error.start_pos[0]
     # I think this is the better position.
     assert error.start_pos[0] == 2
 
 
 def test_statically_nested_blocks():
     def build(code, depth):
         if depth == 0:
@@ -490,7 +493,18 @@
         'del f(x)[y::]',
         'del x[[*y]]',
         'del x[[*y]::]',
     ]
 )
 def test_valid_del(code):
     assert not _get_error_list(code)
+
+
+@pytest.mark.parametrize(
+    ('source', 'version', 'no_errors'), [
+        ('[x for x in range(10) if lambda: 1]', '3.8', True),
+        ('[x for x in range(10) if lambda: 1]', '3.9', False),
+        ('[x for x in range(10) if (lambda: 1)]', '3.9', True),
+    ]
+)
+def test_lambda_in_comp_if(source, version, no_errors):
+    assert bool(_get_error_list(source, version=version)) ^ no_errors
```

### Comparing `parso-0.8.2/test/test_tokenize.py` & `parso-0.8.3/test/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `parso-0.8.2/test/test_utils.py` & `parso-0.8.3/test/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,14 +70,18 @@
     assert unicode_bom == expr_stmt.get_first_leaf().prefix
 
 
 @pytest.mark.parametrize(
     ('code', 'errors'), [
         (b'# coding: wtf-12\nfoo', 'strict'),
         (b'# coding: wtf-12\nfoo', 'replace'),
+        (b'# coding: wtf-12\r\nfoo', 'strict'),
+        (b'# coding: wtf-12\r\nfoo', 'replace'),
+        (b'# coding: wtf-12\rfoo', 'strict'),
+        (b'# coding: wtf-12\rfoo', 'replace'),
     ]
 )
 def test_bytes_to_unicode_failing_encoding(code, errors):
     if errors == 'strict':
         with pytest.raises(LookupError):
             python_bytes_to_unicode(code, errors=errors)
     else:
```

