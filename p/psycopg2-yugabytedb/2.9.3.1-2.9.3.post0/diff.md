# Comparing `tmp/psycopg2-yugabytedb-2.9.3.1.tar.gz` & `tmp/psycopg2-yugabytedb-2.9.3.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psycopg2-yugabytedb-2.9.3.1.tar", last modified: Fri Apr  5 01:46:05 2024, max compression
+gzip compressed data, was "psycopg2-yugabytedb-2.9.3.post0.tar", last modified: Thu Apr 14 04:58:43 2022, max compression
```

## Comparing `psycopg2-yugabytedb-2.9.3.1.tar` & `psycopg2-yugabytedb-2.9.3.post0.tar`

### file list

```diff
@@ -1,192 +1,191 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-05 01:46:05.818394 psycopg2-yugabytedb-2.9.3.1/
--rw-r--r--   0 root         (0) staff       (20)      475 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/AUTHORS
--rw-r--r--   0 root         (0) staff       (20)      155 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/INSTALL
--rw-r--r--   0 root         (0) staff       (20)     2238 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      398 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)     2542 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/Makefile
--rw-r--r--   0 root         (0) staff       (20)    54147 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/NEWS
--rw-r--r--   0 root         (0) staff       (20)     8254 2024-04-05 01:46:05.818534 psycopg2-yugabytedb-2.9.3.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     6676 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/README.rst
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-05 01:46:05.768971 psycopg2-yugabytedb-2.9.3.1/doc/
--rw-r--r--   0 root         (0) staff       (20)     7637 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/COPYING.LESSER
--rw-r--r--   0 root         (0) staff       (20)     1071 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/Makefile
--rw-r--r--   0 root         (0) staff       (20)      628 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/README.rst
--rw-r--r--   0 root         (0) staff       (20)     4178 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/SUCCESS
--rw-r--r--   0 root         (0) staff       (20)    39154 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/pep-0249.txt
--rw-r--r--   0 root         (0) staff       (20)      271 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/requirements.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-05 01:46:05.774672 psycopg2-yugabytedb-2.9.3.1/doc/src/
--rw-r--r--   0 root         (0) staff       (20)     3388 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/Makefile
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-05 01:46:05.775271 psycopg2-yugabytedb-2.9.3.1/doc/src/_static/
--rw-r--r--   0 root         (0) staff       (20)     1784 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/_static/psycopg.css
--rw-r--r--   0 root         (0) staff       (20)    22425 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/advanced.rst
--rw-r--r--   0 root         (0) staff       (20)     8766 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/conf.py
--rw-r--r--   0 root         (0) staff       (20)    34751 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/connection.rst
--rw-r--r--   0 root         (0) staff       (20)    24228 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/cursor.rst
--rw-r--r--   0 root         (0) staff       (20)     2514 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/errorcodes.rst
--rw-r--r--   0 root         (0) staff       (20)     3033 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/errors.rst
--rw-r--r--   0 root         (0) staff       (20)    33081 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/extensions.rst
--rw-r--r--   0 root         (0) staff       (20)    36663 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/extras.rst
--rw-r--r--   0 root         (0) staff       (20)    14989 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/faq.rst
--rw-r--r--   0 root         (0) staff       (20)     1894 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/index.rst
--rw-r--r--   0 root         (0) staff       (20)    11316 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/install.rst
--rw-r--r--   0 root         (0) staff       (20)       76 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/license.rst
--rw-r--r--   0 root         (0) staff       (20)    13348 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/module.rst
--rw-r--r--   0 root         (0) staff       (20)      108 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/news.rst
--rw-r--r--   0 root         (0) staff       (20)     1866 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/pool.rst
--rw-r--r--   0 root         (0) staff       (20)     4697 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/sql.rst
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-05 01:46:05.775429 psycopg2-yugabytedb-2.9.3.1/doc/src/tools/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-05 01:46:05.775893 psycopg2-yugabytedb-2.9.3.1/doc/src/tools/lib/
--rwxr-xr-x   0 root         (0) staff       (20)     1338 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/tools/lib/dbapi_extension.py
--rw-r--r--   0 root         (0) staff       (20)      500 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/tools/lib/sql_role.py
--rw-r--r--   0 root         (0) staff       (20)     1828 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/tools/lib/ticket_role.py
--rw-r--r--   0 root         (0) staff       (20)     1520 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/tools/make_sqlstate_docs.py
--rw-r--r--   0 root         (0) staff       (20)      646 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/tz.rst
--rw-r--r--   0 root         (0) staff       (20)    42328 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/doc/src/usage.rst
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-05 01:46:05.780375 psycopg2-yugabytedb-2.9.3.1/lib/
--rw-r--r--   0 root         (0) staff       (20)     9182 2024-03-27 11:37:17.000000 psycopg2-yugabytedb-2.9.3.1/lib/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     2922 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/lib/_ipaddress.py
--rw-r--r--   0 root         (0) staff       (20)     7153 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/lib/_json.py
--rw-r--r--   0 root         (0) staff       (20)    17608 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/lib/_range.py
--rw-r--r--   0 root         (0) staff       (20)    14308 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/lib/errorcodes.py
--rw-r--r--   0 root         (0) staff       (20)     1425 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/lib/errors.py
--rw-r--r--   0 root         (0) staff       (20)     7869 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/lib/extensions.py
--rw-r--r--   0 root         (0) staff       (20)    42863 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/lib/extras.py
--rw-r--r--   0 root         (0) staff       (20)     4656 2024-03-27 11:37:17.000000 psycopg2-yugabytedb-2.9.3.1/lib/loadbalanceproperties.py
--rw-r--r--   0 root         (0) staff       (20)    18922 2024-04-05 01:44:40.000000 psycopg2-yugabytedb-2.9.3.1/lib/policies.py
--rw-r--r--   0 root         (0) staff       (20)     6316 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/lib/pool.py
--rw-r--r--   0 root         (0) staff       (20)    14779 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/lib/sql.py
--rw-r--r--   0 root         (0) staff       (20)     4870 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/lib/tz.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-05 01:46:05.802407 psycopg2-yugabytedb-2.9.3.1/psycopg/
--rw-r--r--   0 root         (0) staff       (20)      644 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/_psycopg.vc9.amd64.manifest
--rw-r--r--   0 root         (0) staff       (20)      642 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/_psycopg.vc9.x86.manifest
--rw-r--r--   0 root         (0) staff       (20)     4928 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_asis.c
--rw-r--r--   0 root         (0) staff       (20)     1428 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_asis.h
--rw-r--r--   0 root         (0) staff       (20)     7399 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_binary.c
--rw-r--r--   0 root         (0) staff       (20)     1425 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_binary.h
--rw-r--r--   0 root         (0) staff       (20)    13521 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_datetime.c
--rw-r--r--   0 root         (0) staff       (20)     4018 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_datetime.h
--rw-r--r--   0 root         (0) staff       (20)     9352 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_list.c
--rw-r--r--   0 root         (0) staff       (20)     1403 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_list.h
--rw-r--r--   0 root         (0) staff       (20)     4912 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pboolean.c
--rw-r--r--   0 root         (0) staff       (20)     1455 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pboolean.h
--rw-r--r--   0 root         (0) staff       (20)     6472 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pdecimal.c
--rw-r--r--   0 root         (0) staff       (20)     1455 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pdecimal.h
--rw-r--r--   0 root         (0) staff       (20)     5757 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pfloat.c
--rw-r--r--   0 root         (0) staff       (20)     1441 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pfloat.h
--rw-r--r--   0 root         (0) staff       (20)     5663 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pint.c
--rw-r--r--   0 root         (0) staff       (20)     1435 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pint.h
--rw-r--r--   0 root         (0) staff       (20)     8185 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_qstring.c
--rw-r--r--   0 root         (0) staff       (20)     1474 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_qstring.h
--rw-r--r--   0 root         (0) staff       (20)     1854 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/aix_support.c
--rw-r--r--   0 root         (0) staff       (20)     1677 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/aix_support.h
--rw-r--r--   0 root         (0) staff       (20)    11046 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/bytes_format.c
--rw-r--r--   0 root         (0) staff       (20)     1540 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/column.h
--rw-r--r--   0 root         (0) staff       (20)    12071 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/column_type.c
--rw-r--r--   0 root         (0) staff       (20)     6468 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/config.h
--rw-r--r--   0 root         (0) staff       (20)     8892 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/connection.h
--rw-r--r--   0 root         (0) staff       (20)    40966 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/connection_int.c
--rw-r--r--   0 root         (0) staff       (20)    44501 2024-04-05 01:44:40.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/connection_type.c
--rw-r--r--   0 root         (0) staff       (20)     1374 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/conninfo.h
--rw-r--r--   0 root         (0) staff       (20)    18508 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/conninfo_type.c
--rw-r--r--   0 root         (0) staff       (20)     5501 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/cursor.h
--rw-r--r--   0 root         (0) staff       (20)     4808 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/cursor_int.c
--rw-r--r--   0 root         (0) staff       (20)    59927 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/cursor_type.c
--rw-r--r--   0 root         (0) staff       (20)     1423 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/diagnostics.h
--rw-r--r--   0 root         (0) staff       (20)     7095 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/diagnostics_type.c
--rw-r--r--   0 root         (0) staff       (20)     1646 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/error.h
--rw-r--r--   0 root         (0) staff       (20)    11429 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/error_type.c
--rw-r--r--   0 root         (0) staff       (20)     5995 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/green.c
--rw-r--r--   0 root         (0) staff       (20)     2781 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/green.h
--rw-r--r--   0 root         (0) staff       (20)     2712 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/libpq_support.c
--rw-r--r--   0 root         (0) staff       (20)     1908 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/libpq_support.h
--rw-r--r--   0 root         (0) staff       (20)     3719 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/lobject.h
--rw-r--r--   0 root         (0) staff       (20)    11996 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/lobject_int.c
--rw-r--r--   0 root         (0) staff       (20)    12549 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/lobject_type.c
--rw-r--r--   0 root         (0) staff       (20)     8137 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/microprotocols.c
--rw-r--r--   0 root         (0) staff       (20)     2247 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/microprotocols.h
--rw-r--r--   0 root         (0) staff       (20)     4853 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/microprotocols_proto.c
--rw-r--r--   0 root         (0) staff       (20)     1410 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/microprotocols_proto.h
--rw-r--r--   0 root         (0) staff       (20)     1348 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/notify.h
--rw-r--r--   0 root         (0) staff       (20)     9059 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/notify_type.c
--rw-r--r--   0 root         (0) staff       (20)     1501 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/pgtypes.h
--rw-r--r--   0 root         (0) staff       (20)    53540 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/pqpath.c
--rw-r--r--   0 root         (0) staff       (20)     3489 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/pqpath.h
--rw-r--r--   0 root         (0) staff       (20)     3113 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/psycopg.h
--rw-r--r--   0 root         (0) staff       (20)    31621 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/psycopgmodule.c
--rw-r--r--   0 root         (0) staff       (20)     3455 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/python.h
--rw-r--r--   0 root         (0) staff       (20)     1753 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/replication_connection.h
--rw-r--r--   0 root         (0) staff       (20)     6580 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/replication_connection_type.c
--rw-r--r--   0 root         (0) staff       (20)     2459 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/replication_cursor.h
--rw-r--r--   0 root         (0) staff       (20)    12012 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/replication_cursor_type.c
--rw-r--r--   0 root         (0) staff       (20)     1748 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/replication_message.h
--rw-r--r--   0 root         (0) staff       (20)     5606 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/replication_message_type.c
--rw-r--r--   0 root         (0) staff       (20)     1918 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/solaris_support.c
--rw-r--r--   0 root         (0) staff       (20)     1723 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/solaris_support.h
--rw-r--r--   0 root         (0) staff       (20)    11053 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/sqlstate_errors.h
--rw-r--r--   0 root         (0) staff       (20)    17651 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/typecast.c
--rw-r--r--   0 root         (0) staff       (20)     3172 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/typecast.h
--rw-r--r--   0 root         (0) staff       (20)     8944 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/typecast_array.c
--rw-r--r--   0 root         (0) staff       (20)     4146 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/typecast_basic.c
--rw-r--r--   0 root         (0) staff       (20)     8647 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/typecast_binary.c
--rw-r--r--   0 root         (0) staff       (20)     1533 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/typecast_binary.h
--rw-r--r--   0 root         (0) staff       (20)     4615 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/typecast_builtins.c
--rw-r--r--   0 root         (0) staff       (20)    14285 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/typecast_datetime.c
--rw-r--r--   0 root         (0) staff       (20)    11786 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/utils.c
--rw-r--r--   0 root         (0) staff       (20)     2336 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/utils.h
--rw-r--r--   0 root         (0) staff       (20)     2739 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/win32_support.c
--rw-r--r--   0 root         (0) staff       (20)     1804 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/win32_support.h
--rw-r--r--   0 root         (0) staff       (20)     1775 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/xid.h
--rw-r--r--   0 root         (0) staff       (20)    19411 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/psycopg/xid_type.c
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-05 01:46:05.804329 psycopg2-yugabytedb-2.9.3.1/psycopg2_yugabytedb.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     8254 2024-04-05 01:46:05.000000 psycopg2-yugabytedb-2.9.3.1/psycopg2_yugabytedb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     4047 2024-04-05 01:46:05.000000 psycopg2-yugabytedb-2.9.3.1/psycopg2_yugabytedb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-05 01:46:05.000000 psycopg2-yugabytedb-2.9.3.1/psycopg2_yugabytedb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)        9 2024-04-05 01:46:05.000000 psycopg2-yugabytedb-2.9.3.1/psycopg2_yugabytedb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-05 01:46:05.805073 psycopg2-yugabytedb-2.9.3.1/scripts/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-05 01:46:05.807513 psycopg2-yugabytedb-2.9.3.1/scripts/build/
--rwxr-xr-x   0 root         (0) staff       (20)    22465 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/scripts/build/appveyor.py
--rwxr-xr-x   0 root         (0) staff       (20)     3183 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/scripts/build/build_libpq.sh
--rwxr-xr-x   0 root         (0) staff       (20)     2552 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/scripts/build/build_macos.sh
--rwxr-xr-x   0 root         (0) staff       (20)     2446 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/scripts/build/build_manylinux2014.sh
--rwxr-xr-x   0 root         (0) staff       (20)     2457 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/scripts/build/build_manylinux_2_24.sh
--rwxr-xr-x   0 root         (0) staff       (20)      695 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/scripts/build/build_sdist.sh
--rwxr-xr-x   0 root         (0) staff       (20)     3306 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/scripts/build/download_packages_appveyor.py
--rwxr-xr-x   0 root         (0) staff       (20)     2874 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/scripts/build/download_packages_github.py
--rwxr-xr-x   0 root         (0) staff       (20)      960 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/scripts/build/strip_wheel.sh
--rwxr-xr-x   0 root         (0) staff       (20)     4629 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/scripts/make_errorcodes.py
--rwxr-xr-x   0 root         (0) staff       (20)     4267 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/scripts/make_errors.py
--rwxr-xr-x   0 root         (0) staff       (20)     3175 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/scripts/refcounter.py
--rw-r--r--   0 root         (0) staff       (20)      165 2024-04-05 01:46:05.818941 psycopg2-yugabytedb-2.9.3.1/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)    20953 2024-04-05 01:44:40.000000 psycopg2-yugabytedb-2.9.3.1/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-05 01:46:05.818025 psycopg2-yugabytedb-2.9.3.1/tests/
--rwxr-xr-x   0 root         (0) staff       (20)     3601 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    31821 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/dbapi20.py
--rw-r--r--   0 root         (0) staff       (20)     4137 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/dbapi20_tpc.py
--rwxr-xr-x   0 root         (0) staff       (20)    17919 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_async.py
--rwxr-xr-x   0 root         (0) staff       (20)     1783 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_bugX000.py
--rwxr-xr-x   0 root         (0) staff       (20)     1766 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_bug_gc.py
--rwxr-xr-x   0 root         (0) staff       (20)     3725 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_cancel.py
--rwxr-xr-x   0 root         (0) staff       (20)    69190 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_connection.py
--rwxr-xr-x   0 root         (0) staff       (20)    12640 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_copy.py
--rwxr-xr-x   0 root         (0) staff       (20)    25807 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_cursor.py
--rwxr-xr-x   0 root         (0) staff       (20)    23357 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_dates.py
--rwxr-xr-x   0 root         (0) staff       (20)     2524 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_errcodes.py
--rwxr-xr-x   0 root         (0) staff       (20)     3216 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_errors.py
--rwxr-xr-x   0 root         (0) staff       (20)    23864 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_extras_dictcursor.py
--rw-r--r--   0 root         (0) staff       (20)     5723 2024-04-05 01:44:40.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_fallback_topology.py
--rwxr-xr-x   0 root         (0) staff       (20)    10495 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_fast_executemany.py
--rwxr-xr-x   0 root         (0) staff       (20)     8411 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_green.py
--rwxr-xr-x   0 root         (0) staff       (20)     4326 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_ipaddress.py
--rwxr-xr-x   0 root         (0) staff       (20)    15473 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_lobject.py
--rwxr-xr-x   0 root         (0) staff       (20)    12365 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_module.py
--rwxr-xr-x   0 root         (0) staff       (20)     7899 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_notify.py
--rwxr-xr-x   0 root         (0) staff       (20)     2928 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_psycopg2_dbapi20.py
--rwxr-xr-x   0 root         (0) staff       (20)     8189 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_quote.py
--rwxr-xr-x   0 root         (0) staff       (20)     9058 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_replication.py
--rwxr-xr-x   0 root         (0) staff       (20)    15970 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_sql.py
--rwxr-xr-x   0 root         (0) staff       (20)     9432 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_transaction.py
--rwxr-xr-x   0 root         (0) staff       (20)    17653 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_types_basic.py
--rwxr-xr-x   0 root         (0) staff       (20)    56752 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_types_extras.py
--rwxr-xr-x   0 root         (0) staff       (20)    10479 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/test_with.py
--rw-r--r--   0 root         (0) staff       (20)     1505 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/testconfig.py
--rw-r--r--   0 root         (0) staff       (20)    16598 2024-03-08 05:33:39.000000 psycopg2-yugabytedb-2.9.3.1/tests/testutils.py
+drwxr-xr-x   0 sfurtisarah   (501) staff       (20)        0 2022-04-14 04:58:43.205531 psycopg2-yugabytedb-2.9.3.post0/
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)      475 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/AUTHORS
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)      155 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/INSTALL
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     2238 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/LICENSE
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)      398 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/MANIFEST.in
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     2542 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/Makefile
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    54147 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/NEWS
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     7494 2022-04-14 04:58:43.206379 psycopg2-yugabytedb-2.9.3.post0/PKG-INFO
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     5911 2022-04-14 04:57:14.000000 psycopg2-yugabytedb-2.9.3.post0/README.rst
+drwxr-xr-x   0 sfurtisarah   (501) staff       (20)        0 2022-04-14 04:58:42.694804 psycopg2-yugabytedb-2.9.3.post0/doc/
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     7637 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/COPYING.LESSER
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1071 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/Makefile
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)      628 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/README.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     4178 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/SUCCESS
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    39154 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/pep-0249.txt
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)      271 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/requirements.txt
+drwxr-xr-x   0 sfurtisarah   (501) staff       (20)        0 2022-04-14 04:58:42.733568 psycopg2-yugabytedb-2.9.3.post0/doc/src/
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     3388 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/Makefile
+drwxr-xr-x   0 sfurtisarah   (501) staff       (20)        0 2022-04-14 04:58:42.735322 psycopg2-yugabytedb-2.9.3.post0/doc/src/_static/
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1784 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/_static/psycopg.css
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    22425 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/advanced.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     8766 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/conf.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    34751 2022-04-14 04:57:14.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/connection.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    24228 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/cursor.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     2514 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/errorcodes.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     3033 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/errors.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    33081 2022-04-14 04:57:14.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/extensions.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    36663 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/extras.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    14989 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/faq.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1894 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/index.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    11316 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/install.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)       76 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/license.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    13348 2022-04-14 04:57:14.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/module.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)      108 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/news.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1866 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/pool.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     4697 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/sql.rst
+drwxr-xr-x   0 sfurtisarah   (501) staff       (20)        0 2022-04-14 04:58:42.737721 psycopg2-yugabytedb-2.9.3.post0/doc/src/tools/
+drwxr-xr-x   0 sfurtisarah   (501) staff       (20)        0 2022-04-14 04:58:42.752517 psycopg2-yugabytedb-2.9.3.post0/doc/src/tools/lib/
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     1338 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/tools/lib/dbapi_extension.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)      500 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/tools/lib/sql_role.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1828 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/tools/lib/ticket_role.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1520 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/tools/make_sqlstate_docs.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)      646 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/tz.rst
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    42328 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/doc/src/usage.rst
+drwxr-xr-x   0 sfurtisarah   (501) staff       (20)        0 2022-04-14 04:58:42.770308 psycopg2-yugabytedb-2.9.3.post0/lib/
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     8048 2022-04-14 04:57:14.000000 psycopg2-yugabytedb-2.9.3.post0/lib/__init__.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     2922 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/lib/_ipaddress.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     7153 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/lib/_json.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    17608 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/lib/_range.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    14308 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/lib/errorcodes.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1425 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/lib/errors.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     6969 2022-04-14 04:57:14.000000 psycopg2-yugabytedb-2.9.3.post0/lib/extensions.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    42863 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/lib/extras.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     3198 2022-04-14 04:57:14.000000 psycopg2-yugabytedb-2.9.3.post0/lib/loadbalanceproperties.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     6941 2022-04-14 04:57:14.000000 psycopg2-yugabytedb-2.9.3.post0/lib/policies.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     6316 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/lib/pool.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    14779 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/lib/sql.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     4870 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/lib/tz.py
+drwxr-xr-x   0 sfurtisarah   (501) staff       (20)        0 2022-04-14 04:58:43.091840 psycopg2-yugabytedb-2.9.3.post0/psycopg/
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)      644 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/_psycopg.vc9.amd64.manifest
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)      642 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/_psycopg.vc9.x86.manifest
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     4928 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_asis.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1428 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_asis.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     7399 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_binary.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1425 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_binary.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    13521 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_datetime.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     4018 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_datetime.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     9352 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_list.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1403 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_list.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     4912 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pboolean.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1455 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pboolean.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     6472 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pdecimal.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1455 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pdecimal.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     5757 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pfloat.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1441 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pfloat.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     5663 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pint.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1435 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pint.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     8185 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_qstring.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1474 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_qstring.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1854 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/aix_support.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1677 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/aix_support.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    11046 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/bytes_format.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1540 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/column.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    12071 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/column_type.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     6468 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/config.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     8892 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/connection.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    40966 2022-02-14 09:16:05.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/connection_int.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    44104 2022-04-14 04:57:14.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/connection_type.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1374 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/conninfo.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    18508 2022-04-14 04:57:14.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/conninfo_type.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     5501 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/cursor.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     4808 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/cursor_int.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    59927 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/cursor_type.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1423 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/diagnostics.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     7095 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/diagnostics_type.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1646 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/error.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    11429 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/error_type.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     5995 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/green.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     2781 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/green.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     2712 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/libpq_support.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1908 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/libpq_support.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     3719 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/lobject.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    11996 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/lobject_int.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    12549 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/lobject_type.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     8137 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/microprotocols.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     2247 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/microprotocols.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     4853 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/microprotocols_proto.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1410 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/microprotocols_proto.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1348 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/notify.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     9059 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/notify_type.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1501 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/pgtypes.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    53540 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/pqpath.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     3489 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/pqpath.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     3113 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/psycopg.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    31621 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/psycopgmodule.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     3455 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/python.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1753 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/replication_connection.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     6580 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/replication_connection_type.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     2459 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/replication_cursor.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    12012 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/replication_cursor_type.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1748 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/replication_message.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     5606 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/replication_message_type.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1918 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/solaris_support.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1723 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/solaris_support.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    11053 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/sqlstate_errors.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    17651 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     3172 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     8944 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast_array.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     4146 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast_basic.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     8647 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast_binary.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1533 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast_binary.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     4615 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast_builtins.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    14285 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast_datetime.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    11786 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/utils.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     2336 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/utils.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     2739 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/win32_support.c
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1804 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/win32_support.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1775 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/xid.h
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    19411 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg/xid_type.c
+drwxr-xr-x   0 sfurtisarah   (501) staff       (20)        0 2022-04-14 04:58:43.102375 psycopg2-yugabytedb-2.9.3.post0/psycopg2_yugabytedb.egg-info/
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     7494 2022-04-14 04:58:42.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg2_yugabytedb.egg-info/PKG-INFO
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     4015 2022-04-14 04:58:42.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg2_yugabytedb.egg-info/SOURCES.txt
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)        1 2022-04-14 04:58:42.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg2_yugabytedb.egg-info/dependency_links.txt
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)        9 2022-04-14 04:58:42.000000 psycopg2-yugabytedb-2.9.3.post0/psycopg2_yugabytedb.egg-info/top_level.txt
+drwxr-xr-x   0 sfurtisarah   (501) staff       (20)        0 2022-04-14 04:58:43.106788 psycopg2-yugabytedb-2.9.3.post0/scripts/
+drwxr-xr-x   0 sfurtisarah   (501) staff       (20)        0 2022-04-14 04:58:43.159449 psycopg2-yugabytedb-2.9.3.post0/scripts/build/
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)    22465 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/scripts/build/appveyor.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     3183 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/scripts/build/build_libpq.sh
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     2552 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/scripts/build/build_macos.sh
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     2446 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/scripts/build/build_manylinux2014.sh
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     2457 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/scripts/build/build_manylinux_2_24.sh
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)      695 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/scripts/build/build_sdist.sh
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     3306 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/scripts/build/download_packages_appveyor.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     2874 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/scripts/build/download_packages_github.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)      960 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/scripts/build/strip_wheel.sh
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     4629 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/scripts/make_errorcodes.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     4267 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/scripts/make_errors.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     3175 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/scripts/refcounter.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)      165 2022-04-14 04:58:43.208599 psycopg2-yugabytedb-2.9.3.post0/setup.cfg
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    20957 2022-04-14 04:57:14.000000 psycopg2-yugabytedb-2.9.3.post0/setup.py
+drwxr-xr-x   0 sfurtisarah   (501) staff       (20)        0 2022-04-14 04:58:43.203360 psycopg2-yugabytedb-2.9.3.post0/tests/
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     3601 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/__init__.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    31821 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/dbapi20.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     4137 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/dbapi20_tpc.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)    17919 2022-02-02 11:54:41.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_async.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     1783 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_bugX000.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     1766 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_bug_gc.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     3725 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_cancel.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)    69190 2022-01-31 07:53:39.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_connection.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)    12640 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_copy.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)    25807 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_cursor.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)    23357 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_dates.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     2524 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_errcodes.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     3216 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_errors.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)    23864 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_extras_dictcursor.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)    10495 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_fast_executemany.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     8411 2022-04-14 04:57:14.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_green.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     4326 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_ipaddress.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)    15473 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_lobject.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)    12365 2022-04-14 04:57:14.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_module.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     7899 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_notify.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     2928 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_psycopg2_dbapi20.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     8189 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_quote.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     9058 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_replication.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)    15970 2022-02-03 05:23:34.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_sql.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)     9432 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_transaction.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)    17653 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_types_basic.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)    56752 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_types_extras.py
+-rwxr-xr-x   0 sfurtisarah   (501) staff       (20)    10479 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/test_with.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)     1505 2022-03-03 23:15:12.000000 psycopg2-yugabytedb-2.9.3.post0/tests/testconfig.py
+-rw-r--r--   0 sfurtisarah   (501) staff       (20)    16598 2022-01-05 05:58:54.000000 psycopg2-yugabytedb-2.9.3.post0/tests/testutils.py
```

### Comparing `psycopg2-yugabytedb-2.9.3.1/LICENSE` & `psycopg2-yugabytedb-2.9.3.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/Makefile` & `psycopg2-yugabytedb-2.9.3.post0/Makefile`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/NEWS` & `psycopg2-yugabytedb-2.9.3.post0/NEWS`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/PKG-INFO` & `psycopg2-yugabytedb-2.9.3.post0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psycopg2-yugabytedb
-Version: 2.9.3.1
+Version: 2.9.3.post0
 Summary: psycopg2 - Python-PostgreSQL Database Adapter
 Home-page: https://psycopg.org/
 Author: Yugabyte
 Author-email: pypi@yugabyte.com
 Maintainer: Sfurti Sarah
 Maintainer-email: ssarah@yugabyte.com
 License: LGPL with exceptions
@@ -128,15 +128,14 @@
 
 Load balancing connection properties:
 
 The following connection properties need to be added to enable load balancing:
 
 * load_balance - enable cluster-aware load balancing by setting this property to True; disabled by default.
 * topology_keys - provide comma-separated geo-location values to enable topology-aware load balancing. Geo-locations can be provided as cloud.region.zone.
-* yb-servers-refresh-interval - The list of servers, to balance the connection load on, are refreshed periodically every 5 minutes by default. This time can be regulated by this property.
 
 Pass new connection properties for load balancing in the connection URL or in the dictionary. To enable uniform load balancing across all servers, you set the load-balance property to True in the URL, as per the following example.
 
 Connection String::
 
     conn = psycopg2.connect("dbname=database_name host=hostname port=port user=username  password=password load_balance=true")
 
@@ -150,14 +149,7 @@
 
     conn = psycopg2.connect("dbname=database_name host=hostname port=port user=username  password=password load_balance=true topology_keys=cloud1.region1.zone1,cloud2.region2.zone2")
 
 Connection Dictionary::
 
     conn = psycopg2.connect(user = 'username', password='xxx', host = 'hostname', port = 'port', dbname = 'database_name', load_balance='True', topology_keys='cloud1.region1.zone1,cloud2.region2.zone2')
 
-Multiple topologies can also be passed to the Topology Keys property, and each of them can also be given a preference value, as per the following example.::
-
-    conn = psycopg2.connect("host=127.0.0.1 port=5433 user=yugabyte dbname=yugabyte load_balance=True topology_keys=cloud1.region1.zone1:1,cloud2.region2.zone2:2")
-
-The preference value (appended after :) is optional. So it is compatible with previous syntax of specifying cloud placements.
-
-Preference value :1 means primary placement zone(s), value :2 means first fallback, value :3 means second fallback and so on.
```

### Comparing `psycopg2-yugabytedb-2.9.3.1/README.rst` & `psycopg2-yugabytedb-2.9.3.post0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 
 Load balancing connection properties:
 
 The following connection properties need to be added to enable load balancing:
 
 * load_balance - enable cluster-aware load balancing by setting this property to True; disabled by default.
 * topology_keys - provide comma-separated geo-location values to enable topology-aware load balancing. Geo-locations can be provided as cloud.region.zone.
-* yb-servers-refresh-interval - The list of servers, to balance the connection load on, are refreshed periodically every 5 minutes by default. This time can be regulated by this property.
 
 Pass new connection properties for load balancing in the connection URL or in the dictionary. To enable uniform load balancing across all servers, you set the load-balance property to True in the URL, as per the following example.
 
 Connection String::
 
     conn = psycopg2.connect("dbname=database_name host=hostname port=port user=username  password=password load_balance=true")
 
@@ -112,16 +111,8 @@
 
 Connection String::
 
     conn = psycopg2.connect("dbname=database_name host=hostname port=port user=username  password=password load_balance=true topology_keys=cloud1.region1.zone1,cloud2.region2.zone2")
 
 Connection Dictionary::
 
-    conn = psycopg2.connect(user = 'username', password='xxx', host = 'hostname', port = 'port', dbname = 'database_name', load_balance='True', topology_keys='cloud1.region1.zone1,cloud2.region2.zone2')
-
-Multiple topologies can also be passed to the Topology Keys property, and each of them can also be given a preference value, as per the following example.::
-
-    conn = psycopg2.connect("host=127.0.0.1 port=5433 user=yugabyte dbname=yugabyte load_balance=True topology_keys=cloud1.region1.zone1:1,cloud2.region2.zone2:2")
-
-The preference value (appended after :) is optional. So it is compatible with previous syntax of specifying cloud placements.
-
-Preference value :1 means primary placement zone(s), value :2 means first fallback, value :3 means second fallback and so on.
+    conn = psycopg2.connect(user = 'username', password='xxx', host = 'hostname', port = 'port', dbname = 'database_name', load_balance='True', topology_keys='cloud1.region1.zone1,cloud2.region2.zone2')
```

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/COPYING.LESSER` & `psycopg2-yugabytedb-2.9.3.post0/doc/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/Makefile` & `psycopg2-yugabytedb-2.9.3.post0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/README.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/README.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/SUCCESS` & `psycopg2-yugabytedb-2.9.3.post0/doc/SUCCESS`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/pep-0249.txt` & `psycopg2-yugabytedb-2.9.3.post0/doc/pep-0249.txt`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/Makefile` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/Makefile`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/_static/psycopg.css` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/_static/psycopg.css`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/advanced.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/advanced.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/conf.py` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/conf.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/connection.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/connection.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/cursor.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/cursor.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/errorcodes.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/errorcodes.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/errors.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/errors.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/extensions.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/extensions.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/extras.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/extras.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/faq.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/faq.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/index.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/index.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/install.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/install.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/module.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/module.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/pool.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/pool.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/sql.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/sql.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/tools/lib/dbapi_extension.py` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/tools/lib/dbapi_extension.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/tools/lib/ticket_role.py` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/tools/lib/ticket_role.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/tools/make_sqlstate_docs.py` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/tools/make_sqlstate_docs.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/tz.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/tz.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/doc/src/usage.rst` & `psycopg2-yugabytedb-2.9.3.post0/doc/src/usage.rst`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/lib/__init__.py` & `psycopg2-yugabytedb-2.9.3.post0/lib/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -151,23 +151,19 @@
     needsRefresh = loadbalancer.needsRefresh()
     if chosenHost == '' or needsRefresh:
         controlConnection = _connect(dsn, connection_factory=connection_factory, **kwasync)
         if cursor_factory is not None:
             controlConnection.cursor_factory = cursor_factory
         if not loadbalancer.refresh(controlConnection):
             return None
-        if chosenHost != '':
+        if needsRefresh:
             dsnhost = controlConnection.info.host_addr
             loadbalancer.updateConnectionMap(dsnhost, 1)
             loadbalancer.updateConnectionMap(chosenHost, -1)
-        
-        try:
-            controlConnection.close()
-        except Exception as e:
-            print("Could not close control connection:", str(e))
+        controlConnection.close()
 
         # Getting chosenHost again after refresh for the latest least loaded server
         
         chosenHost = loadbalancer.getLeastLoadedServer(failedHosts)
     
     if chosenHost == '':
         return None
@@ -176,52 +172,30 @@
         try :
             dsn = getDSNWithChosenHost(loadbalancer,dsn,chosenHost)
             newconn = _connect(dsn, connection_factory=connection_factory, **kwasync)
             if cursor_factory is not None:
                 newconn.cursor_factory = cursor_factory
             if not loadbalancer.refresh(newconn):
                 loadbalancer.updateConnectionMap(chosenHost, -1)
-                failedHosts.append(chosenHost)
+                failedHosts.add(chosenHost)
                 loadbalancer.setForRefresh()
             else:
-                better_node_available = loadbalancer.hasMorePreferredNodes(chosenHost)
-                if better_node_available:
-                    print('A higher level node is available')
-                    loadbalancer.decrementHostToNumConnCount(chosenHost)
-                    newconn.close()
-                    loadbalancer.has_better_node = False
-                    return getConnectionBalanced(lbprops, connection_factory, cursor_factory, **kwasync)
                 return newconn
         except OperationalError:
-            print('Couldn\'t connect to ', chosenHost, ' adding to failed list')
+            print('Couldnt connect to ', chosenHost, ' adding to failed list')
             failedHosts.append(chosenHost)
             loadbalancer.updateFailedHosts(chosenHost)
             try :
                 newconn.close()
             except Exception:
                 print('For cleanup purposes')
             chosenHost = loadbalancer.getLeastLoadedServer(failedHosts)
     
 def getDSNWithChosenHost(loadbalancer, dsn, chosenHost):
     port = loadbalancer.getPort(chosenHost)
-    """
-    Special case for connection URI
-    """
-    if 'postgresql://' in dsn or 'postgres://' in dsn:
-        if '@' in dsn :
-            host_parameter = '@' + chosenHost + ':' + str(port) + '/'
-            HostRegex = re.compile(r'@([^/]*)/')
-            dsn = HostRegex.sub(host_parameter, dsn)
-            return dsn
-        else :
-            host_parameter = '://' + chosenHost + ':' + str(port) + '/'
-            HostRegex = re.compile(r'://([^/]*)/')
-            dsn = HostRegex.sub(host_parameter, dsn)
-            return dsn
-
     host_parameter = 'host=' + chosenHost + ' '
     port_parameter = 'port=' + str(port) + ' '
     HostRegex = re.compile(r'host( )*=( )*(\S)*( )?')
     PortRegex = re.compile(r'port( )*=( )*[0-9]*(None)*( )?')
     dsn = HostRegex.sub(host_parameter, dsn)
     dsn = PortRegex.sub(port_parameter, dsn)
     return dsn
```

### Comparing `psycopg2-yugabytedb-2.9.3.1/lib/_ipaddress.py` & `psycopg2-yugabytedb-2.9.3.post0/lib/_ipaddress.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/lib/_json.py` & `psycopg2-yugabytedb-2.9.3.post0/lib/_json.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/lib/_range.py` & `psycopg2-yugabytedb-2.9.3.post0/lib/_range.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/lib/errorcodes.py` & `psycopg2-yugabytedb-2.9.3.post0/lib/errorcodes.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/lib/errors.py` & `psycopg2-yugabytedb-2.9.3.post0/lib/errors.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/lib/extensions.py` & `psycopg2-yugabytedb-2.9.3.post0/lib/extensions.py`

 * *Files 9% similar despite different names*

```diff
@@ -138,39 +138,20 @@
 def make_dsn(dsn=None, **kwargs):
     """Convert a set of keywords into a connection strings."""
     if dsn is None and not kwargs:
         return ''
 
     # If no kwarg is specified don't mung the dsn, but verify it
     if not kwargs:
-        # If port is not specified make 5433 the default port
         if not 'port' in dsn:
-            if 'postgresql://'  in dsn or 'postgres://'  in dsn:
-                if '@' in dsn :
-                    idx1 = dsn.index('@')
-                    idx2 = dsn.find('/', idx1)
-                    idx3  = dsn.find(':', idx1)
-                    if idx3 == -1 :
-                        res = dsn[idx1 + len('@') : idx2]
-                        newres = res + ':5433'
-                        dsn = dsn.replace(res,newres)
-                else :
-                    idx1 = dsn.index('://')
-                    idx2 = dsn.find('/', idx1 + len('://'))
-                    idx3  = dsn.find(':', idx1 + len('://'))
-                    if idx3 == -1 :
-                        res = dsn[idx1 + len('://') : idx2]
-                        newres = res + ':5433'
-                        dsn = dsn.replace(res,newres)
-            else: 
-                dsn += ' port=5433' 
+            dsn += ' port=5433' 
         parse_dsn(dsn)
         return dsn
     
-    #Set Default port to 5433 if not specified
+    #Set Default pot to 5433 if not specified
     if not 'port' in kwargs:
         kwargs['port'] = 5433
     # Override the dsn with the parameters
     if 'database' in kwargs:
         if 'dbname' in kwargs:
             raise TypeError(
                 "you can't specify both 'database' and 'dbname' arguments")
```

### Comparing `psycopg2-yugabytedb-2.9.3.1/lib/extras.py` & `psycopg2-yugabytedb-2.9.3.post0/lib/extras.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/lib/pool.py` & `psycopg2-yugabytedb-2.9.3.post0/lib/pool.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/lib/sql.py` & `psycopg2-yugabytedb-2.9.3.post0/lib/sql.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/lib/tz.py` & `psycopg2-yugabytedb-2.9.3.post0/lib/tz.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/_psycopg.vc9.amd64.manifest` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/_psycopg.vc9.amd64.manifest`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/_psycopg.vc9.x86.manifest` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/_psycopg.vc9.x86.manifest`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_asis.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_asis.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_asis.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_asis.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_binary.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_binary.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_binary.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_binary.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_datetime.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_datetime.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_datetime.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_datetime.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_list.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_list.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_list.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_list.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pboolean.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pboolean.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pboolean.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pboolean.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pdecimal.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pdecimal.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pdecimal.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pdecimal.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pfloat.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pfloat.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pfloat.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pfloat.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pint.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pint.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_pint.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_pint.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_qstring.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_qstring.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/adapter_qstring.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/adapter_qstring.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/aix_support.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/aix_support.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/aix_support.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/aix_support.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/bytes_format.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/bytes_format.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/column.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/column.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/column_type.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/column_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/config.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/config.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/connection.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/connection.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/connection_int.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/connection_int.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/connection_type.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/connection_type.c`

 * *Files 2% similar despite different names*

```diff
@@ -145,26 +145,17 @@
     /*
     *
     * Import the loadbalance module and get the appropriate loadbalancer
     *
     */
     PyObject *m = PyImport_ImportModule("psycopg2.loadbalanceproperties");
     PyObject *comp = PyObject_GetAttrString(m, "LoadBalanceProperties");
-    PyObject *pArgs = PyTuple_New(1);
-    PyTuple_SetItem(pArgs, 0, PyUnicode_FromString(self->dsn));
-    
-    // Create a dictionary for the second argument
-    PyObject *pDict = PyDict_New();
-    // Create keyword arguments for the constructor
-    PyObject *pKwargs = PyDict_New();
-    PyDict_SetItemString(pKwargs, "kwargs", pDict);
-    PyObject *instance = PyObject_Call(comp, pArgs, pKwargs);
     PyObject* loadbalancefunc = PyUnicode_FromString((char*)"getAppropriateLoadBalancer");
     PyObject *loadbalancer = PyObject_CallMethodObjArgs(
-                instance, loadbalancefunc, NULL);
+                comp, loadbalancefunc,comp, NULL);
 
     
     if (loadbalancer != NULL){
         const char *val;
         val = PQhostaddr(self->pgconn);
         if (!val) {
             Py_RETURN_NONE;
```

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/conninfo.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/conninfo.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/conninfo_type.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/conninfo_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/cursor.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/cursor.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/cursor_int.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/cursor_int.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/cursor_type.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/cursor_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/diagnostics.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/diagnostics.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/diagnostics_type.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/diagnostics_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/error.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/error.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/error_type.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/error_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/green.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/green.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/green.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/green.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/libpq_support.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/libpq_support.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/libpq_support.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/libpq_support.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/lobject.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/lobject.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/lobject_int.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/lobject_int.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/lobject_type.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/lobject_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/microprotocols.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/microprotocols.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/microprotocols.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/microprotocols.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/microprotocols_proto.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/microprotocols_proto.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/microprotocols_proto.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/microprotocols_proto.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/notify.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/notify.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/notify_type.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/notify_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/pgtypes.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/pgtypes.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/pqpath.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/pqpath.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/pqpath.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/pqpath.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/psycopg.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/psycopg.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/psycopgmodule.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/psycopgmodule.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/python.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/python.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/replication_connection.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/replication_connection.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/replication_connection_type.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/replication_connection_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/replication_cursor.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/replication_cursor.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/replication_cursor_type.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/replication_cursor_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/replication_message.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/replication_message.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/replication_message_type.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/replication_message_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/solaris_support.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/solaris_support.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/solaris_support.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/solaris_support.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/sqlstate_errors.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/sqlstate_errors.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/typecast.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/typecast.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/typecast_array.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast_array.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/typecast_basic.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast_basic.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/typecast_binary.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast_binary.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/typecast_binary.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast_binary.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/typecast_builtins.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast_builtins.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/typecast_datetime.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/typecast_datetime.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/utils.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/utils.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/utils.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/utils.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/win32_support.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/win32_support.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/win32_support.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/win32_support.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/xid.h` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/xid.h`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg/xid_type.c` & `psycopg2-yugabytedb-2.9.3.post0/psycopg/xid_type.c`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg2_yugabytedb.egg-info/PKG-INFO` & `psycopg2-yugabytedb-2.9.3.post0/psycopg2_yugabytedb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psycopg2-yugabytedb
-Version: 2.9.3.1
+Version: 2.9.3.post0
 Summary: psycopg2 - Python-PostgreSQL Database Adapter
 Home-page: https://psycopg.org/
 Author: Yugabyte
 Author-email: pypi@yugabyte.com
 Maintainer: Sfurti Sarah
 Maintainer-email: ssarah@yugabyte.com
 License: LGPL with exceptions
@@ -128,15 +128,14 @@
 
 Load balancing connection properties:
 
 The following connection properties need to be added to enable load balancing:
 
 * load_balance - enable cluster-aware load balancing by setting this property to True; disabled by default.
 * topology_keys - provide comma-separated geo-location values to enable topology-aware load balancing. Geo-locations can be provided as cloud.region.zone.
-* yb-servers-refresh-interval - The list of servers, to balance the connection load on, are refreshed periodically every 5 minutes by default. This time can be regulated by this property.
 
 Pass new connection properties for load balancing in the connection URL or in the dictionary. To enable uniform load balancing across all servers, you set the load-balance property to True in the URL, as per the following example.
 
 Connection String::
 
     conn = psycopg2.connect("dbname=database_name host=hostname port=port user=username  password=password load_balance=true")
 
@@ -150,14 +149,7 @@
 
     conn = psycopg2.connect("dbname=database_name host=hostname port=port user=username  password=password load_balance=true topology_keys=cloud1.region1.zone1,cloud2.region2.zone2")
 
 Connection Dictionary::
 
     conn = psycopg2.connect(user = 'username', password='xxx', host = 'hostname', port = 'port', dbname = 'database_name', load_balance='True', topology_keys='cloud1.region1.zone1,cloud2.region2.zone2')
 
-Multiple topologies can also be passed to the Topology Keys property, and each of them can also be given a preference value, as per the following example.::
-
-    conn = psycopg2.connect("host=127.0.0.1 port=5433 user=yugabyte dbname=yugabyte load_balance=True topology_keys=cloud1.region1.zone1:1,cloud2.region2.zone2:2")
-
-The preference value (appended after :) is optional. So it is compatible with previous syntax of specifying cloud placements.
-
-Preference value :1 means primary placement zone(s), value :2 means first fallback, value :3 means second fallback and so on.
```

### Comparing `psycopg2-yugabytedb-2.9.3.1/psycopg2_yugabytedb.egg-info/SOURCES.txt` & `psycopg2-yugabytedb-2.9.3.post0/psycopg2_yugabytedb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,14 @@
 tests/test_connection.py
 tests/test_copy.py
 tests/test_cursor.py
 tests/test_dates.py
 tests/test_errcodes.py
 tests/test_errors.py
 tests/test_extras_dictcursor.py
-tests/test_fallback_topology.py
 tests/test_fast_executemany.py
 tests/test_green.py
 tests/test_ipaddress.py
 tests/test_lobject.py
 tests/test_module.py
 tests/test_notify.py
 tests/test_psycopg2_dbapi20.py
```

### Comparing `psycopg2-yugabytedb-2.9.3.1/scripts/build/appveyor.py` & `psycopg2-yugabytedb-2.9.3.post0/scripts/build/appveyor.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/scripts/build/build_libpq.sh` & `psycopg2-yugabytedb-2.9.3.post0/scripts/build/build_libpq.sh`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/scripts/build/build_macos.sh` & `psycopg2-yugabytedb-2.9.3.post0/scripts/build/build_macos.sh`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/scripts/build/build_manylinux2014.sh` & `psycopg2-yugabytedb-2.9.3.post0/scripts/build/build_manylinux2014.sh`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/scripts/build/build_manylinux_2_24.sh` & `psycopg2-yugabytedb-2.9.3.post0/scripts/build/build_manylinux_2_24.sh`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/scripts/build/build_sdist.sh` & `psycopg2-yugabytedb-2.9.3.post0/scripts/build/build_sdist.sh`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/scripts/build/download_packages_appveyor.py` & `psycopg2-yugabytedb-2.9.3.post0/scripts/build/download_packages_appveyor.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/scripts/build/download_packages_github.py` & `psycopg2-yugabytedb-2.9.3.post0/scripts/build/download_packages_github.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/scripts/build/strip_wheel.sh` & `psycopg2-yugabytedb-2.9.3.post0/scripts/build/strip_wheel.sh`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/scripts/make_errorcodes.py` & `psycopg2-yugabytedb-2.9.3.post0/scripts/make_errorcodes.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/scripts/make_errors.py` & `psycopg2-yugabytedb-2.9.3.post0/scripts/make_errors.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/scripts/refcounter.py` & `psycopg2-yugabytedb-2.9.3.post0/scripts/refcounter.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/setup.py` & `psycopg2-yugabytedb-2.9.3.post0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     import configparser
 except ImportError:
     import ConfigParser as configparser
 
 # Take a look at https://www.python.org/dev/peps/pep-0440/
 # for a consistent versioning pattern.
 
-PSYCOPG_VERSION = '2.9.3.1'
+PSYCOPG_VERSION = '2.9.3.post0'
 
 
 # note: if you are changing the list of supported Python version please fix
 # the docs in install.rst and the /features/ page on the website.
 classifiers = """\
 Development Status :: 5 - Production/Stable
 Intended Audience :: Developers
```

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/__init__.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/dbapi20.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/dbapi20.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/dbapi20_tpc.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/dbapi20_tpc.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_async.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_bugX000.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_bugX000.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_bug_gc.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_bug_gc.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_cancel.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_cancel.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_connection.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_copy.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_cursor.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_dates.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_errcodes.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_errcodes.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_errors.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_extras_dictcursor.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_extras_dictcursor.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_fast_executemany.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_fast_executemany.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_green.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_green.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_ipaddress.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_ipaddress.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_lobject.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_lobject.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_module.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_notify.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_notify.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_psycopg2_dbapi20.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_psycopg2_dbapi20.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_quote.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_quote.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_replication.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_replication.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_sql.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_transaction.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_types_basic.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_types_basic.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_types_extras.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_types_extras.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/test_with.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/test_with.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/testconfig.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/testconfig.py`

 * *Files identical despite different names*

### Comparing `psycopg2-yugabytedb-2.9.3.1/tests/testutils.py` & `psycopg2-yugabytedb-2.9.3.post0/tests/testutils.py`

 * *Files identical despite different names*

