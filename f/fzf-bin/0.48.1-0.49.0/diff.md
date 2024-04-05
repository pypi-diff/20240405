# Comparing `tmp/fzf_bin-0.48.1.tar.gz` & `tmp/fzf_bin-0.49.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fzf_bin-0.48.1.tar", last modified: Mon Mar 18 04:41:20 2024, max compression
+gzip compressed data, was "fzf_bin-0.49.0.tar", last modified: Fri Apr  5 07:24:44 2024, max compression
```

## Comparing `fzf_bin-0.48.1.tar` & `fzf_bin-0.49.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     1074 2024-03-18 04:40:08.208027 fzf_bin-0.48.1/LICENSE
--rw-r--r--   0        0        0      469 2024-03-18 04:40:08.208027 fzf_bin-0.48.1/README.md
--rw-r--r--   0        0        0       35 2024-03-18 04:40:09.084035 fzf_bin-0.48.1/fzf/.git
--rw-r--r--   0        0        0       17 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/.github/FUNDING.yml
--rw-r--r--   0        0        0      419 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      209 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/.github/dependabot.yml
--rw-r--r--   0        0        0     1111 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      296 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/.github/workflows/depsreview.yaml
--rw-r--r--   0        0        0     1117 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/.github/workflows/linux.yml
--rw-r--r--   0        0        0      999 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/.github/workflows/macos.yml
--rw-r--r--   0        0        0      555 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/.github/workflows/sponsors.yml
--rw-r--r--   0        0        0      193 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/.github/workflows/typos.yml
--rw-r--r--   0        0        0      382 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/.github/workflows/winget.yml
--rw-r--r--   0        0        0      104 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/.gitignore
--rw-r--r--   0        0        0     2657 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/.goreleaser.yml
--rw-r--r--   0        0        0      578 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/.rubocop.yml
--rw-r--r--   0        0        0       15 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/.tool-versions
--rw-r--r--   0        0        0    28068 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/ADVANCED.md
--rw-r--r--   0        0        0     1455 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/BUILD.md
--rw-r--r--   0        0        0    71830 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/CHANGELOG.md
--rw-r--r--   0        0        0      509 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/Dockerfile
--rw-r--r--   0        0        0     1085 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/LICENSE
--rw-r--r--   0        0        0     5245 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/Makefile
--rw-r--r--   0        0        0    17711 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/README-VIM.md
--rw-r--r--   0        0        0    35275 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/README.md
--rwxr-xr-x   0        0        0     2419 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/bin/fzf-preview.sh
--rwxr-xr-x   0        0        0     7079 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/bin/fzf-tmux
--rw-r--r--   0        0        0    21398 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/doc/fzf.txt
--rw-r--r--   0        0        0      496 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/go.mod
--rw-r--r--   0        0        0     5203 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/go.sum
--rwxr-xr-x   0        0        0    10184 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/install
--rw-r--r--   0        0        0     1881 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/install.ps1
--rw-r--r--   0        0        0     1159 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/main.go
--rw-r--r--   0        0        0     1992 2024-03-18 04:40:09.096035 fzf_bin-0.48.1/fzf/man/man1/fzf-tmux.1
--rw-r--r--   0        0        0    49758 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/man/man1/fzf.1
--rw-r--r--   0        0        0    32550 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/plugin/fzf.vim
--rw-r--r--   0        0        0    16128 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/shell/completion.bash
--rw-r--r--   0        0        0    12037 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/shell/completion.zsh
--rw-r--r--   0        0        0     5299 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/shell/key-bindings.bash
--rw-r--r--   0        0        0     5558 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/shell/key-bindings.fish
--rw-r--r--   0        0        0     3877 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/shell/key-bindings.zsh
--rw-r--r--   0        0        0     1085 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/LICENSE
--rw-r--r--   0        0        0     5293 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/actiontype_string.go
--rw-r--r--   0        0        0    25675 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/algo/algo.go
--rw-r--r--   0        0        0     8849 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/algo/algo_test.go
--rw-r--r--   0        0        0    21779 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/algo/normalize.go
--rw-r--r--   0        0        0     9960 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/ansi.go
--rw-r--r--   0        0        0    11138 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/ansi_test.go
--rw-r--r--   0        0        0     1619 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/cache.go
--rw-r--r--   0        0        0      859 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/cache_test.go
--rw-r--r--   0        0        0     1806 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/chunklist.go
--rw-r--r--   0        0        0     1862 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/chunklist_test.go
--rw-r--r--   0        0        0     1667 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/constants.go
--rw-r--r--   0        0        0     9928 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/core.go
--rw-r--r--   0        0        0     2071 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/history.go
--rw-r--r--   0        0        0     1507 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/history_test.go
--rw-r--r--   0        0        0      957 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/item.go
--rw-r--r--   0        0        0      484 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/item_test.go
--rw-r--r--   0        0        0     5411 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/matcher.go
--rw-r--r--   0        0        0     3302 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/merger.go
--rw-r--r--   0        0        0     1989 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/merger_test.go
--rw-r--r--   0        0        0    64808 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/options.go
--rw-r--r--   0        0        0    14755 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/options_test.go
--rw-r--r--   0        0        0    10565 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/pattern.go
--rw-r--r--   0        0        0     8060 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/pattern_test.go
--rw-r--r--   0        0        0      131 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/protector/protector.go
--rw-r--r--   0        0        0      217 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/protector/protector_openbsd.go
--rw-r--r--   0        0        0     4461 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/reader.go
--rw-r--r--   0        0        0     1279 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/reader_test.go
--rw-r--r--   0        0        0     5998 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/result.go
--rw-r--r--   0        0        0      338 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/result_others.go
--rw-r--r--   0        0        0     6064 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/result_test.go
--rw-r--r--   0        0        0      364 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/result_x86.go
--rw-r--r--   0        0        0     6175 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/server.go
--rw-r--r--   0        0        0   112249 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/terminal.go
--rw-r--r--   0        0        0    27879 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/terminal_test.go
--rw-r--r--   0        0        0     1008 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/terminal_unix.go
--rw-r--r--   0        0        0     1088 2024-03-18 04:40:09.100035 fzf_bin-0.48.1/fzf/src/terminal_windows.go
--rw-r--r--   0        0        0     5651 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/tokenizer.go
--rw-r--r--   0        0        0     2858 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/tokenizer_test.go
--rw-r--r--   0        0        0     1794 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/tui/dummy.go
--rw-r--r--   0        0        0    24069 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/tui/light.go
--rw-r--r--   0        0        0     2508 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/tui/light_unix.go
--rw-r--r--   0        0        0     4777 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/tui/light_windows.go
--rw-r--r--   0        0        0    18498 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/tui/tcell.go
--rw-r--r--   0        0        0    17341 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/tui/tcell_test.go
--rw-r--r--   0        0        0      908 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/tui/ttyname_unix.go
--rw-r--r--   0        0        0      164 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/tui/ttyname_windows.go
--rw-r--r--   0        0        0    20523 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/tui/tui.go
--rw-r--r--   0        0        0      399 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/tui/tui_test.go
--rw-r--r--   0        0        0      748 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/util/atomicbool.go
--rw-r--r--   0        0        0      301 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/util/atomicbool_test.go
--rw-r--r--   0        0        0     4241 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/util/chars.go
--rw-r--r--   0        0        0      981 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/util/chars_test.go
--rw-r--r--   0        0        0     1976 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/util/eventbox.go
--rw-r--r--   0        0        0      899 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/util/eventbox_test.go
--rw-r--r--   0        0        0      185 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/util/slab.go
--rw-r--r--   0        0        0     3485 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/util/util.go
--rw-r--r--   0        0        0     4194 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/util/util_test.go
--rw-r--r--   0        0        0     1199 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/util/util_unix.go
--rw-r--r--   0        0        0     2219 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/src/util/util_windows.go
--rw-r--r--   0        0        0     5860 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/test/fzf.vader
--rwxr-xr-x   0        0        0   121853 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/test/test_go.rb
--rw-r--r--   0        0        0      216 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/typos.toml
--rwxr-xr-x   0        0        0     2520 2024-03-18 04:40:09.104035 fzf_bin-0.48.1/fzf/uninstall
--rw-r--r--   0        0        0        0 2024-03-18 04:40:08.208027 fzf_bin-0.48.1/fzf_bin/__init__.py
--rw-r--r--   0        0        0     1392 2024-03-18 04:40:08.208027 fzf_bin-0.48.1/pdm_build.py
--rw-r--r--   0        0        0     1073 2024-03-18 04:41:20.828765 fzf_bin-0.48.1/pyproject.toml
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 fzf_bin-0.48.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-05 07:23:26.410044 fzf_bin-0.49.0/LICENSE
+-rw-r--r--   0        0        0      469 2024-04-05 07:23:26.410044 fzf_bin-0.49.0/README.md
+-rw-r--r--   0        0        0       35 2024-04-05 07:23:28.346023 fzf_bin-0.49.0/fzf/.git
+-rw-r--r--   0        0        0       17 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1031 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/ISSUE_TEMPLATE/issue_template.yml
+-rw-r--r--   0        0        0      209 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/dependabot.yml
+-rw-r--r--   0        0        0     1111 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      296 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/workflows/depsreview.yaml
+-rw-r--r--   0        0        0     1119 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/workflows/linux.yml
+-rw-r--r--   0        0        0     1001 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/workflows/macos.yml
+-rw-r--r--   0        0        0      555 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/workflows/sponsors.yml
+-rw-r--r--   0        0        0      193 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/.github/workflows/typos.yml
+-rw-r--r--   0        0        0      382 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/.github/workflows/winget.yml
+-rw-r--r--   0        0        0      104 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/.gitignore
+-rw-r--r--   0        0        0     2431 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/.goreleaser.yml
+-rw-r--r--   0        0        0      578 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/.rubocop.yml
+-rw-r--r--   0        0        0       15 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/.tool-versions
+-rw-r--r--   0        0        0    28068 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/ADVANCED.md
+-rw-r--r--   0        0        0     1455 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/BUILD.md
+-rw-r--r--   0        0        0    73299 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/CHANGELOG.md
+-rw-r--r--   0        0        0      509 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/Dockerfile
+-rw-r--r--   0        0        0     1085 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/LICENSE
+-rw-r--r--   0        0        0     5245 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/Makefile
+-rw-r--r--   0        0        0    17711 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/README-VIM.md
+-rw-r--r--   0        0        0    35700 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/README.md
+-rwxr-xr-x   0        0        0     2419 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/bin/fzf-preview.sh
+-rwxr-xr-x   0        0        0     7079 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/bin/fzf-tmux
+-rw-r--r--   0        0        0    21398 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/doc/fzf.txt
+-rw-r--r--   0        0        0      496 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/go.mod
+-rw-r--r--   0        0        0     5203 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/go.sum
+-rwxr-xr-x   0        0        0    10184 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/install
+-rw-r--r--   0        0        0     1881 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/install.ps1
+-rw-r--r--   0        0        0     1159 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/main.go
+-rw-r--r--   0        0        0     1992 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/man/man1/fzf-tmux.1
+-rw-r--r--   0        0        0    50220 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/man/man1/fzf.1
+-rw-r--r--   0        0        0    32550 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/plugin/fzf.vim
+-rw-r--r--   0        0        0    16178 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/shell/completion.bash
+-rw-r--r--   0        0        0    12037 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/shell/completion.zsh
+-rw-r--r--   0        0        0     5357 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/shell/key-bindings.bash
+-rw-r--r--   0        0        0     5602 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/shell/key-bindings.fish
+-rw-r--r--   0        0        0     3879 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/shell/key-bindings.zsh
+-rw-r--r--   0        0        0     1085 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/LICENSE
+-rw-r--r--   0        0        0     5422 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/actiontype_string.go
+-rw-r--r--   0        0        0    25675 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/algo/algo.go
+-rw-r--r--   0        0        0     8849 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/algo/algo_test.go
+-rw-r--r--   0        0        0    21779 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/algo/normalize.go
+-rw-r--r--   0        0        0     9960 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/ansi.go
+-rw-r--r--   0        0        0    11138 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/ansi_test.go
+-rw-r--r--   0        0        0     1619 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/cache.go
+-rw-r--r--   0        0        0      859 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/cache_test.go
+-rw-r--r--   0        0        0     1806 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/chunklist.go
+-rw-r--r--   0        0        0     1862 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/chunklist_test.go
+-rw-r--r--   0        0        0     1704 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/constants.go
+-rw-r--r--   0        0        0    10183 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/core.go
+-rw-r--r--   0        0        0     2071 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/history.go
+-rw-r--r--   0        0        0     1507 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/history_test.go
+-rw-r--r--   0        0        0      957 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/item.go
+-rw-r--r--   0        0        0      484 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/item_test.go
+-rw-r--r--   0        0        0     5411 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/matcher.go
+-rw-r--r--   0        0        0     3302 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/merger.go
+-rw-r--r--   0        0        0     1989 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/merger_test.go
+-rw-r--r--   0        0        0    65018 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/options.go
+-rw-r--r--   0        0        0    14755 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/options_test.go
+-rw-r--r--   0        0        0    10565 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/pattern.go
+-rw-r--r--   0        0        0     8060 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/pattern_test.go
+-rw-r--r--   0        0        0      131 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/protector/protector.go
+-rw-r--r--   0        0        0      217 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/protector/protector_openbsd.go
+-rw-r--r--   0        0        0     5485 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/reader.go
+-rw-r--r--   0        0        0     1279 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/reader_test.go
+-rw-r--r--   0        0        0     5998 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/result.go
+-rw-r--r--   0        0        0      338 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/result_others.go
+-rw-r--r--   0        0        0     6064 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/result_test.go
+-rw-r--r--   0        0        0      364 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/result_x86.go
+-rw-r--r--   0        0        0     6297 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/server.go
+-rw-r--r--   0        0        0   113782 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/terminal.go
+-rw-r--r--   0        0        0    27879 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/terminal_test.go
+-rw-r--r--   0        0        0     1008 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/terminal_unix.go
+-rw-r--r--   0        0        0     1088 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/terminal_windows.go
+-rw-r--r--   0        0        0     5651 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tokenizer.go
+-rw-r--r--   0        0        0     2858 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tokenizer_test.go
+-rw-r--r--   0        0        0     1794 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/dummy.go
+-rw-r--r--   0        0        0    24069 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/light.go
+-rw-r--r--   0        0        0     2508 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/light_unix.go
+-rw-r--r--   0        0        0     4777 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/light_windows.go
+-rw-r--r--   0        0        0    18498 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/tcell.go
+-rw-r--r--   0        0        0    17341 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/tcell_test.go
+-rw-r--r--   0        0        0      908 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/ttyname_unix.go
+-rw-r--r--   0        0        0      164 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/ttyname_windows.go
+-rw-r--r--   0        0        0    20523 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/tui.go
+-rw-r--r--   0        0        0      399 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/tui_test.go
+-rw-r--r--   0        0        0      748 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/atomicbool.go
+-rw-r--r--   0        0        0      301 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/atomicbool_test.go
+-rw-r--r--   0        0        0     4284 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/chars.go
+-rw-r--r--   0        0        0      981 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/chars_test.go
+-rw-r--r--   0        0        0     1976 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/eventbox.go
+-rw-r--r--   0        0        0      899 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/eventbox_test.go
+-rw-r--r--   0        0        0      185 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/slab.go
+-rw-r--r--   0        0        0     3485 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/util.go
+-rw-r--r--   0        0        0     4194 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/util_test.go
+-rw-r--r--   0        0        0     1199 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/util_unix.go
+-rw-r--r--   0        0        0     2219 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/util_windows.go
+-rw-r--r--   0        0        0     5860 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/test/fzf.vader
+-rwxr-xr-x   0        0        0   125876 2024-04-05 07:23:28.366023 fzf_bin-0.49.0/fzf/test/test_go.rb
+-rw-r--r--   0        0        0      216 2024-04-05 07:23:28.366023 fzf_bin-0.49.0/fzf/typos.toml
+-rwxr-xr-x   0        0        0     2520 2024-04-05 07:23:28.366023 fzf_bin-0.49.0/fzf/uninstall
+-rw-r--r--   0        0        0        0 2024-04-05 07:23:26.410044 fzf_bin-0.49.0/fzf_bin/__init__.py
+-rw-r--r--   0        0        0     1392 2024-04-05 07:23:26.410044 fzf_bin-0.49.0/pdm_build.py
+-rw-r--r--   0        0        0     1073 2024-04-05 07:24:44.009291 fzf_bin-0.49.0/pyproject.toml
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 fzf_bin-0.49.0/PKG-INFO
```

### Comparing `fzf_bin-0.48.1/LICENSE` & `fzf_bin-0.49.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/.github/workflows/codeql-analysis.yml` & `fzf_bin-0.49.0/fzf/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/.github/workflows/linux.yml` & `fzf_bin-0.49.0/fzf/.github/workflows/linux.yml`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
 
     - name: Set up Go
       uses: actions/setup-go@v5
       with:
-        go-version: 1.19
+        go-version: "1.20"
 
     - name: Setup Ruby
       uses: ruby/setup-ruby@v1
       with:
         ruby-version: 3.1.0
 
     - name: Install packages
```

### Comparing `fzf_bin-0.48.1/fzf/.github/workflows/macos.yml` & `fzf_bin-0.49.0/fzf/.github/workflows/macos.yml`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
 
     - name: Set up Go
       uses: actions/setup-go@v5
       with:
-        go-version: 1.18
+        go-version: "1.20"
 
     - name: Setup Ruby
       uses: ruby/setup-ruby@v1
       with:
         ruby-version: 3.0.0
 
     - name: Install packages
```

### Comparing `fzf_bin-0.48.1/fzf/.github/workflows/sponsors.yml` & `fzf_bin-0.49.0/fzf/.github/workflows/sponsors.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/.goreleaser.yml` & `fzf_bin-0.49.0/fzf/.goreleaser.yml`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,14 @@
       - "-s -w -X main.version={{ .Version }} -X main.revision={{ .ShortCommit }}"
     hooks:
       post: |
         sh -c '
         cat > /tmp/fzf-gon-amd64.hcl << EOF
         source = ["./dist/fzf-macos_darwin_amd64_v1/fzf"]
         bundle_id = "kr.junegunn.fzf"
-        apple_id {
-          username = "junegunn.c@gmail.com"
-          password = "@env:AC_PASSWORD"
-        }
         sign {
           application_identity = "Developer ID Application: Junegunn Choi (Y254DRW44Z)"
         }
         zip {
           output_path = "./dist/fzf-{{ .Version }}-darwin_amd64.zip"
         }
         EOF
@@ -44,18 +40,14 @@
       - "-s -w -X main.version={{ .Version }} -X main.revision={{ .ShortCommit }}"
     hooks:
       post: |
         sh -c '
         cat > /tmp/fzf-gon-arm64.hcl << EOF
         source = ["./dist/fzf-macos-arm_darwin_arm64/fzf"]
         bundle_id = "kr.junegunn.fzf"
-        apple_id {
-          username = "junegunn.c@gmail.com"
-          password = "@env:AC_PASSWORD"
-        }
         sign {
           application_identity = "Developer ID Application: Junegunn Choi (Y254DRW44Z)"
         }
         zip {
           output_path = "./dist/fzf-{{ .Version }}-darwin_arm64.zip"
         }
         EOF
```

### Comparing `fzf_bin-0.48.1/fzf/.rubocop.yml` & `fzf_bin-0.49.0/fzf/.rubocop.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/ADVANCED.md` & `fzf_bin-0.49.0/fzf/ADVANCED.md`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/BUILD.md` & `fzf_bin-0.49.0/fzf/BUILD.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ============
 
 Build instructions
 ------------------
 
 ### Prerequisites
 
-- Go 1.18 or above
+- Go 1.20 or above
 
 ### Using Makefile
 
 ```sh
 # Build fzf binary for your platform in target
 make
```

### Comparing `fzf_bin-0.48.1/fzf/CHANGELOG.md` & `fzf_bin-0.49.0/fzf/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,39 @@
 CHANGELOG
 =========
 
+0.49.0
+------
+- Ingestion performance improved by around 40% (more or less depending on options)
+- `--info=hidden` and `--info=inline-right` will no longer hide the horizontal separator by default. This gives you more flexibility in customizing the layout.
+    ```sh
+    fzf --border --info=inline-right
+    fzf --border --info=inline-right --separator ═
+    fzf --border --info=inline-right --no-separator
+    fzf --border --info=hidden
+    fzf --border --info=hidden --separator ━
+    fzf --border --info=hidden --no-separator
+    ```
+- Added two environment variables exported to the child processes
+    - `FZF_PREVIEW_LABEL`
+    - `FZF_BORDER_LABEL`
+    ```sh
+    # Use the current value of $FZF_PREVIEW_LABEL to determine which actions to perform
+    git ls-files |
+      fzf --header 'Press CTRL-P to change preview mode' \
+          --bind='ctrl-p:transform:[[ $FZF_PREVIEW_LABEL =~ cat ]] \
+          && echo "change-preview(git log --color=always \{})+change-preview-label([[ log ]])" \
+          || echo "change-preview(bat --color=always \{})+change-preview-label([[ cat ]])"'
+    ```
+- Renamed `track` action to `track-current` to highlight the difference between the global tracking state set by `--track` and a one-off tracking action
+    - `track` is still available as an alias
+- Added `untrack-current` and `toggle-track-current` actions
+    - `*-current` actions are no-op when the global tracking state is set
+- Bug fixes and minor improvements
+
 0.48.1
 ------
 - CTRL-T and ALT-C bindings can be disabled by setting `FZF_CTRL_T_COMMAND` and `FZF_ALT_C_COMMAND` to empty strings respectively when sourcing the script
     ```sh
     # bash
     FZF_CTRL_T_COMMAND= FZF_ALT_C_COMMAND= eval "$(fzf --bash)"
```

### Comparing `fzf_bin-0.48.1/fzf/LICENSE` & `fzf_bin-0.49.0/fzf/LICENSE`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/Makefile` & `fzf_bin-0.49.0/fzf/Makefile`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/README-VIM.md` & `fzf_bin-0.49.0/fzf/README-VIM.md`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/README.md` & `fzf_bin-0.49.0/fzf/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 Sponsors ❤️
 -----------
 
 I would like to thank all the sponsors of this project who make it possible for me to continue to improve fzf.
 
 If you'd like to sponsor this project, please visit https://github.com/sponsors/junegunn.
 
-<!-- sponsors --><a href="https://github.com/miyanokomiya"><img src="https://github.com/miyanokomiya.png" width="60px" alt="miyanokomiya" /></a><a href="https://github.com/jonhoo"><img src="https://github.com/jonhoo.png" width="60px" alt="Jon Gjengset" /></a><a href="https://github.com/AceofSpades5757"><img src="https://github.com/AceofSpades5757.png" width="60px" alt="Kyle L. Davis" /></a><a href="https://github.com/Frederick888"><img src="https://github.com/Frederick888.png" width="60px" alt="Frederick Zhang" /></a><a href="https://github.com/moritzdietz"><img src="https://github.com/moritzdietz.png" width="60px" alt="Moritz Dietz" /></a><a href="https://github.com/mikker"><img src="https://github.com/mikker.png" width="60px" alt="Mikkel Malmberg" /></a><a href="https://github.com/pldubouilh"><img src="https://github.com/pldubouilh.png" width="60px" alt="Pierre Dubouilh" /></a><a href="https://github.com/rcorre"><img src="https://github.com/rcorre.png" width="60px" alt="Ryan Roden-Corrent" /></a><a href="https://github.com/blissdev"><img src="https://github.com/blissdev.png" width="60px" alt="Jordan Arentsen" /></a><a href="https://github.com/mislav"><img src="https://github.com/mislav.png" width="60px" alt="Mislav Marohnić" /></a><a href="https://github.com/aexvir"><img src="https://github.com/aexvir.png" width="60px" alt="Alex Viscreanu" /></a><a href="https://github.com/dbalatero"><img src="https://github.com/dbalatero.png" width="60px" alt="David Balatero" /></a><a href="https://github.com/comatory"><img src="https://github.com/comatory.png" width="60px" alt="Ondrej Synacek" /></a><a href="https://github.com/moobar"><img src="https://github.com/moobar.png" width="60px" alt="" /></a><a href="https://github.com/majjoha"><img src="https://github.com/majjoha.png" width="60px" alt="Mathias Jean Johansen" /></a><a href="https://github.com/benelan"><img src="https://github.com/benelan.png" width="60px" alt="Ben Elan" /></a><a href="https://github.com/pawelduda"><img src="https://github.com/pawelduda.png" width="60px" alt="Paweł Duda" /></a><a href="https://github.com/slezica"><img src="https://github.com/slezica.png" width="60px" alt="Santiago Lezica" /></a><a href="https://github.com/pbwn"><img src="https://github.com/pbwn.png" width="60px" alt="" /></a><a href="https://github.com/timgluz"><img src="https://github.com/timgluz.png" width="60px" alt="Timo Sulg" /></a><a href="https://github.com/pyrho"><img src="https://github.com/pyrho.png" width="60px" alt="Damien Rajon" /></a><a href="https://github.com/ArtBIT"><img src="https://github.com/ArtBIT.png" width="60px" alt="ArtBIT" /></a><a href="https://github.com/da-moon"><img src="https://github.com/da-moon.png" width="60px" alt="" /></a><a href="https://github.com/hovissimo"><img src="https://github.com/hovissimo.png" width="60px" alt="Hovis" /></a><a href="https://github.com/dariusjonda"><img src="https://github.com/dariusjonda.png" width="60px" alt="Darius Jonda" /></a><a href="https://github.com/cristiand391"><img src="https://github.com/cristiand391.png" width="60px" alt="Cristian Dominguez" /></a><a href="https://github.com/eliangcs"><img src="https://github.com/eliangcs.png" width="60px" alt="Chang-Hung Liang" /></a><a href="https://github.com/asphaltbuffet"><img src="https://github.com/asphaltbuffet.png" width="60px" alt="Ben Lechlitner" /></a><a href="https://github.com/yash1th"><img src="https://github.com/yash1th.png" width="60px" alt="yash" /></a><a href="https://github.com/looshch"><img src="https://github.com/looshch.png" width="60px" alt="george looshch" /></a><a href="https://github.com/kg8m"><img src="https://github.com/kg8m.png" width="60px" alt="Takumi KAGIYAMA" /></a><a href="https://github.com/polm"><img src="https://github.com/polm.png" width="60px" alt="Paul O'Leary McCann" /></a><a href="https://github.com/rbeeger"><img src="https://github.com/rbeeger.png" width="60px" alt="Robert Beeger" /></a><a href="https://github.com/veebch"><img src="https://github.com/veebch.png" width="60px" alt="VEEB Projects" /></a><a href="https://github.com/khuedoan"><img src="https://github.com/khuedoan.png" width="60px" alt="Khue Doan" /></a><a href="https://github.com/yowayb"><img src="https://github.com/yowayb.png" width="60px" alt="Yoway Buorn" /></a><a href="https://github.com/scalisi"><img src="https://github.com/scalisi.png" width="60px" alt="Josh Scalisi" /></a><a href="https://github.com/alecbcs"><img src="https://github.com/alecbcs.png" width="60px" alt="Alec Scott" /></a><a href="https://github.com/thnxdev"><img src="https://github.com/thnxdev.png" width="60px" alt="thanks.dev" /></a><a href="https://github.com/artursapek"><img src="https://github.com/artursapek.png" width="60px" alt="Artur Sapek" /></a><a href="https://github.com/ramnes"><img src="https://github.com/ramnes.png" width="60px" alt="Guillaume Gelin" /></a><a href="https://github.com/jyc"><img src="https://github.com/jyc.png" width="60px" alt="" /></a><a href="https://github.com/mrcnski"><img src="https://github.com/mrcnski.png" width="60px" alt="Marcin S." /></a><a href="https://github.com/roblevy"><img src="https://github.com/roblevy.png" width="60px" alt="Rob Levy" /></a><a href="https://github.com/glozow"><img src="https://github.com/glozow.png" width="60px" alt="Gloria Zhao" /></a><a href="https://github.com/pooriajr"><img src="https://github.com/pooriajr.png" width="60px" alt="Pooria" /></a><a href="https://github.com/wjt"><img src="https://github.com/wjt.png" width="60px" alt="Will Thompson" /></a><a href="https://github.com/faruzzy"><img src="https://github.com/faruzzy.png" width="60px" alt="Roland" /></a><a href="https://github.com/mrhenry"><img src="https://github.com/mrhenry.png" width="60px" alt="Mr. Henry" /></a><!-- sponsors -->
+<!-- sponsors --><a href="https://github.com/miyanokomiya"><img src="https://github.com/miyanokomiya.png" width="60px" alt="miyanokomiya" /></a><a href="https://github.com/jonhoo"><img src="https://github.com/jonhoo.png" width="60px" alt="Jon Gjengset" /></a><a href="https://github.com/AceofSpades5757"><img src="https://github.com/AceofSpades5757.png" width="60px" alt="Kyle L. Davis" /></a><a href="https://github.com/Frederick888"><img src="https://github.com/Frederick888.png" width="60px" alt="Frederick Zhang" /></a><a href="https://github.com/moritzdietz"><img src="https://github.com/moritzdietz.png" width="60px" alt="Moritz Dietz" /></a><a href="https://github.com/mikker"><img src="https://github.com/mikker.png" width="60px" alt="Mikkel Malmberg" /></a><a href="https://github.com/pldubouilh"><img src="https://github.com/pldubouilh.png" width="60px" alt="Pierre Dubouilh" /></a><a href="https://github.com/rcorre"><img src="https://github.com/rcorre.png" width="60px" alt="Ryan Roden-Corrent" /></a><a href="https://github.com/blissdev"><img src="https://github.com/blissdev.png" width="60px" alt="Jordan Arentsen" /></a><a href="https://github.com/mislav"><img src="https://github.com/mislav.png" width="60px" alt="Mislav Marohnić" /></a><a href="https://github.com/aexvir"><img src="https://github.com/aexvir.png" width="60px" alt="Alex Viscreanu" /></a><a href="https://github.com/dbalatero"><img src="https://github.com/dbalatero.png" width="60px" alt="David Balatero" /></a><a href="https://github.com/comatory"><img src="https://github.com/comatory.png" width="60px" alt="Ondrej Synacek" /></a><a href="https://github.com/moobar"><img src="https://github.com/moobar.png" width="60px" alt="" /></a><a href="https://github.com/majjoha"><img src="https://github.com/majjoha.png" width="60px" alt="Mathias Jean Johansen" /></a><a href="https://github.com/benelan"><img src="https://github.com/benelan.png" width="60px" alt="Ben Elan" /></a><a href="https://github.com/pawelduda"><img src="https://github.com/pawelduda.png" width="60px" alt="Paweł Duda" /></a><a href="https://github.com/slezica"><img src="https://github.com/slezica.png" width="60px" alt="Santiago Lezica" /></a><a href="https://github.com/pbwn"><img src="https://github.com/pbwn.png" width="60px" alt="" /></a><a href="https://github.com/timgluz"><img src="https://github.com/timgluz.png" width="60px" alt="Timo Sulg" /></a><a href="https://github.com/pyrho"><img src="https://github.com/pyrho.png" width="60px" alt="Damien Rajon" /></a><a href="https://github.com/ArtBIT"><img src="https://github.com/ArtBIT.png" width="60px" alt="ArtBIT" /></a><a href="https://github.com/da-moon"><img src="https://github.com/da-moon.png" width="60px" alt="" /></a><a href="https://github.com/hovissimo"><img src="https://github.com/hovissimo.png" width="60px" alt="Hovis" /></a><a href="https://github.com/dariusjonda"><img src="https://github.com/dariusjonda.png" width="60px" alt="Darius Jonda" /></a><a href="https://github.com/cristiand391"><img src="https://github.com/cristiand391.png" width="60px" alt="Cristian Dominguez" /></a><a href="https://github.com/eliangcs"><img src="https://github.com/eliangcs.png" width="60px" alt="Chang-Hung Liang" /></a><a href="https://github.com/asphaltbuffet"><img src="https://github.com/asphaltbuffet.png" width="60px" alt="Ben Lechlitner" /></a><a href="https://github.com/yash1th"><img src="https://github.com/yash1th.png" width="60px" alt="yash" /></a><a href="https://github.com/looshch"><img src="https://github.com/looshch.png" width="60px" alt="george looshch" /></a><a href="https://github.com/kg8m"><img src="https://github.com/kg8m.png" width="60px" alt="Takumi KAGIYAMA" /></a><a href="https://github.com/polm"><img src="https://github.com/polm.png" width="60px" alt="Paul O'Leary McCann" /></a><a href="https://github.com/rbeeger"><img src="https://github.com/rbeeger.png" width="60px" alt="Robert Beeger" /></a><a href="https://github.com/veebch"><img src="https://github.com/veebch.png" width="60px" alt="VEEB Projects" /></a><a href="https://github.com/khuedoan"><img src="https://github.com/khuedoan.png" width="60px" alt="Khue Doan" /></a><a href="https://github.com/yowayb"><img src="https://github.com/yowayb.png" width="60px" alt="Yoway Buorn" /></a><a href="https://github.com/scalisi"><img src="https://github.com/scalisi.png" width="60px" alt="Josh Scalisi" /></a><a href="https://github.com/alecbcs"><img src="https://github.com/alecbcs.png" width="60px" alt="Alec Scott" /></a><a href="https://github.com/thnxdev"><img src="https://github.com/thnxdev.png" width="60px" alt="thanks.dev" /></a><a href="https://github.com/artursapek"><img src="https://github.com/artursapek.png" width="60px" alt="Artur Sapek" /></a><a href="https://github.com/ramnes"><img src="https://github.com/ramnes.png" width="60px" alt="Guillaume Gelin" /></a><a href="https://github.com/jyc"><img src="https://github.com/jyc.png" width="60px" alt="" /></a><a href="https://github.com/mrcnski"><img src="https://github.com/mrcnski.png" width="60px" alt="Marcin S." /></a><a href="https://github.com/roblevy"><img src="https://github.com/roblevy.png" width="60px" alt="Rob Levy" /></a><a href="https://github.com/glozow"><img src="https://github.com/glozow.png" width="60px" alt="Gloria Zhao" /></a><a href="https://github.com/wjt"><img src="https://github.com/wjt.png" width="60px" alt="Will Thompson" /></a><a href="https://github.com/faruzzy"><img src="https://github.com/faruzzy.png" width="60px" alt="Roland" /></a><a href="https://github.com/mrhenry"><img src="https://github.com/mrhenry.png" width="60px" alt="Mr. Henry" /></a><a href="https://github.com/mauricelam"><img src="https://github.com/mauricelam.png" width="60px" alt="Maurice Lam" /></a><a href="https://github.com/toupeira"><img src="https://github.com/toupeira.png" width="60px" alt="Markus Koller" /></a><a href="https://github.com/rkpatel33"><img src="https://github.com/rkpatel33.png" width="60px" alt="" /></a><!-- sponsors -->
 
 Table of Contents
 -----------------
 
 <!-- vim-markdown-toc GFM -->
 
 * [Installation](#installation)
@@ -208,17 +208,20 @@
 * fish
   ```fish
   # Set up fzf key bindings
   fzf --fish | source
   ```
 
 > [!NOTE]
-> `--bash`, `--zsh`, and `--fish` options are only available in
-> fzf 0.48.0 or above. If you have an older version of fzf, refer to the
-> package documentation for more information. (e.g. `apt show fzf`)
+> `--bash`, `--zsh`, and `--fish` options are only available in fzf 0.48.0 or
+> later. If you have an older version of fzf, or want finer control, you can
+> source individual script files in the [/shell](/shell) directory. The
+> location of the files may vary depending on the package manager you use.
+> Please refer to the package documentation for more information.
+> (e.g. `apt show fzf`)
 
 > [!TIP]
 > You can disable CTRL-T or ALT-C binding by setting `FZF_CTRL_T_COMMAND` or
 > `FZF_ALT_C_COMMAND` to an empty string when sourcing the script.
 > For example, to disable ALT-C binding:
 >
 > * bash: `FZF_ALT_C_COMMAND= eval "$(fzf --bash)"`
```

#### html2text {}

```diff
@@ -22,187 +22,190 @@
 _[_M_o_r_i_t_z_ _D_i_e_t_z_]_[_M_i_k_k_e_l_ _M_a_l_m_b_e_r_g_]_[_P_i_e_r_r_e_ _D_u_b_o_u_i_l_h_]_[_R_y_a_n_ _R_o_d_e_n_-_C_o_r_r_e_n_t_]_[_J_o_r_d_a_n
 _A_r_e_n_t_s_e_n_]_[_M_i_s_l_a_v_ _M_a_r_o_h_n_i_Ä__]_[_A_l_e_x_ _V_i_s_c_r_e_a_n_u_]_[_D_a_v_i_d_ _B_a_l_a_t_e_r_o_]_[_O_n_d_r_e_j_ _S_y_n_a_c_e_k_]
 _[_M_a_t_h_i_a_s_ _J_e_a_n_ _J_o_h_a_n_s_e_n_]_[_B_e_n_ _E_l_a_n_]_[_P_a_w_e_Å__ _D_u_d_a_]_[_S_a_n_t_i_a_g_o_ _L_e_z_i_c_a_]_[_T_i_m_o_ _S_u_l_g_]
 _[_D_a_m_i_e_n_ _R_a_j_o_n_]_[_A_r_t_B_I_T_]_[_H_o_v_i_s_]_[_D_a_r_i_u_s_ _J_o_n_d_a_]_[_C_r_i_s_t_i_a_n_ _D_o_m_i_n_g_u_e_z_]_[_C_h_a_n_g_-_H_u_n_g
 _L_i_a_n_g_]_[_B_e_n_ _L_e_c_h_l_i_t_n_e_r_]_[_y_a_s_h_]_[_g_e_o_r_g_e_ _l_o_o_s_h_c_h_]_[_T_a_k_u_m_i_ _K_A_G_I_Y_A_M_A_]_[_P_a_u_l_ _O_'_L_e_a_r_y
 _M_c_C_a_n_n_]_[_R_o_b_e_r_t_ _B_e_e_g_e_r_]_[_V_E_E_B_ _P_r_o_j_e_c_t_s_]_[_K_h_u_e_ _D_o_a_n_]_[_Y_o_w_a_y_ _B_u_o_r_n_]_[_J_o_s_h_ _S_c_a_l_i_s_i_]
 _[_A_l_e_c_ _S_c_o_t_t_]_[_t_h_a_n_k_s_._d_e_v_]_[_A_r_t_u_r_ _S_a_p_e_k_]_[_G_u_i_l_l_a_u_m_e_ _G_e_l_i_n_]_[_M_a_r_c_i_n_ _S_._]_[_R_o_b_ _L_e_v_y_]
-_[_G_l_o_r_i_a_ _Z_h_a_o_]_[_P_o_o_r_i_a_]_[_W_i_l_l_ _T_h_o_m_p_s_o_n_]_[_R_o_l_a_n_d_]_[_M_r_._ _H_e_n_r_y_]Table of Contents ------
------------ * [Installation](#installation) * [Using Homebrew](#using-homebrew)
-* [Using git](#using-git) * [Using Linux package managers](#using-linux-
-package-managers) * [Windows](#windows) * [Setting up shell integration]
-(#setting-up-shell-integration) * [As Vim plugin](#as-vim-plugin) * [Upgrading
-fzf](#upgrading-fzf) * [Building fzf](#building-fzf) * [Usage](#usage) * [Using
-the finder](#using-the-finder) * [Layout](#layout) * [Search syntax](#search-
-syntax) * [Environment variables](#environment-variables) * [Options](#options)
-* [Demo](#demo) * [Examples](#examples) * [`fzf-tmux` script](#fzf-tmux-script)
-* [Key bindings for command-line](#key-bindings-for-command-line) * [Fuzzy
-completion for bash and zsh](#fuzzy-completion-for-bash-and-zsh) * [Files and
-directories](#files-and-directories) * [Process IDs](#process-ids) * [Host
-names](#host-names) * [Environment variables / Aliases](#environment-variables-
--aliases) * [Settings](#settings) * [Supported commands](#supported-commands) *
-[Custom fuzzy completion](#custom-fuzzy-completion) * [Vim plugin](#vim-plugin)
-* [Advanced topics](#advanced-topics) * [Performance](#performance) *
-[Executing external programs](#executing-external-programs) * [Turning into a
-different process](#turning-into-a-different-process) * [Reloading the
-candidate list](#reloading-the-candidate-list) * [1. Update the list of
-processes by pressing CTRL-R](#1-update-the-list-of-processes-by-pressing-ctrl-
-r) * [2. Switch between sources by pressing CTRL-D or CTRL-F](#2-switch-
-between-sources-by-pressing-ctrl-d-or-ctrl-f) * [3. Interactive ripgrep
-integration](#3-interactive-ripgrep-integration) * [Preview window](#preview-
-window) * [Previewing an image](#previewing-an-image) * [Tips](#tips) *
-[Respecting `.gitignore`](#respecting-gitignore) * [Fish shell](#fish-shell) *
-[fzf Theme Playground](#fzf-theme-playground) * [Related projects](#related-
-projects) * [License](#license) Installation ------------ fzf project consists
-of the following components: - `fzf` executable - `fzf-tmux` script for
-launching fzf in a tmux pane - Shell integration - Key bindings (`CTRL-T`,
-`CTRL-R`, and `ALT-C`) (bash, zsh, fish) - Fuzzy completion (bash, zsh) - Vim/
-Neovim plugin You can [download fzf executable][bin] alone if you don't need
-the extra stuff. [bin]: https://github.com/junegunn/fzf/releases ### Using
-Homebrew You can use [Homebrew](https://brew.sh/) (on macOS or Linux) to
-install fzf. ```sh brew install fzf ``` > [!IMPORTANT] > To set up shell
-integration (key bindings and fuzzy completion), > see [the instructions below]
-(#setting-up-shell-integration). fzf is also available [via MacPorts]
-[portfile]: `sudo port install fzf` [portfile]: https://github.com/macports/
-macports-ports/blob/master/sysutils/fzf/Portfile ### Using git Alternatively,
-you can "git clone" this repository to any directory and run [install](https://
-github.com/junegunn/fzf/blob/master/install) script. ```sh git clone --depth 1
-https://github.com/junegunn/fzf.git ~/.fzf ~/.fzf/install ``` The install
-script will add lines to your shell configuration file to modify `$PATH` and
-set up shell integration. ### Using Linux package managers | Package Manager |
-Linux Distribution | Command | | --------------- | ----------------------- | --
--------------------------------- | | APK | Alpine Linux | `sudo apk add fzf` |
-| APT | Debian 9+/Ubuntu 19.10+ | `sudo apt install fzf` | | Conda | | `conda
-install -c conda-forge fzf` | | DNF | Fedora | `sudo dnf install fzf` | | Nix |
-NixOS, etc. | `nix-env -iA nixpkgs.fzf` | | Pacman | Arch Linux | `sudo pacman
--S fzf` | | pkg | FreeBSD | `pkg install fzf` | | pkgin | NetBSD | `pkgin
-install fzf` | | pkg_add | OpenBSD | `pkg_add fzf` | | Portage | Gentoo |
-`emerge --ask app-shells/fzf` | | Spack | | `spack install fzf` | | XBPS | Void
-Linux | `sudo xbps-install -S fzf` | | Zypper | openSUSE | `sudo zypper install
-fzf` | > [!IMPORTANT] > To set up shell integration (key bindings and fuzzy
-completion), > see [the instructions below](#setting-up-shell-integration). [!
-[Packaging status](https://repology.org/badge/vertical-allrepos/fzf.svg)]
-(https://repology.org/project/fzf/versions) ### Windows Pre-built binaries for
-Windows can be downloaded [here][bin]. fzf is also available via [Chocolatey]
-[choco], [Scoop][scoop], [Winget][winget], and [MSYS2][msys2]: | Package
-manager | Command | | --------------- | ------------------------------------- |
-| Chocolatey | `choco install fzf` | | Scoop | `scoop install fzf` | | Winget |
+_[_G_l_o_r_i_a_ _Z_h_a_o_]_[_W_i_l_l_ _T_h_o_m_p_s_o_n_]_[_R_o_l_a_n_d_]_[_M_r_._ _H_e_n_r_y_]_[_M_a_u_r_i_c_e_ _L_a_m_]_[_M_a_r_k_u_s
+_K_o_l_l_e_r_]Table of Contents ----------------- * [Installation](#installation) *
+[Using Homebrew](#using-homebrew) * [Using git](#using-git) * [Using Linux
+package managers](#using-linux-package-managers) * [Windows](#windows) *
+[Setting up shell integration](#setting-up-shell-integration) * [As Vim plugin]
+(#as-vim-plugin) * [Upgrading fzf](#upgrading-fzf) * [Building fzf](#building-
+fzf) * [Usage](#usage) * [Using the finder](#using-the-finder) * [Layout]
+(#layout) * [Search syntax](#search-syntax) * [Environment variables]
+(#environment-variables) * [Options](#options) * [Demo](#demo) * [Examples]
+(#examples) * [`fzf-tmux` script](#fzf-tmux-script) * [Key bindings for
+command-line](#key-bindings-for-command-line) * [Fuzzy completion for bash and
+zsh](#fuzzy-completion-for-bash-and-zsh) * [Files and directories](#files-and-
+directories) * [Process IDs](#process-ids) * [Host names](#host-names) *
+[Environment variables / Aliases](#environment-variables--aliases) * [Settings]
+(#settings) * [Supported commands](#supported-commands) * [Custom fuzzy
+completion](#custom-fuzzy-completion) * [Vim plugin](#vim-plugin) * [Advanced
+topics](#advanced-topics) * [Performance](#performance) * [Executing external
+programs](#executing-external-programs) * [Turning into a different process]
+(#turning-into-a-different-process) * [Reloading the candidate list]
+(#reloading-the-candidate-list) * [1. Update the list of processes by pressing
+CTRL-R](#1-update-the-list-of-processes-by-pressing-ctrl-r) * [2. Switch
+between sources by pressing CTRL-D or CTRL-F](#2-switch-between-sources-by-
+pressing-ctrl-d-or-ctrl-f) * [3. Interactive ripgrep integration](#3-
+interactive-ripgrep-integration) * [Preview window](#preview-window) *
+[Previewing an image](#previewing-an-image) * [Tips](#tips) * [Respecting
+`.gitignore`](#respecting-gitignore) * [Fish shell](#fish-shell) * [fzf Theme
+Playground](#fzf-theme-playground) * [Related projects](#related-projects) *
+[License](#license) Installation ------------ fzf project consists of the
+following components: - `fzf` executable - `fzf-tmux` script for launching fzf
+in a tmux pane - Shell integration - Key bindings (`CTRL-T`, `CTRL-R`, and
+`ALT-C`) (bash, zsh, fish) - Fuzzy completion (bash, zsh) - Vim/Neovim plugin
+You can [download fzf executable][bin] alone if you don't need the extra stuff.
+[bin]: https://github.com/junegunn/fzf/releases ### Using Homebrew You can use
+[Homebrew](https://brew.sh/) (on macOS or Linux) to install fzf. ```sh brew
+install fzf ``` > [!IMPORTANT] > To set up shell integration (key bindings and
+fuzzy completion), > see [the instructions below](#setting-up-shell-
+integration). fzf is also available [via MacPorts][portfile]: `sudo port
+install fzf` [portfile]: https://github.com/macports/macports-ports/blob/
+master/sysutils/fzf/Portfile ### Using git Alternatively, you can "git clone"
+this repository to any directory and run [install](https://github.com/junegunn/
+fzf/blob/master/install) script. ```sh git clone --depth 1 https://github.com/
+junegunn/fzf.git ~/.fzf ~/.fzf/install ``` The install script will add lines to
+your shell configuration file to modify `$PATH` and set up shell integration.
+### Using Linux package managers | Package Manager | Linux Distribution |
+Command | | --------------- | ----------------------- | -----------------------
+----------- | | APK | Alpine Linux | `sudo apk add fzf` | | APT | Debian 9+/
+Ubuntu 19.10+ | `sudo apt install fzf` | | Conda | | `conda install -c conda-
+forge fzf` | | DNF | Fedora | `sudo dnf install fzf` | | Nix | NixOS, etc. |
+`nix-env -iA nixpkgs.fzf` | | Pacman | Arch Linux | `sudo pacman -S fzf` | |
+pkg | FreeBSD | `pkg install fzf` | | pkgin | NetBSD | `pkgin install fzf` | |
+pkg_add | OpenBSD | `pkg_add fzf` | | Portage | Gentoo | `emerge --ask app-
+shells/fzf` | | Spack | | `spack install fzf` | | XBPS | Void Linux | `sudo
+xbps-install -S fzf` | | Zypper | openSUSE | `sudo zypper install fzf` | >
+[!IMPORTANT] > To set up shell integration (key bindings and fuzzy completion),
+> see [the instructions below](#setting-up-shell-integration). [![Packaging
+status](https://repology.org/badge/vertical-allrepos/fzf.svg)](https://
+repology.org/project/fzf/versions) ### Windows Pre-built binaries for Windows
+can be downloaded [here][bin]. fzf is also available via [Chocolatey][choco],
+[Scoop][scoop], [Winget][winget], and [MSYS2][msys2]: | Package manager |
+Command | | --------------- | ------------------------------------- | |
+Chocolatey | `choco install fzf` | | Scoop | `scoop install fzf` | | Winget |
 `winget install fzf` | | MSYS2 (pacman) | `pacman -S $MINGW_PACKAGE_PREFIX-fzf`
 | [choco]: https://chocolatey.org/packages/fzf [scoop]: https://github.com/
 ScoopInstaller/Main/blob/master/bucket/fzf.json [winget]: https://github.com/
 microsoft/winget-pkgs/tree/master/manifests/j/junegunn/fzf [msys2]: https://
 packages.msys2.org/base/mingw-w64-fzf Known issues and limitations on Windows
 can be found on [the wiki page][windows-wiki]. [windows-wiki]: https://
 github.com/junegunn/fzf/wiki/Windows ### Setting up shell integration Add the
 following line to your shell configuration file. * bash ```sh # Set up fzf key
 bindings and fuzzy completion eval "$(fzf --bash)" ``` * zsh ```sh # Set up fzf
 key bindings and fuzzy completion eval "$(fzf --zsh)" ``` * fish ```fish # Set
 up fzf key bindings fzf --fish | source ``` > [!NOTE] > `--bash`, `--zsh`, and
-`--fish` options are only available in > fzf 0.48.0 or above. If you have an
-older version of fzf, refer to the > package documentation for more
-information. (e.g. `apt show fzf`) > [!TIP] > You can disable CTRL-T or ALT-
-C binding by setting `FZF_CTRL_T_COMMAND` or > `FZF_ALT_C_COMMAND` to an empty
-string when sourcing the script. > For example, to disable ALT-C binding: > > *
-bash: `FZF_ALT_C_COMMAND= eval "$(fzf --bash)"` > * zsh: `FZF_ALT_C_COMMAND=
-eval "$(fzf --zsh)"` > * fish: `fzf --fish | FZF_ALT_C_COMMAND= source` > >
-Setting the variables after sourcing the script will have no effect. ### As Vim
-plugin If you use [vim-plug](https://github.com/junegunn/vim-plug), add this
-line to your Vim configuration file: ```vim Plug 'junegunn/fzf', { 'do': { -
-> fzf#install() } } ``` `fzf#install()` makes sure that you have the latest
-binary, but it's optional, so you can omit it if you use a plugin manager that
-doesn't support hooks. For more installation options, see [README-VIM.md]
-(README-VIM.md). Upgrading fzf ------------- fzf is being actively developed,
-and you might want to upgrade it once in a while. Please follow the instruction
-below depending on the installation method used. - git: `cd ~/.fzf && git pull
-&& ./install` - brew: `brew update; brew upgrade fzf` - macports: `sudo port
-upgrade fzf` - chocolatey: `choco upgrade fzf` - vim-plug: `:PlugUpdate fzf`
-Building fzf ------------ See [BUILD.md](BUILD.md). Usage ----- fzf will launch
-interactive finder, read the list from STDIN, and write the selected item to
-STDOUT. ```sh find * -type f | fzf > selected ``` Without STDIN pipe, fzf will
-traverse the file system under the current directory to get the list of files.
-```sh vim $(fzf) ``` > [!NOTE] > You can override the default behavior > *
-Either by setting `$FZF_DEFAULT_COMMAND` to a command that generates the
-desired list > * Or by setting `--walker`, `--walker-root`, and `--walker-skip`
-options in `$FZF_DEFAULT_OPTS` > [!WARNING] > A more robust solution would be
-to use `xargs` but we've presented > the above as it's easier to grasp > ```sh
-> fzf --print0 | xargs -0 -o vim > ``` > [!TIP] > fzf also has the ability to
-turn itself into a different process. > > ```sh > fzf --bind 'enter:become(vim
-{})' > ``` > > *See [Turning into a different process](#turning-into-a-
-different-process) > for more information.* ### Using the finder - `CTRL-K` /
-`CTRL-J` (or `CTRL-P` / `CTRL-N`) to move cursor up and down - `Enter` key to
-select the item, `CTRL-C` / `CTRL-G` / `ESC` to exit - On multi-select mode (`-
-m`), `TAB` and `Shift-TAB` to mark multiple items - Emacs style key bindings -
-Mouse: scroll, click, double-click; shift-click and shift-scroll on multi-
-select mode ### Layout fzf by default starts in fullscreen mode, but you can
-make it start below the cursor with `--height` option. ```sh vim $(fzf --height
-40%) ``` Also, check out `--reverse` and `--layout` options if you prefer "top-
-down" layout instead of the default "bottom-up" layout. ```sh vim $(fzf --
-height 40% --reverse) ``` You can add these options to `$FZF_DEFAULT_OPTS` so
-that they're applied by default. For example, ```sh export FZF_DEFAULT_OPTS='--
-height 40% --layout=reverse --border' ``` ### Search syntax Unless otherwise
-specified, fzf starts in "extended-search mode" where you can type in multiple
-search terms delimited by spaces. e.g. `^music .mp3$ sbtrkt !fire` | Token |
-Match type | Description | | --------- | -------------------------- | ---------
---------------------------- | | `sbtrkt` | fuzzy-match | Items that match
-`sbtrkt` | | `'wild` | exact-match (quoted) | Items that include `wild` | |
-`^music` | prefix-exact-match | Items that start with `music` | | `.mp3$` |
-suffix-exact-match | Items that end with `.mp3` | | `!fire` | inverse-exact-
-match | Items that do not include `fire` | | `!^music` | inverse-prefix-exact-
-match | Items that do not start with `music` | | `!.mp3$` | inverse-suffix-
-exact-match | Items that do not end with `.mp3` | If you don't prefer fuzzy
-matching and do not wish to "quote" every word, start fzf with `-e` or `--
-exact` option. Note that when `--exact` is set, `'`-prefix "unquotes" the term.
-A single bar character term acts as an OR operator. For example, the following
-query matches entries that start with `core` and end with either `go`, `rb`, or
-`py`. ``` ^core go$ | rb$ | py$ ``` ### Environment variables -
-`FZF_DEFAULT_COMMAND` - Default command to use when input is tty - e.g. `export
-FZF_DEFAULT_COMMAND='fd --type f'` - `FZF_DEFAULT_OPTS` - Default options -
-e.g. `export FZF_DEFAULT_OPTS="--layout=reverse --inline-info"` -
-`FZF_DEFAULT_OPTS_FILE` - If you prefer to manage default options in a file,
-set this variable to point to the location of the file - e.g. `export
-FZF_DEFAULT_OPTS_FILE=~/.fzfrc` > [!WARNING] > `FZF_DEFAULT_COMMAND` is not
-used by shell integration due to the > slight difference in requirements. > > *
-`CTRL-T` runs `$FZF_CTRL_T_COMMAND` to get a list of files and directories > *
-`ALT-C` runs `$FZF_ALT_C_COMMAND` to get a list of directories > * `vim ~/**`
-runs `fzf_compgen_path()` with the prefix (`~/`) as the first argument > * `cd
-foo**` runs `fzf_compgen_dir()` with the prefix (`foo`) as the first argument >
-> The available options are described later in this document. ### Options See
-the man page (`man fzf`) for the full list of options. ### Demo If you learn by
-watching videos, check out this screencast by [@samoshkin](https://github.com/
-samoshkin) to explore `fzf` features. _[_h_t_t_p_s_:_/_/_i_._i_m_g_u_r_._c_o_m_/_v_t_G_8_o_l_E_._p_n_g_]Examples
--------- * [Wiki page of examples](https://github.com/junegunn/fzf/wiki/
-examples) * *Disclaimer: The examples on this page are maintained by the
-community and are not thoroughly tested* * [Advanced fzf examples](https://
-github.com/junegunn/fzf/blob/master/ADVANCED.md) `fzf-tmux` script ------------
------ [fzf-tmux](bin/fzf-tmux) is a bash script that opens fzf in a tmux pane.
-```sh # usage: fzf-tmux [LAYOUT OPTIONS] [--] [FZF OPTIONS] # See available
-options fzf-tmux --help # select git branches in horizontal split below (15
-lines) git branch | fzf-tmux -d 15 # select multiple words in vertical split on
-the left (20% of screen width) cat /usr/share/dict/words | fzf-tmux -l 20% --
-multi --reverse ``` It will still work even when you're not on tmux, silently
-ignoring `-[pudlr]` options, so you can invariably use `fzf-tmux` in your
-scripts. Alternatively, you can use `--height HEIGHT[%]` option not to start
-fzf in fullscreen mode. ```sh fzf --height 40% ``` Key bindings for command-
-line ----------------------------- The install script will setup the following
-key bindings for bash, zsh, and fish. - `CTRL-T` - Paste the selected files and
-directories onto the command-line - The list is generated using `--walker
-file,dir,follow,hidden` option - You can override the behavior by setting
-`FZF_CTRL_T_COMMAND` to a custom command that generates the desired list - Or
-you can set `--walker*` options in `FZF_CTRL_T_OPTS` - Set `FZF_CTRL_T_OPTS` to
-pass additional options to fzf ```sh # Preview file content using bat (https://
-github.com/sharkdp/bat) export FZF_CTRL_T_OPTS=" --walker-skip
-.git,node_modules,target --preview 'bat -n --color=always {}' --bind 'ctrl-/:
-change-preview-window(down|hidden|)'" ``` - Can be disabled by setting
-`FZF_CTRL_T_COMMAND` to an empty string when sourcing the script - `CTRL-R` -
-Paste the selected command from history onto the command-line - If you want to
-see the commands in chronological order, press `CTRL-R` again which toggles
-sorting by relevance - Set `FZF_CTRL_R_OPTS` to pass additional options to fzf
-```sh # CTRL-/ to toggle small preview window to see the full command # CTRL-
-Y to copy the command into clipboard using pbcopy export FZF_CTRL_R_OPTS=" --
-preview 'echo {}' --preview-window up:3:hidden:wrap --bind 'ctrl-/:toggle-
+`--fish` options are only available in fzf 0.48.0 or > later. If you have an
+older version of fzf, or want finer control, you can > source individual script
+files in the [/shell](/shell) directory. The > location of the files may vary
+depending on the package manager you use. > Please refer to the package
+documentation for more information. > (e.g. `apt show fzf`) > [!TIP] > You can
+disable CTRL-T or ALT-C binding by setting `FZF_CTRL_T_COMMAND` or >
+`FZF_ALT_C_COMMAND` to an empty string when sourcing the script. > For example,
+to disable ALT-C binding: > > * bash: `FZF_ALT_C_COMMAND= eval "$(fzf --bash)"`
+> * zsh: `FZF_ALT_C_COMMAND= eval "$(fzf --zsh)"` > * fish: `fzf --fish |
+FZF_ALT_C_COMMAND= source` > > Setting the variables after sourcing the script
+will have no effect. ### As Vim plugin If you use [vim-plug](https://
+github.com/junegunn/vim-plug), add this line to your Vim configuration file:
+```vim Plug 'junegunn/fzf', { 'do': { -> fzf#install() } } ``` `fzf#install()`
+makes sure that you have the latest binary, but it's optional, so you can omit
+it if you use a plugin manager that doesn't support hooks. For more
+installation options, see [README-VIM.md](README-VIM.md). Upgrading fzf -------
+------ fzf is being actively developed, and you might want to upgrade it once
+in a while. Please follow the instruction below depending on the installation
+method used. - git: `cd ~/.fzf && git pull && ./install` - brew: `brew update;
+brew upgrade fzf` - macports: `sudo port upgrade fzf` - chocolatey: `choco
+upgrade fzf` - vim-plug: `:PlugUpdate fzf` Building fzf ------------ See
+[BUILD.md](BUILD.md). Usage ----- fzf will launch interactive finder, read the
+list from STDIN, and write the selected item to STDOUT. ```sh find * -type f |
+fzf > selected ``` Without STDIN pipe, fzf will traverse the file system under
+the current directory to get the list of files. ```sh vim $(fzf) ``` > [!NOTE]
+> You can override the default behavior > * Either by setting
+`$FZF_DEFAULT_COMMAND` to a command that generates the desired list > * Or by
+setting `--walker`, `--walker-root`, and `--walker-skip` options in
+`$FZF_DEFAULT_OPTS` > [!WARNING] > A more robust solution would be to use
+`xargs` but we've presented > the above as it's easier to grasp > ```sh > fzf -
+-print0 | xargs -0 -o vim > ``` > [!TIP] > fzf also has the ability to turn
+itself into a different process. > > ```sh > fzf --bind 'enter:become(vim {})'
+> ``` > > *See [Turning into a different process](#turning-into-a-different-
+process) > for more information.* ### Using the finder - `CTRL-K` / `CTRL-J`
+(or `CTRL-P` / `CTRL-N`) to move cursor up and down - `Enter` key to select the
+item, `CTRL-C` / `CTRL-G` / `ESC` to exit - On multi-select mode (`-m`), `TAB`
+and `Shift-TAB` to mark multiple items - Emacs style key bindings - Mouse:
+scroll, click, double-click; shift-click and shift-scroll on multi-select mode
+### Layout fzf by default starts in fullscreen mode, but you can make it start
+below the cursor with `--height` option. ```sh vim $(fzf --height 40%) ```
+Also, check out `--reverse` and `--layout` options if you prefer "top-down"
+layout instead of the default "bottom-up" layout. ```sh vim $(fzf --height 40%
+--reverse) ``` You can add these options to `$FZF_DEFAULT_OPTS` so that they're
+applied by default. For example, ```sh export FZF_DEFAULT_OPTS='--height 40% --
+layout=reverse --border' ``` ### Search syntax Unless otherwise specified, fzf
+starts in "extended-search mode" where you can type in multiple search terms
+delimited by spaces. e.g. `^music .mp3$ sbtrkt !fire` | Token | Match type |
+Description | | --------- | -------------------------- | ----------------------
+-------------- | | `sbtrkt` | fuzzy-match | Items that match `sbtrkt` | |
+`'wild` | exact-match (quoted) | Items that include `wild` | | `^music` |
+prefix-exact-match | Items that start with `music` | | `.mp3$` | suffix-exact-
+match | Items that end with `.mp3` | | `!fire` | inverse-exact-match | Items
+that do not include `fire` | | `!^music` | inverse-prefix-exact-match | Items
+that do not start with `music` | | `!.mp3$` | inverse-suffix-exact-match |
+Items that do not end with `.mp3` | If you don't prefer fuzzy matching and do
+not wish to "quote" every word, start fzf with `-e` or `--exact` option. Note
+that when `--exact` is set, `'`-prefix "unquotes" the term. A single bar
+character term acts as an OR operator. For example, the following query matches
+entries that start with `core` and end with either `go`, `rb`, or `py`. ```
+^core go$ | rb$ | py$ ``` ### Environment variables - `FZF_DEFAULT_COMMAND` -
+Default command to use when input is tty - e.g. `export FZF_DEFAULT_COMMAND='fd
+--type f'` - `FZF_DEFAULT_OPTS` - Default options - e.g. `export
+FZF_DEFAULT_OPTS="--layout=reverse --inline-info"` - `FZF_DEFAULT_OPTS_FILE` -
+If you prefer to manage default options in a file, set this variable to point
+to the location of the file - e.g. `export FZF_DEFAULT_OPTS_FILE=~/.fzfrc` >
+[!WARNING] > `FZF_DEFAULT_COMMAND` is not used by shell integration due to the
+> slight difference in requirements. > > * `CTRL-T` runs `$FZF_CTRL_T_COMMAND`
+to get a list of files and directories > * `ALT-C` runs `$FZF_ALT_C_COMMAND` to
+get a list of directories > * `vim ~/**` runs `fzf_compgen_path()` with the
+prefix (`~/`) as the first argument > * `cd foo**` runs `fzf_compgen_dir()`
+with the prefix (`foo`) as the first argument > > The available options are
+described later in this document. ### Options See the man page (`man fzf`) for
+the full list of options. ### Demo If you learn by watching videos, check out
+this screencast by [@samoshkin](https://github.com/samoshkin) to explore `fzf`
+features. _[_h_t_t_p_s_:_/_/_i_._i_m_g_u_r_._c_o_m_/_v_t_G_8_o_l_E_._p_n_g_]Examples -------- * [Wiki page of
+examples](https://github.com/junegunn/fzf/wiki/examples) * *Disclaimer: The
+examples on this page are maintained by the community and are not thoroughly
+tested* * [Advanced fzf examples](https://github.com/junegunn/fzf/blob/master/
+ADVANCED.md) `fzf-tmux` script ----------------- [fzf-tmux](bin/fzf-tmux) is a
+bash script that opens fzf in a tmux pane. ```sh # usage: fzf-tmux [LAYOUT
+OPTIONS] [--] [FZF OPTIONS] # See available options fzf-tmux --help # select
+git branches in horizontal split below (15 lines) git branch | fzf-tmux -d 15 #
+select multiple words in vertical split on the left (20% of screen width) cat /
+usr/share/dict/words | fzf-tmux -l 20% --multi --reverse ``` It will still work
+even when you're not on tmux, silently ignoring `-[pudlr]` options, so you can
+invariably use `fzf-tmux` in your scripts. Alternatively, you can use `--height
+HEIGHT[%]` option not to start fzf in fullscreen mode. ```sh fzf --height 40%
+``` Key bindings for command-line ----------------------------- The install
+script will setup the following key bindings for bash, zsh, and fish. - `CTRL-
+T` - Paste the selected files and directories onto the command-line - The list
+is generated using `--walker file,dir,follow,hidden` option - You can override
+the behavior by setting `FZF_CTRL_T_COMMAND` to a custom command that generates
+the desired list - Or you can set `--walker*` options in `FZF_CTRL_T_OPTS` -
+Set `FZF_CTRL_T_OPTS` to pass additional options to fzf ```sh # Preview file
+content using bat (https://github.com/sharkdp/bat) export FZF_CTRL_T_OPTS=" --
+walker-skip .git,node_modules,target --preview 'bat -n --color=always {}' --
+bind 'ctrl-/:change-preview-window(down|hidden|)'" ``` - Can be disabled by
+setting `FZF_CTRL_T_COMMAND` to an empty string when sourcing the script -
+`CTRL-R` - Paste the selected command from history onto the command-line - If
+you want to see the commands in chronological order, press `CTRL-R` again which
+toggles sorting by relevance - Set `FZF_CTRL_R_OPTS` to pass additional options
+to fzf ```sh # CTRL-/ to toggle small preview window to see the full command #
+CTRL-Y to copy the command into clipboard using pbcopy export FZF_CTRL_R_OPTS="
+--preview 'echo {}' --preview-window up:3:hidden:wrap --bind 'ctrl-/:toggle-
 preview' --bind 'ctrl-y:execute-silent(echo -n {2..} | pbcopy)+abort' --color
 header:italic --header 'Press CTRL-Y to copy command into clipboard'" ``` -
 `ALT-C` - cd into the selected directory - The list is generated using `--
 walker dir,follow,hidden` option - Set `FZF_ALT_C_COMMAND` to override the
 default command - Or you can set `--walker-*` options in `FZF_ALT_C_OPTS` - Set
 `FZF_ALT_C_OPTS` to pass additional options to fzf ```sh # Print tree structure
 in the preview window export FZF_ALT_C_OPTS=" --walker-skip
```

### Comparing `fzf_bin-0.48.1/fzf/bin/fzf-preview.sh` & `fzf_bin-0.49.0/fzf/bin/fzf-preview.sh`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/bin/fzf-tmux` & `fzf_bin-0.49.0/fzf/bin/fzf-tmux`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/doc/fzf.txt` & `fzf_bin-0.49.0/fzf/doc/fzf.txt`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/go.sum` & `fzf_bin-0.49.0/fzf/go.sum`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-github.com/charlievieth/fastwalk v1.0.2 h1:KYWo7xszmoldOGrwdNIeznSzhj9mhgk+6DwHunG99bc=
-github.com/charlievieth/fastwalk v1.0.2/go.mod h1:JSfglY/gmL/rqsUS1NCsJTocB5n6sSl9ApAqif4CUbs=
+github.com/charlievieth/fastwalk v1.0.3 h1:eNWFaNPe5srPqQ5yyDbhAf11paeZaHWcihRhpuYFfSg=
+github.com/charlievieth/fastwalk v1.0.3/go.mod h1:JSfglY/gmL/rqsUS1NCsJTocB5n6sSl9ApAqif4CUbs=
 github.com/gdamore/encoding v1.0.0 h1:+7OoQ1Bc6eTm5niUzBa0Ctsh6JbMW6Ra+YNuAtDBdko=
 github.com/gdamore/encoding v1.0.0/go.mod h1:alR0ol34c49FCSBLjhosxzcPHQbf2trDkoo5dl+VrEg=
 github.com/gdamore/tcell/v2 v2.7.4 h1:sg6/UnTM9jGpZU+oFYAsDahfchWAFW8Xx2yFinNSAYU=
 github.com/gdamore/tcell/v2 v2.7.4/go.mod h1:dSXtXTSK0VsW1biw65DZLZ2NKr7j0qP/0J7ONmsraWg=
 github.com/lucasb-eyer/go-colorful v1.2.0 h1:1nnpGOrhyZZuNyfu1QjKiUICQ74+3FNCN69Aj6K7nkY=
 github.com/lucasb-eyer/go-colorful v1.2.0/go.mod h1:R4dSotOR9KMtayYi1e77YzuveK+i7ruzyGqttikkLy0=
 github.com/mattn/go-isatty v0.0.20 h1:xfD0iDuEKnDkl03q4limB+vH+GxLEtL/jb4xVJSWWEY=
```

### Comparing `fzf_bin-0.48.1/fzf/install` & `fzf_bin-0.49.0/fzf/install`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env bash
 
 set -u
 
-version=0.48.1
+version=0.49.0
 auto_completion=
 key_bindings=
 update_config=2
 shells="bash zsh fish"
 prefix='~/.fzf'
 prefix_expand=~/.fzf
 fish_dir=${XDG_CONFIG_HOME:-$HOME/.config}/fish
```

### Comparing `fzf_bin-0.48.1/fzf/install.ps1` & `fzf_bin-0.49.0/fzf/install.ps1`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-$version="0.48.1"
+$version="0.49.0"
 
 $fzf_base=Split-Path -Parent $MyInvocation.MyCommand.Definition
 
 function check_binary () {
   Write-Host "  - Checking fzf executable ... " -NoNewline
   $output=cmd /c $fzf_base\bin\fzf.exe --version 2>&1
   if (-not $?) {
```

### Comparing `fzf_bin-0.48.1/fzf/main.go` & `fzf_bin-0.49.0/fzf/main.go`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	"fmt"
 	"strings"
 
 	fzf "github.com/junegunn/fzf/src"
 	"github.com/junegunn/fzf/src/protector"
 )
 
-var version string = "0.48"
+var version string = "0.49"
 var revision string = "devel"
 
 //go:embed shell/key-bindings.bash
 var bashKeyBindings []byte
 
 //go:embed shell/completion.bash
 var bashCompletion []byte
```

### Comparing `fzf_bin-0.48.1/fzf/man/man1/fzf-tmux.1` & `fzf_bin-0.49.0/fzf/man/man1/fzf-tmux.1`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 ..
-.TH fzf-tmux 1 "Mar 2024" "fzf 0.48.1" "fzf-tmux - open fzf in tmux split pane"
+.TH fzf-tmux 1 "Apr 2024" "fzf 0.49.0" "fzf-tmux - open fzf in tmux split pane"
 
 .SH NAME
 fzf-tmux - open fzf in tmux split pane
 
 .SH SYNOPSIS
 .B fzf-tmux [LAYOUT OPTIONS] [--] [FZF OPTIONS]
```

### Comparing `fzf_bin-0.48.1/fzf/man/man1/fzf.1` & `fzf_bin-0.49.0/fzf/man/man1/fzf.1`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 ..
-.TH fzf 1 "Mar 2024" "fzf 0.48.1" "fzf - a command-line fuzzy finder"
+.TH fzf 1 "Apr 2024" "fzf 0.49.0" "fzf - a command-line fuzzy finder"
 
 .SH NAME
 fzf - a command-line fuzzy finder
 
 .SH SYNOPSIS
 fzf [options]
 
@@ -368,28 +368,29 @@
 .br
 .BR T,R,B,L "  Top, right, bottom, left padding"
 .br
 .RE
 
 .TP
 .BI "--info=" "STYLE"
-Determines the display style of finder info (match counters).
+Determines the display style of the finder info. (e.g. match counter, loading indicator, etc.)
 
+.BR default "              On the left end of the horizontal separator"
 .br
-.BR default "          Display on the next line to the prompt"
+.BR right "                On the right end of the horizontal separator"
 .br
-.BR right "            Display on the right end of the next line to the prompt"
+.BR hidden "               Do not display finder info"
 .br
-.BR inline "           Display on the same line with the default separator ' < '"
+.BR inline "               After the prompt with the default prefix ' < '"
 .br
-.BR inline:SEPARATOR " Display on the same line with a non-default separator"
+.BR inline:PREFIX "        After the prompt with a non-default prefix"
 .br
-.BR inline-right "     Display on the right end of the same line
+.BR inline-right "         On the right end of the prompt line"
 .br
-.BR hidden "           Do not display finder info"
+.BR inline-right:PREFIX "  On the right end of the prompt line with a custom prefix"
 .br
 
 .TP
 .B "--no-info"
 A synonym for \fB--info=hidden\fB
 
 .TP
@@ -971,14 +972,18 @@
 .br
 .BR FZF_SELECT_COUNT "    Number of selected items"
 .br
 .BR FZF_QUERY "           Current query string"
 .br
 .BR FZF_PROMPT "          Prompt string"
 .br
+.BR FZF_PREVIEW_LABEL "   Preview label string"
+.br
+.BR FZF_BORDER_LABEL "    Border label string"
+.br
 .BR FZF_ACTION "          The name of the last action performed"
 .br
 .BR FZF_PORT "            Port number when --listen option is used"
 .br
 
 The following variables are additionally exported to the preview commands.
 
@@ -1322,26 +1327,28 @@
     \fBtoggle-header\fR
     \fBtoggle-in\fR                    (\fB--layout=reverse*\fR ? \fBtoggle+up\fR : \fBtoggle+down\fR)
     \fBtoggle-out\fR                   (\fB--layout=reverse*\fR ? \fBtoggle+down\fR : \fBtoggle+up\fR)
     \fBtoggle-preview\fR
     \fBtoggle-preview-wrap\fR
     \fBtoggle-search\fR                (toggle search functionality)
     \fBtoggle-sort\fR
-    \fBtoggle-track\fR
+    \fBtoggle-track\fR                 (toggle global tracking option (\fB--track\fR))
+    \fBtoggle-track-current\fR         (toggle tracking of the current item)
     \fBtoggle+up\fR                    \fIbtab    (shift-tab)\fR
-    \fBtrack\fR                        (track the current item; automatically disabled if focus changes)
+    \fBtrack-current\fR                (track the current item; automatically disabled if focus changes)
     \fBtransform(...)\fR               (transform states using the output of an external command)
     \fBtransform-border-label(...)\fR  (transform border label using an external command)
     \fBtransform-header(...)\fR        (transform header using an external command)
     \fBtransform-preview-label(...)\fR (transform preview label using an external command)
     \fBtransform-prompt(...)\fR        (transform prompt string using an external command)
     \fBtransform-query(...)\fR         (transform query string using an external command)
     \fBunbind(...)\fR                  (unbind bindings)
     \fBunix-line-discard\fR            \fIctrl-u\fR
     \fBunix-word-rubout\fR             \fIctrl-w\fR
+    \fBuntrack-current\fR              (stop tracking the current item; no-op if global tracking is enabled)
     \fBup\fR                           \fIctrl-k  ctrl-p  up\fR
     \fByank\fR                         \fIctrl-y\fR
 
 .SS ACTION COMPOSITION
 
 Multiple actions can be chained using \fB+\fR separator.
```

### Comparing `fzf_bin-0.48.1/fzf/plugin/fzf.vim` & `fzf_bin-0.49.0/fzf/plugin/fzf.vim`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/shell/completion.bash` & `fzf_bin-0.49.0/fzf/shell/completion.bash`

 * *Files 0% similar despite different names*

```diff
@@ -304,14 +304,15 @@
 
       if [[ "${__fzf_nospace_commands-}" = *" $orig_cmd "* ]]; then
         eval "${orig_complete/ -F / -o nospace -F }"
       else
         eval "$orig_complete"
       fi
     fi
+    [[ $ret -eq 0 ]] && return 124
     return $ret
   fi
 }
 
 __fzf_generic_path_completion() {
   local cur base dir leftover matches trigger cmd
   cmd="${COMP_WORDS[0]}"
@@ -543,15 +544,15 @@
 # Anything
 for cmd in $a_cmds; do
   __fzf_defc "$cmd" _fzf_path_completion "-o default -o bashdefault"
 done
 
 # Directory
 for cmd in $d_cmds; do
-  __fzf_defc "$cmd" _fzf_dir_completion "-o nospace -o dirnames"
+  __fzf_defc "$cmd" _fzf_dir_completion "-o bashdefault -o nospace -o dirnames"
 done
 
 # ssh
 __fzf_defc ssh _fzf_complete_ssh "-o default -o bashdefault"
 
 unset cmd d_cmds a_cmds
```

### Comparing `fzf_bin-0.48.1/fzf/shell/completion.zsh` & `fzf_bin-0.49.0/fzf/shell/completion.zsh`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/shell/key-bindings.bash` & `fzf_bin-0.49.0/fzf/shell/key-bindings.bash`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 }
 
 __fzf_cd__() {
   local opts dir
   opts="--height ${FZF_TMUX_HEIGHT:-40%} --bind=ctrl-z:ignore --reverse --walker=dir,follow,hidden --scheme=path ${FZF_DEFAULT_OPTS-} ${FZF_ALT_C_OPTS-} +m"
   dir=$(
     FZF_DEFAULT_COMMAND=${FZF_ALT_C_COMMAND:-} FZF_DEFAULT_OPTS="$opts" $(__fzfcmd)
-  ) && printf 'builtin cd -- %q' "$dir"
+  ) && printf 'builtin cd -- %q' "$(builtin unset CDPATH && builtin cd -- "$dir" && builtin pwd)"
 }
 
 if command -v perl > /dev/null; then
   __fzf_history__() {
     local output opts script
     opts="--height ${FZF_TMUX_HEIGHT:-40%} --bind=ctrl-z:ignore ${FZF_DEFAULT_OPTS-} -n2..,.. --scheme=history --bind=ctrl-r:toggle-sort ${FZF_CTRL_R_OPTS-} +m --read0"
     script='BEGIN { getc; $/ = "\n\t"; $HISTCOUNT = $ENV{last_hist} + 1 } s/^[ *]//; print $HISTCOUNT - $. . "\t$_" if !$seen{$_}++'
```

### Comparing `fzf_bin-0.48.1/fzf/shell/key-bindings.fish` & `fzf_bin-0.49.0/fzf/shell/key-bindings.fish`

 * *Files 7% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 # Key bindings
 # ------------
 function fzf_key_bindings
 
   # Store current token in $dir as root for the 'find' command
   function fzf-file-widget -d "List files and folders"
     set -l commandline (__fzf_parse_commandline)
-    set -l dir $commandline[1]
+    set -lx dir $commandline[1]
     set -l fzf_query $commandline[2]
     set -l prefix $commandline[3]
 
     test -n "$FZF_TMUX_HEIGHT"; or set FZF_TMUX_HEIGHT 40%
     begin
-      set -lx FZF_DEFAULT_OPTS "--height $FZF_TMUX_HEIGHT --reverse --walker=file,dir,follow,hidden --scheme=path --bind=ctrl-z:ignore $FZF_DEFAULT_OPTS $FZF_CTRL_T_OPTS"
+      set -lx FZF_DEFAULT_OPTS "--height $FZF_TMUX_HEIGHT --reverse --walker=file,dir,follow,hidden --walker-root='$dir' --scheme=path --bind=ctrl-z:ignore $FZF_DEFAULT_OPTS $FZF_CTRL_T_OPTS"
       set -lx FZF_DEFAULT_COMMAND "$FZF_CTRL_T_COMMAND"
       eval (__fzfcmd)' -m --query "'$fzf_query'"' | while read -l r; set result $result $r; end
     end
     if [ -z "$result" ]
       commandline -f repaint
       return
     else
@@ -66,21 +66,21 @@
       end
     end
     commandline -f repaint
   end
 
   function fzf-cd-widget -d "Change directory"
     set -l commandline (__fzf_parse_commandline)
-    set -l dir $commandline[1]
+    set -lx dir $commandline[1]
     set -l fzf_query $commandline[2]
     set -l prefix $commandline[3]
 
     test -n "$FZF_TMUX_HEIGHT"; or set FZF_TMUX_HEIGHT 40%
     begin
-      set -lx FZF_DEFAULT_OPTS "--height $FZF_TMUX_HEIGHT --reverse --walker=dir,follow,hidden --scheme=path --bind=ctrl-z:ignore $FZF_DEFAULT_OPTS $FZF_ALT_C_OPTS"
+      set -lx FZF_DEFAULT_OPTS "--height $FZF_TMUX_HEIGHT --reverse --walker=dir,follow,hidden --walker-root='$dir' --scheme=path --bind=ctrl-z:ignore $FZF_DEFAULT_OPTS $FZF_ALT_C_OPTS"
       set -lx FZF_DEFAULT_COMMAND "$FZF_ALT_C_COMMAND"
       eval (__fzfcmd)' +m --query "'$fzf_query'"' | read -l result
 
       if [ -n "$result" ]
         cd -- $result
 
         # Remove last token from commandline.
```

### Comparing `fzf_bin-0.48.1/fzf/shell/key-bindings.zsh` & `fzf_bin-0.49.0/fzf/shell/key-bindings.zsh`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
   setopt localoptions pipefail no_aliases 2> /dev/null
   local dir="$(FZF_DEFAULT_COMMAND=${FZF_ALT_C_COMMAND:-} FZF_DEFAULT_OPTS="--height ${FZF_TMUX_HEIGHT:-40%} --reverse --walker=dir,follow,hidden --scheme=path --bind=ctrl-z:ignore ${FZF_DEFAULT_OPTS-} ${FZF_ALT_C_OPTS-}" $(__fzfcmd) +m < /dev/tty)"
   if [[ -z "$dir" ]]; then
     zle redisplay
     return 0
   fi
   zle push-line # Clear buffer. Auto-restored on next prompt.
-  BUFFER="builtin cd -- ${(q)dir}"
+  BUFFER="builtin cd -- ${(q)dir:a}"
   zle accept-line
   local ret=$?
   unset dir # ensure this doesn't end up appearing in prompt expansion
   zle reset-prompt
   return $ret
 }
 if [[ "${FZF_ALT_C_COMMAND-x}" != "" ]]; then
```

### Comparing `fzf_bin-0.48.1/fzf/src/LICENSE` & `fzf_bin-0.49.0/fzf/src/LICENSE`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/actiontype_string.go` & `fzf_bin-0.49.0/fzf/src/actiontype_string.go`

 * *Files 7% similar despite different names*

```diff
@@ -50,80 +50,82 @@
 	_ = x[actToggleSearch-39]
 	_ = x[actToggleAll-40]
 	_ = x[actToggleDown-41]
 	_ = x[actToggleUp-42]
 	_ = x[actToggleIn-43]
 	_ = x[actToggleOut-44]
 	_ = x[actToggleTrack-45]
-	_ = x[actToggleHeader-46]
-	_ = x[actTrack-47]
-	_ = x[actDown-48]
-	_ = x[actUp-49]
-	_ = x[actPageUp-50]
-	_ = x[actPageDown-51]
-	_ = x[actPosition-52]
-	_ = x[actHalfPageUp-53]
-	_ = x[actHalfPageDown-54]
-	_ = x[actOffsetUp-55]
-	_ = x[actOffsetDown-56]
-	_ = x[actJump-57]
-	_ = x[actJumpAccept-58]
-	_ = x[actPrintQuery-59]
-	_ = x[actRefreshPreview-60]
-	_ = x[actReplaceQuery-61]
-	_ = x[actToggleSort-62]
-	_ = x[actShowPreview-63]
-	_ = x[actHidePreview-64]
-	_ = x[actTogglePreview-65]
-	_ = x[actTogglePreviewWrap-66]
-	_ = x[actTransform-67]
-	_ = x[actTransformBorderLabel-68]
-	_ = x[actTransformHeader-69]
-	_ = x[actTransformPreviewLabel-70]
-	_ = x[actTransformPrompt-71]
-	_ = x[actTransformQuery-72]
-	_ = x[actPreview-73]
-	_ = x[actChangePreview-74]
-	_ = x[actChangePreviewWindow-75]
-	_ = x[actPreviewTop-76]
-	_ = x[actPreviewBottom-77]
-	_ = x[actPreviewUp-78]
-	_ = x[actPreviewDown-79]
-	_ = x[actPreviewPageUp-80]
-	_ = x[actPreviewPageDown-81]
-	_ = x[actPreviewHalfPageUp-82]
-	_ = x[actPreviewHalfPageDown-83]
-	_ = x[actPrevHistory-84]
-	_ = x[actPrevSelected-85]
-	_ = x[actPut-86]
-	_ = x[actNextHistory-87]
-	_ = x[actNextSelected-88]
-	_ = x[actExecute-89]
-	_ = x[actExecuteSilent-90]
-	_ = x[actExecuteMulti-91]
-	_ = x[actSigStop-92]
-	_ = x[actFirst-93]
-	_ = x[actLast-94]
-	_ = x[actReload-95]
-	_ = x[actReloadSync-96]
-	_ = x[actDisableSearch-97]
-	_ = x[actEnableSearch-98]
-	_ = x[actSelect-99]
-	_ = x[actDeselect-100]
-	_ = x[actUnbind-101]
-	_ = x[actRebind-102]
-	_ = x[actBecome-103]
-	_ = x[actResponse-104]
-	_ = x[actShowHeader-105]
-	_ = x[actHideHeader-106]
+	_ = x[actToggleTrackCurrent-46]
+	_ = x[actToggleHeader-47]
+	_ = x[actTrackCurrent-48]
+	_ = x[actUntrackCurrent-49]
+	_ = x[actDown-50]
+	_ = x[actUp-51]
+	_ = x[actPageUp-52]
+	_ = x[actPageDown-53]
+	_ = x[actPosition-54]
+	_ = x[actHalfPageUp-55]
+	_ = x[actHalfPageDown-56]
+	_ = x[actOffsetUp-57]
+	_ = x[actOffsetDown-58]
+	_ = x[actJump-59]
+	_ = x[actJumpAccept-60]
+	_ = x[actPrintQuery-61]
+	_ = x[actRefreshPreview-62]
+	_ = x[actReplaceQuery-63]
+	_ = x[actToggleSort-64]
+	_ = x[actShowPreview-65]
+	_ = x[actHidePreview-66]
+	_ = x[actTogglePreview-67]
+	_ = x[actTogglePreviewWrap-68]
+	_ = x[actTransform-69]
+	_ = x[actTransformBorderLabel-70]
+	_ = x[actTransformHeader-71]
+	_ = x[actTransformPreviewLabel-72]
+	_ = x[actTransformPrompt-73]
+	_ = x[actTransformQuery-74]
+	_ = x[actPreview-75]
+	_ = x[actChangePreview-76]
+	_ = x[actChangePreviewWindow-77]
+	_ = x[actPreviewTop-78]
+	_ = x[actPreviewBottom-79]
+	_ = x[actPreviewUp-80]
+	_ = x[actPreviewDown-81]
+	_ = x[actPreviewPageUp-82]
+	_ = x[actPreviewPageDown-83]
+	_ = x[actPreviewHalfPageUp-84]
+	_ = x[actPreviewHalfPageDown-85]
+	_ = x[actPrevHistory-86]
+	_ = x[actPrevSelected-87]
+	_ = x[actPut-88]
+	_ = x[actNextHistory-89]
+	_ = x[actNextSelected-90]
+	_ = x[actExecute-91]
+	_ = x[actExecuteSilent-92]
+	_ = x[actExecuteMulti-93]
+	_ = x[actSigStop-94]
+	_ = x[actFirst-95]
+	_ = x[actLast-96]
+	_ = x[actReload-97]
+	_ = x[actReloadSync-98]
+	_ = x[actDisableSearch-99]
+	_ = x[actEnableSearch-100]
+	_ = x[actSelect-101]
+	_ = x[actDeselect-102]
+	_ = x[actUnbind-103]
+	_ = x[actRebind-104]
+	_ = x[actBecome-105]
+	_ = x[actResponse-106]
+	_ = x[actShowHeader-107]
+	_ = x[actHideHeader-108]
 }
 
-const _actionType_name = "actIgnoreactStartactClickactInvalidactCharactMouseactBeginningOfLineactAbortactAcceptactAcceptNonEmptyactAcceptOrPrintQueryactBackwardCharactBackwardDeleteCharactBackwardDeleteCharEofactBackwardWordactCancelactChangeBorderLabelactChangeHeaderactChangePreviewLabelactChangePromptactChangeQueryactClearScreenactClearQueryactClearSelectionactCloseactDeleteCharactDeleteCharEofactEndOfLineactForwardCharactForwardWordactKillLineactKillWordactUnixLineDiscardactUnixWordRuboutactYankactBackwardKillWordactSelectAllactDeselectAllactToggleactToggleSearchactToggleAllactToggleDownactToggleUpactToggleInactToggleOutactToggleTrackactToggleHeaderactTrackactDownactUpactPageUpactPageDownactPositionactHalfPageUpactHalfPageDownactOffsetUpactOffsetDownactJumpactJumpAcceptactPrintQueryactRefreshPreviewactReplaceQueryactToggleSortactShowPreviewactHidePreviewactTogglePreviewactTogglePreviewWrapactTransformactTransformBorderLabelactTransformHeaderactTransformPreviewLabelactTransformPromptactTransformQueryactPreviewactChangePreviewactChangePreviewWindowactPreviewTopactPreviewBottomactPreviewUpactPreviewDownactPreviewPageUpactPreviewPageDownactPreviewHalfPageUpactPreviewHalfPageDownactPrevHistoryactPrevSelectedactPutactNextHistoryactNextSelectedactExecuteactExecuteSilentactExecuteMultiactSigStopactFirstactLastactReloadactReloadSyncactDisableSearchactEnableSearchactSelectactDeselectactUnbindactRebindactBecomeactResponseactShowHeaderactHideHeader"
+const _actionType_name = "actIgnoreactStartactClickactInvalidactCharactMouseactBeginningOfLineactAbortactAcceptactAcceptNonEmptyactAcceptOrPrintQueryactBackwardCharactBackwardDeleteCharactBackwardDeleteCharEofactBackwardWordactCancelactChangeBorderLabelactChangeHeaderactChangePreviewLabelactChangePromptactChangeQueryactClearScreenactClearQueryactClearSelectionactCloseactDeleteCharactDeleteCharEofactEndOfLineactForwardCharactForwardWordactKillLineactKillWordactUnixLineDiscardactUnixWordRuboutactYankactBackwardKillWordactSelectAllactDeselectAllactToggleactToggleSearchactToggleAllactToggleDownactToggleUpactToggleInactToggleOutactToggleTrackactToggleTrackCurrentactToggleHeaderactTrackCurrentactUntrackCurrentactDownactUpactPageUpactPageDownactPositionactHalfPageUpactHalfPageDownactOffsetUpactOffsetDownactJumpactJumpAcceptactPrintQueryactRefreshPreviewactReplaceQueryactToggleSortactShowPreviewactHidePreviewactTogglePreviewactTogglePreviewWrapactTransformactTransformBorderLabelactTransformHeaderactTransformPreviewLabelactTransformPromptactTransformQueryactPreviewactChangePreviewactChangePreviewWindowactPreviewTopactPreviewBottomactPreviewUpactPreviewDownactPreviewPageUpactPreviewPageDownactPreviewHalfPageUpactPreviewHalfPageDownactPrevHistoryactPrevSelectedactPutactNextHistoryactNextSelectedactExecuteactExecuteSilentactExecuteMultiactSigStopactFirstactLastactReloadactReloadSyncactDisableSearchactEnableSearchactSelectactDeselectactUnbindactRebindactBecomeactResponseactShowHeaderactHideHeader"
 
-var _actionType_index = [...]uint16{0, 9, 17, 25, 35, 42, 50, 68, 76, 85, 102, 123, 138, 159, 183, 198, 207, 227, 242, 263, 278, 292, 306, 319, 336, 344, 357, 373, 385, 399, 413, 424, 435, 453, 470, 477, 496, 508, 522, 531, 546, 558, 571, 582, 593, 605, 619, 634, 642, 649, 654, 663, 674, 685, 698, 713, 724, 737, 744, 757, 770, 787, 802, 815, 829, 843, 859, 879, 891, 914, 932, 956, 974, 991, 1001, 1017, 1039, 1052, 1068, 1080, 1094, 1110, 1128, 1148, 1170, 1184, 1199, 1205, 1219, 1234, 1244, 1260, 1275, 1285, 1293, 1300, 1309, 1322, 1338, 1353, 1362, 1373, 1382, 1391, 1400, 1411, 1424, 1437}
+var _actionType_index = [...]uint16{0, 9, 17, 25, 35, 42, 50, 68, 76, 85, 102, 123, 138, 159, 183, 198, 207, 227, 242, 263, 278, 292, 306, 319, 336, 344, 357, 373, 385, 399, 413, 424, 435, 453, 470, 477, 496, 508, 522, 531, 546, 558, 571, 582, 593, 605, 619, 640, 655, 670, 687, 694, 699, 708, 719, 730, 743, 758, 769, 782, 789, 802, 815, 832, 847, 860, 874, 888, 904, 924, 936, 959, 977, 1001, 1019, 1036, 1046, 1062, 1084, 1097, 1113, 1125, 1139, 1155, 1173, 1193, 1215, 1229, 1244, 1250, 1264, 1279, 1289, 1305, 1320, 1330, 1338, 1345, 1354, 1367, 1383, 1398, 1407, 1418, 1427, 1436, 1445, 1456, 1469, 1482}
 
 func (i actionType) String() string {
 	if i < 0 || i >= actionType(len(_actionType_index)-1) {
 		return "actionType(" + strconv.FormatInt(int64(i), 10) + ")"
 	}
 	return _actionType_name[_actionType_index[i]:_actionType_index[i+1]]
 }
```

### Comparing `fzf_bin-0.48.1/fzf/src/algo/algo.go` & `fzf_bin-0.49.0/fzf/src/algo/algo.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/algo/algo_test.go` & `fzf_bin-0.49.0/fzf/src/algo/algo_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/algo/normalize.go` & `fzf_bin-0.49.0/fzf/src/algo/normalize.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/ansi.go` & `fzf_bin-0.49.0/fzf/src/ansi.go`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,15 @@
 		s = s[:i]
 	}
 
 	if len(s) > 0 {
 		// Inlined version of strconv.Atoi() that only handles positive
 		// integers and does not allocate on error.
 		code := 0
-		for _, ch := range []byte(s) {
+		for _, ch := range sbytes(s) {
 			ch -= '0'
 			if ch > 9 {
 				return -1, delimiter, remaining
 			}
 			code = code*10 + int(ch)
 		}
 		return code, delimiter, remaining
```

### Comparing `fzf_bin-0.48.1/fzf/src/ansi_test.go` & `fzf_bin-0.49.0/fzf/src/ansi_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/cache.go` & `fzf_bin-0.49.0/fzf/src/cache.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/cache_test.go` & `fzf_bin-0.49.0/fzf/src/cache_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/chunklist.go` & `fzf_bin-0.49.0/fzf/src/chunklist.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/chunklist_test.go` & `fzf_bin-0.49.0/fzf/src/chunklist_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/constants.go` & `fzf_bin-0.49.0/fzf/src/constants.go`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 const (
 	// Core
 	coordinatorDelayMax  time.Duration = 100 * time.Millisecond
 	coordinatorDelayStep time.Duration = 10 * time.Millisecond
 
 	// Reader
 	readerBufferSize       = 64 * 1024
+	readerSlabSize         = 128 * 1024
 	readerPollIntervalMin  = 10 * time.Millisecond
 	readerPollIntervalStep = 5 * time.Millisecond
 	readerPollIntervalMax  = 50 * time.Millisecond
 
 	// Terminal
 	initialDelay      = 20 * time.Millisecond
 	initialDelayTac   = 100 * time.Millisecond
```

### Comparing `fzf_bin-0.48.1/fzf/src/core.go` & `fzf_bin-0.49.0/fzf/src/core.go`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 // Package fzf implements fzf, a command-line fuzzy finder.
 package fzf
 
 import (
 	"fmt"
 	"os"
 	"time"
+	"unsafe"
 
 	"github.com/junegunn/fzf/src/util"
 )
 
 /*
 Reader   -> EvtReadFin
 Reader   -> EvtReadNew        -> Matcher  (restart)
 Terminal -> EvtSearchNew:bool -> Matcher  (restart)
 Matcher  -> EvtSearchProgress -> Terminal (update info)
 Matcher  -> EvtSearchFin      -> Terminal (update list)
 Matcher  -> EvtHeader         -> Terminal (update header)
 */
 
+func ustring(data []byte) string {
+	return unsafe.String(unsafe.SliceData(data), len(data))
+}
+
+func sbytes(data string) []byte {
+	return unsafe.Slice(unsafe.StringData(data), len(data))
+}
+
 // Run starts fzf
 func Run(opts *Options, version string, revision string) {
 	sort := opts.Sort > 0
 	sortCriteria = opts.Criteria
 
 	if opts.Version {
 		if len(revision) > 0 {
@@ -41,47 +50,47 @@
 	}
 
 	var lineAnsiState, prevLineAnsiState *ansiState
 	if opts.Ansi {
 		if opts.Theme.Colored {
 			ansiProcessor = func(data []byte) (util.Chars, *[]ansiOffset) {
 				prevLineAnsiState = lineAnsiState
-				trimmed, offsets, newState := extractColor(string(data), lineAnsiState, nil)
+				trimmed, offsets, newState := extractColor(ustring(data), lineAnsiState, nil)
 				lineAnsiState = newState
-				return util.ToChars([]byte(trimmed)), offsets
+				return util.ToChars(sbytes(trimmed)), offsets
 			}
 		} else {
 			// When color is disabled but ansi option is given,
 			// we simply strip out ANSI codes from the input
 			ansiProcessor = func(data []byte) (util.Chars, *[]ansiOffset) {
-				trimmed, _, _ := extractColor(string(data), nil, nil)
-				return util.ToChars([]byte(trimmed)), nil
+				trimmed, _, _ := extractColor(ustring(data), nil, nil)
+				return util.ToChars(sbytes(trimmed)), nil
 			}
 		}
 	}
 
 	// Chunk list
 	var chunkList *ChunkList
 	var itemIndex int32
 	header := make([]string, 0, opts.HeaderLines)
 	if len(opts.WithNth) == 0 {
 		chunkList = NewChunkList(func(item *Item, data []byte) bool {
 			if len(header) < opts.HeaderLines {
-				header = append(header, string(data))
+				header = append(header, ustring(data))
 				eventBox.Set(EvtHeader, header)
 				return false
 			}
 			item.text, item.colors = ansiProcessor(data)
 			item.text.Index = itemIndex
 			itemIndex++
 			return true
 		})
 	} else {
 		chunkList = NewChunkList(func(item *Item, data []byte) bool {
-			tokens := Tokenize(string(data), opts.Delimiter)
+			tokens := Tokenize(ustring(data), opts.Delimiter)
 			if opts.Ansi && opts.Theme.Colored && len(tokens) > 1 {
 				var ansiState *ansiState
 				if prevLineAnsiState != nil {
 					ansiStateDup := *prevLineAnsiState
 					ansiState = &ansiStateDup
 				}
 				for _, token := range tokens {
@@ -97,15 +106,15 @@
 			trans := Transform(tokens, opts.WithNth)
 			transformed := joinTokens(trans)
 			if len(header) < opts.HeaderLines {
 				header = append(header, transformed)
 				eventBox.Set(EvtHeader, header)
 				return false
 			}
-			item.text, item.colors = ansiProcessor([]byte(transformed))
+			item.text, item.colors = ansiProcessor(sbytes(transformed))
 			item.text.TrimTrailingWhitespaces()
 			item.text.Index = itemIndex
 			item.origText = &data
 			itemIndex++
 			return true
 		})
 	}
@@ -241,19 +250,16 @@
 		header = make([]string, 0, opts.HeaderLines)
 		go reader.restart(command, environ)
 	}
 	for {
 		delay := true
 		ticks++
 		input := func() []rune {
-			reloaded := snapshotRevision != inputRevision
 			paused, input := terminal.Input()
-			if reloaded && paused {
-				query = []rune{}
-			} else if !paused {
+			if !paused {
 				query = input
 			}
 			return query
 		}
 		eventBox.Wait(func(events *util.Events) {
 			if _, fin := (*events)[EvtReadFin]; fin {
 				delete(*events, EvtReadNew)
@@ -274,14 +280,17 @@
 					} else {
 						reading = reading && evt == EvtReadNew
 					}
 					if useSnapshot && evt == EvtReadFin {
 						useSnapshot = false
 					}
 					if !useSnapshot {
+						if snapshotRevision != inputRevision {
+							query = []rune{}
+						}
 						snapshot, count = chunkList.Snapshot()
 						snapshotRevision = inputRevision
 					}
 					total = count
 					terminal.UpdateCount(total, !reading, value.(*string))
 					if opts.Sync {
 						opts.Sync = false
@@ -315,18 +324,21 @@
 							restart(*command, environ)
 						}
 					}
 					if !changed {
 						break
 					}
 					if !useSnapshot {
-						newSnapshot, _ := chunkList.Snapshot()
+						newSnapshot, newCount := chunkList.Snapshot()
 						// We want to avoid showing empty list when reload is triggered
 						// and the query string is changed at the same time i.e. command != nil && changed
-						if command == nil || len(newSnapshot) > 0 {
+						if command == nil || newCount > 0 {
+							if snapshotRevision != inputRevision {
+								query = []rune{}
+							}
 							snapshot = newSnapshot
 							snapshotRevision = inputRevision
 						}
 					}
 					matcher.Reset(snapshot, input(), true, !reading, sort, snapshotRevision)
 					delay = false
```

### Comparing `fzf_bin-0.48.1/fzf/src/history.go` & `fzf_bin-0.49.0/fzf/src/history.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/history_test.go` & `fzf_bin-0.49.0/fzf/src/history_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/item.go` & `fzf_bin-0.49.0/fzf/src/item.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/matcher.go` & `fzf_bin-0.49.0/fzf/src/matcher.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/merger.go` & `fzf_bin-0.49.0/fzf/src/merger.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/merger_test.go` & `fzf_bin-0.49.0/fzf/src/merger_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/options.go` & `fzf_bin-0.49.0/fzf/src/options.go`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     --border-label-pos=COL Position of the border label
                            [POSITIVE_INTEGER: columns from left|
                             NEGATIVE_INTEGER: columns from right][:bottom]
                            (default: 0 or center)
     --margin=MARGIN        Screen margin (TRBL | TB,RL | T,RL,B | T,R,B,L)
     --padding=PADDING      Padding inside border (TRBL | TB,RL | T,RL,B | T,R,B,L)
     --info=STYLE           Finder info style
-                           [default|right|hidden|inline[:SEPARATOR]|inline-right]
+                           [default|right|hidden|inline[-right][:PREFIX]]
     --separator=STR        String to form horizontal separator on info line
     --no-separator         Hide info line separator
     --scrollbar[=C1[C2]]   Scrollbar character(s) (each for main and preview window)
     --no-scrollbar         Hide scrollbar
     --prompt=STR           Input prompt (default: '> ')
     --pointer=STR          Pointer to the current line (default: '>')
     --marker=STR           Multi-select marker (default: '>')
@@ -139,15 +139,15 @@
     FZF_DEFAULT_COMMAND    Default command to use when input is tty
     FZF_DEFAULT_OPTS       Default options (e.g. '--layout=reverse --info=inline')
     FZF_DEFAULT_OPTS_FILE  Location of the file to read default options from
     FZF_API_KEY            X-API-Key header for HTTP server (--listen)
 
 `
 
-const defaultInfoSep = " < "
+const defaultInfoPrefix = " < "
 
 // Case denotes case-sensitivity of search
 type Case int
 
 // Case-sensitivities
 const (
 	CaseSmart Case = iota
@@ -213,18 +213,14 @@
 	infoDefault infoStyle = iota
 	infoRight
 	infoInline
 	infoInlineRight
 	infoHidden
 )
 
-func (s infoStyle) noExtraLine() bool {
-	return s == infoInline || s == infoInlineRight || s == infoHidden
-}
-
 type labelOpts struct {
 	label  string
 	column int
 	bottom bool
 }
 
 type previewOpts struct {
@@ -323,15 +319,15 @@
 	Cycle        bool
 	KeepRight    bool
 	Hscroll      bool
 	HscrollOff   int
 	ScrollOff    int
 	FileWord     bool
 	InfoStyle    infoStyle
-	InfoSep      string
+	InfoPrefix   string
 	Separator    *string
 	JumpLabels   string
 	Prompt       string
 	Pointer      string
 	Marker       string
 	Query        string
 	Select1      bool
@@ -1207,22 +1203,26 @@
 			appendAction(actToggleOut)
 		case "toggle-all":
 			appendAction(actToggleAll)
 		case "toggle-search":
 			appendAction(actToggleSearch)
 		case "toggle-track":
 			appendAction(actToggleTrack)
+		case "toggle-track-current":
+			appendAction(actToggleTrackCurrent)
 		case "toggle-header":
 			appendAction(actToggleHeader)
 		case "show-header":
 			appendAction(actShowHeader)
 		case "hide-header":
 			appendAction(actHideHeader)
-		case "track":
-			appendAction(actTrack)
+		case "track", "track-current":
+			appendAction(actTrackCurrent)
+		case "untrack-current":
+			appendAction(actUntrackCurrent)
 		case "select":
 			appendAction(actSelect)
 		case "select-all":
 			appendAction(actSelectAll)
 		case "deselect-all":
 			appendAction(actDeselectAll)
 		case "close":
@@ -1498,25 +1498,32 @@
 func parseInfoStyle(str string) (infoStyle, string) {
 	switch str {
 	case "default":
 		return infoDefault, ""
 	case "right":
 		return infoRight, ""
 	case "inline":
-		return infoInline, defaultInfoSep
+		return infoInline, defaultInfoPrefix
 	case "inline-right":
 		return infoInlineRight, ""
 	case "hidden":
 		return infoHidden, ""
 	default:
-		prefix := "inline:"
-		if strings.HasPrefix(str, prefix) {
-			return infoInline, strings.ReplaceAll(str[len(prefix):], "\n", " ")
+		type infoSpec struct {
+			name  string
+			style infoStyle
+		}
+		for _, spec := range []infoSpec{
+			{"inline", infoInline},
+			{"inline-right", infoInlineRight}} {
+			if strings.HasPrefix(str, spec.name+":") {
+				return spec.style, strings.ReplaceAll(str[len(spec.name)+1:], "\n", " ")
+			}
 		}
-		errorExit("invalid info style (expected: default|right|hidden|inline[:SEPARATOR]|inline-right)")
+		errorExit("invalid info style (expected: default|right|hidden|inline[-right][:PREFIX])")
 	}
 	return infoDefault, ""
 }
 
 func parsePreviewWindow(opts *previewOpts, input string) {
 	parsePreviewWindowImpl(opts, input, errorExit)
 }
@@ -1799,21 +1806,21 @@
 		case "--scroll-off":
 			opts.ScrollOff = nextInt(allArgs, &i, "scroll offset required")
 		case "--filepath-word":
 			opts.FileWord = true
 		case "--no-filepath-word":
 			opts.FileWord = false
 		case "--info":
-			opts.InfoStyle, opts.InfoSep = parseInfoStyle(
+			opts.InfoStyle, opts.InfoPrefix = parseInfoStyle(
 				nextString(allArgs, &i, "info style required"))
 		case "--no-info":
 			opts.InfoStyle = infoHidden
 		case "--inline-info":
 			opts.InfoStyle = infoInline
-			opts.InfoSep = defaultInfoSep
+			opts.InfoPrefix = defaultInfoPrefix
 		case "--no-inline-info":
 			opts.InfoStyle = infoDefault
 		case "--separator":
 			separator := nextString(allArgs, &i, "separator character required")
 			opts.Separator = &separator
 		case "--no-separator":
 			nosep := ""
@@ -2007,15 +2014,15 @@
 			} else if match, value := optString(arg, "--height="); match {
 				opts.Height = parseHeight(value)
 			} else if match, value := optString(arg, "--min-height="); match {
 				opts.MinHeight = atoi(value)
 			} else if match, value := optString(arg, "--layout="); match {
 				opts.Layout = parseLayout(value)
 			} else if match, value := optString(arg, "--info="); match {
-				opts.InfoStyle, opts.InfoSep = parseInfoStyle(value)
+				opts.InfoStyle, opts.InfoPrefix = parseInfoStyle(value)
 			} else if match, value := optString(arg, "--separator="); match {
 				opts.Separator = &value
 			} else if match, value := optString(arg, "--scrollbar="); match {
 				opts.Scrollbar = &value
 			} else if match, value := optString(arg, "--toggle-sort="); match {
 				parseToggleSort(opts.Keymap, value)
 			} else if match, value := optString(arg, "--expect="); match {
```

### Comparing `fzf_bin-0.48.1/fzf/src/options_test.go` & `fzf_bin-0.49.0/fzf/src/options_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/pattern.go` & `fzf_bin-0.49.0/fzf/src/pattern.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/pattern_test.go` & `fzf_bin-0.49.0/fzf/src/pattern_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/reader.go` & `fzf_bin-0.49.0/fzf/src/reader.go`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 package fzf
 
 import (
-	"bufio"
+	"bytes"
 	"context"
 	"io"
 	"os"
 	"os/exec"
 	"path/filepath"
 	"sync"
 	"sync/atomic"
@@ -107,40 +107,92 @@
 	} else {
 		success = r.readFromStdin()
 	}
 	r.fin(success)
 }
 
 func (r *Reader) feed(src io.Reader) {
+	/*
+		readerSlabSize, ae := strconv.Atoi(os.Getenv("SLAB_KB"))
+		if ae != nil {
+			readerSlabSize = 128 * 1024
+		} else {
+			readerSlabSize *= 1024
+		}
+		readerBufferSize, be := strconv.Atoi(os.Getenv("BUF_KB"))
+		if be != nil {
+			readerBufferSize = 64 * 1024
+		} else {
+			readerBufferSize *= 1024
+		}
+	*/
+
 	delim := byte('\n')
+	trimCR := util.IsWindows()
 	if r.delimNil {
 		delim = '\000'
+		trimCR = false
 	}
-	reader := bufio.NewReaderSize(src, readerBufferSize)
+
+	slab := make([]byte, readerSlabSize)
+	leftover := []byte{}
+	var err error
 	for {
-		// ReadBytes returns err != nil if and only if the returned data does not
-		// end in delim.
-		bytea, err := reader.ReadBytes(delim)
-		byteaLen := len(bytea)
-		if byteaLen > 0 {
-			if err == nil {
-				// get rid of carriage return if under Windows:
-				if util.IsWindows() && byteaLen >= 2 && bytea[byteaLen-2] == byte('\r') {
-					bytea = bytea[:byteaLen-2]
+		n := 0
+		scope := slab[:util.Min(len(slab), readerBufferSize)]
+		for i := 0; i < 100; i++ {
+			n, err = src.Read(scope)
+			if n > 0 || err != nil {
+				break
+			}
+		}
+
+		// We're not making any progress after 100 tries. Stop.
+		if n == 0 && err == nil {
+			break
+		}
+
+		buf := slab[:n]
+		slab = slab[n:]
+
+		for len(buf) > 0 {
+			if i := bytes.IndexByte(buf, delim); i >= 0 {
+				// Found the delimiter
+				slice := buf[:i+1]
+				buf = buf[i+1:]
+				if trimCR && len(slice) >= 2 && slice[len(slice)-2] == byte('\r') {
+					slice = slice[:len(slice)-2]
 				} else {
-					bytea = bytea[:byteaLen-1]
+					slice = slice[:len(slice)-1]
 				}
-			}
-			if r.pusher(bytea) {
-				atomic.StoreInt32(&r.event, int32(EvtReadNew))
+				if len(leftover) > 0 {
+					slice = append(leftover, slice...)
+					leftover = []byte{}
+				}
+				if (err == nil || len(slice) > 0) && r.pusher(slice) {
+					atomic.StoreInt32(&r.event, int32(EvtReadNew))
+				}
+			} else {
+				// Could not find the delimiter in the buffer
+				leftover = append(leftover, buf...)
+				break
 			}
 		}
-		if err != nil {
+
+		if err == io.EOF {
+			leftover = append(leftover, buf...)
 			break
 		}
+
+		if len(slab) == 0 {
+			slab = make([]byte, readerSlabSize)
+		}
+	}
+	if len(leftover) > 0 && r.pusher(leftover) {
+		atomic.StoreInt32(&r.event, int32(EvtReadNew))
 	}
 }
 
 func (r *Reader) readFromStdin() bool {
 	r.feed(os.Stdin)
 	return true
 }
```

### Comparing `fzf_bin-0.48.1/fzf/src/reader_test.go` & `fzf_bin-0.49.0/fzf/src/reader_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/result.go` & `fzf_bin-0.49.0/fzf/src/result.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/result_test.go` & `fzf_bin-0.49.0/fzf/src/result_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/server.go` & `fzf_bin-0.49.0/fzf/src/server.go`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 const (
 	crlf             = "\r\n"
 	httpOk           = "HTTP/1.1 200 OK" + crlf
 	httpBadRequest   = "HTTP/1.1 400 Bad Request" + crlf
 	httpUnauthorized = "HTTP/1.1 401 Unauthorized" + crlf
 	httpUnavailable  = "HTTP/1.1 503 Service Unavailable" + crlf
 	httpReadTimeout  = 10 * time.Second
+	channelTimeout   = 2 * time.Second
 	jsonContentType  = "Content-Type: application/json" + crlf
 	maxContentLength = 1024 * 1024
 )
 
 type httpServer struct {
 	apiKey          []byte
 	actionChannel   chan []*action
@@ -166,15 +167,15 @@
 		case 0:
 			getMatch := getRegex.FindStringSubmatch(text)
 			if len(getMatch) > 0 {
 				server.actionChannel <- []*action{{t: actResponse, a: getMatch[1]}}
 				select {
 				case response := <-server.responseChannel:
 					return good(response)
-				case <-time.After(2 * time.Second):
+				case <-time.After(channelTimeout):
 					go func() {
 						// Drain the channel
 						<-server.responseChannel
 					}()
 					return answer(httpUnavailable+jsonContentType, `{"error":"timeout"}`)
 				}
 			} else if !strings.HasPrefix(text, "POST / HTTP") {
@@ -223,15 +224,19 @@
 	if len(errorMessage) > 0 {
 		return bad(errorMessage)
 	}
 	if len(actions) == 0 {
 		return bad("no action specified")
 	}
 
-	server.actionChannel <- actions
+	select {
+	case server.actionChannel <- actions:
+	case <-time.After(channelTimeout):
+		return httpUnavailable + crlf
+	}
 	return httpOk + crlf
 }
 
 func parseGetParams(query string) getParams {
 	params := getParams{limit: 100, offset: 0}
 	for _, pair := range strings.Split(query, "&") {
 		parts := strings.SplitN(pair, "=", 2)
```

### Comparing `fzf_bin-0.48.1/fzf/src/terminal.go` & `fzf_bin-0.49.0/fzf/src/terminal.go`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 	Selected   []StatusItem `json:"selected"`
 }
 
 // Terminal represents terminal input/output
 type Terminal struct {
 	initDelay          time.Duration
 	infoStyle          infoStyle
-	infoSep            string
+	infoPrefix         string
 	separator          labelPrinter
 	separatorLen       int
 	spinner            []string
 	promptString       string
 	prompt             func()
 	promptLen          int
 	borderLabel        labelPrinter
@@ -390,16 +390,18 @@
 	actToggleSearch
 	actToggleAll
 	actToggleDown
 	actToggleUp
 	actToggleIn
 	actToggleOut
 	actToggleTrack
+	actToggleTrackCurrent
 	actToggleHeader
-	actTrack
+	actTrackCurrent
+	actUntrackCurrent
 	actDown
 	actUp
 	actPageUp
 	actPageDown
 	actPosition
 	actHalfPageUp
 	actHalfPageDown
@@ -671,15 +673,15 @@
 	} else {
 		maxHeightFunc := func(termHeight int) int {
 			// Minimum height required to render fzf excluding margin and padding
 			effectiveMinHeight := minHeight
 			if previewBox != nil && opts.Preview.aboveOrBelow() {
 				effectiveMinHeight += 1 + borderLines(opts.Preview.border)
 			}
-			if opts.InfoStyle.noExtraLine() {
+			if noSeparatorLine(opts.InfoStyle, opts.Separator == nil || uniseg.StringWidth(*opts.Separator) > 0) {
 				effectiveMinHeight--
 			}
 			effectiveMinHeight += borderLines(opts.BorderShape)
 			return util.Min(termHeight, util.Max(evaluateHeight(opts, termHeight), effectiveMinHeight))
 		}
 		renderer = tui.NewLightRenderer(opts.Theme, opts.Black, opts.Mouse, opts.Tabstop, opts.ClearOnExit, false, maxHeightFunc)
 	}
@@ -693,15 +695,15 @@
 	keymapCopy := make(map[tui.Event][]*action)
 	for key, action := range opts.Keymap {
 		keymapCopy[key] = action
 	}
 	t := Terminal{
 		initDelay:          delay,
 		infoStyle:          opts.InfoStyle,
-		infoSep:            opts.InfoSep,
+		infoPrefix:         opts.InfoPrefix,
 		separator:          nil,
 		spinner:            makeSpinner(opts.Unicode),
 		promptString:       opts.Prompt,
 		queryLen:           [2]int{0, 0},
 		layout:             opts.Layout,
 		fullscreen:         fullscreen,
 		keepRight:          opts.KeepRight,
@@ -772,15 +774,15 @@
 		mutex:              sync.Mutex{},
 		suppress:           true,
 		sigstop:            false,
 		slab:               util.MakeSlab(slab16Size, slab32Size),
 		theme:              opts.Theme,
 		startChan:          make(chan fitpad, 1),
 		killChan:           make(chan int),
-		serverInputChan:    make(chan []*action, 10),
+		serverInputChan:    make(chan []*action, 100),
 		serverOutputChan:   make(chan string),
 		eventChan:          make(chan tui.Event, 6), // (load + result + zero|one) | (focus) | (resize) | (GetChar)
 		tui:                renderer,
 		initFunc:           func() { renderer.Init() },
 		executing:          util.NewAtomicBool(false),
 		lastAction:         actStart,
 		lastFocus:          minItem.Index()}
@@ -846,14 +848,16 @@
 	env := os.Environ()
 	if t.listenPort != nil {
 		env = append(env, fmt.Sprintf("FZF_PORT=%d", *t.listenPort))
 	}
 	env = append(env, "FZF_QUERY="+string(t.input))
 	env = append(env, "FZF_ACTION="+t.lastAction.Name())
 	env = append(env, "FZF_PROMPT="+string(t.promptString))
+	env = append(env, "FZF_PREVIEW_LABEL="+t.previewLabelOpts.label)
+	env = append(env, "FZF_BORDER_LABEL="+t.borderLabelOpts.label)
 	env = append(env, fmt.Sprintf("FZF_TOTAL_COUNT=%d", t.count))
 	env = append(env, fmt.Sprintf("FZF_MATCH_COUNT=%d", t.merger.Length()))
 	env = append(env, fmt.Sprintf("FZF_SELECT_COUNT=%d", len(t.selected)))
 	env = append(env, fmt.Sprintf("FZF_LINES=%d", t.areaLines))
 	env = append(env, fmt.Sprintf("FZF_COLUMNS=%d", t.areaColumns))
 	return env
 }
@@ -874,15 +878,15 @@
 	}
 	return len(t.header0) + t.headerLines
 }
 
 // Extra number of lines needed to display fzf
 func (t *Terminal) extraLines() int {
 	extra := t.visibleHeaderLines() + 1
-	if !t.noInfoLine() {
+	if !t.noSeparatorLine() {
 		extra++
 	}
 	return extra
 }
 
 func (t *Terminal) MaxFitAndPad() (int, int) {
 	_, screenHeight, marginInt, paddingInt := t.adjustMarginAndPadding()
@@ -980,16 +984,26 @@
 			Result{item: item}, tui.ColPrompt, tui.ColPrompt, false, false)
 	}
 	_, promptLen := t.processTabs([]rune(trimmed), 0)
 
 	return output, promptLen
 }
 
-func (t *Terminal) noInfoLine() bool {
-	return t.infoStyle.noExtraLine()
+func noSeparatorLine(style infoStyle, separator bool) bool {
+	switch style {
+	case infoInline:
+		return true
+	case infoHidden, infoInlineRight:
+		return !separator
+	}
+	return false
+}
+
+func (t *Terminal) noSeparatorLine() bool {
+	return noSeparatorLine(t.infoStyle, t.separatorLen > 0)
 }
 
 func getScrollbar(total int, height int, offset int) (int, int) {
 	if total == 0 || total <= height {
 		return 0, 0
 	}
 	barLength := util.Max(1, height*height/total)
@@ -1233,15 +1247,15 @@
 			marginInt[idx1] = util.Max(extraMargin[idx1], desired*marginInt[idx1]/margin)
 			marginInt[idx2] = util.Max(extraMargin[idx2], desired*marginInt[idx2]/margin)
 		}
 	}
 
 	minAreaWidth := minWidth
 	minAreaHeight := minHeight
-	if t.noInfoLine() {
+	if t.noSeparatorLine() {
 		minAreaHeight -= 1
 	}
 	if t.needPreviewWindow() {
 		minPreviewHeight := 1 + borderLines(t.previewOpts.border)
 		minPreviewWidth := 5
 		switch t.previewOpts.position {
 		case posUp, posDown:
@@ -1514,15 +1528,15 @@
 	h := t.window.Height()
 
 	switch t.layout {
 	case layoutDefault:
 		y = h - y - 1
 	case layoutReverseList:
 		n := 2 + t.visibleHeaderLines()
-		if t.noInfoLine() {
+		if t.noSeparatorLine() {
 			n--
 		}
 		if y < n {
 			y = h - y - 1
 		} else {
 			y -= n
 		}
@@ -1554,15 +1568,15 @@
 	t.queryLen = [2]int{beforeLen, afterLen}
 	return before, after
 }
 
 func (t *Terminal) promptLine() int {
 	if t.headerFirst {
 		max := t.window.Height() - 1
-		if !t.noInfoLine() {
+		if !t.noSeparatorLine() {
 			max--
 		}
 		return util.Min(t.visibleHeaderLines(), max)
 	}
 	return 0
 }
 
@@ -1599,58 +1613,76 @@
 			duration := int64(spinnerDuration)
 			idx := (time.Now().UnixNano() % (duration * int64(len(t.spinner)))) / duration
 			t.window.CPrint(tui.ColSpinner, t.spinner[idx])
 		} else {
 			t.window.Print(" ") // Clear spinner
 		}
 	}
-	switch t.infoStyle {
-	case infoDefault:
-		t.move(line+1, 0, t.separatorLen == 0)
-		printSpinner()
-		t.move(line+1, 2, false)
-		pos = 2
-	case infoRight:
-		t.move(line+1, 0, false)
-	case infoInlineRight:
-		pos = t.promptLen + t.queryLen[0] + t.queryLen[1] + 1
-		t.move(line, pos, true)
-	case infoInline:
-		pos = t.promptLen + t.queryLen[0] + t.queryLen[1] + 1
-		str := t.infoSep
+	printInfoPrefix := func() {
+		str := t.infoPrefix
 		maxWidth := t.window.Width() - pos
 		width := util.StringWidth(str)
 		if width > maxWidth {
 			trimmed, _ := t.trimRight([]rune(str), maxWidth)
 			str = string(trimmed)
 			width = maxWidth
 		}
 		t.move(line, pos, t.separatorLen == 0)
 		if t.reading {
 			t.window.CPrint(tui.ColSpinner, str)
 		} else {
 			t.window.CPrint(tui.ColPrompt, str)
 		}
 		pos += width
+	}
+	printSeparator := func(fillLength int, pad bool) {
+		// --------_
+		if t.separatorLen > 0 {
+			t.separator(t.window, fillLength)
+			t.window.Print(" ")
+		} else if pad {
+			t.window.Print(strings.Repeat(" ", fillLength+1))
+		}
+	}
+	switch t.infoStyle {
+	case infoDefault:
+		t.move(line+1, 0, t.separatorLen == 0)
+		printSpinner()
+		t.move(line+1, 2, false)
+		pos = 2
+	case infoRight:
+		t.move(line+1, 0, false)
+	case infoInlineRight:
+		pos = t.promptLen + t.queryLen[0] + t.queryLen[1] + 1
+	case infoInline:
+		pos = t.promptLen + t.queryLen[0] + t.queryLen[1] + 1
+		printInfoPrefix()
 	case infoHidden:
+		if t.separatorLen > 0 {
+			t.move(line+1, 0, false)
+			printSeparator(t.window.Width()-1, false)
+		}
 		return
 	}
 
 	found := t.merger.Length()
 	total := util.Max(found, t.count)
 	output := fmt.Sprintf("%d/%d", found, total)
 	if t.toggleSort {
 		if t.sort {
 			output += " +S"
 		} else {
 			output += " -S"
 		}
 	}
-	if t.track != trackDisabled {
+	switch t.track {
+	case trackEnabled:
 		output += " +T"
+	case trackCurrent:
+		output += " +t"
 	}
 	if t.multi > 0 {
 		if t.multi == maxMulti {
 			output += fmt.Sprintf(" (%d)", len(t.selected))
 		} else {
 			output += fmt.Sprintf(" (%d/%d)", len(t.selected), t.multi)
 		}
@@ -1658,23 +1690,14 @@
 	if t.progress > 0 && t.progress < 100 {
 		output += fmt.Sprintf(" (%d%%)", t.progress)
 	}
 	if t.failed != nil && t.count == 0 {
 		output = fmt.Sprintf("[Command failed: %s]", *t.failed)
 	}
 
-	printSeparator := func(fillLength int, pad bool) {
-		// --------_
-		if t.separatorLen > 0 {
-			t.separator(t.window, fillLength)
-			t.window.Print(" ")
-		} else if pad {
-			t.window.Print(strings.Repeat(" ", fillLength+1))
-		}
-	}
 	if t.infoStyle == infoRight {
 		maxWidth := t.window.Width()
 		if t.reading {
 			// Need space for spinner and a margin column
 			maxWidth -= 2
 		}
 		output = t.trimMessage(output, maxWidth)
@@ -1689,42 +1712,58 @@
 			printSeparator(fillLength, true)
 		}
 		t.window.CPrint(tui.ColInfo, output)
 		return
 	}
 
 	if t.infoStyle == infoInlineRight {
-		pos = util.Max(pos, t.window.Width()-util.StringWidth(output)-3)
-		if pos >= t.window.Width() {
-			return
+		if len(t.infoPrefix) == 0 {
+			pos = util.Max(pos, t.window.Width()-util.StringWidth(output)-3)
+			if pos < t.window.Width() {
+				t.move(line, pos, false)
+				printSpinner()
+				pos++
+			}
+			if pos < t.window.Width()-1 {
+				t.window.Print(" ")
+				pos++
+			}
+		} else {
+			pos = util.Max(pos, t.window.Width()-util.StringWidth(output)-util.StringWidth(t.infoPrefix)-1)
+			printInfoPrefix()
 		}
-		t.move(line, pos, false)
-		printSpinner()
-		t.window.Print(" ")
-		pos += 2
 	}
 
 	maxWidth := t.window.Width() - pos
 	output = t.trimMessage(output, maxWidth)
 	t.window.CPrint(tui.ColInfo, output)
+
+	if t.infoStyle == infoInlineRight {
+		if t.separatorLen > 0 {
+			t.move(line+1, 0, false)
+			printSeparator(t.window.Width()-1, false)
+		}
+		return
+	}
+
 	fillLength := maxWidth - len(output) - 2
 	if fillLength > 0 {
 		t.window.CPrint(tui.ColSeparator, " ")
 		printSeparator(fillLength, false)
 	}
 }
 
 func (t *Terminal) printHeader() {
 	if t.visibleHeaderLines() == 0 {
 		return
 	}
 	max := t.window.Height()
 	if t.headerFirst {
 		max--
-		if !t.noInfoLine() {
+		if !t.noSeparatorLine() {
 			max--
 		}
 	}
 	var state *ansiState
 	needReverse := false
 	switch t.layout {
 	case layoutDefault, layoutReverseList:
@@ -1733,15 +1772,15 @@
 	for idx, lineStr := range append(append([]string{}, t.header0...), t.header...) {
 		line := idx
 		if needReverse && idx < len(t.header0) {
 			line = len(t.header0) - idx - 1
 		}
 		if !t.headerFirst {
 			line++
-			if !t.noInfoLine() {
+			if !t.noSeparatorLine() {
 				line++
 			}
 		}
 		if line >= max {
 			continue
 		}
 		trimmed, colors, newState := extractColor(lineStr, state, nil)
@@ -1765,15 +1804,15 @@
 	count := t.merger.Length() - t.offset
 	for j := 0; j < maxy; j++ {
 		i := j
 		if t.layout == layoutDefault {
 			i = maxy - 1 - j
 		}
 		line := i + 2 + t.visibleHeaderLines()
-		if t.noInfoLine() {
+		if t.noSeparatorLine() {
 			line--
 		}
 		if i < count {
 			t.printItem(t.merger.Get(i+t.offset), line, i, i == t.cy-t.offset, i >= barStart && i < barStart+barLength)
 		} else if t.prevLines[i] != emptyLine || t.prevLines[i].offset != line {
 			t.prevLines[i] = emptyLine
 			t.move(line, 0, true)
@@ -3091,15 +3130,15 @@
 			t.reqBox.Wait(func(events *util.Events) {
 				defer events.Clear()
 				t.mutex.Lock()
 				for req, value := range *events {
 					switch req {
 					case reqPrompt:
 						t.printPrompt()
-						if t.noInfoLine() {
+						if t.infoStyle == infoInline || t.infoStyle == infoInlineRight {
 							t.printInfo()
 						}
 					case reqInfo:
 						t.printInfo()
 					case reqList:
 						t.printList()
 						currentIndex := t.currentIndex()
@@ -3467,36 +3506,40 @@
 			case actChangeHeader:
 				if t.changeHeader(a.a) {
 					req(reqFullRedraw)
 				} else {
 					req(reqHeader)
 				}
 			case actChangeBorderLabel:
+				t.borderLabelOpts.label = a.a
 				if t.border != nil {
 					t.borderLabel, t.borderLabelLen = t.ansiLabelPrinter(a.a, &tui.ColBorderLabel, false)
 					req(reqRedrawBorderLabel)
 				}
 			case actChangePreviewLabel:
+				t.previewLabelOpts.label = a.a
 				if t.pborder != nil {
 					t.previewLabel, t.previewLabelLen = t.ansiLabelPrinter(a.a, &tui.ColPreviewLabel, false)
 					req(reqRedrawPreviewLabel)
 				}
 			case actTransform:
 				body := t.executeCommand(a.a, false, true, true, false)
 				actions := parseSingleActionList(strings.Trim(body, "\r\n"), func(message string) {})
 				return doActions(actions)
 			case actTransformBorderLabel:
+				label := t.executeCommand(a.a, false, true, true, true)
+				t.borderLabelOpts.label = label
 				if t.border != nil {
-					label := t.executeCommand(a.a, false, true, true, true)
 					t.borderLabel, t.borderLabelLen = t.ansiLabelPrinter(label, &tui.ColBorderLabel, false)
 					req(reqRedrawBorderLabel)
 				}
 			case actTransformPreviewLabel:
+				label := t.executeCommand(a.a, false, true, true, true)
+				t.previewLabelOpts.label = label
 				if t.pborder != nil {
-					label := t.executeCommand(a.a, false, true, true, true)
 					t.previewLabel, t.previewLabelLen = t.ansiLabelPrinter(label, &tui.ColPreviewLabel, false)
 					req(reqRedrawPreviewLabel)
 				}
 			case actChangePrompt:
 				t.promptString = a.a
 				t.prompt, t.promptLen = t.parsePrompt(a.a)
 				req(reqPrompt)
@@ -3774,28 +3817,41 @@
 				switch t.track {
 				case trackEnabled:
 					t.track = trackDisabled
 				case trackDisabled:
 					t.track = trackEnabled
 				}
 				req(reqInfo)
+			case actToggleTrackCurrent:
+				switch t.track {
+				case trackCurrent:
+					t.track = trackDisabled
+				case trackDisabled:
+					t.track = trackCurrent
+				}
+				req(reqInfo)
 			case actShowHeader:
 				t.headerVisible = true
 				req(reqList, reqInfo, reqPrompt, reqHeader)
 			case actHideHeader:
 				t.headerVisible = false
 				req(reqList, reqInfo, reqPrompt, reqHeader)
 			case actToggleHeader:
 				t.headerVisible = !t.headerVisible
 				req(reqList, reqInfo, reqPrompt, reqHeader)
-			case actTrack:
+			case actTrackCurrent:
 				if t.track == trackDisabled {
 					t.track = trackCurrent
 				}
 				req(reqInfo)
+			case actUntrackCurrent:
+				if t.track == trackCurrent {
+					t.track = trackDisabled
+				}
+				req(reqInfo)
 			case actEnableSearch:
 				t.paused = false
 				changed = true
 				req(reqPrompt)
 			case actDisableSearch:
 				t.paused = true
 				req(reqPrompt)
@@ -3876,15 +3932,15 @@
 					break
 				}
 
 				// Translate coordinates
 				mx -= t.window.Left()
 				my -= t.window.Top()
 				min := 2 + t.visibleHeaderLines()
-				if t.noInfoLine() {
+				if t.noSeparatorLine() {
 					min--
 				}
 				h := t.window.Height()
 				switch t.layout {
 				case layoutDefault:
 					my = h - my - 1
 				case layoutReverseList:
@@ -4168,15 +4224,15 @@
 func (t *Terminal) vset(o int) bool {
 	t.cy = util.Constrain(o, 0, t.merger.Length()-1)
 	return t.cy == o
 }
 
 func (t *Terminal) maxItems() int {
 	max := t.window.Height() - 2 - t.visibleHeaderLines()
-	if t.noInfoLine() {
+	if t.noSeparatorLine() {
 		max++
 	}
 	return util.Max(max, 0)
 }
 
 func (t *Terminal) dumpItem(i *Item) StatusItem {
 	if i == nil {
```

### Comparing `fzf_bin-0.48.1/fzf/src/terminal_test.go` & `fzf_bin-0.49.0/fzf/src/terminal_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/terminal_unix.go` & `fzf_bin-0.49.0/fzf/src/terminal_unix.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/terminal_windows.go` & `fzf_bin-0.49.0/fzf/src/terminal_windows.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/tokenizer.go` & `fzf_bin-0.49.0/fzf/src/tokenizer.go`

 * *Files 5% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 }
 
 func withPrefixLengths(tokens []string, begin int) []Token {
 	ret := make([]Token, len(tokens))
 
 	prefixLength := begin
 	for idx := range tokens {
-		chars := util.ToChars([]byte(tokens[idx]))
+		chars := util.ToChars(sbytes(tokens[idx]))
 		ret[idx] = Token{&chars, int32(prefixLength)}
 		prefixLength += chars.Length()
 	}
 	return ret
 }
 
 const (
@@ -183,15 +183,15 @@
 	numTokens := len(tokens)
 	for idx, r := range withNth {
 		parts := []*util.Chars{}
 		minIdx := 0
 		if r.begin == r.end {
 			idx := r.begin
 			if idx == rangeEllipsis {
-				chars := util.ToChars([]byte(joinTokens(tokens)))
+				chars := util.ToChars(sbytes(joinTokens(tokens)))
 				parts = append(parts, &chars)
 			} else {
 				if idx < 0 {
 					idx += numTokens + 1
 				}
 				if idx >= 1 && idx <= numTokens {
 					minIdx = idx - 1
```

### Comparing `fzf_bin-0.48.1/fzf/src/tokenizer_test.go` & `fzf_bin-0.49.0/fzf/src/tokenizer_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/tui/dummy.go` & `fzf_bin-0.49.0/fzf/src/tui/dummy.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/tui/light.go` & `fzf_bin-0.49.0/fzf/src/tui/light.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/tui/light_unix.go` & `fzf_bin-0.49.0/fzf/src/tui/light_unix.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/tui/light_windows.go` & `fzf_bin-0.49.0/fzf/src/tui/light_windows.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/tui/tcell.go` & `fzf_bin-0.49.0/fzf/src/tui/tcell.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/tui/tcell_test.go` & `fzf_bin-0.49.0/fzf/src/tui/tcell_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/tui/ttyname_unix.go` & `fzf_bin-0.49.0/fzf/src/tui/ttyname_unix.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/tui/tui.go` & `fzf_bin-0.49.0/fzf/src/tui/tui.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/util/atomicbool.go` & `fzf_bin-0.49.0/fzf/src/util/atomicbool.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/util/chars.go` & `fzf_bin-0.49.0/fzf/src/util/chars.go`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 	chars.slice = chars.slice[0 : len(chars.slice)-whitespaces]
 }
 
 func (chars *Chars) ToString() string {
 	if runes := chars.optionalRunes(); runes != nil {
 		return string(runes)
 	}
-	return string(chars.slice)
+	return unsafe.String(unsafe.SliceData(chars.slice), len(chars.slice))
 }
 
 func (chars *Chars) ToRunes() []rune {
 	if runes := chars.optionalRunes(); runes != nil {
 		return runes
 	}
 	bytes := chars.slice
```

### Comparing `fzf_bin-0.48.1/fzf/src/util/chars_test.go` & `fzf_bin-0.49.0/fzf/src/util/chars_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/util/eventbox.go` & `fzf_bin-0.49.0/fzf/src/util/eventbox.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/util/eventbox_test.go` & `fzf_bin-0.49.0/fzf/src/util/eventbox_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/util/util.go` & `fzf_bin-0.49.0/fzf/src/util/util.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/util/util_test.go` & `fzf_bin-0.49.0/fzf/src/util/util_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/util/util_unix.go` & `fzf_bin-0.49.0/fzf/src/util/util_unix.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/src/util/util_windows.go` & `fzf_bin-0.49.0/fzf/src/util/util_windows.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/test/fzf.vader` & `fzf_bin-0.49.0/fzf/test/fzf.vader`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/fzf/test/test_go.rb` & `fzf_bin-0.49.0/fzf/test/test_go.rb`

 * *Files 0% similar despite different names*

```diff
@@ -1715,15 +1715,15 @@
       assert_path_exists tempname
       assert_equal %w[1], File.readlines(tempname, chomp: true)
     end
     tmux.until { |lines| assert_equal prompt, lines[-1] }
   end
 
   def test_info_hidden
-    tmux.send_keys 'seq 10 | fzf --info=hidden', :Enter
+    tmux.send_keys 'seq 10 | fzf --info=hidden --no-separator', :Enter
     tmux.until { |lines| assert_equal '> 1', lines[-2] }
   end
 
   def test_info_inline_separator
     tmux.send_keys 'seq 10 | fzf --info=inline:___ --no-separator', :Enter
     tmux.until { |lines| assert_equal '>  ___10/10', lines[-1] }
   end
@@ -2459,14 +2459,92 @@
     tmux.until { |lines| assert_equal 100, lines.item_count }
     tmux.send_keys '00'
     tmux.until { |lines| assert_equal 1, lines.match_count }
     # After 1 second
     tmux.until { |lines| assert_equal 10, lines.match_count }
   end
 
+  def test_reload_disabled_case1
+    tmux.send_keys "seq 100 | #{FZF} --query 99 --bind 'space:disable-search+reload(sleep 2; seq 1000)'", :Enter
+    tmux.until do |lines|
+      assert_equal 100, lines.item_count
+      assert_equal 1, lines.match_count
+    end
+    tmux.send_keys :Space
+    tmux.until { |lines| assert_equal 1, lines.match_count }
+    tmux.send_keys :BSpace
+    tmux.until { |lines| assert_equal 0, lines.match_count }
+    tmux.until { |lines| assert_equal 1000, lines.match_count }
+  end
+
+  def test_reload_disabled_case2
+    tmux.send_keys "seq 100 | #{FZF} --query 99 --bind 'space:disable-search+reload-sync(sleep 2; seq 1000)'", :Enter
+    tmux.until do |lines|
+      assert_equal 100, lines.item_count
+      assert_equal 1, lines.match_count
+    end
+    tmux.send_keys :Space
+    tmux.until { |lines| assert_equal 1, lines.match_count }
+    tmux.send_keys :BSpace
+    tmux.until { |lines| assert_equal 1, lines.match_count }
+    tmux.until { |lines| assert_equal 1000, lines.match_count }
+  end
+
+  def test_reload_disabled_case3
+    tmux.send_keys "seq 100 | #{FZF} --query 99 --bind 'space:disable-search+reload(sleep 2; seq 1000)+backward-delete-char'", :Enter
+    tmux.until do |lines|
+      assert_equal 100, lines.item_count
+      assert_equal 1, lines.match_count
+    end
+    tmux.send_keys :Space
+    tmux.until { |lines| assert_equal 1, lines.match_count }
+    tmux.send_keys :BSpace
+    tmux.until { |lines| assert_equal 0, lines.match_count }
+    tmux.until { |lines| assert_equal 1000, lines.match_count }
+  end
+
+  def test_reload_disabled_case4
+    tmux.send_keys "seq 100 | #{FZF} --query 99 --bind 'space:disable-search+reload-sync(sleep 2; seq 1000)+backward-delete-char'", :Enter
+    tmux.until do |lines|
+      assert_equal 100, lines.item_count
+      assert_equal 1, lines.match_count
+    end
+    tmux.send_keys :Space
+    tmux.until { |lines| assert_equal 1, lines.match_count }
+    tmux.send_keys :BSpace
+    tmux.until { |lines| assert_equal 1, lines.match_count }
+    tmux.until { |lines| assert_equal 1000, lines.match_count }
+  end
+
+  def test_reload_disabled_case5
+    tmux.send_keys "seq 100 | #{FZF} --query 99 --bind 'space:disable-search+reload(echo xx; sleep 2; seq 1000)'", :Enter
+    tmux.until do |lines|
+      assert_equal 100, lines.item_count
+      assert_equal 1, lines.match_count
+    end
+    tmux.send_keys :Space
+    tmux.until do |lines|
+      assert_equal 1, lines.item_count
+      assert_equal 1, lines.match_count
+    end
+    tmux.send_keys :BSpace
+    tmux.until { |lines| assert_equal 1001, lines.match_count }
+  end
+
+  def test_reload_disabled_case6
+    tmux.send_keys "seq 1000 | #{FZF} --disabled --bind 'change:reload:sleep 0.5; seq {q}'", :Enter
+    tmux.until { |lines| assert_equal 1000, lines.match_count }
+    tmux.send_keys '9'
+    tmux.until { |lines| assert_equal 9, lines.match_count }
+    tmux.send_keys '9'
+    tmux.until { |lines| assert_equal 99, lines.match_count }
+
+    # TODO: How do we verify if an intermediate empty list is not shown?
+  end
+
   def test_scroll_off
     tmux.send_keys "seq 1000 | #{FZF} --scroll-off=3 --bind l:last", :Enter
     tmux.until { |lines| assert_equal 1000, lines.item_count }
     height = tmux.until { |lines| lines }.first.to_i
     tmux.send_keys :PgUp
     tmux.until do |lines|
       assert_equal height + 3, lines.first.to_i
@@ -2795,14 +2873,35 @@
     tmux.send_keys ': | fzf --border rounded --preview-window border-rounded --border-label foobar --border-label-pos 2:bottom --preview : --preview-label barfoo --preview-label-pos -2:bottom', :Enter
     tmux.until do
       assert_includes(_1[-1], '╰foobar─')
       assert_includes(_1[-2], '─barfoo╯')
     end
   end
 
+  def test_labels_variables
+    tmux.send_keys ': | fzf --border --border-label foobar --preview "echo \$FZF_BORDER_LABEL // \$FZF_PREVIEW_LABEL" --preview-label barfoo --bind "space:change-border-label(barbaz)+change-preview-label(bazbar)+refresh-preview,enter:transform-border-label(echo 123)+transform-preview-label(echo 456)+refresh-preview"', :Enter
+    tmux.until do
+      assert_includes(_1[0], '─foobar─')
+      assert_includes(_1[1], '─barfoo─')
+      assert_includes(_1[2], ' foobar // barfoo ')
+    end
+    tmux.send_keys :Space
+    tmux.until do
+      assert_includes(_1[0], '─barbaz─')
+      assert_includes(_1[1], '─bazbar─')
+      assert_includes(_1[2], ' barbaz // bazbar ')
+    end
+    tmux.send_keys :Enter
+    tmux.until do
+      assert_includes(_1[0], '─123─')
+      assert_includes(_1[1], '─456─')
+      assert_includes(_1[2], ' 123 // 456 ')
+    end
+  end
+
   def test_info_separator_unicode
     tmux.send_keys 'seq 100 | fzf -q55', :Enter
     tmux.until { assert_includes(_1[-2], '  1/100 ─') }
   end
 
   def test_info_separator_no_unicode
     tmux.send_keys 'seq 100 | fzf -q55 --no-unicode', :Enter
@@ -2998,40 +3097,40 @@
     tmux.send_keys :BSpace
     tmux.until do |lines|
       assert_equal 28, lines.match_count
       assert_includes lines, '> 55'
     end
     tmux.send_keys :t
     tmux.until do |lines|
-      assert_includes lines[-2], '+T'
+      assert_includes lines[-2], '+t'
     end
     tmux.send_keys :BSpace
     tmux.until do |lines|
       assert_equal 271, lines.match_count
       assert_includes lines, '> 55'
     end
 
     # Automatically disabled when the tracking item is no longer visible
     tmux.send_keys '4'
     tmux.until do |lines|
       assert_equal 28, lines.match_count
-      refute_includes lines[-2], '+T'
+      refute_includes lines[-2], '+t'
     end
     tmux.send_keys :BSpace
     tmux.until do |lines|
       assert_equal 271, lines.match_count
       assert_includes lines, '> 5'
     end
     tmux.send_keys :t
     tmux.until do |lines|
-      assert_includes lines[-2], '+T'
+      assert_includes lines[-2], '+t'
     end
     tmux.send_keys :Up
     tmux.until do |lines|
-      refute_includes lines[-2], '+T'
+      refute_includes lines[-2], '+t'
     end
   end
 
   def test_one_and_zero
     tmux.send_keys "seq 10 | #{FZF} --bind 'zero:preview(echo no match),one:preview(echo {} is the only match)'", :Enter
     tmux.send_keys '1'
     tmux.until do |lines|
@@ -3303,15 +3402,18 @@
     tmux.until(true) { |lines| assert_equal 'cat no~such~user', lines[-1] }
 
     # /tmp/fzf\ test**<TAB>
     tmux.send_keys 'C-u'
     tmux.send_keys 'cat /tmp/fzf\ test/**', :Tab
     tmux.until { |lines| assert_operator lines.match_count, :>, 0 }
     tmux.send_keys 'foobar$'
-    tmux.until { |lines| assert_equal 1, lines.match_count }
+    tmux.until do |lines|
+      assert_equal 1, lines.match_count
+      assert lines.any_include?('> /tmp/fzf test/foobar')
+    end
     tmux.send_keys :Enter
     tmux.until(true) { |lines| assert_equal 'cat /tmp/fzf\ test/foobar', lines[-1] }
 
     # Should include hidden files
     (1..100).each { |i| FileUtils.touch("/tmp/fzf-test/.hidden-#{i}") }
     tmux.send_keys 'C-u'
     tmux.send_keys 'cat /tmp/fzf-test/hidden**', :Tab
```

### Comparing `fzf_bin-0.48.1/fzf/uninstall` & `fzf_bin-0.49.0/fzf/uninstall`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.48.1/pdm_build.py` & `fzf_bin-0.49.0/pdm_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from wheel.cli.tags import tags
 
 if TYPE_CHECKING:
     from pdm.backend.hooks import Context
 
 NAME = "fzf"
-VERSION = "0.48.1"
+VERSION = "0.49.0"
 
 
 def is_windows():
     if "GOOS" in os.environ:
         return os.environ["GOOS"] == "windows"
     return sys.platform == "win32"
```

### Comparing `fzf_bin-0.48.1/pyproject.toml` & `fzf_bin-0.49.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fzf-bin"
 description = "fzf - 🌸 A command-line fuzzy finder"
-version = "0.48.1"
+version = "0.49.0"
 authors = [
     { name = "dowon", email = "ks2515@naver.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
```

### Comparing `fzf_bin-0.48.1/PKG-INFO` & `fzf_bin-0.49.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fzf-bin
-Version: 0.48.1
+Version: 0.49.0
 Summary: fzf - 🌸 A command-line fuzzy finder
 Keywords: fzf tui fuzzy finder
 Author-Email: dowon <ks2515@naver.com>
 License: MIT
 Classifier: Programming Language :: Other
 Classifier: Topic :: Software Development :: User Interfaces
 Project-URL: Repository, https://github.com/Bing-su/pip-binary-factory
```

