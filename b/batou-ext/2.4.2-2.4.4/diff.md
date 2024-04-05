# Comparing `tmp/batou_ext-2.4.2.tar.gz` & `tmp/batou_ext-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batou_ext-2.4.2.tar", last modified: Fri Dec  8 14:07:04 2023, max compression
+gzip compressed data, was "batou_ext-2.4.4.tar", last modified: Fri Apr  5 09:46:31 2024, max compression
```

## Comparing `batou_ext-2.4.2.tar` & `batou_ext-2.4.4.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2023-12-08 14:07:04.197990 batou_ext-2.4.2/
--rw-r--r--   0 zagy       (501) staff       (20)      362 2023-12-08 14:07:03.000000 batou_ext-2.4.2/CHANGES.md
--rw-r--r--   0 zagy       (501) staff       (20)     1608 2023-12-08 14:07:03.000000 batou_ext-2.4.2/LICENSE.txt
--rw-r--r--   0 zagy       (501) staff       (20)      144 2023-12-08 14:07:03.000000 batou_ext-2.4.2/MANIFEST.in
--rw-r--r--   0 zagy       (501) staff       (20)     1937 2023-12-08 14:07:04.197896 batou_ext-2.4.2/PKG-INFO
--rw-r--r--   0 zagy       (501) staff       (20)      660 2023-12-08 14:07:03.000000 batou_ext-2.4.2/README.md
--rw-r--r--   0 zagy       (501) staff       (20)      121 2023-12-08 14:07:03.000000 batou_ext-2.4.2/pyproject.toml
--rw-r--r--   0 zagy       (501) staff       (20)      491 2023-12-08 14:07:04.198257 batou_ext-2.4.2/setup.cfg
--rw-r--r--   0 zagy       (501) staff       (20)     1616 2023-12-08 14:07:03.000000 batou_ext-2.4.2/setup.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2023-12-08 14:07:04.187093 batou_ext-2.4.2/src/
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2023-12-08 14:07:04.192435 batou_ext-2.4.2/src/batou_ext/
--rw-r--r--   0 zagy       (501) staff       (20)       23 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/__init__.py
--rw-r--r--   0 zagy       (501) staff       (20)     1213 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/acl.py
--rw-r--r--   0 zagy       (501) staff       (20)     1080 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/archive.py
--rw-r--r--   0 zagy       (501) staff       (20)     3560 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/config.py
--rw-r--r--   0 zagy       (501) staff       (20)     6795 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/cron.py
--rw-r--r--   0 zagy       (501) staff       (20)    10472 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/fcio.py
--rw-r--r--   0 zagy       (501) staff       (20)     3631 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/file.py
--rw-r--r--   0 zagy       (501) staff       (20)     1498 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/geoip.py
--rw-r--r--   0 zagy       (501) staff       (20)     6059 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/git.py
--rw-r--r--   0 zagy       (501) staff       (20)      616 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/htpasswd.py
--rw-r--r--   0 zagy       (501) staff       (20)     1892 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/http.py
--rw-r--r--   0 zagy       (501) staff       (20)     4162 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/jenkins.py
--rw-r--r--   0 zagy       (501) staff       (20)      714 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/journalbeat.py
--rw-r--r--   0 zagy       (501) staff       (20)      831 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/keypair.py
--rw-r--r--   0 zagy       (501) staff       (20)     5500 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/mail.py
--rw-r--r--   0 zagy       (501) staff       (20)      245 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/mailhog.py
--rw-r--r--   0 zagy       (501) staff       (20)      972 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/memcached.py
--rw-r--r--   0 zagy       (501) staff       (20)     3325 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/mirror.py
--rw-r--r--   0 zagy       (501) staff       (20)     1512 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/mysql.py
--rw-r--r--   0 zagy       (501) staff       (20)      617 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/nfs.py
--rw-r--r--   0 zagy       (501) staff       (20)    23801 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/nix.py
--rw-r--r--   0 zagy       (501) staff       (20)     2214 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/nixos.py
--rw-r--r--   0 zagy       (501) staff       (20)     5407 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/oci.py
--rw-r--r--   0 zagy       (501) staff       (20)     3923 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/php.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2023-12-08 14:07:04.193799 batou_ext-2.4.2/src/batou_ext/postfixadmin/
--rw-r--r--   0 zagy       (501) staff       (20)     1997 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/postfixadmin/__init__.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2023-12-08 14:07:04.194030 batou_ext-2.4.2/src/batou_ext/postfixadmin/dovecot/
--rw-r--r--   0 zagy       (501) staff       (20)      751 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/postfixadmin/dovecot/database.conf
--rw-r--r--   0 zagy       (501) staff       (20)      447 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/postfixadmin/dovecot/local.conf
--rw-r--r--   0 zagy       (501) staff       (20)      584 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/postfixadmin/dovecot.py
--rw-r--r--   0 zagy       (501) staff       (20)      576 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/postfixadmin/goceptnet.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2023-12-08 14:07:04.194610 batou_ext-2.4.2/src/batou_ext/postfixadmin/postfix/
--rw-r--r--   0 zagy       (501) staff       (20)      668 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/postfixadmin/postfix/local.cf
--rw-r--r--   0 zagy       (501) staff       (20)      369 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_alias
--rw-r--r--   0 zagy       (501) staff       (20)      371 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_domains
--rw-r--r--   0 zagy       (501) staff       (20)      376 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_mailboxes
--rw-r--r--   0 zagy       (501) staff       (20)      457 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_sender_login
--rw-r--r--   0 zagy       (501) staff       (20)     1541 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/postfixadmin/postfix.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2023-12-08 14:07:04.194723 batou_ext-2.4.2/src/batou_ext/postfixadmin/postfixadmin/
--rw-r--r--   0 zagy       (501) staff       (20)      864 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/postfixadmin/postfixadmin/config.local.php
--rw-r--r--   0 zagy       (501) staff       (20)      607 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/postfixadmin/postgres.py
--rw-r--r--   0 zagy       (501) staff       (20)     5294 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/postgres.py
--rw-r--r--   0 zagy       (501) staff       (20)     3296 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/python.py
--rw-r--r--   0 zagy       (501) staff       (20)     5691 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/rabbitmq.py
--rw-r--r--   0 zagy       (501) staff       (20)     1268 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/redis.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2023-12-08 14:07:04.196187 batou_ext-2.4.2/src/batou_ext/resources/
--rw-r--r--   0 zagy       (501) staff       (20)      541 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/cert.sh
--rw-r--r--   0 zagy       (501) staff       (20)      388 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/check_systemd_unit.py
--rw-r--r--   0 zagy       (501) staff       (20)      117 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/cron-wrapper.sh
--rw-r--r--   0 zagy       (501) staff       (20)      200 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/geoip-update.sh
--rw-r--r--   0 zagy       (501) staff       (20)      203 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/journalbeat.nix
--rw-r--r--   0 zagy       (501) staff       (20)      955 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/loader.c
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2023-12-08 14:07:04.196296 batou_ext-2.4.2/src/batou_ext/resources/mailhog/
--rw-r--r--   0 zagy       (501) staff       (20)     1061 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/mailhog/mailhog.nix
--rw-r--r--   0 zagy       (501) staff       (20)      946 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/mirror.conf
--rw-r--r--   0 zagy       (501) staff       (20)     1635 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/oci-template.nix
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2023-12-08 14:07:04.196641 batou_ext-2.4.2/src/batou_ext/resources/php/
--rw-r--r--   0 zagy       (501) staff       (20)      588 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/php/php-fpm.conf
--rw-r--r--   0 zagy       (501) staff       (20)      296 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/php/php-fpm.sh
--rw-r--r--   0 zagy       (501) staff       (20)    71038 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/php/php.ini
--rw-r--r--   0 zagy       (501) staff       (20)      576 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/python.nix
--rw-r--r--   0 zagy       (501) staff       (20)      118 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/rediscleanup.sh
--rw-r--r--   0 zagy       (501) staff       (20)      560 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/setupEnv.sh
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2023-12-08 14:07:04.196807 batou_ext-2.4.2/src/batou_ext/resources/ssl/
--rw-r--r--   0 zagy       (501) staff       (20)      597 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/ssl/local_certificate_check.sh
--rw-r--r--   0 zagy       (501) staff       (20)      178 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/systemd.service
--rw-r--r--   0 zagy       (501) staff       (20)      617 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/resources/userenv.nix
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2023-12-08 14:07:04.197303 batou_ext-2.4.2/src/batou_ext/roundcube/
--rw-r--r--   0 zagy       (501) staff       (20)     3456 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/roundcube/__init__.py
--rw-r--r--   0 zagy       (501) staff       (20)     4181 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/roundcube/config.inc.php
--rw-r--r--   0 zagy       (501) staff       (20)      623 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/roundcube/postgres.py
--rw-r--r--   0 zagy       (501) staff       (20)     1525 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/run.py
--rw-r--r--   0 zagy       (501) staff       (20)     4745 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/s3.py
--rw-r--r--   0 zagy       (501) staff       (20)     3572 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/ssh.py
--rw-r--r--   0 zagy       (501) staff       (20)    11133 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/ssl.py
--rw-r--r--   0 zagy       (501) staff       (20)     4984 2023-12-08 14:07:03.000000 batou_ext-2.4.2/src/batou_ext/versions.py
-drwxr-xr-x   0 zagy       (501) staff       (20)        0 2023-12-08 14:07:04.193241 batou_ext-2.4.2/src/batou_ext.egg-info/
--rw-r--r--   0 zagy       (501) staff       (20)     1937 2023-12-08 14:07:04.000000 batou_ext-2.4.2/src/batou_ext.egg-info/PKG-INFO
--rw-r--r--   0 zagy       (501) staff       (20)     2579 2023-12-08 14:07:04.000000 batou_ext-2.4.2/src/batou_ext.egg-info/SOURCES.txt
--rw-r--r--   0 zagy       (501) staff       (20)        1 2023-12-08 14:07:04.000000 batou_ext-2.4.2/src/batou_ext.egg-info/dependency_links.txt
--rw-r--r--   0 zagy       (501) staff       (20)      113 2023-12-08 14:07:04.000000 batou_ext-2.4.2/src/batou_ext.egg-info/entry_points.txt
--rw-r--r--   0 zagy       (501) staff       (20)        1 2023-12-08 14:07:04.000000 batou_ext-2.4.2/src/batou_ext.egg-info/not-zip-safe
--rw-r--r--   0 zagy       (501) staff       (20)      109 2023-12-08 14:07:04.000000 batou_ext-2.4.2/src/batou_ext.egg-info/requires.txt
--rw-r--r--   0 zagy       (501) staff       (20)       10 2023-12-08 14:07:04.000000 batou_ext-2.4.2/src/batou_ext.egg-info/top_level.txt
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.855298 batou_ext-2.4.4/
+-rw-r--r--   0 flanitz    (501) staff       (20)      802 2024-04-05 09:46:30.000000 batou_ext-2.4.4/CHANGES.md
+-rw-r--r--   0 flanitz    (501) staff       (20)     1608 2024-04-05 09:46:30.000000 batou_ext-2.4.4/LICENSE.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)      144 2024-04-05 09:46:30.000000 batou_ext-2.4.4/MANIFEST.in
+-rw-r--r--   0 flanitz    (501) staff       (20)     2064 2024-04-05 09:46:31.855398 batou_ext-2.4.4/PKG-INFO
+-rw-r--r--   0 flanitz    (501) staff       (20)      660 2024-04-05 09:46:30.000000 batou_ext-2.4.4/README.md
+-rw-r--r--   0 flanitz    (501) staff       (20)      121 2024-04-05 09:46:30.000000 batou_ext-2.4.4/pyproject.toml
+-rw-r--r--   0 flanitz    (501) staff       (20)      491 2024-04-05 09:46:31.855785 batou_ext-2.4.4/setup.cfg
+-rw-r--r--   0 flanitz    (501) staff       (20)     1616 2024-04-05 09:46:30.000000 batou_ext-2.4.4/setup.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.844300 batou_ext-2.4.4/src/
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.850134 batou_ext-2.4.4/src/batou_ext/
+-rw-r--r--   0 flanitz    (501) staff       (20)       23 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/__init__.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1213 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/acl.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1080 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/archive.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3560 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/config.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     6795 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/cron.py
+-rw-r--r--   0 flanitz    (501) staff       (20)    10472 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/fcio.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3644 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/file.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1498 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/geoip.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     8165 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/git.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      616 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/htpasswd.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1892 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/http.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     4162 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/jenkins.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      714 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/journalbeat.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      831 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/keypair.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     5500 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/mail.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      245 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/mailhog.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      972 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/memcached.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3325 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/mirror.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1512 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/mysql.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      617 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/nfs.py
+-rw-r--r--   0 flanitz    (501) staff       (20)    24039 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/nix.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     2214 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/nixos.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     5424 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/oci.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3923 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/php.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.851464 batou_ext-2.4.4/src/batou_ext/postfixadmin/
+-rw-r--r--   0 flanitz    (501) staff       (20)     1997 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/__init__.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.851696 batou_ext-2.4.4/src/batou_ext/postfixadmin/dovecot/
+-rw-r--r--   0 flanitz    (501) staff       (20)      751 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/dovecot/database.conf
+-rw-r--r--   0 flanitz    (501) staff       (20)      447 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/dovecot/local.conf
+-rw-r--r--   0 flanitz    (501) staff       (20)      584 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/dovecot.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      576 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/goceptnet.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.852255 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix/
+-rw-r--r--   0 flanitz    (501) staff       (20)      668 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix/local.cf
+-rw-r--r--   0 flanitz    (501) staff       (20)      369 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_alias
+-rw-r--r--   0 flanitz    (501) staff       (20)      371 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_domains
+-rw-r--r--   0 flanitz    (501) staff       (20)      376 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_mailboxes
+-rw-r--r--   0 flanitz    (501) staff       (20)      457 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix/postfixadmin_virtual_sender_login
+-rw-r--r--   0 flanitz    (501) staff       (20)     1541 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.852367 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfixadmin/
+-rw-r--r--   0 flanitz    (501) staff       (20)      864 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postfixadmin/config.local.php
+-rw-r--r--   0 flanitz    (501) staff       (20)      607 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postfixadmin/postgres.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     5294 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/postgres.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3296 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/python.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     5691 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/rabbitmq.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1268 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/redis.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.853866 batou_ext-2.4.4/src/batou_ext/resources/
+-rw-r--r--   0 flanitz    (501) staff       (20)      541 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/cert.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      388 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/check_systemd_unit.py
+-rw-r--r--   0 flanitz    (501) staff       (20)      117 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/cron-wrapper.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      200 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/geoip-update.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      203 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/journalbeat.nix
+-rw-r--r--   0 flanitz    (501) staff       (20)      955 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/loader.c
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.854121 batou_ext-2.4.4/src/batou_ext/resources/mailhog/
+-rw-r--r--   0 flanitz    (501) staff       (20)     1061 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/mailhog/mailhog.nix
+-rw-r--r--   0 flanitz    (501) staff       (20)      946 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/mirror.conf
+-rw-r--r--   0 flanitz    (501) staff       (20)     1635 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/oci-template.nix
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.854549 batou_ext-2.4.4/src/batou_ext/resources/php/
+-rw-r--r--   0 flanitz    (501) staff       (20)      588 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/php/php-fpm.conf
+-rw-r--r--   0 flanitz    (501) staff       (20)      296 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/php/php-fpm.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)    71038 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/php/php.ini
+-rw-r--r--   0 flanitz    (501) staff       (20)      576 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/python.nix
+-rw-r--r--   0 flanitz    (501) staff       (20)      118 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/rediscleanup.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      560 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/setupEnv.sh
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.854738 batou_ext-2.4.4/src/batou_ext/resources/ssl/
+-rw-r--r--   0 flanitz    (501) staff       (20)      597 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/ssl/local_certificate_check.sh
+-rw-r--r--   0 flanitz    (501) staff       (20)      178 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/systemd.service
+-rw-r--r--   0 flanitz    (501) staff       (20)      617 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/resources/userenv.nix
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.855181 batou_ext-2.4.4/src/batou_ext/roundcube/
+-rw-r--r--   0 flanitz    (501) staff       (20)     3456 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/roundcube/__init__.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     4181 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/roundcube/config.inc.php
+-rw-r--r--   0 flanitz    (501) staff       (20)      623 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/roundcube/postgres.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     1525 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/run.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     4745 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/s3.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     3572 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/ssh.py
+-rw-r--r--   0 flanitz    (501) staff       (20)    11133 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/ssl.py
+-rw-r--r--   0 flanitz    (501) staff       (20)     4875 2024-04-05 09:46:30.000000 batou_ext-2.4.4/src/batou_ext/versions.py
+drwxr-xr-x   0 flanitz    (501) staff       (20)        0 2024-04-05 09:46:31.850923 batou_ext-2.4.4/src/batou_ext.egg-info/
+-rw-r--r--   0 flanitz    (501) staff       (20)     2064 2024-04-05 09:46:31.000000 batou_ext-2.4.4/src/batou_ext.egg-info/PKG-INFO
+-rw-r--r--   0 flanitz    (501) staff       (20)     2579 2024-04-05 09:46:31.000000 batou_ext-2.4.4/src/batou_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)        1 2024-04-05 09:46:31.000000 batou_ext-2.4.4/src/batou_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)      113 2024-04-05 09:46:31.000000 batou_ext-2.4.4/src/batou_ext.egg-info/entry_points.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)        1 2024-04-05 09:46:31.000000 batou_ext-2.4.4/src/batou_ext.egg-info/not-zip-safe
+-rw-r--r--   0 flanitz    (501) staff       (20)      109 2024-04-05 09:46:31.000000 batou_ext-2.4.4/src/batou_ext.egg-info/requires.txt
+-rw-r--r--   0 flanitz    (501) staff       (20)       10 2024-04-05 09:46:31.000000 batou_ext-2.4.4/src/batou_ext.egg-info/top_level.txt
```

### Comparing `batou_ext-2.4.2/LICENSE.txt` & `batou_ext-2.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/PKG-INFO` & `batou_ext-2.4.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 Metadata-Version: 2.1
 Name: batou_ext
-Version: 2.4.2
+Version: 2.4.4
 Summary: A library of components for batou.
 Home-page: https://github.com/flyingcircusio/batou_ext
 Author: Flying Circus <support@flyingcircus.io>
 Author-email: support@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: batou>=2.3b4
-Requires-Dist: pyaml
-Requires-Dist: setuptools
-Requires-Dist: six
 Provides-Extra: test
-Requires-Dist: boto3; extra == "test"
-Requires-Dist: passlib>=1.7; extra == "test"
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: version-select
-Requires-Dist: InquirerPy; extra == "version-select"
+License-File: LICENSE.txt
 
 # batou_ext - a library of components for batou
 
 `batou_ext` master is now supporting Python3 and is depending on batou2. If you still want to use batou_ext with batou 1.x running Python2 you still can use the [batou1-py2](https://github.com/flyingcircusio/batou_ext/tree/batou1-py2) branch.
 
 To add `batou_ext` to your deployment, add a like to the `requirements.txt` of your batou deployment::
 
@@ -39,14 +30,28 @@
 
 * Changes should be accompanied with a changelog entry. Use `./changelog.sh` to create one.
 
 * Releasing will create a tag and publishes the package to pypi. Use `./release-this.sh` to create a release.
 
 
 
+## 2.4.4 (2024-04-05)
+
+
+- Change the behaviour of the batou_ext.versions updater to allow environments to share a branch
+
+* Added a component `batou_ext.git.Remote` which allows to manipulate remotes of a git repository.
+
+
+## 2.4.3 (2024-01-17)
+
+
+- Improve output handling for the `PurgePackage` component. Will not appear like a fatal error in logs anymore when the package has been purged already or is not installed for another reason
+
+
 ## 2.4.2 (2023-12-08)
 
 
 * Make it possible to add arbitrary additional configuration to a service created by a `SystemdTimer()`.
 
 * Add `nixos.NixOSModule` to inject component attributes into .nix files.
```

### Comparing `batou_ext-2.4.2/README.md` & `batou_ext-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/setup.py` & `batou_ext-2.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def project_path(*names):
     return os.path.join(*names)
 
 
 setup(
     name="batou_ext",
-    version="2.4.2",
+    version="2.4.4",
     install_requires=[
         "batou >= 2.3b4",
         "pyaml",
         "setuptools",
         "six",
     ],
     extras_require={
```

### Comparing `batou_ext-2.4.2/src/batou_ext/acl.py` & `batou_ext-2.4.4/src/batou_ext/acl.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/archive.py` & `batou_ext-2.4.4/src/batou_ext/archive.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/config.py` & `batou_ext-2.4.4/src/batou_ext/config.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/cron.py` & `batou_ext-2.4.4/src/batou_ext/cron.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/fcio.py` & `batou_ext-2.4.4/src/batou_ext/fcio.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/file.py` & `batou_ext-2.4.4/src/batou_ext/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import glob
 import os
 import os.path
 import shutil
 import urllib.parse
 
+import batou
 import batou.component
 import batou.lib.file
 import batou.lib.git
 
 import batou_ext.ssh
```

### Comparing `batou_ext-2.4.2/src/batou_ext/geoip.py` & `batou_ext-2.4.4/src/batou_ext/geoip.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/git.py` & `batou_ext-2.4.4/src/batou_ext/git.py`

 * *Files 18% similar despite different names*

```diff
@@ -140,14 +140,76 @@
         with self.chdir(self.workingdir):
             stdout, stderr = self.cmd(
                 "git status --porcelain {{component.filename}}"
             )
         return bool(stdout.strip())
 
 
+class Remote(batou.component.Component):
+    """
+    Ensure that a git repository checkout out at `git_repo` has the origin
+    `name` pointing to `url`.
+
+    Usage::
+
+        self += batou_ext.git.Remote(
+            "/path/to/linux",
+            name="upstream",
+            url="ssh://git@github.com/torvalds/linux"
+        )
+
+    By default, the component aborts with an error if `git_repo` does not
+    exist or is not a git repository. This is not always desirable, for
+    instance when this is involved in migrating an existing `git_repo`
+    to a new remote: then, this works fine for migration, but not when
+    bootstrapping e.g. a new environment where `git_repo` doesn't exist
+    yet.
+
+    To solve that, it's possible to let the component do nothing if
+    `git_repo` doesn't exist like this:
+
+        self += batou_ext.git.Remote(
+            "/path/to/linux",
+            ignore_not_existing=True,
+            # ...
+        )
+    """
+
+    namevar = "git_repo"
+    url = batou.component.Attribute(str)
+    name = batou.component.Attribute(str, "origin")
+    ignore_not_existing = batou.component.Attribute(bool, False)
+
+    def verify(self):
+        if not os.path.exists(self.git_repo):
+            if self.ignore_not_existing:
+                return
+            else:
+                raise ValueError(
+                    f"batou_ext.git.Remote({self.git_repo}): path does not exist!"
+                )
+        elif not os.path.exists(f"{self.git_repo}/.git"):
+            raise ValueError(
+                f"batou_ext.git.Remote({self.git_repo}): not a git repository!"
+            )
+
+        with self.chdir(self.git_repo):
+            stdout, _ = self.cmd(
+                f"git remote get-url {self.name}", ignore_returncode=True
+            )
+            if self.url != stdout.strip():
+                raise batou.UpdateNeeded()
+
+    def update(self):
+        with self.chdir(self.git_repo):
+            stdout, _ = self.cmd("git remote")
+            verb = "set-url" if self.name in stdout.splitlines() else "add"
+            self.cmd(f"git remote {verb} {self.name} {self.url}")
+
+
 class Push(batou.component.Component):
     """`git push` if there are outgoing changes."""
 
     workingdir = "."
 
     def verify(self):
         if self.has_outgoing_changesets():
```

### Comparing `batou_ext-2.4.2/src/batou_ext/htpasswd.py` & `batou_ext-2.4.4/src/batou_ext/htpasswd.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/http.py` & `batou_ext-2.4.4/src/batou_ext/http.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/jenkins.py` & `batou_ext-2.4.4/src/batou_ext/jenkins.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/journalbeat.py` & `batou_ext-2.4.4/src/batou_ext/journalbeat.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/keypair.py` & `batou_ext-2.4.4/src/batou_ext/keypair.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/mail.py` & `batou_ext-2.4.4/src/batou_ext/mail.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/memcached.py` & `batou_ext-2.4.4/src/batou_ext/memcached.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/mirror.py` & `batou_ext-2.4.4/src/batou_ext/mirror.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/mysql.py` & `batou_ext-2.4.4/src/batou_ext/mysql.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/nfs.py` & `batou_ext-2.4.4/src/batou_ext/nfs.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/nix.py` & `batou_ext-2.4.4/src/batou_ext/nix.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,18 +88,24 @@
 
 
 class PurgePackage(batou.component.Component):
     namevar = "package"
 
     def verify(self):
         try:
-            self.cmd("nix-env --query {{component.package}}")
+            self.cmd(f"nix-env --query {self.package}")
             raise batou.UpdateNeeded()
         except batou.utils.CmdExecutionError as e:
-            e.report()
+            if e.stderr.endswith("matches no derivations"):
+                batou.output.annotate(
+                    f"Could not find package to purge: {self.package}",
+                    yellow=True,
+                )
+            else:
+                e.report()
 
     def update(self):
         self.cmd("nix-env --uninstall {{component.package}}")
 
 
 class UserEnv(batou.component.Component):
     """Provide a NixOS user environment.
```

### Comparing `batou_ext-2.4.2/src/batou_ext/nixos.py` & `batou_ext-2.4.4/src/batou_ext/nixos.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/oci.py` & `batou_ext-2.4.4/src/batou_ext/oci.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import hashlib
 import os
 import re
 import shlex
 from typing import Optional
 
+import batou
 import pkg_resources
 from batou import UpdateNeeded
 from batou.component import Attribute, Component
 from batou.lib.file import File
 from batou.lib.service import Service
 
 import batou_ext.nix
@@ -80,15 +81,15 @@
         "image": "mysql",
     }
 
     def configure(self):
         if (
             self.registry_user or self.registry_password
         ) and not self.registry_address:
-            batou.output.warn(
+            batou.output.annotate(
                 "WARN: you might want to specify the registry explicitly unless you really intend to log into the default docker registry"
             )
 
         if self.version:
             self.image = f"{self.image}:{self.version}"
 
         if self.registry_address and not self.image.startswith(
```

### Comparing `batou_ext-2.4.2/src/batou_ext/php.py` & `batou_ext-2.4.4/src/batou_ext/php.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/postfixadmin/__init__.py` & `batou_ext-2.4.4/src/batou_ext/postfixadmin/__init__.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/postfixadmin/dovecot/database.conf` & `batou_ext-2.4.4/src/batou_ext/postfixadmin/dovecot/database.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/postfixadmin/dovecot.py` & `batou_ext-2.4.4/src/batou_ext/postfixadmin/dovecot.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/postfixadmin/goceptnet.py` & `batou_ext-2.4.4/src/batou_ext/postfixadmin/goceptnet.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/postfixadmin/postfix/local.cf` & `batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix/local.cf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/postfixadmin/postfix.py` & `batou_ext-2.4.4/src/batou_ext/postfixadmin/postfix.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/postfixadmin/postfixadmin/config.local.php` & `batou_ext-2.4.4/src/batou_ext/postfixadmin/postfixadmin/config.local.php`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/postfixadmin/postgres.py` & `batou_ext-2.4.4/src/batou_ext/postfixadmin/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/postgres.py` & `batou_ext-2.4.4/src/batou_ext/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/python.py` & `batou_ext-2.4.4/src/batou_ext/python.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/rabbitmq.py` & `batou_ext-2.4.4/src/batou_ext/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/redis.py` & `batou_ext-2.4.4/src/batou_ext/redis.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/resources/cert.sh` & `batou_ext-2.4.4/src/batou_ext/resources/cert.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/resources/loader.c` & `batou_ext-2.4.4/src/batou_ext/resources/loader.c`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/resources/mailhog/mailhog.nix` & `batou_ext-2.4.4/src/batou_ext/resources/mailhog/mailhog.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/resources/mirror.conf` & `batou_ext-2.4.4/src/batou_ext/resources/mirror.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/resources/oci-template.nix` & `batou_ext-2.4.4/src/batou_ext/resources/oci-template.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/resources/php/php-fpm.conf` & `batou_ext-2.4.4/src/batou_ext/resources/php/php-fpm.conf`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/resources/php/php.ini` & `batou_ext-2.4.4/src/batou_ext/resources/php/php.ini`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/resources/python.nix` & `batou_ext-2.4.4/src/batou_ext/resources/python.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/resources/setupEnv.sh` & `batou_ext-2.4.4/src/batou_ext/resources/setupEnv.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/resources/ssl/local_certificate_check.sh` & `batou_ext-2.4.4/src/batou_ext/resources/ssl/local_certificate_check.sh`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/resources/userenv.nix` & `batou_ext-2.4.4/src/batou_ext/resources/userenv.nix`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/roundcube/__init__.py` & `batou_ext-2.4.4/src/batou_ext/roundcube/__init__.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/roundcube/config.inc.php` & `batou_ext-2.4.4/src/batou_ext/roundcube/config.inc.php`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/roundcube/postgres.py` & `batou_ext-2.4.4/src/batou_ext/roundcube/postgres.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/run.py` & `batou_ext-2.4.4/src/batou_ext/run.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/s3.py` & `batou_ext-2.4.4/src/batou_ext/s3.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/ssh.py` & `batou_ext-2.4.4/src/batou_ext/ssh.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/ssl.py` & `batou_ext-2.4.4/src/batou_ext/ssl.py`

 * *Files identical despite different names*

### Comparing `batou_ext-2.4.2/src/batou_ext/versions.py` & `batou_ext-2.4.4/src/batou_ext/versions.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,26 +43,24 @@
             assert self.environment_name
             self._environment = batou.environment.Environment(
                 self.environment_name
             )
             self._environment.load()
         return self._environment
 
-    def set_environment_from_branch(self, branch):
+    def update_from_branch(self, branch: str):
         envs = sorted(os.listdir(os.path.join(self.basedir, "environments")))
         for env_name in envs:
             env = batou.environment.Environment(env_name)
             env.load()
             if env.branch == branch:
-                if self.environment_name:
-                    raise ValueError(
-                        f"Branch {branch} is used in multiple enviornments, "
-                        "cannot auto-update."
-                    )
+                print(f"Updating environment: {env_name}")
                 self.environment_name = env_name
+                self.set_versions()
+
         if not self.environment_name:
             raise ValueError(
                 f"Branch {branch} is not used in any environment, "
                 "cannot auto-upate."
             )
 
     @property
@@ -153,16 +151,17 @@
 
     args = parser.parse_args()
 
     update = Updater(args.basedir)
 
     if args.environment:
         update.environment_name = args.environment
+        update.set_versions()
     elif args.branch:
-        update.set_environment_from_branch(args.branch)
+        update.update_from_branch(args.branch)
     else:
         update.interactive()
-    update.set_versions()
+        update.set_versions()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `batou_ext-2.4.2/src/batou_ext.egg-info/PKG-INFO` & `batou_ext-2.4.4/src/batou_ext.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 Metadata-Version: 2.1
 Name: batou-ext
-Version: 2.4.2
+Version: 2.4.4
 Summary: A library of components for batou.
 Home-page: https://github.com/flyingcircusio/batou_ext
 Author: Flying Circus <support@flyingcircus.io>
 Author-email: support@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: batou>=2.3b4
-Requires-Dist: pyaml
-Requires-Dist: setuptools
-Requires-Dist: six
 Provides-Extra: test
-Requires-Dist: boto3; extra == "test"
-Requires-Dist: passlib>=1.7; extra == "test"
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: version-select
-Requires-Dist: InquirerPy; extra == "version-select"
+License-File: LICENSE.txt
 
 # batou_ext - a library of components for batou
 
 `batou_ext` master is now supporting Python3 and is depending on batou2. If you still want to use batou_ext with batou 1.x running Python2 you still can use the [batou1-py2](https://github.com/flyingcircusio/batou_ext/tree/batou1-py2) branch.
 
 To add `batou_ext` to your deployment, add a like to the `requirements.txt` of your batou deployment::
 
@@ -39,14 +30,28 @@
 
 * Changes should be accompanied with a changelog entry. Use `./changelog.sh` to create one.
 
 * Releasing will create a tag and publishes the package to pypi. Use `./release-this.sh` to create a release.
 
 
 
+## 2.4.4 (2024-04-05)
+
+
+- Change the behaviour of the batou_ext.versions updater to allow environments to share a branch
+
+* Added a component `batou_ext.git.Remote` which allows to manipulate remotes of a git repository.
+
+
+## 2.4.3 (2024-01-17)
+
+
+- Improve output handling for the `PurgePackage` component. Will not appear like a fatal error in logs anymore when the package has been purged already or is not installed for another reason
+
+
 ## 2.4.2 (2023-12-08)
 
 
 * Make it possible to add arbitrary additional configuration to a service created by a `SystemdTimer()`.
 
 * Add `nixos.NixOSModule` to inject component attributes into .nix files.
```

### Comparing `batou_ext-2.4.2/src/batou_ext.egg-info/SOURCES.txt` & `batou_ext-2.4.4/src/batou_ext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

