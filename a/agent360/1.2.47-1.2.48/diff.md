# Comparing `tmp/agent360-1.2.47.tar.gz` & `tmp/agent360-1.2.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent360-1.2.47.tar", last modified: Fri Sep 29 20:04:20 2023, max compression
+gzip compressed data, was "agent360-1.2.48.tar", last modified: Fri Apr  5 15:39:44 2024, max compression
```

## Comparing `agent360-1.2.47.tar` & `agent360-1.2.48.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 20:04:20.655636 agent360-1.2.47/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-09-29 20:04:11.000000 agent360-1.2.47/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-29 20:04:11.000000 agent360-1.2.47/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2023-09-29 20:04:20.655636 agent360-1.2.47/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2023-09-29 20:04:11.000000 agent360-1.2.47/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 20:04:20.647636 agent360-1.2.47/agent360/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27744 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/agent360.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 20:04:20.655636 agent360-1.2.47/agent360/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/apt-updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/asterisk.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/bird.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/bitninja.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/cloudlinux-dbgov.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/cloudlinux.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/cpanel.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2020 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/cpu_freq.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/dirsize.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/diskinodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/diskstatus-nvme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/diskstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4140 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/diskusage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/dovecot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/exim.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/fail2ban.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/haproxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/httpd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5227 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/iostat.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/janus.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/kamailio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/litespeed.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      332 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/loadavg.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/loggedin.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/mailq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/mdstat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/megacli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/memcached.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      932 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/minecraft.py
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/nginx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/openvpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/phpfpm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3165 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/ping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6330 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/plesk-cgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/postfix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/powerdns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/proftpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/redis_stat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      244 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/sleeper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/swap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/tcpports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/temp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/unbound.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/vms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/wp-toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360/plugins/yum-updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2023-09-29 20:04:11.000000 agent360-1.2.47/agent360-example.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-29 20:04:20.647636 agent360-1.2.47/agent360.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2023-09-29 20:04:20.000000 agent360-1.2.47/agent360.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-09-29 20:04:20.000000 agent360-1.2.47/agent360.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-29 20:04:20.000000 agent360-1.2.47/agent360.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-09-29 20:04:20.000000 agent360-1.2.47/agent360.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-09-29 20:04:20.000000 agent360-1.2.47/agent360.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-29 20:04:20.000000 agent360-1.2.47/agent360.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-29 20:04:20.655636 agent360-1.2.47/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-09-29 20:04:11.000000 agent360-1.2.47/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:39:44.140929 agent360-1.2.48/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-05 15:39:38.000000 agent360-1.2.48/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 15:39:38.000000 agent360-1.2.48/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-05 15:39:44.140929 agent360-1.2.48/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-05 15:39:38.000000 agent360-1.2.48/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:39:44.132929 agent360-1.2.48/agent360/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27744 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/agent360.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:39:44.140929 agent360-1.2.48/agent360/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/apt-updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/asterisk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/bird.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/bitninja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/cloudlinux-dbgov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/cloudlinux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/cpanel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2020 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/cpu_freq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/dirsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/diskinodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/diskstatus-nvme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/diskstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4140 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/diskusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/dovecot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/exim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/fail2ban.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/haproxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/httpd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5227 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/iostat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/janus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/kamailio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/litespeed.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      332 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/loadavg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/loggedin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/mailq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/mdstat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/megacli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/memcached.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      932 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/minecraft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/openvpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/phpfpm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3165 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/ping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6330 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/plesk-cgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/postfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/powerdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/proftpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/redis_stat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/sleeper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/swap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/tcpports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/temp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/unbound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/vms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/wp-toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360/plugins/yum-updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 15:39:38.000000 agent360-1.2.48/agent360-example.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 15:39:44.140929 agent360-1.2.48/agent360.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-05 15:39:44.000000 agent360-1.2.48/agent360.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-05 15:39:44.000000 agent360-1.2.48/agent360.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 15:39:44.000000 agent360-1.2.48/agent360.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 15:39:44.000000 agent360-1.2.48/agent360.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-05 15:39:44.000000 agent360-1.2.48/agent360.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 15:39:44.000000 agent360-1.2.48/agent360.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 15:39:44.140929 agent360-1.2.48/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-05 15:39:38.000000 agent360-1.2.48/setup.py
```

### Comparing `agent360-1.2.47/LICENSE` & `agent360-1.2.48/LICENSE`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/PKG-INFO` & `agent360-1.2.48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent360
-Version: 1.2.47
+Version: 1.2.48
 Summary: 360 agent
 Home-page: https://github.com/plesk/agent360
 Author: 360
 Author-email: 360support@webpros.com
 Maintainer: 360
 Maintainer-email: 360support@webpros.com
 License: BSD-3-Clause
```

### Comparing `agent360-1.2.47/README.md` & `agent360-1.2.48/README.md`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/agent360.py` & `agent360-1.2.48/agent360/agent360.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     from urllib.request import urlopen, Request
     from urllib.error import HTTPError
 except ImportError:
     from urlparse import urlparse
     from urllib import urlencode
     from urllib2 import urlopen, Request, HTTPError
 
-__version__ = '1.2.47'
+__version__ = '1.2.48'
 __FILEABSDIRNAME__ = os.path.dirname(os.path.abspath(__file__))
 
 ini_files = (
     os.path.join('/etc', 'agent360.ini'),
     os.path.join('/etc', 'agent360-custom.ini'),
     os.path.join('/etc', 'agent360-token.ini'),
     os.path.join(os.path.dirname(__FILEABSDIRNAME__), 'agent360.ini'),
```

### Comparing `agent360-1.2.47/agent360/plugins/apt-updates.py` & `agent360-1.2.48/agent360/plugins/apt-updates.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/asterisk.py` & `agent360-1.2.48/agent360/plugins/asterisk.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/bind.py` & `agent360-1.2.48/agent360/plugins/bind.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/bird.py` & `agent360-1.2.48/agent360/plugins/bird.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/bitninja.py` & `agent360-1.2.48/agent360/plugins/bitninja.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/cloudlinux-dbgov.py` & `agent360-1.2.48/agent360/plugins/cloudlinux-dbgov.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/cloudlinux.py` & `agent360-1.2.48/agent360/plugins/cloudlinux.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/cpanel.py` & `agent360-1.2.48/agent360/plugins/cpanel.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/cpu.py` & `agent360-1.2.48/agent360/plugins/cpu.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/cpu_freq.py` & `agent360-1.2.48/agent360/plugins/cpu_freq.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/dirsize.py` & `agent360-1.2.48/agent360/plugins/dirsize.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/diskinodes.py` & `agent360-1.2.48/agent360/plugins/diskinodes.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/diskstatus-nvme.py` & `agent360-1.2.48/agent360/plugins/diskstatus-nvme.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/diskstatus.py` & `agent360-1.2.48/agent360/plugins/diskstatus.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/diskusage.py` & `agent360-1.2.48/agent360/plugins/diskusage.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/docker.py` & `agent360-1.2.48/agent360/plugins/docker.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/dovecot.py` & `agent360-1.2.48/agent360/plugins/dovecot.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/elasticsearch.py` & `agent360-1.2.48/agent360/plugins/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/fail2ban.py` & `agent360-1.2.48/agent360/plugins/fail2ban.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/gpu.py` & `agent360-1.2.48/agent360/plugins/gpu.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/haproxy.py` & `agent360-1.2.48/agent360/plugins/haproxy.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/httpd.py` & `agent360-1.2.48/agent360/plugins/httpd.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/iostat.py` & `agent360-1.2.48/agent360/plugins/iostat.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/janus.py` & `agent360-1.2.48/agent360/plugins/janus.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/kamailio.py` & `agent360-1.2.48/agent360/plugins/kamailio.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/litespeed.py` & `agent360-1.2.48/agent360/plugins/litespeed.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/mailq.py` & `agent360-1.2.48/agent360/plugins/mailq.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/mdstat.py` & `agent360-1.2.48/agent360/plugins/mdstat.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/megacli.py` & `agent360-1.2.48/agent360/plugins/megacli.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/memcached.py` & `agent360-1.2.48/agent360/plugins/memcached.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/memory.py` & `agent360-1.2.48/agent360/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/minecraft.py` & `agent360-1.2.48/agent360/plugins/minecraft.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/mongodb.py` & `agent360-1.2.48/agent360/plugins/mongodb.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/mysql.py` & `agent360-1.2.48/agent360/plugins/mysql.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/network.py` & `agent360-1.2.48/agent360/plugins/network.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/nginx.py` & `agent360-1.2.48/agent360/plugins/nginx.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/openvpn.py` & `agent360-1.2.48/agent360/plugins/openvpn.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/phpfpm.py` & `agent360-1.2.48/agent360/plugins/phpfpm.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/ping.py` & `agent360-1.2.48/agent360/plugins/ping.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/plesk-cgroups.py` & `agent360-1.2.48/agent360/plugins/plesk-cgroups.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/plugins.py` & `agent360-1.2.48/agent360/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/postfix.py` & `agent360-1.2.48/agent360/plugins/postfix.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/powerdns.py` & `agent360-1.2.48/agent360/plugins/powerdns.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/process.py` & `agent360-1.2.48/agent360/plugins/process.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/proftpd.py` & `agent360-1.2.48/agent360/plugins/proftpd.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/rabbitmq.py` & `agent360-1.2.48/agent360/plugins/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/redis_stat.py` & `agent360-1.2.48/agent360/plugins/redis_stat.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/system.py` & `agent360-1.2.48/agent360/plugins/system.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,14 +36,36 @@
         Stderr = Error.split("\n")
     else:
         Stderr = []
 
     return (Stdout, Stderr)
 
 
+def linux_hardware_memory():
+    block_size = 0
+    try:
+        with open("/sys/devices/system/memory/block_size_bytes", "r") as f:
+            block_size = int(f.readline().strip(), 16)
+
+        memory = 0
+        with os.scandir("/sys/devices/system/memory/") as it:
+            for entry in it:
+                if not entry.name.startswith("memory"):
+                    continue
+                with open(entry.path + "/state", "r") as f:
+                    if "online" != f.readline().strip():
+                        continue
+                    else:
+                        memory += block_size
+
+        return memory
+    except Exception:
+        return 0
+
+
 def ip_addresses():
     ip_list = {}
     ip_list['v4'] = {}
     ip_list['v6'] = {}
     if netifaces is None:
         return ip_list
     for interface in netifaces.interfaces():
@@ -89,16 +111,20 @@
                     if line.strip():
                         if "Model name" == line.rstrip('\n').split(':')[0].strip():
                             cpu['brand'] = line.rstrip('\n').split(':')[1].strip()
                         if "Processor" == line.rstrip('\n').split(':')[0].strip():
                             cpu['brand'] = line.rstrip('\n').split(':')[1].strip()
                         if "CPU(s)" == line.rstrip('\n').split(':')[0].strip():
                             cpu['count'] = line.rstrip('\n').split(':')[1].strip()
-        mem = psutil.virtual_memory()
+        mem = psutil.virtual_memory().total
         if sys.platform == "linux" or sys.platform == "linux2":
+            hw_mem = linux_hardware_memory()
+            if hw_mem != 0:
+                mem = hw_mem
+
             if distro is None:
                 systeminfo['os'] = str(' '.join(platform.linux_distribution()))
             else:
                 systeminfo['os'] = str(' '.join(distro.linux_distribution(full_distribution_name=True)))
         elif sys.platform == "darwin":
             systeminfo['os'] = "Mac OS %s" % platform.mac_ver()[0]
             cpu['brand'] = str(systemCommand('sysctl machdep.cpu.brand_string', False)[0]).split(': ')[1]
@@ -111,15 +137,15 @@
             # https://learn.microsoft.com/en-us/windows/release-health/windows11-release-information
             if sys.getwindowsversion().build >= 22000:
                 systeminfo['os'] = "{} {}".format(platform.uname()[0], 11)
             else:
                 systeminfo['os'] = "{} {}".format(platform.uname()[0], platform.uname()[2])
         systeminfo['cpu'] = cpu['brand']
         systeminfo['cores'] = cpu['count']
-        systeminfo['memory'] = mem.total
+        systeminfo['memory'] = mem
         systeminfo['psutil'] = '.'.join(map(str, psutil.version_info))
         systeminfo['python_version'] = sys.version
         systeminfo['platform'] = platform.platform()
         systeminfo['uptime'] = int(time.time()-psutil.boot_time())
         systeminfo['ip_addresses'] = ip_addresses()
         systeminfo['hostname'] = platform.node()
```

### Comparing `agent360-1.2.47/agent360/plugins/tcpports.py` & `agent360-1.2.48/agent360/plugins/tcpports.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/temp.py` & `agent360-1.2.48/agent360/plugins/temp.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/unbound.py` & `agent360-1.2.48/agent360/plugins/unbound.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/vms.py` & `agent360-1.2.48/agent360/plugins/vms.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/wp-toolkit.py` & `agent360-1.2.48/agent360/plugins/wp-toolkit.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360/plugins/yum-updates.py` & `agent360-1.2.48/agent360/plugins/yum-updates.py`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360-example.ini` & `agent360-1.2.48/agent360-example.ini`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/agent360.egg-info/PKG-INFO` & `agent360-1.2.48/agent360.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent360
-Version: 1.2.47
+Version: 1.2.48
 Summary: 360 agent
 Home-page: https://github.com/plesk/agent360
 Author: 360
 Author-email: 360support@webpros.com
 Maintainer: 360
 Maintainer-email: 360support@webpros.com
 License: BSD-3-Clause
```

### Comparing `agent360-1.2.47/agent360.egg-info/SOURCES.txt` & `agent360-1.2.48/agent360.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agent360-1.2.47/setup.py` & `agent360-1.2.48/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     install_requires = ['psutil==5.6.7', 'netifaces', 'configparser==3.5.0', 'future', 'certifi']
 else:
     install_requires = ['psutil', 'netifaces', 'configparser', 'future', 'certifi']
 
 
 setuptools.setup(
     name='agent360',
-    version='1.2.47',
+    version='1.2.48',
     description='360 agent',
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://github.com/plesk/agent360',
     author='360',
     author_email='360support@webpros.com',
     maintainer='360',
```

