# Comparing `tmp/neon-skill-fallback_wolfram_alpha-2.0.0.tar.gz` & `tmp/neon-skill-fallback_wolfram_alpha-2.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-fallback_wolfram_alpha-2.0.0.tar", last modified: Tue Apr  2 19:42:03 2024, max compression
+gzip compressed data, was "neon-skill-fallback_wolfram_alpha-2.0.1a1.tar", last modified: Fri Apr  5 00:13:36 2024, max compression
```

## Comparing `neon-skill-fallback_wolfram_alpha-2.0.0.tar` & `neon-skill-fallback_wolfram_alpha-2.0.1a1.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.691199 neon-skill-fallback_wolfram_alpha-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-02 19:42:03.691199 neon-skill-fallback_wolfram_alpha-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.663198 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.671198 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ca-es/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ca-es/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ca-es/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ca-es/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ca-es/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.671198 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/cs-cz/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/cs-cz/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/cs-cz/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/cs-cz/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/cs-cz/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.671198 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/da-dk/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/da-dk/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/da-dk/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/da-dk/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/da-dk/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.671198 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/de-de/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/de-de/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/de-de/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/de-de/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/de-de/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.671198 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/el-gr/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/el-gr/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/el-gr/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/el-gr/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/el-gr/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/el-gr/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.675198 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/en-us/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/en-us/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/en-us/no.email.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/en-us/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/en-us/no.response.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/en-us/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/en-us/response.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/en-us/sent.email.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/en-us/wait.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.675198 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/es-es/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/es-es/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/es-es/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/es-es/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/es-es/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.675198 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/es-lm/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/es-lm/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/es-lm/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/es-lm/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/es-lm/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/es-lm/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.675198 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/fr-fr/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/fr-fr/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/fr-fr/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/fr-fr/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/fr-fr/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.675198 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/gl-es/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/gl-es/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/gl-es/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/gl-es/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/gl-es/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/gl-es/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.675198 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/it-it/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/it-it/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/it-it/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/it-it/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/it-it/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.679199 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/kab-dz/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/kab-dz/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/kab-dz/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/kab-dz/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/kab-dz/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/kab-dz/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.679199 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/nl-nl/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/nl-nl/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/nl-nl/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/nl-nl/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/nl-nl/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.679199 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/pl-pl/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/pl-pl/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/pl-pl/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/pl-pl/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/pl-pl/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.679199 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/pt-br/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/pt-br/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/pt-br/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/pt-br/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/pt-br/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.679199 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ro-ro/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ro-ro/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ro-ro/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ro-ro/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ro-ro/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.679199 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ru-ru/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ru-ru/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ru-ru/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ru-ru/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/ru-ru/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/sv-se/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/sv-se/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/sv-se/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/sv-se/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/dialog/sv-se/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/neon_skill_fallback_wolfram_alpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-02 19:42:03.000000 neon-skill-fallback_wolfram_alpha-2.0.0/neon_skill_fallback_wolfram_alpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-04-02 19:42:03.000000 neon-skill-fallback_wolfram_alpha-2.0.0/neon_skill_fallback_wolfram_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:42:03.000000 neon-skill-fallback_wolfram_alpha-2.0.0/neon_skill_fallback_wolfram_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 19:42:03.000000 neon-skill-fallback_wolfram_alpha-2.0.0/neon_skill_fallback_wolfram_alpha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-02 19:42:03.000000 neon-skill-fallback_wolfram_alpha-2.0.0/neon_skill_fallback_wolfram_alpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 19:42:03.000000 neon-skill-fallback_wolfram_alpha-2.0.0/neon_skill_fallback_wolfram_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.667198 neon-skill-fallback_wolfram_alpha-2.0.0/regex/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/ca-es/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/cs-cz/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/da-dk/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/de-de/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/el-gr/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/el-gr/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/en-us/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/es-es/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/es-lm/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/es-lm/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/fr-fr/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/gl-es/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/gl-es/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/it-it/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/kab-dz/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/kab-dz/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/nl-nl/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/pl-dz/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/pl-dz/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/pl-pl/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/pt-br/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/ro-ro/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/ru-ru/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.683199 neon-skill-fallback_wolfram_alpha-2.0.0/regex/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/regex/sv-se/list.rx
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:42:03.691199 neon-skill-fallback_wolfram_alpha-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/skill.json
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.667198 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/ca-es/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/ca-es/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/cs-cz/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/cs-cz/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/da-dk/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/da-dk/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/de-de/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/de-de/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/el-gr/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/el-gr/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/el-gr/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/en-us/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/en-us/Request.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/en-us/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/es-es/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/es-es/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/es-lm/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/es-lm/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/es-lm/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/fr-fr/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/fr-fr/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/gl-es/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/gl-es/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/gl-es/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/it-it/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/it-it/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/kab-dz/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/kab-dz/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/kab-dz/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/nl-nl/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/nl-nl/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/pl-pl/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/pl-pl/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.687199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/pt-br/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/pt-br/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.691199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/ro-ro/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/ro-ro/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.691199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/ru-ru/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/ru-ru/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:42:03.691199 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/sv-se/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 19:41:59.000000 neon-skill-fallback_wolfram_alpha-2.0.0/vocab/sv-se/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.737174 neon-skill-fallback_wolfram_alpha-2.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-05 00:13:36.737174 neon-skill-fallback_wolfram_alpha-2.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10055 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.709174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.713174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ca-es/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ca-es/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ca-es/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ca-es/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ca-es/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.713174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/cs-cz/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/cs-cz/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/cs-cz/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/cs-cz/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/cs-cz/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.713174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/da-dk/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/da-dk/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/da-dk/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/da-dk/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/da-dk/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.717174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/de-de/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/de-de/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/de-de/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/de-de/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/de-de/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.717174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/el-gr/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/el-gr/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/el-gr/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/el-gr/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/el-gr/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.717174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/en-us/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/en-us/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/en-us/no.email.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/en-us/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/en-us/no.response.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/en-us/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/en-us/response.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/en-us/sent.email.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/en-us/wait.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.717174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/es-es/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/es-es/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/es-es/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/es-es/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/es-es/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.721174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/es-lm/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/es-lm/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/es-lm/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/es-lm/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/es-lm/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/es-lm/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.721174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/fr-fr/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/fr-fr/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/fr-fr/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/fr-fr/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/fr-fr/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.721174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/gl-es/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/gl-es/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/gl-es/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/gl-es/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/gl-es/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.721174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/it-it/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/it-it/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/it-it/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/it-it/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/it-it/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.721174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/kab-dz/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/kab-dz/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/kab-dz/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/kab-dz/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/kab-dz/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/kab-dz/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.721174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/nl-nl/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/nl-nl/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/nl-nl/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/nl-nl/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/nl-nl/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.725174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/pl-pl/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/pl-pl/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/pl-pl/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/pl-pl/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/pl-pl/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.725174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/pt-br/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/pt-br/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/pt-br/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/pt-br/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/pt-br/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.725174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ro-ro/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ro-ro/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ro-ro/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ro-ro/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ro-ro/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.725174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ru-ru/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ru-ru/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ru-ru/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ru-ru/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/ru-ru/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.725174 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/sv-se/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/sv-se/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/sv-se/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/sv-se/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/dialog/sv-se/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/neon_skill_fallback_wolfram_alpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-05 00:13:36.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/neon_skill_fallback_wolfram_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-04-05 00:13:36.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/neon_skill_fallback_wolfram_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:13:36.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/neon_skill_fallback_wolfram_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 00:13:36.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/neon_skill_fallback_wolfram_alpha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 00:13:36.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/neon_skill_fallback_wolfram_alpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 00:13:36.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/neon_skill_fallback_wolfram_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.709174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/ca-es/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/cs-cz/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/da-dk/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/de-de/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/el-gr/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/en-us/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/es-es/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/es-lm/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/es-lm/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/fr-fr/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/gl-es/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/it-it/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/kab-dz/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/kab-dz/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/nl-nl/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/pl-dz/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/pl-dz/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/pl-pl/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/pt-br/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/ro-ro/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/ru-ru/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/regex/sv-se/list.rx
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 00:13:36.737174 neon-skill-fallback_wolfram_alpha-2.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/skill.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.713174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/ca-es/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/ca-es/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.729174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/cs-cz/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/cs-cz/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.733174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/da-dk/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/da-dk/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.733174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/de-de/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/de-de/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.733174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/el-gr/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/el-gr/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.733174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/en-us/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/en-us/Request.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/en-us/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.733174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/es-es/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/es-es/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.733174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/es-lm/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/es-lm/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/es-lm/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.733174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/fr-fr/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/fr-fr/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.733174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/gl-es/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/gl-es/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.733174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/it-it/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/it-it/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.733174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/kab-dz/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/kab-dz/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/kab-dz/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.733174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/nl-nl/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/nl-nl/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.733174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/pl-pl/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/pl-pl/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.733174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/pt-br/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/pt-br/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.737174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/ro-ro/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/ro-ro/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.737174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/ru-ru/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/ru-ru/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:13:36.737174 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/sv-se/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 00:13:30.000000 neon-skill-fallback_wolfram_alpha-2.0.1a1/vocab/sv-se/Source.voc
```

### Comparing `neon-skill-fallback_wolfram_alpha-2.0.0/LICENSE` & `neon-skill-fallback_wolfram_alpha-2.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_wolfram_alpha-2.0.0/LICENSE.md` & `neon-skill-fallback_wolfram_alpha-2.0.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_wolfram_alpha-2.0.0/PKG-INFO` & `neon-skill-fallback_wolfram_alpha-2.0.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-fallback_wolfram_alpha
-Version: 2.0.0
+Version: 2.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-fallback_wolfram_alpha
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-fallback_wolfram_alpha-2.0.0/README.md` & `neon-skill-fallback_wolfram_alpha-2.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_wolfram_alpha-2.0.0/__init__.py` & `neon-skill-fallback_wolfram_alpha-2.0.1a1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,18 +145,17 @@
 
     def CQS_action(self, phrase, data):
         """ If selected prepare to send sources. """
         if data:
             LOG.info('Setting information for source')
             user = data['user']
             self.queries[user] = data["query"]
-            if self.gui_enabled:
-                url = 'https://www.wolframalpha.com/input?i=' + \
-                      data["query"].replace(' ', '+')
-                self.gui.show_url(url)
+            url = 'https://www.wolframalpha.com/input?i=' + \
+                  data["query"].replace(' ', '+')
+            self.gui.show_url(url)
 
     def handle_get_sources(self, message):
         user = get_message_user(message)
         if user in self.queries.keys():
             last_query = self.queries[user]
             preference_user = get_user_prefs(message)["user"]
             email_addr = preference_user["email"]
@@ -173,18 +172,14 @@
                 self.speak_dialog("sent.email", {"email": email_addr},
                                   private=True)
             else:
                 self.speak_dialog("no.email", private=True)
         else:
             self.speak_dialog("no.info.to.send", private=True)
 
-    def stop(self):
-        if self.gui_enabled:
-            self.gui.clear()
-
     def _query_wolfram(self, utterance, message) -> tuple:
         utterance = normalize(utterance, remove_articles=False)
         parsed_question = self.question_parser.parse(utterance)
         LOG.debug(parsed_question)
         if not parsed_question:
             return None, None
```

### Comparing `neon-skill-fallback_wolfram_alpha-2.0.0/neon_skill_fallback_wolfram_alpha.egg-info/PKG-INFO` & `neon-skill-fallback_wolfram_alpha-2.0.1a1/neon_skill_fallback_wolfram_alpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-fallback-wolfram-alpha
-Version: 2.0.0
+Version: 2.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-fallback_wolfram_alpha
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-fallback_wolfram_alpha-2.0.0/neon_skill_fallback_wolfram_alpha.egg-info/SOURCES.txt` & `neon-skill-fallback_wolfram_alpha-2.0.1a1/neon_skill_fallback_wolfram_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_wolfram_alpha-2.0.0/setup.py` & `neon-skill-fallback_wolfram_alpha-2.0.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_wolfram_alpha-2.0.0/skill.json` & `neon-skill-fallback_wolfram_alpha-2.0.1a1/skill.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992424242424243%*

 * *Differences: {"'requirements'": "{'python': {insert: [(3, 'ovos-workshop~=0.0.15')]}}"}*

```diff
@@ -28,14 +28,15 @@
         "arm"
     ],
     "requirements": {
         "python": [
             "adapt-parser>=0.5,<2.0",
             "neon-utils~=1.9",
             "ovos-utils~=0.0, >=0.0.28",
+            "ovos-workshop~=0.0.15",
             "requests>=2.13.0"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "General knowledge fallback handler based on [Wolfram Alpha](https://wolframalpha.com) services",
     "skillname": "skill-fallback_wolfram_alpha",
```

### Comparing `neon-skill-fallback_wolfram_alpha-2.0.0/version.py` & `neon-skill-fallback_wolfram_alpha-2.0.1a1/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.0.0"
+__version__ = "2.0.1a1"
```

