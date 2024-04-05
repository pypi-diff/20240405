# Comparing `tmp/linktools-0.8.3rc0.tar.gz` & `tmp/linktools-0.8.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktools-0.8.3rc0.tar", last modified: Wed Apr  3 08:10:39 2024, max compression
+gzip compressed data, was "linktools-0.8.3rc1.tar", last modified: Fri Apr  5 13:46:49 2024, max compression
```

## Comparing `linktools-0.8.3rc0.tar` & `linktools-0.8.3rc1.tar`

### file list

```diff
@@ -1,129 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.478895 linktools-0.8.3rc0/
--rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    34580 2024-04-03 08:10:39.478895 linktools-0.8.3rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32666 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:10:39.478895 linktools-0.8.3rc0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.454895 linktools-0.8.3rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.458895 linktools-0.8.3rc0/src/linktools/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21599 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/_environ.py
--rw-r--r--   0 runner    (1001) docker     (127)    18049 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.458895 linktools-0.8.3rc0/src/linktools/android/
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/android/adb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/android/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.462895 linktools-0.8.3rc0/src/linktools/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-04-03 08:10:23.000000 linktools-0.8.3rc0/src/linktools/assets/android-tools.apk
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-03 08:10:23.000000 linktools-0.8.3rc0/src/linktools/assets/android-tools.json
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/chrome-driver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.454895 linktools-0.8.3rc0/src/linktools/assets/containers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.462895 linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/http.conf
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/https.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.462895 linktools-0.8.3rc0/src/linktools/assets/containers/110-portainer/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/110-portainer/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/110-portainer/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/110-portainer/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.462895 linktools-0.8.3rc0/src/linktools/assets/containers/120-flare/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/120-flare/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/120-flare/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/containers/120-flare/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/fake_useragent.json
--rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-04-03 08:08:17.000000 linktools-0.8.3rc0/src/linktools/assets/frida.js
--rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-04-03 08:08:17.000000 linktools-0.8.3rc0/src/linktools/assets/frida.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.454895 linktools-0.8.3rc0/src/linktools/assets/objection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.462895 linktools-0.8.3rc0/src/linktools/assets/objection/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/assets/objection/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12251 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools/assets/tools.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.466895 linktools-0.8.3rc0/src/linktools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    30240 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.466895 linktools-0.8.3rc0/src/linktools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.466895 linktools-0.8.3rc0/src/linktools/cli/commands/android/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/adb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15337 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/debug.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4914 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/objection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/pidcat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/android/top.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.466895 linktools-0.8.3rc0/src/linktools/cli/commands/common/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/common/cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/common/cntr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/common/env.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/common/grep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/common/shell.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4118 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/common/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.470895 linktools-0.8.3rc0/src/linktools/cli/commands/ios/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/ios/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/ios/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/ios/objection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/ios/scp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/commands/ios/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/cli/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.470895 linktools-0.8.3rc0/src/linktools/container/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15359 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/container/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    21272 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/container/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/container/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.470895 linktools-0.8.3rc0/src/linktools/frida/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/frida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/frida/android.py
--rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/frida/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/frida/ios.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/frida/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/frida/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.470895 linktools-0.8.3rc0/src/linktools/ida/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/ida/ida.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.470895 linktools-0.8.3rc0/src/linktools/ios/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/reactor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.470895 linktools-0.8.3rc0/src/linktools/references/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.474895 linktools-0.8.3rc0/src/linktools/references/fake_useragent/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/references/fake_useragent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/references/fake_useragent/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/references/fake_useragent/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/references/fake_useragent/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/references/fake_useragent/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/references/fake_useragent/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/rich.py
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.474895 linktools-0.8.3rc0/src/linktools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/utils/_lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/utils/_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/utils/_subprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17283 2024-04-03 08:08:05.000000 linktools-0.8.3rc0/src/linktools/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:10:39.474895 linktools-0.8.3rc0/src/linktools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    34580 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 08:10:39.000000 linktools-0.8.3rc0/src/linktools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.452102 linktools-0.8.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35093 2024-04-05 13:46:49.448102 linktools-0.8.3rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33179 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:46:49.452102 linktools-0.8.3rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.424102 linktools-0.8.3rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.432102 linktools-0.8.3rc1/src/linktools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/_environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.432102 linktools-0.8.3rc1/src/linktools/android/
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/android/adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/android/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.436102 linktools-0.8.3rc1/src/linktools/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-04-05 13:46:39.000000 linktools-0.8.3rc1/src/linktools/assets/android-tools.apk
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-05 13:46:39.000000 linktools-0.8.3rc1/src/linktools/assets/android-tools.json
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/chrome-driver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.428102 linktools-0.8.3rc1/src/linktools/assets/containers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.436102 linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/dnsapi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/http.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/https.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.436102 linktools-0.8.3rc1/src/linktools/assets/containers/110-portainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/110-portainer/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/110-portainer/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/110-portainer/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.436102 linktools-0.8.3rc1/src/linktools/assets/containers/120-flare/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/120-flare/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/120-flare/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/containers/120-flare/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/fake_useragent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    51432 2024-04-05 13:44:38.000000 linktools-0.8.3rc1/src/linktools/assets/frida.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-04-05 13:44:38.000000 linktools-0.8.3rc1/src/linktools/assets/frida.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.428102 linktools-0.8.3rc1/src/linktools/assets/objection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.436102 linktools-0.8.3rc1/src/linktools/assets/objection/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/assets/objection/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools/assets/tools.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.436102 linktools-0.8.3rc1/src/linktools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30240 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.436102 linktools-0.8.3rc1/src/linktools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.440102 linktools-0.8.3rc1/src/linktools/cli/commands/android/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/adb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15337 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/debug.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4914 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/objection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/pidcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/android/top.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.440102 linktools-0.8.3rc1/src/linktools/cli/commands/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/common/cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/common/cntr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/common/env.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/common/grep.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4118 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/common/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.440102 linktools-0.8.3rc1/src/linktools/cli/commands/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/ios/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/ios/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/ios/objection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/ios/scp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/commands/ios/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/cli/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.444102 linktools-0.8.3rc1/src/linktools/container/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16099 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/container/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21176 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/container/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/container/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.444102 linktools-0.8.3rc1/src/linktools/frida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/frida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/frida/android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/frida/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/frida/ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/frida/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/frida/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.444102 linktools-0.8.3rc1/src/linktools/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/ida/ida.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.444102 linktools-0.8.3rc1/src/linktools/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/reactor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.444102 linktools-0.8.3rc1/src/linktools/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.444102 linktools-0.8.3rc1/src/linktools/references/fake_useragent/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/references/fake_useragent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/references/fake_useragent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/references/fake_useragent/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/references/fake_useragent/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/references/fake_useragent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/references/fake_useragent/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.448102 linktools-0.8.3rc1/src/linktools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/utils/_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/utils/_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/utils/_subprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18061 2024-04-05 13:44:31.000000 linktools-0.8.3rc1/src/linktools/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:46:49.448102 linktools-0.8.3rc1/src/linktools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35093 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 13:46:49.000000 linktools-0.8.3rc1/src/linktools.egg-info/top_level.txt
```

### Comparing `linktools-0.8.3rc0/LICENSE` & `linktools-0.8.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/PKG-INFO` & `linktools-0.8.3rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.3rc0
+Version: 0.8.3rc1
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -102,34 +102,78 @@
 ├── 📖 at: Android scripts
 │   ├── 👉 adb: Adb supports managing multiple android devices
 │   ├── 👉 agent: Debug android-tools.apk
 │   ├── 👉 app: Fetch application info
 │   ├── 👉 debug: Debug app by jdb
 │   ├── 👉 frida: Easy to use frida (require Android device rooted)
 │   ├── 👉 info: Fetch device information
-│   ├── 👉 intent: Common intent actions
+│   ├── 📘 intent: Common intent actions
 │   ├── 👉 objection: Easy to use objection (require Android device rooted)
 │   ├── 👉 pidcat: Filter logcat by package name
 │   └── 👉 top: Fetch current running app's basic information
 ├── 📖 ct: Common scripts
-│   ├── 👉 cert: Display X.509 certificate information.
+│   ├── 👉 cert: Display X.509 certificate information
+│   ├── 📘 cntr: Deploy docker/pod containers
+│   ├── 📘 env: Linktools environment commands
 │   ├── 👉 grep: Match files with regular expression
-│   ├── 👉 shell: Shell with environment variables already initialized
 │   └── 👉 tools: Download and use tools
 └── 📖 it: iOS scripts
     ├── 👉 frida: Easy to use frida (require iOS device jailbreak)
-    ├── 👉 ipa: Parser ipa file
+    ├── 👉 ipa: Parse ipa file
     ├── 👉 objection: Easy to use objection (require iOS device jailbreak)
     ├── 👉 scp: OpenSSH secure file copy (require iOS device jailbreak)
     ├── 👉 sib: Sib supports managing multiple ios devices
     └── 👉 ssh: OpenSSH remote login client (require iOS device jailbreak)
 ```
 
 ### 通用功能（脚本前缀为ct-）
 
+#### 👉 ct-cntr
+
+<details>
+<summary>docker/pod容器一键部署工具，集成了包括nginx、nextcloud、redorid等等容器</summary>
+
+```
+$ ct-cntr -h
+usage: ct-cntr [-h] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [--version] COMMAND ...
+
+Deploy docker/pod containers
+
+    ___       __   __              __
+   / (_)___  / /__/ /_____  ____  / /____
+  / / / __ \/ //_/ __/ __ \/ __ \/ / ___/  linktools toolkit (v0.0.1.dev0)
+ / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
+/_/_/_/ /_/_/|_|\__/\____/\____/_/____/
+
+positional arguments:
+  COMMAND              Command Help
+    list               list all containers
+    add                add containers to installed list
+    remove             remove containers from installed list
+    info               display container info
+    up                 deploy installed containers
+    restart            restart installed containers
+    down               stop installed containers
+    exec               exec container command
+    config             manage container configs
+    repo               manage container repository
+
+options:
+  -h, --help           show this help message and exit
+  --version            show program's version number and exit
+
+log options:
+  --verbose            increase log verbosity
+  --debug              increase linktools's log verbosity, and enable debug mode
+  --time, --no-time    show log time
+  --level, --no-level  show log level
+```
+
+</details>
+
 #### 👉 ct-grep
 
 <details>
 <summary>类似linux中的grep，正则匹配文件内容 ，额外添加解析zip、elf等格等功能</summary>
 
 ```
 $ usage: ct-grep [-h] [--version] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [-i] pattern [file ...]
@@ -191,46 +235,14 @@
 
 log arguments:
   --verbose             increase log verbosity
   --debug               enable debug mode and increase log verbosity
   --time, --no-time     show log time
   --level, --no-level   show log level
 ```
-
-</details>
-
-#### 👉 ct-shell
-
-<details>
-<summary>已初始化常用工具环境变量的bash（mac/linux）、cmd（windows）</summary>
-
-```
-$ ct-shell -h
-usage: ct-shell [-h] [--version] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [-c COMMAND]
-
-Shell with environment variables already initialized
-
-    ___       __   __              __
-   / (_)___  / /__/ /_____  ____  / /____
-  / / / __ \/ //_/ __/ __ \/ __ \/ / ___/  linktools toolkit (v0.0.1.dev0)
- / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
-/_/_/_/ /_/_/|_|\__/\____/\____/_/____/
-
-options:
-  -h, --help            show this help message and exit
-  --version             show program's version number and exit
-  -c COMMAND, --command COMMAND
-                        shell command
-
-log arguments:
-  --verbose             increase log verbosity
-  --debug               enable debug mode and increase log verbosity
-  --time, --no-time     show log time
-  --level, --no-level   show log level
-```
 
 </details>
 
 ### android相关功能（脚本前缀为at-）
 
 #### 👉 at-adb
```

### Comparing `linktools-0.8.3rc0/README.md` & `linktools-0.8.3rc1/src/linktools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,55 @@
+Metadata-Version: 2.1
+Name: linktools
+Version: 0.8.3rc1
+Summary: linktools toolkit
+Author-email: Hu Ji <669898595@qq.com>
+License: Apache 2.0
+Project-URL: Homepage, https://github.com/ice-black-tea/linktools
+Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: rich
+Requires-Dist: filelock>=3.4.0
+Provides-Extra: requests
+Requires-Dist: requests[socks]; extra == "requests"
+Provides-Extra: frida
+Requires-Dist: frida>=15.0.0; extra == "frida"
+Provides-Extra: objection
+Requires-Dist: objection; extra == "objection"
+Provides-Extra: lief
+Requires-Dist: lief>0.10.1; extra == "lief"
+Requires-Dist: python-magic; platform_system == "Linux" and extra == "lief"
+Requires-Dist: python-magic; platform_system == "Darwin" and extra == "lief"
+Requires-Dist: python-magic-bin; platform_system == "Windows" and extra == "lief"
+Provides-Extra: ssh
+Requires-Dist: paramiko; extra == "ssh"
+Requires-Dist: scp; extra == "ssh"
+Provides-Extra: ssl
+Requires-Dist: pyOpenSSL; extra == "ssl"
+Provides-Extra: container
+Requires-Dist: GitPython; extra == "container"
+Requires-Dist: jinja2; extra == "container"
+Requires-Dist: pyyaml; extra == "container"
+Provides-Extra: all
+Requires-Dist: requests[socks]; extra == "all"
+Requires-Dist: frida>=15.0.0; extra == "all"
+Requires-Dist: objection; extra == "all"
+Requires-Dist: lief>0.10.1; extra == "all"
+Requires-Dist: python-magic; platform_system == "Linux" and extra == "all"
+Requires-Dist: python-magic; platform_system == "Darwin" and extra == "all"
+Requires-Dist: python-magic-bin; platform_system == "Windows" and extra == "all"
+Requires-Dist: paramiko; extra == "all"
+Requires-Dist: scp; extra == "all"
+Requires-Dist: pyOpenSSL; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: pyyaml; extra == "all"
+
 # Linktools Toolkit
 
 ## 开始使用
 
 ### 依赖项
 
 python & pip (3.6及以上): <https://www.python.org/downloads/>
@@ -54,34 +102,78 @@
 ├── 📖 at: Android scripts
 │   ├── 👉 adb: Adb supports managing multiple android devices
 │   ├── 👉 agent: Debug android-tools.apk
 │   ├── 👉 app: Fetch application info
 │   ├── 👉 debug: Debug app by jdb
 │   ├── 👉 frida: Easy to use frida (require Android device rooted)
 │   ├── 👉 info: Fetch device information
-│   ├── 👉 intent: Common intent actions
+│   ├── 📘 intent: Common intent actions
 │   ├── 👉 objection: Easy to use objection (require Android device rooted)
 │   ├── 👉 pidcat: Filter logcat by package name
 │   └── 👉 top: Fetch current running app's basic information
 ├── 📖 ct: Common scripts
-│   ├── 👉 cert: Display X.509 certificate information.
+│   ├── 👉 cert: Display X.509 certificate information
+│   ├── 📘 cntr: Deploy docker/pod containers
+│   ├── 📘 env: Linktools environment commands
 │   ├── 👉 grep: Match files with regular expression
-│   ├── 👉 shell: Shell with environment variables already initialized
 │   └── 👉 tools: Download and use tools
 └── 📖 it: iOS scripts
     ├── 👉 frida: Easy to use frida (require iOS device jailbreak)
-    ├── 👉 ipa: Parser ipa file
+    ├── 👉 ipa: Parse ipa file
     ├── 👉 objection: Easy to use objection (require iOS device jailbreak)
     ├── 👉 scp: OpenSSH secure file copy (require iOS device jailbreak)
     ├── 👉 sib: Sib supports managing multiple ios devices
     └── 👉 ssh: OpenSSH remote login client (require iOS device jailbreak)
 ```
 
 ### 通用功能（脚本前缀为ct-）
 
+#### 👉 ct-cntr
+
+<details>
+<summary>docker/pod容器一键部署工具，集成了包括nginx、nextcloud、redorid等等容器</summary>
+
+```
+$ ct-cntr -h
+usage: ct-cntr [-h] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [--version] COMMAND ...
+
+Deploy docker/pod containers
+
+    ___       __   __              __
+   / (_)___  / /__/ /_____  ____  / /____
+  / / / __ \/ //_/ __/ __ \/ __ \/ / ___/  linktools toolkit (v0.0.1.dev0)
+ / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
+/_/_/_/ /_/_/|_|\__/\____/\____/_/____/
+
+positional arguments:
+  COMMAND              Command Help
+    list               list all containers
+    add                add containers to installed list
+    remove             remove containers from installed list
+    info               display container info
+    up                 deploy installed containers
+    restart            restart installed containers
+    down               stop installed containers
+    exec               exec container command
+    config             manage container configs
+    repo               manage container repository
+
+options:
+  -h, --help           show this help message and exit
+  --version            show program's version number and exit
+
+log options:
+  --verbose            increase log verbosity
+  --debug              increase linktools's log verbosity, and enable debug mode
+  --time, --no-time    show log time
+  --level, --no-level  show log level
+```
+
+</details>
+
 #### 👉 ct-grep
 
 <details>
 <summary>类似linux中的grep，正则匹配文件内容 ，额外添加解析zip、elf等格等功能</summary>
 
 ```
 $ usage: ct-grep [-h] [--version] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [-i] pattern [file ...]
@@ -143,46 +235,14 @@
 
 log arguments:
   --verbose             increase log verbosity
   --debug               enable debug mode and increase log verbosity
   --time, --no-time     show log time
   --level, --no-level   show log level
 ```
-
-</details>
-
-#### 👉 ct-shell
-
-<details>
-<summary>已初始化常用工具环境变量的bash（mac/linux）、cmd（windows）</summary>
-
-```
-$ ct-shell -h
-usage: ct-shell [-h] [--version] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [-c COMMAND]
-
-Shell with environment variables already initialized
-
-    ___       __   __              __
-   / (_)___  / /__/ /_____  ____  / /____
-  / / / __ \/ //_/ __/ __ \/ __ \/ / ___/  linktools toolkit (v0.0.1.dev0)
- / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
-/_/_/_/ /_/_/|_|\__/\____/\____/_/____/
-
-options:
-  -h, --help            show this help message and exit
-  --version             show program's version number and exit
-  -c COMMAND, --command COMMAND
-                        shell command
-
-log arguments:
-  --verbose             increase log verbosity
-  --debug               enable debug mode and increase log verbosity
-  --time, --no-time     show log time
-  --level, --no-level   show log level
-```
 
 </details>
 
 ### android相关功能（脚本前缀为at-）
 
 #### 👉 at-adb
```

### Comparing `linktools-0.8.3rc0/pyproject.toml` & `linktools-0.8.3rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/setup.py` & `linktools-0.8.3rc1/setup.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/__init__.py` & `linktools-0.8.3rc1/src/linktools/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/__main__.py` & `linktools-0.8.3rc1/src/linktools/__main__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/_config.py` & `linktools-0.8.3rc1/src/linktools/_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,19 @@
     if obj is None:
         return ""
     return str(obj)
 
 
 def cast_path(obj: Any) -> str:
     if isinstance(obj, str):
-        return os.path.abspath(os.path.expanduser(obj))
+        return os.path.abspath(
+            os.path.expanduser(
+                str(obj)  # support Proxy object
+            )
+        )
     raise TypeError(f"{type(obj)} cannot be converted to path")
 
 
 def cast_json(obj: Any) -> Union[List, Dict]:
     if isinstance(obj, str):
         return json.loads(obj)
     if isinstance(obj, (Tuple, List, Dict)):
```

### Comparing `linktools-0.8.3rc0/src/linktools/_environ.py` & `linktools-0.8.3rc1/src/linktools/_environ.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,30 +28,28 @@
 """
 import abc
 import json
 import logging
 import os
 import pathlib
 import shutil
+import sys
 import time
 from typing import TYPE_CHECKING, TypeVar, Type, Any
 
 from . import utils, metadata
 from .decorator import cached_property, cached_classproperty
 
 if TYPE_CHECKING:
     from ._config import ConfigDict, Config
     from ._tools import Tools, Tool
     from ._url import UrlFile
 
     T = TypeVar("T")
 
-root_path = os.path.dirname(__file__)
-asset_path = os.path.join(root_path, "assets")
-
 
 class BaseEnviron(abc.ABC):
 
     @property
     @abc.abstractmethod
     def name(self) -> str:
         """
@@ -81,22 +79,22 @@
         raise NotImplemented
 
     @property
     def system(self) -> str:
         """
         系统名称
         """
-        return self.tools.system
+        return utils.get_system()
 
     @property
     def machine(self) -> str:
         """
         机器类型，e.g. 'i386'
         """
-        return self.tools.machine
+        return utils.get_machine()
 
     @property
     def debug(self) -> bool:
         """
         debug模式
         """
         return self.get_config("DEBUG", type=bool, default=False)
@@ -252,26 +250,22 @@
 
     @cached_classproperty
     def _default_config(self) -> "ConfigDict":
         from ._config import ConfigDict
 
         config = ConfigDict()
 
-        yaml_path = os.path.join(root_path, "template", "tools.yml")
-        if metadata.__release__ or not os.path.exists(yaml_path):
-            config.update_from_file(
-                os.path.join(asset_path, "tools.json"),
-                json.load
-            )
-        else:
-            import yaml
-            config.update_from_file(
-                yaml_path,
-                yaml.safe_load
-            )
+        config.update({
+            "TOOL_SHELL": {
+                "absolute_path": utils.get_shell_path(),
+            },
+            "TOOL_PYTHON": {
+                "absolute_path": sys.executable,
+            }
+        })
 
         return config
 
     def _create_config(self) -> "Config":
         from ._config import Config
 
         return Config(
@@ -379,17 +373,17 @@
     def version(self) -> str:
         return metadata.__version__
 
     @property
     def description(self) -> str:
         return metadata.__description__
 
-    @property
+    @cached_property
     def root_path(self) -> str:
-        return root_path
+        return os.path.dirname(__file__)
 
     def _create_config(self):
         config = super()._create_config()
 
         # 初始化下载相关参数
         config.set(
             "DEFAULT_USER_AGENT",
@@ -397,18 +391,31 @@
             "AppleWebKit/537.36 (KHTML, like Gecko) "
             "Chrome/123.0.0.0 "
             "Safari/537.36"
         )
 
         # 导入configs文件夹中所有配置文件
         config.update_from_file(
-            os.path.join(asset_path, "android-tools.json"),
+            self.get_asset_path("android-tools.json"),
             load=json.load
         )
 
+        yaml_path = self.get_path("template", "tools.yml")
+        if metadata.__release__ or not os.path.exists(yaml_path):
+            config.update_from_file(
+                self.get_asset_path("tools.json"),
+                json.load
+            )
+        else:
+            import yaml
+            config.update_from_file(
+                yaml_path,
+                yaml.safe_load
+            )
+
         return config
 
     def get_asset_path(self, *paths: str) -> str:
-        return utils.get_path(asset_path, *paths)
+        return self.get_path("assets", *paths)
 
 
 environ = Environ()
```

### Comparing `linktools-0.8.3rc0/src/linktools/_tools.py` & `linktools-0.8.3rc1/src/linktools/_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,15 +26,14 @@
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 import os
 import pickle
 import shutil
-import sys
 import warnings
 from typing import TYPE_CHECKING, Dict, Union, Mapping, Iterator, Any, Tuple, List, Type
 
 from . import utils
 from .decorator import cached_property
 from .metadata import __missing__
 
@@ -204,176 +203,176 @@
     cmdline: str = ToolProperty(default=__missing__)
     executable: bool = ToolProperty(default=True)
     executable_cmdline: tuple = ToolProperty(default=[])
 
     exists: bool = property(lambda self: self.absolute_path and os.path.exists(self.absolute_path))
     dirname: bool = property(lambda self: None if not self.absolute_path else os.path.dirname(self.absolute_path))
 
-    def __init__(self, container: "Tools", config: Union[dict, str], **kwargs):
-        self._container = container
+    def __init__(self, tools: "Tools", config: Union[dict, str], **kwargs):
+        self._tools = tools
         self._config = config
 
         self._raw_config = pickle.loads(pickle.dumps(self.__default__))
-        self._raw_config.update(container.config)
+        self._raw_config.update(tools.config)
         self._raw_config.update(config)
         self._raw_config.update(kwargs)
 
     @cached_property
     def config(self) -> dict:
-        cfg = self.__parser__.parse(self._raw_config)
+        config = self.__parser__.parse(self._raw_config)
 
-        depends_on = utils.get_item(cfg, "depends_on")
+        depends_on = utils.get_item(config, "depends_on")
         if depends_on:
             assert isinstance(depends_on, (str, Tuple, List)), \
-                f"Tool<{cfg['name']}>.depends_on type error, " \
+                f"Tool<{config['name']}>.depends_on type error, " \
                 f"str/tuple/list was expects, got {type(depends_on)}"
             if isinstance(depends_on, str):
                 depends_on = [depends_on]
             for dependency in depends_on:
-                assert dependency in self._container.items, \
-                    f"Tool<{cfg['name']}>.depends_on error: not found Tool<{dependency}>"
-            cfg["depends_on"] = depends_on
+                assert dependency in self._tools.items, \
+                    f"Tool<{config['name']}>.depends_on error: not found Tool<{dependency}>"
+            config["depends_on"] = depends_on
 
         # download url
-        download_url = utils.get_item(cfg, "download_url") or ""
+        download_url = utils.get_item(config, "download_url") or ""
         if download_url == __missing__:
             download_url = ""
         assert isinstance(download_url, str), \
-            f"Tool<{cfg['name']}>.download_url type error, " \
+            f"Tool<{config['name']}>.download_url type error, " \
             f"str was expects, got {type(download_url)}"
-        cfg["download_url"] = download_url.format(tools=self._container, **cfg)
+        config["download_url"] = download_url.format(tools=self._tools, **config)
 
-        unpack_path = utils.get_item(cfg, "unpack_path") or ""
+        unpack_path = utils.get_item(config, "unpack_path") or ""
         if unpack_path == __missing__:
             unpack_path = ""
         assert isinstance(unpack_path, str), \
-            f"Tool<{cfg['name']}>.unpack_path type error, " \
+            f"Tool<{config['name']}>.unpack_path type error, " \
             f"str was expects, got {type(unpack_path)}"
 
-        target_path = utils.get_item(cfg, "target_path") or ""
+        target_path = utils.get_item(config, "target_path") or ""
         if target_path == __missing__:
             target_path = ""
         assert isinstance(target_path, str), \
-            f"Tool<{cfg['name']}>.target_path type error, " \
+            f"Tool<{config['name']}>.target_path type error, " \
             f"str was expects, got {type(target_path)}"
 
-        absolute_path = utils.get_item(cfg, "absolute_path") or ""
+        absolute_path = utils.get_item(config, "absolute_path") or ""
         if absolute_path == __missing__:
             absolute_path = ""
         assert isinstance(absolute_path, str), \
-            f"Tool<{cfg['name']}>.absolute_path type error, " \
+            f"Tool<{config['name']}>.absolute_path type error, " \
             f"str was expects, got {type(absolute_path)}"
 
         if download_url and not unpack_path and not target_path:
             target_path = utils.guess_file_name(download_url)
 
         # target path: {target_path}
         # unpack path: {unpack_path}
         # root path: {data_path}/tools/{unpack_path}/
         # absolute path: {data_path}/tools/{unpack_path}/{target_path}
-        cfg["target_path"] = target_path.format(tools=self._container, **cfg)
-        cfg["unpack_path"] = unpack_path.format(tools=self._container, **cfg)
+        config["target_path"] = target_path.format(tools=self._tools, **config)
+        config["unpack_path"] = unpack_path.format(tools=self._tools, **config)
         paths = ["tools"]
-        if not utils.is_empty(cfg["unpack_path"]):
-            paths.append(cfg["unpack_path"])
-        cfg["root_path"] = self._container.environ.get_data_dir(*paths)
+        if not utils.is_empty(config["unpack_path"]):
+            paths.append(config["unpack_path"])
+        config["root_path"] = self._tools.environ.get_data_dir(*paths)
 
         if absolute_path:
-            cfg["absolute_path"] = absolute_path.format(tools=self._container, **cfg)
-        elif cfg["target_path"]:
-            cfg["absolute_path"] = os.path.join(cfg["root_path"], cfg["target_path"])
+            config["absolute_path"] = absolute_path.format(tools=self._tools, **config)
+        elif config["target_path"]:
+            config["absolute_path"] = os.path.join(config["root_path"], config["target_path"])
         else:
-            cfg["absolute_path"] = ""
+            config["absolute_path"] = ""
 
         # set executable cmdline
-        cmdline = utils.get_item(cfg, "cmdline") or ""
+        cmdline = utils.get_item(config, "cmdline") or ""
         if cmdline == __missing__:
-            cmdline = cfg["name"]
+            cmdline = config["name"]
         assert isinstance(cmdline, str), \
-            f"Tool<{cfg['name']}>.cmdline type error, " \
+            f"Tool<{config['name']}>.cmdline type error, " \
             f"str was expects, got {type(absolute_path)}"
-        cfg["cmdline"] = cmdline
+        config["cmdline"] = cmdline
 
         if not utils.is_empty(cmdline):
             cmdline = shutil.which(cmdline)
         if not utils.is_empty(cmdline):
-            cfg["absolute_path"] = cmdline
-            cfg["executable_cmdline"] = [cmdline]
+            config["absolute_path"] = cmdline
+            config["executable_cmdline"] = [cmdline]
         else:
-            executable_cmdline = utils.get_item(cfg, "executable_cmdline")
+            executable_cmdline = utils.get_item(config, "executable_cmdline")
             if executable_cmdline:
                 assert isinstance(executable_cmdline, (str, Tuple, List)), \
-                    f"Tool<{cfg['name']}>.executable_cmdline type error, " \
+                    f"Tool<{config['name']}>.executable_cmdline type error, " \
                     f"str/tuple/list was expects, got {type(executable_cmdline)}"
                 # if executable_cmdline is not empty,
                 # set the executable flag to false
-                cfg["executable"] = False
+                config["executable"] = False
             else:
                 # if executable_cmdline is empty,
                 # set absolute_path as executable_cmdline
-                executable_cmdline = cfg["absolute_path"]
+                executable_cmdline = config["absolute_path"]
             if isinstance(executable_cmdline, str):
                 executable_cmdline = [executable_cmdline]
-            cfg["executable_cmdline"] = [str(i).format(tools=self._container, **cfg) \
-                                         for i in executable_cmdline]
+            config["executable_cmdline"] = [str(i).format(tools=self._tools, **config) \
+                                            for i in executable_cmdline]
 
-        return cfg
+        return config
 
     def copy(self, **kwargs):
-        return Tool(self._container, self._config, **kwargs)
+        return Tool(self._tools, self._config, **kwargs)
 
     def prepare(self) -> None:
         for dependency in self.depends_on:
-            tool = self._container[dependency]
+            tool = self._tools[dependency]
             tool.prepare()
 
         # download and unzip file
         if self.exists:
             pass
         elif not self.download_url or not self.absolute_path:
             raise ToolError(
                 f"{self} does not support on "
-                f"{self._container.system} ({self._container.machine})")
+                f"{self._tools.environ.system} ({self._tools.environ.machine})")
         else:
-            self._container.logger.info(f"Download {self}: {self.download_url}")
-            url_file = self._container.environ.get_url_file(self.download_url)
-            temp_dir = self._container.environ.get_temp_path("tools", "cache")
+            self._tools.logger.info(f"Download {self}: {self.download_url}")
+            url_file = self._tools.environ.get_url_file(self.download_url)
+            temp_dir = self._tools.environ.get_temp_path("tools", "cache")
             temp_path = url_file.save(to_dir=temp_dir)
             if not utils.is_empty(self.unpack_path):
-                self._container.logger.debug(f"Unpack {self} to {self.root_path}")
+                self._tools.logger.debug(f"Unpack {self} to {self.root_path}")
                 shutil.unpack_archive(temp_path, self.root_path)
                 os.remove(temp_path)
             else:
-                self._container.logger.debug(f"Move {self} to {self.absolute_path}")
+                self._tools.logger.debug(f"Move {self} to {self.absolute_path}")
                 shutil.move(temp_path, self.absolute_path)
 
         # change tool file mode
         if self.executable and not os.access(self.absolute_path, os.X_OK):
-            self._container.logger.debug(f"Chmod 755 {self.absolute_path}")
+            self._tools.logger.debug(f"Chmod 755 {self.absolute_path}")
             os.chmod(self.absolute_path, 0o0755)
 
     def clear(self) -> None:
         if not self.exists:
-            self._container.logger.debug(f"{self} does not exist, skip")
+            self._tools.logger.debug(f"{self} does not exist, skip")
             return
         if not utils.is_empty(self.unpack_path):
-            self._container.logger.debug(f"Delete {self.root_path}")
+            self._tools.logger.debug(f"Delete {self.root_path}")
             shutil.rmtree(self.root_path, ignore_errors=True)
         elif self.absolute_path.startswith(self.root_path):
-            self._container.logger.debug(f"Delete {self.absolute_path}")
+            self._tools.logger.debug(f"Delete {self.absolute_path}")
             os.remove(self.absolute_path)
 
     def popen(self, *args: [Any], **kwargs) -> utils.Process:
         self.prepare()
 
         # java or other
         executable_cmdline = self.executable_cmdline
-        if executable_cmdline[0] in self._container.items:
+        if executable_cmdline[0] in self._tools.items:
             args = [*executable_cmdline[1:], *args]
-            tool = self._container.items[executable_cmdline[0]]
+            tool = self._tools.items[executable_cmdline[0]]
             return tool.popen(*args, **kwargs)
 
         return utils.Process(*[*executable_cmdline, *args], **kwargs)
 
     @utils.timeoutable
     def exec(
             self,
@@ -393,16 +392,16 @@
         :return: 返回stdout输出内容
         """
         process = self.popen(*args, capture_output=True)
 
         try:
             out, err = process.exec(
                 timeout=timeout,
-                on_stdout=self._container.logger.info if log_output else None,
-                on_stderr=self._container.logger.error if log_output else None
+                on_stdout=self._tools.logger.info if log_output else None,
+                on_stderr=self._tools.logger.error if log_output else None
             )
             if not ignore_errors and process.poll() not in (0, None):
                 if isinstance(err, bytes):
                     err = err.decode(errors="ignore")
                     err = err.strip()
                 elif isinstance(err, str):
                     err = err.strip()
@@ -422,42 +421,33 @@
 
     def __repr__(self):
         return f"Tool<{self.name}>"
 
 
 class Tools(object):
 
-    def __init__(self, env: "BaseEnviron", **kwargs):
-        self.environ = env
-        self.logger = env.get_logger("tools")
-
-        self.config = kwargs
-        self.config.setdefault("system", utils.get_system())
-        self.config.setdefault("machine", utils.get_machine())
-        self.config.setdefault("interpreter", sys.executable)
-
-    @property
-    def system(self) -> str:
-        return self.config["system"]
-
-    @property
-    def machine(self) -> str:
-        return self.config["machine"]
+    def __init__(self, environ: "BaseEnviron"):
+        self.environ = environ
+        self.logger = environ.get_logger("tools")
+
+        self.config = dict()
+        self.config.setdefault("system", environ.system)
+        self.config.setdefault("machine", environ.machine)
 
     @cached_property
     def items(self) -> Mapping[str, Tool]:
         items = {}
         for key in self.environ.config.keys():
-            if not key.startswith("GENERAL_TOOL_"):
+            if not key.startswith("TOOL_"):
                 continue
             value = self.environ.config.get(key)
             if not isinstance(value, dict):
                 warnings.warn(f"dict was expected, got {type(value)}, ignored.")
                 continue
-            key = key[len("GENERAL_TOOL_"):]
+            key = key[len("TOOL_"):]
             key = key.lower()
             name = value.setdefault("name", key)
             items[name] = Tool(self, value)
         return items
 
     def __iter__(self) -> Iterator[Tool]:
         return iter(self.items.values())
```

### Comparing `linktools-0.8.3rc0/src/linktools/_url.py` & `linktools-0.8.3rc1/src/linktools/_url.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/android/__init__.py` & `linktools-0.8.3rc1/src/linktools/android/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/android/adb.py` & `linktools-0.8.3rc1/src/linktools/android/adb.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/android/struct.py` & `linktools-0.8.3rc1/src/linktools/android/struct.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/assets/android-tools.json` & `linktools-0.8.3rc1/src/linktools/assets/android-tools.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'ANDROID_TOOL_BRIDGE_APK'": "{'md5': '3097e19b66070036181860877768b952', 'time': '2024-04-05 "*

 * *                              "21:46:39'}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "ANDROID_TOOL_BRIDGE_APK": {
         "main": "android.tools.Main",
-        "md5": "6a8c9cfb8555846bee1b972b63331027",
+        "md5": "3097e19b66070036181860877768b952",
         "name": "android-tools.apk",
         "size": 82987,
-        "time": "2024-04-03 16:10:23"
+        "time": "2024-04-05 21:46:39"
     },
     "ANDROID_TOOL_FRIDA_SERVER": [
         {
             "min_version": "15.1.8",
             "name": "strong-frida-server-{version}-android-{abi}",
             "url": "https://github.com/hzzheyang/strongR-frida-android/releases/download/{version}/hluda-server-{version}-android-{abi}.xz"
         },
```

### Comparing `linktools-0.8.3rc0/src/linktools/assets/chrome-driver.json` & `linktools-0.8.3rc1/src/linktools/assets/chrome-driver.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/Dockerfile` & `linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/Dockerfile`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/container.py` & `linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt` & `linktools-0.8.3rc1/src/linktools/assets/containers/100-nginx/dnsapi.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/assets/containers/110-portainer/container.py` & `linktools-0.8.3rc1/src/linktools/assets/containers/110-portainer/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/assets/containers/120-flare/compose.yml` & `linktools-0.8.3rc1/src/linktools/assets/containers/120-flare/compose.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 services:
   flare:
     image: soulteary/flare
-    user: '{{ DOCKER_PUID }}:{{ DOCKER_PGID }}'
+    user: '{{ DOCKER_UID }}:{{ DOCKER_GID }}'
 #   {% if int(FLARE_EXPOSE_PORT, 0) > 0 %}
     ports:
       - '{{ FLARE_EXPOSE_PORT }}:5005'
 #   {% endif %}
 #   {% if bool(FLARE_DISABLE_LOGIN) %}
     command: flare --disable_login=1 --visibility=private
     environment:
```

### Comparing `linktools-0.8.3rc0/src/linktools/assets/containers/120-flare/container.py` & `linktools-0.8.3rc1/src/linktools/assets/containers/120-flare/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/assets/containers/120-flare/nginx.conf` & `linktools-0.8.3rc1/src/linktools/assets/containers/120-flare/nginx.conf`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/assets/fake_useragent.json` & `linktools-0.8.3rc1/src/linktools/assets/fake_useragent.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/assets/frida.js` & `linktools-0.8.3rc1/src/linktools/assets/frida.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -944,8 +944,8 @@
             }, t;
         }();
 
         exports.ObjCHelper = t;
 
     }, {}]
 }, {}, [1])
-//# sourceMappingURL=data:application/json;charset=utf-8;base64,eyJ2ZXJzaW9uIjozLCJzb3VyY2VzIjpbIm5vZGVfbW9kdWxlcy9icm93c2VyLXBhY2svX3ByZWx1ZGUuanMiLCJpbmRleC50cyIsImxpYi9hbmRyb2lkLnRzIiwibGliL2MudHMiLCJsaWIvaW9zLnRzIiwibGliL2phdmEudHMiLCJsaWIvb2JqYy50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiQUFBQTs7Ozs7OztBQ0tBLElBQUEsSUFBQTtFQUFBLFNBQUE7SUFBQSxJQUFBLElBQUE7SUFFWSxLQUFBLGdCQUF1QixJQUN2QixLQUFBLGFBQWtCLE1Bd0JsQixLQUFBLFFBQVE7TUFNWixJQUx3QixTQUFwQixFQUFLLGVBQ0wsYUFBYSxFQUFLLGFBQ2xCLEVBQUssYUFBYTtNQUdZLE1BQTlCLEVBQUssY0FBYyxRQUF2QjtRQUlBLElBQU0sSUFBUyxFQUFLO1FBQ3BCLEVBQUssZ0JBQWdCLElBRXJCLEtBQUs7VUFBRSxTQUFTOzs7QUFDcEI7QUFDSjtFQUFBLE9BckNJLEVBQUEsVUFBQSxPQUFBLFNBQUssR0FBYyxHQUFjO0lBQzdCLElBQU0sSUFBUTtJQUNkLEVBQU0sS0FBUSxHQUVGLFFBQVIsS0FFQSxLQUFLLGNBQWMsS0FBSyxJQUNwQixLQUFLLGNBQWMsVUFBVSxLQUc3QixLQUFLLFVBQ3NCLFNBQXBCLEtBQUssZUFDWixLQUFLLGFBQWEsV0FBVyxLQUFLLE9BQU8sU0FLN0MsS0FBSztJQUNMLEtBQUs7TUFBRSxTQUFTLEVBQUM7T0FBVTtBQUVuQyxLQWlCSjtBQUFBLENBMUNBLElBNkNBLElBQUE7RUFBQSxTQUFBLEtBS0E7RUFBQSxPQUhJLEVBQUEsVUFBQSxPQUFBLFNBQUssR0FBYztJQUNmLEVBQWMsS0FBSyxPQUFPLEdBQVM7QUFDdkMsS0FDSjtBQUFBLENBTEEsSUFZQSxJQUFBO0VBUUksU0FBQTtJQU5BLEtBQUEsUUFBUSxHQUNSLEtBQUEsT0FBTyxHQUNQLEtBQUEsVUFBVSxHQUNWLEtBQUEsUUFBUSxHQUNBLEtBQUEsU0FBUyxLQUFLO0lBR2xCLElBQU0sSUFBVyxTQUFXO01BQ3hC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QUFRO01BSXBCLFlBSHFDLE1BQWpDLEVBQXdCLE9BQ3hCLEVBQXdCLEtBQU8sWUFBWSxZQUFZLEtBRXBELEVBQXdCO0FBQ25DOzs7OztBQ3pUUjtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTs7Ozs7Ozs7QUM1SUEsSUFBQSxJQUFBO0VBQUEsU0FBQTtJQUVJLEtBQUEsY0FBYztBQXdO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SztBQUNqQixPQUVPO0FBQ1gsS0FFSjtBQUFBLENBMU5BOztBQUFhLFFBQUE7OztBQ2JiO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTs7QUNuQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTs7QUM1UUE7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0EiLCJmaWxlIjoiZ2VuZXJhdGVkLmpzIiwic291cmNlUm9vdCI6IiJ9
+//# sourceMappingURL=data:application/json;charset=utf-8;base64,eyJ2ZXJzaW9uIjozLCJzb3VyY2VzIjpbIm5vZGVfbW9kdWxlcy9icm93c2VyLXBhY2svX3ByZWx1ZGUuanMiLCJpbmRleC50cyIsImxpYi9hbmRyb2lkLnRzIiwibGliL2MudHMiLCJsaWIvaW9zLnRzIiwibGliL2phdmEudHMiLCJsaWIvb2JqYy50cyJdLCJuYW1lcyI6W10sIm1hcHBpbmdzIjoiQUFBQTs7Ozs7OztBQ0tBLElBQUEsSUFBQTtFQUFBLFNBQUE7SUFBQSxJQUFBLElBQUE7SUFFWSxLQUFBLGdCQUF1QixJQUN2QixLQUFBLGFBQWtCLE1Bd0JsQixLQUFBLFFBQVE7TUFNWixJQUx3QixTQUFwQixFQUFLLGVBQ0wsYUFBYSxFQUFLLGFBQ2xCLEVBQUssYUFBYTtNQUdZLE1BQTlCLEVBQUssY0FBYyxRQUF2QjtRQUlBLElBQU0sSUFBUyxFQUFLO1FBQ3BCLEVBQUssZ0JBQWdCLElBRXJCLEtBQUs7VUFBRSxTQUFTOzs7QUFDcEI7QUFDSjtFQUFBLE9BckNJLEVBQUEsVUFBQSxPQUFBLFNBQUssR0FBYyxHQUFjO0lBQzdCLElBQU0sSUFBUTtJQUNkLEVBQU0sS0FBUSxHQUVGLFFBQVIsS0FFQSxLQUFLLGNBQWMsS0FBSyxJQUNwQixLQUFLLGNBQWMsVUFBVSxLQUc3QixLQUFLLFVBQ3NCLFNBQXBCLEtBQUssZUFDWixLQUFLLGFBQWEsV0FBVyxLQUFLLE9BQU8sU0FLN0MsS0FBSztJQUNMLEtBQUs7TUFBRSxTQUFTLEVBQUM7T0FBVTtBQUVuQyxLQWlCSjtBQUFBLENBMUNBLElBNkNBLElBQUE7RUFBQSxTQUFBLEtBS0E7RUFBQSxPQUhJLEVBQUEsVUFBQSxPQUFBLFNBQUssR0FBYztJQUNmLEVBQWMsS0FBSyxPQUFPLEdBQVM7QUFDdkMsS0FDSjtBQUFBLENBTEEsSUFZQSxJQUFBO0VBUUksU0FBQTtJQU5BLEtBQUEsUUFBUSxHQUNSLEtBQUEsT0FBTyxHQUNQLEtBQUEsVUFBVSxHQUNWLEtBQUEsUUFBUSxHQUNBLEtBQUEsU0FBUyxLQUFLO0lBR2xCLElBQU0sSUFBVyxTQUFXO01BQ3hC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QUFRO01BSXBCLFlBSHFDLE1BQWpDLEVBQXdCLE9BQ3hCLEVBQXdCLEtBQU8sWUFBWSxZQUFZLEtBRXBELEVBQXdCO0FBQ25DOzs7OztBQ3pUUjtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTtBQUNBO0FBQ0E7QUFDQTs7Ozs7Ozs7QUM1SUEsSUFBQSxJQUFBO0VBQUEsU0FBQTtJQUVJLEtBQUEsY0FBYztBQXdO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
```

### Comparing `linktools-0.8.3rc0/src/linktools/assets/frida.min.js` & `linktools-0.8.3rc1/src/linktools/assets/frida.min.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/assets/objection/plugins/__init__.py` & `linktools-0.8.3rc1/src/linktools/assets/objection/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/assets/tools.json` & `linktools-0.8.3rc1/src/linktools/assets/tools.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('TOOL_BAKSMALI', OrderedDict([('depends_on', 'java'), "*

 * *            "('executable_cmdline', ['java', '-jar', '{absolute_path}']), ('version', '2.5.2'), "*

 * *            "('download_url', "*

 * *            "'https://bitbucket.org/JesusFreke/smali/downloads/baksmali-{version}.jar')])), "*

 * *            "('TOOL_SMALI', OrderedDict([('depends_on', 'java'), ('executable_cmdline', ['java', "*

 * *            "'-jar', '{absolute_path}']), ('version', '2.5.2'), ('download_url', "*

 * *            "'https://b […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "GENERAL_TOOL_AAPT": {
+    "TOOL_AAPT": {
         "download_url": {
             "case": [
                 {
                     "then": "https://dl.google.com/android/repository/build-tools_{version}-macosx.zip",
                     "when": {
                         "system": "darwin"
                     }
@@ -47,15 +47,15 @@
                 }
             ]
         },
         "unpack_path": "build-tools-{version}",
         "version": "r33",
         "version_name": "android-13"
     },
-    "GENERAL_TOOL_ADB": {
+    "TOOL_ADB": {
         "download_url": "https://dl.google.com/android/repository/platform-tools-latest-{system}.zip",
         "target_path": {
             "case": [
                 {
                     "then": "platform-tools/{name}",
                     "when": {
                         "system": [
@@ -73,15 +73,15 @@
                 {
                     "else": null
                 }
             ]
         },
         "unpack_path": "platform-tools"
     },
-    "GENERAL_TOOL_APKSIGNER": {
+    "TOOL_APKSIGNER": {
         "download_url": {
             "case": [
                 {
                     "then": "https://dl.google.com/android/repository/build-tools_{version}-macosx.zip",
                     "when": {
                         "system": "darwin"
                     }
@@ -125,42 +125,45 @@
                 }
             ]
         },
         "unpack_path": "build-tools-{version}",
         "version": "r33",
         "version_name": "android-13"
     },
-    "GENERAL_TOOL_APKTOOL": {
+    "TOOL_APKTOOL": {
+        "depends_on": "java",
         "download_url": "https://bitbucket.org/iBotPeaches/apktool/downloads/apktool_{version}.jar",
         "executable_cmdline": [
             "java",
             "-jar",
             "{absolute_path}"
         ],
         "version": "2.8.1"
     },
-    "GENERAL_TOOL_APPCRAWLER": {
+    "TOOL_APPCRAWLER": {
+        "depends_on": "java",
         "download_url": "https://github.com/seveniruby/AppCrawler/releases/download/{version}/appcrawler-{version}-hogwarts.jar",
         "executable_cmdline": [
             "java",
             "-jar",
             "{absolute_path}"
         ],
         "version": "2.7.4"
     },
-    "GENERAL_TOOL_BAKSMALI": {
+    "TOOL_BAKSMALI": {
+        "depends_on": "java",
         "download_url": "https://bitbucket.org/JesusFreke/smali/downloads/baksmali-{version}.jar",
         "executable_cmdline": [
             "java",
             "-jar",
             "{absolute_path}"
         ],
         "version": "2.5.2"
     },
-    "GENERAL_TOOL_BURPSUITE": {
+    "TOOL_BURPSUITE": {
         "depends_on": "burpsuite-keygen",
         "download_url": "https://portswigger-cdn.net/burp/releases/download?product=pro&type=Jar&version={version}",
         "executable_cmdline": {
             "case": [
                 {
                     "then": [
                         "java",
@@ -199,24 +202,25 @@
                     "else": null
                 }
             ]
         },
         "target_path": "burpsuite_pro_v{version}.jar",
         "version": "2023.10"
     },
-    "GENERAL_TOOL_BURPSUITE_KEYGEN": {
+    "TOOL_BURPSUITE_KEYGEN": {
+        "depends_on": "java",
         "download_url": "https://github.com/ice-black-tea/archives/releases/download/burp-loader-keygen-2_1_06/burp-loader-keygen-2_1_06.jar",
         "executable_cmdline": [
             "java",
             "-jar",
             "{absolute_path}"
         ],
         "name": "burpsuite-keygen"
     },
-    "GENERAL_TOOL_CHROMEDRIVER": {
+    "TOOL_CHROMEDRIVER": {
         "base_url": "http://chromedriver.storage.googleapis.com",
         "download_url": {
             "case": [
                 {
                     "then": "{base_url}/{version}/chromedriver_mac64_m1.zip",
                     "when": {
                         "machine": "arm64",
@@ -269,15 +273,15 @@
                     "else": null
                 }
             ]
         },
         "unpack_path": "chromedriver-{version}",
         "version": "80.0.3987.106"
     },
-    "GENERAL_TOOL_DEX2JAR": {
+    "TOOL_DEX2JAR": {
         "download_url": "https://github.com/pxb1988/dex2jar/releases/download/v{version}{version_suffix}/dex-tools-{version}{version_suffix}.zip",
         "target_path": {
             "case": [
                 {
                     "then": "dex-tools-{version}/d2j-{name}.sh",
                     "when": {
                         "system": [
@@ -297,15 +301,15 @@
                 }
             ]
         },
         "unpack_path": "dex2jar-{version}",
         "version": "2.2-SNAPSHOT",
         "version_suffix": "-2021-10-31"
     },
-    "GENERAL_TOOL_FASTBOOT": {
+    "TOOL_FASTBOOT": {
         "download_url": "https://dl.google.com/android/repository/platform-tools-latest-{system}.zip",
         "target_path": {
             "case": [
                 {
                     "then": "platform-tools/{name}",
                     "when": {
                         "system": [
@@ -323,15 +327,15 @@
                 {
                     "else": null
                 }
             ]
         },
         "unpack_path": "platform-tools"
     },
-    "GENERAL_TOOL_IPATOOL": {
+    "TOOL_IPATOOL": {
         "download_url": {
             "case": [
                 {
                     "then": "https://github.com/majd/ipatool/releases/download/v{version}/ipatool-{version}-macos-arm64.tar.gz",
                     "when": {
                         "machine": "arm64",
                         "system": "darwin"
@@ -397,15 +401,15 @@
                     "else": null
                 }
             ]
         },
         "unpack_path": "ipatool-{version}",
         "version": "2.1.3"
     },
-    "GENERAL_TOOL_JADX": {
+    "TOOL_JADX": {
         "download_url": "https://github.com/skylot/jadx/releases/download/v{version}/jadx-{version}.zip",
         "target_path": {
             "case": [
                 {
                     "then": "bin/{name}",
                     "when": {
                         "system": [
@@ -424,15 +428,15 @@
                     "else": null
                 }
             ]
         },
         "unpack_path": "jadx-{version}",
         "version": "1.4.7"
     },
-    "GENERAL_TOOL_JADX_GUI": {
+    "TOOL_JADX_GUI": {
         "download_url": "https://github.com/skylot/jadx/releases/download/v{version}/jadx-{version}.zip",
         "name": "jadx-gui",
         "target_path": {
             "case": [
                 {
                     "then": "bin/{name}",
                     "when": {
@@ -452,15 +456,15 @@
                     "else": null
                 }
             ]
         },
         "unpack_path": "jadx-{version}",
         "version": "1.4.7"
     },
-    "GENERAL_TOOL_JAR2DEX": {
+    "TOOL_JAR2DEX": {
         "download_url": "https://github.com/pxb1988/dex2jar/releases/download/v{version}{version_suffix}/dex-tools-{version}{version_suffix}.zip",
         "target_path": {
             "case": [
                 {
                     "then": "dex-tools-{version}/d2j-{name}.sh",
                     "when": {
                         "system": [
@@ -480,15 +484,15 @@
                 }
             ]
         },
         "unpack_path": "dex2jar-{version}",
         "version": "2.2-SNAPSHOT",
         "version_suffix": "-2021-10-31"
     },
-    "GENERAL_TOOL_JARSIGNER": {
+    "TOOL_JARSIGNER": {
         "download_url": {
             "case": [
                 {
                     "then": "https://github.com/SAP/SapMachine/releases/download/sapmachine-{version}/sapmachine-jdk-{version}_macos-aarch64_bin.tar.gz",
                     "when": {
                         "machine": "arm64",
                         "system": "darwin"
@@ -544,15 +548,15 @@
                     "else": null
                 }
             ]
         },
         "unpack_path": "java-{version}",
         "version": "17.0.8"
     },
-    "GENERAL_TOOL_JAVA": {
+    "TOOL_JAVA": {
         "download_url": {
             "case": [
                 {
                     "then": "https://github.com/SAP/SapMachine/releases/download/sapmachine-{version}/sapmachine-jdk-{version}_macos-aarch64_bin.tar.gz",
                     "when": {
                         "machine": "arm64",
                         "system": "darwin"
@@ -608,15 +612,15 @@
                     "else": null
                 }
             ]
         },
         "unpack_path": "java-{version}",
         "version": "17.0.8"
     },
-    "GENERAL_TOOL_SIB": {
+    "TOOL_SIB": {
         "download_url": {
             "case": [
                 {
                     "then": "https://github.com/ice-black-tea/sonic-ios-bridge/releases/download/v{version}/sonic-ios-bridge_{version}_macosx_arm64.tar.gz",
                     "when": {
                         "machine": "arm64",
                         "system": "darwin"
@@ -669,41 +673,44 @@
                     "else": null
                 }
             ]
         },
         "unpack_path": "sib-{version}",
         "version": "1.3.17-20240112"
     },
-    "GENERAL_TOOL_SMALI": {
+    "TOOL_SMALI": {
+        "depends_on": "java",
         "download_url": "https://bitbucket.org/JesusFreke/smali/downloads/smali-{version}.jar",
         "executable_cmdline": [
             "java",
             "-jar",
             "{absolute_path}"
         ],
         "version": "2.5.2"
     },
-    "GENERAL_TOOL_TIDEVICE": {
-        "absolute_path": "{interpreter}",
+    "TOOL_TIDEVICE": {
+        "absolute_path": "{tools.python.absolute_path}",
+        "depends_on": "python",
         "executable_cmdline": [
-            "{interpreter}",
+            "python",
             "-m",
             "{name}"
         ]
     },
-    "GENERAL_TOOL_XPATCH": {
+    "TOOL_XPATCH": {
+        "depends_on": "java",
         "download_url": "https://github.com/WindySha/Xpatch/releases/download/v{version}/xpatch-{version}.jar",
         "executable_cmdline": [
             "java",
             "-jar",
             "{absolute_path}"
         ],
         "version": "5.2"
     },
-    "GENERAL_TOOL_ZIPALIGN": {
+    "TOOL_ZIPALIGN": {
         "download_url": {
             "case": [
                 {
                     "then": "https://dl.google.com/android/repository/build-tools_{version}-macosx.zip",
                     "when": {
                         "system": "darwin"
                     }
```

### Comparing `linktools-0.8.3rc0/src/linktools/cli/__init__.py` & `linktools-0.8.3rc1/src/linktools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/argparse.py` & `linktools-0.8.3rc1/src/linktools/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/command.py` & `linktools-0.8.3rc1/src/linktools/cli/command.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/android/adb.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/android/adb.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/android/agent.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/android/agent.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/android/app.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/android/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/android/debug.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/android/debug.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/android/frida.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/android/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/android/info.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/android/info.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/android/intent.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/android/intent.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/android/objection.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/android/objection.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/android/pidcat.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/android/pidcat.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/android/top.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/android/top.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/common/cert.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/common/cert.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 from linktools import utils
 from linktools.cli import BaseCommand
 
 
 class Command(BaseCommand):
     """
-    Display X.509 certificate information.
+    Display X.509 certificate information
     """
 
     @property
     def known_errors(self) -> List[Type[BaseException]]:
         return super().known_errors + [OpenSSL.crypto.Error]
 
     def init_arguments(self, parser: ArgumentParser) -> None:
```

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/common/cntr.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/common/cntr.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/common/env.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/common/env.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     ___________________________/___  `,
    /  oooooooooooooooo  .o.  oooo /,   \,"-----------
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from typing import Any
 
+from linktools import utils
 from linktools.cli import subcommand, subcommand_argument, SubCommandWrapper, BaseCommandGroup
 
 
 class InitCommand(BaseCommandGroup):
     """
     initialize environment
     """
@@ -62,23 +63,37 @@
             self.environ.tools["sib"].prepare()
         except Exception as e:
             self.logger.warning(f"initialize sib failed: {e}")
 
 
 class Command(BaseCommandGroup):
     """
-    environment configuration
+    Linktools environment commands
     """
 
     def init_subcommands(self) -> Any:
         return [
             SubCommandWrapper(InitCommand()),
             self
         ]
 
+    @subcommand("shell", help="run shell command")
+    @subcommand_argument("-c", "--command", help="shell command")
+    def on_shell(self, command: str = None):
+        shell = self.environ.tools["shell"]
+        if not shell.exists:
+            raise NotImplementedError(f"Not found shell path")
+
+        if command:
+            process = utils.Process(command, shell=True)
+            return process.call()
+
+        process = shell.popen()
+        return process.call()
+
     @subcommand("clean", help="clean temporary files")
     @subcommand_argument("days", metavar="DAYS", nargs="?", help="expire days")
     def on_clean_temp(self, days: int = 7):
         self.environ.clean_temp_files(days)
 
 
 command = Command()
```

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/common/grep.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/common/grep.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/common/tools.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/common/tools.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/ios/frida.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/ios/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/ios/ipa.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/ios/objection.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/ios/objection.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/ios/scp.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/ios/scp.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/ios/sib.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/ios/sib.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/commands/ios/ssh.py` & `linktools-0.8.3rc1/src/linktools/cli/commands/ios/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/cli/device.py` & `linktools-0.8.3rc1/src/linktools/cli/device.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/container/__init__.py` & `linktools-0.8.3rc1/src/linktools/container/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,9 +23,9 @@
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
    /  oooooooooooooooo  .o.  oooo /,   \,"-----------
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
-from .container import BaseContainer, ExposeLink, ExposeCategory
-from .manager import ContainerManager, ContainerError
+from .container import ContainerError, BaseContainer, ExposeLink, ExposeCategory
+from .manager import ContainerManager
```

### Comparing `linktools-0.8.3rc0/src/linktools/container/container.py` & `linktools-0.8.3rc1/src/linktools/container/container.py`

 * *Files 7% similar despite different names*

```diff
@@ -120,14 +120,18 @@
             self.render_template(
                 template,
                 nginx.get_app_path("conf.d", f"{domain}_confs", f"{name or self.name}.conf", create_parent=True),
                 DOMAIN=domain
             )
 
 
+class ContainerError(Exception):
+    pass
+
+
 class AbstractMetaClass(type):
 
     def __new__(mcs, name, bases, namespace):
         if "__abstract__" not in namespace:
             namespace["__abstract__"] = False
         return super().__new__(mcs, name, bases, namespace)
 
@@ -197,19 +201,25 @@
                         "driver": "json-file",
                         "options": {
                             "max-size": "10m",
                         }
                     })
                     if "image" not in service and "build" not in service:
                         path = self.get_docker_file_path()
-                        if path:
+                        if path and os.path.exists(path):
                             service["build"] = {
                                 "context": self.get_path(),
                                 "dockerfile": path
                             }
+                    if "env_file" not in service:
+                        path = self.get_path(".env")
+                        if path and os.path.exists(path):
+                            service["env_file"] = [
+                                path
+                            ]
                 return data
         return None
 
     @cached_property
     def docker_file(self) -> Optional[str]:
         path = self.get_path("Dockerfile")
         if os.path.exists(path):
@@ -237,35 +247,44 @@
 
     def on_stopped(self):
         pass
 
     def on_removed(self):
         pass
 
-    @subcommand("shell", help="exec into container using command sh", prefix_chars=chr(0))
-    @subcommand_argument("args", nargs="...")
-    def on_exec_shell(self, args: List[str]):
+    @subcommand("shell", help="exec into container using command sh")
+    @subcommand_argument("-c", "--command", help="shell command")
+    @subcommand_argument("--privileged", help="give extended privileges to the command")
+    @subcommand_argument("-u", "--user", help="Username or UID (format: \"<name|uid>[:<group|gid>]\")")
+    def on_exec_shell(self, command: str = None, privileged: bool = False, user: str = None):
         service = self.choose_service()
-        if not service:
-            self.logger.error(f"Not found any service in {self}")
-            return -1
+
+        options = []
+        if privileged:
+            options.append("--privileged")
+        if user:
+            options.append("--user")
+            options.append(user)
+
+        shell_args = []
+        if command:
+            shell_args = ["-c", command]
 
         commands = []
-        for command in ["/bin/zsh", "/bin/fish", "/bin/bash", "/bin/ash", "/bin/sh"]:
-            shell_args = ["-c", utils.list2cmdline(args)] if args else []
+        for shell in ["/bin/zsh", "/bin/fish", "/bin/bash", "/bin/ash", "/bin/sh"]:
             shell_command = [
-                "if" if len(commands) == 0 else "elif", "[", "-f", command, "]", ";",
-                "then", command, *shell_args, ";",
+                "if" if len(commands) == 0 else "elif", "[", "-f", shell, "]", ";",
+                "then", shell, *shell_args, ";",
             ]
             commands.extend(shell_command)
-        commands.extend(["else", "sh", ";"])
+        commands.extend(["else", "sh", *shell_args, ";"])
         commands.append("fi")
 
         return self.manager.create_docker_process(
-            "exec", "-it", service.get("container_name"),
+            "exec", "-it", *options, service.get("container_name"),
             "sh", "-c", utils.list2cmdline(commands)
         ).call()
 
     @subcommand("logs", help="fetch the logs of container")
     @subcommand_argument("-f", "--follow",
                          help="follow log output")
     @subcommand_argument("-t", "--timestamps",
@@ -275,17 +294,14 @@
     @subcommand_argument("--since", metavar="string",
                          help="show logs since timestamp (e.g. \"2013-01-02T13:23:37Z\") or relative (e.g. \"42m\" for 42 minutes)")
     @subcommand_argument("--until", metavar="string",
                          help="show logs before a timestamp (e.g. \"2013-01-02T13:23:37Z\") or relative (e.g. \"42m\" for 42 minutes)")
     def on_exec_logs(self, follow: bool = True, tail: str = None, timestamps: bool = True,
                      since: str = None, until: str = None):
         service = self.choose_service()
-        if not service:
-            self.logger.error(f"Not found any service in {self}")
-            return -1
 
         options = []
         if follow:
             options.append("--follow")
         if timestamps:
             options.append("--timestamps")
         if tail:
@@ -350,15 +366,15 @@
             create=create,
             create_parent=create_parent
         )
 
     def choose_service(self) -> Optional[Dict[str, Any]]:
         services = list(self.services.values())
         if len(services) == 0:
-            return None
+            raise ContainerError(f"Not found any service in {self}")
         if len(services) == 1:
             return services[0]
         index = choose(
             "Please choose service",
             choices=[service.get("container_name") for service in services],
             default=0
         )
@@ -406,29 +422,29 @@
             for next_name in current_items:
                 for next_dependency in self.manager.containers[next_name].dependencies:
                     if next_dependency not in exclude_items:
                         next_items.add(next_dependency)
         return False
 
     def render_template(self, source: str, destination: str = None, **kwargs: Any):
-        context = {
-            key: utils.lazy_load(self.manager.config.get, key)
-            for key in self.manager.config.keys()
-        }
+        config = self.manager.config
 
+        context = {key: utils.lazy_load(config.get, key) for key in config.keys()}
         context.update(kwargs)
-        context.setdefault("DEBUG", self.manager.debug)
 
-        context.setdefault("bool", lambda obj, default=False: self.manager.config.cast(obj, type=bool, default=default))
-        context.setdefault("str", lambda obj, default="": self.manager.config.cast(obj, type=str, default=default))
-        context.setdefault("int", lambda obj, default=0: self.manager.config.cast(obj, type=int, default=default))
-        context.setdefault("float", lambda obj, default=0.0: self.manager.config.cast(obj, type=float, default=default))
+        context.setdefault("DEBUG", self.manager.debug)
+        context.setdefault("bool", lambda obj, default=False: config.cast(obj, type=bool, default=default))
+        context.setdefault("str", lambda obj, default="": config.cast(obj, type=str, default=default))
+        context.setdefault("int", lambda obj, default=0: config.cast(obj, type=int, default=default))
+        context.setdefault("float", lambda obj, default=0.0: config.cast(obj, type=float, default=default))
+        context.setdefault("path", lambda obj, default="": config.cast(obj, type="path", default=default))
+        context.setdefault("json", lambda obj, default="": config.cast(obj, type="json", default=default))
 
         context.setdefault("manager", self.manager)
-        context.setdefault("config", self.manager.config)
+        context.setdefault("config", config)
         context.setdefault("container", self)
 
         template = Template(utils.read_file(source, text=True))
         result = template.render(context)
         if destination:
             utils.write_file(destination, result)
```

### Comparing `linktools-0.8.3rc0/src/linktools/container/manager.py` & `linktools-0.8.3rc1/src/linktools/container/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,61 +31,52 @@
 import os
 import os.path
 import shutil
 from typing import TYPE_CHECKING, Dict, Any, List, Union, Callable, Tuple, Set
 
 from filelock import FileLock
 
-from .container import BaseContainer, SimpleContainer
+from .container import BaseContainer, SimpleContainer, ContainerError
 from .repository import Repository
 from .. import utils, Config
 from .._environ import environ
 from ..decorator import cached_property
 
 if TYPE_CHECKING:
     from .._environ import BaseEnviron
 
 
-class ContainerError(Exception):
-    pass
-
-
 class ContainerManager:
 
     def __init__(self, environ: "BaseEnviron", name: str = "aio"):  # all_in_one
         self.user = utils.get_user()
         self.uid = utils.get_uid()
         self.gid = utils.get_gid()
 
+        self.system = environ.system
+        self.machine = environ.machine
+
         self.environ = environ
         self.logger = environ.get_logger("container")
 
         self.config = self.environ.wrap_config(namespace="container", prefix="")
         self.config.update_defaults(
             COMPOSE_PROJECT_NAME=name or self.environ.name,
-            DOCKER_USER=Config.Prompt(default=os.environ.get("SUDO_USER", self.user), cached=True),
-            DOCKER_PUID=Config.Lazy(lambda cfg: utils.get_uid(cfg.get("DOCKER_USER", type=str))),
-            DOCKER_PGID=Config.Lazy(lambda cfg: utils.get_gid(cfg.get("DOCKER_USER", type=str))),
+            DOCKER_USER=Config.Prompt(default=os.environ.get("SUDO_USER", self.user).replace(" ", ""), cached=True),
+            DOCKER_UID=Config.Lazy(lambda cfg: utils.get_uid(cfg.get("DOCKER_USER", type=str))),
+            DOCKER_GID=Config.Lazy(lambda cfg: utils.get_gid(cfg.get("DOCKER_USER", type=str))),
         )
 
         self.docker_container_name = "container.py"
         self.docker_compose_names = ("compose.yaml", "compose.yml", "docker-compose.yaml", "docker-compose.yml")
 
     @property
     def debug(self) -> bool:
         return os.environ.get("DEBUG", self.environ.debug)
 
-    @property
-    def system(self) -> str:
-        return self.environ.system
-
-    @property
-    def machine(self) -> str:
-        return self.environ.machine
-
     @cached_property
     def container_type(self) -> str:
         choices = ["docker", "docker-rootless", "podman"] \
             if self.system in ("darwin", "linux") and os.getuid() != 0 \
             else ["docker", "podman"]
         return self.config.get(
             "CONTAINER_TYPE",
```

### Comparing `linktools-0.8.3rc0/src/linktools/container/repository.py` & `linktools-0.8.3rc1/src/linktools/container/repository.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/decorator.py` & `linktools-0.8.3rc1/src/linktools/decorator.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/device.py` & `linktools-0.8.3rc1/src/linktools/device.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/frida/__init__.py` & `linktools-0.8.3rc1/src/linktools/frida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/frida/android.py` & `linktools-0.8.3rc1/src/linktools/frida/android.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/frida/app.py` & `linktools-0.8.3rc1/src/linktools/frida/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/frida/ios.py` & `linktools-0.8.3rc1/src/linktools/frida/ios.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/frida/script.py` & `linktools-0.8.3rc1/src/linktools/frida/script.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/frida/server.py` & `linktools-0.8.3rc1/src/linktools/frida/server.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/ida/__init__.py` & `linktools-0.8.3rc1/src/linktools/ida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/ida/ida.py` & `linktools-0.8.3rc1/src/linktools/ida/ida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/ios/ipa.py` & `linktools-0.8.3rc1/src/linktools/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/ios/sib.py` & `linktools-0.8.3rc1/src/linktools/ios/sib.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/metadata.py` & `linktools-0.8.3rc1/src/linktools/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 class __MissingType:
     __eq__ = lambda l, r: \
         l is r or type(l) is type(r)
 
 
 __name__ = "linktools"
 __release__ = True
-__version__ = "0.8.3rc0"
+__version__ = "0.8.3rc1"
 __missing__ = __MissingType()
 __description__ = f"""\
     ___       __   __              __
    / (_)___  / /__/ /_____  ____  / /____
-  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.3rc0)
+  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.3rc1)
  / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
 /_/_/_/ /_/_/|_|\\__/\\____/\\____/_/____/
 """
```

### Comparing `linktools-0.8.3rc0/src/linktools/reactor.py` & `linktools-0.8.3rc1/src/linktools/reactor.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/references/fake_useragent/fake.py` & `linktools-0.8.3rc1/src/linktools/references/fake_useragent/fake.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/references/fake_useragent/utils.py` & `linktools-0.8.3rc1/src/linktools/references/fake_useragent/utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/rich.py` & `linktools-0.8.3rc1/src/linktools/rich.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/ssh.py` & `linktools-0.8.3rc1/src/linktools/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/utils/__init__.py` & `linktools-0.8.3rc1/src/linktools/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,26 +24,25 @@
     ___________________________/___  `,
    /  oooooooooooooooo  .o.  oooo /,   \,"-----------
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
 from ._utils import (
-    timeoutable, Timeout,
-    InterruptableEvent,
+    timeoutable, Timeout, InterruptableEvent,
     ignore_error,
     cast, cast_int as int, cast_bool as bool,
     coalesce, is_contain, is_empty,
     get_item, pop_item, get_list_item,
     get_md5, get_sha1, get_sha256, make_uuid, gzip_compress,
     get_path, read_file, write_file,
     get_lan_ip, get_wan_ip,
     parse_version, get_char_width,
     make_url, parse_header, parser_cookie, guess_file_name, user_agent,
-    get_system, get_machine, get_user, get_uid, get_gid,
+    get_system, get_machine, get_user, get_uid, get_gid, get_shell_path,
 )
 
 from ._lazy import (
     get_derived_type, lazy_load, lazy_iter, lazy_raise, lazy_import, lazy_import_file
 )
 
 from ._subprocess import (
```

### Comparing `linktools-0.8.3rc0/src/linktools/utils/_lazy.py` & `linktools-0.8.3rc1/src/linktools/utils/_lazy.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/utils/_port.py` & `linktools-0.8.3rc1/src/linktools/utils/_port.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.3rc0/src/linktools/utils/_subprocess.py` & `linktools-0.8.3rc1/src/linktools/utils/_subprocess.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 # -*- coding:utf-8 -*-
 
 import errno
 import os
 import queue
 import subprocess
 import threading
-from typing import AnyStr, Tuple, Optional, IO, Callable, Any
+from typing import AnyStr, Tuple, Optional, IO, Callable, Any, Dict, Union
 
 from . import Timeout, timeoutable
 from .._environ import environ
 from ..decorator import cached_property
 
-
 list2cmdline = subprocess.list2cmdline
 
 
 class Output:
     STDOUT = 1
     STDERR = 2
 
@@ -84,39 +83,47 @@
                     yield flag, data
             except queue.Empty:
                 break
 
 
 class Process(subprocess.Popen):
 
-    def __init__(self, *args, **kwargs):
-        capture_output = kwargs.pop("capture_output", False)
+    def __init__(
+            self,
+            *args: Any,
+            capture_output: bool = False,
+            stdin: Union[int, IO] = None, stdout: Union[int, IO] = None, stderr: Union[int, IO] = None,
+            shell: bool = False, cwd: str = None,
+            env: Dict[str, str] = None, append_env: Dict[str, str] = None,
+            **kwargs,
+    ):
         if capture_output is True:
-            if kwargs.get("stdout") is not None or kwargs.get("stderr") is not None:
+            if stdout is not None or stderr is not None:
                 raise ValueError("stdout and stderr arguments may not be used "
                                  "with capture_output.")
-            kwargs["stdout"] = subprocess.PIPE
-            kwargs["stderr"] = subprocess.PIPE
-        if "cwd" not in kwargs:
+            stdout = subprocess.PIPE
+            stderr = subprocess.PIPE
+        if cwd:
             try:
-                kwargs["cwd"] = os.getcwd()
+                cwd = os.getcwd()
             except FileNotFoundError:
-                kwargs["cwd"] = environ.get_temp_dir(create=True)
-        if "append_env" in kwargs:
-            env = kwargs.pop("env", None)
-            env = dict(env) if env else dict()
-            env.update(kwargs.pop("append_env"))
-            for key, value in os.environ.items():
-                env.setdefault(key, value)
-            kwargs["env"] = env
-
-        args = [str(arg) for arg in args]
-        environ.logger.debug(f"Exec cmdline: {list2cmdline(args)}")
+                cwd = environ.get_temp_dir(create=True)
+        if append_env:
+            env = dict(env) if env else dict(os.environ)
+            env.update(append_env)
+
+        super().__init__(
+            [str(arg) for arg in args],
+            stdin=stdin, stdout=stdout, stderr=stderr,
+            shell=shell, cwd=cwd,
+            env=env,
+            **kwargs
+        )
 
-        super().__init__(args, **kwargs)
+        environ.logger.debug(f"Exec cmdline: {list2cmdline(self.args)}")
 
     @timeoutable
     def call(self, timeout: Timeout = None) -> int:
         with self:
             try:
                 return self.wait(timeout=timeout.remain)
             except Exception:
```

### Comparing `linktools-0.8.3rc0/src/linktools/utils/_utils.py` & `linktools-0.8.3rc1/src/linktools/utils/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import gzip
 import hashlib
 import inspect
 import os
 import platform
 import random
 import re
+import shutil
 import socket
 import threading
 import time
 import uuid
 from collections.abc import Iterable, Sized
 from typing import TYPE_CHECKING, Union, Callable, Optional, Type, Any, List, TypeVar, Tuple, Set, Dict
 from urllib import parse
@@ -690,7 +691,33 @@
         if user:
             import pwd
             return pwd.getpwnam(user).pw_gid
         else:
             return os.getgid()
     else:
         return 0
+
+
+def get_shell_path():
+    """
+    获取当前用户shell路径
+    """
+
+    if _SYSTEM in ["darwin", "linux"]:
+        if "SHELL" in os.environ:
+            shell_path = os.environ["SHELL"]
+            if shell_path and os.path.exists(shell_path):
+                return shell_path
+        try:
+            import pwd
+            return pwd.getpwnam(get_user()).pw_shell
+        except:
+            return shutil.which("zsh") or shutil.which("bash") or shutil.which("sh")
+
+    elif _SYSTEM in ["windows"]:
+        if "ComSpec" in os.environ:
+            shell_path = os.environ["ComSpec"]
+            if shell_path and os.path.exists(shell_path):
+                return shell_path
+        return shutil.which("powershell") or shutil.which("cmd")
+
+    return ""
```

### Comparing `linktools-0.8.3rc0/src/linktools.egg-info/PKG-INFO` & `linktools-0.8.3rc1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,7 @@
-Metadata-Version: 2.1
-Name: linktools
-Version: 0.8.3rc0
-Summary: linktools toolkit
-Author-email: Hu Ji <669898595@qq.com>
-License: Apache 2.0
-Project-URL: Homepage, https://github.com/ice-black-tea/linktools
-Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: rich
-Requires-Dist: filelock>=3.4.0
-Provides-Extra: requests
-Requires-Dist: requests[socks]; extra == "requests"
-Provides-Extra: frida
-Requires-Dist: frida>=15.0.0; extra == "frida"
-Provides-Extra: objection
-Requires-Dist: objection; extra == "objection"
-Provides-Extra: lief
-Requires-Dist: lief>0.10.1; extra == "lief"
-Requires-Dist: python-magic; platform_system == "Linux" and extra == "lief"
-Requires-Dist: python-magic; platform_system == "Darwin" and extra == "lief"
-Requires-Dist: python-magic-bin; platform_system == "Windows" and extra == "lief"
-Provides-Extra: ssh
-Requires-Dist: paramiko; extra == "ssh"
-Requires-Dist: scp; extra == "ssh"
-Provides-Extra: ssl
-Requires-Dist: pyOpenSSL; extra == "ssl"
-Provides-Extra: container
-Requires-Dist: GitPython; extra == "container"
-Requires-Dist: jinja2; extra == "container"
-Requires-Dist: pyyaml; extra == "container"
-Provides-Extra: all
-Requires-Dist: requests[socks]; extra == "all"
-Requires-Dist: frida>=15.0.0; extra == "all"
-Requires-Dist: objection; extra == "all"
-Requires-Dist: lief>0.10.1; extra == "all"
-Requires-Dist: python-magic; platform_system == "Linux" and extra == "all"
-Requires-Dist: python-magic; platform_system == "Darwin" and extra == "all"
-Requires-Dist: python-magic-bin; platform_system == "Windows" and extra == "all"
-Requires-Dist: paramiko; extra == "all"
-Requires-Dist: scp; extra == "all"
-Requires-Dist: pyOpenSSL; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: pyyaml; extra == "all"
-
 # Linktools Toolkit
 
 ## 开始使用
 
 ### 依赖项
 
 python & pip (3.6及以上): <https://www.python.org/downloads/>
@@ -102,34 +54,78 @@
 ├── 📖 at: Android scripts
 │   ├── 👉 adb: Adb supports managing multiple android devices
 │   ├── 👉 agent: Debug android-tools.apk
 │   ├── 👉 app: Fetch application info
 │   ├── 👉 debug: Debug app by jdb
 │   ├── 👉 frida: Easy to use frida (require Android device rooted)
 │   ├── 👉 info: Fetch device information
-│   ├── 👉 intent: Common intent actions
+│   ├── 📘 intent: Common intent actions
 │   ├── 👉 objection: Easy to use objection (require Android device rooted)
 │   ├── 👉 pidcat: Filter logcat by package name
 │   └── 👉 top: Fetch current running app's basic information
 ├── 📖 ct: Common scripts
-│   ├── 👉 cert: Display X.509 certificate information.
+│   ├── 👉 cert: Display X.509 certificate information
+│   ├── 📘 cntr: Deploy docker/pod containers
+│   ├── 📘 env: Linktools environment commands
 │   ├── 👉 grep: Match files with regular expression
-│   ├── 👉 shell: Shell with environment variables already initialized
 │   └── 👉 tools: Download and use tools
 └── 📖 it: iOS scripts
     ├── 👉 frida: Easy to use frida (require iOS device jailbreak)
-    ├── 👉 ipa: Parser ipa file
+    ├── 👉 ipa: Parse ipa file
     ├── 👉 objection: Easy to use objection (require iOS device jailbreak)
     ├── 👉 scp: OpenSSH secure file copy (require iOS device jailbreak)
     ├── 👉 sib: Sib supports managing multiple ios devices
     └── 👉 ssh: OpenSSH remote login client (require iOS device jailbreak)
 ```
 
 ### 通用功能（脚本前缀为ct-）
 
+#### 👉 ct-cntr
+
+<details>
+<summary>docker/pod容器一键部署工具，集成了包括nginx、nextcloud、redorid等等容器</summary>
+
+```
+$ ct-cntr -h
+usage: ct-cntr [-h] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [--version] COMMAND ...
+
+Deploy docker/pod containers
+
+    ___       __   __              __
+   / (_)___  / /__/ /_____  ____  / /____
+  / / / __ \/ //_/ __/ __ \/ __ \/ / ___/  linktools toolkit (v0.0.1.dev0)
+ / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
+/_/_/_/ /_/_/|_|\__/\____/\____/_/____/
+
+positional arguments:
+  COMMAND              Command Help
+    list               list all containers
+    add                add containers to installed list
+    remove             remove containers from installed list
+    info               display container info
+    up                 deploy installed containers
+    restart            restart installed containers
+    down               stop installed containers
+    exec               exec container command
+    config             manage container configs
+    repo               manage container repository
+
+options:
+  -h, --help           show this help message and exit
+  --version            show program's version number and exit
+
+log options:
+  --verbose            increase log verbosity
+  --debug              increase linktools's log verbosity, and enable debug mode
+  --time, --no-time    show log time
+  --level, --no-level  show log level
+```
+
+</details>
+
 #### 👉 ct-grep
 
 <details>
 <summary>类似linux中的grep，正则匹配文件内容 ，额外添加解析zip、elf等格等功能</summary>
 
 ```
 $ usage: ct-grep [-h] [--version] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [-i] pattern [file ...]
@@ -191,46 +187,14 @@
 
 log arguments:
   --verbose             increase log verbosity
   --debug               enable debug mode and increase log verbosity
   --time, --no-time     show log time
   --level, --no-level   show log level
 ```
-
-</details>
-
-#### 👉 ct-shell
-
-<details>
-<summary>已初始化常用工具环境变量的bash（mac/linux）、cmd（windows）</summary>
-
-```
-$ ct-shell -h
-usage: ct-shell [-h] [--version] [--verbose] [--debug] [--time | --no-time] [--level | --no-level] [-c COMMAND]
-
-Shell with environment variables already initialized
-
-    ___       __   __              __
-   / (_)___  / /__/ /_____  ____  / /____
-  / / / __ \/ //_/ __/ __ \/ __ \/ / ___/  linktools toolkit (v0.0.1.dev0)
- / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
-/_/_/_/ /_/_/|_|\__/\____/\____/_/____/
-
-options:
-  -h, --help            show this help message and exit
-  --version             show program's version number and exit
-  -c COMMAND, --command COMMAND
-                        shell command
-
-log arguments:
-  --verbose             increase log verbosity
-  --debug               enable debug mode and increase log verbosity
-  --time, --no-time     show log time
-  --level, --no-level   show log level
-```
 
 </details>
 
 ### android相关功能（脚本前缀为at-）
 
 #### 👉 at-adb
```

### Comparing `linktools-0.8.3rc0/src/linktools.egg-info/SOURCES.txt` & `linktools-0.8.3rc1/src/linktools.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 src/linktools/cli/commands/android/pidcat.py
 src/linktools/cli/commands/android/top.py
 src/linktools/cli/commands/common/__init__.py
 src/linktools/cli/commands/common/cert.py
 src/linktools/cli/commands/common/cntr.py
 src/linktools/cli/commands/common/env.py
 src/linktools/cli/commands/common/grep.py
-src/linktools/cli/commands/common/shell.py
 src/linktools/cli/commands/common/tools.py
 src/linktools/cli/commands/ios/__init__.py
 src/linktools/cli/commands/ios/frida.py
 src/linktools/cli/commands/ios/ipa.py
 src/linktools/cli/commands/ios/objection.py
 src/linktools/cli/commands/ios/scp.py
 src/linktools/cli/commands/ios/sib.py
```

### Comparing `linktools-0.8.3rc0/src/linktools.egg-info/entry_points.txt` & `linktools-0.8.3rc1/src/linktools.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 at-objection = linktools.cli.commands.android.objection:command.main
 at-pidcat = linktools.cli.commands.android.pidcat:command.main
 at-top = linktools.cli.commands.android.top:command.main
 ct-cert = linktools.cli.commands.common.cert:command.main
 ct-cntr = linktools.cli.commands.common.cntr:command.main
 ct-env = linktools.cli.commands.common.env:command.main
 ct-grep = linktools.cli.commands.common.grep:command.main
-ct-shell = linktools.cli.commands.common.shell:command.main
 ct-tools = linktools.cli.commands.common.tools:command.main
 it-frida = linktools.cli.commands.ios.frida:command.main
 it-ipa = linktools.cli.commands.ios.ipa:command.main
 it-objection = linktools.cli.commands.ios.objection:command.main
 it-scp = linktools.cli.commands.ios.scp:command.main
 it-sib = linktools.cli.commands.ios.sib:command.main
 it-ssh = linktools.cli.commands.ios.ssh:command.main
```

### Comparing `linktools-0.8.3rc0/src/linktools.egg-info/requires.txt` & `linktools-0.8.3rc1/src/linktools.egg-info/requires.txt`

 * *Files identical despite different names*

