# Comparing `tmp/jupyter_ai-2.9.0.tar.gz` & `tmp/jupyter_ai-2.9.1.tar.gz`

## Comparing `jupyter_ai-2.9.0.tar` & `jupyter_ai-2.9.1.tar`

### file list

```diff
@@ -1,185 +1,185 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/.eslintignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/.eslintrc.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/.prettierrc
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/babel.config.js
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/install.json
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jest.config.js
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/package.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/project.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/setup.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/tsconfig.json
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/tsconfig.test.json
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter-config/nb-config/jupyter_ai.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter-config/server-config/jupyter_ai.json
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/_version.py
--rw-r--r--   0        0        0    15284 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/config_manager.py
--rw-r--r--   0        0        0    11154 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/extension.py
--rw-r--r--   0        0        0    13416 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/handlers.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/models.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/chat_handlers/__init__.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/chat_handlers/ask.py
--rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/chat_handlers/base.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/chat_handlers/clear.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/chat_handlers/default.py
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/chat_handlers/generate.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/chat_handlers/help.py
--rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/chat_handlers/learn.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/config/config_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/document_loaders/__init__.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/document_loaders/directory.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/document_loaders/splitter.py
--rw-r--r--   0        0        0     4562 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/package.json
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/00b26ac825e209505639.woff2
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/036d4e95149b69ff9bcc.woff2
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb5.ttf
--rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/08ce98e51b04d58945a3.ttf
--rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f979.woff2
--rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f.ttf
--rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8.woff2
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee5.woff
--rw-r--r--   0        0        0    11275 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/136.25db938f4dec1af075df.js
--rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c.ttf
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/1ae6bd7475590e97e7f1.woff
--rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf09.ttf
--rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8.ttf
--rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc.ttf
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/2014c523c3210bcc1666.woff
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js
--rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/30da91e84c893f875e25.woff
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/3398dd02302557a793f2.woff
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/341.bf295a98a382d909aca3.js
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/342.133afdc0cac64ea6f3b3.js
--rw-r--r--   0        0        0    37391 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/380.1d8633fd1460b6a300c6.js
--rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/3931dd81faed86ba021b.ttf
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/397.d17905aa3243f76edf83.js
--rw-r--r--   0        0        0     7588 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/500e04d54f0d51666332.ttf
--rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/51814d270d06ff0255db.woff2
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/527.fbb5737cced749a84de3.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/527.fbb5737cced749a84de3.js.LICENSE.txt
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/560.2fa7b4ae7a0d43e8eb1f.js
--rw-r--r--   0        0        0  1567983 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/598.4f92e467887ba95a5a14.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/598.4f92e467887ba95a5a14.js.LICENSE.txt
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/5d53e70ad607c2352162.woff2
--rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/5e28753be717dac97f55.woff
--rw-r--r--   0        0        0    35427 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/620.cf49ee12c0ebc3f9bdbd.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/620.cf49ee12c0ebc3f9bdbd.js.LICENSE.txt
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/643.86c5b64b2c003759c197.js
--rw-r--r--   0        0        0    11044 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/675.756cf111884ba023580a.js
--rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f.ttf
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec5.woff2
--rw-r--r--   0        0        0    21811 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/693.2c3da85cc10c904e2289.js
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/6ab6b62e9b62dae2c00d.woff
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/6b47c40166b6dbe21a5d.woff2
--rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/703.0ff36d6afd3dad9af47a.js
--rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/70ee1f64a20f2048c219.ttf
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/71d517d67827787cfabd.woff2
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/73d591271b1604960cb1.woff2
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/74444efd593c005e3f45.woff2
--rw-r--r--   0        0        0   467656 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/787.e4b10d337857bc144420.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/787.e4b10d337857bc144420.js.LICENSE.txt
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde.woff2
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/819.5cf2eced87f9df904298.js
--rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/850c0af5c2238497feba.woff
--rw-r--r--   0        0        0    92803 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/861.9c6afbfd5c181c7781b4.js
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/861.9c6afbfd5c181c7781b4.js.LICENSE.txt
--rw-r--r--   0        0        0    32061 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/864.76bba6e73ce66305b0b7.js
--rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/8a8d244581371912b8f3.woff
--rw-r--r--   0        0        0   273048 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/900.e5afa91e5717cd8b1f97.js
--rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/9163df9c7122432e6495.ttf
--rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ac.woff
--rw-r--r--   0        0        0  4112827 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/928.604addfd69ea7b34b76b.js
--rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8.ttf
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/97479ca6cce906abc961.woff2
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f4.woff2
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/99f9c6750b489c9462bf.woff
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124.woff
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/a4af7d414440a1c17908.woff2
--rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0d.ttf
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975a.woff
--rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9.woff2
--rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337.woff
--rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/c647367d1dd4e1624687.ttf
--rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1.woff
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/c943cc986384f59e86be.woff
--rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/d0332f52868370fd83ae.ttf
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/d04c54219f9eaec6d4d4.woff2
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd.woff
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8.woff2
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/de7701e42cf1f4cf0b76.woff2
--rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5a.woff
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc.woff2
--rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/ece03cfd83e22c212cde.woff
--rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c06.ttf
--rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c08.ttf
--rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5.woff
--rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d.ttf
--rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/f9377ab0271cda59af24.ttf
--rw-r--r--   0        0        0    12578 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/remoteEntry.48d67235106ea0e8e7c5.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/style.js
--rw-r--r--   0        0        0   110333 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/tests/__init__.py
--rw-r--r--   0        0        0    10962 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/tests/test_config_manager.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/tests/test_extension.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/tests/test_handlers.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/jupyter_ai/tests/__snapshots__/test_config_manager.ambr
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/schema/plugin.json
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/chat_handler.ts
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/handler.ts
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/icons.ts
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/index.ts
--rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/selection-watcher.ts
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/theme-provider.ts
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/utils.ts
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/chat-code-view.tsx
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/chat-input.tsx
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/chat-messages.tsx
--rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/chat-settings.tsx
--rw-r--r--   0        0        0     7117 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/chat.tsx
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/expandable-text-field.tsx
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/jl-theme-provider.tsx
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/scroll-container.tsx
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/select.tsx
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/mui-extras/async-icon-button.tsx
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/mui-extras/contrasting-tooltip.tsx
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/mui-extras/stacking-alert.tsx
--rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/settings/existing-api-keys.tsx
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/settings/minify.ts
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/settings/model-fields.tsx
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/settings/use-server-info.ts
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/settings/validator.ts
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/components/settings/__tests__/chat-settings.spec.ts
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/contexts/collaborators-context.tsx
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/contexts/selection-context.tsx
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/types/mui.d.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/types/svg.d.ts
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/widgets/chat-error.tsx
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/src/widgets/chat-sidebar.tsx
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/style/base.css
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/style/chat-settings.css
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/style/expandable-text-field.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/style/index.js
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/style/react-markdown.css
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/style/icons/chat.svg
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/style/icons/jupyternaut.svg
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   151924 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/ui-tests/tests/jupyter-ai.spec.ts
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/ui-tests/tests/helpers/AIHelper.ts
--rw-r--r--   0        0        0    16744 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/ui-tests/tests/jupyter-ai.spec.ts-snapshots/chat-welcome-message-linux.png
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/ui-tests/tests/jupyter-ai.spec.ts-snapshots/sidebar-linux.png
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/LICENSE
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/README.md
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/pyproject.toml
--rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 jupyter_ai-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/.eslintignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/.eslintrc.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/.prettierrc
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/babel.config.js
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/install.json
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jest.config.js
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/package.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/project.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/setup.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/tsconfig.json
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/tsconfig.test.json
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter-config/nb-config/jupyter_ai.json
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter-config/server-config/jupyter_ai.json
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/_version.py
+-rw-r--r--   0        0        0    15284 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/config_manager.py
+-rw-r--r--   0        0        0    11154 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/extension.py
+-rw-r--r--   0        0        0    13416 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/handlers.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/models.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/chat_handlers/__init__.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/chat_handlers/ask.py
+-rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/chat_handlers/base.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/chat_handlers/clear.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/chat_handlers/default.py
+-rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/chat_handlers/generate.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/chat_handlers/help.py
+-rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/chat_handlers/learn.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/config/config_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/document_loaders/__init__.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/document_loaders/directory.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/document_loaders/splitter.py
+-rw-r--r--   0        0        0     4562 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/package.json
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
+-rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/00b26ac825e209505639.woff2
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/036d4e95149b69ff9bcc.woff2
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb5.ttf
+-rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/08ce98e51b04d58945a3.ttf
+-rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/0cdd387c9590a1a9f979.woff2
+-rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f.ttf
+-rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/0f60d1b897938ec918c8.woff2
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee5.woff
+-rw-r--r--   0        0        0    11275 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/136.25db938f4dec1af075df.js
+-rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/138ac28d1663b3037e9c.ttf
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/1ae6bd7475590e97e7f1.woff
+-rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/1c67f068fea8bb09bf09.ttf
+-rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8.ttf
+-rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/1ece03f79f95277d57dc.ttf
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/2014c523c3210bcc1666.woff
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js
+-rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/30da91e84c893f875e25.woff
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/3398dd02302557a793f2.woff
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/341.bf295a98a382d909aca3.js
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/342.133afdc0cac64ea6f3b3.js
+-rw-r--r--   0        0        0    37391 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/380.1d8633fd1460b6a300c6.js
+-rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/3931dd81faed86ba021b.ttf
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/397.d17905aa3243f76edf83.js
+-rw-r--r--   0        0        0     7588 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/500e04d54f0d51666332.ttf
+-rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/51814d270d06ff0255db.woff2
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/527.fbb5737cced749a84de3.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/527.fbb5737cced749a84de3.js.LICENSE.txt
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/560.2fa7b4ae7a0d43e8eb1f.js
+-rw-r--r--   0        0        0  1567983 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/598.4f92e467887ba95a5a14.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/598.4f92e467887ba95a5a14.js.LICENSE.txt
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/5d53e70ad607c2352162.woff2
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/5e28753be717dac97f55.woff
+-rw-r--r--   0        0        0    35427 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/620.cf49ee12c0ebc3f9bdbd.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/620.cf49ee12c0ebc3f9bdbd.js.LICENSE.txt
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/643.86c5b64b2c003759c197.js
+-rw-r--r--   0        0        0    11044 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/675.756cf111884ba023580a.js
+-rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/68534840bcfdd2bffb6f.ttf
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/68e8c73ef42afd3ccec5.woff2
+-rw-r--r--   0        0        0    21811 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/693.2c3da85cc10c904e2289.js
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/6ab6b62e9b62dae2c00d.woff
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/6b47c40166b6dbe21a5d.woff2
+-rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/703.0ff36d6afd3dad9af47a.js
+-rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/70ee1f64a20f2048c219.ttf
+-rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/71d517d67827787cfabd.woff2
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/73d591271b1604960cb1.woff2
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/74444efd593c005e3f45.woff2
+-rw-r--r--   0        0        0   467656 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/787.e4b10d337857bc144420.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/787.e4b10d337857bc144420.js.LICENSE.txt
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde.woff2
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/819.5cf2eced87f9df904298.js
+-rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/850c0af5c2238497feba.woff
+-rw-r--r--   0        0        0    92803 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/861.9c6afbfd5c181c7781b4.js
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/861.9c6afbfd5c181c7781b4.js.LICENSE.txt
+-rw-r--r--   0        0        0    32061 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/864.76bba6e73ce66305b0b7.js
+-rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/8a8d244581371912b8f3.woff
+-rw-r--r--   0        0        0   273048 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/900.e5afa91e5717cd8b1f97.js
+-rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/9163df9c7122432e6495.ttf
+-rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/91ee67500cc0129aa0ac.woff
+-rw-r--r--   0        0        0  4112827 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/928.604addfd69ea7b34b76b.js
+-rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8.ttf
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/97479ca6cce906abc961.woff2
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/99cd42a3c072d918f2f4.woff2
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/99f9c6750b489c9462bf.woff
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/9be7ceb88004ab8ad124.woff
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/a4af7d414440a1c17908.woff2
+-rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/a6b2099fb555c60e3a0d.ttf
+-rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975a.woff
+-rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/c2342cd8b869e01752a9.woff2
+-rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337.woff
+-rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/c647367d1dd4e1624687.ttf
+-rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/c76c5d696297d51b9cb1.woff
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/c943cc986384f59e86be.woff
+-rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/d0332f52868370fd83ae.ttf
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/d04c54219f9eaec6d4d4.woff2
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd.woff
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8.woff2
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/de7701e42cf1f4cf0b76.woff2
+-rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5a.woff
+-rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/e99ae51144bf1232efcc.woff2
+-rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/ece03cfd83e22c212cde.woff
+-rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/ed0b74372feefcbb9c06.ttf
+-rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c08.ttf
+-rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5.woff
+-rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/f36ea897e19f4a2e571d.ttf
+-rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/f9377ab0271cda59af24.ttf
+-rw-r--r--   0        0        0    12578 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/remoteEntry.f6392b10c1a26f830995.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/style.js
+-rw-r--r--   0        0        0   110333 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/tests/__init__.py
+-rw-r--r--   0        0        0    10962 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/tests/test_config_manager.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/tests/test_extension.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/tests/test_handlers.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/jupyter_ai/tests/__snapshots__/test_config_manager.ambr
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/schema/plugin.json
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/chat_handler.ts
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/handler.ts
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/icons.ts
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/index.ts
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/selection-watcher.ts
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/theme-provider.ts
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/utils.ts
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/chat-code-view.tsx
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/chat-input.tsx
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/chat-messages.tsx
+-rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/chat-settings.tsx
+-rw-r--r--   0        0        0     7117 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/chat.tsx
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/expandable-text-field.tsx
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/jl-theme-provider.tsx
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/scroll-container.tsx
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/select.tsx
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/mui-extras/async-icon-button.tsx
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/mui-extras/contrasting-tooltip.tsx
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/mui-extras/stacking-alert.tsx
+-rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/settings/existing-api-keys.tsx
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/settings/minify.ts
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/settings/model-fields.tsx
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/settings/use-server-info.ts
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/settings/validator.ts
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/components/settings/__tests__/chat-settings.spec.ts
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/contexts/collaborators-context.tsx
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/contexts/selection-context.tsx
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/types/mui.d.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/types/svg.d.ts
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/widgets/chat-error.tsx
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/src/widgets/chat-sidebar.tsx
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/style/base.css
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/style/chat-settings.css
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/style/expandable-text-field.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/style/index.js
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/style/react-markdown.css
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/style/icons/chat.svg
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/style/icons/jupyternaut.svg
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   151924 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/ui-tests/tests/jupyter-ai.spec.ts
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/ui-tests/tests/helpers/AIHelper.ts
+-rw-r--r--   0        0        0    16744 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/ui-tests/tests/jupyter-ai.spec.ts-snapshots/chat-welcome-message-linux.png
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/ui-tests/tests/jupyter-ai.spec.ts-snapshots/sidebar-linux.png
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/LICENSE
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/README.md
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 jupyter_ai-2.9.1/PKG-INFO
```

### Comparing `jupyter_ai-2.9.0/.eslintrc.js` & `jupyter_ai-2.9.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/RELEASE.md` & `jupyter_ai-2.9.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jest.config.js` & `jupyter_ai-2.9.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/package.json` & `jupyter_ai-2.9.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'2.9.1'"}*

```diff
@@ -124,9 +124,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.9.0"
+    "version": "2.9.1"
 }
```

### Comparing `jupyter_ai-2.9.0/tsconfig.json` & `jupyter_ai-2.9.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/config_manager.py` & `jupyter_ai-2.9.1/jupyter_ai/config_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/extension.py` & `jupyter_ai-2.9.1/jupyter_ai/extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/handlers.py` & `jupyter_ai-2.9.1/jupyter_ai/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/models.py` & `jupyter_ai-2.9.1/jupyter_ai/models.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/chat_handlers/ask.py` & `jupyter_ai-2.9.1/jupyter_ai/chat_handlers/ask.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/chat_handlers/base.py` & `jupyter_ai-2.9.1/jupyter_ai/chat_handlers/base.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/chat_handlers/clear.py` & `jupyter_ai-2.9.1/jupyter_ai/chat_handlers/clear.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/chat_handlers/default.py` & `jupyter_ai-2.9.1/jupyter_ai/chat_handlers/default.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,26 +49,26 @@
         model_parameters = self.get_model_parameters(provider, provider_params)
         llm = provider(**provider_params, **model_parameters)
 
         if llm.is_chat_provider:
             prompt_template = ChatPromptTemplate.from_messages(
                 [
                     SystemMessagePromptTemplate.from_template(SYSTEM_PROMPT).format(
-                        provider_name=llm.name, local_model_id=llm.model_id
+                        provider_name=provider.name, local_model_id=llm.model_id
                     ),
                     MessagesPlaceholder(variable_name="history"),
                     HumanMessagePromptTemplate.from_template("{input}"),
                 ]
             )
             self.memory = ConversationBufferWindowMemory(return_messages=True, k=2)
         else:
             prompt_template = PromptTemplate(
                 input_variables=["history", "input"],
                 template=SYSTEM_PROMPT.format(
-                    provider_name=llm.name, local_model_id=llm.model_id
+                    provider_name=provider.name, local_model_id=llm.model_id
                 )
                 + "\n\n"
                 + DEFAULT_TEMPLATE,
             )
             self.memory = ConversationBufferWindowMemory(k=2)
 
         self.llm = llm
```

### Comparing `jupyter_ai-2.9.0/jupyter_ai/chat_handlers/generate.py` & `jupyter_ai-2.9.1/jupyter_ai/chat_handlers/generate.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/chat_handlers/help.py` & `jupyter_ai-2.9.1/jupyter_ai/chat_handlers/help.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/chat_handlers/learn.py` & `jupyter_ai-2.9.1/jupyter_ai/chat_handlers/learn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import argparse
 import json
 import os
-from typing import Any, Awaitable, Coroutine, List, Optional, Tuple
+from typing import Any, Coroutine, List, Optional, Tuple
 
 from dask.distributed import Client as DaskClient
-from jupyter_ai.config_manager import ConfigManager
 from jupyter_ai.document_loaders.directory import get_embeddings, split
 from jupyter_ai.document_loaders.splitter import ExtensionSplitter, NotebookSplitter
 from jupyter_ai.models import (
     DEFAULT_CHUNK_OVERLAP,
     DEFAULT_CHUNK_SIZE,
     HumanChatMessage,
     IndexedDir,
@@ -18,15 +17,15 @@
 from langchain.schema import BaseRetriever, Document
 from langchain.text_splitter import (
     LatexTextSplitter,
     MarkdownTextSplitter,
     PythonCodeTextSplitter,
     RecursiveCharacterTextSplitter,
 )
-from langchain.vectorstores import FAISS
+from langchain_community.vectorstores import FAISS
 
 from .base import BaseChatHandler, SlashCommandRoutingType
 
 INDEX_SAVE_DIR = os.path.join(jupyter_data_dir(), "jupyter_ai", "indices")
 METADATA_SAVE_PATH = os.path.join(INDEX_SAVE_DIR, "metadata.json")
 
 
@@ -137,15 +136,15 @@
         message = f"""I can answer questions from docs in these directories:
         {dir_list}"""
         return message
 
     async def learn_dir(
         self, path: str, chunk_size: int, chunk_overlap: int, all_files: bool
     ):
-        dask_client = await self.dask_client_future
+        dask_client: DaskClient = await self.dask_client_future
         splitter_kwargs = {"chunk_size": chunk_size, "chunk_overlap": chunk_overlap}
         splitters = {
             ".py": PythonCodeTextSplitter(**splitter_kwargs),
             ".md": MarkdownTextSplitter(**splitter_kwargs),
             ".tex": LatexTextSplitter(**splitter_kwargs),
             ".ipynb": NotebookSplitter(**splitter_kwargs),
         }
```

### Comparing `jupyter_ai-2.9.0/jupyter_ai/config/config_schema.json` & `jupyter_ai-2.9.1/jupyter_ai/config/config_schema.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/document_loaders/directory.py` & `jupyter_ai-2.9.1/jupyter_ai/document_loaders/directory.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/document_loaders/splitter.py` & `jupyter_ai-2.9.1/jupyter_ai/document_loaders/splitter.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/package.json` & `jupyter_ai-2.9.1/jupyter_ai/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745833333333334%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.f6392b10c1a26f830995.js'}}",*

 * * "'version'": "'2.9.1'"}*

```diff
@@ -61,15 +61,15 @@
         "schema/*.json",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-ai",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.48d67235106ea0e8e7c5.js",
+            "load": "static/remoteEntry.f6392b10c1a26f830995.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_ai"
                 },
@@ -129,9 +129,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.9.0"
+    "version": "2.9.1"
 }
```

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig` & `jupyter_ai-2.9.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'2.9.1'"}*

```diff
@@ -124,9 +124,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.9.0"
+    "version": "2.9.1"
 }
```

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json` & `jupyter_ai-2.9.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/00b26ac825e209505639.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/00b26ac825e209505639.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/036d4e95149b69ff9bcc.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/036d4e95149b69ff9bcc.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb5.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb5.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/08ce98e51b04d58945a3.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/08ce98e51b04d58945a3.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f979.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/0cdd387c9590a1a9f979.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/0f60d1b897938ec918c8.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee5.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee5.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/136.25db938f4dec1af075df.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/136.25db938f4dec1af075df.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/138ac28d1663b3037e9c.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/1ae6bd7475590e97e7f1.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/1ae6bd7475590e97e7f1.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf09.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/1c67f068fea8bb09bf09.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/1ece03f79f95277d57dc.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/2014c523c3210bcc1666.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/2014c523c3210bcc1666.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/30da91e84c893f875e25.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/30da91e84c893f875e25.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/3398dd02302557a793f2.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/3398dd02302557a793f2.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/341.bf295a98a382d909aca3.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/341.bf295a98a382d909aca3.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/342.133afdc0cac64ea6f3b3.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/342.133afdc0cac64ea6f3b3.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/380.1d8633fd1460b6a300c6.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/380.1d8633fd1460b6a300c6.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/3931dd81faed86ba021b.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/3931dd81faed86ba021b.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/397.d17905aa3243f76edf83.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/397.d17905aa3243f76edf83.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/500e04d54f0d51666332.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/500e04d54f0d51666332.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/51814d270d06ff0255db.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/51814d270d06ff0255db.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/527.fbb5737cced749a84de3.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/527.fbb5737cced749a84de3.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/598.4f92e467887ba95a5a14.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/598.4f92e467887ba95a5a14.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/5d53e70ad607c2352162.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/5d53e70ad607c2352162.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/5e28753be717dac97f55.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/5e28753be717dac97f55.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/620.cf49ee12c0ebc3f9bdbd.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/620.cf49ee12c0ebc3f9bdbd.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/643.86c5b64b2c003759c197.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/643.86c5b64b2c003759c197.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/675.756cf111884ba023580a.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/675.756cf111884ba023580a.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/68534840bcfdd2bffb6f.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec5.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/68e8c73ef42afd3ccec5.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/693.2c3da85cc10c904e2289.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/693.2c3da85cc10c904e2289.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/6ab6b62e9b62dae2c00d.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/6ab6b62e9b62dae2c00d.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/6b47c40166b6dbe21a5d.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/6b47c40166b6dbe21a5d.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/703.0ff36d6afd3dad9af47a.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/703.0ff36d6afd3dad9af47a.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/70ee1f64a20f2048c219.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/70ee1f64a20f2048c219.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/71d517d67827787cfabd.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/71d517d67827787cfabd.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/73d591271b1604960cb1.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/73d591271b1604960cb1.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/74444efd593c005e3f45.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/74444efd593c005e3f45.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/787.e4b10d337857bc144420.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/787.e4b10d337857bc144420.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/819.5cf2eced87f9df904298.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/819.5cf2eced87f9df904298.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/850c0af5c2238497feba.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/850c0af5c2238497feba.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/861.9c6afbfd5c181c7781b4.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/861.9c6afbfd5c181c7781b4.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/864.76bba6e73ce66305b0b7.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/864.76bba6e73ce66305b0b7.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/8a8d244581371912b8f3.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/8a8d244581371912b8f3.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/900.e5afa91e5717cd8b1f97.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/900.e5afa91e5717cd8b1f97.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/9163df9c7122432e6495.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/9163df9c7122432e6495.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ac.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/91ee67500cc0129aa0ac.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/928.604addfd69ea7b34b76b.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/928.604addfd69ea7b34b76b.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/97479ca6cce906abc961.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/97479ca6cce906abc961.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f4.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/99cd42a3c072d918f2f4.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/99f9c6750b489c9462bf.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/99f9c6750b489c9462bf.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/9be7ceb88004ab8ad124.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/a4af7d414440a1c17908.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/a4af7d414440a1c17908.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0d.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/a6b2099fb555c60e3a0d.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975a.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975a.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/c2342cd8b869e01752a9.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/c647367d1dd4e1624687.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/c647367d1dd4e1624687.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/c76c5d696297d51b9cb1.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/c943cc986384f59e86be.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/c943cc986384f59e86be.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/d0332f52868370fd83ae.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/d0332f52868370fd83ae.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/d04c54219f9eaec6d4d4.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/d04c54219f9eaec6d4d4.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/de7701e42cf1f4cf0b76.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/de7701e42cf1f4cf0b76.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5a.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5a.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc.woff2` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/e99ae51144bf1232efcc.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/ece03cfd83e22c212cde.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/ece03cfd83e22c212cde.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c06.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/ed0b74372feefcbb9c06.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c08.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c08.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5.woff` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/f36ea897e19f4a2e571d.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/f9377ab0271cda59af24.ttf` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/f9377ab0271cda59af24.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/remoteEntry.48d67235106ea0e8e7c5.js` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/remoteEntry.f6392b10c1a26f830995.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -170,15 +170,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     d = [];
-                return "default" === t && (l("@emotion/react", "11.11.1", (() => Promise.all([x.e(296), x.e(527), x.e(29), x.e(342)]).then((() => () => x(26527))))), l("@emotion/styled", "11.11.0", (() => Promise.all([x.e(675), x.e(29), x.e(564), x.e(407), x.e(560)]).then((() => () => x(52675))))), l("@jupyter-ai/core", "2.9.0", (() => Promise.all([x.e(620), x.e(341), x.e(380), x.e(29), x.e(963), x.e(132), x.e(864)]).then((() => () => x(30864))))), l("@jupyter/collaboration", "1.0.1", (() => Promise.all([x.e(136), x.e(29), x.e(648), x.e(132)]).then((() => () => x(29136))))), l("@mui/icons-material", "5.14.1", (() => Promise.all([x.e(620), x.e(928), x.e(29), x.e(963)]).then((() => () => x(13928))))), l("@mui/material", "5.14.2", (() => Promise.all([x.e(296), x.e(620), x.e(787), x.e(341), x.e(29), x.e(564), x.e(963), x.e(704)]).then((() => () => x(34787))))), l("react-markdown", "8.0.7", (() => Promise.all([x.e(693), x.e(861), x.e(29)]).then((() => () => x(81861))))), l("react-syntax-highlighter", "15.5.0", (() => Promise.all([x.e(598), x.e(29), x.e(397)]).then((() => () => x(95598))))), l("rehype-katex", "6.0.3", (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))), l("remark-math", "5.1.1", (() => x.e(703).then((() => () => x(7703)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@emotion/react", "11.11.1", (() => Promise.all([x.e(296), x.e(527), x.e(29), x.e(342)]).then((() => () => x(26527))))), l("@emotion/styled", "11.11.0", (() => Promise.all([x.e(675), x.e(29), x.e(564), x.e(407), x.e(560)]).then((() => () => x(52675))))), l("@jupyter-ai/core", "2.9.1", (() => Promise.all([x.e(620), x.e(341), x.e(380), x.e(29), x.e(963), x.e(132), x.e(864)]).then((() => () => x(30864))))), l("@jupyter/collaboration", "1.0.1", (() => Promise.all([x.e(136), x.e(29), x.e(648), x.e(132)]).then((() => () => x(29136))))), l("@mui/icons-material", "5.14.1", (() => Promise.all([x.e(620), x.e(928), x.e(29), x.e(963)]).then((() => () => x(13928))))), l("@mui/material", "5.14.2", (() => Promise.all([x.e(296), x.e(620), x.e(787), x.e(341), x.e(29), x.e(564), x.e(963), x.e(704)]).then((() => () => x(34787))))), l("react-markdown", "8.0.7", (() => Promise.all([x.e(693), x.e(861), x.e(29)]).then((() => () => x(81861))))), l("react-syntax-highlighter", "15.5.0", (() => Promise.all([x.e(598), x.e(29), x.e(397)]).then((() => () => x(95598))))), l("rehype-katex", "6.0.3", (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))), l("remark-math", "5.1.1", (() => x.e(703).then((() => () => x(7703)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyter_ai-2.9.0/jupyter_ai/labextension/static/third-party-licenses.json` & `jupyter_ai-2.9.1/jupyter_ai/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/tests/test_config_manager.py` & `jupyter_ai-2.9.1/jupyter_ai/tests/test_config_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/jupyter_ai/tests/test_extension.py` & `jupyter_ai-2.9.1/jupyter_ai/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/schema/plugin.json` & `jupyter_ai-2.9.1/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/chat_handler.ts` & `jupyter_ai-2.9.1/src/chat_handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/handler.ts` & `jupyter_ai-2.9.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/icons.ts` & `jupyter_ai-2.9.1/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/index.ts` & `jupyter_ai-2.9.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/selection-watcher.ts` & `jupyter_ai-2.9.1/src/selection-watcher.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/theme-provider.ts` & `jupyter_ai-2.9.1/src/theme-provider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/utils.ts` & `jupyter_ai-2.9.1/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/chat-code-view.tsx` & `jupyter_ai-2.9.1/src/components/chat-code-view.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/chat-input.tsx` & `jupyter_ai-2.9.1/src/components/chat-input.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/chat-messages.tsx` & `jupyter_ai-2.9.1/src/components/chat-messages.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/chat-settings.tsx` & `jupyter_ai-2.9.1/src/components/chat-settings.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/chat.tsx` & `jupyter_ai-2.9.1/src/components/chat.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/expandable-text-field.tsx` & `jupyter_ai-2.9.1/src/components/expandable-text-field.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/jl-theme-provider.tsx` & `jupyter_ai-2.9.1/src/components/jl-theme-provider.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/scroll-container.tsx` & `jupyter_ai-2.9.1/src/components/scroll-container.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/select.tsx` & `jupyter_ai-2.9.1/src/components/select.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/mui-extras/async-icon-button.tsx` & `jupyter_ai-2.9.1/src/components/mui-extras/async-icon-button.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/mui-extras/contrasting-tooltip.tsx` & `jupyter_ai-2.9.1/src/components/mui-extras/contrasting-tooltip.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/mui-extras/stacking-alert.tsx` & `jupyter_ai-2.9.1/src/components/mui-extras/stacking-alert.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/settings/existing-api-keys.tsx` & `jupyter_ai-2.9.1/src/components/settings/existing-api-keys.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/settings/minify.ts` & `jupyter_ai-2.9.1/src/components/settings/minify.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/settings/model-fields.tsx` & `jupyter_ai-2.9.1/src/components/settings/model-fields.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/settings/use-server-info.ts` & `jupyter_ai-2.9.1/src/components/settings/use-server-info.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/components/settings/__tests__/chat-settings.spec.ts` & `jupyter_ai-2.9.1/src/components/settings/__tests__/chat-settings.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/contexts/collaborators-context.tsx` & `jupyter_ai-2.9.1/src/contexts/collaborators-context.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/contexts/selection-context.tsx` & `jupyter_ai-2.9.1/src/contexts/selection-context.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/widgets/chat-error.tsx` & `jupyter_ai-2.9.1/src/widgets/chat-error.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/src/widgets/chat-sidebar.tsx` & `jupyter_ai-2.9.1/src/widgets/chat-sidebar.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/style/icons/jupyternaut.svg` & `jupyter_ai-2.9.1/style/icons/jupyternaut.svg`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/ui-tests/README.md` & `jupyter_ai-2.9.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/ui-tests/yarn.lock` & `jupyter_ai-2.9.1/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/ui-tests/tests/jupyter-ai.spec.ts` & `jupyter_ai-2.9.1/ui-tests/tests/jupyter-ai.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/ui-tests/tests/helpers/AIHelper.ts` & `jupyter_ai-2.9.1/ui-tests/tests/helpers/AIHelper.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/ui-tests/tests/jupyter-ai.spec.ts-snapshots/chat-welcome-message-linux.png` & `jupyter_ai-2.9.1/ui-tests/tests/jupyter-ai.spec.ts-snapshots/chat-welcome-message-linux.png`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/ui-tests/tests/jupyter-ai.spec.ts-snapshots/sidebar-linux.png` & `jupyter_ai-2.9.1/ui-tests/tests/jupyter-ai.spec.ts-snapshots/sidebar-linux.png`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/.gitignore` & `jupyter_ai-2.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/LICENSE` & `jupyter_ai-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/README.md` & `jupyter_ai-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.9.0/pyproject.toml` & `jupyter_ai-2.9.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,14 @@
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "jupyter_server>=1.6,<3",
     "jupyterlab~=4.0",
     "aiosqlite>=0.18",
     "importlib_metadata>=5.2.0",
-    "langchain==0.0.350",
-    "langchain-core>=0.1.0,<0.1.4",
     "tiktoken",                  # required for OpenAIEmbeddings
     "jupyter_ai_magics",
     "dask[distributed]",
     "faiss-cpu",                 # Not distributed by official repo
     "typing_extensions>=4.5.0",
     "traitlets>=5.0",
     "deepmerge>=1.0",
```

### Comparing `jupyter_ai-2.9.0/PKG-INFO` & `jupyter_ai-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai
-Version: 2.9.0
+Version: 2.9.1
 Summary: A generative AI extension for JupyterLab
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -53,16 +53,14 @@
 Requires-Dist: dask[distributed]
 Requires-Dist: deepmerge>=1.0
 Requires-Dist: faiss-cpu
 Requires-Dist: importlib-metadata>=5.2.0
 Requires-Dist: jupyter-ai-magics
 Requires-Dist: jupyter-server<3,>=1.6
 Requires-Dist: jupyterlab~=4.0
-Requires-Dist: langchain-core<0.1.4,>=0.1.0
-Requires-Dist: langchain==0.0.350
 Requires-Dist: tiktoken
 Requires-Dist: traitlets>=5.0
 Requires-Dist: typing-extensions>=4.5.0
 Provides-Extra: all
 Requires-Dist: jupyter-ai-magics[all]; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: jupyter-ai-magics[dev]; extra == 'dev'
```

