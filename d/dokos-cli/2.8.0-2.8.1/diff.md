# Comparing `tmp/dokos_cli-2.8.0.tar.gz` & `tmp/dokos_cli-2.8.1.tar.gz`

## Comparing `dokos_cli-2.8.0.tar` & `dokos_cli-2.8.1.tar`

### file list

```diff
@@ -1,154 +1,154 @@
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/__init__.py
--rwxr-xr-x   0        0        0    29580 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/app.py
--rw-r--r--   0        0        0    13585 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/bench.py
--rwxr-xr-x   0        0        0     6484 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/cli.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/exceptions.py
--rw-r--r--   0        0        0    18004 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/install.py
--rwxr-xr-x   0        0        0    10051 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/release.py
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/commands/__init__.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/commands/config.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/commands/git.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/commands/install.py
--rwxr-xr-x   0        0        0     7206 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/commands/make.py
--rwxr-xr-x   0        0        0    12749 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/commands/setup.py
--rwxr-xr-x   0        0        0     2798 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/commands/update.py
--rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/commands/utils.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/__init__.py
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/common_site_config.py
--rwxr-xr-x   0        0        0     5457 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/lets_encrypt.py
--rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/nginx.py
--rwxr-xr-x   0        0        0      872 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/procfile.py
--rwxr-xr-x   0        0        0     5702 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/production_setup.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/redis.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/site_config.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/supervisor.py
--rw-r--r--   0        0        0     9909 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/systemd.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/502.html
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/Procfile
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/bench_manager_nginx.conf
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/frappe_sudoers
--rwxr-xr-x   0        0        0      620 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/letsencrypt.cfg
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/nginx.conf
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/nginx_default.conf
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/redis_cache.conf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/redis_queue.conf
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/supervisor.conf
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/systemd/frappe-bench-frappe-default-worker.service
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/systemd/frappe-bench-frappe-long-worker.service
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/systemd/frappe-bench-frappe-schedule.service
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/systemd/frappe-bench-frappe-short-worker.service
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/systemd/frappe-bench-frappe-web.service
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/systemd/frappe-bench-node-socketio.service
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/systemd/frappe-bench-redis-cache.service
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/systemd/frappe-bench-redis-queue.service
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/systemd/frappe-bench-redis.target
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/systemd/frappe-bench-web.target
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/systemd/frappe-bench-workers.target
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/config/templates/systemd/frappe-bench.target
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/patches/__init__.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/patches/patches.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/patches/v2/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/patches/v2/fix_backup_cronjob.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/patches/v2/fix_user_permissions.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/patches/v2/set_live_reload_config.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/patches/v2/update_archived_sites.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/README.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/create_user.yml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/macosx.yml
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/site.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/bash_screen_wall/files/screen_wall.sh
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/bash_screen_wall/tasks/main.yml
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/bench/tasks/change_ssh_port.yml
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/bench/tasks/main.yml
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/bench/tasks/setup_bench_production.yml
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/bench/tasks/setup_dokos.yml
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/bench/tasks/setup_firewall.yml
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/bench/tasks/setup_inputrc.yml
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/common/tasks/debian.yml
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/common/tasks/debian_family.yml
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/common/tasks/macos.yml
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/common/tasks/main.yml
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/common/tasks/redhat_family.yml
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/common/tasks/ubuntu.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/dns_caching/handlers/main.yml
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/dns_caching/tasks/main.yml
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/fail2ban/defaults/main.yml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/fail2ban/handlers/main.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/fail2ban/tasks/configure_nginx_jail.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/fail2ban/tasks/main.yml
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/fail2ban/templates/nginx-proxy-jail.conf.j2
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/frappe_selinux/files/frappe_selinux.te
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/frappe_selinux/tasks/main.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/locale/defaults/main.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/locale/tasks/main.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/logwatch/defaults/main.yml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/logwatch/tasks/main.yml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/logwatch/templates/logwatch.conf.j2
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/README.md
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/defaults/main.yml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/files/debian_mariadb_config.cnf
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/files/mariadb_config.cnf
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/handlers/main.yml
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/tasks/centos.yml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/tasks/debian.yml
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/tasks/main.yml
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/templates/mariadb_centos.repo.j2
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/templates/mariadb_debian.list.j2
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/templates/mariadb_ubuntu.list.j2
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/templates/my.cnf.j2
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/mariadb/vars/main.yml
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/README.md
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/defaults/main.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/handlers/main.yml
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/meta/main.yml
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/tasks/main.yml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/tasks/setup-Debian.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/tasks/setup-RedHat.yml
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/tasks/vhosts.yml
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/templates/nginx.conf.j2
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/templates/nginx.repo.j2
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/templates/vhosts.j2
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/tests/inventory
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/tests/test.yml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/vars/Debian.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nginx/vars/RedHat.yml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nodejs/defaults/main.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nodejs/tasks/debian_family.yml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nodejs/tasks/main.yml
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/nodejs/tasks/redhat_family.yml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/ntpd/tasks/main.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/packer/tasks/debian_family.yml
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/packer/tasks/main.yml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/packer/tasks/redhat_family.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/psutil/tasks/main.yml
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/redis/tasks/main.yml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/supervisor/tasks/main.yml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/swap/defaults/main.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/swap/tasks/main.yml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/virtualbox/defaults/main.yml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/virtualbox/files/virtualbox_centos.repo
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/virtualbox/tasks/debian_family.yml
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/virtualbox/tasks/main.yml
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/virtualbox/tasks/redhat_family.yml
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/playbooks/roles/wkhtmltopdf/tasks/main.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/tests/__init__.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/tests/test_base.py
--rwxr-xr-x   0        0        0     7403 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/tests/test_init.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/tests/test_setup_production.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/tests/test_utils.py
--rw-r--r--   0        0        0    15606 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/utils/__init__.py
--rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/utils/app.py
--rw-r--r--   0        0        0    22038 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/utils/bench.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/utils/cli.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/utils/render.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/utils/system.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/bench/utils/translation.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/.gitignore
--rw-r--r--   0        0        0    35121 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/LICENSE.md
--rwxr-xr-x   0        0        0     2469 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/README.md
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/pyproject.toml
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 dokos_cli-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/__init__.py
+-rwxr-xr-x   0        0        0    29586 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/app.py
+-rw-r--r--   0        0        0    13585 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/bench.py
+-rwxr-xr-x   0        0        0     6484 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/cli.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/exceptions.py
+-rw-r--r--   0        0        0    18004 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/install.py
+-rwxr-xr-x   0        0        0    10051 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/release.py
+-rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/commands/__init__.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/commands/config.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/commands/git.py
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/commands/install.py
+-rwxr-xr-x   0        0        0     7206 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/commands/make.py
+-rwxr-xr-x   0        0        0    12749 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/commands/setup.py
+-rwxr-xr-x   0        0        0     2798 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/commands/update.py
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/commands/utils.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/__init__.py
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/common_site_config.py
+-rwxr-xr-x   0        0        0     5457 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/lets_encrypt.py
+-rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/nginx.py
+-rwxr-xr-x   0        0        0      872 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/procfile.py
+-rwxr-xr-x   0        0        0     5702 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/production_setup.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/redis.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/site_config.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/supervisor.py
+-rw-r--r--   0        0        0     9909 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/systemd.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/502.html
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/Procfile
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/bench_manager_nginx.conf
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/frappe_sudoers
+-rwxr-xr-x   0        0        0      620 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/letsencrypt.cfg
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/nginx.conf
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/nginx_default.conf
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/redis_cache.conf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/redis_queue.conf
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/supervisor.conf
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/systemd/frappe-bench-frappe-default-worker.service
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/systemd/frappe-bench-frappe-long-worker.service
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/systemd/frappe-bench-frappe-schedule.service
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/systemd/frappe-bench-frappe-short-worker.service
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/systemd/frappe-bench-frappe-web.service
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/systemd/frappe-bench-node-socketio.service
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/systemd/frappe-bench-redis-cache.service
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/systemd/frappe-bench-redis-queue.service
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/systemd/frappe-bench-redis.target
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/systemd/frappe-bench-web.target
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/systemd/frappe-bench-workers.target
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/config/templates/systemd/frappe-bench.target
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/patches/__init__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/patches/patches.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/patches/v2/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/patches/v2/fix_backup_cronjob.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/patches/v2/fix_user_permissions.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/patches/v2/set_live_reload_config.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/patches/v2/update_archived_sites.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/README.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/create_user.yml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/macosx.yml
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/site.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/bash_screen_wall/files/screen_wall.sh
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/bash_screen_wall/tasks/main.yml
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/bench/tasks/change_ssh_port.yml
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/bench/tasks/main.yml
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/bench/tasks/setup_bench_production.yml
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/bench/tasks/setup_dokos.yml
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/bench/tasks/setup_firewall.yml
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/bench/tasks/setup_inputrc.yml
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/common/tasks/debian.yml
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/common/tasks/debian_family.yml
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/common/tasks/macos.yml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/common/tasks/main.yml
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/common/tasks/redhat_family.yml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/common/tasks/ubuntu.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/dns_caching/handlers/main.yml
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/dns_caching/tasks/main.yml
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/fail2ban/defaults/main.yml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/fail2ban/handlers/main.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/fail2ban/tasks/configure_nginx_jail.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/fail2ban/tasks/main.yml
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/fail2ban/templates/nginx-proxy-jail.conf.j2
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/frappe_selinux/files/frappe_selinux.te
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/frappe_selinux/tasks/main.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/locale/defaults/main.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/locale/tasks/main.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/logwatch/defaults/main.yml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/logwatch/tasks/main.yml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/logwatch/templates/logwatch.conf.j2
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/README.md
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/defaults/main.yml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/files/debian_mariadb_config.cnf
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/files/mariadb_config.cnf
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/handlers/main.yml
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/tasks/centos.yml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/tasks/debian.yml
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/tasks/main.yml
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/templates/mariadb_centos.repo.j2
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/templates/mariadb_debian.list.j2
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/templates/mariadb_ubuntu.list.j2
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/templates/my.cnf.j2
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/mariadb/vars/main.yml
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/README.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/defaults/main.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/handlers/main.yml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/meta/main.yml
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/tasks/main.yml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/tasks/setup-Debian.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/tasks/setup-RedHat.yml
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/tasks/vhosts.yml
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/templates/nginx.conf.j2
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/templates/nginx.repo.j2
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/templates/vhosts.j2
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/tests/inventory
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/tests/test.yml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/vars/Debian.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nginx/vars/RedHat.yml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nodejs/defaults/main.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nodejs/tasks/debian_family.yml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nodejs/tasks/main.yml
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/nodejs/tasks/redhat_family.yml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/ntpd/tasks/main.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/packer/tasks/debian_family.yml
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/packer/tasks/main.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/packer/tasks/redhat_family.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/psutil/tasks/main.yml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/redis/tasks/main.yml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/supervisor/tasks/main.yml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/swap/defaults/main.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/swap/tasks/main.yml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/virtualbox/defaults/main.yml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/virtualbox/files/virtualbox_centos.repo
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/virtualbox/tasks/debian_family.yml
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/virtualbox/tasks/main.yml
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/virtualbox/tasks/redhat_family.yml
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/playbooks/roles/wkhtmltopdf/tasks/main.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/tests/__init__.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/tests/test_base.py
+-rwxr-xr-x   0        0        0     7403 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/tests/test_init.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/tests/test_setup_production.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/tests/test_utils.py
+-rw-r--r--   0        0        0    15606 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/utils/__init__.py
+-rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/utils/app.py
+-rw-r--r--   0        0        0    22038 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/utils/bench.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/utils/cli.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/utils/render.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/utils/system.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/bench/utils/translation.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/.gitignore
+-rw-r--r--   0        0        0    35121 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/LICENSE.md
+-rwxr-xr-x   0        0        0     2469 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/README.md
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 dokos_cli-2.8.1/PKG-INFO
```

### Comparing `dokos_cli-2.8.0/bench/app.py` & `dokos_cli-2.8.1/bench/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 		# fetch meta from installed apps
 		if self.bench and os.path.exists(os.path.join(self.bench.cwd, "apps", self.name)):
 			self.mount_path = os.path.join(self.bench.cwd, "apps", self.name)
 			self.from_apps = True
 			self._setup_details_from_mounted_disk()
 
 		# fetch meta for repo on mounted disk
-		elif os.path.exists(self.name):
+		elif os.path.exists(self.mount_path):
 			self.on_disk = True
 			self._setup_details_from_mounted_disk()
 
 		# fetch meta for repo from remote git server - traditional get-app url
 		elif is_git_url(self.name):
 			self.is_url = True
 			self.__setup_details_from_git()
```

### Comparing `dokos_cli-2.8.0/bench/bench.py` & `dokos_cli-2.8.1/bench/bench.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/cli.py` & `dokos_cli-2.8.1/bench/cli.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/exceptions.py` & `dokos_cli-2.8.1/bench/exceptions.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/install.py` & `dokos_cli-2.8.1/bench/install.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/release.py` & `dokos_cli-2.8.1/bench/release.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/commands/__init__.py` & `dokos_cli-2.8.1/bench/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/commands/config.py` & `dokos_cli-2.8.1/bench/commands/config.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/commands/git.py` & `dokos_cli-2.8.1/bench/commands/git.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/commands/install.py` & `dokos_cli-2.8.1/bench/commands/install.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/commands/make.py` & `dokos_cli-2.8.1/bench/commands/make.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/commands/setup.py` & `dokos_cli-2.8.1/bench/commands/setup.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/commands/update.py` & `dokos_cli-2.8.1/bench/commands/update.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/commands/utils.py` & `dokos_cli-2.8.1/bench/commands/utils.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/common_site_config.py` & `dokos_cli-2.8.1/bench/config/common_site_config.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/lets_encrypt.py` & `dokos_cli-2.8.1/bench/config/lets_encrypt.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/nginx.py` & `dokos_cli-2.8.1/bench/config/nginx.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/procfile.py` & `dokos_cli-2.8.1/bench/config/procfile.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/production_setup.py` & `dokos_cli-2.8.1/bench/config/production_setup.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/redis.py` & `dokos_cli-2.8.1/bench/config/redis.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/site_config.py` & `dokos_cli-2.8.1/bench/config/site_config.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/supervisor.py` & `dokos_cli-2.8.1/bench/config/supervisor.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/systemd.py` & `dokos_cli-2.8.1/bench/config/systemd.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/templates/502.html` & `dokos_cli-2.8.1/bench/config/templates/502.html`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/templates/Procfile` & `dokos_cli-2.8.1/bench/config/templates/Procfile`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/templates/bench_manager_nginx.conf` & `dokos_cli-2.8.1/bench/config/templates/bench_manager_nginx.conf`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/templates/frappe_sudoers` & `dokos_cli-2.8.1/bench/config/templates/frappe_sudoers`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/templates/letsencrypt.cfg` & `dokos_cli-2.8.1/bench/config/templates/letsencrypt.cfg`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/templates/nginx.conf` & `dokos_cli-2.8.1/bench/config/templates/nginx.conf`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/templates/nginx_default.conf` & `dokos_cli-2.8.1/bench/config/templates/nginx_default.conf`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/templates/supervisor.conf` & `dokos_cli-2.8.1/bench/config/templates/supervisor.conf`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/config/templates/systemd/frappe-bench-frappe-web.service` & `dokos_cli-2.8.1/bench/config/templates/systemd/frappe-bench-frappe-web.service`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/patches/__init__.py` & `dokos_cli-2.8.1/bench/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/patches/v2/fix_user_permissions.py` & `dokos_cli-2.8.1/bench/patches/v2/fix_user_permissions.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/patches/v2/update_archived_sites.py` & `dokos_cli-2.8.1/bench/patches/v2/update_archived_sites.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/create_user.yml` & `dokos_cli-2.8.1/bench/playbooks/create_user.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/macosx.yml` & `dokos_cli-2.8.1/bench/playbooks/macosx.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/site.yml` & `dokos_cli-2.8.1/bench/playbooks/site.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/bench/tasks/main.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/bench/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/bench/tasks/setup_bench_production.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/bench/tasks/setup_bench_production.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/bench/tasks/setup_dokos.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/bench/tasks/setup_dokos.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/bench/tasks/setup_firewall.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/bench/tasks/setup_firewall.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/common/tasks/debian_family.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/common/tasks/debian_family.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/common/tasks/macos.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/common/tasks/macos.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/common/tasks/redhat_family.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/common/tasks/redhat_family.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/fail2ban/tasks/main.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/fail2ban/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2` & `dokos_cli-2.8.1/bench/playbooks/roles/fail2ban/templates/nginx-proxy-filter.conf.j2`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/frappe_selinux/files/frappe_selinux.te` & `dokos_cli-2.8.1/bench/playbooks/roles/frappe_selinux/files/frappe_selinux.te`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/frappe_selinux/tasks/main.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/frappe_selinux/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/locale/tasks/main.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/locale/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/mariadb/README.md` & `dokos_cli-2.8.1/bench/playbooks/roles/mariadb/README.md`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/mariadb/files/mariadb_config.cnf` & `dokos_cli-2.8.1/bench/playbooks/roles/mariadb/files/mariadb_config.cnf`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/mariadb/tasks/debian.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/mariadb/tasks/debian.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/mariadb/tasks/main.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/mariadb/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/mariadb/tasks/mysql_secure_installation.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/mariadb/tasks/ubuntu-trusty.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/mariadb/tasks/ubuntu-xenial_bionic.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/nginx/README.md` & `dokos_cli-2.8.1/bench/playbooks/roles/nginx/README.md`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/nginx/defaults/main.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/nginx/defaults/main.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/nginx/tasks/main.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/nginx/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/nginx/tasks/setup-Debian.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/nginx/tasks/setup-Debian.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/nginx/tasks/vhosts.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/nginx/tasks/vhosts.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/nginx/templates/nginx.conf.j2` & `dokos_cli-2.8.1/bench/playbooks/roles/nginx/templates/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/nginx/templates/vhosts.j2` & `dokos_cli-2.8.1/bench/playbooks/roles/nginx/templates/vhosts.j2`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/ntpd/tasks/main.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/ntpd/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/packer/tasks/main.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/packer/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/redis/tasks/main.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/redis/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/swap/tasks/main.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/swap/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/virtualbox/tasks/debian_family.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/virtualbox/tasks/debian_family.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/playbooks/roles/wkhtmltopdf/tasks/main.yml` & `dokos_cli-2.8.1/bench/playbooks/roles/wkhtmltopdf/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/tests/test_base.py` & `dokos_cli-2.8.1/bench/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/tests/test_init.py` & `dokos_cli-2.8.1/bench/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/tests/test_setup_production.py` & `dokos_cli-2.8.1/bench/tests/test_setup_production.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/tests/test_utils.py` & `dokos_cli-2.8.1/bench/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/utils/__init__.py` & `dokos_cli-2.8.1/bench/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/utils/app.py` & `dokos_cli-2.8.1/bench/utils/app.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/utils/bench.py` & `dokos_cli-2.8.1/bench/utils/bench.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/utils/cli.py` & `dokos_cli-2.8.1/bench/utils/cli.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/utils/render.py` & `dokos_cli-2.8.1/bench/utils/render.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/utils/system.py` & `dokos_cli-2.8.1/bench/utils/system.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/bench/utils/translation.py` & `dokos_cli-2.8.1/bench/utils/translation.py`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/.gitignore` & `dokos_cli-2.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/LICENSE.md` & `dokos_cli-2.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/README.md` & `dokos_cli-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/pyproject.toml` & `dokos_cli-2.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dokos_cli-2.8.0/PKG-INFO` & `dokos_cli-2.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dokos-cli
-Version: 2.8.0
+Version: 2.8.1
 Summary: CLI to manage Multi-tenant deployments for Dodock apps
 Project-URL: Changelog, https://github.com/frappe/bench/releases
 Project-URL: Documentation, https://frappeframework.com/docs/user/en/bench
 Project-URL: Homepage, https://frappe.io/bench
 Project-URL: Source, https://github.com/frappe/bench
 Author-email: Dokos SAS <hello@dokos.io>
 License-Expression: GPL-3.0-only
```

