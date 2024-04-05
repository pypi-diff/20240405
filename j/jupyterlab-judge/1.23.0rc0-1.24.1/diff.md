# Comparing `tmp/jupyterlab_judge-1.23.0rc0.tar.gz` & `tmp/jupyterlab_judge-1.24.1.tar.gz`

## Comparing `jupyterlab_judge-1.23.0rc0.tar` & `jupyterlab_judge-1.24.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/.copier-answers.yml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/.yarnrc.yml
--rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/CHANGELOG.md
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/babel.config.js
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/conftest.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jest.config.js
--rw-r--r--   0        0        0     8106 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/setup.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/tsconfig.test.json
--rw-r--r--   0        0        0   435917 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/yarn.lock
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyter-config/nb-config/jupyterlab_judge.json
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyter-config/server-config/jupyterlab_judge.json
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/_version.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/handlers.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/yjudge.py
--rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/package.json
--rw-r--r--   0        0        0     8106 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/schemas/jupyterlab-judge/plugin.json
--rw-r--r--   0        0        0    14975 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js.LICENSE.txt
--rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js
--rw-r--r--   0        0        0     6939 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js
--rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/747.13907913bad1ebbd3546.js
--rw-r--r--   0        0        0    54375 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js
--rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js
--rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js
--rw-r--r--   0        0        0  4279528 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js.LICENSE.txt
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js
--rw-r--r--   0        0        0    32819 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/960.30572a65d088e05e87a5.js
--rw-r--r--   0        0        0    10423 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/remoteEntry.5c8a6aaf9a330f5d95c4.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/style.js
--rw-r--r--   0        0        0    38387 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json
--rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/tests/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/jupyterlab_judge/tests/test_handlers.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/schema/plugin.json
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/commands.ts
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/constants.ts
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/handler.ts
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/index.ts
--rw-r--r--   0        0        0    16041 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/model.ts
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/tokens.ts
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/toolbar.tsx
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/__tests__/jupyterlab_judge.spec.ts
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/components/SubmissionArea.tsx
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/components/SubmissionControl.tsx
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/components/SubmissionItem.tsx
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/components/SubmissionItemStatus.tsx
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/components/SubmissionItemWait.tsx
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/components/SubmissionItemWaitStatus.tsx
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/components/SubmissionList.tsx
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/components/index.ts
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/problemProvider/HardCodedProblemProvider.ts
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/problemProvider/index.ts
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/problemProvider/problemProvider.ts
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/widgets/JudgeOutputArea.ts
--rw-r--r--   0        0        0    21448 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/widgets/JudgePanel.ts
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/widgets/JudgeProblemPanel.ts
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/widgets/JudgeSubmissionArea.tsx
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/widgets/JudgeTerminal.ts
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/src/widgets/index.ts
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/style/index.js
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/style/judgeOutputArea.css
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/style/judgePanel.css
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/style/judgeTerminal.css
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/ui-tests/yarn.lock
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/ui-tests/tests/jupyterlab_judge.spec.ts
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/.gitignore
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/LICENSE
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/README.md
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/pyproject.toml
--rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 jupyterlab_judge-1.23.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/.copier-answers.yml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/.yarnrc.yml
+-rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/babel.config.js
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/conftest.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jest.config.js
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/setup.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/tsconfig.test.json
+-rw-r--r--   0        0        0   435917 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/yarn.lock
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyter-config/nb-config/jupyterlab_judge.json
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyter-config/server-config/jupyterlab_judge.json
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/_version.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/handlers.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/yjudge.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/package.json
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/schemas/jupyterlab-judge/plugin.json
+-rw-r--r--   0        0        0    14975 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js.LICENSE.txt
+-rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js
+-rw-r--r--   0        0        0     6939 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/747.2841a40cba671c554a8c.js
+-rw-r--r--   0        0        0    54375 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js
+-rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js
+-rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js
+-rw-r--r--   0        0        0  4279528 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js.LICENSE.txt
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js
+-rw-r--r--   0        0        0    33276 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/960.248f24628be1ecbf1885.js
+-rw-r--r--   0        0        0    10420 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/remoteEntry.5b4a6b2fd107c17f4d34.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/style.js
+-rw-r--r--   0        0        0    38387 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json
+-rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/tests/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/jupyterlab_judge/tests/test_handlers.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/schema/plugin.json
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/commands.ts
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/constants.ts
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/handler.ts
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/index.ts
+-rw-r--r--   0        0        0    16041 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/model.ts
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/tokens.ts
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/toolbar.tsx
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/__tests__/jupyterlab_judge.spec.ts
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/SubmissionArea.tsx
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/SubmissionControl.tsx
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/SubmissionItem.tsx
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/SubmissionItemStatus.tsx
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/SubmissionItemWait.tsx
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/SubmissionItemWaitStatus.tsx
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/SubmissionList.tsx
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/components/index.ts
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/problemProvider/HardCodedProblemProvider.ts
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/problemProvider/index.ts
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/problemProvider/problemProvider.ts
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/widgets/JudgeOutputArea.ts
+-rw-r--r--   0        0        0    22446 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/widgets/JudgePanel.ts
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/widgets/JudgeProblemPanel.ts
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/widgets/JudgeSubmissionArea.tsx
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/widgets/JudgeTerminal.ts
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/src/widgets/index.ts
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/style/index.js
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/style/judgeOutputArea.css
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/style/judgePanel.css
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/style/judgeTerminal.css
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/ui-tests/tests/jupyterlab_judge.spec.ts
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/LICENSE
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/README.md
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/pyproject.toml
+-rw-r--r--   0        0        0     9296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.1/PKG-INFO
```

### Comparing `jupyterlab_judge-1.23.0rc0/.copier-answers.yml` & `jupyterlab_judge-1.24.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/CHANGELOG.md` & `jupyterlab_judge-1.24.1/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,56 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.24.1
+
+No merged PRs
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
+## 1.24.0
+
+([Full Changelog](https://github.com/team-monolith-product/jupyterlab-judge/compare/v1.23.0...79c3c0c4960119fb18d7d5af68ab1734edb4d1d6))
+
+### Merged PRs
+
+- Implement robust input mechanism [#55](https://github.com/team-monolith-product/jupyterlab-judge/pull/55) ([@a3626a](https://github.com/a3626a))
+- fix: height 100% 추가 [#46](https://github.com/team-monolith-product/jupyterlab-judge/pull/46) ([@a3626a](https://github.com/a3626a))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/team-monolith-product/jupyterlab-judge/graphs/contributors?from=2024-01-29&to=2024-04-05&type=c))
+
+[@a3626a](https://github.com/search?q=repo%3Ateam-monolith-product%2Fjupyterlab-judge+involves%3Aa3626a+updated%3A2024-01-29..2024-04-05&type=Issues)
+
+## 1.23.0
+
+([Full Changelog](https://github.com/team-monolith-product/jupyterlab-judge/compare/v1.23.0rc0...e2e16a5d26c010a51241cbada5cbc23a5030bfa2))
+
+### Merged PRs
+
+- fix collaborative logic [#50](https://github.com/team-monolith-product/jupyterlab-judge/pull/50) ([@paulkim3151](https://github.com/paulkim3151))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/team-monolith-product/jupyterlab-judge/graphs/contributors?from=2024-01-29&to=2024-01-29&type=c))
+
+[@paulkim3151](https://github.com/search?q=repo%3Ateam-monolith-product%2Fjupyterlab-judge+involves%3Apaulkim3151+updated%3A2024-01-29..2024-01-29&type=Issues) | [@sweep-ai](https://github.com/search?q=repo%3Ateam-monolith-product%2Fjupyterlab-judge+involves%3Asweep-ai+updated%3A2024-01-29..2024-01-29&type=Issues)
+
 ## 1.23.0rc0
 
 ([Full Changelog](https://github.com/team-monolith-product/jupyterlab-judge/compare/v1.22.0))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/team-monolith-product/jupyterlab-judge/graphs/contributors?from=2024-01-29&to=2024-01-29&type=c))
 
 [@sweep-ai](https://github.com/search?q=repo%3Ateam-monolith-product%2Fjupyterlab-judge+involves%3Asweep-ai+updated%3A2024-01-29..2024-01-29&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.22.0
 
 ([Full Changelog](https://github.com/team-monolith-product/jupyterlab-judge/compare/v1.21.0...ecaba1ccf106d138c3df7864fc9be9d1e81d9f81))
 
 ### Merged PRs
 
 - Add panel arg to submit [#47](https://github.com/team-monolith-product/jupyterlab-judge/pull/47) ([@a3626a](https://github.com/a3626a))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jupyterlab_judge-1.23.0rc0/RELEASE.md` & `jupyterlab_judge-1.24.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jest.config.js` & `jupyterlab_judge-1.24.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/package.json` & `jupyterlab_judge-1.24.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'1.24.1'"}*

```diff
@@ -231,9 +231,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.23.0-rc0"
+    "version": "1.24.1"
 }
```

### Comparing `jupyterlab_judge-1.23.0rc0/tsconfig.json` & `jupyterlab_judge-1.24.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/yarn.lock` & `jupyterlab_judge-1.24.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/__init__.py` & `jupyterlab_judge-1.24.1/jupyterlab_judge/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/handlers.py` & `jupyterlab_judge-1.24.1/jupyterlab_judge/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/yjudge.py` & `jupyterlab_judge-1.24.1/jupyterlab_judge/yjudge.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/package.json` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9796666666666667%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.5b4a6b2fd107c17f4d34.js'}}",*

 * * "'version'": "'1.24.1'"}*

```diff
@@ -135,15 +135,15 @@
         "schema/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/team-monolith-product/jupyterlab-judge",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.5c8a6aaf9a330f5d95c4.js",
+            "load": "static/remoteEntry.5b4a6b2fd107c17f4d34.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_judge"
                 },
@@ -236,9 +236,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.23.0-rc0"
+    "version": "1.24.1"
 }
```

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'1.24.1'"}*

```diff
@@ -231,9 +231,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.23.0-rc0"
+    "version": "1.24.1"
 }
```

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/747.13907913bad1ebbd3546.js` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/747.2841a40cba671c554a8c.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -31,15 +31,15 @@
             t.d(e, {
                 Z: () => p
             });
             var r = t(8081),
                 o = t.n(r),
                 a = t(3645),
                 i = t.n(a)()(o());
-            i.push([n.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n\n.jp-JudgePanel-problem {\n  padding: 20px;\n  box-shadow: none;\n  border-top: 0 none;\n  border-bottom: 0 none;\n  border-left: 0 none;\n  border-right: 1px solid var(--jp-border-color0);\n  min-width: 200px;\n  overflow-y: auto;\n}\n\n/*\nmin-width has no effect on the right panel, so we need to set it on the children.\n.jp-JudgePanel-rightPanel {\n  min-width: 500px;\n}\n*/\n\n.jp-JudgePanel-rightPanel .CodeMirror-gutters {\n  border-right: 1px solid var(--jp-border-color0);\n}\n\n.jp-JudgePanel-editor {\n  min-height: 100px;\n  min-width: 500px;\n}\n\n.jp-JudgePanel-terminal {\n  min-height: 100px;\n  min-width: 500px;\n}\n\n.jp-JudgePanel-submissionPanel {\n  min-height: 100px;\n  min-width: 500px;\n}\n\n.jp-JudgePanel-editor .cm-editor {\n  height: 100%;\n}\n", ""]);
+            i.push([n.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n\n.jp-JudgePanel-problem {\n  padding: 20px;\n  box-shadow: none;\n  border-top: 0 none;\n  border-bottom: 0 none;\n  border-left: 0 none;\n  border-right: 1px solid var(--jp-border-color0);\n  min-width: 200px;\n  height: 100%;\n  overflow-y: auto;\n}\n\n/*\nmin-width has no effect on the right panel, so we need to set it on the children.\n.jp-JudgePanel-rightPanel {\n  min-width: 500px;\n}\n*/\n\n.jp-JudgePanel-rightPanel .CodeMirror-gutters {\n  border-right: 1px solid var(--jp-border-color0);\n}\n\n.jp-JudgePanel-editor {\n  min-height: 100px;\n  min-width: 500px;\n}\n\n.jp-JudgePanel-terminal {\n  min-height: 100px;\n  min-width: 500px;\n}\n\n.jp-JudgePanel-submissionPanel {\n  min-height: 100px;\n  min-width: 500px;\n}\n\n.jp-JudgePanel-editor .cm-editor {\n  height: 100%;\n}\n", ""]);
             const p = i
         },
         1600: (n, e, t) => {
             t.d(e, {
                 Z: () => p
             });
             var r = t(8081),
@@ -95,27 +95,27 @@
                 for (var a = {}, i = [], p = 0; p < n.length; p++) {
                     var l = n[p],
                         u = r.base ? l[0] + r.base : l[0],
                         d = a[u] || 0,
                         s = "".concat(u, " ").concat(d);
                     a[u] = d + 1;
                     var c = t(s),
-                        f = {
+                        h = {
                             css: l[1],
                             media: l[2],
                             sourceMap: l[3],
                             supports: l[4],
                             layer: l[5]
                         };
-                    if (-1 !== c) e[c].references++, e[c].updater(f);
+                    if (-1 !== c) e[c].references++, e[c].updater(h);
                     else {
-                        var h = o(f, r);
+                        var f = o(h, r);
                         r.byIndex = p, e.splice(p, 0, {
                             identifier: s,
-                            updater: h,
+                            updater: f,
                             references: 1
                         })
                     }
                     i.push(s)
                 }
                 return i
             }
@@ -221,15 +221,15 @@
                 i = t.n(a),
                 p = t(569),
                 l = t.n(p),
                 u = t(3565),
                 d = t.n(u),
                 s = t(9216),
                 c = t.n(s),
-                f = t(4589),
-                h = t.n(f),
+                h = t(4589),
+                f = t.n(h),
                 m = t(1150),
                 g = {};
-            g.styleTagTransform = h(), g.setAttributes = d(), g.insert = l().bind(null, "head"), g.domAPI = i(), g.insertStyleElement = c(), o()(m.Z, g), m.Z && m.Z.locals && m.Z.locals
+            g.styleTagTransform = f(), g.setAttributes = d(), g.insert = l().bind(null, "head"), g.domAPI = i(), g.insertStyleElement = c(), o()(m.Z, g), m.Z && m.Z.locals && m.Z.locals
         }
     }
 ]);
```

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/960.30572a65d088e05e87a5.js` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/960.248f24628be1ecbf1885.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,50 +1,50 @@
 "use strict";
 (self.webpackChunkjupyterlab_judge = self.webpackChunkjupyterlab_judge || []).push([
     [960], {
         960: (e, t, s) => {
             s.r(t), s.d(t, {
-                HardCodedProblemProvider: () => U,
-                IJudgePanelFactory: () => $,
+                HardCodedProblemProvider: () => q,
+                IJudgePanelFactory: () => R,
                 IJudgeSignal: () => z,
-                IJudgeSubmissionAreaFactory: () => R,
-                IJudgeTerminalFactory: () => K,
-                IProblemProvider: () => W,
-                ISubmissionListFactory: () => B,
+                IJudgeSubmissionAreaFactory: () => K,
+                IJudgeTerminalFactory: () => B,
+                IProblemProvider: () => $,
+                ISubmissionListFactory: () => U,
                 JudgeDocument: () => E,
-                JudgeDocumentFactory: () => I,
-                JudgeError: () => f,
-                JudgeKernelImplementationError: () => v,
-                JudgeKernelNotConnectedError: () => w,
-                JudgeKernelReconnectingFailedError: () => S,
-                JudgeModel: () => J,
-                JudgeOutputArea: () => je,
-                JudgePanel: () => j,
+                JudgeDocumentFactory: () => k,
+                JudgeError: () => w,
+                JudgeKernelImplementationError: () => S,
+                JudgeKernelNotConnectedError: () => v,
+                JudgeKernelReconnectingFailedError: () => j,
+                JudgeModel: () => M,
+                JudgeOutputArea: () => Ie,
+                JudgePanel: () => I,
                 JudgeProblemPanel: () => C,
-                JudgeSubmissionArea: () => ve,
-                JudgeTerminal: () => Ie,
-                SubmissionArea: () => be,
+                JudgeSubmissionArea: () => Se,
+                JudgeTerminal: () => ke,
+                SubmissionArea: () => ye,
                 SubmissionControl: () => V,
-                SubmissionItem: () => te,
-                SubmissionItemStatus: () => Z,
-                SubmissionItemWait: () => ae,
-                SubmissionListImpl: () => ce,
-                SubmissionListSignalWrapper: () => ue,
-                default: () => Te,
-                factoryContext: () => we,
-                openOrCreateFromId: () => N,
-                transContext: () => fe
+                SubmissionItem: () => se,
+                SubmissionItemStatus: () => ee,
+                SubmissionItemWait: () => de,
+                SubmissionListImpl: () => me,
+                SubmissionListSignalWrapper: () => ce,
+                default: () => Ne,
+                factoryContext: () => ve,
+                openOrCreateFromId: () => A,
+                transContext: () => we
             });
-            var n = s(4111),
-                o = s(5123),
-                i = s(1562),
-                r = s(2038),
-                a = s(678),
-                d = s(8060),
-                l = s(1645),
+            var n = s(8368),
+                o = s(9510),
+                i = s(5962),
+                r = s(3452),
+                a = s(3471),
+                d = s(1638),
+                l = s(1778),
                 u = s(6029),
                 c = s.n(u);
             const m = "jupyterlab-judge",
                 h = ".jce-judge",
                 p = "jupyterlab-judge";
             var g;
             ! function(e) {
@@ -75,55 +75,60 @@
                 e.createSaveButton = t, e.getDefaultItems = function(e, s, n) {
                     return [{
                         name: "save",
                         widget: t(e, s)
                     }]
                 }
             }(g || (g = {}));
-            var _ = s(8778),
+            var _ = s(4882),
                 b = s(5536),
-                y = s(4938);
+                y = s(8048);
             class C extends _.Panel {
                 constructor(e, t) {
                     super(), this._model = e.model, this._trans = e.translator.load(m), this._markdownRenderer = t.createRenderer("text/markdown"), this._markdownRenderer.addClass("jp-JudgePanel-problem"), this.addWidget(this._markdownRenderer)
                 }
                 renderProblem() {
                     var e, t;
                     this._markdownRenderer.renderModel(new y.MimeModel({
                         data: {
                             "text/markdown": null !== (t = null === (e = this._model.problem) || void 0 === e ? void 0 : e.content) && void 0 !== t ? t : this._trans.__("Problem Not Available.")
                         }
                     }))
                 }
             }
+
+            function f(e) {
+                const t = Array.from(e, (e => String.fromCodePoint(e))).join("");
+                return btoa(t)
+            }
             const x = new r.LabIcon({
                 name: "jupyterlab-judge:problem-icon",
                 svgstr: b.customJudgeColorSvg
             });
-            class f extends Error {
+            class w extends Error {
                 constructor(e) {
                     super(e), this.name = this.constructor.name
                 }
             }
-            class w extends f {
+            class v extends w {
                 constructor(e) {
                     super(e), this.name = this.constructor.name
                 }
             }
-            class v extends f {
+            class S extends w {
                 constructor(e) {
                     super(e), this.name = this.constructor.name
                 }
             }
-            class S extends f {
+            class j extends w {
                 constructor(e) {
                     super(e), this.name = this.constructor.name
                 }
             }
-            class j extends _.BoxPanel {
+            class I extends _.BoxPanel {
                 constructor(e) {
                     super(), this.addClass("jp-JudgePanel"), this._context = e.context, this._translator = e.translator, this._sessionContextDialogs = e.sessionContextDialogs, this._trans = this._translator.load(m), this._submitted = e.submitted, this._executed = e.executed, this._rendermime = e.rendermime, this.id = "jce-judge-panel", this.title.closable = !0;
                     const t = new _.SplitPanel({
                         spacing: 0
                     });
                     t.addClass("jp-JudgePanel-splitPanel"), this._editorWidget = new a.CodeEditorWrapper({
                         model: this.model.codeModel,
@@ -252,20 +257,20 @@
                     this.model.submissionStatus = {
                         type: "progress",
                         runCount: 0,
                         totalCount: i.length
                     };
                     for (let e = 0; e < 20 && "idle" !== a.kernelDisplayStatus; e++) await new Promise((e => setTimeout(e, 1e3)));
                     if ("idle" !== a.kernelDisplayStatus) {
-                        if ("connecting" !== a.kernelDisplayStatus) throw console.warn(`Kernel is still ${a.kernelDisplayStatus} after 20s`), new f(this._trans.__("Kernel is not responding. Please try again."));
+                        if ("connecting" !== a.kernelDisplayStatus) throw console.warn(`Kernel is still ${a.kernelDisplayStatus} after 20s`), new w(this._trans.__("Kernel is not responding. Please try again."));
                         {
                             const e = d._reconnectAttempt;
-                            if (void 0 === e) throw new v(this._trans.__("Kernel is still connecting. Please check your network."));
-                            if (e > 0) throw new S(this._trans.__("Kernel is still connecting. Please check your network."));
-                            if (0 === e) throw new w(this._trans.__("Kernel is still connecting. Please check your network."))
+                            if (void 0 === e) throw new S(this._trans.__("Kernel is still connecting. Please check your network."));
+                            if (e > 0) throw new j(this._trans.__("Kernel is still connecting. Please check your network."));
+                            if (0 === e) throw new v(this._trans.__("Kernel is still connecting. Please check your network."))
                         }
                     }
                     const l = [];
                     for (const e of i) {
                         const t = await this.runWithInput(d, n, s, e);
                         l.push(t), this.model.submissionStatus = {
                             type: "progress",
@@ -292,70 +297,73 @@
                     }, this._submitted.emit({
                         widget: this,
                         submission: m,
                         problem: s
                     })
                 }
                 async runWithInput(e, t, s, n) {
-                    const o = {
-                        code: t,
-                        stop_on_error: !0,
-                        allow_stdin: !0
-                    };
-                    let i = [];
-                    i = "one_line" === s.inputTransferType ? n.split(/\r?\n/) : [n];
-                    const r = Date.now(),
-                        a = e.requestExecute(o, !0, {});
-                    a.onStdin = e => {
-                        if ("input_request" === e.header.msg_type) {
-                            const t = i.shift();
-                            a.sendInputReply({
-                                value: null != t ? t : "",
-                                status: "ok"
-                            }, e.header)
-                        }
-                    };
-                    const d = {
-                        output: "",
-                        status: "OK",
-                        cpuTime: 0
-                    };
-                    a.onIOPub = e => {
+                    const o = `\nimport io\nimport base64\n\ndef input():  \t\n    r = JUDGE_INPUT_STRING_IO.${"one_line"===s.inputTransferType?"readline":"read"}()  \t\n    if not r:  \t\t\n        return ''\n    return r\n\nJUDGE_INPUT_STRING_IO = io.StringIO()\n`;
+                    await e.requestExecute({
+                        code: o,
+                        stop_on_error: !0
+                    }, !0, {}).done;
+                    const i = 1e6;
+                    for (let t = 0; t < n.length; t += i) {
+                        const s = n.slice(t, t + i),
+                            o = `\nJUDGE_INPUT_STRING_IO.write(base64.b64decode('${f((new TextEncoder).encode(s))}').decode("utf-8"))\n`;
+                        await e.requestExecute({
+                            code: o,
+                            stop_on_error: !0
+                        }, !0, {}).done
+                    }
+                    const r = {
+                            code: "\nJUDGE_INPUT_STRING_IO.seek(0)\n" + t,
+                            stop_on_error: !0,
+                            allow_stdin: !0
+                        },
+                        a = Date.now(),
+                        d = e.requestExecute(r, !0, {}),
+                        l = {
+                            output: "",
+                            status: "OK",
+                            cpuTime: 0
+                        };
+                    d.onIOPub = e => {
                         switch (e.header.msg_type) {
                             case "stream": {
                                 const t = e;
-                                "stdout" === t.content.name && (d.output = d.output.concat(t.content.text));
+                                "stdout" === t.content.name && (l.output = l.output.concat(t.content.text));
                                 break
                             }
                             case "error":
-                                d.status = "RE"
+                                l.status = "RE"
                         }
                     };
-                    const l = 1e3 * s.timeout,
-                        u = new Promise((e => {
+                    const u = 1e3 * s.timeout,
+                        c = new Promise((e => {
                             setTimeout((() => {
                                 e(0)
-                            }), 1.2 * l)
+                            }), 1.2 * u)
                         }));
-                    if (0 === await Promise.race([a.done, u])) a.dispose(), await e.interrupt(), d.status = "TLE";
+                    if (0 === await Promise.race([d.done, c])) d.dispose(), await e.interrupt(), l.status = "TLE";
                     else {
-                        const e = Date.now() - r;
-                        e > l ? d.status = "TLE" : d.cpuTime = e
+                        const e = Date.now() - a;
+                        e > u ? l.status = "TLE" : l.cpuTime = e
                     }
-                    return d
+                    return l
                 }
             }
             class E extends d.DocumentWidget {
                 constructor(e) {
                     super(e), g.getDefaultItems(this.content, e.translator).forEach((e => {
                         this.toolbar.addItem(e.name, e.widget)
                     }))
                 }
             }
-            class I extends d.ABCWidgetFactory {
+            class k extends d.ABCWidgetFactory {
                 constructor(e) {
                     super(e.factoryOptions), this._editorServices = e.editorServices, this._rendermime = e.rendermime, this._commands = e.commands, this._editorConfig = e.editorConfig, this._sessionContextDialogs = e.sessionContextDialogs, this._judgePanelFactory = e.judgePanelFactory, this._judgeSubmissionAreaFactory = e.judgeSubmissionAreaFactory, this._judgeTerminalFactory = e.judgeTerminalFactory, this._submissionListFactory = e.submissionListFactory, this._submitted = e.submitted, this._executed = e.executed
                 }
                 createNewWidget(e) {
                     const t = this._judgePanelFactory({
                         rendermime: this._rendermime,
                         editorServices: this._editorServices,
@@ -373,27 +381,27 @@
                         content: t,
                         context: e,
                         commands: this._commands,
                         translator: this.translator
                     })
                 }
             }
-            var k, F = s(2737),
-                P = s(8093),
-                T = s(4901),
-                M = s(1509);
-            class J {
+            var T, P = s(7217),
+                F = s(8093),
+                N = s(4901),
+                J = s(2425);
+            class M {
                 constructor(e, t) {
-                    this._contentChanged = new T.Signal(this), this._stateChanged = new T.Signal(this), this._isDisposed = !1, this._dirty = !1, this._problemChanged = new T.Signal(this), this._submissionsChanged = new T.Signal(this), this._submissionStatus = {
+                    this._contentChanged = new N.Signal(this), this._stateChanged = new N.Signal(this), this._isDisposed = !1, this._dirty = !1, this._problemChanged = new N.Signal(this), this._submissionsChanged = new N.Signal(this), this._submissionStatus = {
                         type: "idle"
-                    }, this._submissionStatusChanged = new T.Signal(this), this.sharedModel = new J.YJudge, this.sharedModel.changed.connect((async (e, t) => {
+                    }, this._submissionStatusChanged = new N.Signal(this), this.sharedModel = new M.YJudge, this.sharedModel.changed.connect((async (e, t) => {
                         t.problemIdChange && (this._problem = await this._problemProvider.getProblem(t.problemIdChange), this._problemChanged.emit(this._problem)), t.stateChange && t.stateChange.forEach((e => {
                             "dirty" === e.name && (this.dirty = e.newValue)
                         })), t.sourceChange && (this._contentChanged.emit(), this.dirty = !0)
-                    })), this._codeModel = new M.CodeCellModel({
+                    })), this._codeModel = new J.CodeCellModel({
                         sharedModel: this.sharedModel.yCodeCell
                     }), this._codeModel.mimeType = "text/x-python", this._problem = null, this._problemProvider = e, this._collaborationEnabled = !!(null == t ? void 0 : t.collaborationEnabled)
                 }
                 get collaborative() {
                     return this._collaborationEnabled
                 }
                 get contentChanged() {
@@ -417,15 +425,15 @@
                     return !1
                 }
                 set readOnly(e) {}
                 get isDisposed() {
                     return this._isDisposed
                 }
                 dispose() {
-                    this.isDisposed || (this._isDisposed = !0, T.Signal.clearData(this))
+                    this.isDisposed || (this._isDisposed = !0, N.Signal.clearData(this))
                 }
                 initialize() {}
                 get defaultKernelName() {
                     return `Judge: Problem ${this.sharedModel.problemId}`
                 }
                 get defaultKernelLanguage() {
                     return "python"
@@ -502,15 +510,15 @@
                     return await this._problemProvider.validate(this.sharedModel.problemId, e)
                 }
                 async submit(e, t) {
                     const s = await this._problemProvider.submit(e, t);
                     return this._submissionsChanged.emit(await this._problemProvider.getSubmissions(this.sharedModel.problemId)), s
                 }
             }
-            async function N(e, t, s) {
+            async function A(e, t, s) {
                     const n = await e.getProblem(s);
                     if (n) {
                         const o = n.title,
                             i = `${h}/${s}/${o}.judge`,
                             r = `${h}`;
                         await t.services.contents.save(r, {
                             name: r,
@@ -520,19 +528,19 @@
                         return await t.services.contents.save(a, {
                             name: a,
                             type: "directory"
                         }), await async function(e, t, s, n) {
                             try {
                                 await t.services.contents.get(s)
                             } catch (o) {
-                                throw o instanceof F.ServerConnection.ResponseError && 404 === o.response.status && await t.services.contents.save(s, {
+                                throw o instanceof P.ServerConnection.ResponseError && 404 === o.response.status && await t.services.contents.save(s, {
                                     name: s,
                                     type: "file",
                                     format: "text",
-                                    content: await J.newFileContent(e, n)
+                                    content: await M.newFileContent(e, n)
                                 }), o
                             } finally {
                                 return t.openOrReveal(s)
                             }
                         }(e, t, i, s)
                     }
                 }! function(e) {
@@ -552,15 +560,15 @@
                         preferredLanguage(e) {
                             return "python"
                         }
                         createNew(t) {
                             return new e(this._problemProviderFactory(), t)
                         }
                     };
-                    class t extends P.YDocument {
+                    class t extends F.YDocument {
                         constructor() {
                             super(), this._version = "1.0.0", this._problemId = this.ydoc.getText("problem_id"), this._source = this.ydoc.getText("source"), this._outputs = this.ydoc.getArray("outputs"), this._metadata = this.ydoc.getMap("metadata"), this._ycodeCell = new s(this, this._source, this._outputs), this._problemId.observe((e => {
                                 this._changed.emit({
                                     problemIdChange: this.problemId
                                 })
                             })), this._ycodeCell.changed.connect(((e, t) => {
                                 this._changed.emit(t)
@@ -595,23 +603,23 @@
                         get version() {
                             return this._version
                         }
                     }
                     e.YJudge = t;
                     class s {
                         constructor(e, t, s) {
-                            this.id = "", this.cell_type = "code", this.execution_count = 0, this.isStandalone = !0, this.notebook = null, this.metadata = {}, this.metadataChanged = new T.Signal(this), this._sourceObserver = e => {
+                            this.id = "", this.cell_type = "code", this.execution_count = 0, this.isStandalone = !0, this.notebook = null, this.metadata = {}, this.metadataChanged = new N.Signal(this), this._sourceObserver = e => {
                                 this._changed.emit({
                                     sourceChange: e.changes.delta
                                 })
                             }, this._outputsObserver = e => {
                                 this._changed.emit({
                                     outputsChange: e.changes.delta
                                 })
-                            }, this._changed = new T.Signal(this), this._isDisposed = !1, this._disposed = new T.Signal(this), this._yjudge = e, this._source = t, this._outputs = s, this._source.observe(this._sourceObserver), this._outputs.observe(this._outputsObserver)
+                            }, this._changed = new N.Signal(this), this._isDisposed = !1, this._disposed = new N.Signal(this), this._yjudge = e, this._source = t, this._outputs = s, this._source.observe(this._sourceObserver), this._outputs.observe(this._outputsObserver)
                         }
                         get changed() {
                             return this._changed
                         }
                         get outputs() {
                             return this.getOutputs()
                         }
@@ -679,15 +687,15 @@
                         get disposed() {
                             return this._disposed
                         }
                         get isDisposed() {
                             return this._isDisposed
                         }
                         dispose() {
-                            this._isDisposed || (this._isDisposed = !0, this._source.unobserve(this._sourceObserver), this._outputs.unobserve(this._outputsObserver), this._disposed.emit(), T.Signal.clearData(this))
+                            this._isDisposed || (this._isDisposed = !0, this._source.unobserve(this._sourceObserver), this._outputs.unobserve(this._outputsObserver), this._disposed.emit(), N.Signal.clearData(this))
                         }
                         get ysource() {
                             return this._source
                         }
                         get awareness() {
                             return this._yjudge.awareness
                         }
@@ -700,29 +708,29 @@
                         const o = {
                             problem_id: t,
                             code: null !== (n = null === (s = await e.getProblem(t)) || void 0 === s ? void 0 : s.skeletonCode) && void 0 !== n ? n : "# 여기에 입력하세요",
                             judge_format: 1
                         };
                         return JSON.stringify(o)
                     }
-                }(J || (J = {})),
+                }(M || (M = {})),
                 function(e) {
                     e.open = `${p}:plugin:open`, e.openOrCreateFromId = `${p}:plugin:open-or-create-from-id`, e.execute = `${p}:plugin:execute`, e.undo = `${p}:plugin:undo`, e.redo = `${p}:plugin:redo`, e.run = `${p}:plugin:run`, e.runAll = `${p}:plugin:run-all`
-                }(k || (k = {}));
-            var A = s(3e3),
-                O = s(6105),
-                D = s(1801),
-                L = s(7930);
-            const W = new L.Token(`${p}:IProblemProvider`),
-                $ = new L.Token(`${p}:IJudgePanelFactory`),
-                R = new L.Token(`${p}:IJudgeSubmissionAreaFactory`),
-                K = new L.Token(`${p}:IJudgeTerminalFactory`),
-                B = new L.Token(`${p}:ISubmissionListFactory`),
-                z = new L.Token(`${p}:IJudgeSignal`);
-            class U {
+                }(T || (T = {}));
+            var O = s(5326),
+                D = s(9557),
+                L = s(4008),
+                W = s(7930);
+            const $ = new W.Token(`${p}:IProblemProvider`),
+                R = new W.Token(`${p}:IJudgePanelFactory`),
+                K = new W.Token(`${p}:IJudgeSubmissionAreaFactory`),
+                B = new W.Token(`${p}:IJudgeTerminalFactory`),
+                U = new W.Token(`${p}:ISubmissionListFactory`),
+                z = new W.Token(`${p}:IJudgeSignal`);
+            class q {
                 constructor() {
                     this.problems = {
                         1: {
                             id: "1",
                             title: "덧셈",
                             timeout: 1,
                             inputTransferType: "one_line",
@@ -779,43 +787,43 @@
                         userId: "",
                         createdAt: (new Date).toISOString()
                     };
                     return this._idToSubmissions[e.problemId].push(t), t
                 }
             }
             var H = s(3848),
-                q = s(8149),
-                Q = s.n(q);
+                G = s(8149),
+                Q = s.n(G);
 
             function V(e) {
-                const t = (0, u.useContext)(fe),
+                const t = (0, u.useContext)(we),
                     [s, n] = (0, u.useState)(!1);
                 return c().createElement(Y, {
                     className: e.className
-                }, c().createElement(G, {
+                }, c().createElement(X, {
                     onClick: async () => {
                         n(!0);
                         try {
                             await e.panel.judge()
                         } catch (s) {
                             let o = "";
-                            if (o = s instanceof f ? s.message : t.__("An error occurred during submission."), e.panel.model.submissionStatus = {
+                            if (o = s instanceof w ? s.message : t.__("An error occurred during submission."), e.panel.model.submissionStatus = {
                                     type: "error",
                                     errorDetails: o
-                                }, n(!1), !(s instanceof w)) throw s
+                                }, n(!1), !(s instanceof v)) throw s
                         }
                         n(!1)
                     },
                     disabled: s
                 }, t.__("Submit")))
             }
             const Y = Q().div`
   background: var(--jp-layout-color2);
 `,
-                G = Q().button`
+                X = Q().button`
   display: block;
   margin-top: 12px;
   margin-left: 20px;
   margin-right: 20px;
   padding: 11px 17px;
 
   cursor: pointer;
@@ -844,18 +852,18 @@
     cursor: not-allowed;
   }
 
   :not(:disabled):hover {
     background: var(--jp-brand-color0);
   }
 `;
-            var X = s(6108);
+            var Z = s(6311);
 
-            function Z(e) {
-                const t = (0, u.useContext)(fe);
+            function ee(e) {
+                const t = (0, u.useContext)(we);
                 let s = "",
                     n = "";
                 switch (e.status) {
                     case "AC":
                         s = `👍 ${t.__("Accepted")}`;
                         break;
                     case "WA":
@@ -869,129 +877,129 @@
                         break;
                     case "OLE":
                         s = `👀 ${t.__("Output Limit")}`;
                         break;
                     case "IE":
                         s = `☠ ${t.__("Please Try Again")}`
                 }
-                return c().createElement(ee, {
+                return c().createElement(te, {
                     className: e.className,
                     title: n
                 }, s)
             }
-            const ee = Q().span``;
+            const te = Q().span``;
 
-            function te(e) {
-                const t = (0, u.useContext)(fe),
-                    s = X.Time.formatHuman(new Date(e.submission.createdAt)),
-                    n = X.Time.format(new Date(e.submission.createdAt));
-                return c().createElement(se, {
+            function se(e) {
+                const t = (0, u.useContext)(we),
+                    s = Z.Time.formatHuman(new Date(e.submission.createdAt)),
+                    n = Z.Time.format(new Date(e.submission.createdAt));
+                return c().createElement(ne, {
                     className: e.className
-                }, c().createElement(ne, {
+                }, c().createElement(oe, {
                     status: e.submission.status,
                     acceptedCount: e.submission.acceptedCount,
                     totalCount: e.submission.totalCount
-                }), c().createElement(oe, {
+                }), c().createElement(ie, {
                     onClick: () => {
                         e.setCode(e.submission.code)
                     },
                     title: e.submission.code.substring(0, 1e3)
-                }, t.__("Load this submission")), c().createElement(ie, {
+                }, t.__("Load this submission")), c().createElement(re, {
                     title: n
                 }, s))
             }
-            const se = Q().li`
+            const ne = Q().li`
   display: flex;
   padding: 5px 12px;
   height: 16px;
 
   font-family: var(--jp-ui-font-family);
   font-style: normal;
   font-size: 12px;
   line-height: 16px;
 `,
-                ne = Q()(Z)`
+                oe = Q()(ee)`
   height: 16px;
   flex-grow: 0;
   flex-shrink: 0;
 
   width: 101px;
   margin-right: 8px;
 `,
-                oe = Q().button`
+                ie = Q().button`
   height: 16px;
   flex-grow: 0;
   flex-shrink: 0;
 
   all: unset;
   cursor: pointer;
 
   font-family: var(--jp-ui-font-family);
   font-style: normal;
   font-weight: 700;
   font-size: 12px;
   line-height: 16px;
   color: var(--jp-brand-color1);
 `,
-                ie = Q().span`
+                re = Q().span`
   height: 16px;
   flex-grow: 1;
   flex-shrink: 1;
 
   text-align: right;
 
   font-family: var(--jp-ui-font-family);
   font-style: normal;
   font-weight: 400;
   font-size: 12px;
   line-height: 16px;
 
   color: var(--jp-ui-font-color3);
 `,
-                re = Q().span``;
+                ae = Q().span``;
 
-            function ae(e) {
-                return c().createElement(de, {
+            function de(e) {
+                return c().createElement(le, {
                     className: e.className
-                }, c().createElement(le, {
+                }, c().createElement(ue, {
                     status: e.status
                 }))
             }
-            const de = Q().li`
+            const le = Q().li`
   display: flex;
   padding: 5px 12px;
   height: 16px;
 
   font-family: var(--jp-ui-font-family);
   font-style: normal;
   font-size: 12px;
   line-height: 16px;
 `,
-                le = Q()((function(e) {
+                ue = Q()((function(e) {
                     const {
                         status: t
-                    } = e, s = (0, u.useContext)(fe);
-                    return "idle" === t.type ? c().createElement(c().Fragment, null) : "error" === t.type ? c().createElement(re, {
+                    } = e, s = (0, u.useContext)(we);
+                    return "idle" === t.type ? c().createElement(c().Fragment, null) : "error" === t.type ? c().createElement(ae, {
                         className: e.className
-                    }, `🚫 ${t.errorDetails}`) : c().createElement(re, {
+                    }, `🚫 ${t.errorDetails}`) : c().createElement(ae, {
                         className: e.className
                     }, 0 === t.totalCount ? `⌛ ${s.__("In Progress")}` : `⌛ ${s.__("In Progress")} (${t.runCount}/${t.totalCount})`)
                 }))`
   height: 16px;
   flex-grow: 0;
   flex-shrink: 0;
 
   margin-right: 8px;
 `;
 
-            function ue(e) {
+            function ce(e) {
                 const t = (0, H.useQueryClient)(),
                     {
                         submissionListFactory: s
-                    } = (0, u.useContext)(we);
+                    } = (0, u.useContext)(ve);
                 return c().createElement(o.UseSignal, {
                     signal: e.model.problemChanged,
                     initialSender: e.model,
                     initialArgs: e.model.problem
                 }, ((n, i) => c().createElement(o.UseSignal, {
                     signal: e.model.submissionsChanged,
                     initialSender: e.model
@@ -1013,43 +1021,43 @@
                             e.model.source = t
                         },
                         submissionStatus: null != n ? n : null
                     })))
                 }))))
             }
 
-            function ce(e) {
-                const t = (0, u.useContext)(fe);
-                if (null === e.problemId) return c().createElement(ge, {
+            function me(e) {
+                const t = (0, u.useContext)(we);
+                if (null === e.problemId) return c().createElement(_e, {
                     className: e.className
                 }, "⌛ ", t.__("Loading History"));
                 const {
                     data: s,
                     isLoading: n
                 } = (0, H.useQuery)(["submissions", e.problemId], e.getSubmissions);
-                if (n) return c().createElement(ge, {
+                if (n) return c().createElement(_e, {
                     className: e.className
                 }, "⌛ ", t.__("Loading History"));
-                if (void 0 === s) return c().createElement(ge, {
+                if (void 0 === s) return c().createElement(_e, {
                     className: e.className
                 }, "🚫 ", t.__("History Not Available"));
                 const o = e.submissionStatus && "idle" === e.submissionStatus.type;
-                return 0 === s.length && o ? c().createElement(_e, {
+                return 0 === s.length && o ? c().createElement(be, {
                     className: e.className
-                }, t.__("Submit your code to get results here.")) : c().createElement(me, {
+                }, t.__("Submit your code to get results here.")) : c().createElement(he, {
                     className: e.className
-                }, e.submissionStatus && "idle" !== e.submissionStatus.type && c().createElement(pe, {
+                }, e.submissionStatus && "idle" !== e.submissionStatus.type && c().createElement(ge, {
                     status: e.submissionStatus
-                }), s.map((t => c().createElement(he, {
+                }), s.map((t => c().createElement(pe, {
                     submission: t,
                     key: t.id,
                     setCode: e.setCode
                 }))))
             }
-            const me = Q().ul`
+            const he = Q().ul`
   padding: 7px 0px 0px 0px;
   margin: 0px;
 
   overflow-y: auto;
 
   /* width */
   ::-webkit-scrollbar {
@@ -1058,117 +1066,117 @@
 
   /* Handle */
   ::-webkit-scrollbar-thumb {
     background: var(--jp-border-color0);
     border-radius: 12px;
   }
 `,
-                he = Q()(te)``,
-                pe = Q()(ae)``,
-                ge = Q().div`
+                pe = Q()(se)``,
+                ge = Q()(de)``,
+                _e = Q().div`
   text-align: center;
   padding: 5px;
   font-size: var(--jp-ui-font-size2);
 `,
-                _e = Q().div`
+                be = Q().div`
   padding: 12px;
   font-weight: 700;
   font-size: 12px;
   line-height: 16px;
   color: var(--jp-ui-font-color3);
 `;
 
-            function be(e) {
-                const t = (0, u.useContext)(fe);
-                return null === e.model ? c().createElement("div", null, t.__("No Submission History Found.")) : c().createElement(ye, null, c().createElement(Ce, {
+            function ye(e) {
+                const t = (0, u.useContext)(we);
+                return null === e.model ? c().createElement("div", null, t.__("No Submission History Found.")) : c().createElement(Ce, null, c().createElement(fe, {
                     model: e.model
                 }), c().createElement(xe, {
                     panel: e.panel
                 }))
             }
-            const ye = Q().div`
+            const Ce = Q().div`
   display: flex;
   border-top: 4px solid var(--jp-border-color0);
   font-size: var(--jp-ui-font-size1);
 
   height: 100%;
 `,
-                Ce = Q()(ue)`
+                fe = Q()(ce)`
   flex-grow: 1;
   flex-shrink: 1;
 
   margin-right: 2px;
 `,
                 xe = Q()(V)`
   flex-grow: 0;
   flex-shrink: 0;
 `,
-                fe = c().createContext(i.nullTranslator.load(m)),
-                we = c().createContext({
-                    submissionListFactory: ce
+                we = c().createContext(i.nullTranslator.load(m)),
+                ve = c().createContext({
+                    submissionListFactory: me
                 });
-            class ve extends o.ReactWidget {
+            class Se extends o.ReactWidget {
                 constructor(e) {
                     super(), this.queryClient = new H.QueryClient, this._panel = e.panel, this._model = e.model, this._trans = e.translator.load(m), this._submissionListFactory = e.submissionListFactory
                 }
                 render() {
                     var e, t;
-                    return c().createElement(we.Provider, {
+                    return c().createElement(ve.Provider, {
                         value: {
                             submissionListFactory: this._submissionListFactory
                         }
-                    }, c().createElement(fe.Provider, {
+                    }, c().createElement(we.Provider, {
                         value: this._trans
                     }, c().createElement(H.QueryClientProvider, {
                         client: this.queryClient
-                    }, c().createElement(be, {
+                    }, c().createElement(ye, {
                         key: null !== (t = null === (e = this._model.problem) || void 0 === e ? void 0 : e.id) && void 0 !== t ? t : "",
                         panel: this._panel,
                         model: this._model
                     }))))
                 }
             }
-            const Se = "jp-OutputArea-output";
-            class je extends l.OutputArea {
+            const je = "jp-OutputArea-output";
+            class Ie extends l.OutputArea {
                 constructor(e) {
                     super(e), this.addClass("jp-JudgeOutputArea");
                     const t = e.translator.load(m),
                         s = document.createElement("div");
                     s.className = "jp-JudgeOutputArea-placeholder", s.textContent = t.__("Execution result will be shown here"), this.node.appendChild(s)
                 }
                 createOutputItem(e) {
                     const t = this.createRenderedMimetype(e);
-                    return t && t.addClass(Se), t
+                    return t && t.addClass(je), t
                 }
                 onInputRequest(e, t) {
                     const s = this.contentFactory,
                         n = e.content.prompt,
                         o = e.content.password,
                         i = new _.Panel;
                     i.addClass("jp-OutputArea-child"), i.addClass("jp-OutputArea-stdin-item");
                     const r = s.createStdin({
                         parent_header: e.header,
                         prompt: n,
                         password: o,
                         future: t
                     });
-                    r.addClass(Se), i.addWidget(r), this.layout.addWidget(i), r.value.then((e => {
+                    r.addClass(je), i.addWidget(r), this.layout.addWidget(i), r.value.then((e => {
                         this.model.add({
                             output_type: "stream",
                             name: "stdin",
                             text: e + "\n"
                         }), i.dispose()
                     }))
                 }
             }
             const Ee = new r.LabIcon({
                 name: "judge-icon:reset",
                 svgstr: b.cornerUpLeftDoubleFillSvg
             });
-            class Ie extends _.Panel {
+            class ke extends _.Panel {
                 constructor(e) {
                     super(), this.addClass("jp-JudgeTerminal");
                     const t = e.translator.load(m),
                         s = new _.Widget,
                         n = document.createElement("button");
                     n.className = "jp-JudgeTerminal-resetButton", Ee.element({
                         container: n
@@ -1201,155 +1209,155 @@
                     const c = document.createElement("button");
                     c.className = "jp-JudgeTerminal-stopButton", r.stopIcon.element({
                         container: c
                     });
                     const h = document.createElement("span");
                     h.className = "jp-JudgeTerminal-stopButtonLabel", h.textContent = t.__("Stop"), c.addEventListener("click", (async () => {
                         await e.panel.session.shutdown()
-                    })), c.appendChild(h), s.node.appendChild(n), s.node.appendChild(a), s.node.appendChild(d), s.node.appendChild(u), s.node.appendChild(c), this.addWidget(s), this._outputArea = new je(e), this.addWidget(this._outputArea)
+                    })), c.appendChild(h), s.node.appendChild(n), s.node.appendChild(a), s.node.appendChild(d), s.node.appendChild(u), s.node.appendChild(c), this.addWidget(s), this._outputArea = new Ie(e), this.addWidget(this._outputArea)
                 }
                 get outputArea() {
                     return this._outputArea
                 }
             }
-            const ke = new T.Signal({}),
-                Fe = new T.Signal({}),
-                Pe = {
+            const Te = new N.Signal({}),
+                Pe = new N.Signal({}),
+                Fe = {
                     id: `${p}:IJudgeSignal`,
                     provides: z,
                     activate: e => ({
                         get submitted() {
-                            return ke
+                            return Te
                         },
                         get executed() {
-                            return Fe
+                            return Pe
                         }
                     }),
                     autoStart: !0
                 },
-                Te = [{
+                Ne = [{
                     id: `${p}:plugin`,
                     autoStart: !0,
-                    requires: [i.ITranslator, a.IEditorServices, y.IRenderMimeRegistry, A.IDocumentManager, O.IMainMenu, o.ICommandPalette, o.ISessionContextDialogs],
-                    optional: [$, R, K, B, W, D.ISettingRegistry, n.ILayoutRestorer],
+                    requires: [i.ITranslator, a.IEditorServices, y.IRenderMimeRegistry, O.IDocumentManager, D.IMainMenu, o.ICommandPalette, o.ISessionContextDialogs],
+                    optional: [R, K, B, U, $, L.ISettingRegistry, n.ILayoutRestorer],
                     activate: async (e, t, s, n, i, r, a, d, l, u, c, h, p, g, _) => {
                         const b = t.load(m),
                             y = new o.WidgetTracker({
                                 namespace: "judge"
                             }),
                             C = b.__("Judge");
-                        let x;
-                        x = g ? (await g.load("@jupyterlab/notebook-extension:tracker")).get("codeCellConfig").composite : {};
-                        const f = new I({
+                        let f;
+                        f = g ? (await g.load("@jupyterlab/notebook-extension:tracker")).get("codeCellConfig").composite : {};
+                        const x = new k({
                             editorServices: s,
                             rendermime: n,
                             commands: e.commands,
-                            editorConfig: x,
+                            editorConfig: f,
                             sessionContextDialogs: d,
-                            judgePanelFactory: null != l ? l : e => new j(e),
-                            judgeSubmissionAreaFactory: null != u ? u : e => new ve(e),
-                            judgeTerminalFactory: null != c ? c : e => new Ie(e),
-                            submissionListFactory: null != h ? h : ce,
-                            submitted: ke,
-                            executed: Fe,
+                            judgePanelFactory: null != l ? l : e => new I(e),
+                            judgeSubmissionAreaFactory: null != u ? u : e => new Se(e),
+                            judgeTerminalFactory: null != c ? c : e => new ke(e),
+                            submissionListFactory: null != h ? h : me,
+                            submitted: Te,
+                            executed: Pe,
                             factoryOptions: {
                                 name: C,
                                 modelName: "judge-model",
                                 fileTypes: ["judge"],
                                 defaultFor: ["judge"],
                                 preferKernel: !0,
                                 canStartKernel: !0,
                                 shutdownOnClose: !0,
                                 translator: t
                             }
                         });
-                        f.widgetCreated.connect(((e, t) => {
+                        x.widgetCreated.connect(((e, t) => {
                             t.context.pathChanged.connect((() => {
                                 y.save(t)
                             })), y.add(t)
-                        })), e.docRegistry.addWidgetFactory(f);
-                        const w = null != p ? p : new U;
-                        e.docRegistry.addModelFactory(new J.JudgeModelFactory({
+                        })), e.docRegistry.addWidgetFactory(x);
+                        const w = null != p ? p : new q;
+                        e.docRegistry.addModelFactory(new M.JudgeModelFactory({
                                 problemProviderFactory: () => w
                             })), e.docRegistry.addFileType({
                                 name: "judge",
                                 contentType: "file",
                                 fileFormat: "text",
                                 displayName: b.__("Judge File"),
                                 extensions: [".judge"],
                                 mimeTypes: ["text/json", "application/json"]
                             }),
                             function(e, t, s, n, o) {
-                                e.addCommand(k.open, {
+                                e.addCommand(T.open, {
                                     execute: async e => {
                                         s.openOrReveal(e.path)
                                     },
                                     label: t.__("Open Judge")
-                                }), e.addCommand(k.openOrCreateFromId, {
+                                }), e.addCommand(T.openOrCreateFromId, {
                                     execute: async e => {
-                                        e.problemId && await N(o, s, e.problemId)
+                                        e.problemId && await A(o, s, e.problemId)
                                     },
                                     label: t.__("Open or Create Judge From Id")
-                                }), e.addCommand(k.execute, {
+                                }), e.addCommand(T.execute, {
                                     execute: async e => {
                                         n.currentWidget && n.currentWidget.content.execute()
                                     },
                                     label: t.__("Execute")
-                                }), e.addCommand(k.redo, {
+                                }), e.addCommand(T.redo, {
                                     execute: async () => {
                                         n.currentWidget && n.currentWidget.content.editor.redo()
                                     },
                                     label: t.__("Redo")
-                                }), e.addCommand(k.undo, {
+                                }), e.addCommand(T.undo, {
                                     execute: async () => {
                                         n.currentWidget && n.currentWidget.content.editor.undo()
                                     },
                                     label: t.__("Undo")
-                                }), e.addCommand(k.run, {
+                                }), e.addCommand(T.run, {
                                     execute: async () => {
                                         n.currentWidget && n.currentWidget.content.execute()
                                     },
                                     label: t.__("Run")
-                                }), e.addCommand(k.runAll, {
+                                }), e.addCommand(T.runAll, {
                                     execute: async () => {
                                         n.currentWidget && n.currentWidget.content.execute()
                                     },
                                     label: t.__("Run All")
                                 })
                             }(e.commands, b, i, y, w),
                             function(e, t, s) {
                                 ! function(e) {
                                     e.editMenu.undoers.undo.add({
-                                        id: k.undo,
+                                        id: T.undo,
                                         isEnabled: e => e instanceof E
                                     }), e.editMenu.undoers.redo.add({
-                                        id: k.redo,
+                                        id: T.redo,
                                         isEnabled: e => e instanceof E
                                     })
                                 }(e),
                                 function(e) {
                                     e.runMenu.codeRunners.run.add({
-                                        id: k.run,
+                                        id: T.run,
                                         isEnabled: e => e instanceof E
                                     }), e.runMenu.codeRunners.runAll.add({
-                                        id: k.runAll,
+                                        id: T.runAll,
                                         isEnabled: e => e instanceof E
                                     })
                                 }(e)
                             }(r), a.addItem({
-                                command: k.openOrCreateFromId,
+                                command: T.openOrCreateFromId,
                                 category: "Judge",
                                 args: {
                                     problemId: "1"
                                 }
                             }), _ && _.restore(y, {
-                                command: k.open,
+                                command: T.open,
                                 args: e => ({
                                     path: e.context.path
                                 }),
                                 name: e => e.context.path
                             })
                     }
-                }, Pe]
+                }, Fe]
         }
     }
 ]);
```

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/remoteEntry.5c8a6aaf9a330f5d95c4.js` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/remoteEntry.5b4a6b2fd107c17f4d34.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -51,37 +51,37 @@
         146: "ffbfc6be3b1d44378330",
         316: "18d9e632074f3acc892c",
         378: "2c7a4a82fbc8f09f2463",
         505: "fe5d2436cfe6faec3918",
         599: "7e6937b28ad247ccde7c",
         704: "e67611936df713555ea4",
         732: "d368cf762f465d394900",
-        747: "13907913bad1ebbd3546",
+        747: "2841a40cba671c554a8c",
         767: "69c7e698f115ea487665",
         860: "fee57e15b3a40a2d65fa",
         893: "389b596eee368876402a",
         901: "b84e014859b58a1fa86a",
         917: "ab3207654a9c812bc979",
-        960: "30572a65d088e05e87a5"
+        960: "248f24628be1ecbf1885"
     } [e] + ".js?v=" + {
         29: "d2153138b471f40c1c27",
         146: "ffbfc6be3b1d44378330",
         316: "18d9e632074f3acc892c",
         378: "2c7a4a82fbc8f09f2463",
         505: "fe5d2436cfe6faec3918",
         599: "7e6937b28ad247ccde7c",
         704: "e67611936df713555ea4",
         732: "d368cf762f465d394900",
-        747: "13907913bad1ebbd3546",
+        747: "2841a40cba671c554a8c",
         767: "69c7e698f115ea487665",
         860: "fee57e15b3a40a2d65fa",
         893: "389b596eee368876402a",
         901: "b84e014859b58a1fa86a",
         917: "ab3207654a9c812bc979",
-        960: "30572a65d088e05e87a5"
+        960: "248f24628be1ecbf1885"
     } [e], T.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -133,15 +133,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (o[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (i("@emotion/react", "11.11.1", (() => Promise.all([T.e(146), T.e(29), T.e(599)]).then((() => () => T(917))))), i("@emotion/styled", "11.11.0", (() => Promise.all([T.e(29), T.e(505), T.e(378)]).then((() => () => T(4378))))), i("@team-monolith/cds", "1.0.1", (() => Promise.all([T.e(146), T.e(901), T.e(29), T.e(704), T.e(316)]).then((() => () => T(7210))))), i("jupyterlab-judge", "1.23.0-rc0", (() => Promise.all([T.e(29), T.e(960)]).then((() => () => T(960))))), i("react-query", "3.39.3", (() => Promise.all([T.e(767), T.e(29), T.e(704)]).then((() => () => T(8767)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@emotion/react", "11.11.1", (() => Promise.all([T.e(146), T.e(29), T.e(599)]).then((() => () => T(917))))), i("@emotion/styled", "11.11.0", (() => Promise.all([T.e(29), T.e(505), T.e(378)]).then((() => () => T(4378))))), i("@team-monolith/cds", "1.0.1", (() => Promise.all([T.e(146), T.e(901), T.e(29), T.e(704), T.e(316)]).then((() => () => T(7210))))), i("jupyterlab-judge", "1.24.1", (() => Promise.all([T.e(29), T.e(960)]).then((() => () => T(960))))), i("react-query", "3.39.3", (() => Promise.all([T.e(767), T.e(29), T.e(704)]).then((() => () => T(8767)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         T.g.importScripts && (e = T.g.location + "");
         var r = T.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -250,48 +250,48 @@
         var n = T.I(r);
         return n && n.then ? n.then(e.bind(e, r, T.S[r], t, a, o)) : e(r, T.S[r], t, a, o)
     })(((e, r, t, a) => r && T.o(r, t) ? h(i(r, t)) : a())), y = m(((e, r, t, a) => (l(e, t), h(s(r, t, a) || b(r, e, t, a) || i(r, t))))), g = m(((e, r, t, a) => (l(e, t), f(r, 0, t, a)))), j = m(((e, r, t, a, o) => {
         var n = r && T.o(r, t) && s(r, t, a);
         return n ? h(n) : o()
     })), P = {}, w = {
         6029: () => g("default", "react", [1, 18, 2, 0]),
-        678: () => g("default", "@jupyterlab/codeeditor", [1, 4, 0, 11]),
-        1509: () => y("default", "@jupyterlab/cells", [1, 4, 0, 11]),
-        1562: () => g("default", "@jupyterlab/translation", [1, 4, 0, 11]),
-        1645: () => y("default", "@jupyterlab/outputarea", [1, 4, 0, 11]),
-        1801: () => g("default", "@jupyterlab/settingregistry", [1, 4, 0, 11]),
-        2038: () => g("default", "@jupyterlab/ui-components", [1, 4, 0, 11]),
-        2737: () => g("default", "@jupyterlab/services", [1, 7, 0, 11]),
-        3e3: () => g("default", "@jupyterlab/docmanager", [1, 4, 0, 11]),
+        1638: () => y("default", "@jupyterlab/docregistry", [1, 4, 1, 5]),
+        1778: () => y("default", "@jupyterlab/outputarea", [1, 4, 1, 5]),
+        2425: () => y("default", "@jupyterlab/cells", [1, 4, 1, 5]),
+        3452: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
+        3471: () => g("default", "@jupyterlab/codeeditor", [1, 4, 1, 5]),
         3848: () => j("default", "react-query", [2, 3, 39, 0], (() => Promise.all([T.e(767), T.e(704)]).then((() => () => T(8767))))),
-        4111: () => g("default", "@jupyterlab/application", [1, 4, 0, 11]),
+        4008: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 5]),
+        4882: () => g("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         4901: () => g("default", "@lumino/signaling", [1, 2, 0, 0]),
-        4938: () => g("default", "@jupyterlab/rendermime", [1, 4, 0, 11]),
-        5123: () => g("default", "@jupyterlab/apputils", [1, 4, 1, 11]),
+        5326: () => g("default", "@jupyterlab/docmanager", [1, 4, 1, 5]),
         5536: () => j("default", "@team-monolith/cds", [1, 1, 0, 1], (() => Promise.all([T.e(146), T.e(901), T.e(704), T.e(316)]).then((() => () => T(7210))))),
-        6105: () => g("default", "@jupyterlab/mainmenu", [1, 4, 0, 11]),
-        6108: () => g("default", "@jupyterlab/coreutils", [1, 6, 0, 11]),
+        5962: () => g("default", "@jupyterlab/translation", [1, 4, 1, 5]),
+        6311: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 5]),
+        7217: () => g("default", "@jupyterlab/services", [1, 7, 1, 5]),
         7930: () => g("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        8060: () => y("default", "@jupyterlab/docregistry", [1, 4, 0, 11]),
+        8048: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 5]),
         8093: () => g("default", "@jupyter/ydoc", [1, 1, 1, 1]),
         8149: () => j("default", "@emotion/styled", [1, 11, 6, 0], (() => Promise.all([T.e(505), T.e(860)]).then((() => () => T(4378))))),
-        8778: () => g("default", "@lumino/widgets", [1, 2, 0, 1]),
+        8368: () => g("default", "@jupyterlab/application", [1, 4, 1, 5]),
+        9510: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
+        9557: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 5]),
         799: () => j("default", "@emotion/react", [1, 11, 0, 0, , "rc", 0], (() => Promise.all([T.e(146), T.e(917)]).then((() => () => T(917))))),
         5211: () => v("default", "@emotion/react", (() => Promise.all([T.e(146), T.e(917)]).then((() => () => T(917))))),
         7704: () => g("default", "react-dom", [1, 18, 2, 0]),
         718: () => j("default", "@emotion/styled", [1, 11, 8, 1], (() => Promise.all([T.e(505), T.e(893)]).then((() => () => T(4378))))),
         2148: () => j("default", "@emotion/react", [1, 11, 4, 1], (() => T.e(732).then((() => () => T(917))))),
         8800: () => j("default", "@emotion/styled", [1, 11, 3, 0], (() => Promise.all([T.e(505), T.e(893)]).then((() => () => T(4378))))),
         9558: () => j("default", "@emotion/react", [1, 11, 8, 2], (() => T.e(732).then((() => () => T(917)))))
     }, S = {
         29: [6029],
         316: [718, 2148, 8800, 9558],
         505: [799, 5211],
         704: [7704],
-        960: [678, 1509, 1562, 1645, 1801, 2038, 2737, 3e3, 3848, 4111, 4901, 4938, 5123, 5536, 6105, 6108, 7930, 8060, 8093, 8149, 8778]
+        960: [1638, 1778, 2425, 3452, 3471, 3848, 4008, 4882, 4901, 5326, 5536, 5962, 6311, 7217, 7930, 8048, 8093, 8149, 8368, 9510, 9557]
     }, T.f.consumes = (e, r) => {
         T.o(S, e) && S[e].forEach((e => {
             if (T.o(P, e)) return r.push(P[e]);
             var t = r => {
                     P[e] = 0, T.m[e] = t => {
                         delete T.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/labextension/static/third-party-licenses.json` & `jupyterlab_judge-1.24.1/jupyterlab_judge/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json` & `jupyterlab_judge-1.24.1/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po` & `jupyterlab_judge-1.24.1/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/commands.ts` & `jupyterlab_judge-1.24.1/src/commands.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/handler.ts` & `jupyterlab_judge-1.24.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/index.ts` & `jupyterlab_judge-1.24.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/model.ts` & `jupyterlab_judge-1.24.1/src/model.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/tokens.ts` & `jupyterlab_judge-1.24.1/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/toolbar.tsx` & `jupyterlab_judge-1.24.1/src/toolbar.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/components/SubmissionArea.tsx` & `jupyterlab_judge-1.24.1/src/components/SubmissionArea.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/components/SubmissionControl.tsx` & `jupyterlab_judge-1.24.1/src/components/SubmissionControl.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/components/SubmissionItem.tsx` & `jupyterlab_judge-1.24.1/src/components/SubmissionItem.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/components/SubmissionItemStatus.tsx` & `jupyterlab_judge-1.24.1/src/components/SubmissionItemStatus.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/components/SubmissionItemWait.tsx` & `jupyterlab_judge-1.24.1/src/components/SubmissionItemWait.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/components/SubmissionItemWaitStatus.tsx` & `jupyterlab_judge-1.24.1/src/components/SubmissionItemWaitStatus.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/components/SubmissionList.tsx` & `jupyterlab_judge-1.24.1/src/components/SubmissionList.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/problemProvider/HardCodedProblemProvider.ts` & `jupyterlab_judge-1.24.1/src/problemProvider/HardCodedProblemProvider.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/problemProvider/problemProvider.ts` & `jupyterlab_judge-1.24.1/src/problemProvider/problemProvider.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/widgets/JudgeOutputArea.ts` & `jupyterlab_judge-1.24.1/src/widgets/JudgeOutputArea.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/widgets/JudgePanel.ts` & `jupyterlab_judge-1.24.1/src/widgets/JudgePanel.ts`

 * *Files 6% similar despite different names*

```diff
@@ -19,29 +19,36 @@
   DocumentWidget,
   IDocumentWidget
 } from '@jupyterlab/docregistry';
 import { IRenderMimeRegistry } from '@jupyterlab/rendermime';
 import { CommandRegistry } from '@lumino/commands';
 import { OutputArea } from '@jupyterlab/outputarea';
 import { KernelMessage } from '@jupyterlab/services';
-import { IHeader, IStreamMsg } from '@jupyterlab/services/lib/kernel/messages';
+import { IStreamMsg } from '@jupyterlab/services/lib/kernel/messages';
 import { JudgeModel } from '../model';
 import { ProblemProvider } from '../problemProvider/problemProvider';
 import { ToolbarItems } from '../toolbar';
 import { TRANSLATOR_DOMAIN } from '../constants';
 import { Signal } from '@lumino/signaling';
 import { BoxPanel, SplitPanel, Widget } from '@lumino/widgets';
 import { JudgeTerminal } from './JudgeTerminal';
 import { JudgeSubmissionArea } from './JudgeSubmissionArea';
 import { SubmissionList } from '../components/SubmissionList';
 import { IKernelConnection } from '@jupyterlab/services/lib/kernel/kernel';
 import { JudgeSignal } from '../tokens';
 import { customJudgeColorSvg } from '@team-monolith/cds';
 import { IJudgeProblemPanel, JudgeProblemPanel } from './JudgeProblemPanel';
 
+function bytesToBase64(bytes: Uint8Array) {
+  const binString = Array.from(bytes, byte => String.fromCodePoint(byte)).join(
+    ''
+  );
+  return btoa(binString);
+}
+
 const JudgeColorLabIcon = new LabIcon({
   name: 'jupyterlab-judge:problem-icon',
   svgstr: customJudgeColorSvg
 });
 
 interface IRunResult {
   status: 'OK' | 'TLE' | 'OLE' | 'RE';
@@ -484,43 +491,77 @@
 
   private async runWithInput(
     kernel: IKernelConnection,
     code: string,
     problem: ProblemProvider.IProblem,
     input: string
   ): Promise<IRunResult> {
+    // Transfer inputs to python kernel first,
+    // and then run the code with timeout.
+
+    // Step 1: Override input function
+    //         Prepare StringIO for input
+    const prepareInput = `
+import io
+import base64
+
+def input():  	
+    r = JUDGE_INPUT_STRING_IO.${
+      problem.inputTransferType === 'one_line' ? 'readline' : 'read'
+    }()  	
+    if not r:  		
+        return ''
+    return r
+
+JUDGE_INPUT_STRING_IO = io.StringIO()
+`;
+    await kernel.requestExecute(
+      {
+        code: prepareInput,
+        stop_on_error: true
+      },
+      true,
+      {}
+    ).done;
+
+    // Step 2: Push input to StringIO
+    //         Encode input to base64 (to avoid escape problem)
+    //         Divide input to chunks (1MB)
+    const CHUNK_SIZE = 1000000;
+    for (let i = 0; i < input.length; i += CHUNK_SIZE) {
+      const chunk = input.slice(i, i + CHUNK_SIZE);
+      const uint8array = new TextEncoder().encode(chunk);
+      const base64EncodedInput = bytesToBase64(uint8array);
+      const pushInput = `
+JUDGE_INPUT_STRING_IO.write(base64.b64decode('${base64EncodedInput}').decode("utf-8"))
+`;
+      await kernel.requestExecute(
+        {
+          code: pushInput,
+          stop_on_error: true
+        },
+        true,
+        {}
+      ).done;
+    }
+
+    // Step 3: Seek to the beginning of StringIO
+    //         This code is prepended to the user code
+    const seekInput = `
+JUDGE_INPUT_STRING_IO.seek(0)
+`;
+
     const content: KernelMessage.IExecuteRequestMsg['content'] = {
-      code,
+      code: seekInput + code,
       stop_on_error: true,
       allow_stdin: true
     };
 
-    let inputLinesLeft: string[] = [];
-    if (problem.inputTransferType === 'one_line') {
-      inputLinesLeft = input.split(/\r?\n/);
-    } else {
-      inputLinesLeft = [input];
-    }
-
     const startTime = Date.now();
     const future = kernel.requestExecute(content, true, {});
-    future.onStdin = (
-      msg: KernelMessage.IStdinMessage<KernelMessage.StdinMessageType>
-    ) => {
-      if (msg.header.msg_type === 'input_request') {
-        const currentInputLine = inputLinesLeft.shift();
-        future.sendInputReply(
-          {
-            value: currentInputLine ?? '',
-            status: 'ok'
-          },
-          msg.header as IHeader<'input_request'>
-        );
-      }
-    };
 
     const result: IRunResult = { output: '', status: 'OK', cpuTime: 0 };
     future.onIOPub = (msg: KernelMessage.IIOPubMessage) => {
       const msgType = msg.header.msg_type;
 
       switch (msgType) {
         case 'stream': {
```

### Comparing `jupyterlab_judge-1.23.0rc0/src/widgets/JudgeProblemPanel.ts` & `jupyterlab_judge-1.24.1/src/widgets/JudgeProblemPanel.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/widgets/JudgeSubmissionArea.tsx` & `jupyterlab_judge-1.24.1/src/widgets/JudgeSubmissionArea.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/src/widgets/JudgeTerminal.ts` & `jupyterlab_judge-1.24.1/src/widgets/JudgeTerminal.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/style/judgePanel.css` & `jupyterlab_judge-1.24.1/style/judgePanel.css`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
   padding: 20px;
   box-shadow: none;
   border-top: 0 none;
   border-bottom: 0 none;
   border-left: 0 none;
   border-right: 1px solid var(--jp-border-color0);
   min-width: 200px;
+  height: 100%;
   overflow-y: auto;
 }
 
 /*
 min-width has no effect on the right panel, so we need to set it on the children.
 .jp-JudgePanel-rightPanel {
   min-width: 500px;
```

### Comparing `jupyterlab_judge-1.23.0rc0/style/judgeTerminal.css` & `jupyterlab_judge-1.24.1/style/judgeTerminal.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/ui-tests/README.md` & `jupyterlab_judge-1.24.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/ui-tests/tests/jupyterlab_judge.spec.ts` & `jupyterlab_judge-1.24.1/ui-tests/tests/jupyterlab_judge.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/.gitignore` & `jupyterlab_judge-1.24.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/LICENSE` & `jupyterlab_judge-1.24.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/README.md` & `jupyterlab_judge-1.24.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/pyproject.toml` & `jupyterlab_judge-1.24.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.23.0rc0/PKG-INFO` & `jupyterlab_judge-1.24.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyterlab_judge
-Version: 1.23.0rc0
+Version: 1.24.1
+Dynamic: Keywords
 Summary: A simple online judge for Jupyter Lab.
 Project-URL: Homepage, https://github.com/team-monolith-product/jupyterlab-judge
 Project-URL: Bug Tracker, https://github.com/team-monolith-product/jupyterlab-judge/issues
 Project-URL: Repository, https://github.com/team-monolith-product/jupyterlab-judge.git
 Author-email: ChangHwan Lee <lch@team-mono.com>
 License: BSD 3-Clause License
```

