# Comparing `tmp/tuack-0.1.5.3.tar.gz` & `tmp/tuack-0.1.5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuack-0.1.5.3.tar", last modified: Fri Nov  3 07:57:40 2023, max compression
+gzip compressed data, was "tuack-0.1.5.3.1.tar", last modified: Fri Apr  5 03:17:02 2024, max compression
```

## Comparing `tuack-0.1.5.3.tar` & `tuack-0.1.5.3.1.tar`

### file list

```diff
@@ -1,107 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.409720 tuack-0.1.5.3/
--rw-rw-rw-   0        0        0    35055 2019-01-19 08:45:12.000000 tuack-0.1.5.3/LICENSE
--rw-rw-rw-   0        0        0       17 2018-03-03 08:40:20.000000 tuack-0.1.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0      520 2023-11-03 07:57:40.409720 tuack-0.1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     1717 2023-05-18 04:27:25.000000 tuack-0.1.5.3/README.md
--rw-rw-rw-   0        0        0       42 2023-11-03 07:57:40.409720 tuack-0.1.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1928 2023-11-03 07:57:24.000000 tuack-0.1.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:39.950207 tuack-0.1.5.3/tuack/
--rw-rw-rw-   0        0        0      116 2018-03-03 08:40:20.000000 tuack-0.1.5.3/tuack/__init__.py
--rw-rw-rw-   0        0        0    35277 2023-11-03 07:57:24.000000 tuack-0.1.5.3/tuack/base.py
--rw-rw-rw-   0        0        0    14854 2023-11-03 07:57:24.000000 tuack-0.1.5.3/tuack/doc.py
--rw-rw-rw-   0        0        0    27596 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/dump.py
--rw-rw-rw-   0        0        0    16233 2023-11-03 07:57:24.000000 tuack-0.1.5.3/tuack/gen.py
--rw-rw-rw-   0        0        0     2334 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/install.py
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.141286 tuack-0.1.5.3/tuack/lex/
--rw-rw-rw-   0        0        0        0 2018-09-07 13:38:42.000000 tuack-0.1.5.3/tuack/lex/compile.log
--rw-rw-rw-   0        0        0      971 2019-01-19 08:45:12.000000 tuack-0.1.5.3/tuack/lex/compile.pyinc
--rw-rw-rw-   0        0        0  2295192 2019-01-19 08:45:12.000000 tuack-0.1.5.3/tuack/lex/format-linux
--rw-rw-rw-   0        0        0    61896 2019-01-19 08:45:12.000000 tuack-0.1.5.3/tuack/lex/format-mac
--rwxrwxrwx   0        0        0  2178321 2019-01-19 08:45:12.000000 tuack-0.1.5.3/tuack/lex/format-win.exe
--rw-rw-rw-   0        0        0      320 2018-08-27 16:45:44.000000 tuack-0.1.5.3/tuack/lex/hehe.log
--rw-rw-rw-   0        0        0    11191 2019-01-19 08:45:12.000000 tuack-0.1.5.3/tuack/lex/lex.l
--rw-rw-rw-   0        0        0    94066 2018-09-07 13:38:44.000000 tuack-0.1.5.3/tuack/lex/lex.yy.c
--rw-rw-rw-   0        0        0    36942 2018-06-11 12:35:42.000000 tuack-0.1.5.3/tuack/lex/lex.yy.o
--rw-rw-rw-   0        0        0      185 2019-01-19 08:45:12.000000 tuack-0.1.5.3/tuack/lex/main.h
--rw-rw-rw-   0        0        0    42594 2018-09-07 13:38:44.000000 tuack-0.1.5.3/tuack/lex/yacc.tab.c
--rw-rw-rw-   0        0        0     1906 2018-09-07 13:38:44.000000 tuack-0.1.5.3/tuack/lex/yacc.tab.h
--rw-rw-rw-   0        0        0     9007 2018-06-11 12:35:42.000000 tuack-0.1.5.3/tuack/lex/yacc.tab.o
--rw-rw-rw-   0        0        0      388 2019-01-19 08:45:12.000000 tuack-0.1.5.3/tuack/lex/yacc.y
--rw-rw-rw-   0        0        0    12217 2023-05-20 05:40:17.000000 tuack-0.1.5.3/tuack/load.py
--rw-rw-rw-   0        0        0     3605 2019-01-19 08:45:12.000000 tuack-0.1.5.3/tuack/num2chinese.py
--rw-rw-rw-   0        0        0    13010 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/packer.py
--rw-rw-rw-   0        0        0    25267 2023-11-03 07:57:24.000000 tuack-0.1.5.3/tuack/ren.py
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.219426 tuack-0.1.5.3/tuack/sample/
--rw-rw-rw-   0        0        0     7909 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample/arbiter_e.noi_linux1.sample
--rw-rw-rw-   0        0        0    23576 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample/arbiter_e.sample
--rw-rw-rw-   0        0        0     5586 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample/chk.cpp
--rw-rw-rw-   0        0        0      195 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample/contest.gitignore
--rw-rw-rw-   0        0        0      266 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample/contest.json
--rw-rw-rw-   0        0        0      186 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample/day.gitignore
--rw-rw-rw-   0        0        0      207 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample/day.json
--rw-rw-rw-   0        0        0      351 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample/empty.gitattributes
--rw-rw-rw-   0        0        0      254 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample/empty.gitignore
--rw-rw-rw-   0        0        0      435 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample/empty.json
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.298196 tuack-0.1.5.3/tuack/sample/precautions/
--rw-rw-rw-   0        0        0       60 2023-05-18 04:27:16.000000 tuack-0.1.5.3/tuack/sample/precautions/zh-cn.md
--rw-rw-rw-   0        0        0      342 2018-03-03 08:40:20.000000 tuack-0.1.5.3/tuack/sample/problem.gitattributes
--rw-rw-rw-   0        0        0      254 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample/problem.gitignore
--rw-rw-rw-   0        0        0      466 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample/problem.json
--rw-rw-rw-   0        0        0       76 2018-03-03 08:40:20.000000 tuack-0.1.5.3/tuack/sample/uoj.json
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:39.822383 tuack-0.1.5.3/tuack/sample-empty/
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.219426 tuack-0.1.5.3/tuack/sample-empty/statement/
--rw-rw-rw-   0        0        0      411 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample-empty/statement/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:39.822383 tuack-0.1.5.3/tuack/sample-problem/
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.219426 tuack-0.1.5.3/tuack/sample-problem/data/
--rw-rw-rw-   0        0        0       44 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample-problem/data/1.ans
--rw-rw-rw-   0        0        0       43 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample-problem/data/1.in
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.239355 tuack-0.1.5.3/tuack/sample-problem/down/
--rw-rw-rw-   0        0        0       79 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample-problem/down/1.ans
--rw-rw-rw-   0        0        0       77 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample-problem/down/1.in
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.250426 tuack-0.1.5.3/tuack/sample-problem/pre/
--rw-rw-rw-   0        0        0       80 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample-problem/pre/1.ans
--rw-rw-rw-   0        0        0       78 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample-problem/pre/1.in
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.266121 tuack-0.1.5.3/tuack/sample-problem/resources/
--rw-rw-rw-   0        0        0  3293583 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample-problem/resources/sample.png
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.266121 tuack-0.1.5.3/tuack/sample-problem/solution/
--rw-rw-rw-   0        0        0     1968 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample-problem/solution/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.283193 tuack-0.1.5.3/tuack/sample-problem/statement/
--rw-rw-rw-   0        0        0     6933 2023-11-03 07:57:24.000000 tuack-0.1.5.3/tuack/sample-problem/statement/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.298196 tuack-0.1.5.3/tuack/sample-problem/tables/
--rw-rw-rw-   0        0        0     1060 2023-11-03 07:57:24.000000 tuack-0.1.5.3/tuack/sample-problem/tables/data.pyinc
--rw-rw-rw-   0        0        0     1227 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample-problem/tables/json_data.json
--rw-rw-rw-   0        0        0      205 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/sample-problem/tables/table.json
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.379618 tuack-0.1.5.3/tuack/templates/
--rw-rw-rw-   0        0        0      911 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/templates/ccc.tex.jinja
--rw-rw-rw-   0        0        0    71170 2018-03-03 08:40:20.000000 tuack-0.1.5.3/tuack/templates/ccpc.png
--rw-rw-rw-   0        0        0     1240 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/templates/ccpc.tex.jinja
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:39.822383 tuack-0.1.5.3/tuack/templates/en/
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.393868 tuack-0.1.5.3/tuack/templates/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2978 2019-01-19 08:45:12.000000 tuack-0.1.5.3/tuack/templates/en/LC_MESSAGES/lang.mo
--rw-rw-rw-   0        0        0     3681 2019-01-19 08:45:12.000000 tuack-0.1.5.3/tuack/templates/en/LC_MESSAGES/lang.po
--rw-rw-rw-   0        0        0       77 2019-01-19 08:45:12.000000 tuack-0.1.5.3/tuack/templates/font.html.jinja
--rw-rw-rw-   0        0        0       70 2019-01-19 08:45:12.000000 tuack-0.1.5.3/tuack/templates/font.tex.jinja
--rw-rw-rw-   0        0        0      670 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/templates/hand.tex.jinja
--rw-rw-rw-   0        0        0      144 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/templates/image.html.jinja
--rw-rw-rw-   0        0        0      530 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/templates/image.tex.jinja
--rw-rw-rw-   0        0        0     5116 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/templates/problem_base.md.jinja
--rw-rw-rw-   0        0        0     1051 2019-01-19 08:45:12.000000 tuack-0.1.5.3/tuack/templates/table.html.jinja
--rw-rw-rw-   0        0        0      402 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/templates/table.md.jinja
--rw-rw-rw-   0        0        0     2295 2018-03-03 08:40:20.000000 tuack-0.1.5.3/tuack/templates/table.tex.jinja
--rw-rw-rw-   0        0        0     2125 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/templates/template_base.tex.jinja
--rw-rw-rw-   0        0        0      182 2019-01-19 08:45:12.000000 tuack-0.1.5.3/tuack/templates/template_base.tex.jinja.tex
--rw-rw-rw-   0        0        0     4756 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/templates/tuack.cls
--rw-rw-rw-   0        0        0     8743 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/templates/tuoi.tex.jinja
--rw-rw-rw-   0        0        0     1443 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/templates/tupc.tex.jinja
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:39.822383 tuack-0.1.5.3/tuack/templates/zh-cn/
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:40.409720 tuack-0.1.5.3/tuack/templates/zh-cn/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3139 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/templates/zh-cn/LC_MESSAGES/lang.mo
--rw-rw-rw-   0        0        0     3543 2023-05-18 04:27:25.000000 tuack-0.1.5.3/tuack/templates/zh-cn/LC_MESSAGES/lang.po
--rw-rw-rw-   0        0        0    17556 2023-05-20 05:40:17.000000 tuack-0.1.5.3/tuack/test.py
--rw-rw-rw-   0        0        0     4790 2023-11-03 07:57:24.000000 tuack-0.1.5.3/tuack/tools.py
-drwxrwxrwx   0        0        0        0 2023-11-03 07:57:39.950207 tuack-0.1.5.3/tuack.egg-info/
--rw-rw-rw-   0        0        0      520 2023-11-03 07:57:39.000000 tuack-0.1.5.3/tuack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2261 2023-11-03 07:57:39.000000 tuack-0.1.5.3/tuack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-03 07:57:39.000000 tuack-0.1.5.3/tuack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-11-03 07:57:39.000000 tuack-0.1.5.3/tuack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-11-03 07:57:39.000000 tuack-0.1.5.3/tuack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:02.007196 tuack-0.1.5.3.1/
+-rw-rw-rw-   0        0        0    35055 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/LICENSE
+-rw-rw-rw-   0        0        0       17 2018-03-03 08:40:20.000000 tuack-0.1.5.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      522 2024-04-05 03:17:02.007196 tuack-0.1.5.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1692 2024-04-05 03:14:10.000000 tuack-0.1.5.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 03:17:02.007196 tuack-0.1.5.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1930 2024-04-05 03:14:12.000000 tuack-0.1.5.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.957151 tuack-0.1.5.3.1/tuack/
+-rw-rw-rw-   0        0        0      116 2018-03-03 08:40:20.000000 tuack-0.1.5.3.1/tuack/__init__.py
+-rw-rw-rw-   0        0        0    35277 2024-01-01 10:29:06.000000 tuack-0.1.5.3.1/tuack/base.py
+-rw-rw-rw-   0        0        0    14874 2024-04-05 03:14:11.000000 tuack-0.1.5.3.1/tuack/doc.py
+-rw-rw-rw-   0        0        0    27961 2024-04-05 03:13:19.000000 tuack-0.1.5.3.1/tuack/dump.py
+-rw-rw-rw-   0        0        0    16960 2024-04-05 03:13:19.000000 tuack-0.1.5.3.1/tuack/gen.py
+-rw-rw-rw-   0        0        0     2334 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/install.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.975997 tuack-0.1.5.3.1/tuack/lex/
+-rw-rw-rw-   0        0        0      971 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/tuack/lex/compile.pyinc
+-rw-rw-rw-   0        0        0  2295192 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/tuack/lex/format-linux
+-rw-rw-rw-   0        0        0    61896 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/tuack/lex/format-mac
+-rwxrwxrwx   0        0        0  2178321 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/tuack/lex/format-win.exe
+-rw-rw-rw-   0        0        0    11191 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/tuack/lex/lex.l
+-rw-rw-rw-   0        0        0      185 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/tuack/lex/main.h
+-rw-rw-rw-   0        0        0      388 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/tuack/lex/yacc.y
+-rw-rw-rw-   0        0        0    12217 2023-05-20 05:40:18.000000 tuack-0.1.5.3.1/tuack/load.py
+-rw-rw-rw-   0        0        0     3605 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/tuack/num2chinese.py
+-rw-rw-rw-   0        0        0    13010 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/packer.py
+-rw-rw-rw-   0        0        0    25275 2024-04-05 03:13:19.000000 tuack-0.1.5.3.1/tuack/ren.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.983969 tuack-0.1.5.3.1/tuack/sample/
+-rw-rw-rw-   0        0        0     7909 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample/arbiter_e.noi_linux1.sample
+-rw-rw-rw-   0        0        0    23576 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample/arbiter_e.sample
+-rw-rw-rw-   0        0        0     5586 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample/chk.cpp
+-rw-rw-rw-   0        0        0      195 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample/contest.gitignore
+-rw-rw-rw-   0        0        0      266 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample/contest.json
+-rw-rw-rw-   0        0        0      186 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample/day.gitignore
+-rw-rw-rw-   0        0        0      207 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample/day.json
+-rw-rw-rw-   0        0        0      351 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample/empty.gitattributes
+-rw-rw-rw-   0        0        0      254 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample/empty.gitignore
+-rw-rw-rw-   0        0        0      435 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample/empty.json
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.996034 tuack-0.1.5.3.1/tuack/sample/precautions/
+-rw-rw-rw-   0        0        0       60 2023-05-18 04:27:18.000000 tuack-0.1.5.3.1/tuack/sample/precautions/zh-cn.md
+-rw-rw-rw-   0        0        0      342 2018-03-03 08:40:20.000000 tuack-0.1.5.3.1/tuack/sample/problem.gitattributes
+-rw-rw-rw-   0        0        0      254 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample/problem.gitignore
+-rw-rw-rw-   0        0        0      466 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample/problem.json
+-rw-rw-rw-   0        0        0       76 2018-03-03 08:40:20.000000 tuack-0.1.5.3.1/tuack/sample/uoj.json
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.906893 tuack-0.1.5.3.1/tuack/sample-empty/
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.983969 tuack-0.1.5.3.1/tuack/sample-empty/statement/
+-rw-rw-rw-   0        0        0      411 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample-empty/statement/zh-cn.md
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.908897 tuack-0.1.5.3.1/tuack/sample-problem/
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.984965 tuack-0.1.5.3.1/tuack/sample-problem/data/
+-rw-rw-rw-   0        0        0       44 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample-problem/data/1.ans
+-rw-rw-rw-   0        0        0       43 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample-problem/data/1.in
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.985962 tuack-0.1.5.3.1/tuack/sample-problem/down/
+-rw-rw-rw-   0        0        0       79 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample-problem/down/1.ans
+-rw-rw-rw-   0        0        0       77 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample-problem/down/1.in
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.987956 tuack-0.1.5.3.1/tuack/sample-problem/pre/
+-rw-rw-rw-   0        0        0       80 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample-problem/pre/1.ans
+-rw-rw-rw-   0        0        0       78 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample-problem/pre/1.in
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.987956 tuack-0.1.5.3.1/tuack/sample-problem/resources/
+-rw-rw-rw-   0        0        0  3293583 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample-problem/resources/sample.png
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.991942 tuack-0.1.5.3.1/tuack/sample-problem/solution/
+-rw-rw-rw-   0        0        0     1968 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample-problem/solution/zh-cn.md
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.992939 tuack-0.1.5.3.1/tuack/sample-problem/statement/
+-rw-rw-rw-   0        0        0     6933 2023-11-03 07:57:26.000000 tuack-0.1.5.3.1/tuack/sample-problem/statement/zh-cn.md
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.994933 tuack-0.1.5.3.1/tuack/sample-problem/tables/
+-rw-rw-rw-   0        0        0     1181 2024-04-05 03:13:19.000000 tuack-0.1.5.3.1/tuack/sample-problem/tables/data.pyinc
+-rw-rw-rw-   0        0        0     1227 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample-problem/tables/json_data.json
+-rw-rw-rw-   0        0        0      205 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/sample-problem/tables/table.json
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:02.004149 tuack-0.1.5.3.1/tuack/templates/
+-rw-rw-rw-   0        0        0      911 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/templates/ccc.tex.jinja
+-rw-rw-rw-   0        0        0    71170 2018-03-03 08:40:20.000000 tuack-0.1.5.3.1/tuack/templates/ccpc.png
+-rw-rw-rw-   0        0        0     1240 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/templates/ccpc.tex.jinja
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.908897 tuack-0.1.5.3.1/tuack/templates/en/
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:02.005145 tuack-0.1.5.3.1/tuack/templates/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2978 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/tuack/templates/en/LC_MESSAGES/lang.mo
+-rw-rw-rw-   0        0        0     3681 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/tuack/templates/en/LC_MESSAGES/lang.po
+-rw-rw-rw-   0        0        0       77 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/tuack/templates/font.html.jinja
+-rw-rw-rw-   0        0        0       70 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/tuack/templates/font.tex.jinja
+-rw-rw-rw-   0        0        0      670 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/templates/hand.tex.jinja
+-rw-rw-rw-   0        0        0      144 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/templates/image.html.jinja
+-rw-rw-rw-   0        0        0      530 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/templates/image.tex.jinja
+-rw-rw-rw-   0        0        0     5116 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/templates/problem_base.md.jinja
+-rw-rw-rw-   0        0        0     1051 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/tuack/templates/table.html.jinja
+-rw-rw-rw-   0        0        0      402 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/templates/table.md.jinja
+-rw-rw-rw-   0        0        0     2295 2018-03-03 08:40:20.000000 tuack-0.1.5.3.1/tuack/templates/table.tex.jinja
+-rw-rw-rw-   0        0        0     2125 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/templates/template_base.tex.jinja
+-rw-rw-rw-   0        0        0      182 2019-01-19 08:45:12.000000 tuack-0.1.5.3.1/tuack/templates/template_base.tex.jinja.tex
+-rw-rw-rw-   0        0        0     4756 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/templates/tuack.cls
+-rw-rw-rw-   0        0        0     8743 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/templates/tuoi.tex.jinja
+-rw-rw-rw-   0        0        0     1443 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/templates/tupc.tex.jinja
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.909893 tuack-0.1.5.3.1/tuack/templates/zh-cn/
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:02.006141 tuack-0.1.5.3.1/tuack/templates/zh-cn/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     3139 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/templates/zh-cn/LC_MESSAGES/lang.mo
+-rw-rw-rw-   0        0        0     3543 2023-05-18 04:27:26.000000 tuack-0.1.5.3.1/tuack/templates/zh-cn/LC_MESSAGES/lang.po
+-rw-rw-rw-   0        0        0    17556 2023-05-20 05:40:18.000000 tuack-0.1.5.3.1/tuack/test.py
+-rw-rw-rw-   0        0        0     4790 2023-11-03 07:57:26.000000 tuack-0.1.5.3.1/tuack/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-05 03:17:01.967023 tuack-0.1.5.3.1/tuack.egg-info/
+-rw-rw-rw-   0        0        0      522 2024-04-05 03:17:01.000000 tuack-0.1.5.3.1/tuack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2119 2024-04-05 03:17:01.000000 tuack-0.1.5.3.1/tuack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 03:17:01.000000 tuack-0.1.5.3.1/tuack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2024-04-05 03:17:01.000000 tuack-0.1.5.3.1/tuack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-05 03:17:01.000000 tuack-0.1.5.3.1/tuack.egg-info/top_level.txt
```

### Comparing `tuack-0.1.5.3/LICENSE` & `tuack-0.1.5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/PKG-INFO` & `tuack-0.1.5.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuack
-Version: 0.1.5.3
+Version: 0.1.5.3.1
 Summary: Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.
 Home-page: 
 Author: Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan
 Author-email: chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn
 License: https://git.thusaac.com/publish/tuack/blob/master/LICENSE
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `tuack-0.1.5.3/README.md` & `tuack-0.1.5.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 ## 简介
 
 一般在 4 个地方更新：
 
 * [https://gitee.com/mulab/oi_tools](https://gitee.com/mulab/oi_tools)：主要的工作地址，所有分支都会在这里；可以提 issue。
-* [https://git.thusaac.com/publish/tuack](https://git.thusaac.com/publish/tuack)：最近算协服务器又没人管了，正常所有分支都会在这里；非清华贵系算协成员不能提 issue。
-* [https://saac.cs.tsinghua.edu.cn/publish/tuack](https://git.thusaac.org/publish/tuack)：清华校内的服务器现在搬到这里了。
 * [https://github.com/Mulab11/tuack](https://github.com/Mulab11/tuack)：可以提 issue，可能不会及时更新。
+* <del>[https://saac.cs.tsinghua.edu.cn/publish/tuack](https://git.thusaac.org/publish/tuack)：清华校内的服务器现在搬到这里了。</del>
+* <del>[https://git.thusaac.com/publish/tuack](https://git.thusaac.com/publish/tuack)：最近算协服务器又没人管了，正常所有分支都会在这里；非清华贵系算协成员不能提 issue。</del>
+
 
 此外如果有任何疑问或建议，知道我 QQ 或微信的小伙伴也可以用这些工具告诉我。
 
 这个轮子打算逐步实现：
 
 * 合作：通过共同使用git和遵循一些约定，降低合作命题者之间版本控制，题面修改，代码、数据交换，bug修复等的成本。
 * 规范：对题目的各个方面进行评估，找出可能出错的风险点，帮助出题人减少出锅的概率。
@@ -18,9 +19,7 @@
 这个轮子主要是面向出题人、OJ站长和教师，方便大家造题和分享题目。
 
 目前这个轮子还在you开yi发dui中bug。如果希望我们支持其他格式的题面，其他工具的导入导出，对这个轮子有任何建议或意见，发现了任何bug，或是有兴趣加入我们，欢迎随时联系。
 
 ## 文档
 
 [文档在这里](https://gitee.com/mulab/oi_tools/wikis/home)
-
-这个文档有一些图是坏的，待修。
```

### Comparing `tuack-0.1.5.3/setup.py` & `tuack-0.1.5.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 	'pyyaml >= 5.1',
 	'rarfile >= 3.0',
 	'requests_toolbelt >= 0.9.1'
 ]
 
 setup(
 	name = 'tuack',
-	version = '0.1.5.3',
+	version = '0.1.5.3.1',
 	packages = find_packages(),
 	author = 'Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan',
 	author_email = 'chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn',
 	url = '',
 	license = 'https://git.thusaac.com/publish/tuack/blob/master/LICENSE',
 	description = 'Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.',
 	cmdclass={
```

### Comparing `tuack-0.1.5.3/tuack/base.py` & `tuack-0.1.5.3.1/tuack/base.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/doc.py` & `tuack-0.1.5.3.1/tuack/doc.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,15 +353,15 @@
 			if line.startswith('|') and line.endswith('|'):
 				if tbl_lino == 0:
 					tbl_no += 1
 					log.info(f"表格：{tbl_no}")
 					buff = clear(buff)
 					cur.lines.append("{{ tbl('%d') }}\n" % tbl_no)
 					base.mkdir('tables')
-					ftbl = open(f"tables/{tbl_no}.pyinc", 'w')
+					ftbl = open(f"tables/{tbl_no}.pyinc", 'w', encoding = 'utf-8')
 					ftbl.write('return [\n')
 				tbl_lino += 1
 				if tbl_lino != 2:
 					ftbl.write("\t[r'" + "', r'".join(map(lambda x : x.strip(), line.strip('|').split('|'))) + "'],\n")
 				continue
 			elif tbl_lino != 0:
 				ftbl.write(']\n')
```

### Comparing `tuack-0.1.5.3/tuack/dump.py` & `tuack-0.1.5.3.1/tuack/dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,23 @@
 				dirname = prob['name']+'-'+str(idx)+str(idx2)
 				codename = userdir + code
 				tmplist = prob['users'][userdir][code].split('/')
 				codedir = base.pjoin(prob.path,*tmplist)
 				os.makedirs(base.pjoin('arbiter','players',conf['name'],dirname,prob['name']))
 				shutil.copy(codedir,base.pjoin('arbiter','players',conf['name'],dirname,prob['name']))
 				userlist[dirname + '@'] =  codename'''
-		shutil.copy(base.pjoin(base.path,'sample','arbiter_e.sample'),base.pjoin('arbiter', 'main','filter',prob['name']+'_e'))
+		
+		if os.path.isdir(base.pjoin(prob.path, 'data', 'chk')) and os.path.isfile(base.pjoin(prob.path, 'data', 'chk', 'chk.cpp')):
+			log.info('发现chk，尝试编译。')
+			os.system("g++ %s -o %s -O2 -std=c++17" % (
+				base.pjoin(prob.path, 'data', 'chk', 'chk.cpp'),
+				base.pjoin('arbiter', 'main','filter',prob['name']+'_e')
+			))
+		else:
+			shutil.copy(base.pjoin(base.path,'sample','arbiter_e.sample'),base.pjoin('arbiter', 'main','filter',prob['name']+'_e'))
 		arbiter_info(probinfo,base.pjoin('arbiter', 'main','task'+str(daynum)+'_'+str(probnum)+'.info'))
 
 def arbiter_down(conf = None):
 	if not conf:
 		conf = base.conf
 		if not os.path.exists('arbiter'):
 			base.remkdir('arbiter')
@@ -568,15 +576,15 @@
 		}
 	if conf['type'] == 'output':
 		data_yml['userOutput'] = (conf['name'] if conf.get('file io') else '') + '#.out'
 	if conf.get('extra'):
 		files = [{'name' : exname, 'dest' : exname} for exname in conf['extra']]
 		data_yml['extraSourceFiles'] = [
 			{'language' : lan, 'files' : files} \
-			for lan in ['cpp', 'c', 'cpp11', 'cpp17']
+			for lan in ['cpp', 'c', 'cpp11', 'cpp17', 'cpp14']
 		]
 	data_path = 'data' if not pre else 'pre'
 	open(pjoin(base.work, data_path, conf.route + '.yml'), 'wb').write(base.dump_formats['yaml'](data_yml))
 	def pack(z, path, fname, force_file = False):
 		full_path = pjoin(path, fname)
 		print(u"打包文件`%s`  " % full_path, end = '\r')
 		sys.stdout.flush()
```

### Comparing `tuack-0.1.5.3/tuack/gen.py` & `tuack-0.1.5.3.1/tuack/gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,18 +316,20 @@
 		st_path = pjoin(path, ff)
 		if not os.path.exists(st_path):
 			os.makedirs(st_path)
 		for f in os.listdir(pjoin(base.path, 'sample', ff)):
 			copy(pjoin(ff, f), pjoin(ff, f))
 
 def set_conf(params, folders, tp = str):
+	if type(params) != tuple and type(params) != list:
+		params = (params,)
 	if base.conf['folder'] not in folders:
 		log.error(f"只能在{folders}类型目录下运行当前命令")
 		return
-	for sub, val in zip(base.conf.sub, sys.argv[2:]):
+	for sub, val in zip(base.conf.sub, sys.argv[2+int(tp == json.loads):]):
 		t = sub
 		for i in params[:-1]:
 			t = t[i]
 		t[params[-1]] = tp(val)
 		base.save_json(sub)
 
 def set_length():
@@ -350,14 +352,15 @@
 	'upgrade' : upgrade,
 	'lfs' : copy_lfs,
 	'chk' : copy_chk,
 	'prec' : copy_prec,
 	'title' : lambda : set_conf(('title', 'zh-cn'), {'contest', 'day'}),
 	'time' : lambda : set_conf(('time limit', ), {'day'}, float),
 	'memory' : lambda : set_conf(('memory limit', ), {'day'}, float),
+	'conf' : lambda : set_conf(json.loads(sys.argv[2]), {'contest', 'day', 'problem'}, json.loads),
 	'length' : set_length
 }
 work_list['auto'] = lambda : [work_list[key]() for key in ['data', 'samples', 'pre', 'code']]
 work_list['n'] = work_list['contest']
 work_list['d'] = work_list['day']
 work_list['p'] = work_list['problem']
 work_list['e'] = work_list['empty']
@@ -365,14 +368,15 @@
 work_list['s'] = work_list['samples']
 work_list['u'] = work_list['upgrade']
 work_list['a'] = work_list['auto']
 work_list['l'] = work_list['title']
 work_list['i'] = work_list['time']
 work_list['m'] = work_list['memory']
 work_list['g'] = work_list['length']
+work_list['f'] = work_list['conf']
 
 if __name__ == '__main__':
 	try:
 		result = base.init()
 	except base.NoFileException as e:
 		base.conf = None
 		result = True
@@ -415,7 +419,12 @@
 		log.info(u'  l        同title。')
 		log.info(u'  time     设置每道题的时间限制，依次传入每道题的时间限制。')
 		log.info(u'  i        同time。')
 		log.info(u'  memory   设置每道题的空间限制，依次传入每道题的时间限制。')
 		log.info(u'  m        同memory。')
 		log.info(u'  length   设置每个比赛日或当前比赛日的时长，依次用浮点数以小时为单位传入。')
 		log.info(u'  g        同length。')
+		log.info(u'  conf     批量设置字段，先传入字段名（可用数组表示层次），然后依次用json格式传入要改的内容。例如：')
+		log.info(u'           tuack.gen conf \'"file io"\' true true true true')
+		log.info(u'           tuack.gen conf \'"compile"\' \'{"cpp" : "-O2 -std=c++14"}\' \'{"cpp" : "-O2 -std=c++14"}\'')
+		log.info(u'           tuack.gen conf \'["compile","cpp"]\' \'"-O2 -std=c++14"\' \'"-O2 -std=c++14"\'')
+		log.info(u'  f        同conf。')
```

### Comparing `tuack-0.1.5.3/tuack/install.py` & `tuack-0.1.5.3.1/tuack/install.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/lex/compile.pyinc` & `tuack-0.1.5.3.1/tuack/lex/compile.pyinc`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/lex/format-linux` & `tuack-0.1.5.3.1/tuack/lex/format-linux`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/lex/format-mac` & `tuack-0.1.5.3.1/tuack/lex/format-mac`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/lex/format-win.exe` & `tuack-0.1.5.3.1/tuack/lex/format-win.exe`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/lex/lex.l` & `tuack-0.1.5.3.1/tuack/lex/lex.l`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/load.py` & `tuack-0.1.5.3.1/tuack/load.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/num2chinese.py` & `tuack-0.1.5.3.1/tuack/num2chinese.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/packer.py` & `tuack-0.1.5.3.1/tuack/packer.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/ren.py` & `tuack-0.1.5.3.1/tuack/ren.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
 		if len(args) > 0:
 			try:
 				ret = ret % args
 			except Exception as e:
 				ret = ret + ''.join(map(str, args))
 		elif title == 'sample explanation':
 			try:
-				ret = ret % (self.context['vars']['sample_id'], )
+				ret = ret % (self.context['vars'].get('sample_id', ''), )
 			except Exception as e:
 				pass
 		else:
 			try:
 				ret = ret % ('',)
 			except Exception as e:
 				pass
```

### Comparing `tuack-0.1.5.3/tuack/sample/arbiter_e.noi_linux1.sample` & `tuack-0.1.5.3.1/tuack/sample/arbiter_e.noi_linux1.sample`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/sample/arbiter_e.sample` & `tuack-0.1.5.3.1/tuack/sample/arbiter_e.sample`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/sample/chk.cpp` & `tuack-0.1.5.3.1/tuack/sample/chk.cpp`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/sample-problem/resources/sample.png` & `tuack-0.1.5.3.1/tuack/sample-problem/resources/sample.png`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/sample-problem/solution/zh-cn.md` & `tuack-0.1.5.3.1/tuack/sample-problem/solution/zh-cn.md`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/sample-problem/statement/zh-cn.md` & `tuack-0.1.5.3.1/tuack/sample-problem/statement/zh-cn.md`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/sample-problem/tables/data.pyinc` & `tuack-0.1.5.3.1/tuack/sample-problem/tables/data.pyinc`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ret = [["测试点","$n$","$m$","是否为完全二叉树"]]	#注意右斜杠经常需要两次转义
+	#表格中的竖线（绝对值符号）一般用\lvert\rvert，否则会和某些环境下的表格分隔符号冲突
 for datum in prob['data']:	#引用conf.json/yaml中的变量
 	args = datum['args']
 	row = [
 		tl.cases(datum['cases']),			#tl.cases(数组)对于整数编号数组会整合成形如$1\sim 3,5$
 		"$= %s$" % tl.hn(args['n']),		#tl.hn函数用于把10000输出成10^{4}这样好看的样子
 											#python的字符串可以直接用百分号格式化成新的字符串
 		r"$\le %s$" % args['m'].hn(),		#Python可以用前面加r的禁止转义字符串解决右斜杠需要两次转义的问题
```

### Comparing `tuack-0.1.5.3/tuack/sample-problem/tables/json_data.json` & `tuack-0.1.5.3.1/tuack/sample-problem/tables/json_data.json`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/ccc.tex.jinja` & `tuack-0.1.5.3.1/tuack/templates/ccc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/ccpc.png` & `tuack-0.1.5.3.1/tuack/templates/ccpc.png`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/ccpc.tex.jinja` & `tuack-0.1.5.3.1/tuack/templates/ccpc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/en/LC_MESSAGES/lang.mo` & `tuack-0.1.5.3.1/tuack/templates/en/LC_MESSAGES/lang.mo`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/en/LC_MESSAGES/lang.po` & `tuack-0.1.5.3.1/tuack/templates/en/LC_MESSAGES/lang.po`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/hand.tex.jinja` & `tuack-0.1.5.3.1/tuack/templates/hand.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/image.tex.jinja` & `tuack-0.1.5.3.1/tuack/templates/image.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/problem_base.md.jinja` & `tuack-0.1.5.3.1/tuack/templates/problem_base.md.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/table.html.jinja` & `tuack-0.1.5.3.1/tuack/templates/table.html.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/table.tex.jinja` & `tuack-0.1.5.3.1/tuack/templates/table.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/template_base.tex.jinja` & `tuack-0.1.5.3.1/tuack/templates/template_base.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/tuack.cls` & `tuack-0.1.5.3.1/tuack/templates/tuack.cls`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/tuoi.tex.jinja` & `tuack-0.1.5.3.1/tuack/templates/tuoi.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/tupc.tex.jinja` & `tuack-0.1.5.3.1/tuack/templates/tupc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/zh-cn/LC_MESSAGES/lang.mo` & `tuack-0.1.5.3.1/tuack/templates/zh-cn/LC_MESSAGES/lang.mo`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/templates/zh-cn/LC_MESSAGES/lang.po` & `tuack-0.1.5.3.1/tuack/templates/zh-cn/LC_MESSAGES/lang.po`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/test.py` & `tuack-0.1.5.3.1/tuack/test.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack/tools.py` & `tuack-0.1.5.3.1/tuack/tools.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.3/tuack.egg-info/PKG-INFO` & `tuack-0.1.5.3.1/tuack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuack
-Version: 0.1.5.3
+Version: 0.1.5.3.1
 Summary: Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.
 Home-page: 
 Author: Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan
 Author-email: chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn
 License: https://git.thusaac.com/publish/tuack/blob/master/LICENSE
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `tuack-0.1.5.3/tuack.egg-info/SOURCES.txt` & `tuack-0.1.5.3.1/tuack.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,27 +15,20 @@
 tuack/test.py
 tuack/tools.py
 tuack.egg-info/PKG-INFO
 tuack.egg-info/SOURCES.txt
 tuack.egg-info/dependency_links.txt
 tuack.egg-info/requires.txt
 tuack.egg-info/top_level.txt
-tuack/lex/compile.log
 tuack/lex/compile.pyinc
 tuack/lex/format-linux
 tuack/lex/format-mac
 tuack/lex/format-win.exe
-tuack/lex/hehe.log
 tuack/lex/lex.l
-tuack/lex/lex.yy.c
-tuack/lex/lex.yy.o
 tuack/lex/main.h
-tuack/lex/yacc.tab.c
-tuack/lex/yacc.tab.h
-tuack/lex/yacc.tab.o
 tuack/lex/yacc.y
 tuack/sample/arbiter_e.noi_linux1.sample
 tuack/sample/arbiter_e.sample
 tuack/sample/chk.cpp
 tuack/sample/contest.gitignore
 tuack/sample/contest.json
 tuack/sample/day.gitignore
```

