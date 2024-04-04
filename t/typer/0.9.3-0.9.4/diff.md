# Comparing `tmp/typer-0.9.3.tar.gz` & `tmp/typer-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer-0.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "typer-0.9.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `typer-0.9.3.tar` & `typer-0.9.4.tar`

### file list

```diff
@@ -1,649 +1,649 @@
--rw-r--r--   0        0        0      310 2024-03-23 17:03:25.226094 typer-0.9.3/.coveragerc
--rw-r--r--   0        0        0     5303 2024-03-23 17:03:25.226094 typer-0.9.3/.github/DISCUSSION_TEMPLATE/questions.yml
--rw-r--r--   0        0        0       19 2024-03-23 17:03:25.226094 typer-0.9.3/.github/FUNDING.yml
--rw-r--r--   0        0        0      758 2024-03-23 17:03:25.226094 typer-0.9.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      885 2024-03-23 17:03:25.226094 typer-0.9.3/.github/ISSUE_TEMPLATE/privileged.yml
--rw-r--r--   0        0        0      115 2024-03-23 17:03:25.226094 typer-0.9.3/.github/actions/comment-docs-preview-in-pr/Dockerfile
--rw-r--r--   0        0        0      394 2024-03-23 17:03:25.226094 typer-0.9.3/.github/actions/comment-docs-preview-in-pr/action.yml
--rw-r--r--   0        0        0     2074 2024-03-23 17:03:25.226094 typer-0.9.3/.github/actions/comment-docs-preview-in-pr/app/main.py
--rw-r--r--   0        0        0      309 2024-03-23 17:03:25.226094 typer-0.9.3/.github/dependabot.yml
--rw-r--r--   0        0        0     3029 2024-03-23 17:03:25.226094 typer-0.9.3/.github/workflows/build-docs.yml
--rw-r--r--   0        0        0     1630 2024-03-23 17:03:25.226094 typer-0.9.3/.github/workflows/deploy-docs.yml
--rw-r--r--   0        0        0      576 2024-03-23 17:03:25.226094 typer-0.9.3/.github/workflows/issue-manager.yml
--rw-r--r--   0        0        0     1256 2024-03-23 17:03:25.226094 typer-0.9.3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0      567 2024-03-23 17:03:25.226094 typer-0.9.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      957 2024-03-23 17:03:25.226094 typer-0.9.3/.github/workflows/smokeshow.yml
--rw-r--r--   0        0        0     2266 2024-03-23 17:03:25.226094 typer-0.9.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      117 2024-03-23 17:03:25.226094 typer-0.9.3/.gitignore
--rw-r--r--   0        0        0     1525 2024-03-23 17:03:25.230094 typer-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      568 2024-03-23 17:03:25.230094 typer-0.9.3/CITATION.cff
--rw-r--r--   0        0        0      125 2024-03-23 17:03:25.230094 typer-0.9.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1086 2024-03-23 17:03:25.230094 typer-0.9.3/LICENSE
--rw-r--r--   0        0        0    11885 2024-03-23 17:03:25.230094 typer-0.9.3/README.md
--rw-r--r--   0        0        0     1160 2024-03-23 17:03:25.230094 typer-0.9.3/SECURITY.md
--rw-r--r--   0        0        0     4876 2024-03-23 17:03:25.230094 typer-0.9.3/docs/alternatives.md
--rw-r--r--   0        0        0     5980 2024-03-23 17:03:25.230094 typer-0.9.3/docs/contributing.md
--rw-r--r--   0        0        0      451 2024-03-23 17:03:25.230094 typer-0.9.3/docs/css/custom.css
--rw-r--r--   0        0        0     2214 2024-03-23 17:03:25.230094 typer-0.9.3/docs/css/termynal.css
--rw-r--r--   0        0        0     4434 2024-03-23 17:03:25.230094 typer-0.9.3/docs/features.md
--rw-r--r--   0        0        0    12075 2024-03-23 17:03:25.230094 typer-0.9.3/docs/help-typer.md
--rwxr-xr-x   0        0        0      439 2024-03-23 17:03:25.230094 typer-0.9.3/docs/img/favicon.png
--rw-r--r--   0        0        0    48377 2024-03-23 17:03:25.230094 typer-0.9.3/docs/img/github-social-preview.png
--rw-r--r--   0        0        0     3936 2024-03-23 17:03:25.230094 typer-0.9.3/docs/img/github-social-preview.svg
--rw-r--r--   0        0        0      284 2024-03-23 17:03:25.230094 typer-0.9.3/docs/img/icon-black.svg
--rw-r--r--   0        0        0     1743 2024-03-23 17:03:25.230094 typer-0.9.3/docs/img/icon-white.svg
--rw-r--r--   0        0        0     6768 2024-03-23 17:03:25.230094 typer-0.9.3/docs/img/logo-margin/logo-margin-vector.svg
--rw-r--r--   0        0        0     3010 2024-03-23 17:03:25.230094 typer-0.9.3/docs/img/logo-margin/logo-margin.svg
--rw-r--r--   0        0        0    13924 2024-03-23 17:03:25.230094 typer-0.9.3/docs/img/pycharm-completion.png
--rw-r--r--   0        0        0    22753 2024-03-23 17:03:25.230094 typer-0.9.3/docs/img/vscode-completion.png
--rw-r--r--   0        0        0    11885 2024-03-23 17:03:25.230094 typer-0.9.3/docs/index.md
--rw-r--r--   0        0        0     3897 2024-03-23 17:03:25.230094 typer-0.9.3/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2024-03-23 17:03:25.230094 typer-0.9.3/docs/js/termynal.js
--rw-r--r--   0        0        0       26 2024-03-23 17:03:25.230094 typer-0.9.3/docs/overrides/main.html
--rw-r--r--   0        0        0    36538 2024-03-23 17:03:25.230094 typer-0.9.3/docs/release-notes.md
--rw-r--r--   0        0        0     1445 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/app-dir.md
--rw-r--r--   0        0        0     2698 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/arguments/default.md
--rw-r--r--   0        0        0     3287 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/arguments/envvar.md
--rw-r--r--   0        0        0    11973 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/arguments/help.md
--rw-r--r--   0        0        0      173 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/arguments/index.md
--rw-r--r--   0        0        0     6809 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/arguments/optional.md
--rw-r--r--   0        0        0      163 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/arguments/other-uses.md
--rw-r--r--   0        0        0     1084 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/commands/arguments.md
--rw-r--r--   0        0        0     4837 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/commands/callback.md
--rw-r--r--   0        0        0     3551 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/commands/context.md
--rw-r--r--   0        0        0    34041 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/commands/help.md
--rw-r--r--   0        0        0     8202 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/commands/index.md
--rw-r--r--   0        0        0     1380 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/commands/name.md
--rw-r--r--   0        0        0     3454 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/commands/one-or-multiple.md
--rw-r--r--   0        0        0     2293 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/commands/options.md
--rw-r--r--   0        0        0    24658 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/exceptions.md
--rw-r--r--   0        0        0    22035 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     2367 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/index.md
--rw-r--r--   0        0        0      974 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/launch.md
--rw-r--r--   0        0        0     1969 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/multiple-values/arguments-with-multiple-values.md
--rw-r--r--   0        0        0      133 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/multiple-values/index.md
--rw-r--r--   0        0        0     1728 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/multiple-values/multiple-options.md
--rw-r--r--   0        0        0     2386 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/multiple-values/options-with-multiple-values.md
--rw-r--r--   0        0        0    14803 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/options-autocompletion.md
--rw-r--r--   0        0        0     8041 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/options/callback-and-context.md
--rw-r--r--   0        0        0     7673 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/options/help.md
--rw-r--r--   0        0        0      202 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/options/index.md
--rw-r--r--   0        0        0     9245 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/options/name.md
--rw-r--r--   0        0        0     1754 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/options/password.md
--rw-r--r--   0        0        0     2579 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/options/prompt.md
--rw-r--r--   0        0        0     2190 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/options/required.md
--rw-r--r--   0        0        0     3980 2024-03-23 17:03:25.230094 typer-0.9.3/docs/tutorial/options/version.md
--rw-r--r--   0        0        0    20799 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/package.md
--rw-r--r--   0        0        0     4288 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/parameter-types/bool.md
--rw-r--r--   0        0        0     1694 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/parameter-types/custom-types.md
--rw-r--r--   0        0        0     2490 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/parameter-types/datetime.md
--rw-r--r--   0        0        0     3108 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/parameter-types/enum.md
--rw-r--r--   0        0        0     8645 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/parameter-types/file.md
--rw-r--r--   0        0        0     2016 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/parameter-types/index.md
--rw-r--r--   0        0        0     3782 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/parameter-types/number.md
--rw-r--r--   0        0        0     3861 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/parameter-types/path.md
--rw-r--r--   0        0        0     1739 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/parameter-types/uuid.md
--rw-r--r--   0        0        0    10363 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/printing.md
--rw-r--r--   0        0        0     6259 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/progressbar.md
--rw-r--r--   0        0        0     1909 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/prompt.md
--rw-r--r--   0        0        0     3795 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/subcommands/add-typer.md
--rw-r--r--   0        0        0     2984 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/subcommands/callback-override.md
--rw-r--r--   0        0        0     1201 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/subcommands/index.md
--rw-r--r--   0        0        0    12517 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/subcommands/name-and-help.md
--rw-r--r--   0        0        0     6077 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/subcommands/nested-subcommands.md
--rw-r--r--   0        0        0     2729 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/subcommands/single-file.md
--rw-r--r--   0        0        0     3013 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/terminating.md
--rw-r--r--   0        0        0     6367 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/testing.md
--rw-r--r--   0        0        0     6469 2024-03-23 17:03:25.234094 typer-0.9.3/docs/tutorial/using-click.md
--rw-r--r--   0        0        0     9703 2024-03-23 17:03:25.234094 typer-0.9.3/docs/typer-cli.md
--rw-r--r--   0        0        0      310 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/app_dir/tutorial001.py
--rw-r--r--   0        0        0      144 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/default/tutorial001.py
--rw-r--r--   0        0        0      197 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/default/tutorial001_an.py
--rw-r--r--   0        0        0      252 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/default/tutorial002.py
--rw-r--r--   0        0        0      302 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/default/tutorial002_an.py
--rw-r--r--   0        0        0      165 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/envvar/tutorial001.py
--rw-r--r--   0        0        0      216 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/envvar/tutorial001_an.py
--rw-r--r--   0        0        0      179 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/envvar/tutorial002.py
--rw-r--r--   0        0        0      236 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/envvar/tutorial002_an.py
--rw-r--r--   0        0        0      184 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/envvar/tutorial003.py
--rw-r--r--   0        0        0      255 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/envvar/tutorial003_an.py
--rw-r--r--   0        0        0      172 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial001.py
--rw-r--r--   0        0        0      217 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial001_an.py
--rw-r--r--   0        0        0      231 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial002.py
--rw-r--r--   0        0        0      276 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial002_an.py
--rw-r--r--   0        0        0      218 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial003.py
--rw-r--r--   0        0        0      269 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial003_an.py
--rw-r--r--   0        0        0      238 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial004.py
--rw-r--r--   0        0        0      309 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial004_an.py
--rw-r--r--   0        0        0      231 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial005.py
--rw-r--r--   0        0        0      313 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial005_an.py
--rw-r--r--   0        0        0      164 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial006.py
--rw-r--r--   0        0        0      215 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial006_an.py
--rw-r--r--   0        0        0      447 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial007.py
--rw-r--r--   0        0        0      523 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial007_an.py
--rw-r--r--   0        0        0      210 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial008.py
--rw-r--r--   0        0        0      261 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/help/tutorial008_an.py
--rw-r--r--   0        0        0      131 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/optional/tutorial001.py
--rw-r--r--   0        0        0      181 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/optional/tutorial001_an.py
--rw-r--r--   0        0        0      247 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/optional/tutorial002.py
--rw-r--r--   0        0        0      292 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/optional/tutorial002_an.py
--rw-r--r--   0        0        0      142 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/arguments/optional/tutorial003.py
--rw-r--r--   0        0        0      241 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/arguments/tutorial001.py
--rw-r--r--   0        0        0      721 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/callback/tutorial001.py
--rw-r--r--   0        0        0      216 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/callback/tutorial002.py
--rw-r--r--   0        0        0      304 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/callback/tutorial003.py
--rw-r--r--   0        0        0      315 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/callback/tutorial004.py
--rw-r--r--   0        0        0      411 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/context/tutorial001.py
--rw-r--r--   0        0        0      390 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/context/tutorial002.py
--rw-r--r--   0        0        0      451 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/context/tutorial003.py
--rw-r--r--   0        0        0      277 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/context/tutorial004.py
--rw-r--r--   0        0        0     1196 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/help/tutorial001.py
--rw-r--r--   0        0        0     1300 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/help/tutorial001_an.py
--rw-r--r--   0        0        0      439 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/help/tutorial002.py
--rw-r--r--   0        0        0      386 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/help/tutorial003.py
--rw-r--r--   0        0        0      826 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/help/tutorial004.py
--rw-r--r--   0        0        0      902 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/help/tutorial004_an.py
--rw-r--r--   0        0        0      786 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/help/tutorial005.py
--rw-r--r--   0        0        0      854 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/help/tutorial005_an.py
--rw-r--r--   0        0        0     1143 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/help/tutorial006.py
--rw-r--r--   0        0        0     1044 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/help/tutorial007.py
--rw-r--r--   0        0        0     1200 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/help/tutorial007_an.py
--rw-r--r--   0        0        0      293 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/help/tutorial008.py
--rw-r--r--   0        0        0      138 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/index/tutorial001.py
--rw-r--r--   0        0        0      215 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/index/tutorial002.py
--rw-r--r--   0        0        0      235 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/index/tutorial003.py
--rw-r--r--   0        0        0      275 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/name/tutorial001.py
--rw-r--r--   0        0        0      187 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/one_or_multiple/tutorial001.py
--rw-r--r--   0        0        0      287 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/one_or_multiple/tutorial002.py
--rw-r--r--   0        0        0      693 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/options/tutorial001.py
--rw-r--r--   0        0        0      771 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/commands/options/tutorial001_an.py
--rw-r--r--   0        0        0      115 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/exceptions/tutorial001.py
--rw-r--r--   0        0        0      174 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/exceptions/tutorial002.py
--rw-r--r--   0        0        0      170 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/exceptions/tutorial003.py
--rw-r--r--   0        0        0      171 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/exceptions/tutorial004.py
--rw-r--r--   0        0        0      101 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/first_steps/tutorial001.py
--rw-r--r--   0        0        0      112 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/first_steps/tutorial002.py
--rw-r--r--   0        0        0      138 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/first_steps/tutorial003.py
--rw-r--r--   0        0        0      239 2024-03-23 17:03:25.234094 typer-0.9.3/docs_src/first_steps/tutorial004.py
--rw-r--r--   0        0        0      244 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/first_steps/tutorial005.py
--rw-r--r--   0        0        0      358 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/first_steps/tutorial006.py
--rw-r--r--   0        0        0      157 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/launch/tutorial001.py
--rw-r--r--   0        0        0      527 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/launch/tutorial002.py
--rw-r--r--   0        0        0      294 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/multiple_values/arguments_with_multiple_values/tutorial001.py
--rw-r--r--   0        0        0      291 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/multiple_values/arguments_with_multiple_values/tutorial002.py
--rw-r--r--   0        0        0      342 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/multiple_values/arguments_with_multiple_values/tutorial002_an.py
--rw-r--r--   0        0        0      295 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/multiple_values/multiple_options/tutorial001.py
--rw-r--r--   0        0        0      348 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/multiple_values/multiple_options/tutorial001_an.py
--rw-r--r--   0        0        0      178 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/multiple_values/multiple_options/tutorial002.py
--rw-r--r--   0        0        0      231 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/multiple_values/multiple_options/tutorial002_an.py
--rw-r--r--   0        0        0      403 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/multiple_values/options_with_multiple_values/tutorial001.py
--rw-r--r--   0        0        0      456 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/multiple_values/options_with_multiple_values/tutorial001_an.py
--rw-r--r--   0        0        0      291 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/callback/tutorial001.py
--rw-r--r--   0        0        0      336 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/callback/tutorial001_an.py
--rw-r--r--   0        0        0      320 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/callback/tutorial002.py
--rw-r--r--   0        0        0      365 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/callback/tutorial002_an.py
--rw-r--r--   0        0        0      385 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/callback/tutorial003.py
--rw-r--r--   0        0        0      430 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/callback/tutorial003_an.py
--rw-r--r--   0        0        0      429 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/callback/tutorial004.py
--rw-r--r--   0        0        0      474 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/callback/tutorial004_an.py
--rw-r--r--   0        0        0      464 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/help/tutorial001.py
--rw-r--r--   0        0        0      526 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/help/tutorial001_an.py
--rw-r--r--   0        0        0      643 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/help/tutorial002.py
--rw-r--r--   0        0        0      778 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/help/tutorial002_an.py
--rw-r--r--   0        0        0      170 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/help/tutorial003.py
--rw-r--r--   0        0        0      221 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/help/tutorial003_an.py
--rw-r--r--   0        0        0      216 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/help/tutorial004.py
--rw-r--r--   0        0        0      267 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/help/tutorial004_an.py
--rw-r--r--   0        0        0      152 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/name/tutorial001.py
--rw-r--r--   0        0        0      197 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/name/tutorial001_an.py
--rw-r--r--   0        0        0      158 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/name/tutorial002.py
--rw-r--r--   0        0        0      203 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/name/tutorial002_an.py
--rw-r--r--   0        0        0      148 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/name/tutorial003.py
--rw-r--r--   0        0        0      193 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/name/tutorial003_an.py
--rw-r--r--   0        0        0      163 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/name/tutorial004.py
--rw-r--r--   0        0        0      208 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/name/tutorial004_an.py
--rw-r--r--   0        0        0      281 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/name/tutorial005.py
--rw-r--r--   0        0        0      337 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/name/tutorial005_an.py
--rw-r--r--   0        0        0      212 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/password/tutorial001.py
--rw-r--r--   0        0        0      262 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/password/tutorial001_an.py
--rw-r--r--   0        0        0      341 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/password/tutorial002.py
--rw-r--r--   0        0        0      386 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/password/tutorial002_an.py
--rw-r--r--   0        0        0      171 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/prompt/tutorial001.py
--rw-r--r--   0        0        0      216 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/prompt/tutorial001_an.py
--rw-r--r--   0        0        0      204 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/prompt/tutorial002.py
--rw-r--r--   0        0        0      254 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/prompt/tutorial002_an.py
--rw-r--r--   0        0        0      198 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/prompt/tutorial003.py
--rw-r--r--   0        0        0      249 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/prompt/tutorial003_an.py
--rw-r--r--   0        0        0      155 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/required/tutorial001.py
--rw-r--r--   0        0        0      205 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/required/tutorial001_an.py
--rw-r--r--   0        0        0      166 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/required/tutorial002.py
--rw-r--r--   0        0        0      430 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/version/tutorial001.py
--rw-r--r--   0        0        0      494 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/version/tutorial001_an.py
--rw-r--r--   0        0        0      566 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/version/tutorial002.py
--rw-r--r--   0        0        0      622 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/version/tutorial002_an.py
--rw-r--r--   0        0        0      597 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/version/tutorial003.py
--rw-r--r--   0        0        0      662 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options/version/tutorial003_an.py
--rw-r--r--   0        0        0      193 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial001.py
--rw-r--r--   0        0        0      244 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial001_an.py
--rw-r--r--   0        0        0      312 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial002.py
--rw-r--r--   0        0        0      364 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial002_an.py
--rw-r--r--   0        0        0      478 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial003.py
--rw-r--r--   0        0        0      530 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial003_an.py
--rw-r--r--   0        0        0      664 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial004.py
--rw-r--r--   0        0        0      716 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial004_an.py
--rw-r--r--   0        0        0      563 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial005.py
--rw-r--r--   0        0        0      615 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial005_an.py
--rw-r--r--   0        0        0      262 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial006.py
--rw-r--r--   0        0        0      319 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial006_an.py
--rw-r--r--   0        0        0      699 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial007.py
--rw-r--r--   0        0        0      760 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial007_an.py
--rw-r--r--   0        0        0      735 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial008.py
--rw-r--r--   0        0        0      796 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial008_an.py
--rw-r--r--   0        0        0      818 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial009.py
--rw-r--r--   0        0        0      879 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/options_autocompletion/tutorial009_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/bool/__init__.py
--rw-r--r--   0        0        0      208 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/bool/tutorial001.py
--rw-r--r--   0        0        0      259 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/bool/tutorial001_an.py
--rw-r--r--   0        0        0      323 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/bool/tutorial002.py
--rw-r--r--   0        0        0      374 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/bool/tutorial002_an.py
--rw-r--r--   0        0        0      228 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/bool/tutorial003.py
--rw-r--r--   0        0        0      279 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/bool/tutorial003_an.py
--rw-r--r--   0        0        0      225 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/bool/tutorial004.py
--rw-r--r--   0        0        0      276 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/bool/tutorial004_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/custom_types/__init__.py
--rw-r--r--   0        0        0      542 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/custom_types/tutorial001.py
--rw-r--r--   0        0        0      605 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/custom_types/tutorial001_an.py
--rw-r--r--   0        0        0      646 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/custom_types/tutorial002.py
--rw-r--r--   0        0        0      721 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/custom_types/tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/datetime/__init__.py
--rw-r--r--   0        0        0      211 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/datetime/tutorial001.py
--rw-r--r--   0        0        0      293 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/datetime/tutorial002.py
--rw-r--r--   0        0        0      369 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/datetime/tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/enum/__init__.py
--rw-r--r--   0        0        0      299 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/enum/tutorial001.py
--rw-r--r--   0        0        0      341 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/enum/tutorial002.py
--rw-r--r--   0        0        0      406 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/enum/tutorial002_an.py
--rw-r--r--   0        0        0      349 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/enum/tutorial003.py
--rw-r--r--   0        0        0      402 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/enum/tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/file/__init__.py
--rw-r--r--   0        0        0      180 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/file/tutorial001.py
--rw-r--r--   0        0        0      227 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/file/tutorial001_an.py
--rw-r--r--   0        0        0      202 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/file/tutorial002.py
--rw-r--r--   0        0        0      249 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/file/tutorial002_an.py
--rw-r--r--   0        0        0      321 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/file/tutorial003.py
--rw-r--r--   0        0        0      368 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/file/tutorial003_an.py
--rw-r--r--   0        0        0      547 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/file/tutorial004.py
--rw-r--r--   0        0        0      594 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/file/tutorial004_an.py
--rw-r--r--   0        0        0      205 2024-03-23 17:03:25.238094 typer-0.9.3/docs_src/parameter_types/file/tutorial005.py
--rw-r--r--   0        0        0      250 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/file/tutorial005_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/index/__init__.py
--rw-r--r--   0        0        0      394 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/index/tutorial001.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/number/__init__.py
--rw-r--r--   0        0        0      302 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/number/tutorial001.py
--rw-r--r--   0        0        0      369 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/number/tutorial001_an.py
--rw-r--r--   0        0        0      335 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/number/tutorial002.py
--rw-r--r--   0        0        0      402 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/number/tutorial002_an.py
--rw-r--r--   0        0        0      178 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/number/tutorial003.py
--rw-r--r--   0        0        0      229 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/number/tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/path/__init__.py
--rw-r--r--   0        0        0      530 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/path/tutorial001.py
--rw-r--r--   0        0        0      583 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/path/tutorial001_an.py
--rw-r--r--   0        0        0      371 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/path/tutorial002.py
--rw-r--r--   0        0        0      459 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/path/tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/uuid/__init__.py
--rw-r--r--   0        0        0      196 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/parameter_types/uuid/tutorial001.py
--rw-r--r--   0        0        0      296 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/printing/tutorial001.py
--rw-r--r--   0        0        0      183 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/printing/tutorial002.py
--rw-r--r--   0        0        0      296 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/printing/tutorial003.py
--rw-r--r--   0        0        0      214 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/printing/tutorial004.py
--rw-r--r--   0        0        0      365 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/printing/tutorial005.py
--rw-r--r--   0        0        0      150 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/printing/tutorial006.py
--rw-r--r--   0        0        0      315 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/progressbar/tutorial001.py
--rw-r--r--   0        0        0      476 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/progressbar/tutorial002.py
--rw-r--r--   0        0        0      313 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/progressbar/tutorial003.py
--rw-r--r--   0        0        0      455 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/progressbar/tutorial004.py
--rw-r--r--   0        0        0      333 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/progressbar/tutorial005.py
--rw-r--r--   0        0        0      336 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/progressbar/tutorial006.py
--rw-r--r--   0        0        0      162 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/prompt/tutorial001.py
--rw-r--r--   0        0        0      245 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/prompt/tutorial002.py
--rw-r--r--   0        0        0      180 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/prompt/tutorial003.py
--rw-r--r--   0        0        0      193 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/prompt/tutorial004.py
--rw-r--r--   0        0        0      304 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/callback_override/tutorial001.py
--rw-r--r--   0        0        0      306 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/callback_override/tutorial002.py
--rw-r--r--   0        0        0      409 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/callback_override/tutorial003.py
--rw-r--r--   0        0        0      533 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/callback_override/tutorial004.py
--rw-r--r--   0        0        0      254 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/name_help/tutorial001.py
--rw-r--r--   0        0        0      289 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/name_help/tutorial002.py
--rw-r--r--   0        0        0      282 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/name_help/tutorial003.py
--rw-r--r--   0        0        0      372 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/name_help/tutorial004.py
--rw-r--r--   0        0        0      473 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/name_help/tutorial005.py
--rw-r--r--   0        0        0      514 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/name_help/tutorial006.py
--rw-r--r--   0        0        0      564 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/name_help/tutorial007.py
--rw-r--r--   0        0        0      644 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/name_help/tutorial008.py
--rw-r--r--   0        0        0      298 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/tutorial001/items.py
--rw-r--r--   0        0        0      177 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/tutorial001/main.py
--rw-r--r--   0        0        0      245 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/tutorial001/users.py
--rw-r--r--   0        0        0      698 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/tutorial002/main.py
--rw-r--r--   0        0        0      298 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/tutorial003/items.py
--rw-r--r--   0        0        0      180 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/tutorial003/lands.py
--rw-r--r--   0        0        0      229 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/tutorial003/main.py
--rw-r--r--   0        0        0      233 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/tutorial003/reigns.py
--rw-r--r--   0        0        0      221 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/tutorial003/towns.py
--rw-r--r--   0        0        0      245 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/subcommands/tutorial003/users.py
--rw-r--r--   0        0        0      598 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/terminating/tutorial001.py
--rw-r--r--   0        0        0      235 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/terminating/tutorial002.py
--rw-r--r--   0        0        0      230 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/terminating/tutorial003.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/testing/app01/__init__.py
--rw-r--r--   0        0        0      256 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/testing/app01/main.py
--rw-r--r--   0        0        0      299 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/testing/app01/test_main.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/testing/app02/__init__.py
--rw-r--r--   0        0        0      207 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/testing/app02/main.py
--rw-r--r--   0        0        0      284 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/testing/app02/test_main.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/testing/app02_an/__init__.py
--rw-r--r--   0        0        0      252 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/testing/app02_an/main.py
--rw-r--r--   0        0        0      284 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/testing/app02_an/test_main.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/testing/app03/__init__.py
--rw-r--r--   0        0        0      122 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/testing/app03/main.py
--rw-r--r--   0        0        0      284 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/testing/app03/test_main.py
--rw-r--r--   0        0        0      371 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/using_click/tutorial001.py
--rw-r--r--   0        0        0      287 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/using_click/tutorial002.py
--rw-r--r--   0        0        0      626 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/using_click/tutorial003.py
--rw-r--r--   0        0        0      511 2024-03-23 17:03:25.242094 typer-0.9.3/docs_src/using_click/tutorial004.py
--rw-r--r--   0        0        0       51 2024-03-23 17:03:25.242094 typer-0.9.3/mkdocs.insiders.yml
--rw-r--r--   0        0        0     5528 2024-03-23 17:03:25.242094 typer-0.9.3/mkdocs.yml
--rw-r--r--   0        0        0       96 2024-03-23 17:03:25.242094 typer-0.9.3/mypy.ini
--rw-r--r--   0        0        0     3002 2024-03-23 17:03:25.242094 typer-0.9.3/pyproject.toml
--rwxr-xr-x   0        0        0       76 2024-03-23 17:03:25.242094 typer-0.9.3/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       98 2024-03-23 17:03:25.242094 typer-0.9.3/scripts/clean.sh
--rwxr-xr-x   0        0        0       68 2024-03-23 17:03:25.242094 typer-0.9.3/scripts/docs-live.sh
--rwxr-xr-x   0        0        0      167 2024-03-23 17:03:25.242094 typer-0.9.3/scripts/format-imports.sh
--rwxr-xr-x   0        0        0      205 2024-03-23 17:03:25.242094 typer-0.9.3/scripts/format.sh
--rw-r--r--   0        0        0      112 2024-03-23 17:03:25.242094 typer-0.9.3/scripts/get-pwsh-activate.sh
--rwxr-xr-x   0        0        0      122 2024-03-23 17:03:25.242094 typer-0.9.3/scripts/lint.sh
--rwxr-xr-x   0        0        0      339 2024-03-23 17:03:25.242094 typer-0.9.3/scripts/netlify-docs.sh
--rwxr-xr-x   0        0        0       42 2024-03-23 17:03:25.242094 typer-0.9.3/scripts/publish.sh
--rwxr-xr-x   0        0        0       80 2024-03-23 17:03:25.242094 typer-0.9.3/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0      350 2024-03-23 17:03:25.242094 typer-0.9.3/scripts/test-files.sh
--rwxr-xr-x   0        0        0      490 2024-03-23 17:03:25.242094 typer-0.9.3/scripts/test.sh
--rw-r--r--   0        0        0      115 2024-03-23 17:03:25.242094 typer-0.9.3/scripts/zip-docs.sh
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.242094 typer-0.9.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.242094 typer-0.9.3/tests/assets/__init__.py
--rw-r--r--   0        0        0      675 2024-03-23 17:03:25.242094 typer-0.9.3/tests/assets/compat_click7_8.py
--rw-r--r--   0        0        0      542 2024-03-23 17:03:25.242094 typer-0.9.3/tests/assets/completion_no_types.py
--rw-r--r--   0        0        0      542 2024-03-23 17:03:25.242094 typer-0.9.3/tests/assets/completion_no_types_order.py
--rw-r--r--   0        0        0      160 2024-03-23 17:03:25.242094 typer-0.9.3/tests/assets/prog_name.py
--rw-r--r--   0        0        0      157 2024-03-23 17:03:25.242094 typer-0.9.3/tests/assets/type_error_no_rich.py
--rw-r--r--   0        0        0      213 2024-03-23 17:03:25.242094 typer-0.9.3/tests/assets/type_error_no_rich_short_disable.py
--rw-r--r--   0        0        0      306 2024-03-23 17:03:25.242094 typer-0.9.3/tests/assets/type_error_normal_traceback.py
--rw-r--r--   0        0        0     6941 2024-03-23 17:03:25.242094 typer-0.9.3/tests/test_ambiguous_params.py
--rw-r--r--   0        0        0     2081 2024-03-23 17:03:25.242094 typer-0.9.3/tests/test_annotated.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.242094 typer-0.9.3/tests/test_compat/__init__.py
--rw-r--r--   0        0        0     1618 2024-03-23 17:03:25.242094 typer-0.9.3/tests/test_compat/test_option_get_help.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.242094 typer-0.9.3/tests/test_completion/__init__.py
--rw-r--r--   0        0        0     5328 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_completion/test_completion.py
--rw-r--r--   0        0        0     5782 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_completion/test_completion_complete.py
--rw-r--r--   0        0        0     2209 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_completion/test_completion_complete_no_help.py
--rw-r--r--   0        0        0     5943 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_completion/test_completion_install.py
--rw-r--r--   0        0        0     3891 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_completion/test_completion_show.py
--rw-r--r--   0        0        0      797 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_exit_errors.py
--rw-r--r--   0        0        0     8120 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_others.py
--rw-r--r--   0        0        0      410 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_prog_name.py
--rw-r--r--   0        0        0      849 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_rich_utils.py
--rw-r--r--   0        0        0     2556 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tracebacks.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_default/__init__.py
--rw-r--r--   0        0        0      980 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py
--rw-r--r--   0        0        0      998 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_default/test_tutorial001_an.py
--rw-r--r--   0        0        0     1105 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py
--rw-r--r--   0        0        0     1108 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_default/test_tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_envvar/__init__.py
--rw-r--r--   0        0        0     1654 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py
--rw-r--r--   0        0        0     1657 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001_an.py
--rw-r--r--   0        0        0     1250 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py
--rw-r--r--   0        0        0     1253 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002_an.py
--rw-r--r--   0        0        0     1271 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py
--rw-r--r--   0        0        0     1274 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/__init__.py
--rw-r--r--   0        0        0     1343 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py
--rw-r--r--   0        0        0     1346 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial001_an.py
--rw-r--r--   0        0        0      988 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py
--rw-r--r--   0        0        0      991 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial002_an.py
--rw-r--r--   0        0        0      979 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py
--rw-r--r--   0        0        0      982 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial003_an.py
--rw-r--r--   0        0        0      983 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py
--rw-r--r--   0        0        0      986 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial004_an.py
--rw-r--r--   0        0        0      901 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py
--rw-r--r--   0        0        0      904 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial005_an.py
--rw-r--r--   0        0        0      885 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py
--rw-r--r--   0        0        0      888 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial006_an.py
--rw-r--r--   0        0        0      875 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py
--rw-r--r--   0        0        0      878 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial007_an.py
--rw-r--r--   0        0        0     1323 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py
--rw-r--r--   0        0        0     1326 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial008_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_optional/__init__.py
--rw-r--r--   0        0        0     1188 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py
--rw-r--r--   0        0        0     1191 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_optional/test_tutorial001_an.py
--rw-r--r--   0        0        0      883 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py
--rw-r--r--   0        0        0      886 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_optional/test_tutorial002_an.py
--rw-r--r--   0        0        0     1188 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_arguments/test_optional/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_arguments/__init__.py
--rw-r--r--   0        0        0     1078 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_callback/__init__.py
--rw-r--r--   0        0        0     2333 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py
--rw-r--r--   0        0        0      624 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py
--rw-r--r--   0        0        0      741 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py
--rw-r--r--   0        0        0      864 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_context/__init__.py
--rw-r--r--   0        0        0      864 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_context/test_tutorial001.py
--rw-r--r--   0        0        0      982 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_context/test_tutorial002.py
--rw-r--r--   0        0        0      990 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_context/test_tutorial003.py
--rw-r--r--   0        0        0      749 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_context/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_help/__init__.py
--rw-r--r--   0        0        0     4223 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial001.py
--rw-r--r--   0        0        0     4226 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial001_an.py
--rw-r--r--   0        0        0     1679 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial002.py
--rw-r--r--   0        0        0     1138 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial003.py
--rw-r--r--   0        0        0     1839 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial004.py
--rw-r--r--   0        0        0     1844 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial004_an.py
--rw-r--r--   0        0        0     1906 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial005.py
--rw-r--r--   0        0        0     1911 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial005_an.py
--rw-r--r--   0        0        0     1610 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial006.py
--rw-r--r--   0        0        0     1707 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial007.py
--rw-r--r--   0        0        0     1710 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial007_an.py
--rw-r--r--   0        0        0      743 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial008.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_index/__init__.py
--rw-r--r--   0        0        0      695 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_index/test_tutorial001.py
--rw-r--r--   0        0        0      993 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_index/test_tutorial002.py
--rw-r--r--   0        0        0      983 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_index/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_name/__init__.py
--rw-r--r--   0        0        0      944 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_name/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_one_or_multiple/__init__.py
--rw-r--r--   0        0        0      754 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py
--rw-r--r--   0        0        0      898 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_options/__init__.py
--rw-r--r--   0        0        0     3052 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_options/test_tutorial001.py
--rw-r--r--   0        0        0     3055 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_commands/test_options/test_tutorial001_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_exceptions/__init__.py
--rw-r--r--   0        0        0     1963 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_exceptions/test_tutorial001.py
--rw-r--r--   0        0        0     1975 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_exceptions/test_tutorial002.py
--rw-r--r--   0        0        0     1200 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_exceptions/test_tutorial003.py
--rw-r--r--   0        0        0     1145 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_exceptions/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_first_steps/__init__.py
--rw-r--r--   0        0        0      561 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_first_steps/test_tutorial001.py
--rw-r--r--   0        0        0      731 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_first_steps/test_tutorial002.py
--rw-r--r--   0        0        0      768 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_first_steps/test_tutorial003.py
--rw-r--r--   0        0        0     1554 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_first_steps/test_tutorial004.py
--rw-r--r--   0        0        0     1543 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_first_steps/test_tutorial005.py
--rw-r--r--   0        0        0     1419 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_first_steps/test_tutorial006.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_multiple_values/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/__init__.py
--rw-r--r--   0        0        0      757 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py
--rw-r--r--   0        0        0     1512 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py
--rw-r--r--   0        0        0     1524 2024-03-23 17:03:25.246094 typer-0.9.3/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_multiple_values/test_multiple_options/__init__.py
--rw-r--r--   0        0        0     1126 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py
--rw-r--r--   0        0        0     1129 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001_an.py
--rw-r--r--   0        0        0      943 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py
--rw-r--r--   0        0        0      946 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/__init__.py
--rw-r--r--   0        0        0     1466 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py
--rw-r--r--   0        0        0     1469 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_callback/__init__.py
--rw-r--r--   0        0        0      789 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_callback/test_tutorial001.py
--rw-r--r--   0        0        0      792 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_callback/test_tutorial001_an.py
--rw-r--r--   0        0        0     1335 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_callback/test_tutorial003.py
--rw-r--r--   0        0        0     1344 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_callback/test_tutorial003_an.py
--rw-r--r--   0        0        0     1342 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_callback/test_tutorial004.py
--rw-r--r--   0        0        0     1351 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_callback/test_tutorial004_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_help/__init__.py
--rw-r--r--   0        0        0     1334 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_help/test_tutorial001.py
--rw-r--r--   0        0        0     1337 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_help/test_tutorial001_an.py
--rw-r--r--   0        0        0     1103 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_help/test_tutorial002.py
--rw-r--r--   0        0        0     1106 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_help/test_tutorial002_an.py
--rw-r--r--   0        0        0      818 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_help/test_tutorial003.py
--rw-r--r--   0        0        0      821 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_help/test_tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_name/__init__.py
--rw-r--r--   0        0        0     1138 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial001.py
--rw-r--r--   0        0        0     1141 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial001_an.py
--rw-r--r--   0        0        0     1010 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial002.py
--rw-r--r--   0        0        0     1013 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial002_an.py
--rw-r--r--   0        0        0      860 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial003.py
--rw-r--r--   0        0        0      863 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial003_an.py
--rw-r--r--   0        0        0     1015 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial004.py
--rw-r--r--   0        0        0     1018 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial004_an.py
--rw-r--r--   0        0        0     1344 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial005.py
--rw-r--r--   0        0        0     1347 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial005_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_prompt/__init__.py
--rw-r--r--   0        0        0     1090 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py
--rw-r--r--   0        0        0     1093 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_prompt/test_tutorial001_an.py
--rw-r--r--   0        0        0     1111 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py
--rw-r--r--   0        0        0     1114 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_prompt/test_tutorial002_an.py
--rw-r--r--   0        0        0     1537 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py
--rw-r--r--   0        0        0     1540 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_prompt/test_tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_required/__init__.py
--rw-r--r--   0        0        0     1335 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_required/test_tutorial001.py
--rw-r--r--   0        0        0     1338 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_required/test_tutorial001_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_version/__init__.py
--rw-r--r--   0        0        0     1475 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_version/test_tutorial003.py
--rw-r--r--   0        0        0     1484 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options/test_version/test_tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options_autocompletion/__init__.py
--rw-r--r--   0        0        0     1119 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial002.py
--rw-r--r--   0        0        0     1128 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial002_an.py
--rw-r--r--   0        0        0     1130 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial003.py
--rw-r--r--   0        0        0     1139 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial003_an.py
--rw-r--r--   0        0        0     1199 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial004.py
--rw-r--r--   0        0        0     1208 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial004_an.py
--rw-r--r--   0        0        0     1285 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial007.py
--rw-r--r--   0        0        0     1294 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial007_an.py
--rw-r--r--   0        0        0     1389 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial008.py
--rw-r--r--   0        0        0     1398 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial008_an.py
--rw-r--r--   0        0        0     1433 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial009.py
--rw-r--r--   0        0        0     1442 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial009_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/__init__.py
--rw-r--r--   0        0        0     1222 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py
--rw-r--r--   0        0        0     1225 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001_an.py
--rw-r--r--   0        0        0     1745 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py
--rw-r--r--   0        0        0     1748 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002_an.py
--rw-r--r--   0        0        0      985 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py
--rw-r--r--   0        0        0      988 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003_an.py
--rw-r--r--   0        0        0     1047 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py
--rw-r--r--   0        0        0     1050 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_custom_types/__init__.py
--rw-r--r--   0        0        0     1017 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001.py
--rw-r--r--   0        0        0     1024 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001_an.py
--rw-r--r--   0        0        0     1027 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002.py
--rw-r--r--   0        0        0     1030 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_datetime/__init__.py
--rw-r--r--   0        0        0     1471 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py
--rw-r--r--   0        0        0      824 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py
--rw-r--r--   0        0        0      827 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_enum/__init__.py
--rw-r--r--   0        0        0     1849 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py
--rw-r--r--   0        0        0      815 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py
--rw-r--r--   0        0        0      818 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002_an.py
--rw-r--r--   0        0        0     1238 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003.py
--rw-r--r--   0        0        0     1241 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/__init__.py
--rw-r--r--   0        0        0      866 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py
--rw-r--r--   0        0        0      869 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001_an.py
--rw-r--r--   0        0        0      892 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py
--rw-r--r--   0        0        0      895 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002_an.py
--rw-r--r--   0        0        0      811 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py
--rw-r--r--   0        0        0      814 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003_an.py
--rw-r--r--   0        0        0      926 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py
--rw-r--r--   0        0        0      929 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004_an.py
--rw-r--r--   0        0        0     1080 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py
--rw-r--r--   0        0        0     1083 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_index/__init__.py
--rw-r--r--   0        0        0     1534 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_number/__init__.py
--rw-r--r--   0        0        0     2816 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py
--rw-r--r--   0        0        0     2819 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001_an.py
--rw-r--r--   0        0        0     1091 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py
--rw-r--r--   0        0        0     1094 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002_an.py
--rw-r--r--   0        0        0     1412 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py
--rw-r--r--   0        0        0     1415 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_path/__init__.py
--rw-r--r--   0        0        0     1495 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py
--rw-r--r--   0        0        0     1498 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001_an.py
--rw-r--r--   0        0        0     1345 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py
--rw-r--r--   0        0        0     1348 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_uuid/__init__.py
--rw-r--r--   0        0        0     1139 2024-03-23 17:03:25.250094 typer-0.9.3/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_prompt/__init__.py
--rw-r--r--   0        0        0      644 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_prompt/test_tutorial001.py
--rw-r--r--   0        0        0      920 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_prompt/test_tutorial002.py
--rw-r--r--   0        0        0      877 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_prompt/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_callback_override/__init__.py
--rw-r--r--   0        0        0      651 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py
--rw-r--r--   0        0        0      651 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py
--rw-r--r--   0        0        0      780 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py
--rw-r--r--   0        0        0      882 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/__init__.py
--rw-r--r--   0        0        0      987 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py
--rw-r--r--   0        0        0      987 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py
--rw-r--r--   0        0        0      987 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py
--rw-r--r--   0        0        0      987 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py
--rw-r--r--   0        0        0     1029 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py
--rw-r--r--   0        0        0      979 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py
--rw-r--r--   0        0        0     1012 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py
--rw-r--r--   0        0        0     1025 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py
--rw-r--r--   0        0        0     2726 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_tutorial001.py
--rw-r--r--   0        0        0     2178 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_tutorial002.py
--rw-r--r--   0        0        0     5668 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_subcommands/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_terminating/__init__.py
--rw-r--r--   0        0        0     1168 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_terminating/test_tutorial001.py
--rw-r--r--   0        0        0      756 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_terminating/test_tutorial002.py
--rw-r--r--   0        0        0     1273 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_terminating/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_testing/__init__.py
--rw-r--r--   0        0        0      423 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_testing/test_app01.py
--rw-r--r--   0        0        0      423 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_testing/test_app02.py
--rw-r--r--   0        0        0      432 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_testing/test_app02_an.py
--rw-r--r--   0        0        0      423 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_testing/test_app03.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_using_click/__init__.py
--rw-r--r--   0        0        0     1118 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_using_click/test_tutorial003.py
--rw-r--r--   0        0        0      971 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_tutorial/test_using_click/test_tutorial004.py
--rw-r--r--   0        0        0     3316 2024-03-23 17:03:25.254094 typer-0.9.3/tests/test_type_conversion.py
--rw-r--r--   0        0        0      125 2024-03-23 17:03:25.254094 typer-0.9.3/tests/utils.py
--rw-r--r--   0        0        0     1602 2024-03-23 17:03:25.254094 typer-0.9.3/typer/__init__.py
--rw-r--r--   0        0        0       94 2024-03-23 17:03:25.254094 typer-0.9.3/typer/_compat_utils.py
--rw-r--r--   0        0        0     4957 2024-03-23 17:03:25.254094 typer-0.9.3/typer/_completion_click7.py
--rw-r--r--   0        0        0     6688 2024-03-23 17:03:25.254094 typer-0.9.3/typer/_completion_click8.py
--rw-r--r--   0        0        0     8541 2024-03-23 17:03:25.254094 typer-0.9.3/typer/_completion_shared.py
--rw-r--r--   0        0        0    19713 2024-03-23 17:03:25.254094 typer-0.9.3/typer/_typing.py
--rw-r--r--   0        0        0      430 2024-03-23 17:03:25.254094 typer-0.9.3/typer/colors.py
--rw-r--r--   0        0        0     4999 2024-03-23 17:03:25.254094 typer-0.9.3/typer/completion.py
--rw-r--r--   0        0        0    26858 2024-03-23 17:03:25.254094 typer-0.9.3/typer/core.py
--rw-r--r--   0        0        0    39286 2024-03-23 17:03:25.254094 typer-0.9.3/typer/main.py
--rw-r--r--   0        0        0    15993 2024-03-23 17:03:25.254094 typer-0.9.3/typer/models.py
--rw-r--r--   0        0        0    13787 2024-03-23 17:03:25.254094 typer-0.9.3/typer/params.py
--rw-r--r--   0        0        0        0 2024-03-23 17:03:25.254094 typer-0.9.3/typer/py.typed
--rw-r--r--   0        0        0    23654 2024-03-23 17:03:25.254094 typer-0.9.3/typer/rich_utils.py
--rw-r--r--   0        0        0      874 2024-03-23 17:03:25.254094 typer-0.9.3/typer/testing.py
--rw-r--r--   0        0        0     7414 2024-03-23 17:03:25.254094 typer-0.9.3/typer/utils.py
--rw-r--r--   0        0        0    14615 1970-01-01 00:00:00.000000 typer-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      310 2024-03-23 17:07:37.117673 typer-0.9.4/.coveragerc
+-rw-r--r--   0        0        0     5303 2024-03-23 17:07:37.117673 typer-0.9.4/.github/DISCUSSION_TEMPLATE/questions.yml
+-rw-r--r--   0        0        0       19 2024-03-23 17:07:37.117673 typer-0.9.4/.github/FUNDING.yml
+-rw-r--r--   0        0        0      758 2024-03-23 17:07:37.117673 typer-0.9.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      885 2024-03-23 17:07:37.117673 typer-0.9.4/.github/ISSUE_TEMPLATE/privileged.yml
+-rw-r--r--   0        0        0      115 2024-03-23 17:07:37.117673 typer-0.9.4/.github/actions/comment-docs-preview-in-pr/Dockerfile
+-rw-r--r--   0        0        0      394 2024-03-23 17:07:37.117673 typer-0.9.4/.github/actions/comment-docs-preview-in-pr/action.yml
+-rw-r--r--   0        0        0     2074 2024-03-23 17:07:37.117673 typer-0.9.4/.github/actions/comment-docs-preview-in-pr/app/main.py
+-rw-r--r--   0        0        0      309 2024-03-23 17:07:37.117673 typer-0.9.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     3029 2024-03-23 17:07:37.117673 typer-0.9.4/.github/workflows/build-docs.yml
+-rw-r--r--   0        0        0     1630 2024-03-23 17:07:37.117673 typer-0.9.4/.github/workflows/deploy-docs.yml
+-rw-r--r--   0        0        0      576 2024-03-23 17:07:37.117673 typer-0.9.4/.github/workflows/issue-manager.yml
+-rw-r--r--   0        0        0     1256 2024-03-23 17:07:37.117673 typer-0.9.4/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0      567 2024-03-23 17:07:37.117673 typer-0.9.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      957 2024-03-23 17:07:37.117673 typer-0.9.4/.github/workflows/smokeshow.yml
+-rw-r--r--   0        0        0     2266 2024-03-23 17:07:37.117673 typer-0.9.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      117 2024-03-23 17:07:37.117673 typer-0.9.4/.gitignore
+-rw-r--r--   0        0        0     1525 2024-03-23 17:07:37.117673 typer-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      568 2024-03-23 17:07:37.117673 typer-0.9.4/CITATION.cff
+-rw-r--r--   0        0        0      125 2024-03-23 17:07:37.117673 typer-0.9.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1086 2024-03-23 17:07:37.117673 typer-0.9.4/LICENSE
+-rw-r--r--   0        0        0    11885 2024-03-23 17:07:37.117673 typer-0.9.4/README.md
+-rw-r--r--   0        0        0     1160 2024-03-23 17:07:37.117673 typer-0.9.4/SECURITY.md
+-rw-r--r--   0        0        0     4876 2024-03-23 17:07:37.117673 typer-0.9.4/docs/alternatives.md
+-rw-r--r--   0        0        0     5980 2024-03-23 17:07:37.117673 typer-0.9.4/docs/contributing.md
+-rw-r--r--   0        0        0      451 2024-03-23 17:07:37.117673 typer-0.9.4/docs/css/custom.css
+-rw-r--r--   0        0        0     2214 2024-03-23 17:07:37.117673 typer-0.9.4/docs/css/termynal.css
+-rw-r--r--   0        0        0     4434 2024-03-23 17:07:37.117673 typer-0.9.4/docs/features.md
+-rw-r--r--   0        0        0    12075 2024-03-23 17:07:37.117673 typer-0.9.4/docs/help-typer.md
+-rwxr-xr-x   0        0        0      439 2024-03-23 17:07:37.117673 typer-0.9.4/docs/img/favicon.png
+-rw-r--r--   0        0        0    48377 2024-03-23 17:07:37.117673 typer-0.9.4/docs/img/github-social-preview.png
+-rw-r--r--   0        0        0     3936 2024-03-23 17:07:37.117673 typer-0.9.4/docs/img/github-social-preview.svg
+-rw-r--r--   0        0        0      284 2024-03-23 17:07:37.117673 typer-0.9.4/docs/img/icon-black.svg
+-rw-r--r--   0        0        0     1743 2024-03-23 17:07:37.117673 typer-0.9.4/docs/img/icon-white.svg
+-rw-r--r--   0        0        0     6768 2024-03-23 17:07:37.117673 typer-0.9.4/docs/img/logo-margin/logo-margin-vector.svg
+-rw-r--r--   0        0        0     3010 2024-03-23 17:07:37.117673 typer-0.9.4/docs/img/logo-margin/logo-margin.svg
+-rw-r--r--   0        0        0    13924 2024-03-23 17:07:37.117673 typer-0.9.4/docs/img/pycharm-completion.png
+-rw-r--r--   0        0        0    22753 2024-03-23 17:07:37.117673 typer-0.9.4/docs/img/vscode-completion.png
+-rw-r--r--   0        0        0    11885 2024-03-23 17:07:37.117673 typer-0.9.4/docs/index.md
+-rw-r--r--   0        0        0     3897 2024-03-23 17:07:37.117673 typer-0.9.4/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2024-03-23 17:07:37.117673 typer-0.9.4/docs/js/termynal.js
+-rw-r--r--   0        0        0       26 2024-03-23 17:07:37.117673 typer-0.9.4/docs/overrides/main.html
+-rw-r--r--   0        0        0    36717 2024-03-23 17:07:37.117673 typer-0.9.4/docs/release-notes.md
+-rw-r--r--   0        0        0     1445 2024-03-23 17:07:37.117673 typer-0.9.4/docs/tutorial/app-dir.md
+-rw-r--r--   0        0        0     2698 2024-03-23 17:07:37.117673 typer-0.9.4/docs/tutorial/arguments/default.md
+-rw-r--r--   0        0        0     3287 2024-03-23 17:07:37.117673 typer-0.9.4/docs/tutorial/arguments/envvar.md
+-rw-r--r--   0        0        0    11973 2024-03-23 17:07:37.117673 typer-0.9.4/docs/tutorial/arguments/help.md
+-rw-r--r--   0        0        0      173 2024-03-23 17:07:37.117673 typer-0.9.4/docs/tutorial/arguments/index.md
+-rw-r--r--   0        0        0     6809 2024-03-23 17:07:37.117673 typer-0.9.4/docs/tutorial/arguments/optional.md
+-rw-r--r--   0        0        0      163 2024-03-23 17:07:37.117673 typer-0.9.4/docs/tutorial/arguments/other-uses.md
+-rw-r--r--   0        0        0     1084 2024-03-23 17:07:37.117673 typer-0.9.4/docs/tutorial/commands/arguments.md
+-rw-r--r--   0        0        0     4837 2024-03-23 17:07:37.117673 typer-0.9.4/docs/tutorial/commands/callback.md
+-rw-r--r--   0        0        0     3551 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/commands/context.md
+-rw-r--r--   0        0        0    34041 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/commands/help.md
+-rw-r--r--   0        0        0     8202 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/commands/index.md
+-rw-r--r--   0        0        0     1380 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/commands/name.md
+-rw-r--r--   0        0        0     3454 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/commands/one-or-multiple.md
+-rw-r--r--   0        0        0     2293 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/commands/options.md
+-rw-r--r--   0        0        0    24658 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/exceptions.md
+-rw-r--r--   0        0        0    22035 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     2367 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/index.md
+-rw-r--r--   0        0        0      974 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/launch.md
+-rw-r--r--   0        0        0     1969 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/multiple-values/arguments-with-multiple-values.md
+-rw-r--r--   0        0        0      133 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/multiple-values/index.md
+-rw-r--r--   0        0        0     1728 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/multiple-values/multiple-options.md
+-rw-r--r--   0        0        0     2386 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/multiple-values/options-with-multiple-values.md
+-rw-r--r--   0        0        0    14803 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/options-autocompletion.md
+-rw-r--r--   0        0        0     8041 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/options/callback-and-context.md
+-rw-r--r--   0        0        0     7673 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/options/help.md
+-rw-r--r--   0        0        0      202 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/options/index.md
+-rw-r--r--   0        0        0     9245 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/options/name.md
+-rw-r--r--   0        0        0     1754 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/options/password.md
+-rw-r--r--   0        0        0     2579 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/options/prompt.md
+-rw-r--r--   0        0        0     2190 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/options/required.md
+-rw-r--r--   0        0        0     3980 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/options/version.md
+-rw-r--r--   0        0        0    20799 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/package.md
+-rw-r--r--   0        0        0     4288 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/parameter-types/bool.md
+-rw-r--r--   0        0        0     1694 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/parameter-types/custom-types.md
+-rw-r--r--   0        0        0     2490 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/parameter-types/datetime.md
+-rw-r--r--   0        0        0     3108 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/parameter-types/enum.md
+-rw-r--r--   0        0        0     8645 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/parameter-types/file.md
+-rw-r--r--   0        0        0     2016 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/parameter-types/index.md
+-rw-r--r--   0        0        0     3782 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/parameter-types/number.md
+-rw-r--r--   0        0        0     3861 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/parameter-types/path.md
+-rw-r--r--   0        0        0     1739 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/parameter-types/uuid.md
+-rw-r--r--   0        0        0    10363 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/printing.md
+-rw-r--r--   0        0        0     6259 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/progressbar.md
+-rw-r--r--   0        0        0     1909 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/prompt.md
+-rw-r--r--   0        0        0     3795 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/subcommands/add-typer.md
+-rw-r--r--   0        0        0     2984 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/subcommands/callback-override.md
+-rw-r--r--   0        0        0     1201 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/subcommands/index.md
+-rw-r--r--   0        0        0    12517 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/subcommands/name-and-help.md
+-rw-r--r--   0        0        0     6077 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/subcommands/nested-subcommands.md
+-rw-r--r--   0        0        0     2729 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/subcommands/single-file.md
+-rw-r--r--   0        0        0     3013 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/terminating.md
+-rw-r--r--   0        0        0     6367 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/testing.md
+-rw-r--r--   0        0        0     6469 2024-03-23 17:07:37.121673 typer-0.9.4/docs/tutorial/using-click.md
+-rw-r--r--   0        0        0     9703 2024-03-23 17:07:37.121673 typer-0.9.4/docs/typer-cli.md
+-rw-r--r--   0        0        0      310 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/app_dir/tutorial001.py
+-rw-r--r--   0        0        0      144 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/default/tutorial001.py
+-rw-r--r--   0        0        0      197 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/default/tutorial001_an.py
+-rw-r--r--   0        0        0      252 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/default/tutorial002.py
+-rw-r--r--   0        0        0      302 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/default/tutorial002_an.py
+-rw-r--r--   0        0        0      165 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/envvar/tutorial001.py
+-rw-r--r--   0        0        0      216 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/envvar/tutorial001_an.py
+-rw-r--r--   0        0        0      179 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/envvar/tutorial002.py
+-rw-r--r--   0        0        0      236 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/envvar/tutorial002_an.py
+-rw-r--r--   0        0        0      184 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/envvar/tutorial003.py
+-rw-r--r--   0        0        0      255 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/envvar/tutorial003_an.py
+-rw-r--r--   0        0        0      172 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial001.py
+-rw-r--r--   0        0        0      217 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial001_an.py
+-rw-r--r--   0        0        0      231 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial002.py
+-rw-r--r--   0        0        0      276 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial002_an.py
+-rw-r--r--   0        0        0      218 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial003.py
+-rw-r--r--   0        0        0      269 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial003_an.py
+-rw-r--r--   0        0        0      238 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial004.py
+-rw-r--r--   0        0        0      309 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial004_an.py
+-rw-r--r--   0        0        0      231 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial005.py
+-rw-r--r--   0        0        0      313 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial005_an.py
+-rw-r--r--   0        0        0      164 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial006.py
+-rw-r--r--   0        0        0      215 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial006_an.py
+-rw-r--r--   0        0        0      447 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial007.py
+-rw-r--r--   0        0        0      523 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial007_an.py
+-rw-r--r--   0        0        0      210 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial008.py
+-rw-r--r--   0        0        0      261 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/help/tutorial008_an.py
+-rw-r--r--   0        0        0      131 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/optional/tutorial001.py
+-rw-r--r--   0        0        0      181 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/optional/tutorial001_an.py
+-rw-r--r--   0        0        0      247 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/optional/tutorial002.py
+-rw-r--r--   0        0        0      292 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/optional/tutorial002_an.py
+-rw-r--r--   0        0        0      142 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/arguments/optional/tutorial003.py
+-rw-r--r--   0        0        0      241 2024-03-23 17:07:37.121673 typer-0.9.4/docs_src/commands/arguments/tutorial001.py
+-rw-r--r--   0        0        0      721 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/callback/tutorial001.py
+-rw-r--r--   0        0        0      216 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/callback/tutorial002.py
+-rw-r--r--   0        0        0      304 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/callback/tutorial003.py
+-rw-r--r--   0        0        0      315 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/callback/tutorial004.py
+-rw-r--r--   0        0        0      411 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/context/tutorial001.py
+-rw-r--r--   0        0        0      390 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/context/tutorial002.py
+-rw-r--r--   0        0        0      451 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/context/tutorial003.py
+-rw-r--r--   0        0        0      277 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/context/tutorial004.py
+-rw-r--r--   0        0        0     1196 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/help/tutorial001.py
+-rw-r--r--   0        0        0     1300 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/help/tutorial001_an.py
+-rw-r--r--   0        0        0      439 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/help/tutorial002.py
+-rw-r--r--   0        0        0      386 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/help/tutorial003.py
+-rw-r--r--   0        0        0      826 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/help/tutorial004.py
+-rw-r--r--   0        0        0      902 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/help/tutorial004_an.py
+-rw-r--r--   0        0        0      786 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/help/tutorial005.py
+-rw-r--r--   0        0        0      854 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/help/tutorial005_an.py
+-rw-r--r--   0        0        0     1143 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/help/tutorial006.py
+-rw-r--r--   0        0        0     1044 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/help/tutorial007.py
+-rw-r--r--   0        0        0     1200 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/help/tutorial007_an.py
+-rw-r--r--   0        0        0      293 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/help/tutorial008.py
+-rw-r--r--   0        0        0      138 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/index/tutorial001.py
+-rw-r--r--   0        0        0      215 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/index/tutorial002.py
+-rw-r--r--   0        0        0      235 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/index/tutorial003.py
+-rw-r--r--   0        0        0      275 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/name/tutorial001.py
+-rw-r--r--   0        0        0      187 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/one_or_multiple/tutorial001.py
+-rw-r--r--   0        0        0      287 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/one_or_multiple/tutorial002.py
+-rw-r--r--   0        0        0      693 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/options/tutorial001.py
+-rw-r--r--   0        0        0      771 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/commands/options/tutorial001_an.py
+-rw-r--r--   0        0        0      115 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/exceptions/tutorial001.py
+-rw-r--r--   0        0        0      174 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/exceptions/tutorial002.py
+-rw-r--r--   0        0        0      170 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/exceptions/tutorial003.py
+-rw-r--r--   0        0        0      171 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/exceptions/tutorial004.py
+-rw-r--r--   0        0        0      101 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/first_steps/tutorial001.py
+-rw-r--r--   0        0        0      112 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/first_steps/tutorial002.py
+-rw-r--r--   0        0        0      138 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/first_steps/tutorial003.py
+-rw-r--r--   0        0        0      239 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/first_steps/tutorial004.py
+-rw-r--r--   0        0        0      244 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/first_steps/tutorial005.py
+-rw-r--r--   0        0        0      358 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/first_steps/tutorial006.py
+-rw-r--r--   0        0        0      157 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/launch/tutorial001.py
+-rw-r--r--   0        0        0      527 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/launch/tutorial002.py
+-rw-r--r--   0        0        0      294 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/multiple_values/arguments_with_multiple_values/tutorial001.py
+-rw-r--r--   0        0        0      291 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/multiple_values/arguments_with_multiple_values/tutorial002.py
+-rw-r--r--   0        0        0      342 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/multiple_values/arguments_with_multiple_values/tutorial002_an.py
+-rw-r--r--   0        0        0      295 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/multiple_values/multiple_options/tutorial001.py
+-rw-r--r--   0        0        0      348 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/multiple_values/multiple_options/tutorial001_an.py
+-rw-r--r--   0        0        0      178 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/multiple_values/multiple_options/tutorial002.py
+-rw-r--r--   0        0        0      231 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/multiple_values/multiple_options/tutorial002_an.py
+-rw-r--r--   0        0        0      403 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/multiple_values/options_with_multiple_values/tutorial001.py
+-rw-r--r--   0        0        0      456 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/multiple_values/options_with_multiple_values/tutorial001_an.py
+-rw-r--r--   0        0        0      291 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/callback/tutorial001.py
+-rw-r--r--   0        0        0      336 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/callback/tutorial001_an.py
+-rw-r--r--   0        0        0      320 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/callback/tutorial002.py
+-rw-r--r--   0        0        0      365 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/callback/tutorial002_an.py
+-rw-r--r--   0        0        0      385 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/callback/tutorial003.py
+-rw-r--r--   0        0        0      430 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/callback/tutorial003_an.py
+-rw-r--r--   0        0        0      429 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/callback/tutorial004.py
+-rw-r--r--   0        0        0      474 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/callback/tutorial004_an.py
+-rw-r--r--   0        0        0      464 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/help/tutorial001.py
+-rw-r--r--   0        0        0      526 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/help/tutorial001_an.py
+-rw-r--r--   0        0        0      643 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/help/tutorial002.py
+-rw-r--r--   0        0        0      778 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/help/tutorial002_an.py
+-rw-r--r--   0        0        0      170 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/help/tutorial003.py
+-rw-r--r--   0        0        0      221 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/help/tutorial003_an.py
+-rw-r--r--   0        0        0      216 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/help/tutorial004.py
+-rw-r--r--   0        0        0      267 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/help/tutorial004_an.py
+-rw-r--r--   0        0        0      152 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/name/tutorial001.py
+-rw-r--r--   0        0        0      197 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/name/tutorial001_an.py
+-rw-r--r--   0        0        0      158 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/name/tutorial002.py
+-rw-r--r--   0        0        0      203 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/name/tutorial002_an.py
+-rw-r--r--   0        0        0      148 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/name/tutorial003.py
+-rw-r--r--   0        0        0      193 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/name/tutorial003_an.py
+-rw-r--r--   0        0        0      163 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/name/tutorial004.py
+-rw-r--r--   0        0        0      208 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/name/tutorial004_an.py
+-rw-r--r--   0        0        0      281 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/name/tutorial005.py
+-rw-r--r--   0        0        0      337 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/name/tutorial005_an.py
+-rw-r--r--   0        0        0      212 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/password/tutorial001.py
+-rw-r--r--   0        0        0      262 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/password/tutorial001_an.py
+-rw-r--r--   0        0        0      341 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/password/tutorial002.py
+-rw-r--r--   0        0        0      386 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/password/tutorial002_an.py
+-rw-r--r--   0        0        0      171 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/prompt/tutorial001.py
+-rw-r--r--   0        0        0      216 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/prompt/tutorial001_an.py
+-rw-r--r--   0        0        0      204 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/prompt/tutorial002.py
+-rw-r--r--   0        0        0      254 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/prompt/tutorial002_an.py
+-rw-r--r--   0        0        0      198 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/prompt/tutorial003.py
+-rw-r--r--   0        0        0      249 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/prompt/tutorial003_an.py
+-rw-r--r--   0        0        0      155 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/required/tutorial001.py
+-rw-r--r--   0        0        0      205 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/required/tutorial001_an.py
+-rw-r--r--   0        0        0      166 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/required/tutorial002.py
+-rw-r--r--   0        0        0      430 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/version/tutorial001.py
+-rw-r--r--   0        0        0      494 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/version/tutorial001_an.py
+-rw-r--r--   0        0        0      566 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/version/tutorial002.py
+-rw-r--r--   0        0        0      622 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/version/tutorial002_an.py
+-rw-r--r--   0        0        0      597 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/version/tutorial003.py
+-rw-r--r--   0        0        0      662 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options/version/tutorial003_an.py
+-rw-r--r--   0        0        0      193 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options_autocompletion/tutorial001.py
+-rw-r--r--   0        0        0      244 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options_autocompletion/tutorial001_an.py
+-rw-r--r--   0        0        0      312 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options_autocompletion/tutorial002.py
+-rw-r--r--   0        0        0      364 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options_autocompletion/tutorial002_an.py
+-rw-r--r--   0        0        0      478 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options_autocompletion/tutorial003.py
+-rw-r--r--   0        0        0      530 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options_autocompletion/tutorial003_an.py
+-rw-r--r--   0        0        0      664 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options_autocompletion/tutorial004.py
+-rw-r--r--   0        0        0      716 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options_autocompletion/tutorial004_an.py
+-rw-r--r--   0        0        0      563 2024-03-23 17:07:37.125673 typer-0.9.4/docs_src/options_autocompletion/tutorial005.py
+-rw-r--r--   0        0        0      615 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/options_autocompletion/tutorial005_an.py
+-rw-r--r--   0        0        0      262 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/options_autocompletion/tutorial006.py
+-rw-r--r--   0        0        0      319 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/options_autocompletion/tutorial006_an.py
+-rw-r--r--   0        0        0      699 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/options_autocompletion/tutorial007.py
+-rw-r--r--   0        0        0      760 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/options_autocompletion/tutorial007_an.py
+-rw-r--r--   0        0        0      735 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/options_autocompletion/tutorial008.py
+-rw-r--r--   0        0        0      796 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/options_autocompletion/tutorial008_an.py
+-rw-r--r--   0        0        0      818 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/options_autocompletion/tutorial009.py
+-rw-r--r--   0        0        0      879 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/options_autocompletion/tutorial009_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/bool/__init__.py
+-rw-r--r--   0        0        0      208 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/bool/tutorial001.py
+-rw-r--r--   0        0        0      259 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/bool/tutorial001_an.py
+-rw-r--r--   0        0        0      323 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/bool/tutorial002.py
+-rw-r--r--   0        0        0      374 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/bool/tutorial002_an.py
+-rw-r--r--   0        0        0      228 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/bool/tutorial003.py
+-rw-r--r--   0        0        0      279 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/bool/tutorial003_an.py
+-rw-r--r--   0        0        0      225 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/bool/tutorial004.py
+-rw-r--r--   0        0        0      276 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/bool/tutorial004_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/custom_types/__init__.py
+-rw-r--r--   0        0        0      542 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/custom_types/tutorial001.py
+-rw-r--r--   0        0        0      605 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/custom_types/tutorial001_an.py
+-rw-r--r--   0        0        0      646 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/custom_types/tutorial002.py
+-rw-r--r--   0        0        0      721 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/custom_types/tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/datetime/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/datetime/tutorial001.py
+-rw-r--r--   0        0        0      293 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/datetime/tutorial002.py
+-rw-r--r--   0        0        0      369 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/datetime/tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/enum/__init__.py
+-rw-r--r--   0        0        0      299 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/enum/tutorial001.py
+-rw-r--r--   0        0        0      341 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/enum/tutorial002.py
+-rw-r--r--   0        0        0      406 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/enum/tutorial002_an.py
+-rw-r--r--   0        0        0      349 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/enum/tutorial003.py
+-rw-r--r--   0        0        0      402 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/enum/tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/file/__init__.py
+-rw-r--r--   0        0        0      180 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/file/tutorial001.py
+-rw-r--r--   0        0        0      227 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/file/tutorial001_an.py
+-rw-r--r--   0        0        0      202 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/file/tutorial002.py
+-rw-r--r--   0        0        0      249 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/file/tutorial002_an.py
+-rw-r--r--   0        0        0      321 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/file/tutorial003.py
+-rw-r--r--   0        0        0      368 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/file/tutorial003_an.py
+-rw-r--r--   0        0        0      547 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/file/tutorial004.py
+-rw-r--r--   0        0        0      594 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/file/tutorial004_an.py
+-rw-r--r--   0        0        0      205 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/file/tutorial005.py
+-rw-r--r--   0        0        0      250 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/file/tutorial005_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/index/__init__.py
+-rw-r--r--   0        0        0      394 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/index/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/number/__init__.py
+-rw-r--r--   0        0        0      302 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/number/tutorial001.py
+-rw-r--r--   0        0        0      369 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/number/tutorial001_an.py
+-rw-r--r--   0        0        0      335 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/number/tutorial002.py
+-rw-r--r--   0        0        0      402 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/number/tutorial002_an.py
+-rw-r--r--   0        0        0      178 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/number/tutorial003.py
+-rw-r--r--   0        0        0      229 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/number/tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/path/__init__.py
+-rw-r--r--   0        0        0      530 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/path/tutorial001.py
+-rw-r--r--   0        0        0      583 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/path/tutorial001_an.py
+-rw-r--r--   0        0        0      371 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/path/tutorial002.py
+-rw-r--r--   0        0        0      459 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/path/tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/uuid/__init__.py
+-rw-r--r--   0        0        0      196 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/parameter_types/uuid/tutorial001.py
+-rw-r--r--   0        0        0      296 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/printing/tutorial001.py
+-rw-r--r--   0        0        0      183 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/printing/tutorial002.py
+-rw-r--r--   0        0        0      296 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/printing/tutorial003.py
+-rw-r--r--   0        0        0      214 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/printing/tutorial004.py
+-rw-r--r--   0        0        0      365 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/printing/tutorial005.py
+-rw-r--r--   0        0        0      150 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/printing/tutorial006.py
+-rw-r--r--   0        0        0      315 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/progressbar/tutorial001.py
+-rw-r--r--   0        0        0      476 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/progressbar/tutorial002.py
+-rw-r--r--   0        0        0      313 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/progressbar/tutorial003.py
+-rw-r--r--   0        0        0      455 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/progressbar/tutorial004.py
+-rw-r--r--   0        0        0      333 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/progressbar/tutorial005.py
+-rw-r--r--   0        0        0      336 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/progressbar/tutorial006.py
+-rw-r--r--   0        0        0      162 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/prompt/tutorial001.py
+-rw-r--r--   0        0        0      245 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/prompt/tutorial002.py
+-rw-r--r--   0        0        0      180 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/prompt/tutorial003.py
+-rw-r--r--   0        0        0      193 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/prompt/tutorial004.py
+-rw-r--r--   0        0        0      304 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/callback_override/tutorial001.py
+-rw-r--r--   0        0        0      306 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/callback_override/tutorial002.py
+-rw-r--r--   0        0        0      409 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/callback_override/tutorial003.py
+-rw-r--r--   0        0        0      533 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/callback_override/tutorial004.py
+-rw-r--r--   0        0        0      254 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/name_help/tutorial001.py
+-rw-r--r--   0        0        0      289 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/name_help/tutorial002.py
+-rw-r--r--   0        0        0      282 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/name_help/tutorial003.py
+-rw-r--r--   0        0        0      372 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/name_help/tutorial004.py
+-rw-r--r--   0        0        0      473 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/name_help/tutorial005.py
+-rw-r--r--   0        0        0      514 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/name_help/tutorial006.py
+-rw-r--r--   0        0        0      564 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/name_help/tutorial007.py
+-rw-r--r--   0        0        0      644 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/name_help/tutorial008.py
+-rw-r--r--   0        0        0      298 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/tutorial001/items.py
+-rw-r--r--   0        0        0      177 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/tutorial001/main.py
+-rw-r--r--   0        0        0      245 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/tutorial001/users.py
+-rw-r--r--   0        0        0      698 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/tutorial002/main.py
+-rw-r--r--   0        0        0      298 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/tutorial003/items.py
+-rw-r--r--   0        0        0      180 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/tutorial003/lands.py
+-rw-r--r--   0        0        0      229 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/tutorial003/main.py
+-rw-r--r--   0        0        0      233 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/tutorial003/reigns.py
+-rw-r--r--   0        0        0      221 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/tutorial003/towns.py
+-rw-r--r--   0        0        0      245 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/subcommands/tutorial003/users.py
+-rw-r--r--   0        0        0      598 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/terminating/tutorial001.py
+-rw-r--r--   0        0        0      235 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/terminating/tutorial002.py
+-rw-r--r--   0        0        0      230 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/terminating/tutorial003.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/testing/app01/__init__.py
+-rw-r--r--   0        0        0      256 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/testing/app01/main.py
+-rw-r--r--   0        0        0      299 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/testing/app01/test_main.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/testing/app02/__init__.py
+-rw-r--r--   0        0        0      207 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/testing/app02/main.py
+-rw-r--r--   0        0        0      284 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/testing/app02/test_main.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.129673 typer-0.9.4/docs_src/testing/app02_an/__init__.py
+-rw-r--r--   0        0        0      252 2024-03-23 17:07:37.133673 typer-0.9.4/docs_src/testing/app02_an/main.py
+-rw-r--r--   0        0        0      284 2024-03-23 17:07:37.133673 typer-0.9.4/docs_src/testing/app02_an/test_main.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/docs_src/testing/app03/__init__.py
+-rw-r--r--   0        0        0      122 2024-03-23 17:07:37.133673 typer-0.9.4/docs_src/testing/app03/main.py
+-rw-r--r--   0        0        0      284 2024-03-23 17:07:37.133673 typer-0.9.4/docs_src/testing/app03/test_main.py
+-rw-r--r--   0        0        0      371 2024-03-23 17:07:37.133673 typer-0.9.4/docs_src/using_click/tutorial001.py
+-rw-r--r--   0        0        0      287 2024-03-23 17:07:37.133673 typer-0.9.4/docs_src/using_click/tutorial002.py
+-rw-r--r--   0        0        0      626 2024-03-23 17:07:37.133673 typer-0.9.4/docs_src/using_click/tutorial003.py
+-rw-r--r--   0        0        0      511 2024-03-23 17:07:37.133673 typer-0.9.4/docs_src/using_click/tutorial004.py
+-rw-r--r--   0        0        0       51 2024-03-23 17:07:37.133673 typer-0.9.4/mkdocs.insiders.yml
+-rw-r--r--   0        0        0     5528 2024-03-23 17:07:37.133673 typer-0.9.4/mkdocs.yml
+-rw-r--r--   0        0        0       96 2024-03-23 17:07:37.133673 typer-0.9.4/mypy.ini
+-rw-r--r--   0        0        0     3002 2024-03-23 17:07:37.133673 typer-0.9.4/pyproject.toml
+-rwxr-xr-x   0        0        0       76 2024-03-23 17:07:37.133673 typer-0.9.4/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       98 2024-03-23 17:07:37.133673 typer-0.9.4/scripts/clean.sh
+-rwxr-xr-x   0        0        0       68 2024-03-23 17:07:37.133673 typer-0.9.4/scripts/docs-live.sh
+-rwxr-xr-x   0        0        0      167 2024-03-23 17:07:37.133673 typer-0.9.4/scripts/format-imports.sh
+-rwxr-xr-x   0        0        0      205 2024-03-23 17:07:37.133673 typer-0.9.4/scripts/format.sh
+-rw-r--r--   0        0        0      112 2024-03-23 17:07:37.133673 typer-0.9.4/scripts/get-pwsh-activate.sh
+-rwxr-xr-x   0        0        0      122 2024-03-23 17:07:37.133673 typer-0.9.4/scripts/lint.sh
+-rwxr-xr-x   0        0        0      339 2024-03-23 17:07:37.133673 typer-0.9.4/scripts/netlify-docs.sh
+-rwxr-xr-x   0        0        0       42 2024-03-23 17:07:37.133673 typer-0.9.4/scripts/publish.sh
+-rwxr-xr-x   0        0        0       80 2024-03-23 17:07:37.133673 typer-0.9.4/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0      350 2024-03-23 17:07:37.133673 typer-0.9.4/scripts/test-files.sh
+-rwxr-xr-x   0        0        0      490 2024-03-23 17:07:37.133673 typer-0.9.4/scripts/test.sh
+-rw-r--r--   0        0        0      115 2024-03-23 17:07:37.133673 typer-0.9.4/scripts/zip-docs.sh
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/tests/assets/__init__.py
+-rw-r--r--   0        0        0      675 2024-03-23 17:07:37.133673 typer-0.9.4/tests/assets/compat_click7_8.py
+-rw-r--r--   0        0        0      542 2024-03-23 17:07:37.133673 typer-0.9.4/tests/assets/completion_no_types.py
+-rw-r--r--   0        0        0      542 2024-03-23 17:07:37.133673 typer-0.9.4/tests/assets/completion_no_types_order.py
+-rw-r--r--   0        0        0      160 2024-03-23 17:07:37.133673 typer-0.9.4/tests/assets/prog_name.py
+-rw-r--r--   0        0        0      157 2024-03-23 17:07:37.133673 typer-0.9.4/tests/assets/type_error_no_rich.py
+-rw-r--r--   0        0        0      213 2024-03-23 17:07:37.133673 typer-0.9.4/tests/assets/type_error_no_rich_short_disable.py
+-rw-r--r--   0        0        0      306 2024-03-23 17:07:37.133673 typer-0.9.4/tests/assets/type_error_normal_traceback.py
+-rw-r--r--   0        0        0     6941 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_ambiguous_params.py
+-rw-r--r--   0        0        0     2081 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_annotated.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_compat/__init__.py
+-rw-r--r--   0        0        0     1618 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_compat/test_option_get_help.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_completion/__init__.py
+-rw-r--r--   0        0        0     5328 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_completion/test_completion.py
+-rw-r--r--   0        0        0     5782 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_completion/test_completion_complete.py
+-rw-r--r--   0        0        0     2209 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_completion/test_completion_complete_no_help.py
+-rw-r--r--   0        0        0     5943 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_completion/test_completion_install.py
+-rw-r--r--   0        0        0     3891 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_completion/test_completion_show.py
+-rw-r--r--   0        0        0      797 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_exit_errors.py
+-rw-r--r--   0        0        0     8120 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_others.py
+-rw-r--r--   0        0        0      410 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_prog_name.py
+-rw-r--r--   0        0        0      849 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_rich_utils.py
+-rw-r--r--   0        0        0     2556 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tracebacks.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_default/__init__.py
+-rw-r--r--   0        0        0      980 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py
+-rw-r--r--   0        0        0      998 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_default/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1105 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py
+-rw-r--r--   0        0        0     1108 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_default/test_tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_envvar/__init__.py
+-rw-r--r--   0        0        0     1654 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py
+-rw-r--r--   0        0        0     1657 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1250 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py
+-rw-r--r--   0        0        0     1253 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002_an.py
+-rw-r--r--   0        0        0     1271 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py
+-rw-r--r--   0        0        0     1274 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/__init__.py
+-rw-r--r--   0        0        0     1343 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py
+-rw-r--r--   0        0        0     1346 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial001_an.py
+-rw-r--r--   0        0        0      988 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py
+-rw-r--r--   0        0        0      991 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial002_an.py
+-rw-r--r--   0        0        0      979 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py
+-rw-r--r--   0        0        0      982 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial003_an.py
+-rw-r--r--   0        0        0      983 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py
+-rw-r--r--   0        0        0      986 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial004_an.py
+-rw-r--r--   0        0        0      901 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py
+-rw-r--r--   0        0        0      904 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial005_an.py
+-rw-r--r--   0        0        0      885 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py
+-rw-r--r--   0        0        0      888 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial006_an.py
+-rw-r--r--   0        0        0      875 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py
+-rw-r--r--   0        0        0      878 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial007_an.py
+-rw-r--r--   0        0        0     1323 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py
+-rw-r--r--   0        0        0     1326 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial008_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_optional/__init__.py
+-rw-r--r--   0        0        0     1188 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py
+-rw-r--r--   0        0        0     1191 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_optional/test_tutorial001_an.py
+-rw-r--r--   0        0        0      883 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py
+-rw-r--r--   0        0        0      886 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_optional/test_tutorial002_an.py
+-rw-r--r--   0        0        0     1188 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_arguments/test_optional/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_commands/test_arguments/__init__.py
+-rw-r--r--   0        0        0     1078 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_commands/test_callback/__init__.py
+-rw-r--r--   0        0        0     2333 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py
+-rw-r--r--   0        0        0      624 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py
+-rw-r--r--   0        0        0      741 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py
+-rw-r--r--   0        0        0      864 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_commands/test_context/__init__.py
+-rw-r--r--   0        0        0      864 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_commands/test_context/test_tutorial001.py
+-rw-r--r--   0        0        0      982 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_commands/test_context/test_tutorial002.py
+-rw-r--r--   0        0        0      990 2024-03-23 17:07:37.133673 typer-0.9.4/tests/test_tutorial/test_commands/test_context/test_tutorial003.py
+-rw-r--r--   0        0        0      749 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_context/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_help/__init__.py
+-rw-r--r--   0        0        0     4223 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial001.py
+-rw-r--r--   0        0        0     4226 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1679 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial002.py
+-rw-r--r--   0        0        0     1138 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial003.py
+-rw-r--r--   0        0        0     1839 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial004.py
+-rw-r--r--   0        0        0     1844 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial004_an.py
+-rw-r--r--   0        0        0     1906 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial005.py
+-rw-r--r--   0        0        0     1911 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial005_an.py
+-rw-r--r--   0        0        0     1610 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial006.py
+-rw-r--r--   0        0        0     1707 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial007.py
+-rw-r--r--   0        0        0     1710 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial007_an.py
+-rw-r--r--   0        0        0      743 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial008.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_index/__init__.py
+-rw-r--r--   0        0        0      695 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_index/test_tutorial001.py
+-rw-r--r--   0        0        0      993 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_index/test_tutorial002.py
+-rw-r--r--   0        0        0      983 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_index/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_name/__init__.py
+-rw-r--r--   0        0        0      944 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_name/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_one_or_multiple/__init__.py
+-rw-r--r--   0        0        0      754 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py
+-rw-r--r--   0        0        0      898 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_options/__init__.py
+-rw-r--r--   0        0        0     3052 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_options/test_tutorial001.py
+-rw-r--r--   0        0        0     3055 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_commands/test_options/test_tutorial001_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_exceptions/__init__.py
+-rw-r--r--   0        0        0     1963 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_exceptions/test_tutorial001.py
+-rw-r--r--   0        0        0     1975 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_exceptions/test_tutorial002.py
+-rw-r--r--   0        0        0     1200 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_exceptions/test_tutorial003.py
+-rw-r--r--   0        0        0     1145 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_exceptions/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_first_steps/__init__.py
+-rw-r--r--   0        0        0      561 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_first_steps/test_tutorial001.py
+-rw-r--r--   0        0        0      731 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_first_steps/test_tutorial002.py
+-rw-r--r--   0        0        0      768 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_first_steps/test_tutorial003.py
+-rw-r--r--   0        0        0     1554 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_first_steps/test_tutorial004.py
+-rw-r--r--   0        0        0     1543 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_first_steps/test_tutorial005.py
+-rw-r--r--   0        0        0     1419 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_first_steps/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_multiple_values/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/__init__.py
+-rw-r--r--   0        0        0      757 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py
+-rw-r--r--   0        0        0     1512 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py
+-rw-r--r--   0        0        0     1524 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_multiple_values/test_multiple_options/__init__.py
+-rw-r--r--   0        0        0     1126 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py
+-rw-r--r--   0        0        0     1129 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001_an.py
+-rw-r--r--   0        0        0      943 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py
+-rw-r--r--   0        0        0      946 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/__init__.py
+-rw-r--r--   0        0        0     1466 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py
+-rw-r--r--   0        0        0     1469 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_callback/__init__.py
+-rw-r--r--   0        0        0      789 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_callback/test_tutorial001.py
+-rw-r--r--   0        0        0      792 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_callback/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1335 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_callback/test_tutorial003.py
+-rw-r--r--   0        0        0     1344 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_callback/test_tutorial003_an.py
+-rw-r--r--   0        0        0     1342 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_callback/test_tutorial004.py
+-rw-r--r--   0        0        0     1351 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_callback/test_tutorial004_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_help/__init__.py
+-rw-r--r--   0        0        0     1334 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_help/test_tutorial001.py
+-rw-r--r--   0        0        0     1337 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_help/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1103 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_help/test_tutorial002.py
+-rw-r--r--   0        0        0     1106 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_help/test_tutorial002_an.py
+-rw-r--r--   0        0        0      818 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_help/test_tutorial003.py
+-rw-r--r--   0        0        0      821 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_help/test_tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_name/__init__.py
+-rw-r--r--   0        0        0     1138 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial001.py
+-rw-r--r--   0        0        0     1141 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1010 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial002.py
+-rw-r--r--   0        0        0     1013 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial002_an.py
+-rw-r--r--   0        0        0      860 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial003.py
+-rw-r--r--   0        0        0      863 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial003_an.py
+-rw-r--r--   0        0        0     1015 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial004.py
+-rw-r--r--   0        0        0     1018 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial004_an.py
+-rw-r--r--   0        0        0     1344 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial005.py
+-rw-r--r--   0        0        0     1347 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial005_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_prompt/__init__.py
+-rw-r--r--   0        0        0     1090 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py
+-rw-r--r--   0        0        0     1093 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_prompt/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1111 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py
+-rw-r--r--   0        0        0     1114 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_prompt/test_tutorial002_an.py
+-rw-r--r--   0        0        0     1537 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py
+-rw-r--r--   0        0        0     1540 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_prompt/test_tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_required/__init__.py
+-rw-r--r--   0        0        0     1335 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_required/test_tutorial001.py
+-rw-r--r--   0        0        0     1338 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_required/test_tutorial001_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_version/__init__.py
+-rw-r--r--   0        0        0     1475 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_version/test_tutorial003.py
+-rw-r--r--   0        0        0     1484 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options/test_version/test_tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options_autocompletion/__init__.py
+-rw-r--r--   0        0        0     1119 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial002.py
+-rw-r--r--   0        0        0     1128 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial002_an.py
+-rw-r--r--   0        0        0     1130 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial003.py
+-rw-r--r--   0        0        0     1139 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial003_an.py
+-rw-r--r--   0        0        0     1199 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial004.py
+-rw-r--r--   0        0        0     1208 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial004_an.py
+-rw-r--r--   0        0        0     1285 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial007.py
+-rw-r--r--   0        0        0     1294 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial007_an.py
+-rw-r--r--   0        0        0     1389 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial008.py
+-rw-r--r--   0        0        0     1398 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial008_an.py
+-rw-r--r--   0        0        0     1433 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial009.py
+-rw-r--r--   0        0        0     1442 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial009_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_parameter_types/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/__init__.py
+-rw-r--r--   0        0        0     1222 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py
+-rw-r--r--   0        0        0     1225 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1745 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py
+-rw-r--r--   0        0        0     1748 2024-03-23 17:07:37.137673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002_an.py
+-rw-r--r--   0        0        0      985 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py
+-rw-r--r--   0        0        0      988 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003_an.py
+-rw-r--r--   0        0        0     1047 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py
+-rw-r--r--   0        0        0     1050 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_custom_types/__init__.py
+-rw-r--r--   0        0        0     1017 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001.py
+-rw-r--r--   0        0        0     1024 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1027 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002.py
+-rw-r--r--   0        0        0     1030 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_datetime/__init__.py
+-rw-r--r--   0        0        0     1471 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py
+-rw-r--r--   0        0        0      824 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py
+-rw-r--r--   0        0        0      827 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_enum/__init__.py
+-rw-r--r--   0        0        0     1849 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py
+-rw-r--r--   0        0        0      815 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py
+-rw-r--r--   0        0        0      818 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002_an.py
+-rw-r--r--   0        0        0     1238 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003.py
+-rw-r--r--   0        0        0     1241 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/__init__.py
+-rw-r--r--   0        0        0      866 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py
+-rw-r--r--   0        0        0      869 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001_an.py
+-rw-r--r--   0        0        0      892 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py
+-rw-r--r--   0        0        0      895 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002_an.py
+-rw-r--r--   0        0        0      811 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py
+-rw-r--r--   0        0        0      814 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003_an.py
+-rw-r--r--   0        0        0      926 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py
+-rw-r--r--   0        0        0      929 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004_an.py
+-rw-r--r--   0        0        0     1080 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py
+-rw-r--r--   0        0        0     1083 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_index/__init__.py
+-rw-r--r--   0        0        0     1534 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_number/__init__.py
+-rw-r--r--   0        0        0     2816 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py
+-rw-r--r--   0        0        0     2819 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1091 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py
+-rw-r--r--   0        0        0     1094 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002_an.py
+-rw-r--r--   0        0        0     1412 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py
+-rw-r--r--   0        0        0     1415 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_path/__init__.py
+-rw-r--r--   0        0        0     1495 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py
+-rw-r--r--   0        0        0     1498 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1345 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py
+-rw-r--r--   0        0        0     1348 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_uuid/__init__.py
+-rw-r--r--   0        0        0     1139 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_prompt/__init__.py
+-rw-r--r--   0        0        0      644 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_prompt/test_tutorial001.py
+-rw-r--r--   0        0        0      920 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_prompt/test_tutorial002.py
+-rw-r--r--   0        0        0      877 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_prompt/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_callback_override/__init__.py
+-rw-r--r--   0        0        0      651 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py
+-rw-r--r--   0        0        0      651 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py
+-rw-r--r--   0        0        0      780 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py
+-rw-r--r--   0        0        0      882 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/__init__.py
+-rw-r--r--   0        0        0      987 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py
+-rw-r--r--   0        0        0      987 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py
+-rw-r--r--   0        0        0      987 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py
+-rw-r--r--   0        0        0      987 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py
+-rw-r--r--   0        0        0     1029 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py
+-rw-r--r--   0        0        0      979 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py
+-rw-r--r--   0        0        0     1012 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py
+-rw-r--r--   0        0        0     1025 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py
+-rw-r--r--   0        0        0     2726 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_tutorial001.py
+-rw-r--r--   0        0        0     2178 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_tutorial002.py
+-rw-r--r--   0        0        0     5668 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_subcommands/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_terminating/__init__.py
+-rw-r--r--   0        0        0     1168 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_terminating/test_tutorial001.py
+-rw-r--r--   0        0        0      756 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_terminating/test_tutorial002.py
+-rw-r--r--   0        0        0     1273 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_terminating/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_testing/__init__.py
+-rw-r--r--   0        0        0      423 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_testing/test_app01.py
+-rw-r--r--   0        0        0      423 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_testing/test_app02.py
+-rw-r--r--   0        0        0      432 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_testing/test_app02_an.py
+-rw-r--r--   0        0        0      423 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_testing/test_app03.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_using_click/__init__.py
+-rw-r--r--   0        0        0     1118 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_using_click/test_tutorial003.py
+-rw-r--r--   0        0        0      971 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_tutorial/test_using_click/test_tutorial004.py
+-rw-r--r--   0        0        0     3316 2024-03-23 17:07:37.141673 typer-0.9.4/tests/test_type_conversion.py
+-rw-r--r--   0        0        0      125 2024-03-23 17:07:37.141673 typer-0.9.4/tests/utils.py
+-rw-r--r--   0        0        0     1602 2024-03-23 17:07:37.141673 typer-0.9.4/typer/__init__.py
+-rw-r--r--   0        0        0       94 2024-03-23 17:07:37.141673 typer-0.9.4/typer/_compat_utils.py
+-rw-r--r--   0        0        0     4957 2024-03-23 17:07:37.141673 typer-0.9.4/typer/_completion_click7.py
+-rw-r--r--   0        0        0     6688 2024-03-23 17:07:37.141673 typer-0.9.4/typer/_completion_click8.py
+-rw-r--r--   0        0        0     8541 2024-03-23 17:07:37.141673 typer-0.9.4/typer/_completion_shared.py
+-rw-r--r--   0        0        0    19713 2024-03-23 17:07:37.141673 typer-0.9.4/typer/_typing.py
+-rw-r--r--   0        0        0      430 2024-03-23 17:07:37.141673 typer-0.9.4/typer/colors.py
+-rw-r--r--   0        0        0     4999 2024-03-23 17:07:37.141673 typer-0.9.4/typer/completion.py
+-rw-r--r--   0        0        0    26715 2024-03-23 17:07:37.141673 typer-0.9.4/typer/core.py
+-rw-r--r--   0        0        0    39286 2024-03-23 17:07:37.141673 typer-0.9.4/typer/main.py
+-rw-r--r--   0        0        0    15993 2024-03-23 17:07:37.141673 typer-0.9.4/typer/models.py
+-rw-r--r--   0        0        0    13787 2024-03-23 17:07:37.141673 typer-0.9.4/typer/params.py
+-rw-r--r--   0        0        0        0 2024-03-23 17:07:37.141673 typer-0.9.4/typer/py.typed
+-rw-r--r--   0        0        0    23714 2024-03-23 17:07:37.145673 typer-0.9.4/typer/rich_utils.py
+-rw-r--r--   0        0        0      874 2024-03-23 17:07:37.145673 typer-0.9.4/typer/testing.py
+-rw-r--r--   0        0        0     7414 2024-03-23 17:07:37.145673 typer-0.9.4/typer/utils.py
+-rw-r--r--   0        0        0    14615 1970-01-01 00:00:00.000000 typer-0.9.4/PKG-INFO
```

### Comparing `typer-0.9.3/.github/DISCUSSION_TEMPLATE/questions.yml` & `typer-0.9.4/.github/DISCUSSION_TEMPLATE/questions.yml`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/.github/ISSUE_TEMPLATE/config.yml` & `typer-0.9.4/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/.github/ISSUE_TEMPLATE/privileged.yml` & `typer-0.9.4/.github/ISSUE_TEMPLATE/privileged.yml`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/.github/actions/comment-docs-preview-in-pr/app/main.py` & `typer-0.9.4/.github/actions/comment-docs-preview-in-pr/app/main.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/.github/workflows/build-docs.yml` & `typer-0.9.4/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/.github/workflows/deploy-docs.yml` & `typer-0.9.4/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/.github/workflows/issue-manager.yml` & `typer-0.9.4/.github/workflows/issue-manager.yml`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/.github/workflows/latest-changes.yml` & `typer-0.9.4/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/.github/workflows/publish.yml` & `typer-0.9.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/.github/workflows/smokeshow.yml` & `typer-0.9.4/.github/workflows/smokeshow.yml`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/.github/workflows/test.yml` & `typer-0.9.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/.pre-commit-config.yaml` & `typer-0.9.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/CITATION.cff` & `typer-0.9.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/LICENSE` & `typer-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/README.md` & `typer-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/SECURITY.md` & `typer-0.9.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/alternatives.md` & `typer-0.9.4/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/contributing.md` & `typer-0.9.4/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/css/termynal.css` & `typer-0.9.4/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/features.md` & `typer-0.9.4/docs/features.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/help-typer.md` & `typer-0.9.4/docs/help-typer.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/img/github-social-preview.png` & `typer-0.9.4/docs/img/github-social-preview.png`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/img/github-social-preview.svg` & `typer-0.9.4/docs/img/github-social-preview.svg`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/img/icon-white.svg` & `typer-0.9.4/docs/img/icon-white.svg`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/img/logo-margin/logo-margin-vector.svg` & `typer-0.9.4/docs/img/logo-margin/logo-margin-vector.svg`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/img/logo-margin/logo-margin.svg` & `typer-0.9.4/docs/img/logo-margin/logo-margin.svg`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/img/pycharm-completion.png` & `typer-0.9.4/docs/img/pycharm-completion.png`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/img/vscode-completion.png` & `typer-0.9.4/docs/img/vscode-completion.png`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/index.md` & `typer-0.9.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/js/custom.js` & `typer-0.9.4/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/js/termynal.js` & `typer-0.9.4/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/release-notes.md` & `typer-0.9.4/docs/release-notes.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 ## Latest Changes
 
+### 0.9.4
+
+### Features
+
+* ✨ Improve support for CLI translations using gettext. PR [#417](https://github.com/tiangolo/typer/pull/417) by [@mjodmj](https://github.com/mjodmj).
+
 ## 0.9.3
 
 ### Fixes
 
 * 🐛 Fix evaluating stringified annotations in Python 3.10 (also `from __future__ import annotations`). PR [#721](https://github.com/tiangolo/typer/pull/721) by [@heckad](https://github.com/heckad).
 
 ## 0.9.2
```

### Comparing `typer-0.9.3/docs/tutorial/app-dir.md` & `typer-0.9.4/docs/tutorial/app-dir.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/arguments/default.md` & `typer-0.9.4/docs/tutorial/arguments/default.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/arguments/envvar.md` & `typer-0.9.4/docs/tutorial/arguments/envvar.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/arguments/help.md` & `typer-0.9.4/docs/tutorial/arguments/help.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/arguments/optional.md` & `typer-0.9.4/docs/tutorial/arguments/optional.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/commands/arguments.md` & `typer-0.9.4/docs/tutorial/commands/arguments.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/commands/callback.md` & `typer-0.9.4/docs/tutorial/commands/callback.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/commands/context.md` & `typer-0.9.4/docs/tutorial/commands/context.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/commands/help.md` & `typer-0.9.4/docs/tutorial/commands/help.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/commands/index.md` & `typer-0.9.4/docs/tutorial/commands/index.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/commands/name.md` & `typer-0.9.4/docs/tutorial/commands/name.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/commands/one-or-multiple.md` & `typer-0.9.4/docs/tutorial/commands/one-or-multiple.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/commands/options.md` & `typer-0.9.4/docs/tutorial/commands/options.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/exceptions.md` & `typer-0.9.4/docs/tutorial/exceptions.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/first-steps.md` & `typer-0.9.4/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/index.md` & `typer-0.9.4/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/launch.md` & `typer-0.9.4/docs/tutorial/launch.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/multiple-values/arguments-with-multiple-values.md` & `typer-0.9.4/docs/tutorial/multiple-values/arguments-with-multiple-values.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/multiple-values/multiple-options.md` & `typer-0.9.4/docs/tutorial/multiple-values/multiple-options.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/multiple-values/options-with-multiple-values.md` & `typer-0.9.4/docs/tutorial/multiple-values/options-with-multiple-values.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/options-autocompletion.md` & `typer-0.9.4/docs/tutorial/options-autocompletion.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/options/callback-and-context.md` & `typer-0.9.4/docs/tutorial/options/callback-and-context.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/options/help.md` & `typer-0.9.4/docs/tutorial/options/help.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/options/name.md` & `typer-0.9.4/docs/tutorial/options/name.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/options/password.md` & `typer-0.9.4/docs/tutorial/options/password.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/options/prompt.md` & `typer-0.9.4/docs/tutorial/options/prompt.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/options/required.md` & `typer-0.9.4/docs/tutorial/options/required.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/options/version.md` & `typer-0.9.4/docs/tutorial/options/version.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/package.md` & `typer-0.9.4/docs/tutorial/package.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/parameter-types/bool.md` & `typer-0.9.4/docs/tutorial/parameter-types/bool.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/parameter-types/custom-types.md` & `typer-0.9.4/docs/tutorial/parameter-types/custom-types.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/parameter-types/datetime.md` & `typer-0.9.4/docs/tutorial/parameter-types/datetime.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/parameter-types/enum.md` & `typer-0.9.4/docs/tutorial/parameter-types/enum.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/parameter-types/file.md` & `typer-0.9.4/docs/tutorial/parameter-types/file.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/parameter-types/index.md` & `typer-0.9.4/docs/tutorial/parameter-types/index.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/parameter-types/number.md` & `typer-0.9.4/docs/tutorial/parameter-types/number.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/parameter-types/path.md` & `typer-0.9.4/docs/tutorial/parameter-types/path.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/parameter-types/uuid.md` & `typer-0.9.4/docs/tutorial/parameter-types/uuid.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/printing.md` & `typer-0.9.4/docs/tutorial/printing.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/progressbar.md` & `typer-0.9.4/docs/tutorial/progressbar.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/prompt.md` & `typer-0.9.4/docs/tutorial/prompt.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/subcommands/add-typer.md` & `typer-0.9.4/docs/tutorial/subcommands/add-typer.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/subcommands/callback-override.md` & `typer-0.9.4/docs/tutorial/subcommands/callback-override.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/subcommands/index.md` & `typer-0.9.4/docs/tutorial/subcommands/index.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/subcommands/name-and-help.md` & `typer-0.9.4/docs/tutorial/subcommands/name-and-help.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/subcommands/nested-subcommands.md` & `typer-0.9.4/docs/tutorial/subcommands/nested-subcommands.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/subcommands/single-file.md` & `typer-0.9.4/docs/tutorial/subcommands/single-file.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/terminating.md` & `typer-0.9.4/docs/tutorial/terminating.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/testing.md` & `typer-0.9.4/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/tutorial/using-click.md` & `typer-0.9.4/docs/tutorial/using-click.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs/typer-cli.md` & `typer-0.9.4/docs/typer-cli.md`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/arguments/help/tutorial007_an.py` & `typer-0.9.4/docs_src/arguments/help/tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/commands/callback/tutorial001.py` & `typer-0.9.4/docs_src/commands/callback/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/commands/help/tutorial001.py` & `typer-0.9.4/docs_src/commands/help/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/commands/help/tutorial001_an.py` & `typer-0.9.4/docs_src/commands/help/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/commands/help/tutorial004.py` & `typer-0.9.4/docs_src/commands/help/tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/commands/help/tutorial004_an.py` & `typer-0.9.4/docs_src/commands/help/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/commands/help/tutorial005.py` & `typer-0.9.4/docs_src/commands/help/tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/commands/help/tutorial005_an.py` & `typer-0.9.4/docs_src/commands/help/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/commands/help/tutorial006.py` & `typer-0.9.4/docs_src/commands/help/tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/commands/help/tutorial007.py` & `typer-0.9.4/docs_src/commands/help/tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/commands/help/tutorial007_an.py` & `typer-0.9.4/docs_src/commands/help/tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/commands/options/tutorial001.py` & `typer-0.9.4/docs_src/commands/options/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/commands/options/tutorial001_an.py` & `typer-0.9.4/docs_src/commands/options/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/launch/tutorial002.py` & `typer-0.9.4/docs_src/launch/tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options/help/tutorial001_an.py` & `typer-0.9.4/docs_src/options/help/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options/help/tutorial002.py` & `typer-0.9.4/docs_src/options/help/tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options/help/tutorial002_an.py` & `typer-0.9.4/docs_src/options/help/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options/version/tutorial002.py` & `typer-0.9.4/docs_src/options/version/tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options/version/tutorial002_an.py` & `typer-0.9.4/docs_src/options/version/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options/version/tutorial003.py` & `typer-0.9.4/docs_src/options/version/tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options/version/tutorial003_an.py` & `typer-0.9.4/docs_src/options/version/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options_autocompletion/tutorial003_an.py` & `typer-0.9.4/docs_src/options_autocompletion/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options_autocompletion/tutorial004.py` & `typer-0.9.4/docs_src/options_autocompletion/tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options_autocompletion/tutorial004_an.py` & `typer-0.9.4/docs_src/options_autocompletion/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options_autocompletion/tutorial005.py` & `typer-0.9.4/docs_src/options_autocompletion/tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options_autocompletion/tutorial005_an.py` & `typer-0.9.4/docs_src/options_autocompletion/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options_autocompletion/tutorial007.py` & `typer-0.9.4/docs_src/options_autocompletion/tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options_autocompletion/tutorial007_an.py` & `typer-0.9.4/docs_src/options_autocompletion/tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options_autocompletion/tutorial008.py` & `typer-0.9.4/docs_src/options_autocompletion/tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options_autocompletion/tutorial008_an.py` & `typer-0.9.4/docs_src/options_autocompletion/tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options_autocompletion/tutorial009.py` & `typer-0.9.4/docs_src/options_autocompletion/tutorial009.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/options_autocompletion/tutorial009_an.py` & `typer-0.9.4/docs_src/options_autocompletion/tutorial009_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/parameter_types/custom_types/tutorial001.py` & `typer-0.9.4/docs_src/parameter_types/custom_types/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/parameter_types/custom_types/tutorial001_an.py` & `typer-0.9.4/docs_src/parameter_types/custom_types/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/parameter_types/custom_types/tutorial002.py` & `typer-0.9.4/docs_src/parameter_types/custom_types/tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/parameter_types/custom_types/tutorial002_an.py` & `typer-0.9.4/docs_src/parameter_types/custom_types/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/parameter_types/file/tutorial004.py` & `typer-0.9.4/docs_src/parameter_types/file/tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/parameter_types/file/tutorial004_an.py` & `typer-0.9.4/docs_src/parameter_types/file/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/parameter_types/path/tutorial001.py` & `typer-0.9.4/docs_src/parameter_types/path/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/parameter_types/path/tutorial001_an.py` & `typer-0.9.4/docs_src/parameter_types/path/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/subcommands/callback_override/tutorial004.py` & `typer-0.9.4/docs_src/subcommands/callback_override/tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/subcommands/name_help/tutorial006.py` & `typer-0.9.4/docs_src/subcommands/name_help/tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/subcommands/name_help/tutorial007.py` & `typer-0.9.4/docs_src/subcommands/name_help/tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/subcommands/name_help/tutorial008.py` & `typer-0.9.4/docs_src/subcommands/name_help/tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/subcommands/tutorial002/main.py` & `typer-0.9.4/docs_src/subcommands/tutorial002/main.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/terminating/tutorial001.py` & `typer-0.9.4/docs_src/terminating/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/docs_src/using_click/tutorial003.py` & `typer-0.9.4/docs_src/using_click/tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/mkdocs.yml` & `typer-0.9.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/pyproject.toml` & `typer-0.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/assets/compat_click7_8.py` & `typer-0.9.4/tests/assets/compat_click7_8.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/assets/completion_no_types.py` & `typer-0.9.4/tests/assets/completion_no_types.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/assets/completion_no_types_order.py` & `typer-0.9.4/tests/assets/completion_no_types_order.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_ambiguous_params.py` & `typer-0.9.4/tests/test_ambiguous_params.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_annotated.py` & `typer-0.9.4/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_compat/test_option_get_help.py` & `typer-0.9.4/tests/test_compat/test_option_get_help.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_completion/test_completion.py` & `typer-0.9.4/tests/test_completion/test_completion.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_completion/test_completion_complete.py` & `typer-0.9.4/tests/test_completion/test_completion_complete.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_completion/test_completion_complete_no_help.py` & `typer-0.9.4/tests/test_completion/test_completion_complete_no_help.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_completion/test_completion_install.py` & `typer-0.9.4/tests/test_completion/test_completion_install.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_completion/test_completion_show.py` & `typer-0.9.4/tests/test_completion/test_completion_show.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_exit_errors.py` & `typer-0.9.4/tests/test_exit_errors.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_others.py` & `typer-0.9.4/tests/test_others.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_rich_utils.py` & `typer-0.9.4/tests/test_rich_utils.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tracebacks.py` & `typer-0.9.4/tests/test_tracebacks.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_default/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_default/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_default/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_default/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial003_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial004_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial005_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial006_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial007_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_help/test_tutorial008_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_help/test_tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_optional/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_optional/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_optional/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_optional/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_arguments/test_optional/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_arguments/test_optional/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_context/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_context/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_context/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_context/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_context/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_context/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_context/test_tutorial004.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_context/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial004.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial004_an.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial005.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial005_an.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial006.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial007.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial007_an.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_help/test_tutorial008.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_help/test_tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_index/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_index/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_index/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_index/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_index/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_index/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_name/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_name/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_options/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_options/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_commands/test_options/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_commands/test_options/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_exceptions/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_exceptions/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_exceptions/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_exceptions/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_exceptions/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_exceptions/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_exceptions/test_tutorial004.py` & `typer-0.9.4/tests/test_tutorial/test_exceptions/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_first_steps/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_first_steps/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_first_steps/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_first_steps/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_first_steps/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_first_steps/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_first_steps/test_tutorial004.py` & `typer-0.9.4/tests/test_tutorial/test_first_steps/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_first_steps/test_tutorial005.py` & `typer-0.9.4/tests/test_tutorial/test_first_steps/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_first_steps/test_tutorial006.py` & `typer-0.9.4/tests/test_tutorial/test_first_steps/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_callback/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_callback/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_callback/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_callback/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_callback/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_callback/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_callback/test_tutorial003_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_callback/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_callback/test_tutorial004.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_callback/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_callback/test_tutorial004_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_callback/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_help/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_help/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_help/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_help/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_help/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_help/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_help/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_help/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_help/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_help/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_help/test_tutorial003_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_help/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial003_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial004.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial004_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial005.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_name/test_tutorial005_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_name/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_prompt/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_prompt/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_prompt/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_prompt/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_prompt/test_tutorial003_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_prompt/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_required/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_required/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_required/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_required/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_version/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_version/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options/test_version/test_tutorial003_an.py` & `typer-0.9.4/tests/test_tutorial/test_options/test_version/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial003_an.py` & `typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial004.py` & `typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial004_an.py` & `typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial007.py` & `typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial007_an.py` & `typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial008.py` & `typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial008_an.py` & `typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial009.py` & `typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial009.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_options_autocompletion/test_tutorial009_an.py` & `typer-0.9.4/tests/test_tutorial/test_options_autocompletion/test_tutorial009_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002_an.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_prompt/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_prompt/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_prompt/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_prompt/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_prompt/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_prompt/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_subcommands/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_subcommands/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_terminating/test_tutorial001.py` & `typer-0.9.4/tests/test_tutorial/test_terminating/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_terminating/test_tutorial002.py` & `typer-0.9.4/tests/test_tutorial/test_terminating/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_terminating/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_terminating/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_using_click/test_tutorial003.py` & `typer-0.9.4/tests/test_tutorial/test_using_click/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_tutorial/test_using_click/test_tutorial004.py` & `typer-0.9.4/tests/test_tutorial/test_using_click/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/tests/test_type_conversion.py` & `typer-0.9.4/tests/test_type_conversion.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/typer/__init__.py` & `typer-0.9.4/typer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Typer, build great CLIs. Easy to code. Based on Python type hints."""
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 
 from shutil import get_terminal_size as get_terminal_size
 
 from click.exceptions import Abort as Abort
 from click.exceptions import BadParameter as BadParameter
 from click.exceptions import Exit as Exit
 from click.termui import clear as clear
```

### Comparing `typer-0.9.3/typer/_completion_click7.py` & `typer-0.9.4/typer/_completion_click7.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/typer/_completion_click8.py` & `typer-0.9.4/typer/_completion_click8.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/typer/_completion_shared.py` & `typer-0.9.4/typer/_completion_shared.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/typer/_typing.py` & `typer-0.9.4/typer/_typing.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/typer/completion.py` & `typer-0.9.4/typer/completion.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/typer/core.py` & `typer-0.9.4/typer/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     ctx.resilient_parsing = True
 
     try:
         if _get_click_major() > 7:
             default_value = obj.get_default(ctx, call=False)
         else:
             if inspect.isfunction(obj.default):
-                default_value = "(dynamic)"
+                default_value = _("(dynamic)")
             else:
                 default_value = obj.default
     finally:
         ctx.resilient_parsing = resilient
     return default_value
 
 
@@ -392,15 +392,15 @@
                 show_default_is_str=show_default_is_str,
                 default_value=default_value,
             )
             # Typer override end
             if default_string:
                 extra.append(_("default: {default}").format(default=default_string))
         if self.required:
-            extra.append("required")
+            extra.append(_("required"))
         if extra:
             extra_str = ";".join(extra)
             help = f"{help}  [{extra_str}]" if help else f"[{extra_str}]"
         return name, help
 
     def make_metavar(self) -> str:
         # Modified version of click.core.Argument.make_metavar()
@@ -624,23 +624,19 @@
         rv = param.get_help_record(ctx)
         if rv is not None:
             if param.param_type_name == "argument":
                 args.append(rv)
             elif param.param_type_name == "option":
                 opts.append(rv)
 
-    # TODO: explore adding Click's gettext support, e.g.:
-    # from gettext import gettext as _
-    # with formatter.section(_("Options")):
-    #     ...
     if args:
-        with formatter.section("Arguments"):
+        with formatter.section(_("Arguments")):
             formatter.write_dl(args)
     if opts:
-        with formatter.section("Options"):
+        with formatter.section(_("Options")):
             formatter.write_dl(opts)
 
 
 def _typer_main_shell_completion(
     self: click.core.Command,
     *,
     ctx_args: MutableMapping[str, Any],
```

### Comparing `typer-0.9.3/typer/main.py` & `typer-0.9.4/typer/main.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/typer/models.py` & `typer-0.9.4/typer/models.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/typer/params.py` & `typer-0.9.4/typer/params.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/typer/rich_utils.py` & `typer-0.9.4/typer/rich_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Extracted and modified from https://github.com/ewels/rich-click
 
 import inspect
 import sys
 from collections import defaultdict
+from gettext import gettext as _
 from os import getenv
 from typing import Any, DefaultDict, Dict, Iterable, List, Optional, Union
 
 import click
 from rich import box
 from rich.align import Align
 from rich.columns import Columns
@@ -76,25 +77,25 @@
     if getenv("GITHUB_ACTIONS") or getenv("FORCE_COLOR") or getenv("PY_COLORS")
     else None
 )
 if _TYPER_FORCE_DISABLE_TERMINAL:
     FORCE_TERMINAL = False
 
 # Fixed strings
-DEPRECATED_STRING = "(deprecated) "
-DEFAULT_STRING = "[default: {}]"
-ENVVAR_STRING = "[env var: {}]"
+DEPRECATED_STRING = _("(deprecated) ")
+DEFAULT_STRING = _("[default: {}]")
+ENVVAR_STRING = _("[env var: {}]")
 REQUIRED_SHORT_STRING = "*"
-REQUIRED_LONG_STRING = "[required]"
+REQUIRED_LONG_STRING = _("[required]")
 RANGE_STRING = " [{}]"
-ARGUMENTS_PANEL_TITLE = "Arguments"
-OPTIONS_PANEL_TITLE = "Options"
-COMMANDS_PANEL_TITLE = "Commands"
-ERRORS_PANEL_TITLE = "Error"
-ABORTED_TEXT = "Aborted."
+ARGUMENTS_PANEL_TITLE = _("Arguments")
+OPTIONS_PANEL_TITLE = _("Options")
+COMMANDS_PANEL_TITLE = _("Commands")
+ERRORS_PANEL_TITLE = _("Error")
+ABORTED_TEXT = _("Aborted.")
 
 MARKUP_MODE_MARKDOWN = "markdown"
 MARKUP_MODE_RICH = "rich"
 _RICH_HELP_PANEL_NAME = "rich_help_panel"
 
 MarkupMode = Literal["markdown", "rich", None]
```

### Comparing `typer-0.9.3/typer/testing.py` & `typer-0.9.4/typer/testing.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/typer/utils.py` & `typer-0.9.4/typer/utils.py`

 * *Files identical despite different names*

### Comparing `typer-0.9.3/PKG-INFO` & `typer-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer
-Version: 0.9.3
+Version: 0.9.4
 Summary: Typer, build great CLIs. Easy to code. Based on Python type hints.
 Home-page: https://github.com/tiangolo/typer
 Author: Sebastián Ramírez
 Author-email: tiangolo@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: typer Version: 0.9.3 Summary: Typer, build great
+Metadata-Version: 2.1 Name: typer Version: 0.9.4 Summary: Typer, build great
 CLIs. Easy to code. Based on Python type hints. Home-page: https://github.com/
 tiangolo/typer Author: SebastiÃ¡n RamÃ­rez Author-email: tiangolo@gmail.com
 Requires-Python: >=3.6 Description-Content-Type: text/markdown Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 System Administrators Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python Classifier: Topic :: Software Development :: Libraries ::
```

