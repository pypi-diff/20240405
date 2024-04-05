# Comparing `tmp/sketchingpy-0.1.7.tar.gz` & `tmp/sketchingpy-0.1.8.tar.gz`

## Comparing `sketchingpy-0.1.7.tar` & `sketchingpy-0.1.8.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/.gitattributes
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/CONDUCT.md
--rw-r--r--   0        0        0     9389 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/GOVERNANCE.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/setup.cfg
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/.woodpecker/build.yml
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/.woodpecker/deploy.yml
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/ci-image/Dockerfile
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/ci-image/README.md
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/__init__.py
--rw-r--r--   0        0        0    29739 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/abstracted.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/bezier_util.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/const.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/control_struct.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/data_struct.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/dialog_struct.py
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/geo.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/local_data_struct.py
--rw-r--r--   0        0        0    14290 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/pillow_struct.py
--rw-r--r--   0        0        0    14907 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/pillow_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/py.typed
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/pygame_prompt.py
--rw-r--r--   0        0        0    12404 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/shape_struct.py
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/sketch2d_keymap.py
--rw-r--r--   0        0        0    36231 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/sketch2dapp.py
--rw-r--r--   0        0        0    19729 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/sketch2dstatic.py
--rw-r--r--   0        0        0    31381 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/sketch2dweb.py
--rw-r--r--   0        0        0    12390 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/state_struct.py
--rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/transform.py
--rw-r--r--   0        0        0   133720 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/test/IBMPlexMono-Regular.ttf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/test/__init__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/test/test_abstracted.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/test/test_bezier_util.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/test/test_control_struct.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/test/test_geo.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/test/test_local_data_struct.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/test/test_pillow_struct.py
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/test/test_pillow_util.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/test/test_shape_struct.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/test/test_sketch2d_keymap.py
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/test/test_state_struct.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/sketchingpy/test/test_transform.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/support/check_website.sh
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/support/make_twine_config.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/support/render_and_serve_web.sh
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/support/render_example_test.py
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/support/render_website.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/support/render_website.sh
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/support/run_all_local.sh
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/support/run_all_static.sh
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/support/run_all_web.sh
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/support/serve_local.sh
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/support/update_version.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/web_test_harness/example.html
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/web_test_harness/run_harness.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/web_test_harness/template.html
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/base.html
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/community.html
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/editor.html
--rw-r--r--   0        0        0    31056 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/examples.html
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/guides.html
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/index.html
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/pages.yml
--rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/privacy.html
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/reference.html
--rw-r--r--   0        0        0   112869 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/reference.yml
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/reference_page.html
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/toc.html
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/community/code.html
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/community/conventions.html
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/community/discord.html
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/community/document.html
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/community/issue.html
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/community/showcase.html
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/css/base.css
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/css/editor.css
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/css/index.css
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/guides/deploy.html
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/guides/start.html
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/guides/web_detailed.html
--rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/guides/why.html
--rw-r--r--   0        0        0    72393 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/code.png
--rw-r--r--   0        0        0   102405 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/conventions.png
--rw-r--r--   0        0        0    37446 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/data_write_csv.png
--rw-r--r--   0        0        0    33466 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/data_write_json.png
--rw-r--r--   0        0        0    18883 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/deploy.png
--rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/dialog_simple.png
--rw-r--r--   0        0        0    14777 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/discord.png
--rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/document.png
--rw-r--r--   0        0        0    34074 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/hello_interactive.png
--rw-r--r--   0        0        0   286632 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/home_screen.png
--rw-r--r--   0        0        0    12681 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/inputs_keyboard.png
--rw-r--r--   0        0        0    17039 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/inputs_mouse.png
--rw-r--r--   0        0        0    63534 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/issue.png
--rw-r--r--   0        0        0    74013 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/start.png
--rw-r--r--   0        0        0    74440 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/web_detailed.png
--rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/img/why.png
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/js/editor.js
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/js/index.js
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party/README.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party/core.css
--rw-r--r--   0        0        0    73905 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party/core.js
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party/error-96hMSEw8.js
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party/es.js
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party/py-terminal-XWbSa71s.js
--rw-r--r--   0        0        0    84412 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party/pyodide-lock.json
--rw-r--r--   0        0        0  1157891 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party/pyodide.asm.js
--rw-r--r--   0        0        0  8995509 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party/pyodide.asm.wasm
--rw-r--r--   0        0        0    17133 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party/pyodide.mjs
--rw-r--r--   0        0        0  8882369 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party/python_stdlib.zip
--rw-r--r--   0        0        0    21511 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party/toml--Dzglv4T.js
--rw-r--r--   0        0        0   133720 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party_site/IBMPlexMono-Regular.ttf
--rw-r--r--   0        0        0   192980 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party_site/IBMPlexSans-Regular.ttf
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party_site/README.md
--rw-r--r--   0        0        0   425040 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party_site/ace.min.js
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party_site/mode-python.js
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party_site/theme-textmate-css.js
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/website_src/third_party_site/theme-textmate.js
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/.gitignore
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/LICENSE.md
--rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/README.md
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0    15875 2020-02-02 00:00:00.000000 sketchingpy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/.gitattributes
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/CONDUCT.md
+-rw-r--r--   0        0        0     9389 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/GOVERNANCE.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/setup.cfg
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/.woodpecker/build.yml
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/.woodpecker/deploy.yml
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/ci-image/Dockerfile
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/ci-image/README.md
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/__init__.py
+-rw-r--r--   0        0        0    30238 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/abstracted.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/bezier_util.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/const.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/control_struct.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/data_struct.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/dialog_struct.py
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/geo.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/local_data_struct.py
+-rw-r--r--   0        0        0    14290 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/pillow_struct.py
+-rw-r--r--   0        0        0    14907 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/pillow_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/py.typed
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/pygame_prompt.py
+-rw-r--r--   0        0        0    12404 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/shape_struct.py
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/sketch2d_keymap.py
+-rw-r--r--   0        0        0    36231 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/sketch2dapp.py
+-rw-r--r--   0        0        0    19729 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/sketch2dstatic.py
+-rw-r--r--   0        0        0    31211 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/sketch2dweb.py
+-rw-r--r--   0        0        0    12390 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/state_struct.py
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/transform.py
+-rw-r--r--   0        0        0   133720 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/test/IBMPlexMono-Regular.ttf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/test/__init__.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/test/test_abstracted.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/test/test_bezier_util.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/test/test_control_struct.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/test/test_geo.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/test/test_local_data_struct.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/test/test_pillow_struct.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/test/test_pillow_util.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/test/test_shape_struct.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/test/test_sketch2d_keymap.py
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/test/test_state_struct.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/sketchingpy/test/test_transform.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/support/check_website.sh
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/support/make_twine_config.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/support/render_and_serve_web.sh
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/support/render_example_test.py
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/support/render_website.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/support/render_website.sh
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/support/run_all_local.sh
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/support/run_all_static.sh
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/support/run_all_web.sh
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/support/serve_local.sh
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/support/update_version.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/web_test_harness/example.html
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/web_test_harness/run_harness.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/web_test_harness/template.html
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/base.html
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/community.html
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/editor.html
+-rw-r--r--   0        0        0    21068 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/examples.html
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/guides.html
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/index.html
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/pages.yml
+-rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/privacy.html
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/reference.html
+-rw-r--r--   0        0        0   112924 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/reference.yml
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/reference_page.html
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/toc.html
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/community/code.html
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/community/conventions.html
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/community/discord.html
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/community/document.html
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/community/issue.html
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/community/showcase.html
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/css/base.css
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/css/editor.css
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/css/index.css
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/guides/deploy.html
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/guides/start.html
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/guides/web_detailed.html
+-rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/guides/why.html
+-rw-r--r--   0        0        0    72393 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/code.png
+-rw-r--r--   0        0        0   102405 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/conventions.png
+-rw-r--r--   0        0        0    37446 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/data_write_csv.png
+-rw-r--r--   0        0        0    33466 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/data_write_json.png
+-rw-r--r--   0        0        0    18883 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/deploy.png
+-rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/dialog_simple.png
+-rw-r--r--   0        0        0    14777 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/discord.png
+-rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/document.png
+-rw-r--r--   0        0        0    34074 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/hello_interactive.png
+-rw-r--r--   0        0        0   286632 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/home_screen.png
+-rw-r--r--   0        0        0    12681 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/inputs_keyboard.png
+-rw-r--r--   0        0        0    17039 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/inputs_mouse.png
+-rw-r--r--   0        0        0    63534 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/issue.png
+-rw-r--r--   0        0        0    74013 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/start.png
+-rw-r--r--   0        0        0    74440 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/web_detailed.png
+-rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/img/why.png
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/js/editor.js
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/js/index.js
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party/README.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party/core.css
+-rw-r--r--   0        0        0    73905 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party/core.js
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party/error-96hMSEw8.js
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party/es.js
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party/py-terminal-XWbSa71s.js
+-rw-r--r--   0        0        0    84412 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party/pyodide-lock.json
+-rw-r--r--   0        0        0  1157891 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party/pyodide.asm.js
+-rw-r--r--   0        0        0  8995509 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party/pyodide.asm.wasm
+-rw-r--r--   0        0        0    17133 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party/pyodide.mjs
+-rw-r--r--   0        0        0  8882369 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party/python_stdlib.zip
+-rw-r--r--   0        0        0    21511 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party/toml--Dzglv4T.js
+-rw-r--r--   0        0        0   133720 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party_site/IBMPlexMono-Regular.ttf
+-rw-r--r--   0        0        0   192980 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party_site/IBMPlexSans-Regular.ttf
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party_site/README.md
+-rw-r--r--   0        0        0   425040 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party_site/ace.min.js
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party_site/mode-python.js
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party_site/theme-textmate-css.js
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/website_src/third_party_site/theme-textmate.js
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/README.md
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    15875 2020-02-02 00:00:00.000000 sketchingpy-0.1.8/PKG-INFO
```

### Comparing `sketchingpy-0.1.7/CONDUCT.md` & `sketchingpy-0.1.8/CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/CONTRIBUTING.md` & `sketchingpy-0.1.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/GOVERNANCE.md` & `sketchingpy-0.1.8/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/.woodpecker/build.yml` & `sketchingpy-0.1.8/.woodpecker/build.yml`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/.woodpecker/deploy.yml` & `sketchingpy-0.1.8/.woodpecker/deploy.yml`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/ci-image/Dockerfile` & `sketchingpy-0.1.8/ci-image/Dockerfile`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/__init__.py` & `sketchingpy-0.1.8/sketchingpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/abstracted.py` & `sketchingpy-0.1.8/sketchingpy/abstracted.py`

 * *Files 2% similar despite different names*

```diff
@@ -843,7 +843,26 @@
         List of form [min_x, min_y, max_x, max_y].
     """
     x_coords = [x1, x2]
     y_coords = [y1, y2]
     x_coords.sort()
     y_coords.sort()
     return [x_coords[0], y_coords[0], x_coords[1], y_coords[1]]
+
+
+def get_font_name(font, sep_char: str) -> str:
+    """Get the web version of a font.
+
+    Args:
+        font: The font to convert to a web font identifier.
+        sep_char: Path separator char.
+
+    Returns:
+        Web font identifier.
+    """
+    identifier = font.get_identifier()
+    identifier = identifier.split(sep_char)[-1]
+
+    if identifier.endswith('.ttf') or identifier.endswith('.otf'):
+        identifier = identifier[:-4]
+
+    return '%dpx %s' % (int(font.get_size()), identifier)
```

### Comparing `sketchingpy-0.1.7/sketchingpy/bezier_util.py` & `sketchingpy-0.1.8/sketchingpy/bezier_util.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/const.py` & `sketchingpy-0.1.8/sketchingpy/const.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/control_struct.py` & `sketchingpy-0.1.8/sketchingpy/control_struct.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/data_struct.py` & `sketchingpy-0.1.8/sketchingpy/data_struct.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/dialog_struct.py` & `sketchingpy-0.1.8/sketchingpy/dialog_struct.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/geo.py` & `sketchingpy-0.1.8/sketchingpy/geo.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/local_data_struct.py` & `sketchingpy-0.1.8/sketchingpy/local_data_struct.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/pillow_struct.py` & `sketchingpy-0.1.8/sketchingpy/pillow_struct.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/pillow_util.py` & `sketchingpy-0.1.8/sketchingpy/pillow_util.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/pygame_prompt.py` & `sketchingpy-0.1.8/sketchingpy/pygame_prompt.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/shape_struct.py` & `sketchingpy-0.1.8/sketchingpy/shape_struct.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/sketch2d_keymap.py` & `sketchingpy-0.1.8/sketchingpy/sketch2d_keymap.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/sketch2dapp.py` & `sketchingpy-0.1.8/sketchingpy/sketch2dapp.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/sketch2dstatic.py` & `sketchingpy-0.1.8/sketchingpy/sketch2dstatic.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/sketch2dweb.py` & `sketchingpy-0.1.8/sketchingpy/sketch2dweb.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 License:
     BSD
 """
 
 import csv
 import io
 import json
+import os.path
 import time
 import typing
 import urllib.parse
 
 has_js = False
 try:
     import js  # type: ignore
@@ -660,23 +661,15 @@
         super().set_text_align(text_align)
         self._text_align_native = self._transform_text_align(super().get_text_align_native())
 
     def get_text_align_native(self):
         return self._text_align_native
 
     def get_text_font_native(self):
-        font = self.get_text_font()
-
-        identifier = font.get_identifier()
-        identifier = identifier.split('/')[-1]
-
-        if identifier.endswith('.ttf'):
-            identifier = identifier[:-4]
-
-        return '%dpx %s' % (int(font.get_size()), identifier)
+        return sketchingpy.abstracted.get_font_name(self.get_text_font(), os.path.sep)
 
     def _transform_text_align(self,
         text_align: sketchingpy.state_struct.TextAlign) -> sketchingpy.state_struct.TextAlign:
 
         HORIZONTAL_ALIGNS = {
             sketchingpy.const.LEFT: 'left',
             sketchingpy.const.CENTER: 'center',
```

### Comparing `sketchingpy-0.1.7/sketchingpy/state_struct.py` & `sketchingpy-0.1.8/sketchingpy/state_struct.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/transform.py` & `sketchingpy-0.1.8/sketchingpy/transform.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/test/IBMPlexMono-Regular.ttf` & `sketchingpy-0.1.8/sketchingpy/test/IBMPlexMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/test/test_bezier_util.py` & `sketchingpy-0.1.8/sketchingpy/test/test_bezier_util.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/test/test_geo.py` & `sketchingpy-0.1.8/sketchingpy/test/test_geo.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/test/test_local_data_struct.py` & `sketchingpy-0.1.8/sketchingpy/test/test_local_data_struct.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/test/test_pillow_struct.py` & `sketchingpy-0.1.8/sketchingpy/test/test_pillow_struct.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/test/test_pillow_util.py` & `sketchingpy-0.1.8/sketchingpy/test/test_pillow_util.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/test/test_shape_struct.py` & `sketchingpy-0.1.8/sketchingpy/test/test_shape_struct.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/test/test_sketch2d_keymap.py` & `sketchingpy-0.1.8/sketchingpy/test/test_sketch2d_keymap.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/test/test_state_struct.py` & `sketchingpy-0.1.8/sketchingpy/test/test_state_struct.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/sketchingpy/test/test_transform.py` & `sketchingpy-0.1.8/sketchingpy/test/test_transform.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/support/check_website.sh` & `sketchingpy-0.1.8/support/check_website.sh`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/support/render_example_test.py` & `sketchingpy-0.1.8/support/render_example_test.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/support/render_website.py` & `sketchingpy-0.1.8/support/render_website.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/support/render_website.sh` & `sketchingpy-0.1.8/support/render_website.sh`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/support/run_all_local.sh` & `sketchingpy-0.1.8/support/run_all_local.sh`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/support/run_all_static.sh` & `sketchingpy-0.1.8/support/run_all_static.sh`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/support/run_all_web.sh` & `sketchingpy-0.1.8/support/run_all_web.sh`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/support/update_version.py` & `sketchingpy-0.1.8/support/update_version.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/web_test_harness/example.html` & `sketchingpy-0.1.8/web_test_harness/example.html`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         <meta name="viewport" content="width=device-width, initial-scale=1">
         <link rel="stylesheet" href="/third_party/core.css">
         <script type="module" src="/third_party/core.js"></script>
     </head>
     <body>
         <py-config>
         {
-            "packages": ["/dist/sketchingpy-0.1.7-py3-none-any.whl"]
+            "packages": ["/dist/sketchingpy-0.1.8-py3-none-any.whl"]
         }
         </py-config>
 
         <main id="#main">
             <div class="sketch-load-message" id="sketch-load-message">Waiting...</div>
             <canvas id="sketch-canvas" style="display: none"></canvas>
         </main>
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
-{ "packages": ["/dist/sketchingpy-0.1.7-py3-none-any.whl"] }
+{ "packages": ["/dist/sketchingpy-0.1.8-py3-none-any.whl"] }
 Waiting...
 import sketchingpy sketch = sketchingpy.Sketch2D(500, 500) sketch.clear
 ('#505050') sketch.set_stroke_weight(3) sketch.set_fill('#B2DF8A50')
 sketch.set_stroke('#F0F0F0') sketch.draw_ellipse(150, 250, 20, 20)
 sketch.push_style() sketch.clear_fill() sketch.draw_ellipse(250, 250, 20, 20)
 sketch.pop_style() sketch.draw_ellipse(350, 250, 20, 20) sketch.show()
```

### Comparing `sketchingpy-0.1.7/web_test_harness/run_harness.py` & `sketchingpy-0.1.8/web_test_harness/run_harness.py`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/web_test_harness/template.html` & `sketchingpy-0.1.8/web_test_harness/template.html`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         <meta name="viewport" content="width=device-width, initial-scale=1">
         <link rel="stylesheet" href="/third_party/core.css">
         <script type="module" src="/third_party/core.js"></script>
     </head>
     <body>
         <py-config>
         {
-            "packages": ["/dist/sketchingpy-0.1.7-py3-none-any.whl"]
+            "packages": ["/dist/sketchingpy-0.1.8-py3-none-any.whl"]
         }
         </py-config>
 
         <main id="#main">
             <div class="sketch-load-message" id="sketch-load-message">Waiting...</div>
             <canvas id="sketch-canvas" style="display: none"></canvas>
         </main>
```

#### html2text {}

```diff
@@ -1,3 +1,3 @@
-{ "packages": ["/dist/sketchingpy-0.1.7-py3-none-any.whl"] }
+{ "packages": ["/dist/sketchingpy-0.1.8-py3-none-any.whl"] }
 Waiting...
 {{ script }}
```

### Comparing `sketchingpy-0.1.7/website_src/base.html` & `sketchingpy-0.1.8/website_src/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
         {% block style %}{% endblock %}
     </head>
     <body>
         {% if enable_pyscript %}
         <py-config>
         {
-            "packages": ["/dist/sketchingpy-0.1.7-py3-none-any.whl"]
+            "packages": ["/dist/sketchingpy-0.1.8-py3-none-any.whl"]
         }
         </py-config>
         {% endif %}
-        <div class="in-dev-message">🧪 Version 0.1.7 is our alpha release candidate. Please <a href="/community/issue.html">send us bug reports and suggestions</a>!</div>
+        <div class="in-dev-message">🧪 Version 0.1.8 is our alpha release candidate. Please <a href="/community/issue.html">send us bug reports and suggestions</a>!</div>
         <header>
             <a href="#main" class="skip-link">Skip to content</a>
             <h1>Sketchingpy</h1>
             <div class="subtitle">Creative coding and interactive science everywhere for everyone: <a href="/guides/start.html#web">web</a>, <a href="/guides/start.html#local">desktop</a>, <a href="/guides/start.html#mobile">mobile</a>, <a href="/guides/start.html#notebook">Jupyter</a>, and <a href="/guides/start.html#static">more</a>. <a href="https://codeberg.org/sketchingpy/Sketchingpy">Open source</a>!</div>
         </header>
         <nav>
             {% for section in sections %}
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% if enable_pyscript %}
 {% endif %} {% block metatags %}{% endblock %} {% block style %}{% endblock %}
-{% if enable_pyscript %} { "packages": ["/dist/sketchingpy-0.1.7-py3-none-
+{% if enable_pyscript %} { "packages": ["/dist/sketchingpy-0.1.8-py3-none-
 any.whl"] } {% endif %}
-🧪 Version 0.1.7 is our alpha release candidate. Please _s_e_n_d_ _u_s_ _b_u_g_ _r_e_p_o_r_t_s_ _a_n_d
+🧪 Version 0.1.8 is our alpha release candidate. Please _s_e_n_d_ _u_s_ _b_u_g_ _r_e_p_o_r_t_s_ _a_n_d
 _s_u_g_g_e_s_t_i_o_n_s!
 _S_k_i_p_ _t_o_ _c_o_n_t_e_n_t
 ************ SSkkeettcchhiinnggppyy ************
 Creative coding and interactive science everywhere for everyone: _w_e_b, _d_e_s_k_t_o_p,
 _m_o_b_i_l_e, _J_u_p_y_t_e_r, and _m_o_r_e. _O_p_e_n_ _s_o_u_r_c_e!
 {% for section in sections %}
 % if current_section == section['section'] %}class="selected" aria-
```

### Comparing `sketchingpy-0.1.7/website_src/community.html` & `sketchingpy-0.1.8/website_src/community.html`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/guides.html` & `sketchingpy-0.1.8/website_src/guides.html`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/index.html` & `sketchingpy-0.1.8/website_src/index.html`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/pages.yml` & `sketchingpy-0.1.8/website_src/pages.yml`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/privacy.html` & `sketchingpy-0.1.8/website_src/privacy.html`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/reference.html` & `sketchingpy-0.1.8/website_src/reference.html`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/reference.yml` & `sketchingpy-0.1.8/website_src/reference.yml`

 * *Files 0% similar despite different names*

```diff
@@ -2806,15 +2806,15 @@
           caption: >
             Draw "Hello World" in 12 point IBM Plex Mono at x coordinate 50 and y coordinate 100.
           code: >
             sketch.set_text_font('./IBMPlexMono-Regular.ttf', 12)\n
             sketch.draw_text(50, 100, 'Hello World')
         arguments:
           - name: "font"
-            description: Path to the TTF font file.
+            description: Path to the TTF or OTF font file. For web renderer, name of web font can be used.
           - name: "size"
             description: Size of the font (px).
         examples:
           - text_fill_stroke
           - text_horiz_align
           - text_vert_align
         availability: >
```

### Comparing `sketchingpy-0.1.7/website_src/reference_page.html` & `sketchingpy-0.1.8/website_src/reference_page.html`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             <section class="reference-item subsection">
                 <h3>Purpose</h3>
                 <div>{{ reference_item['long'] | safe }}</div>
             </section>
 
             {% if 'snippet' in reference_item %}
             <section class="reference-item subsection">
-                <h3>Example</h3>
+                <h3>Snippet</h3>
                 <div>{{ reference_item['snippet']['caption'] }}</div>
                 <pre>{{ snippet_code }}</pre>
             </section>
             {% endif %}
 
             {% if 'arguments' in reference_item %}
             <section class="reference-item subsection">
@@ -47,33 +47,33 @@
                         {{ arg['description'] }}
                     </li>
                     {% endfor %}
                 </ul>
             </section>
             {% endif %}
 
-            <section class="reference-item subsection">
-                <h3>Availability</h3>
-                <div>{{ reference_item['availability'] }}</div>
-            </section>
-
             {% if 'examples' in reference_item %}
             <section class="reference-item subsection">
-                <h3>Other examples</h3>
+                <h3>Examples</h3>
                 <ul>
                     {% for example in reference_item['examples'] %}
                     <li><a href="/examples/web/example.html?sketch={{ example }}">{{ example }}</a></li>
                     {% endfor %}
                 </ul>
             </section>
             {% endif %}
 
+            <section class="reference-item subsection">
+                <h3>Availability</h3>
+                <div>{{ reference_item['availability'] }}</div>
+            </section>
+
             {% if 'also' in reference_item %}
             <section class="reference-item subsection">
-                <h3>See also in reference</h3>
+                <h3>See also</h3>
                 <ul>
                     {% for other in reference_item['also'] %}
                     <li><a href="/reference/{{ other }}.html">{{ other }}</a></li>
                     {% endfor %}
                 </ul>
             </section>
             {% endif %}
```

#### html2text {}

```diff
@@ -6,29 +6,29 @@
 {% for item in section['items'] %}
 {% if item['name'] == reference_item['name'] %} {{ item['name'] }} {% else %} _{
 _{_ _i_t_e_m_[_'_n_a_m_e_'_]_ _}_} {% endif %}
 {% endfor %} {% endfor %}
 ******** PPuurrppoossee ********
 {{ reference_item['long'] | safe }}
 {% if 'snippet' in reference_item %}
-******** EExxaammppllee ********
+******** SSnniippppeett ********
 {{ reference_item['snippet']['caption'] }}
 {{ snippet_code }}
 {% endif %} {% if 'arguments' in reference_item %}
 ******** AArrgguummeennttss ********
     * {% for arg in reference_item['arguments'] %}
     * {{ arg['name'] }}: {{ arg['description'] }}
     * {% endfor %}
-{% endif %}
-******** AAvvaaiillaabbiilliittyy ********
-{{ reference_item['availability'] }}
-{% if 'examples' in reference_item %}
-******** OOtthheerr eexxaammpplleess ********
+{% endif %} {% if 'examples' in reference_item %}
+******** EExxaammpplleess ********
     * {% for example in reference_item['examples'] %}
     * _{_{_ _e_x_a_m_p_l_e_ _}_}
     * {% endfor %}
-{% endif %} {% if 'also' in reference_item %}
-******** SSeeee aallssoo iinn rreeffeerreennccee ********
+{% endif %}
+******** AAvvaaiillaabbiilliittyy ********
+{{ reference_item['availability'] }}
+{% if 'also' in reference_item %}
+******** SSeeee aallssoo ********
     * {% for other in reference_item['also'] %}
     * _{_{_ _o_t_h_e_r_ _}_}
     * {% endfor %}
 {% endif %} {% endblock %}
```

### Comparing `sketchingpy-0.1.7/website_src/community/code.html` & `sketchingpy-0.1.8/website_src/community/code.html`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/community/conventions.html` & `sketchingpy-0.1.8/website_src/community/conventions.html`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/community/discord.html` & `sketchingpy-0.1.8/website_src/community/discord.html`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/community/document.html` & `sketchingpy-0.1.8/website_src/community/document.html`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/community/issue.html` & `sketchingpy-0.1.8/website_src/community/issue.html`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/community/showcase.html` & `sketchingpy-0.1.8/website_src/community/showcase.html`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/css/base.css` & `sketchingpy-0.1.8/website_src/css/base.css`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     padding-bottom: 25px;
 }
 
 .gallery {
     padding-top: 40px;
 }
 
-.gallery a:link, .gallery a:visited, .gallery a:hover, .gallery a:active {
+.gallery a.button:link, .gallery a.button:visited, .gallery a.button:hover, .gallery a.button:active {
     -webkit-appearance: none;
     background: none;
     border: none;
     outline: none;
     box-shadow: none;
     background-color: #FFFFFF;
     color: #6161CC;
@@ -146,15 +146,15 @@
     margin-top: 5px;
     border-radius: 5px;
     border: 1px solid #6161CC;
     padding: 5px 10px;
     text-decoration: none;
 }
 
-.gallery a:hover, .gallery a:active {
+.gallery a.button:hover, .gallery a.button:active {
     cursor: pointer;
     background-color: #5050D0;
     color: white;
 }
 
 .gallery .item {
     margin: 10px;
```

### Comparing `sketchingpy-0.1.7/website_src/css/editor.css` & `sketchingpy-0.1.8/website_src/css/editor.css`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/css/index.css` & `sketchingpy-0.1.8/website_src/css/index.css`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/guides/deploy.html` & `sketchingpy-0.1.8/website_src/guides/deploy.html`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         &lt;!-- PyScript --&gt;
         &lt;link rel=&quot;stylesheet&quot; href=&quot;https://pyscript.net/releases/2023.11.2/core.css&quot;&gt;
         &lt;script type=&quot;module&quot; src=&quot;https://pyscript.net/releases/2023.11.2/core.js&quot;&gt;&lt;/script&gt;
     &lt;/head&gt;
     &lt;body&gt;
         &lt;py-config&gt;
         {
-            &quot;packages&quot;: [&quot;sketchingpy==0.1.7&quot;]
+            &quot;packages&quot;: [&quot;sketchingpy==0.1.8&quot;]
         }
         &lt;/py-config&gt;
 
         &lt;!-- You may need to change this ID to match your code. --&gt;
         &lt;div id=&quot;sketch-load-message&quot;&gt;Loading...&lt;/div&gt;
         &lt;canvas id=&quot;sketch-canvas&quot;&gt;&lt;/canvas&gt;
```

#### html2text {}

```diff
@@ -46,15 +46,15 @@
 core.css">
         <script type="module" src="https://pyscript.net/releases/2023.11.2/
 core.js"></script>
     </head>
     <body>
         <py-config>
         {
-            "packages": ["sketchingpy==0.1.7"]
+            "packages": ["sketchingpy==0.1.8"]
         }
         </py-config>
 
         <!-- You may need to change this ID to match your code. -->
         <div id="sketch-load-message">Loading...</div>
         <canvas id="sketch-canvas"></canvas>
```

### Comparing `sketchingpy-0.1.7/website_src/guides/start.html` & `sketchingpy-0.1.8/website_src/guides/start.html`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/guides/web_detailed.html` & `sketchingpy-0.1.8/website_src/guides/web_detailed.html`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     <section class="subsection" id="altid">
         <h3>Multiple Python Files</h3>
         <div>
             The py-config element can add additional resources to the environment of your scripts including adding other Python files which can be imported.
 <pre>
 &lt;py-config&gt;
 {
-    &quot;packages&quot;: [&quot;sketchingpy==0.1.7&quot;],
+    &quot;packages&quot;: [&quot;sketchingpy==0.1.8&quot;],
     &quot;files&quot;: {
         &quot;/a.py&quot;: &quot;a.py&quot;,
         &quot;/b.py&quot;: &quot;b.py&quot;
     }
 }
 &lt;/py-config&gt;
 
@@ -104,15 +104,15 @@
         &lt;!-- You may need to change these paths to pyscript files. --&gt;
         &lt;link rel=&quot;stylesheet&quot; href=&quot;/third_party/core.css&quot;&gt;
         &lt;script type=&quot;module&quot; src=&quot;/third_party/core.js&quot;&gt;&lt;/script&gt;
     &lt;/head&gt;
     &lt;body&gt;
         &lt;py-config&gt;
         {
-            &quot;packages&quot;: [&quot;/third_party/sketchingpy-0.1.7-py3-none-any.whl&quot;]
+            &quot;packages&quot;: [&quot;/third_party/sketchingpy-0.1.8-py3-none-any.whl&quot;]
         }
         &lt;/py-config&gt;
 
         &lt;!-- You may need to change this ID to match your code. --&gt;
         &lt;div id=&quot;sketch-load-message&quot;&gt;Loading...&lt;/div&gt;
         &lt;canvas id=&quot;sketch-canvas&quot;&gt;&lt;/canvas&gt;
```

#### html2text {}

```diff
@@ -31,15 +31,15 @@
 Note that this examples uses the canvas_id and loading_id variables but the
 strings can be passed direclty if preferred.
 ******** MMuullttiippllee PPyytthhoonn FFiilleess ********
 The py-config element can add additional resources to the environment of your
 scripts including adding other Python files which can be imported.
 <py-config>
 {
-    "packages": ["sketchingpy==0.1.7"],
+    "packages": ["sketchingpy==0.1.8"],
     "files": {
         "/a.py": "a.py",
         "/b.py": "b.py"
     }
 }
 </py-config>
 
@@ -68,15 +68,15 @@
         <!-- You may need to change these paths to pyscript files. -->
         <link rel="stylesheet" href="/third_party/core.css">
         <script type="module" src="/third_party/core.js"></script>
     </head>
     <body>
         <py-config>
         {
-            "packages": ["/third_party/sketchingpy-0.1.7-py3-none-any.whl"]
+            "packages": ["/third_party/sketchingpy-0.1.8-py3-none-any.whl"]
         }
         </py-config>
 
         <!-- You may need to change this ID to match your code. -->
         <div id="sketch-load-message">Loading...</div>
         <canvas id="sketch-canvas"></canvas>
```

### Comparing `sketchingpy-0.1.7/website_src/guides/why.html` & `sketchingpy-0.1.8/website_src/guides/why.html`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/code.png` & `sketchingpy-0.1.8/website_src/img/code.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/conventions.png` & `sketchingpy-0.1.8/website_src/img/conventions.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/data_write_csv.png` & `sketchingpy-0.1.8/website_src/img/data_write_csv.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/data_write_json.png` & `sketchingpy-0.1.8/website_src/img/data_write_json.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/deploy.png` & `sketchingpy-0.1.8/website_src/img/deploy.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/dialog_simple.png` & `sketchingpy-0.1.8/website_src/img/dialog_simple.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/discord.png` & `sketchingpy-0.1.8/website_src/img/discord.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/document.png` & `sketchingpy-0.1.8/website_src/img/document.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/hello_interactive.png` & `sketchingpy-0.1.8/website_src/img/hello_interactive.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/home_screen.png` & `sketchingpy-0.1.8/website_src/img/home_screen.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/inputs_keyboard.png` & `sketchingpy-0.1.8/website_src/img/inputs_keyboard.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/inputs_mouse.png` & `sketchingpy-0.1.8/website_src/img/inputs_mouse.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/issue.png` & `sketchingpy-0.1.8/website_src/img/issue.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/start.png` & `sketchingpy-0.1.8/website_src/img/start.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/web_detailed.png` & `sketchingpy-0.1.8/website_src/img/web_detailed.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/img/why.png` & `sketchingpy-0.1.8/website_src/img/why.png`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/js/editor.js` & `sketchingpy-0.1.8/website_src/js/editor.js`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/js/index.js` & `sketchingpy-0.1.8/website_src/js/index.js`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party/README.md` & `sketchingpy-0.1.8/website_src/third_party/README.md`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party/core.js` & `sketchingpy-0.1.8/website_src/third_party/core.js`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party/error-96hMSEw8.js` & `sketchingpy-0.1.8/website_src/third_party/error-96hMSEw8.js`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party/es.js` & `sketchingpy-0.1.8/website_src/third_party/es.js`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party/py-terminal-XWbSa71s.js` & `sketchingpy-0.1.8/website_src/third_party/py-terminal-XWbSa71s.js`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party/pyodide-lock.json` & `sketchingpy-0.1.8/website_src/third_party/pyodide-lock.json`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party/pyodide.asm.js` & `sketchingpy-0.1.8/website_src/third_party/pyodide.asm.js`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party/pyodide.asm.wasm` & `sketchingpy-0.1.8/website_src/third_party/pyodide.asm.wasm`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party/pyodide.mjs` & `sketchingpy-0.1.8/website_src/third_party/pyodide.mjs`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party/python_stdlib.zip` & `sketchingpy-0.1.8/website_src/third_party/python_stdlib.zip`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party/toml--Dzglv4T.js` & `sketchingpy-0.1.8/website_src/third_party/toml--Dzglv4T.js`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party_site/IBMPlexMono-Regular.ttf` & `sketchingpy-0.1.8/website_src/third_party_site/IBMPlexMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party_site/IBMPlexSans-Regular.ttf` & `sketchingpy-0.1.8/website_src/third_party_site/IBMPlexSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party_site/README.md` & `sketchingpy-0.1.8/website_src/third_party_site/README.md`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party_site/ace.min.js` & `sketchingpy-0.1.8/website_src/third_party_site/ace.min.js`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/website_src/third_party_site/mode-python.js` & `sketchingpy-0.1.8/website_src/third_party_site/mode-python.js`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/.gitignore` & `sketchingpy-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/LICENSE.md` & `sketchingpy-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/README.md` & `sketchingpy-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `sketchingpy-0.1.7/pyproject.toml` & `sketchingpy-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sketchingpy"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="A Samuel Pottinger", email="hello@sketchingpy.org" }
 ]
 description = "Tools for quick creative programmig."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sketchingpy-0.1.7/PKG-INFO` & `sketchingpy-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sketchingpy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Tools for quick creative programmig.
 Project-URL: Homepage, https://sketchingpy.org
 Project-URL: Documentation, https://sketchingpy.org/reference
 Project-URL: Source, https://codeberg.org/sketchingpy/Sketchingpy
 Project-URL: Issue Tracker, https://codeberg.org/sketchingpy/Sketchingpy/issues
 Project-URL: Changelog, https://codeberg.org/sketchingpy/Sketchingpy/commits/branch/main
 Author-email: A Samuel Pottinger <hello@sketchingpy.org>
```

