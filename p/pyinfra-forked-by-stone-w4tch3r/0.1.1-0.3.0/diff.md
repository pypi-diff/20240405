# Comparing `tmp/pyinfra_forked_by_stone-w4tch3r-0.1.1.tar.gz` & `tmp/pyinfra_forked_by_stone-w4tch3r-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinfra_forked_by_stone-w4tch3r-0.1.1.tar", last modified: Sun Nov 19 18:36:32 2023, max compression
+gzip compressed data, was "pyinfra_forked_by_stone-w4tch3r-0.3.0.tar", last modified: Fri Apr  5 14:23:50 2024, max compression
```

## Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1.tar` & `pyinfra_forked_by_stone-w4tch3r-0.3.0.tar`

### file list

```diff
@@ -1,197 +1,190 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.197099 pyinfra_forked_by_stone-w4tch3r-0.1.1/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11377 2023-11-19 18:35:30.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/CHANGELOG.md
--rw-rw-r--   0 user1     (1000) user1     (1000)     1076 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/LICENSE.md
--rw-rw-r--   0 user1     (1000) user1     (1000)       59 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/MANIFEST.in
--rw-r--r--   0 user1     (1000) user1     (1000)     8405 2023-11-19 18:36:32.197099 pyinfra_forked_by_stone-w4tch3r-0.1.1/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     4230 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/README.md
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.137101 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/
--rw-rw-r--   0 user1     (1000) user1     (1000)      535 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)       47 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/__main__.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.141101 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/
--rw-rw-r--   0 user1     (1000) user1     (1000)      888 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    10238 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/arguments.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     6561 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/command.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3824 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/config.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1417 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/connect.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1016 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/connectors.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3909 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/deploy.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1185 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/exceptions.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    11227 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/facts.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    11473 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/host.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     7785 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/inventory.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    12571 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/operation.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    12146 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/operations.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    11272 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/state.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    11690 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/util.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.145101 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5638 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/ansible.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5367 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/chroot.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     8549 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/docker.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     8504 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/dockerssh.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     6381 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/local.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4454 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/mech.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.145101 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/pyinfrawinrmsession/
--rw-rw-r--   0 user1     (1000) user1     (1000)     1113 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/pyinfrawinrmsession/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    21254 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/ssh.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.145101 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/sshuserclient/
--rw-rw-r--   0 user1     (1000) user1     (1000)       44 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/sshuserclient/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     9606 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/sshuserclient/client.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2721 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/sshuserclient/config.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3014 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/terraform.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     9157 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/util.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4376 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/vagrant.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    10047 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/winrm.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3351 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/context.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.153100 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/
--rw-rw-r--   0 user1     (1000) user1     (1000)      347 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      482 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/apk.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1999 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/apt.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2266 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/brew.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      490 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/bsdinit.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      531 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/cargo.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      716 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/choco.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1662 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/deb.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      862 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/dnf.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1657 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/docker.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    11071 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/files.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      473 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/gem.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1236 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/git.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3688 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/gpg.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     9125 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/hardware.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3313 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/iptables.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      668 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/launchd.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      337 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/lxd.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5873 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/mysql.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      674 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/npm.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1350 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/openrc.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1001 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/pacman.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      702 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/pip.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      452 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/pkg.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      481 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/pkgin.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4035 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/postgresql.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1973 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/rpm.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4219 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/selinux.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    16093 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/server.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1910 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/snap.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3290 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/systemd.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1414 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/sysvinit.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      543 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/upstart.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.157100 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/util/
--rw-rw-r--   0 user1     (1000) user1     (1000)      521 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/util/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      730 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/util/databases.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1017 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/util/packaging.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2561 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/util/win_files.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      591 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/vzctl.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     8664 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/windows.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2101 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/windows_files.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      481 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/xbps.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      827 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/yum.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      766 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/zypper.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2827 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/local.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.165100 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/
--rw-rw-r--   0 user1     (1000) user1     (1000)      357 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2033 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/apk.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    14106 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/apt.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4316 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/brew.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1559 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/bsdinit.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1040 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/cargo.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1451 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/choco.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5537 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/dnf.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    59202 2023-11-19 18:33:13.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/files.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1068 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/gem.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    12493 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/git.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     9098 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/iptables.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1162 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/launchd.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1845 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/lxd.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    19968 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/mysql.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1402 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/npm.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1508 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/openrc.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1656 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/pacman.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5515 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/pip.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2220 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/pkg.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1914 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/pkgin.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    10500 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/postgresql.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      797 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/puppet.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2398 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/python.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     6149 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/selinux.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    35225 2023-11-19 18:33:17.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/server.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3077 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/snap.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5933 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/ssh.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3799 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/systemd.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4326 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/sysvinit.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1887 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/upstart.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.169100 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/util/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/util/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3329 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/util/files.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     9004 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/util/packaging.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1990 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/util/service.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2996 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/vzctl.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1660 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/windows.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    16125 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/windows_files.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1430 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/xbps.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5530 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/yum.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5481 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/zypper.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4193 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/progress.py
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/py.typed
--rw-rw-r--   0 user1     (1000) user1     (1000)      153 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/version.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.173100 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/
--rw-rw-r--   0 user1     (1000) user1     (1000)      284 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      859 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/__main__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1669 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/commands.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3704 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/exceptions.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     8733 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/inventory.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1714 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/log.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    18266 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/main.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    10426 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/prints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5374 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/util.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2466 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/virtualenv.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.173100 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_forked_by_stone_w4tch3r.egg-info/
--rw-r--r--   0 user1     (1000) user1     (1000)     8405 2023-11-19 18:36:32.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_forked_by_stone_w4tch3r.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     5060 2023-11-19 18:36:32.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_forked_by_stone_w4tch3r.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-11-19 18:36:32.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_forked_by_stone_w4tch3r.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)      439 2023-11-19 18:36:32.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_forked_by_stone_w4tch3r.egg-info/entry_points.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)     1090 2023-11-19 18:36:32.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_forked_by_stone_w4tch3r.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       26 2023-11-19 18:36:32.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_forked_by_stone_w4tch3r.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)      534 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/pyproject.toml
--rw-rw-r--   0 user1     (1000) user1     (1000)      663 2023-11-19 18:36:32.197099 pyinfra_forked_by_stone-w4tch3r-0.1.1/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)     5045 2023-11-19 18:33:17.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/setup.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.173100 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.177099 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2295 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2043 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_arguments.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3204 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_command.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      708 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_config.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4194 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_deploys.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    11745 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_facts.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1119 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_host.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2013 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_inventory.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    23145 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_operations.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      684 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_util.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.181099 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_cli/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_cli/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     6967 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_cli/test_cli.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5794 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_cli/test_cli_deploy.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1565 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_cli/test_cli_exceptions.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2562 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_cli/test_cli_util.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2130 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_cli/test_context_objects.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      315 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_cli/util.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-11-19 18:36:32.185099 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2009 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_ansible.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5904 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_chroot.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     6563 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_docker.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     9438 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_dockerssh.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     7494 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_local.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4307 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_mech.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    37584 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_ssh.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5681 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_sshuserclient.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3569 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_terraform.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5195 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_util.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3542 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_vagrant.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2466 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_winrm.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3308 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_facts.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1688 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_global_arguments.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     8187 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_operations.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      557 2023-11-19 17:34:04.000000 pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_operations_utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.310376 pyinfra_forked_by_stone-w4tch3r-0.3.0/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1630 2024-04-05 14:22:05.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/CHANGELOG.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1076 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/LICENSE.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)       59 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/MANIFEST.in
+-rw-r--r--   0 user1     (1000) user1     (1000)     8076 2024-04-05 14:23:50.310376 pyinfra_forked_by_stone-w4tch3r-0.3.0/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4526 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/README.md
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.282390 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      535 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)       47 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/__main__.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.286388 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      942 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     9748 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/arguments.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2254 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/arguments_typed.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     7176 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/command.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4221 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/config.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1416 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/connect.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      544 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/connectors.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2756 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/deploy.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1861 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/exceptions.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    10282 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/facts.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    13164 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/host.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     7663 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/inventory.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    14374 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/operation.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    10942 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/operations.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    12622 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/state.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11977 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/util.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.286388 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3756 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/base.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5931 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/chroot.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     8964 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/docker.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     8919 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/dockerssh.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     6929 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/local.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    21018 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/ssh.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3683 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/ssh_util.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.286388 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/sshuserclient/
+-rw-rw-r--   0 user1     (1000) user1     (1000)       44 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/sshuserclient/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     9720 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/sshuserclient/client.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2721 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/sshuserclient/config.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3617 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/terraform.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11321 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/util.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4722 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/vagrant.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3394 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/context.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.290386 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      347 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      482 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/apk.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1999 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/apt.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2266 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/brew.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      490 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/bsdinit.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      531 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/cargo.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      703 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/choco.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1666 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/deb.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      862 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/dnf.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1678 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/docker.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11475 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/files.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      473 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/gem.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1294 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/git.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3729 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/gpg.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11402 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/hardware.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3374 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/iptables.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      668 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/launchd.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      337 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/lxd.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5936 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/mysql.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      674 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/npm.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1350 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/openrc.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1001 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/pacman.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      702 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/pip.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      452 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/pkg.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      481 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/pkgin.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4146 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/postgres.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      187 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/postgresql.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1973 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/rpm.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4272 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/selinux.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    19794 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/server.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1910 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/snap.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3927 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/systemd.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1490 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/sysvinit.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      543 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/upstart.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.290386 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/util/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      521 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/util/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      730 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/util/databases.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1161 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/util/packaging.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2561 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/util/win_files.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      591 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/vzctl.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      481 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/xbps.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      827 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/yum.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      766 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/zypper.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2751 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/local.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.298382 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      357 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2068 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/apk.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    13621 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/apt.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5086 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/brew.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1598 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/bsdinit.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1061 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/cargo.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1472 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/choco.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5546 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/dnf.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    53012 2024-04-05 14:20:30.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/files.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1089 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/gem.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11669 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/git.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     9180 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/iptables.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1134 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/launchd.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1727 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/lxd.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    19530 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/mysql.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1430 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/npm.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1530 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/openrc.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1691 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/pacman.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5771 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/pip.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2248 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/pkg.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1949 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/pkgin.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     9401 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/postgres.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      797 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/postgresql.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      811 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/puppet.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1959 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/python.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5768 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/selinux.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    36016 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/server.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3006 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/snap.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5563 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/ssh.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3866 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/systemd.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4028 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/sysvinit.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1928 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/upstart.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.298382 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/util/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      366 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/util/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3521 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/util/files.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     8637 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/util/packaging.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1146 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/util/service.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3067 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/vzctl.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1465 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/xbps.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5548 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/yum.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5477 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/zypper.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4193 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/progress.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/py.typed
+-rw-rw-r--   0 user1     (1000) user1     (1000)      153 2024-03-10 12:59:09.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/version.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.298382 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      284 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      881 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/__main__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1832 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/commands.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4806 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/exceptions.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     9513 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/inventory.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2201 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/log.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    19715 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/main.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11859 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/prints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     6322 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/util.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2466 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/virtualenv.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.306378 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_forked_by_stone_w4tch3r.egg-info/
+-rw-r--r--   0 user1     (1000) user1     (1000)     8076 2024-04-05 14:23:50.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_forked_by_stone_w4tch3r.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4839 2024-04-05 14:23:50.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_forked_by_stone_w4tch3r.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2024-04-05 14:23:50.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_forked_by_stone_w4tch3r.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)      471 2024-04-05 14:23:50.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_forked_by_stone_w4tch3r.egg-info/entry_points.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)      884 2024-04-05 14:23:50.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_forked_by_stone_w4tch3r.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       26 2024-04-05 14:23:50.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_forked_by_stone_w4tch3r.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)      381 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/pyproject.toml
+-rw-rw-r--   0 user1     (1000) user1     (1000)      663 2024-04-05 14:23:50.310376 pyinfra_forked_by_stone-w4tch3r-0.3.0/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4714 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.302380 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.302380 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2413 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1961 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_arguments.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3204 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_command.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      708 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_config.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4200 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_deploys.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    10687 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_facts.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1119 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_host.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2013 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_inventory.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    20162 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_operations.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1716 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_util.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.302380 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_cli/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_cli/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     6045 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_cli/test_cli.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4858 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_cli/test_cli_deploy.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3088 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_cli/test_cli_exceptions.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2562 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_cli/test_cli_util.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2130 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_cli/test_context_objects.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      338 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_cli/util.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-05 14:23:50.306378 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/
+-rw-rw-r--   0 user1     (1000) user1     (1000)        0 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5907 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_chroot.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     6566 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_docker.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     9303 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_dockerssh.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     7442 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_local.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    38399 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_ssh.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5734 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_sshuserclient.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3743 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_terraform.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4647 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_util.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3646 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_vagrant.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3308 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_facts.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     1696 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_global_arguments.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     6074 2024-04-05 14:20:10.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_operations.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      557 2024-03-14 07:58:06.000000 pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_operations_utils.py
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/LICENSE.md` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/PKG-INFO` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 696e  : 2.1.Name: pyin
 00000020: 6672 615f 666f 726b 6564 5f62 795f 7374  fra_forked_by_st
 00000030: 6f6e 652d 7734 7463 6833 720a 5665 7273  one-w4tch3r.Vers
-00000040: 696f 6e3a 2030 2e31 2e31 0a53 756d 6d61  ion: 0.1.1.Summa
+00000040: 696f 6e3a 2030 2e33 2e30 0a53 756d 6d61  ion: 0.3.0.Summa
 00000050: 7279 3a20 4375 7374 6f6d 2076 6572 7369  ry: Custom versi
 00000060: 6f6e 2066 6f72 2064 6576 656c 6f70 696e  on for developin
 00000070: 6720 7079 696e 6672 610a 486f 6d65 2d70  g pyinfra.Home-p
 00000080: 6167 653a 2068 7474 7073 3a2f 2f70 7969  age: https://pyi
 00000090: 6e66 7261 2e63 6f6d 0a41 7574 686f 723a  nfra.com.Author:
 000000a0: 2073 746f 6e65 2d77 3474 6368 3372 0a41   stone-w4tch3r.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2031 3030  uthor-email: 100
@@ -44,483 +44,462 @@
 000002b0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
 000002c0: 6e64 6570 656e 6465 6e74 0a43 6c61 7373  ndependent.Class
 000002d0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
 000002e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 000002f0: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
 00000300: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
 00000310: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000320: 7974 686f 6e20 3a3a 2033 2e36 0a43 6c61  ython :: 3.6.Cla
+00000320: 7974 686f 6e20 3a3a 2033 2e37 0a43 6c61  ython :: 3.7.Cla
 00000330: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
 00000340: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000350: 2050 7974 686f 6e20 3a3a 2033 2e37 0a43   Python :: 3.7.C
+00000350: 2050 7974 686f 6e20 3a3a 2033 2e38 0a43   Python :: 3.8.C
 00000360: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
 00000370: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000380: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+00000380: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
 00000390: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
 000003a0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 000003b0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000003c0: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
-000003d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000003e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000003f0: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
-00000400: 3a20 546f 7069 6320 3a3a 2053 7973 7465  : Topic :: Syste
-00000410: 6d20 3a3a 2053 7973 7465 6d73 2041 646d  m :: Systems Adm
-00000420: 696e 6973 7472 6174 696f 6e0a 436c 6173  inistration.Clas
+000003c0: 2e31 300a 436c 6173 7369 6669 6572 3a20  .10.Classifier: 
+000003d0: 546f 7069 6320 3a3a 2053 7973 7465 6d20  Topic :: System 
+000003e0: 3a3a 2053 7973 7465 6d73 2041 646d 696e  :: Systems Admin
+000003f0: 6973 7472 6174 696f 6e0a 436c 6173 7369  istration.Classi
+00000400: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
+00000410: 7973 7465 6d20 3a3a 2049 6e73 7461 6c6c  ystem :: Install
+00000420: 6174 696f 6e2f 5365 7475 700a 436c 6173  ation/Setup.Clas
 00000430: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
-00000440: 2053 7973 7465 6d20 3a3a 2049 6e73 7461   System :: Insta
-00000450: 6c6c 6174 696f 6e2f 5365 7475 700a 436c  llation/Setup.Cl
-00000460: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00000470: 3a3a 2055 7469 6c69 7469 6573 0a44 6573  :: Utilities.Des
-00000480: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-00000490: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-000004a0: 646f 776e 0a4c 6963 656e 7365 2d46 696c  down.License-Fil
-000004b0: 653a 204c 4943 454e 5345 2e6d 640a 5265  e: LICENSE.md.Re
-000004c0: 7175 6972 6573 2d44 6973 743a 2067 6576  quires-Dist: gev
-000004d0: 656e 743e 3d31 2e35 0a52 6571 7569 7265  ent>=1.5.Require
-000004e0: 732d 4469 7374 3a20 7061 7261 6d69 6b6f  s-Dist: paramiko
-000004f0: 3c34 2c3e 3d32 2e37 0a52 6571 7569 7265  <4,>=2.7.Require
-00000500: 732d 4469 7374 3a20 636c 6963 6b3e 320a  s-Dist: click>2.
-00000510: 5265 7175 6972 6573 2d44 6973 743a 206a  Requires-Dist: j
-00000520: 696e 6a61 323c 342c 3e32 0a52 6571 7569  inja2<4,>2.Requi
-00000530: 7265 732d 4469 7374 3a20 7079 7468 6f6e  res-Dist: python
-00000540: 2d64 6174 6575 7469 6c3c 332c 3e32 0a52  -dateutil<3,>2.R
-00000550: 6571 7569 7265 732d 4469 7374 3a20 7365  equires-Dist: se
-00000560: 7475 7074 6f6f 6c73 0a52 6571 7569 7265  tuptools.Require
-00000570: 732d 4469 7374 3a20 636f 6e66 6967 7061  s-Dist: configpa
-00000580: 7273 6572 0a52 6571 7569 7265 732d 4469  rser.Requires-Di
-00000590: 7374 3a20 7079 7769 6e72 6d0a 5265 7175  st: pywinrm.Requ
-000005a0: 6972 6573 2d44 6973 743a 2064 6973 7472  ires-Dist: distr
-000005b0: 6f3c 322c 3e3d 312e 360a 5265 7175 6972  o<2,>=1.6.Requir
-000005c0: 6573 2d44 6973 743a 2067 7261 7068 6c69  es-Dist: graphli
-000005d0: 625f 6261 636b 706f 7274 3b20 7079 7468  b_backport; pyth
-000005e0: 6f6e 5f76 6572 7369 6f6e 203c 2022 332e  on_version < "3.
-000005f0: 3922 0a50 726f 7669 6465 732d 4578 7472  9".Provides-Extr
-00000600: 613a 2074 6573 740a 5265 7175 6972 6573  a: test.Requires
-00000610: 2d44 6973 743a 2070 7979 616d 6c3b 2065  -Dist: pyyaml; e
-00000620: 7874 7261 203d 3d20 2274 6573 7422 0a52  xtra == "test".R
-00000630: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
-00000640: 7465 7374 3d3d 372e 302e 313b 2070 7974  test==7.0.1; pyt
-00000650: 686f 6e5f 7665 7273 696f 6e20 3c3d 2022  hon_version <= "
-00000660: 332e 3622 2061 6e64 2065 7874 7261 203d  3.6" and extra =
-00000670: 3d20 2274 6573 7422 0a52 6571 7569 7265  = "test".Require
-00000680: 732d 4469 7374 3a20 636f 7665 7261 6765  s-Dist: coverage
-00000690: 3d3d 362e 323b 2070 7974 686f 6e5f 7665  ==6.2; python_ve
-000006a0: 7273 696f 6e20 3c3d 2022 332e 3622 2061  rsion <= "3.6" a
-000006b0: 6e64 2065 7874 7261 203d 3d20 2274 6573  nd extra == "tes
-000006c0: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
-000006d0: 3a20 7079 7465 7374 3d3d 372e 322e 303b  : pytest==7.2.0;
-000006e0: 2070 7974 686f 6e5f 7665 7273 696f 6e20   python_version 
-000006f0: 3e20 2233 2e36 2220 616e 6420 6578 7472  > "3.6" and extr
-00000700: 6120 3d3d 2022 7465 7374 220a 5265 7175  a == "test".Requ
-00000710: 6972 6573 2d44 6973 743a 2063 6f76 6572  ires-Dist: cover
-00000720: 6167 653d 3d36 2e35 3b20 7079 7468 6f6e  age==6.5; python
-00000730: 5f76 6572 7369 6f6e 203e 2022 332e 3622  _version > "3.6"
-00000740: 2061 6e64 2065 7874 7261 203d 3d20 2274   and extra == "t
-00000750: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
-00000760: 7374 3a20 7079 7465 7374 2d63 6f76 3d3d  st: pytest-cov==
-00000770: 342e 302e 303b 2065 7874 7261 203d 3d20  4.0.0; extra == 
-00000780: 2274 6573 7422 0a52 6571 7569 7265 732d  "test".Requires-
-00000790: 4469 7374 3a20 626c 6163 6b3d 3d32 322e  Dist: black==22.
-000007a0: 332e 303b 2065 7874 7261 203d 3d20 2274  3.0; extra == "t
-000007b0: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
-000007c0: 7374 3a20 6973 6f72 743d 3d35 2e31 302e  st: isort==5.10.
-000007d0: 313b 2065 7874 7261 203d 3d20 2274 6573  1; extra == "tes
-000007e0: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
-000007f0: 3a20 666c 616b 6538 3d3d 342e 302e 313b  : flake8==4.0.1;
-00000800: 2065 7874 7261 203d 3d20 2274 6573 7422   extra == "test"
-00000810: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000820: 666c 616b 6538 2d62 6c61 636b 3d3d 302e  flake8-black==0.
-00000830: 332e 303b 2065 7874 7261 203d 3d20 2274  3.0; extra == "t
-00000840: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
-00000850: 7374 3a20 666c 616b 6538 2d69 736f 7274  st: flake8-isort
-00000860: 3d3d 342e 312e 313b 2065 7874 7261 203d  ==4.1.1; extra =
-00000870: 3d20 2274 6573 7422 0a52 6571 7569 7265  = "test".Require
-00000880: 732d 4469 7374 3a20 6d79 7079 3d3d 302e  s-Dist: mypy==0.
-00000890: 3937 313b 2065 7874 7261 203d 3d20 2274  971; extra == "t
-000008a0: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
-000008b0: 7374 3a20 7479 7065 732d 6372 7970 746f  st: types-crypto
-000008c0: 6772 6170 6879 3b20 6578 7472 6120 3d3d  graphy; extra ==
-000008d0: 2022 7465 7374 220a 5265 7175 6972 6573   "test".Requires
-000008e0: 2d44 6973 743a 2074 7970 6573 2d70 6172  -Dist: types-par
-000008f0: 616d 696b 6f3b 2065 7874 7261 203d 3d20  amiko; extra == 
-00000900: 2274 6573 7422 0a52 6571 7569 7265 732d  "test".Requires-
-00000910: 4469 7374 3a20 7479 7065 732d 7079 7468  Dist: types-pyth
-00000920: 6f6e 2d64 6174 6575 7469 6c3b 2065 7874  on-dateutil; ext
-00000930: 7261 203d 3d20 2274 6573 7422 0a52 6571  ra == "test".Req
-00000940: 7569 7265 732d 4469 7374 3a20 7479 7065  uires-Dist: type
-00000950: 732d 5079 5941 4d4c 3b20 6578 7472 6120  s-PyYAML; extra 
-00000960: 3d3d 2022 7465 7374 220a 5265 7175 6972  == "test".Requir
-00000970: 6573 2d44 6973 743a 2074 7970 6573 2d73  es-Dist: types-s
-00000980: 6574 7570 746f 6f6c 733b 2065 7874 7261  etuptools; extra
-00000990: 203d 3d20 2274 6573 7422 0a50 726f 7669   == "test".Provi
-000009a0: 6465 732d 4578 7472 613a 2064 6f63 730a  des-Extra: docs.
-000009b0: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-000009c0: 7969 6e66 7261 2d67 757a 7a6c 655f 7370  yinfra-guzzle_sp
-000009d0: 6869 6e78 5f74 6865 6d65 3d3d 302e 3134  hinx_theme==0.14
-000009e0: 3b20 6578 7472 6120 3d3d 2022 646f 6373  ; extra == "docs
-000009f0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000a00: 2072 6563 6f6d 6d6f 6e6d 6172 6b3d 3d30   recommonmark==0
-00000a10: 2e35 2e30 3b20 6578 7472 6120 3d3d 2022  .5.0; extra == "
-00000a20: 646f 6373 220a 5265 7175 6972 6573 2d44  docs".Requires-D
-00000a30: 6973 743a 2073 7068 696e 783d 3d32 2e32  ist: sphinx==2.2
-00000a40: 2e31 3b20 6578 7472 6120 3d3d 2022 646f  .1; extra == "do
-00000a50: 6373 220a 5265 7175 6972 6573 2d44 6973  cs".Requires-Dis
-00000a60: 743a 2064 6f63 7574 696c 733d 3d30 2e31  t: docutils==0.1
-00000a70: 372e 313b 2065 7874 7261 203d 3d20 2264  7.1; extra == "d
-00000a80: 6f63 7322 0a50 726f 7669 6465 732d 4578  ocs".Provides-Ex
-00000a90: 7472 613a 2064 6576 0a52 6571 7569 7265  tra: dev.Require
-00000aa0: 732d 4469 7374 3a20 7079 7961 6d6c 3b20  s-Dist: pyyaml; 
-00000ab0: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
-00000ac0: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
-00000ad0: 7465 7374 3d3d 372e 302e 313b 2070 7974  test==7.0.1; pyt
-00000ae0: 686f 6e5f 7665 7273 696f 6e20 3c3d 2022  hon_version <= "
-00000af0: 332e 3622 2061 6e64 2065 7874 7261 203d  3.6" and extra =
+00000440: 2055 7469 6c69 7469 6573 0a44 6573 6372   Utilities.Descr
+00000450: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
+00000460: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
+00000470: 776e 0a4c 6963 656e 7365 2d46 696c 653a  wn.License-File:
+00000480: 204c 4943 454e 5345 2e6d 640a 5265 7175   LICENSE.md.Requ
+00000490: 6972 6573 2d44 6973 743a 2067 6576 656e  ires-Dist: geven
+000004a0: 743e 3d31 2e35 0a52 6571 7569 7265 732d  t>=1.5.Requires-
+000004b0: 4469 7374 3a20 7061 7261 6d69 6b6f 3c34  Dist: paramiko<4
+000004c0: 2c3e 3d32 2e37 0a52 6571 7569 7265 732d  ,>=2.7.Requires-
+000004d0: 4469 7374 3a20 636c 6963 6b3e 320a 5265  Dist: click>2.Re
+000004e0: 7175 6972 6573 2d44 6973 743a 206a 696e  quires-Dist: jin
+000004f0: 6a61 323c 342c 3e32 0a52 6571 7569 7265  ja2<4,>2.Require
+00000500: 732d 4469 7374 3a20 7079 7468 6f6e 2d64  s-Dist: python-d
+00000510: 6174 6575 7469 6c3c 332c 3e32 0a52 6571  ateutil<3,>2.Req
+00000520: 7569 7265 732d 4469 7374 3a20 7365 7475  uires-Dist: setu
+00000530: 7074 6f6f 6c73 0a52 6571 7569 7265 732d  ptools.Requires-
+00000540: 4469 7374 3a20 636f 6e66 6967 7061 7273  Dist: configpars
+00000550: 6572 0a52 6571 7569 7265 732d 4469 7374  er.Requires-Dist
+00000560: 3a20 7079 7769 6e72 6d0a 5265 7175 6972  : pywinrm.Requir
+00000570: 6573 2d44 6973 743a 2074 7970 6567 7561  es-Dist: typegua
+00000580: 7264 0a52 6571 7569 7265 732d 4469 7374  rd.Requires-Dist
+00000590: 3a20 6469 7374 726f 3c32 2c3e 3d31 2e36  : distro<2,>=1.6
+000005a0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000005b0: 6772 6170 686c 6962 5f62 6163 6b70 6f72  graphlib_backpor
+000005c0: 743b 2070 7974 686f 6e5f 7665 7273 696f  t; python_versio
+000005d0: 6e20 3c20 2233 2e39 220a 5265 7175 6972  n < "3.9".Requir
+000005e0: 6573 2d44 6973 743a 2074 7970 696e 672d  es-Dist: typing-
+000005f0: 6578 7465 6e73 696f 6e73 3b20 7079 7468  extensions; pyth
+00000600: 6f6e 5f76 6572 7369 6f6e 203c 2022 332e  on_version < "3.
+00000610: 3131 220a 5072 6f76 6964 6573 2d45 7874  11".Provides-Ext
+00000620: 7261 3a20 7465 7374 0a52 6571 7569 7265  ra: test.Require
+00000630: 732d 4469 7374 3a20 7079 7465 7374 3d3d  s-Dist: pytest==
+00000640: 372e 322e 303b 2065 7874 7261 203d 3d20  7.2.0; extra == 
+00000650: 2274 6573 7422 0a52 6571 7569 7265 732d  "test".Requires-
+00000660: 4469 7374 3a20 636f 7665 7261 6765 3d3d  Dist: coverage==
+00000670: 362e 353b 2065 7874 7261 203d 3d20 2274  6.5; extra == "t
+00000680: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
+00000690: 7374 3a20 7079 7465 7374 2d63 6f76 3d3d  st: pytest-cov==
+000006a0: 342e 302e 303b 2065 7874 7261 203d 3d20  4.0.0; extra == 
+000006b0: 2274 6573 7422 0a52 6571 7569 7265 732d  "test".Requires-
+000006c0: 4469 7374 3a20 626c 6163 6b3d 3d32 322e  Dist: black==22.
+000006d0: 332e 303b 2065 7874 7261 203d 3d20 2274  3.0; extra == "t
+000006e0: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
+000006f0: 7374 3a20 6973 6f72 743d 3d35 2e31 302e  st: isort==5.10.
+00000700: 313b 2065 7874 7261 203d 3d20 2274 6573  1; extra == "tes
+00000710: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
+00000720: 3a20 666c 616b 6538 3d3d 342e 302e 313b  : flake8==4.0.1;
+00000730: 2065 7874 7261 203d 3d20 2274 6573 7422   extra == "test"
+00000740: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000750: 666c 616b 6538 2d62 6c61 636b 3d3d 302e  flake8-black==0.
+00000760: 332e 303b 2065 7874 7261 203d 3d20 2274  3.0; extra == "t
+00000770: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
+00000780: 7374 3a20 666c 616b 6538 2d69 736f 7274  st: flake8-isort
+00000790: 3d3d 342e 312e 313b 2065 7874 7261 203d  ==4.1.1; extra =
+000007a0: 3d20 2274 6573 7422 0a52 6571 7569 7265  = "test".Require
+000007b0: 732d 4469 7374 3a20 6d79 7079 3b20 6578  s-Dist: mypy; ex
+000007c0: 7472 6120 3d3d 2022 7465 7374 220a 5265  tra == "test".Re
+000007d0: 7175 6972 6573 2d44 6973 743a 2074 7970  quires-Dist: typ
+000007e0: 6573 2d63 7279 7074 6f67 7261 7068 793b  es-cryptography;
+000007f0: 2065 7874 7261 203d 3d20 2274 6573 7422   extra == "test"
+00000800: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000810: 7479 7065 732d 7061 7261 6d69 6b6f 3b20  types-paramiko; 
+00000820: 6578 7472 6120 3d3d 2022 7465 7374 220a  extra == "test".
+00000830: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
+00000840: 7970 6573 2d70 7974 686f 6e2d 6461 7465  ypes-python-date
+00000850: 7574 696c 3b20 6578 7472 6120 3d3d 2022  util; extra == "
+00000860: 7465 7374 220a 5265 7175 6972 6573 2d44  test".Requires-D
+00000870: 6973 743a 2074 7970 6573 2d50 7959 414d  ist: types-PyYAM
+00000880: 4c3b 2065 7874 7261 203d 3d20 2274 6573  L; extra == "tes
+00000890: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
+000008a0: 3a20 7479 7065 732d 7365 7475 7074 6f6f  : types-setuptoo
+000008b0: 6c73 3b20 6578 7472 6120 3d3d 2022 7465  ls; extra == "te
+000008c0: 7374 220a 5072 6f76 6964 6573 2d45 7874  st".Provides-Ext
+000008d0: 7261 3a20 646f 6373 0a52 6571 7569 7265  ra: docs.Require
+000008e0: 732d 4469 7374 3a20 7079 696e 6672 612d  s-Dist: pyinfra-
+000008f0: 6775 7a7a 6c65 5f73 7068 696e 785f 7468  guzzle_sphinx_th
+00000900: 656d 653d 3d30 2e31 353b 2065 7874 7261  eme==0.15; extra
+00000910: 203d 3d20 2264 6f63 7322 0a52 6571 7569   == "docs".Requi
+00000920: 7265 732d 4469 7374 3a20 6d79 7374 2d70  res-Dist: myst-p
+00000930: 6172 7365 723d 3d32 2e30 2e30 3b20 6578  arser==2.0.0; ex
+00000940: 7472 6120 3d3d 2022 646f 6373 220a 5265  tra == "docs".Re
+00000950: 7175 6972 6573 2d44 6973 743a 2073 7068  quires-Dist: sph
+00000960: 696e 783d 3d36 2e32 2e31 3b20 6578 7472  inx==6.2.1; extr
+00000970: 6120 3d3d 2022 646f 6373 220a 5072 6f76  a == "docs".Prov
+00000980: 6964 6573 2d45 7874 7261 3a20 6465 760a  ides-Extra: dev.
+00000990: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+000009a0: 7974 6573 743d 3d37 2e32 2e30 3b20 6578  ytest==7.2.0; ex
+000009b0: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+000009c0: 7569 7265 732d 4469 7374 3a20 636f 7665  uires-Dist: cove
+000009d0: 7261 6765 3d3d 362e 353b 2065 7874 7261  rage==6.5; extra
+000009e0: 203d 3d20 2264 6576 220a 5265 7175 6972   == "dev".Requir
+000009f0: 6573 2d44 6973 743a 2070 7974 6573 742d  es-Dist: pytest-
+00000a00: 636f 763d 3d34 2e30 2e30 3b20 6578 7472  cov==4.0.0; extr
+00000a10: 6120 3d3d 2022 6465 7622 0a52 6571 7569  a == "dev".Requi
+00000a20: 7265 732d 4469 7374 3a20 626c 6163 6b3d  res-Dist: black=
+00000a30: 3d32 322e 332e 303b 2065 7874 7261 203d  =22.3.0; extra =
+00000a40: 3d20 2264 6576 220a 5265 7175 6972 6573  = "dev".Requires
+00000a50: 2d44 6973 743a 2069 736f 7274 3d3d 352e  -Dist: isort==5.
+00000a60: 3130 2e31 3b20 6578 7472 6120 3d3d 2022  10.1; extra == "
+00000a70: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
+00000a80: 7374 3a20 666c 616b 6538 3d3d 342e 302e  st: flake8==4.0.
+00000a90: 313b 2065 7874 7261 203d 3d20 2264 6576  1; extra == "dev
+00000aa0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000ab0: 2066 6c61 6b65 382d 626c 6163 6b3d 3d30   flake8-black==0
+00000ac0: 2e33 2e30 3b20 6578 7472 6120 3d3d 2022  .3.0; extra == "
+00000ad0: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
+00000ae0: 7374 3a20 666c 616b 6538 2d69 736f 7274  st: flake8-isort
+00000af0: 3d3d 342e 312e 313b 2065 7874 7261 203d  ==4.1.1; extra =
 00000b00: 3d20 2264 6576 220a 5265 7175 6972 6573  = "dev".Requires
-00000b10: 2d44 6973 743a 2063 6f76 6572 6167 653d  -Dist: coverage=
-00000b20: 3d36 2e32 3b20 7079 7468 6f6e 5f76 6572  =6.2; python_ver
-00000b30: 7369 6f6e 203c 3d20 2233 2e36 2220 616e  sion <= "3.6" an
-00000b40: 6420 6578 7472 6120 3d3d 2022 6465 7622  d extra == "dev"
-00000b50: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000b60: 7079 7465 7374 3d3d 372e 322e 303b 2070  pytest==7.2.0; p
-00000b70: 7974 686f 6e5f 7665 7273 696f 6e20 3e20  ython_version > 
-00000b80: 2233 2e36 2220 616e 6420 6578 7472 6120  "3.6" and extra 
-00000b90: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
-00000ba0: 732d 4469 7374 3a20 636f 7665 7261 6765  s-Dist: coverage
-00000bb0: 3d3d 362e 353b 2070 7974 686f 6e5f 7665  ==6.5; python_ve
-00000bc0: 7273 696f 6e20 3e20 2233 2e36 2220 616e  rsion > "3.6" an
-00000bd0: 6420 6578 7472 6120 3d3d 2022 6465 7622  d extra == "dev"
-00000be0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000bf0: 7079 7465 7374 2d63 6f76 3d3d 342e 302e  pytest-cov==4.0.
-00000c00: 303b 2065 7874 7261 203d 3d20 2264 6576  0; extra == "dev
-00000c10: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000c20: 2062 6c61 636b 3d3d 3232 2e33 2e30 3b20   black==22.3.0; 
-00000c30: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
-00000c40: 6571 7569 7265 732d 4469 7374 3a20 6973  equires-Dist: is
-00000c50: 6f72 743d 3d35 2e31 302e 313b 2065 7874  ort==5.10.1; ext
-00000c60: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
-00000c70: 6972 6573 2d44 6973 743a 2066 6c61 6b65  ires-Dist: flake
-00000c80: 383d 3d34 2e30 2e31 3b20 6578 7472 6120  8==4.0.1; extra 
-00000c90: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
-00000ca0: 732d 4469 7374 3a20 666c 616b 6538 2d62  s-Dist: flake8-b
-00000cb0: 6c61 636b 3d3d 302e 332e 303b 2065 7874  lack==0.3.0; ext
-00000cc0: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
-00000cd0: 6972 6573 2d44 6973 743a 2066 6c61 6b65  ires-Dist: flake
-00000ce0: 382d 6973 6f72 743d 3d34 2e31 2e31 3b20  8-isort==4.1.1; 
-00000cf0: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
-00000d00: 6571 7569 7265 732d 4469 7374 3a20 6d79  equires-Dist: my
-00000d10: 7079 3d3d 302e 3937 313b 2065 7874 7261  py==0.971; extra
-00000d20: 203d 3d20 2264 6576 220a 5265 7175 6972   == "dev".Requir
-00000d30: 6573 2d44 6973 743a 2074 7970 6573 2d63  es-Dist: types-c
-00000d40: 7279 7074 6f67 7261 7068 793b 2065 7874  ryptography; ext
-00000d50: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
-00000d60: 6972 6573 2d44 6973 743a 2074 7970 6573  ires-Dist: types
-00000d70: 2d70 6172 616d 696b 6f3b 2065 7874 7261  -paramiko; extra
-00000d80: 203d 3d20 2264 6576 220a 5265 7175 6972   == "dev".Requir
-00000d90: 6573 2d44 6973 743a 2074 7970 6573 2d70  es-Dist: types-p
-00000da0: 7974 686f 6e2d 6461 7465 7574 696c 3b20  ython-dateutil; 
-00000db0: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
-00000dc0: 6571 7569 7265 732d 4469 7374 3a20 7479  equires-Dist: ty
-00000dd0: 7065 732d 5079 5941 4d4c 3b20 6578 7472  pes-PyYAML; extr
-00000de0: 6120 3d3d 2022 6465 7622 0a52 6571 7569  a == "dev".Requi
-00000df0: 7265 732d 4469 7374 3a20 7479 7065 732d  res-Dist: types-
-00000e00: 7365 7475 7074 6f6f 6c73 3b20 6578 7472  setuptools; extr
-00000e10: 6120 3d3d 2022 6465 7622 0a52 6571 7569  a == "dev".Requi
-00000e20: 7265 732d 4469 7374 3a20 7079 696e 6672  res-Dist: pyinfr
-00000e30: 612d 6775 7a7a 6c65 5f73 7068 696e 785f  a-guzzle_sphinx_
-00000e40: 7468 656d 653d 3d30 2e31 343b 2065 7874  theme==0.14; ext
-00000e50: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
-00000e60: 6972 6573 2d44 6973 743a 2072 6563 6f6d  ires-Dist: recom
-00000e70: 6d6f 6e6d 6172 6b3d 3d30 2e35 2e30 3b20  monmark==0.5.0; 
-00000e80: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
-00000e90: 6571 7569 7265 732d 4469 7374 3a20 7370  equires-Dist: sp
-00000ea0: 6869 6e78 3d3d 322e 322e 313b 2065 7874  hinx==2.2.1; ext
-00000eb0: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
-00000ec0: 6972 6573 2d44 6973 743a 2064 6f63 7574  ires-Dist: docut
-00000ed0: 696c 733d 3d30 2e31 372e 313b 2065 7874  ils==0.17.1; ext
-00000ee0: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
-00000ef0: 6972 6573 2d44 6973 743a 2077 6865 656c  ires-Dist: wheel
-00000f00: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
-00000f10: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000f20: 7477 696e 653b 2065 7874 7261 203d 3d20  twine; extra == 
-00000f30: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
-00000f40: 6973 743a 2069 7079 7468 6f6e 3b20 6578  ist: ipython; ex
-00000f50: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
-00000f60: 7569 7265 732d 4469 7374 3a20 6970 6462  uires-Dist: ipdb
-00000f70: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
-00000f80: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000f90: 6970 6462 706c 7567 696e 3b20 6578 7472  ipdbplugin; extr
-00000fa0: 6120 3d3d 2022 6465 7622 0a52 6571 7569  a == "dev".Requi
-00000fb0: 7265 732d 4469 7374 3a20 666c 616b 6538  res-Dist: flake8
-00000fc0: 2d73 7065 6c6c 6368 6563 6b3d 3d30 2e31  -spellcheck==0.1
-00000fd0: 322e 313b 2065 7874 7261 203d 3d20 2264  2.1; extra == "d
-00000fe0: 6576 220a 5265 7175 6972 6573 2d44 6973  ev".Requires-Dis
-00000ff0: 743a 2072 6564 6261 726f 6e3b 2065 7874  t: redbaron; ext
-00001000: 7261 203d 3d20 2264 6576 220a 5072 6f76  ra == "dev".Prov
-00001010: 6964 6573 2d45 7874 7261 3a20 616e 7369  ides-Extra: ansi
-00001020: 626c 650a 5265 7175 6972 6573 2d44 6973  ble.Requires-Dis
-00001030: 743a 2070 7979 616d 6c3b 2065 7874 7261  t: pyyaml; extra
-00001040: 203d 3d20 2261 6e73 6962 6c65 220a 0a3c   == "ansible"..<
-00001050: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00001060: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
-00001070: 7474 7073 3a2f 2f70 7969 6e66 7261 2e63  ttps://pyinfra.c
-00001080: 6f6d 223e 0a20 2020 2020 2020 203c 696d  om">.        <im
-00001090: 6720 7372 633d 2268 7474 7073 3a2f 2f70  g src="https://p
-000010a0: 7969 6e66 7261 2e63 6f6d 2f73 7461 7469  yinfra.com/stati
-000010b0: 632f 6c6f 676f 5f72 6561 646d 652e 706e  c/logo_readme.pn
-000010c0: 6722 2061 6c74 3d22 7079 696e 6672 6122  g" alt="pyinfra"
-000010d0: 202f 3e0a 2020 2020 3c2f 613e 0a3c 2f70   />.    </a>.</p
-000010e0: 3e0a 0a3c 7020 616c 6967 6e3d 2263 656e  >..<p align="cen
-000010f0: 7465 7222 3e0a 2020 2020 3c65 6d3e 7079  ter">.    <em>py
-00001100: 696e 6672 6120 6175 746f 6d61 7465 7320  infra automates 
-00001110: 696e 6672 6173 7472 7563 7475 7265 2075  infrastructure u
-00001120: 7369 6e67 2050 7974 686f 6e2e 2049 74e2  sing Python. It.
-00001130: 8099 7320 6661 7374 2061 6e64 2073 6361  ..s fast and sca
-00001140: 6c65 7320 6672 6f6d 206f 6e65 2073 6572  les from one ser
-00001150: 7665 7220 746f 2074 686f 7573 616e 6473  ver to thousands
-00001160: 2e20 4772 6561 7420 666f 7220 6164 2d68  . Great for ad-h
-00001170: 6f63 2063 6f6d 6d61 6e64 2065 7865 6375  oc command execu
-00001180: 7469 6f6e 2c20 7365 7276 6963 6520 6465  tion, service de
-00001190: 706c 6f79 6d65 6e74 2c20 636f 6e66 6967  ployment, config
-000011a0: 7572 6174 696f 6e20 6d61 6e61 6765 6d65  uration manageme
-000011b0: 6e74 2061 6e64 206d 6f72 652e 3c2f 656d  nt and more.</em
-000011c0: 3e0a 3c2f 703e 0a0a 2d2d 2d0a 0a3c 7020  >.</p>..---..<p 
-000011d0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-000011e0: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-000011f0: 7073 3a2f 2f64 6f63 732e 7079 696e 6672  ps://docs.pyinfr
-00001200: 612e 636f 6d22 3e3c 7374 726f 6e67 3e44  a.com"><strong>D
-00001210: 6f63 756d 656e 7461 7469 6f6e 3c2f 7374  ocumentation</st
-00001220: 726f 6e67 3e3c 2f61 3e20 2672 4172 723b  rong></a> &rArr;
-00001230: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-00001240: 7470 733a 2f2f 646f 6373 2e70 7969 6e66  tps://docs.pyinf
-00001250: 7261 2e63 6f6d 2f70 6167 652f 6765 7474  ra.com/page/gett
-00001260: 696e 672d 7374 6172 7465 642e 6874 6d6c  ing-started.html
-00001270: 223e 3c73 7472 6f6e 673e 4765 7474 696e  "><strong>Gettin
-00001280: 6720 5374 6172 7465 643c 2f73 7472 6f6e  g Started</stron
-00001290: 673e 3c2f 613e 2026 6275 6c6c 3b0a 2020  g></a> &bull;.  
-000012a0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-000012b0: 3a2f 2f64 6f63 732e 7079 696e 6672 612e  ://docs.pyinfra.
-000012c0: 636f 6d2f 7061 6765 2f65 7861 6d70 6c65  com/page/example
-000012d0: 732e 6874 6d6c 223e 3c73 7472 6f6e 673e  s.html"><strong>
-000012e0: 4578 616d 706c 6573 3c2f 7374 726f 6e67  Examples</strong
-000012f0: 3e3c 2f61 3e20 2662 756c 6c3b 0a20 2020  ></a> &bull;.   
-00001300: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00001310: 2f2f 646f 6373 2e70 7969 6e66 7261 2e63  //docs.pyinfra.c
-00001320: 6f6d 2f70 6167 652f 7375 7070 6f72 742e  om/page/support.
-00001330: 6874 6d6c 223e 3c73 7472 6f6e 673e 4865  html"><strong>He
-00001340: 6c70 2026 2053 7570 706f 7274 3c2f 7374  lp & Support</st
-00001350: 726f 6e67 3e3c 2f61 3e20 2662 756c 6c3b  rong></a> &bull;
-00001360: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-00001370: 7470 733a 2f2f 646f 6373 2e70 7969 6e66  tps://docs.pyinf
-00001380: 7261 2e63 6f6d 2f70 6167 652f 636f 6e74  ra.com/page/cont
-00001390: 7269 6275 7469 6e67 2e68 746d 6c22 3e3c  ributing.html"><
-000013a0: 7374 726f 6e67 3e43 6f6e 7472 6962 7574  strong>Contribut
-000013b0: 696e 673c 2f73 7472 6f6e 673e 3c2f 613e  ing</strong></a>
-000013c0: 0a3c 2f70 3e0a 0a3c 7020 616c 6967 6e3d  .</p>..<p align=
-000013d0: 2263 656e 7465 7222 3e0a 2020 2020 4368  "center">.    Ch
-000013e0: 6174 2026 7241 7272 3b0a 2020 2020 3c61  at &rArr;.    <a
-000013f0: 2068 7265 663d 2268 7474 7073 3a2f 2f6d   href="https://m
-00001400: 6174 7269 782e 746f 2f23 2f23 7079 696e  atrix.to/#/#pyin
-00001410: 6672 613a 6d61 7472 6978 2e6f 7267 223e  fra:matrix.org">
-00001420: 3c73 7472 6f6e 673e 3c63 6f64 653e 2370  <strong><code>#p
-00001430: 7969 6e66 7261 3c2f 636f 6465 3e20 6f6e  yinfra</code> on
-00001440: 204d 6174 7269 783c 2f73 7472 6f6e 673e   Matrix</strong>
-00001450: 3c2f 613e 0a3c 2f70 3e0a 0a2d 2d2d 0a0a  </a>.</p>..---..
-00001460: 5768 7920 7079 696e 6672 613f 2044 6573  Why pyinfra? Des
-00001470: 6967 6e20 6665 6174 7572 6573 2069 6e63  ign features inc
-00001480: 6c75 6465 3a0a 0a2b 20f0 9f9a 8020 2a2a  lude:..+ .... **
-00001490: 5375 7065 7220 6661 7374 2a2a 2065 7865  Super fast** exe
-000014a0: 6375 7469 6f6e 206f 7665 7220 7468 6f75  cution over thou
-000014b0: 7361 6e64 7320 6f66 2068 6f73 7473 2077  sands of hosts w
-000014c0: 6974 6820 7072 6564 6963 7461 626c 6520  ith predictable 
-000014d0: 7065 7266 6f72 6d61 6e63 652e 0a2b 20f0  performance..+ .
-000014e0: 9f9a a820 2a2a 496e 7374 616e 7420 6465  ... **Instant de
-000014f0: 6275 6767 696e 672a 2a20 7769 7468 2072  bugging** with r
-00001500: 6561 6c74 696d 6520 7374 6469 6e2f 7374  ealtime stdin/st
-00001510: 646f 7574 2f73 7464 6572 7220 6f75 7470  dout/stderr outp
-00001520: 7574 2028 602d 7676 7660 292e 0a2b 20f0  ut (`-vvv`)..+ .
-00001530: 9f94 8420 2a2a 4964 656d 706f 7465 6e74  ... **Idempotent
-00001540: 206f 7065 7261 7469 6f6e 732a 2a20 7468   operations** th
-00001550: 6174 2065 6e61 626c 6520 6469 6666 7320  at enable diffs 
-00001560: 616e 6420 6472 7920 7275 6e73 2062 6566  and dry runs bef
-00001570: 6f72 6520 6d61 6b69 6e67 2063 6861 6e67  ore making chang
-00001580: 6573 2e0a 2b20 f09f 93a6 202a 2a45 7874  es..+ .... **Ext
-00001590: 656e 6461 626c 652a 2a20 7769 7468 2074  endable** with t
-000015a0: 6865 2065 6e74 6972 6520 5079 7468 6f6e  he entire Python
-000015b0: 2070 6163 6b61 6765 2065 636f 7379 7374   package ecosyst
-000015c0: 656d 2e0a 2b20 f09f 92bb 202a 2a41 6765  em..+ .... **Age
-000015d0: 6e74 6c65 7373 2065 7865 6375 7469 6f6e  ntless execution
-000015e0: 2a2a 2061 6761 696e 7374 2061 6e79 7468  ** against anyth
-000015f0: 696e 6720 7769 7468 2073 6865 6c6c 2061  ing with shell a
-00001600: 6363 6573 732e 0a2b 20f0 9f94 8c20 2a2a  ccess..+ .... **
-00001610: 496e 7465 6772 6174 6564 2a2a 2077 6974  Integrated** wit
-00001620: 6820 636f 6e6e 6563 746f 7273 2066 6f72  h connectors for
-00001630: 2044 6f63 6b65 722c 2054 6572 7261 666f   Docker, Terrafo
-00001640: 726d 2c20 5661 6772 616e 7420 616e 6420  rm, Vagrant and 
-00001650: 6d6f 7265 2e0a 0a3c 696d 6720 7769 6474  more...<img widt
-00001660: 683d 2231 3030 2522 2073 7263 3d22 6874  h="100%" src="ht
-00001670: 7470 733a 2f2f 7079 696e 6672 612e 636f  tps://pyinfra.co
-00001680: 6d2f 7374 6174 6963 2f65 7861 6d70 6c65  m/static/example
-00001690: 5f64 6570 6c6f 792e 6769 6622 202f 3e0a  _deploy.gif" />.
-000016a0: 0a23 2320 5175 6963 6b73 7461 7274 0a0a  .## Quickstart..
-000016b0: 496e 7374 616c 6c20 7079 696e 6672 6120  Install pyinfra 
-000016c0: 7769 7468 2060 7069 7060 3a0a 0a60 6060  with `pip`:..```
-000016d0: 0a70 6970 2069 6e73 7461 6c6c 2070 7969  .pip install pyi
-000016e0: 6e66 7261 0a60 6060 0a0a 4e6f 7720 796f  nfra.```..Now yo
-000016f0: 7520 6361 6e20 6578 6563 7574 6520 636f  u can execute co
-00001700: 6d6d 616e 6473 206f 6e20 686f 7374 7320  mmands on hosts 
-00001710: 7669 6120 5353 483a 0a0a 6060 6073 680a  via SSH:..```sh.
-00001720: 7079 696e 6672 6120 6d79 2d73 6572 7665  pyinfra my-serve
-00001730: 722e 6e65 7420 6578 6563 202d 2d20 6563  r.net exec -- ec
-00001740: 686f 2022 6865 6c6c 6f20 776f 726c 6422  ho "hello world"
-00001750: 0a60 6060 0a0a 4f72 2074 6172 6765 7420  .```..Or target 
-00001760: 446f 636b 6572 2063 6f6e 7461 696e 6572  Docker container
-00001770: 732c 2074 6865 206c 6f63 616c 206d 6163  s, the local mac
-00001780: 6869 6e65 2c20 616e 6420 6f74 6865 7220  hine, and other 
-00001790: 5b63 6f6e 6e65 6374 6f72 735d 2868 7474  [connectors](htt
-000017a0: 7073 3a2f 2f64 6f63 732e 7079 696e 6672  ps://docs.pyinfr
-000017b0: 612e 636f 6d2f 7061 6765 2f63 6f6e 6e65  a.com/page/conne
-000017c0: 6374 6f72 732e 6874 6d6c 293a 0a0a 6060  ctors.html):..``
-000017d0: 6073 680a 7079 696e 6672 6120 4064 6f63  `sh.pyinfra @doc
-000017e0: 6b65 722f 7562 756e 7475 2065 7865 6320  ker/ubuntu exec 
-000017f0: 2d2d 2065 6368 6f20 2248 656c 6c6f 2077  -- echo "Hello w
-00001800: 6f72 6c64 220a 7079 696e 6672 6120 406c  orld".pyinfra @l
-00001810: 6f63 616c 2065 7865 6320 2d2d 2065 6368  ocal exec -- ech
-00001820: 6f20 2248 656c 6c6f 2077 6f72 6c64 220a  o "Hello world".
-00001830: 6060 600a 0a41 7320 7765 6c6c 2061 7320  ```..As well as 
-00001840: 6578 6563 7574 696e 6720 636f 6d6d 616e  executing comman
-00001850: 6473 2079 6f75 2063 616e 2064 6566 696e  ds you can defin
-00001860: 6520 7374 6174 6520 7573 696e 6720 5b6f  e state using [o
-00001870: 7065 7261 7469 6f6e 735d 2868 7474 7073  perations](https
-00001880: 3a2f 2f64 6f63 732e 7079 696e 6672 612e  ://docs.pyinfra.
-00001890: 636f 6d2f 7061 6765 2f6f 7065 7261 7469  com/page/operati
-000018a0: 6f6e 732e 6874 6d6c 293a 0a0a 6060 6073  ons.html):..```s
-000018b0: 680a 2320 496e 7374 616c 6c20 6966 746f  h.# Install ifto
-000018c0: 7020 6170 7420 7061 636b 6167 6520 6966  p apt package if
-000018d0: 206e 6f74 2070 7265 7365 6e74 0a70 7969   not present.pyi
-000018e0: 6e66 7261 2040 646f 636b 6572 2f75 6275  nfra @docker/ubu
-000018f0: 6e74 7520 6170 742e 7061 636b 6167 6573  ntu apt.packages
-00001900: 2069 6674 6f70 2075 7064 6174 653d 7472   iftop update=tr
-00001910: 7565 205f 7375 646f 3d74 7275 650a 6060  ue _sudo=true.``
-00001920: 600a 0a57 6869 6368 2063 616e 2074 6865  `..Which can the
-00001930: 6e20 6265 2073 6176 6564 2061 7320 6120  n be saved as a 
-00001940: 5079 7468 6f6e 2066 696c 6520 6c69 6b65  Python file like
-00001950: 2060 6465 706c 6f79 2e70 7960 3a0a 0a0a   `deploy.py`:...
-00001960: 6060 6070 790a 6672 6f6d 2070 7969 6e66  ```py.from pyinf
-00001970: 7261 2e6f 7065 7261 7469 6f6e 7320 696d  ra.operations im
-00001980: 706f 7274 2061 7074 0a0a 6170 742e 7061  port apt..apt.pa
-00001990: 636b 6167 6573 280a 2020 2020 6e61 6d65  ckages(.    name
-000019a0: 3d22 456e 7375 7265 2069 6674 6f70 2069  ="Ensure iftop i
-000019b0: 7320 696e 7374 616c 6c65 6422 2c0a 2020  s installed",.  
-000019c0: 2020 7061 636b 6167 6573 3d5b 2769 6674    packages=['ift
-000019d0: 6f70 275d 2c0a 2020 2020 7570 6461 7465  op'],.    update
-000019e0: 3d54 7275 652c 0a20 2020 205f 7375 646f  =True,.    _sudo
-000019f0: 3d54 7275 652c 0a29 0a60 6060 0a0a 5468  =True,.).```..Th
-00001a00: 6520 686f 7374 7320 6361 6e20 616c 736f  e hosts can also
-00001a10: 2062 6520 7361 7665 6420 696e 2061 2066   be saved in a f
-00001a20: 696c 652c 2066 6f72 2065 7861 6d70 6c65  ile, for example
-00001a30: 2060 696e 7665 6e74 6f72 792e 7079 603a   `inventory.py`:
-00001a40: 0a0a 6060 6070 790a 7461 7267 6574 7320  ..```py.targets 
-00001a50: 3d20 5b22 4064 6f63 6b65 722f 7562 756e  = ["@docker/ubun
-00001a60: 7475 222c 2022 6d79 2d74 6573 742d 7365  tu", "my-test-se
-00001a70: 7276 6572 2e6e 6574 225d 0a60 6060 0a0a  rver.net"].```..
-00001a80: 0a41 6e64 2065 7865 6375 7465 6420 746f  .And executed to
-00001a90: 6765 7468 6572 3a0a 0a60 6060 7368 0a70  gether:..```sh.p
-00001aa0: 7969 6e66 7261 2069 6e76 656e 746f 7279  yinfra inventory
-00001ab0: 2e70 7920 6465 706c 6f79 2e70 790a 6060  .py deploy.py.``
-00001ac0: 600a 0a4e 6f77 2079 6f75 206b 6e6f 7720  `..Now you know 
-00001ad0: 7468 6520 6275 696c 6469 6e67 2062 6c6f  the building blo
-00001ae0: 636b 7320 6f66 2070 7969 6e66 7261 2120  cks of pyinfra! 
-00001af0: 4279 2063 6f6d 6269 6e69 6e67 2069 6e76  By combining inv
-00001b00: 656e 746f 7279 2c20 6f70 6572 6174 696f  entory, operatio
-00001b10: 6e73 2061 6e64 2050 7974 686f 6e20 636f  ns and Python co
-00001b20: 6465 2079 6f75 2063 616e 2064 6570 6c6f  de you can deplo
-00001b30: 7920 616e 7974 6869 6e67 2e0a 0a53 6565  y anything...See
-00001b40: 2074 6865 206d 6f72 6520 6465 7461 696c   the more detail
-00001b50: 6564 205b 6765 7474 696e 6720 7374 6172  ed [getting star
-00001b60: 7465 645d 2868 7474 7073 3a2f 2f64 6f63  ted](https://doc
-00001b70: 732e 7079 696e 6672 612e 636f 6d2f 7061  s.pyinfra.com/pa
-00001b80: 6765 2f67 6574 7469 6e67 2d73 7461 7274  ge/getting-start
-00001b90: 6564 2e68 746d 6c29 206f 7220 5b75 7369  ed.html) or [usi
-00001ba0: 6e67 206f 7065 7261 7469 6f6e 735d 2868  ng operations](h
-00001bb0: 7474 7073 3a2f 2f64 6f63 732e 7079 696e  ttps://docs.pyin
-00001bc0: 6672 612e 636f 6d2f 7061 6765 2f75 7369  fra.com/page/usi
-00001bd0: 6e67 2d6f 7065 7261 7469 6f6e 732e 6874  ng-operations.ht
-00001be0: 6d6c 2920 6775 6964 6573 2e20 5365 6520  ml) guides. See 
-00001bf0: 686f 7720 746f 2075 7365 205b 696e 7665  how to use [inve
-00001c00: 6e74 6f72 7920 2620 6461 7461 5d28 6874  ntory & data](ht
-00001c10: 7470 733a 2f2f 646f 6373 2e70 7969 6e66  tps://docs.pyinf
-00001c20: 7261 2e63 6f6d 2f70 6167 652f 696e 7665  ra.com/page/inve
-00001c30: 6e74 6f72 792d 6461 7461 2e68 746d 6c29  ntory-data.html)
-00001c40: 2c20 5b67 6c6f 6261 6c20 6172 6775 6d65  , [global argume
-00001c50: 6e74 735d 2868 7474 7073 3a2f 2f64 6f63  nts](https://doc
-00001c60: 732e 7079 696e 6672 612e 636f 6d2f 7061  s.pyinfra.com/pa
-00001c70: 6765 2f61 7267 756d 656e 7473 2e68 746d  ge/arguments.htm
-00001c80: 6c29 2061 6e64 205b 7468 6520 434c 495d  l) and [the CLI]
-00001c90: 2868 7474 7073 3a2f 2f64 6f63 732e 7079  (https://docs.py
-00001ca0: 696e 6672 612e 636f 6d2f 7061 6765 2f63  infra.com/page/c
-00001cb0: 6c69 2e68 746d 6c29 206f 7220 6368 6563  li.html) or chec
-00001cc0: 6b20 6f75 7420 7468 6520 5b64 6f63 756d  k out the [docum
-00001cd0: 656e 7465 6420 6578 616d 706c 6573 5d28  ented examples](
-00001ce0: 6874 7470 733a 2f2f 646f 6373 2e70 7969  https://docs.pyi
-00001cf0: 6e66 7261 2e63 6f6d 2f70 6167 652f 6578  nfra.com/page/ex
-00001d00: 616d 706c 6573 2e68 746d 6c29 2e0a 0a2d  amples.html)...-
-00001d10: 2d2d 0a0a 3c70 2061 6c69 676e 3d22 6365  --..<p align="ce
-00001d20: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
-00001d30: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
-00001d40: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
-00001d50: 2f70 7969 6e66 7261 223e 3c69 6d67 2061  /pyinfra"><img a
-00001d60: 6c74 3d22 5079 5049 2076 6572 7369 6f6e  lt="PyPI version
-00001d70: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00001d80: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00001d90: 7069 2f76 2f70 7969 6e66 7261 3f63 6f6c  pi/v/pyinfra?col
-00001da0: 6f72 3d62 6c75 6522 3e3c 2f61 3e0a 2020  or=blue"></a>.  
-00001db0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00001dc0: 3a2f 2f70 6570 792e 7465 6368 2f70 726f  ://pepy.tech/pro
-00001dd0: 6a65 6374 2f70 7969 6e66 7261 223e 3c69  ject/pyinfra"><i
-00001de0: 6d67 2061 6c74 3d22 5079 5069 2064 6f77  mg alt="PyPi dow
-00001df0: 6e6c 6f61 6473 2220 7372 633d 2268 7474  nloads" src="htt
-00001e00: 7073 3a2f 2f70 6570 792e 7465 6368 2f62  ps://pepy.tech/b
-00001e10: 6164 6765 2f70 7969 6e66 7261 223e 3c2f  adge/pyinfra"></
-00001e20: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
-00001e30: 6874 7470 733a 2f2f 646f 6373 2e70 7969  https://docs.pyi
-00001e40: 6e66 7261 2e63 6f6d 223e 3c69 6d67 2061  nfra.com"><img a
-00001e50: 6c74 3d22 446f 6373 2073 7461 7475 7322  lt="Docs status"
-00001e60: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00001e70: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
-00001e80: 6875 622f 6163 7469 6f6e 732f 776f 726b  hub/actions/work
-00001e90: 666c 6f77 2f73 7461 7475 732f 4669 7a7a  flow/status/Fizz
-00001ea0: 6164 6172 2f70 7969 6e66 7261 2f64 6f63  adar/pyinfra/doc
-00001eb0: 732e 796d 6c3f 6272 616e 6368 3d32 2e78  s.yml?branch=2.x
-00001ec0: 223e 3c2f 613e 0a20 2020 203c 6120 6872  "></a>.    <a hr
-00001ed0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00001ee0: 7562 2e63 6f6d 2f46 697a 7a61 6461 722f  ub.com/Fizzadar/
-00001ef0: 7079 696e 6672 612f 6163 7469 6f6e 733f  pyinfra/actions?
-00001f00: 7175 6572 793d 776f 726b 666c 6f77 2533  query=workflow%3
-00001f10: 4125 3232 4578 6563 7574 652b 7465 7374  A%22Execute+test
-00001f20: 7325 3232 223e 3c69 6d67 2061 6c74 3d22  s%22"><img alt="
-00001f30: 4578 6563 7574 6520 7465 7374 7320 7374  Execute tests st
-00001f40: 6174 7573 2220 7372 633d 2268 7474 7073  atus" src="https
-00001f50: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00001f60: 6f2f 6769 7468 7562 2f61 6374 696f 6e73  o/github/actions
-00001f70: 2f77 6f72 6b66 6c6f 772f 7374 6174 7573  /workflow/status
-00001f80: 2f46 697a 7a61 6461 722f 7079 696e 6672  /Fizzadar/pyinfr
-00001f90: 612f 7465 7374 2e79 6d6c 3f62 7261 6e63  a/test.yml?branc
-00001fa0: 683d 322e 7822 3e3c 2f61 3e0a 2020 2020  h=2.x"></a>.    
-00001fb0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001fc0: 2f63 6f64 6563 6f76 2e69 6f2f 6769 7468  /codecov.io/gith
-00001fd0: 7562 2f46 697a 7a61 6461 722f 7079 696e  ub/Fizzadar/pyin
-00001fe0: 6672 6122 3e3c 696d 6720 616c 743d 2243  fra"><img alt="C
-00001ff0: 6f64 6563 6f76 2043 6f76 6572 6167 6522  odecov Coverage"
-00002000: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00002010: 672e 7368 6965 6c64 732e 696f 2f63 6f64  g.shields.io/cod
-00002020: 6563 6f76 2f63 2f67 682f 4669 7a7a 6164  ecov/c/gh/Fizzad
-00002030: 6172 2f70 7969 6e66 7261 223e 3c2f 613e  ar/pyinfra"></a>
-00002040: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-00002050: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002060: 2f46 697a 7a61 6461 722f 7079 696e 6672  /Fizzadar/pyinfr
-00002070: 612f 626c 6f62 2f32 2e78 2f4c 4943 454e  a/blob/2.x/LICEN
-00002080: 5345 2e6d 6422 3e3c 696d 6720 616c 743d  SE.md"><img alt=
-00002090: 224d 4954 204c 6963 656e 7365 6422 2073  "MIT Licensed" s
-000020a0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-000020b0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-000020c0: 6c2f 7079 696e 6672 6122 3e3c 2f61 3e0a  l/pyinfra"></a>.
-000020d0: 3c2f 703e 0a                             </p>.
+00000b10: 2d44 6973 743a 206d 7970 793b 2065 7874  -Dist: mypy; ext
+00000b20: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+00000b30: 6972 6573 2d44 6973 743a 2074 7970 6573  ires-Dist: types
+00000b40: 2d63 7279 7074 6f67 7261 7068 793b 2065  -cryptography; e
+00000b50: 7874 7261 203d 3d20 2264 6576 220a 5265  xtra == "dev".Re
+00000b60: 7175 6972 6573 2d44 6973 743a 2074 7970  quires-Dist: typ
+00000b70: 6573 2d70 6172 616d 696b 6f3b 2065 7874  es-paramiko; ext
+00000b80: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+00000b90: 6972 6573 2d44 6973 743a 2074 7970 6573  ires-Dist: types
+00000ba0: 2d70 7974 686f 6e2d 6461 7465 7574 696c  -python-dateutil
+00000bb0: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
+00000bc0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000bd0: 7479 7065 732d 5079 5941 4d4c 3b20 6578  types-PyYAML; ex
+00000be0: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+00000bf0: 7569 7265 732d 4469 7374 3a20 7479 7065  uires-Dist: type
+00000c00: 732d 7365 7475 7074 6f6f 6c73 3b20 6578  s-setuptools; ex
+00000c10: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+00000c20: 7569 7265 732d 4469 7374 3a20 7079 696e  uires-Dist: pyin
+00000c30: 6672 612d 6775 7a7a 6c65 5f73 7068 696e  fra-guzzle_sphin
+00000c40: 785f 7468 656d 653d 3d30 2e31 353b 2065  x_theme==0.15; e
+00000c50: 7874 7261 203d 3d20 2264 6576 220a 5265  xtra == "dev".Re
+00000c60: 7175 6972 6573 2d44 6973 743a 206d 7973  quires-Dist: mys
+00000c70: 742d 7061 7273 6572 3d3d 322e 302e 303b  t-parser==2.0.0;
+00000c80: 2065 7874 7261 203d 3d20 2264 6576 220a   extra == "dev".
+00000c90: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
+00000ca0: 7068 696e 783d 3d36 2e32 2e31 3b20 6578  phinx==6.2.1; ex
+00000cb0: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+00000cc0: 7569 7265 732d 4469 7374 3a20 7768 6565  uires-Dist: whee
+00000cd0: 6c3b 2065 7874 7261 203d 3d20 2264 6576  l; extra == "dev
+00000ce0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000cf0: 2074 7769 6e65 3b20 6578 7472 6120 3d3d   twine; extra ==
+00000d00: 2022 6465 7622 0a52 6571 7569 7265 732d   "dev".Requires-
+00000d10: 4469 7374 3a20 6970 7974 686f 6e3b 2065  Dist: ipython; e
+00000d20: 7874 7261 203d 3d20 2264 6576 220a 5265  xtra == "dev".Re
+00000d30: 7175 6972 6573 2d44 6973 743a 2069 7064  quires-Dist: ipd
+00000d40: 623b 2065 7874 7261 203d 3d20 2264 6576  b; extra == "dev
+00000d50: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000d60: 2069 7064 6270 6c75 6769 6e3b 2065 7874   ipdbplugin; ext
+00000d70: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+00000d80: 6972 6573 2d44 6973 743a 2066 6c61 6b65  ires-Dist: flake
+00000d90: 382d 7370 656c 6c63 6865 636b 3d3d 302e  8-spellcheck==0.
+00000da0: 3132 2e31 3b20 6578 7472 6120 3d3d 2022  12.1; extra == "
+00000db0: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
+00000dc0: 7374 3a20 7265 6462 6172 6f6e 3b20 6578  st: redbaron; ex
+00000dd0: 7472 6120 3d3d 2022 6465 7622 0a0a 3c70  tra == "dev"..<p
+00000de0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000df0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000e00: 7470 733a 2f2f 7079 696e 6672 612e 636f  tps://pyinfra.co
+00000e10: 6d22 3e0a 2020 2020 2020 2020 3c69 6d67  m">.        <img
+00000e20: 2073 7263 3d22 6874 7470 733a 2f2f 7079   src="https://py
+00000e30: 696e 6672 612e 636f 6d2f 7374 6174 6963  infra.com/static
+00000e40: 2f6c 6f67 6f5f 7265 6164 6d65 2e70 6e67  /logo_readme.png
+00000e50: 2220 616c 743d 2270 7969 6e66 7261 2220  " alt="pyinfra" 
+00000e60: 2f3e 0a20 2020 203c 2f61 3e0a 3c2f 703e  />.    </a>.</p>
+00000e70: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00000e80: 6572 223e 0a20 2020 203c 7374 726f 6e67  er">.    <strong
+00000e90: 3e4e 6f74 653a 2074 6869 7320 6973 2074  >Note: this is t
+00000ea0: 6865 2076 3320 6272 616e 6368 2c20 7768  he v3 branch, wh
+00000eb0: 6963 6820 6973 2063 7572 7265 6e74 6c79  ich is currently
+00000ec0: 2069 6e20 6265 7461 2e20 3c61 2068 7265   in beta. <a hre
+00000ed0: 663d 2268 7474 7073 3a2f 2f64 6f63 732e  f="https://docs.
+00000ee0: 7079 696e 6672 612e 636f 6d2f 656e 2f6e  pyinfra.com/en/n
+00000ef0: 6578 7422 3e53 6565 2074 6865 2064 6f63  ext">See the doc
+00000f00: 7320 666f 7220 7633 3c2f 613e 2e20 4966  s for v3</a>. If
+00000f10: 206e 6565 6465 6420 7468 6520 3c61 2068   needed the <a h
+00000f20: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000f30: 6875 622e 636f 6d2f 7079 696e 6672 612d  hub.com/pyinfra-
+00000f40: 6465 762f 7079 696e 6672 612f 7472 6565  dev/pyinfra/tree
+00000f50: 2f32 2e78 2f22 3e32 2e78 2062 7261 6e63  /2.x/">2.x branc
+00000f60: 6820 6973 2068 6572 653c 2f61 3e2c 2062  h is here</a>, b
+00000f70: 7574 2069 7320 696e 2062 7567 6669 7820  ut is in bugfix 
+00000f80: 6f6e 6c79 206d 6f64 652e 3c2f 7374 726f  only mode.</stro
+00000f90: 6e67 3e0a 3c2f 703e 0a0a 3c70 2061 6c69  ng>.</p>..<p ali
+00000fa0: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
+00000fb0: 203c 656d 3e70 7969 6e66 7261 2061 7574   <em>pyinfra aut
+00000fc0: 6f6d 6174 6573 2069 6e66 7261 7374 7275  omates infrastru
+00000fd0: 6374 7572 6520 7573 696e 6720 5079 7468  cture using Pyth
+00000fe0: 6f6e 2e20 4974 e280 9973 2066 6173 7420  on. It...s fast 
+00000ff0: 616e 6420 7363 616c 6573 2066 726f 6d20  and scales from 
+00001000: 6f6e 6520 7365 7276 6572 2074 6f20 7468  one server to th
+00001010: 6f75 7361 6e64 732e 2047 7265 6174 2066  ousands. Great f
+00001020: 6f72 2061 642d 686f 6320 636f 6d6d 616e  or ad-hoc comman
+00001030: 6420 6578 6563 7574 696f 6e2c 2073 6572  d execution, ser
+00001040: 7669 6365 2064 6570 6c6f 796d 656e 742c  vice deployment,
+00001050: 2063 6f6e 6669 6775 7261 7469 6f6e 206d   configuration m
+00001060: 616e 6167 656d 656e 7420 616e 6420 6d6f  anagement and mo
+00001070: 7265 2e3c 2f65 6d3e 0a3c 2f70 3e0a 0a2d  re.</em>.</p>..-
+00001080: 2d2d 0a0a 3c70 2061 6c69 676e 3d22 6365  --..<p align="ce
+00001090: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
+000010a0: 6566 3d22 6874 7470 733a 2f2f 646f 6373  ef="https://docs
+000010b0: 2e70 7969 6e66 7261 2e63 6f6d 223e 3c73  .pyinfra.com"><s
+000010c0: 7472 6f6e 673e 446f 6375 6d65 6e74 6174  trong>Documentat
+000010d0: 696f 6e3c 2f73 7472 6f6e 673e 3c2f 613e  ion</strong></a>
+000010e0: 2026 7241 7272 3b0a 2020 2020 3c61 2068   &rArr;.    <a h
+000010f0: 7265 663d 2268 7474 7073 3a2f 2f64 6f63  ref="https://doc
+00001100: 732e 7079 696e 6672 612e 636f 6d2f 7061  s.pyinfra.com/pa
+00001110: 6765 2f67 6574 7469 6e67 2d73 7461 7274  ge/getting-start
+00001120: 6564 2e68 746d 6c22 3e3c 7374 726f 6e67  ed.html"><strong
+00001130: 3e47 6574 7469 6e67 2053 7461 7274 6564  >Getting Started
+00001140: 3c2f 7374 726f 6e67 3e3c 2f61 3e20 2662  </strong></a> &b
+00001150: 756c 6c3b 0a20 2020 203c 6120 6872 6566  ull;.    <a href
+00001160: 3d22 6874 7470 733a 2f2f 646f 6373 2e70  ="https://docs.p
+00001170: 7969 6e66 7261 2e63 6f6d 2f70 6167 652f  yinfra.com/page/
+00001180: 6578 616d 706c 6573 2e68 746d 6c22 3e3c  examples.html"><
+00001190: 7374 726f 6e67 3e45 7861 6d70 6c65 733c  strong>Examples<
+000011a0: 2f73 7472 6f6e 673e 3c2f 613e 2026 6275  /strong></a> &bu
+000011b0: 6c6c 3b0a 2020 2020 3c61 2068 7265 663d  ll;.    <a href=
+000011c0: 2268 7474 7073 3a2f 2f64 6f63 732e 7079  "https://docs.py
+000011d0: 696e 6672 612e 636f 6d2f 7061 6765 2f73  infra.com/page/s
+000011e0: 7570 706f 7274 2e68 746d 6c22 3e3c 7374  upport.html"><st
+000011f0: 726f 6e67 3e48 656c 7020 2620 5375 7070  rong>Help & Supp
+00001200: 6f72 743c 2f73 7472 6f6e 673e 3c2f 613e  ort</strong></a>
+00001210: 2026 6275 6c6c 3b0a 2020 2020 3c61 2068   &bull;.    <a h
+00001220: 7265 663d 2268 7474 7073 3a2f 2f64 6f63  ref="https://doc
+00001230: 732e 7079 696e 6672 612e 636f 6d2f 7061  s.pyinfra.com/pa
+00001240: 6765 2f63 6f6e 7472 6962 7574 696e 672e  ge/contributing.
+00001250: 6874 6d6c 223e 3c73 7472 6f6e 673e 436f  html"><strong>Co
+00001260: 6e74 7269 6275 7469 6e67 3c2f 7374 726f  ntributing</stro
+00001270: 6e67 3e3c 2f61 3e0a 3c2f 703e 0a0a 3c70  ng></a>.</p>..<p
+00001280: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00001290: 0a20 2020 2043 6861 7420 2672 4172 723b  .    Chat &rArr;
+000012a0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+000012b0: 7470 733a 2f2f 6d61 7472 6978 2e74 6f2f  tps://matrix.to/
+000012c0: 232f 2370 7969 6e66 7261 3a6d 6174 7269  #/#pyinfra:matri
+000012d0: 782e 6f72 6722 3e3c 7374 726f 6e67 3e3c  x.org"><strong><
+000012e0: 636f 6465 3e23 7079 696e 6672 613c 2f63  code>#pyinfra</c
+000012f0: 6f64 653e 206f 6e20 4d61 7472 6978 3c2f  ode> on Matrix</
+00001300: 7374 726f 6e67 3e3c 2f61 3e0a 3c2f 703e  strong></a>.</p>
+00001310: 0a0a 2d2d 2d0a 0a57 6879 2070 7969 6e66  ..---..Why pyinf
+00001320: 7261 3f20 4465 7369 676e 2066 6561 7475  ra? Design featu
+00001330: 7265 7320 696e 636c 7564 653a 0a0a 2b20  res include:..+ 
+00001340: f09f 9a80 202a 2a53 7570 6572 2066 6173  .... **Super fas
+00001350: 742a 2a20 6578 6563 7574 696f 6e20 6f76  t** execution ov
+00001360: 6572 2074 686f 7573 616e 6473 206f 6620  er thousands of 
+00001370: 686f 7374 7320 7769 7468 2070 7265 6469  hosts with predi
+00001380: 6374 6162 6c65 2070 6572 666f 726d 616e  ctable performan
+00001390: 6365 2e0a 2b20 f09f 9aa8 202a 2a49 6e73  ce..+ .... **Ins
+000013a0: 7461 6e74 2064 6562 7567 6769 6e67 2a2a  tant debugging**
+000013b0: 2077 6974 6820 7265 616c 7469 6d65 2073   with realtime s
+000013c0: 7464 696e 2f73 7464 6f75 742f 7374 6465  tdin/stdout/stde
+000013d0: 7272 206f 7574 7075 7420 2860 2d76 7676  rr output (`-vvv
+000013e0: 6029 2e0a 2b20 f09f 9484 202a 2a49 6465  `)..+ .... **Ide
+000013f0: 6d70 6f74 656e 7420 6f70 6572 6174 696f  mpotent operatio
+00001400: 6e73 2a2a 2074 6861 7420 656e 6162 6c65  ns** that enable
+00001410: 2064 6966 6673 2061 6e64 2064 7279 2072   diffs and dry r
+00001420: 756e 7320 6265 666f 7265 206d 616b 696e  uns before makin
+00001430: 6720 6368 616e 6765 732e 0a2b 20f0 9f93  g changes..+ ...
+00001440: a620 2a2a 4578 7465 6e64 6162 6c65 2a2a  . **Extendable**
+00001450: 2077 6974 6820 7468 6520 656e 7469 7265   with the entire
+00001460: 2050 7974 686f 6e20 7061 636b 6167 6520   Python package 
+00001470: 6563 6f73 7973 7465 6d2e 0a2b 20f0 9f92  ecosystem..+ ...
+00001480: bb20 2a2a 4167 656e 746c 6573 7320 6578  . **Agentless ex
+00001490: 6563 7574 696f 6e2a 2a20 6167 6169 6e73  ecution** agains
+000014a0: 7420 616e 7974 6869 6e67 2077 6974 6820  t anything with 
+000014b0: 7368 656c 6c20 6163 6365 7373 2e0a 2b20  shell access..+ 
+000014c0: f09f 948c 202a 2a49 6e74 6567 7261 7465  .... **Integrate
+000014d0: 642a 2a20 7769 7468 2063 6f6e 6e65 6374  d** with connect
+000014e0: 6f72 7320 666f 7220 446f 636b 6572 2c20  ors for Docker, 
+000014f0: 5465 7272 6166 6f72 6d2c 2056 6167 7261  Terraform, Vagra
+00001500: 6e74 2061 6e64 206d 6f72 652e 0a0a 3c69  nt and more...<i
+00001510: 6d67 2077 6964 7468 3d22 3130 3025 2220  mg width="100%" 
+00001520: 7372 633d 2268 7474 7073 3a2f 2f70 7969  src="https://pyi
+00001530: 6e66 7261 2e63 6f6d 2f73 7461 7469 632f  nfra.com/static/
+00001540: 6578 616d 706c 655f 6465 706c 6f79 2e67  example_deploy.g
+00001550: 6966 2220 2f3e 0a0a 2323 2051 7569 636b  if" />..## Quick
+00001560: 7374 6172 740a 0a49 6e73 7461 6c6c 2070  start..Install p
+00001570: 7969 6e66 7261 2077 6974 6820 6070 6970  yinfra with `pip
+00001580: 603a 0a0a 6060 600a 7069 7020 696e 7374  `:..```.pip inst
+00001590: 616c 6c20 7079 696e 6672 610a 6060 600a  all pyinfra.```.
+000015a0: 0a4e 6f77 2079 6f75 2063 616e 2065 7865  .Now you can exe
+000015b0: 6375 7465 2063 6f6d 6d61 6e64 7320 6f6e  cute commands on
+000015c0: 2068 6f73 7473 2076 6961 2053 5348 3a0a   hosts via SSH:.
+000015d0: 0a60 6060 7368 0a70 7969 6e66 7261 206d  .```sh.pyinfra m
+000015e0: 792d 7365 7276 6572 2e6e 6574 2065 7865  y-server.net exe
+000015f0: 6320 2d2d 2065 6368 6f20 2268 656c 6c6f  c -- echo "hello
+00001600: 2077 6f72 6c64 220a 6060 600a 0a4f 7220   world".```..Or 
+00001610: 7461 7267 6574 2044 6f63 6b65 7220 636f  target Docker co
+00001620: 6e74 6169 6e65 7273 2c20 7468 6520 6c6f  ntainers, the lo
+00001630: 6361 6c20 6d61 6368 696e 652c 2061 6e64  cal machine, and
+00001640: 206f 7468 6572 205b 636f 6e6e 6563 746f   other [connecto
+00001650: 7273 5d28 6874 7470 733a 2f2f 646f 6373  rs](https://docs
+00001660: 2e70 7969 6e66 7261 2e63 6f6d 2f70 6167  .pyinfra.com/pag
+00001670: 652f 636f 6e6e 6563 746f 7273 2e68 746d  e/connectors.htm
+00001680: 6c29 3a0a 0a60 6060 7368 0a70 7969 6e66  l):..```sh.pyinf
+00001690: 7261 2040 646f 636b 6572 2f75 6275 6e74  ra @docker/ubunt
+000016a0: 7520 6578 6563 202d 2d20 6563 686f 2022  u exec -- echo "
+000016b0: 4865 6c6c 6f20 776f 726c 6422 0a70 7969  Hello world".pyi
+000016c0: 6e66 7261 2040 6c6f 6361 6c20 6578 6563  nfra @local exec
+000016d0: 202d 2d20 6563 686f 2022 4865 6c6c 6f20   -- echo "Hello 
+000016e0: 776f 726c 6422 0a60 6060 0a0a 4173 2077  world".```..As w
+000016f0: 656c 6c20 6173 2065 7865 6375 7469 6e67  ell as executing
+00001700: 2063 6f6d 6d61 6e64 7320 796f 7520 6361   commands you ca
+00001710: 6e20 6465 6669 6e65 2073 7461 7465 2075  n define state u
+00001720: 7369 6e67 205b 6f70 6572 6174 696f 6e73  sing [operations
+00001730: 5d28 6874 7470 733a 2f2f 646f 6373 2e70  ](https://docs.p
+00001740: 7969 6e66 7261 2e63 6f6d 2f70 6167 652f  yinfra.com/page/
+00001750: 6f70 6572 6174 696f 6e73 2e68 746d 6c29  operations.html)
+00001760: 3a0a 0a60 6060 7368 0a23 2049 6e73 7461  :..```sh.# Insta
+00001770: 6c6c 2069 6674 6f70 2061 7074 2070 6163  ll iftop apt pac
+00001780: 6b61 6765 2069 6620 6e6f 7420 7072 6573  kage if not pres
+00001790: 656e 740a 7079 696e 6672 6120 4064 6f63  ent.pyinfra @doc
+000017a0: 6b65 722f 7562 756e 7475 2061 7074 2e70  ker/ubuntu apt.p
+000017b0: 6163 6b61 6765 7320 6966 746f 7020 7570  ackages iftop up
+000017c0: 6461 7465 3d74 7275 6520 5f73 7564 6f3d  date=true _sudo=
+000017d0: 7472 7565 0a60 6060 0a0a 5768 6963 6820  true.```..Which 
+000017e0: 6361 6e20 7468 656e 2062 6520 7361 7665  can then be save
+000017f0: 6420 6173 2061 2050 7974 686f 6e20 6669  d as a Python fi
+00001800: 6c65 206c 696b 6520 6064 6570 6c6f 792e  le like `deploy.
+00001810: 7079 603a 0a0a 0a60 6060 7079 0a66 726f  py`:...```py.fro
+00001820: 6d20 7079 696e 6672 612e 6f70 6572 6174  m pyinfra.operat
+00001830: 696f 6e73 2069 6d70 6f72 7420 6170 740a  ions import apt.
+00001840: 0a61 7074 2e70 6163 6b61 6765 7328 0a20  .apt.packages(. 
+00001850: 2020 206e 616d 653d 2245 6e73 7572 6520     name="Ensure 
+00001860: 6966 746f 7020 6973 2069 6e73 7461 6c6c  iftop is install
+00001870: 6564 222c 0a20 2020 2070 6163 6b61 6765  ed",.    package
+00001880: 733d 5b27 6966 746f 7027 5d2c 0a20 2020  s=['iftop'],.   
+00001890: 2075 7064 6174 653d 5472 7565 2c0a 2020   update=True,.  
+000018a0: 2020 5f73 7564 6f3d 5472 7565 2c0a 290a    _sudo=True,.).
+000018b0: 6060 600a 0a54 6865 2068 6f73 7473 2063  ```..The hosts c
+000018c0: 616e 2061 6c73 6f20 6265 2073 6176 6564  an also be saved
+000018d0: 2069 6e20 6120 6669 6c65 2c20 666f 7220   in a file, for 
+000018e0: 6578 616d 706c 6520 6069 6e76 656e 746f  example `invento
+000018f0: 7279 2e70 7960 3a0a 0a60 6060 7079 0a74  ry.py`:..```py.t
+00001900: 6172 6765 7473 203d 205b 2240 646f 636b  argets = ["@dock
+00001910: 6572 2f75 6275 6e74 7522 2c20 226d 792d  er/ubuntu", "my-
+00001920: 7465 7374 2d73 6572 7665 722e 6e65 7422  test-server.net"
+00001930: 5d0a 6060 600a 0a0a 416e 6420 6578 6563  ].```...And exec
+00001940: 7574 6564 2074 6f67 6574 6865 723a 0a0a  uted together:..
+00001950: 6060 6073 680a 7079 696e 6672 6120 696e  ```sh.pyinfra in
+00001960: 7665 6e74 6f72 792e 7079 2064 6570 6c6f  ventory.py deplo
+00001970: 792e 7079 0a60 6060 0a0a 4e6f 7720 796f  y.py.```..Now yo
+00001980: 7520 6b6e 6f77 2074 6865 2062 7569 6c64  u know the build
+00001990: 696e 6720 626c 6f63 6b73 206f 6620 7079  ing blocks of py
+000019a0: 696e 6672 6121 2042 7920 636f 6d62 696e  infra! By combin
+000019b0: 696e 6720 696e 7665 6e74 6f72 792c 206f  ing inventory, o
+000019c0: 7065 7261 7469 6f6e 7320 616e 6420 5079  perations and Py
+000019d0: 7468 6f6e 2063 6f64 6520 796f 7520 6361  thon code you ca
+000019e0: 6e20 6465 706c 6f79 2061 6e79 7468 696e  n deploy anythin
+000019f0: 672e 0a0a 5365 6520 7468 6520 6d6f 7265  g...See the more
+00001a00: 2064 6574 6169 6c65 6420 5b67 6574 7469   detailed [getti
+00001a10: 6e67 2073 7461 7274 6564 5d28 6874 7470  ng started](http
+00001a20: 733a 2f2f 646f 6373 2e70 7969 6e66 7261  s://docs.pyinfra
+00001a30: 2e63 6f6d 2f70 6167 652f 6765 7474 696e  .com/page/gettin
+00001a40: 672d 7374 6172 7465 642e 6874 6d6c 2920  g-started.html) 
+00001a50: 6f72 205b 7573 696e 6720 6f70 6572 6174  or [using operat
+00001a60: 696f 6e73 5d28 6874 7470 733a 2f2f 646f  ions](https://do
+00001a70: 6373 2e70 7969 6e66 7261 2e63 6f6d 2f70  cs.pyinfra.com/p
+00001a80: 6167 652f 7573 696e 672d 6f70 6572 6174  age/using-operat
+00001a90: 696f 6e73 2e68 746d 6c29 2067 7569 6465  ions.html) guide
+00001aa0: 732e 2053 6565 2068 6f77 2074 6f20 7573  s. See how to us
+00001ab0: 6520 5b69 6e76 656e 746f 7279 2026 2064  e [inventory & d
+00001ac0: 6174 615d 2868 7474 7073 3a2f 2f64 6f63  ata](https://doc
+00001ad0: 732e 7079 696e 6672 612e 636f 6d2f 7061  s.pyinfra.com/pa
+00001ae0: 6765 2f69 6e76 656e 746f 7279 2d64 6174  ge/inventory-dat
+00001af0: 612e 6874 6d6c 292c 205b 676c 6f62 616c  a.html), [global
+00001b00: 2061 7267 756d 656e 7473 5d28 6874 7470   arguments](http
+00001b10: 733a 2f2f 646f 6373 2e70 7969 6e66 7261  s://docs.pyinfra
+00001b20: 2e63 6f6d 2f70 6167 652f 6172 6775 6d65  .com/page/argume
+00001b30: 6e74 732e 6874 6d6c 2920 616e 6420 5b74  nts.html) and [t
+00001b40: 6865 2043 4c49 5d28 6874 7470 733a 2f2f  he CLI](https://
+00001b50: 646f 6373 2e70 7969 6e66 7261 2e63 6f6d  docs.pyinfra.com
+00001b60: 2f70 6167 652f 636c 692e 6874 6d6c 2920  /page/cli.html) 
+00001b70: 6f72 2063 6865 636b 206f 7574 2074 6865  or check out the
+00001b80: 205b 646f 6375 6d65 6e74 6564 2065 7861   [documented exa
+00001b90: 6d70 6c65 735d 2868 7474 7073 3a2f 2f64  mples](https://d
+00001ba0: 6f63 732e 7079 696e 6672 612e 636f 6d2f  ocs.pyinfra.com/
+00001bb0: 7061 6765 2f65 7861 6d70 6c65 732e 6874  page/examples.ht
+00001bc0: 6d6c 292e 0a0a 2d2d 2d0a 0a3c 7020 616c  ml)...---..<p al
+00001bd0: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00001be0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00001bf0: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+00001c00: 7267 2f70 7970 692f 7079 696e 6672 6122  rg/pypi/pyinfra"
+00001c10: 3e3c 696d 6720 616c 743d 2250 7950 4920  ><img alt="PyPI 
+00001c20: 7665 7273 696f 6e22 2073 7263 3d22 6874  version" src="ht
+00001c30: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00001c40: 732e 696f 2f70 7970 692f 762f 7079 696e  s.io/pypi/v/pyin
+00001c50: 6672 613f 636f 6c6f 723d 626c 7565 223e  fra?color=blue">
+00001c60: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
+00001c70: 3d22 6874 7470 733a 2f2f 7065 7079 2e74  ="https://pepy.t
+00001c80: 6563 682f 7072 6f6a 6563 742f 7079 696e  ech/project/pyin
+00001c90: 6672 6122 3e3c 696d 6720 616c 743d 2250  fra"><img alt="P
+00001ca0: 7950 6920 646f 776e 6c6f 6164 7322 2073  yPi downloads" s
+00001cb0: 7263 3d22 6874 7470 733a 2f2f 7065 7079  rc="https://pepy
+00001cc0: 2e74 6563 682f 6261 6467 652f 7079 696e  .tech/badge/pyin
+00001cd0: 6672 6122 3e3c 2f61 3e0a 2020 2020 3c61  fra"></a>.    <a
+00001ce0: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+00001cf0: 6f63 732e 7079 696e 6672 612e 636f 6d22  ocs.pyinfra.com"
+00001d00: 3e3c 696d 6720 616c 743d 2244 6f63 7320  ><img alt="Docs 
+00001d10: 7374 6174 7573 2220 7372 633d 2268 7474  status" src="htt
+00001d20: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00001d30: 2e69 6f2f 6769 7468 7562 2f61 6374 696f  .io/github/actio
+00001d40: 6e73 2f77 6f72 6b66 6c6f 772f 7374 6174  ns/workflow/stat
+00001d50: 7573 2f46 697a 7a61 6461 722f 7079 696e  us/Fizzadar/pyin
+00001d60: 6672 612f 646f 6373 2e79 6d6c 3f62 7261  fra/docs.yml?bra
+00001d70: 6e63 683d 322e 7822 3e3c 2f61 3e0a 2020  nch=2.x"></a>.  
+00001d80: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00001d90: 3a2f 2f67 6974 6875 622e 636f 6d2f 4669  ://github.com/Fi
+00001da0: 7a7a 6164 6172 2f70 7969 6e66 7261 2f61  zzadar/pyinfra/a
+00001db0: 6374 696f 6e73 3f71 7565 7279 3d77 6f72  ctions?query=wor
+00001dc0: 6b66 6c6f 7725 3341 2532 3245 7865 6375  kflow%3A%22Execu
+00001dd0: 7465 2b74 6573 7473 2532 3222 3e3c 696d  te+tests%22"><im
+00001de0: 6720 616c 743d 2245 7865 6375 7465 2074  g alt="Execute t
+00001df0: 6573 7473 2073 7461 7475 7322 2073 7263  ests status" src
+00001e00: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00001e10: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00001e20: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00001e30: 2f73 7461 7475 732f 4669 7a7a 6164 6172  /status/Fizzadar
+00001e40: 2f70 7969 6e66 7261 2f74 6573 742e 796d  /pyinfra/test.ym
+00001e50: 6c3f 6272 616e 6368 3d32 2e78 223e 3c2f  l?branch=2.x"></
+00001e60: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00001e70: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+00001e80: 696f 2f67 6974 6875 622f 4669 7a7a 6164  io/github/Fizzad
+00001e90: 6172 2f70 7969 6e66 7261 223e 3c69 6d67  ar/pyinfra"><img
+00001ea0: 2061 6c74 3d22 436f 6465 636f 7620 436f   alt="Codecov Co
+00001eb0: 7665 7261 6765 2220 7372 633d 2268 7474  verage" src="htt
+00001ec0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00001ed0: 2e69 6f2f 636f 6465 636f 762f 632f 6768  .io/codecov/c/gh
+00001ee0: 2f46 697a 7a61 6461 722f 7079 696e 6672  /Fizzadar/pyinfr
+00001ef0: 6122 3e3c 2f61 3e0a 2020 2020 3c61 2068  a"></a>.    <a h
+00001f00: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00001f10: 6875 622e 636f 6d2f 4669 7a7a 6164 6172  hub.com/Fizzadar
+00001f20: 2f70 7969 6e66 7261 2f62 6c6f 622f 322e  /pyinfra/blob/2.
+00001f30: 782f 4c49 4345 4e53 452e 6d64 223e 3c69  x/LICENSE.md"><i
+00001f40: 6d67 2061 6c74 3d22 4d49 5420 4c69 6365  mg alt="MIT Lice
+00001f50: 6e73 6564 2220 7372 633d 2268 7474 7073  nsed" src="https
+00001f60: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00001f70: 6f2f 7079 7069 2f6c 2f70 7969 6e66 7261  o/pypi/l/pyinfra
+00001f80: 223e 3c2f 613e 0a3c 2f70 3e0a            "></a>.</p>.
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/README.md` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 <p align="center">
     <a href="https://pyinfra.com">
         <img src="https://pyinfra.com/static/logo_readme.png" alt="pyinfra" />
     </a>
 </p>
 
 <p align="center">
+    <strong>Note: this is the v3 branch, which is currently in beta. <a href="https://docs.pyinfra.com/en/next">See the docs for v3</a>. If needed the <a href="https://github.com/pyinfra-dev/pyinfra/tree/2.x/">2.x branch is here</a>, but is in bugfix only mode.</strong>
+</p>
+
+<p align="center">
     <em>pyinfra automates infrastructure using Python. It’s fast and scales from one server to thousands. Great for ad-hoc command execution, service deployment, configuration management and more.</em>
 </p>
 
 ---
 
 <p align="center">
     <a href="https://docs.pyinfra.com"><strong>Documentation</strong></a> &rArr;
```

#### html2text {}

```diff
@@ -1,8 +1,10 @@
                                    _[_p_y_i_n_f_r_a_]
+ NNoottee:: tthhiiss iiss tthhee vv33 bbrraanncchh,, wwhhiicchh iiss ccuurrrreennttllyy iinn bbeettaa.. _SS_ee_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _ff_oo_rr_ _vv_33..
+         IIff nneeeeddeedd tthhee _22_.._xx_ _bb_rr_aa_nn_cc_hh_ _ii_ss_ _hh_ee_rr_ee,, bbuutt iiss iinn bbuuggffiixx oonnllyy mmooddee..
 ppyyiinnffrraa aauuttoommaatteess iinnffrraassttrruuccttuurree uussiinngg PPyytthhoonn.. IItt?â??ss ffaasstt aanndd ssccaalleess ffrroomm oonnee
  sseerrvveerr ttoo tthhoouussaannddss.. GGrreeaatt ffoorr aadd--hhoocc ccoommmmaanndd eexxeeccuuttiioonn,, sseerrvviiccee ddeeppllooyymmeenntt,,
                       ccoonnffiigguurraattiioonn mmaannaaggeemmeenntt aanndd mmoorree..
 ---
   _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ⇒ _GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd • _EE_xx_aa_mm_pp_ll_ee_ss • _HH_ee_ll_pp_ _&&_ _SS_uu_pp_pp_oo_rr_tt • _CC_oo_nn_tt_rr_ii_bb_uu_tt_ii_nn_gg
                            Chat ⇒ _##_pp_yy_ii_nn_ff_rr_aa_ _oo_nn_ _MM_aa_tt_rr_ii_xx
 --- Why pyinfra? Design features include: + ð **Super fast** execution over
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/__init__.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/__init__.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     RsyncCommand,
     StringCommand,
 )
 from .config import Config  # noqa: F401 # pragma: no cover
 from .deploy import deploy  # noqa: F401 # pragma: no cover
 from .exceptions import DeployError  # noqa: F401 # pragma: no cover
 from .exceptions import (  # noqa: F401
+    FactError,
+    FactTypeError,
+    FactValueError,
     InventoryError,
     OperationError,
     OperationTypeError,
     OperationValueError,
 )
 from .facts import FactBase, ShortFactBase  # noqa: F401 # pragma: no cover
 from .host import Host  # noqa: F401 # pragma: no cover
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/command.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/command.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import shlex
 from inspect import getfullargspec
 from string import Formatter
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Callable, Union
 
 import gevent
+from typing_extensions import Unpack
 
 from pyinfra.context import ctx_config, ctx_host
 
-from .arguments import get_executor_kwarg_keys
+from .arguments import ConnectorArguments
 
 if TYPE_CHECKING:
     from pyinfra.api.host import Host
     from pyinfra.api.state import State
 
 
-def make_formatted_string_command(string: str, *args, **kwargs):
+def make_formatted_string_command(string: str, *args, **kwargs) -> "StringCommand":
     """
     Helper function that takes a shell command or script as a string, splits it
     using ``shlex.split`` and then formats each bit, returning a ``StringCommand``
     instance with each bit.
 
     Useful to enable string formatted commands/scripts, for example:
 
@@ -46,183 +47,207 @@
 
 
 class MaskString(str):
     pass
 
 
 class QuoteString:
-    def __init__(self, obj):
-        self.object = obj
+    obj: Union[str, "StringCommand"]
 
-    def __repr__(self):
-        return "QuoteString({0})".format(self.object)
+    def __init__(self, obj: Union[str, "StringCommand"]):
+        self.obj = obj
+
+    def __repr__(self) -> str:
+        return f"QuoteString({self.obj})"
 
 
 class PyinfraCommand:
-    def __init__(self, *args, **kwargs):
-        self.executor_kwargs = {
-            key: kwargs[key] for key in get_executor_kwarg_keys() if key in kwargs
-        }
+    connector_arguments: ConnectorArguments
+
+    def __init__(self, **arguments: Unpack[ConnectorArguments]):
+        self.connector_arguments = arguments
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         if isinstance(other, self.__class__) and repr(self) == repr(other):
             return True
         return False
 
-    def execute(self, state: "State", host: "Host", executor_kwargs):
+    def execute(self, state: "State", host: "Host", connector_arguments: ConnectorArguments):
         raise NotImplementedError
 
 
 class StringCommand(PyinfraCommand):
-    def __init__(self, *bits, **kwargs):
-        super().__init__(**kwargs)
+    def __init__(
+        self,
+        *bits,
+        _separator=" ",
+        **arguments: Unpack[ConnectorArguments],
+    ):
+        super().__init__(**arguments)
         self.bits = bits
-        self.separator = kwargs.pop("_separator", " ")
+        self.separator = _separator
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.get_masked_value()
 
-    def __repr__(self):
-        return "StringCommand({0})".format(self.get_masked_value())
+    def __repr__(self) -> str:
+        return f"StringCommand({self.get_masked_value()})"
 
     def _get_all_bits(self, bit_accessor):
         all_bits = []
 
         for bit in self.bits:
             quote = False
             if isinstance(bit, QuoteString):
                 quote = True
-                bit = bit.object
+                bit = bit.obj
 
             if isinstance(bit, StringCommand):
                 bit = bit_accessor(bit)
 
             if not isinstance(bit, str):
                 bit = "{0}".format(bit)
 
             if quote:
                 bit = shlex.quote(bit)
 
             all_bits.append(bit)
 
         return all_bits
 
-    def get_raw_value(self):
+    def get_raw_value(self) -> str:
         return self.separator.join(
             self._get_all_bits(
                 lambda bit: bit.get_raw_value(),
             ),
         )
 
-    def get_masked_value(self):
+    def get_masked_value(self) -> str:
         return self.separator.join(
             [
                 "***" if isinstance(bit, MaskString) else bit
                 for bit in self._get_all_bits(lambda bit: bit.get_masked_value())
             ],
         )
 
-    def execute(self, state: "State", host: "Host", executor_kwargs):
-        executor_kwargs.update(self.executor_kwargs)
+    def execute(self, state: "State", host: "Host", connector_arguments: ConnectorArguments):
+        connector_arguments.update(self.connector_arguments)
 
         return host.run_shell_command(
             self,
             print_output=state.print_output,
             print_input=state.print_input,
-            return_combined_output=True,
-            **executor_kwargs,
+            **connector_arguments,
         )
 
 
 class FileUploadCommand(PyinfraCommand):
-    def __init__(self, src: str, dest: str, remote_temp_filename=None, **kwargs):
+    def __init__(
+        self,
+        src: str,
+        dest: str,
+        remote_temp_filename=None,
+        **kwargs: Unpack[ConnectorArguments],
+    ):
         super().__init__(**kwargs)
         self.src = src
         self.dest = dest
         self.remote_temp_filename = remote_temp_filename
 
     def __repr__(self):
         return "FileUploadCommand({0}, {1})".format(self.src, self.dest)
 
-    def execute(self, state: "State", host: "Host", executor_kwargs):
-        executor_kwargs.update(self.executor_kwargs)
+    def execute(self, state: "State", host: "Host", connector_arguments: ConnectorArguments):
+        connector_arguments.update(self.connector_arguments)
 
         return host.put_file(
             self.src,
             self.dest,
             remote_temp_filename=self.remote_temp_filename,
             print_output=state.print_output,
             print_input=state.print_input,
-            **executor_kwargs,
+            **connector_arguments,
         )
 
 
 class FileDownloadCommand(PyinfraCommand):
-    def __init__(self, src: str, dest: str, remote_temp_filename=None, **kwargs):
+    def __init__(
+        self,
+        src: str,
+        dest: str,
+        remote_temp_filename=None,
+        **kwargs: Unpack[ConnectorArguments],
+    ):
         super().__init__(**kwargs)
         self.src = src
         self.dest = dest
         self.remote_temp_filename = remote_temp_filename
 
     def __repr__(self):
         return "FileDownloadCommand({0}, {1})".format(self.src, self.dest)
 
-    def execute(self, state: "State", host: "Host", executor_kwargs):
-        executor_kwargs.update(self.executor_kwargs)
+    def execute(self, state: "State", host: "Host", connector_arguments: ConnectorArguments):
+        connector_arguments.update(self.connector_arguments)
 
         return host.get_file(
             self.src,
             self.dest,
             remote_temp_filename=self.remote_temp_filename,
             print_output=state.print_output,
             print_input=state.print_input,
-            **executor_kwargs,
+            **connector_arguments,
         )
 
 
 class FunctionCommand(PyinfraCommand):
-    def __init__(self, function, args, func_kwargs, **kwargs):
+    def __init__(
+        self,
+        function: Callable,
+        args,
+        func_kwargs,
+        **kwargs: Unpack[ConnectorArguments],
+    ):
         super().__init__(**kwargs)
         self.function = function
         self.args = args
         self.kwargs = func_kwargs
 
     def __repr__(self):
         return "FunctionCommand({0}, {1}, {2})".format(
             self.function.__name__,
             self.args,
             self.kwargs,
         )
 
-    def execute(self, state: "State", host: "Host", executor_kwargs):
+    def execute(self, state: "State", host: "Host", connector_arguments: ConnectorArguments):
         argspec = getfullargspec(self.function)
         if "state" in argspec.args and "host" in argspec.args:
             return self.function(state, host, *self.args, **self.kwargs)
 
         def execute_function():
             with ctx_config.use(state.config.copy()):
                 with ctx_host.use(host):
                     self.function(*self.args, **self.kwargs)
 
         greenlet = gevent.spawn(execute_function)
         return greenlet.get()
 
 
 class RsyncCommand(PyinfraCommand):
-    def __init__(self, src: str, dest: str, flags, **kwargs):
+    def __init__(self, src: str, dest: str, flags, **kwargs: Unpack[ConnectorArguments]):
         super().__init__(**kwargs)
         self.src = src
         self.dest = dest
         self.flags = flags
 
     def __repr__(self):
         return "RsyncCommand({0}, {1}, {2})".format(self.src, self.dest, self.flags)
 
-    def execute(self, state: "State", host: "Host", executor_kwargs):
+    def execute(self, state: "State", host: "Host", connector_arguments: ConnectorArguments):
         return host.rsync(
             self.src,
             self.dest,
             self.flags,
             print_output=state.print_output,
             print_input=state.print_input,
-            **executor_kwargs,
+            **connector_arguments,
         )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/config.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,80 +1,79 @@
 from os import path
+from typing import Optional
 
+# TODO: move to importlib.resources
 from pkg_resources import Requirement, ResolutionError, parse_version, require
 
 from pyinfra import __version__, state
 
 from .exceptions import PyinfraError
 
 
 class ConfigDefaults:
     # % of hosts which have to fail for all operations to stop
-    FAIL_PERCENT = None
+    FAIL_PERCENT: Optional[int] = None
     # Seconds to timeout SSH connections
-    CONNECT_TIMEOUT = 10
-    # Temporary directory (on the remote side) to use for caching any files/downloads
-    TEMP_DIR = "/tmp"
+    CONNECT_TIMEOUT: int = 10
+    # Temporary directory (on the remote side) to use for caching any files/downloads, the default
+    # None value first tries to load the hosts' temporary directory configured via "TMPDIR" env
+    # variable, falling back to DEFAULT_TEMP_DIR if not set.
+    TEMP_DIR: Optional[str] = None
+    DEFAULT_TEMP_DIR: str = "/tmp"
     # Gevent pool size (defaults to #of target hosts)
-    PARALLEL = 0
+    PARALLEL: int = 0
     # Specify the required pyinfra version (using PEP 440 setuptools specifier)
-    REQUIRE_PYINFRA_VERSION = None
+    REQUIRE_PYINFRA_VERSION: Optional[str] = None
     # Specify any required packages (either using PEP 440 or a requirements file)
     # Note: this can also include pyinfra potentially replacing REQUIRE_PYINFRA_VERSION
-    REQUIRE_PACKAGES = None
+    REQUIRE_PACKAGES: Optional[str] = None
     # All these can be overridden inside individual operation calls:
     # Switch to this user (from ssh_user) using su before executing operations
-    SU_USER = None
-    USE_SU_LOGIN = False
-    SU_SHELL = None
-    PRESERVE_SU_ENV = False
+    SU_USER: Optional[str] = None
+    USE_SU_LOGIN: bool = False
+    SU_SHELL: bool = False
+    PRESERVE_SU_ENV: bool = False
     # Use sudo and optional user
-    SUDO = False
-    SUDO_USER = None
-    PRESERVE_SUDO_ENV = False
-    USE_SUDO_LOGIN = False
-    USE_SUDO_PASSWORD = False
+    SUDO: bool = False
+    SUDO_USER: Optional[str] = None
+    PRESERVE_SUDO_ENV: bool = False
+    USE_SUDO_LOGIN: bool = False
+    SUDO_PASSWORD: Optional[str] = None
     # Use doas and optional user
-    DOAS = False
-    DOAS_USER = None
+    DOAS: bool = False
+    DOAS_USER: Optional[str] = None
     # Only show errors but don't count as failure
-    IGNORE_ERRORS = False
+    IGNORE_ERRORS: bool = False
     # Shell to use to execute commands
-    SHELL = "sh"
+    SHELL: str = "sh"
 
 
 config_defaults = {key: value for key, value in ConfigDefaults.__dict__.items() if key.isupper()}
 
 
 def check_pyinfra_version(version: str):
     if not version:
         return
-
     running_version = parse_version(__version__)
-    required_versions = Requirement.parse(
-        "pyinfra{0}".format(version),
-    )
+    required_versions = Requirement.parse("pyinfra{0}".format(version))
 
-    if running_version not in required_versions:
+    if running_version not in required_versions:  # type: ignore[operator]
         raise PyinfraError(
-            ("pyinfra version requirement not met " "(requires {0}, running {1})").format(
-                version,
-                __version__,
-            ),
+            f"pyinfra version requirement not met (requires {version}, running {__version__})"
         )
 
 
 def check_require_packages(requirements_config):
     if not requirements_config:
         return
 
     if isinstance(requirements_config, (list, tuple)):
         requirements = requirements_config
     else:
-        with open(path.join(state.cwd, requirements_config), encoding="utf-8") as f:
+        with open(path.join(state.cwd or "", requirements_config), encoding="utf-8") as f:
             requirements = [line.split("#egg=")[-1] for line in f.read().splitlines()]
 
     try:
         require(requirements)
     except ResolutionError as e:
         raise PyinfraError(
             "Deploy requirements ({0}) not met: {1}".format(
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/connect.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     # Get/set the results
     failed_hosts = set()
 
     for greenlet, host in greenlet_to_host.items():
         # Raise any unexpected exception
         greenlet.get()
 
-        if host.connection:
+        if host.connected:
             state.activate_host(host)
         else:
             failed_hosts.add(host)
 
     # Remove those that failed, triggering FAIL_PERCENT check
     state.fail_hosts(failed_hosts, activated_count=len(hosts))
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/connectors.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/connectors.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,24 @@
 import pkg_resources
 
 
-class BaseConnectorMeta:
-    handles_execution = False
-    keys_prefix = ""
-
-    class DataKeys:
-        pass
-
-    @classmethod
-    def keys(cls):
-        class Keys:
-            pass
-
-        for key in cls.DataKeys.__dict__:
-            if not key.startswith("_"):
-                setattr(Keys, key, f"{cls.keys_prefix}_{key}")
-
-        return Keys
-
-
 def _load_connector(entrypoint):
-    connector = entrypoint.load()
-    if not getattr(connector, "Meta", None):
-        connector.Meta = BaseConnectorMeta
-    return connector
+    return entrypoint.load()
 
 
 def get_all_connectors():
     return {
         entrypoint.name: _load_connector(entrypoint)
         for entrypoint in pkg_resources.iter_entry_points("pyinfra.connectors")
     }
 
 
 def get_execution_connectors():
     return {
         connector: connector_mod
         for connector, connector_mod in get_all_connectors().items()
-        if connector_mod.Meta.handles_execution
+        if connector_mod.handles_execution
     }
 
 
 def get_execution_connector(name):
     return get_execution_connectors()[name]
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/exceptions.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,33 @@
 
 class ConnectError(PyinfraError):
     """
     Exception raised when connecting fails.
     """
 
 
+class FactError(PyinfraError):
+    """
+    Exception raised during fact gathering staging if a fact is unable to
+    generate output/change state.
+    """
+
+
+class FactTypeError(FactError, TypeError):
+    """
+    Exception raised when a fact is passed invalid argument types.
+    """
+
+
+class FactValueError(FactError, ValueError):
+    """
+    Exception raised when a fact is passed invalid argument values.
+    """
+
+
 class OperationError(PyinfraError):
     """
     Exception raised during fact gathering staging if an operation is unable to
     generate output/change state.
     """
 
 
@@ -37,23 +56,35 @@
 
 class InventoryError(PyinfraError):
     """
     Exception raised for inventory related errors.
     """
 
 
-class NoConnectorError(PyinfraError, TypeError):
+class NoConnectorError(PyinfraError, ValueError):
     """
     Raised when a requested connector is missing.
     """
 
 
-class NoHostError(PyinfraError, TypeError):
+class NoHostError(PyinfraError, KeyError):
     """
     Raised when an inventory is missing a host.
     """
 
 
-class NoGroupError(PyinfraError, TypeError):
+class NoGroupError(PyinfraError, KeyError):
+    """
+    Raised when an inventory is missing a group.
+    """
+
+
+class ConnectorDataTypeError(PyinfraError, TypeError):
+    """
+    Raised when host connector data has invalid types.
+    """
+
+
+class ArgumentTypeError(PyinfraError, TypeError):
     """
-    Raise when an inventory is missing a group.
+    Raised when global arguments are passed with invalid types.
     """
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/facts.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/facts.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,31 @@
 for a deploy.
 
 Note that the facts API does *not* use the global currently in context host so
 it's possible to call facts on hosts out of context (ie give me the IP of this
 other host B while I operate on this host A).
 """
 
+from __future__ import annotations
+
 import re
 from inspect import getcallargs
 from socket import error as socket_error, timeout as timeout_error
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Type, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Generic,
+    Iterable,
+    Optional,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import click
 import gevent
 from paramiko import SSHException
 
 from pyinfra import logger
 from pyinfra.api import StringCommand
@@ -23,66 +36,75 @@
 from pyinfra.api.util import (
     get_kwargs_str,
     log_error_or_warning,
     log_host_command_error,
     make_hash,
     print_host_combined_output,
 )
-from pyinfra.connectors.util import split_combined_output
+from pyinfra.connectors.util import CommandOutput
 from pyinfra.context import ctx_host, ctx_state
 from pyinfra.progress import progress_spinner
 
-from .arguments import get_executor_kwarg_keys
+from .arguments import CONNECTOR_ARGUMENT_KEYS
 
 if TYPE_CHECKING:
     from pyinfra.api.host import Host
     from pyinfra.api.state import State
 
-SUDO_REGEX = r"^sudo: unknown user:"
+SUDO_REGEX = r"^sudo: unknown user"
 SU_REGEXES = (
     r"^su: user .+ does not exist",
     r"^su: unknown login",
 )
 
 
-class FactNameMeta(type):
-    def __init__(cls, name: str, bases, attrs, **kwargs):
-        super().__init__(name, bases, attrs, **kwargs)
-        module_name = cls.__module__.replace("pyinfra.facts.", "")
-        cls.name = f"{module_name}.{cls.__name__}"
+T = TypeVar("T")
 
 
-class FactBase(metaclass=FactNameMeta):
+class FactBase(Generic[T]):
     name: str
 
     abstract: bool = True
 
     shell_executable: Optional[str] = None
 
     requires_command: Optional[str] = None
 
     command: Union[str, Callable]
 
+    def __init_subclass__(cls) -> None:
+        super().__init_subclass__()
+        module_name = cls.__module__.replace("pyinfra.facts.", "")
+        cls.name = f"{module_name}.{cls.__name__}"
+
     @staticmethod
-    def default():
+    def default() -> T:
         """
         Set the default attribute to be a type (eg list/dict).
         """
 
-    @staticmethod
-    def process(output):
-        return "\n".join(output)
+        return cast(T, None)
+
+    def process(self, output: Iterable[str]) -> T:
+        # NOTE: TypeVar does not support a default, so we have to cast this str -> T
+        return cast(T, "\n".join(output))
 
     def process_pipeline(self, args, output):
         return {arg: self.process([output[i]]) for i, arg in enumerate(args)}
 
 
-class ShortFactBase(metaclass=FactNameMeta):
+class ShortFactBase(Generic[T]):
+    name: str
     fact: Type[FactBase]
 
+    def __init_subclass__(cls) -> None:
+        super().__init_subclass__()
+        module_name = cls.__module__.replace("pyinfra.facts.", "")
+        cls.name = f"{module_name}.{cls.__name__}"
+
     @staticmethod
     def process_data(data):
         return data
 
 
 def get_short_facts(state: "State", host: "Host", short_fact, **kwargs):
     fact_data = get_fact(state, host, short_fact.fact, **kwargs)
@@ -95,35 +117,33 @@
         return command_attribute(**host_args)
     return command_attribute
 
 
 def _get_executor_kwargs(
     state: "State",
     host: "Host",
-    override_kwargs: Optional[Dict[str, Any]] = None,
-    override_kwarg_keys: Optional[List[str]] = None,
+    override_kwargs: Optional[dict[str, Any]] = None,
+    override_kwarg_keys: Optional[list[str]] = None,
 ):
     if override_kwargs is None:
         override_kwargs = {}
     if override_kwarg_keys is None:
         override_kwarg_keys = []
 
     # Use the current operation global kwargs, or generate defaults
-    global_kwargs = host.current_op_global_kwargs
+    global_kwargs = host.current_op_global_arguments
     if not global_kwargs:
         global_kwargs, _ = pop_global_arguments({}, state, host)
 
     # Apply any current op kwargs that *weren't* found in the overrides
     override_kwargs.update(
         {key: value for key, value in global_kwargs.items() if key not in override_kwarg_keys},
     )
 
-    return {
-        key: value for key, value in override_kwargs.items() if key in get_executor_kwarg_keys()
-    }
+    return {key: value for key, value in override_kwargs.items() if key in CONNECTOR_ARGUMENT_KEYS}
 
 
 def _handle_fact_kwargs(state, host, cls, args, kwargs):
     args = args or []
     kwargs = kwargs or {}
 
     # TODO: this is here to avoid popping stuff accidentally, this is horrible! Change the
@@ -132,21 +152,21 @@
 
     # Get the defaults *and* overrides by popping from kwargs, executor kwargs passed
     # into get_fact override everything else (applied below).
     override_kwargs, override_kwarg_keys = pop_global_arguments(
         kwargs,
         state=state,
         host=host,
-        keys_to_check=get_executor_kwarg_keys(),
+        keys_to_check=CONNECTOR_ARGUMENT_KEYS,
     )
 
     executor_kwargs = _get_executor_kwargs(
         state,
         host,
-        override_kwargs=override_kwargs,
+        override_kwargs=override_kwargs,  # type: ignore[arg-type]
         override_kwarg_keys=override_kwarg_keys,
     )
 
     fact_kwargs = {}
 
     if args or kwargs:
         assert not isinstance(cls.command, str)
@@ -177,61 +197,51 @@
 
     return results
 
 
 def get_fact(
     state: "State",
     host: "Host",
-    cls: Type[FactBase],
+    cls: type[FactBase],
     args: Optional[Any] = None,
     kwargs: Optional[Any] = None,
     ensure_hosts: Optional[Any] = None,
     apply_failed_hosts: bool = True,
-    fact_hash: Optional[Any] = None,
-    use_cache: bool = True,
-):
+) -> Any:
     if issubclass(cls, ShortFactBase):
         return get_short_facts(
             state,
             host,
             cls,
             args=args,
             kwargs=kwargs,
             ensure_hosts=ensure_hosts,
             apply_failed_hosts=apply_failed_hosts,
-            fact_hash=fact_hash,
-            use_cache=use_cache,
         )
 
-    with host.facts_lock:
-        if use_cache and fact_hash and fact_hash in host.facts:
-            return host.facts[fact_hash]
-
-        return _get_fact(
-            state,
-            host,
-            cls,
-            args,
-            kwargs,
-            ensure_hosts,
-            apply_failed_hosts,
-            fact_hash,
-        )
+    return _get_fact(
+        state,
+        host,
+        cls,
+        args,
+        kwargs,
+        ensure_hosts,
+        apply_failed_hosts,
+    )
 
 
 def _get_fact(
     state: "State",
     host: "Host",
-    cls: Type[FactBase],
-    args: Optional[List] = None,
-    kwargs: Optional[Dict] = None,
+    cls: type[FactBase],
+    args: Optional[list] = None,
+    kwargs: Optional[dict] = None,
     ensure_hosts: Optional[Any] = None,
     apply_failed_hosts: bool = True,
-    fact_hash: Optional[Any] = None,
-):
+) -> Any:
     fact = cls()
     name = fact.name
 
     fact_kwargs, executor_kwargs = _handle_fact_kwargs(state, host, cls, args, kwargs)
 
     kwargs_str = get_kwargs_str(fact_kwargs)
     logger.debug(
@@ -243,22 +253,23 @@
 
     if not host.connected:
         host.connect(
             reason=f"to load fact: {name} ({kwargs_str})",
             raise_exceptions=True,
         )
 
-    ignore_errors = (host.current_op_global_kwargs or {}).get(
-        "ignore_errors",
-        state.config.IGNORE_ERRORS,
+    ignore_errors = (
+        host.current_op_global_arguments["_ignore_errors"]
+        if host.in_op and host.current_op_global_arguments
+        else state.config.IGNORE_ERRORS
     )
 
     # Facts can override the shell (winrm powershell vs cmd support)
     if fact.shell_executable:
-        executor_kwargs["shell_executable"] = fact.shell_executable
+        executor_kwargs["_shell_executable"] = fact.shell_executable
 
     command = _make_command(fact.command, fact_kwargs)
     requires_command = _make_command(fact.requires_command, fact_kwargs)
     if requires_command:
         command = StringCommand(
             # Command doesn't exist, return 0 *or* run & return fact command
             "!",
@@ -267,48 +278,46 @@
             requires_command,
             ">/dev/null",
             "||",
             command,
         )
 
     status = False
-    stdout = []
-    combined_output_lines = []
+    output = CommandOutput([])
 
     try:
-        status, combined_output_lines = host.run_shell_command(
+        status, output = host.run_shell_command(
             command,
             print_output=state.print_fact_output,
             print_input=state.print_fact_input,
-            return_combined_output=True,
             **executor_kwargs,
         )
     except (timeout_error, socket_error, SSHException) as e:
         log_host_command_error(
             host,
             e,
-            timeout=executor_kwargs["timeout"],
+            timeout=executor_kwargs["_timeout"],
         )
 
-    stdout, stderr = split_combined_output(combined_output_lines)
+    stdout_lines, stderr_lines = output.stdout_lines, output.stderr_lines
 
     data = fact.default()
 
     if status:
-        if stdout:
-            data = fact.process(stdout)
-    elif stderr:
+        if stdout_lines:
+            data = fact.process(stdout_lines)
+    elif stderr_lines:
         # If we have error output and that error is sudo or su stating the user
         # does not exist, do not fail but instead return the default fact value.
         # This allows for users that don't currently but may be created during
         # other operations.
-        first_line = stderr[0]
-        if executor_kwargs["sudo_user"] and re.match(SUDO_REGEX, first_line):
+        first_line = stderr_lines[0]
+        if executor_kwargs["_sudo_user"] and re.match(SUDO_REGEX, first_line):
             status = True
-        if executor_kwargs["su_user"] and any(re.match(regex, first_line) for regex in SU_REGEXES):
+        if executor_kwargs["_su_user"] and any(re.match(regex, first_line) for regex in SU_REGEXES):
             status = True
 
     if status:
         log_message = "{0}{1}".format(
             host.print_prefix,
             "Loaded fact {0}{1}".format(
                 click.style(name, bold=True),
@@ -317,82 +326,37 @@
         )
         if state.print_fact_info:
             logger.info(log_message)
         else:
             logger.debug(log_message)
     else:
         if not state.print_fact_output:
-            print_host_combined_output(host, combined_output_lines)
+            print_host_combined_output(host, output)
 
         log_error_or_warning(
             host,
             ignore_errors,
             description=("could not load fact: {0} {1}").format(name, get_kwargs_str(fact_kwargs)),
         )
 
     # Check we've not failed
     if not status and not ignore_errors and apply_failed_hosts:
         state.fail_hosts({host})
 
-    if fact_hash:
-        host.facts[fact_hash] = data
     return data
 
 
 def _get_fact_hash(state: "State", host: "Host", cls, args, kwargs):
     if issubclass(cls, ShortFactBase):
         cls = cls.fact
     fact_kwargs, executor_kwargs = _handle_fact_kwargs(state, host, cls, args, kwargs)
     return make_hash((cls, fact_kwargs, executor_kwargs))
 
 
 def get_host_fact(
     state: "State",
     host: "Host",
     cls,
-    args: Optional[List] = None,
-    kwargs: Optional[Dict] = None,
-):
-    fact_hash = _get_fact_hash(state, host, cls, args, kwargs)
-    return get_fact(state, host, cls, args=args, kwargs=kwargs, fact_hash=fact_hash)
-
-
-def reload_host_fact(
-    state: "State",
-    host: "Host",
-    cls,
-    args: Optional[List] = None,
-    kwargs: Optional[Dict] = None,
-):
-    fact_hash = _get_fact_hash(state, host, cls, args, kwargs)
-    return get_fact(
-        state,
-        host,
-        cls,
-        args=args,
-        kwargs=kwargs,
-        fact_hash=fact_hash,
-        use_cache=False,
-    )
-
-
-def create_host_fact(
-    state: "State",
-    host: "Host",
-    cls,
-    data,
-    args: Optional[List] = None,
-    kwargs: Optional[Dict] = None,
-):
-    fact_hash = _get_fact_hash(state, host, cls, args, kwargs)
-    host.facts[fact_hash] = data
-
-
-def delete_host_fact(
-    state: "State",
-    host: "Host",
-    cls,
-    args: Optional[List] = None,
-    kwargs: Optional[Dict] = None,
-):
-    fact_hash = _get_fact_hash(state, host, cls, args, kwargs)
-    host.facts.pop(fact_hash, None)
+    args: Optional[Iterable] = None,
+    kwargs: Optional[dict] = None,
+) -> Any:
+    return get_fact(state, host, cls, args=args, kwargs=kwargs)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/host.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/host.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,58 @@
+from __future__ import annotations
+
 from contextlib import contextmanager
-from typing import TYPE_CHECKING, Any, Callable, Dict, Generator, List, Optional, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Generator,
+    Optional,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+    overload,
+)
+from uuid import uuid4
 
 import click
-from gevent.lock import BoundedSemaphore
+from typing_extensions import Unpack
 
 from pyinfra import logger
-from pyinfra.connectors.util import remove_any_sudo_askpass_file
+from pyinfra.connectors.base import BaseConnector
+from pyinfra.connectors.util import CommandOutput, remove_any_sudo_askpass_file
 
 from .connectors import get_execution_connector
 from .exceptions import ConnectError
-from .facts import create_host_fact, delete_host_fact, get_host_fact, reload_host_fact
+from .facts import FactBase, ShortFactBase, get_host_fact
+from .util import memoize, sha1_hash
 
 if TYPE_CHECKING:
+    from pyinfra.api.arguments import AllArguments
     from pyinfra.api.inventory import Inventory
     from pyinfra.api.state import State
 
 
-def extract_callable_datas(datas: List[Union[Callable[..., Any], Any]]) -> Generator[Any, Any, Any]:
+def extract_callable_datas(datas: list[Union[Callable[..., Any], Any]]) -> Generator[Any, Any, Any]:
     for data in datas:
         # Support for dynamic data, ie @deploy wrapped data defaults where
         # the data is stored on the state temporarily.
         if callable(data):
             data = data()
 
         yield data
 
 
 class HostData:
     """
     Combines multiple AttrData's to search for attributes.
     """
 
-    override_datas: Dict[str, Any]
+    override_datas: dict[str, Any]
 
     def __init__(self, host: "Host", *datas):
         self.__dict__["host"] = host
 
         parsed_datas = list(datas)
 
         # Inject an empty override data so we can assign during deploy
@@ -78,135 +95,162 @@
 
 class Host:
     """
     Represents a target host. Thin class that links up to facts and host/group
     data.
     """
 
-    connection = None
     state: "State"
+    connector_cls: type[BaseConnector]
+    connector: BaseConnector
+    connected: bool = False
 
     # Current context inside an @operation function (op gen stage)
     in_op: bool = False
+    in_callback_op: bool = False
     current_op_hash: Optional[str] = None
-    current_op_global_kwargs: Dict[str, Any]
+    current_op_global_arguments: Optional["AllArguments"] = None
 
     # Current context inside a @deploy function (op gen stage)
     in_deploy: bool = False
     current_deploy_name: Optional[str] = None
     current_deploy_kwargs = None
     current_deploy_data = None
 
     # Current context during operation execution
-    executing_op_hash = None
-    nested_executing_op_hash = None
+    executing_op_hash: Optional[str] = None
+    nested_executing_op_hash: Optional[str] = None
 
-    loop_position: List[int]
+    loop_position: list[int]
 
     # Arbitrary data dictionary connectors may use
-    connector_data: Dict[str, Any]
+    connector_data: dict[str, Any]
 
     def loop(self, iterable):
         self.loop_position.append(0)
         for i, item in enumerate(iterable):
             self.loop_position[-1] = i
             yield item
         self.loop_position.pop()
 
     def __init__(
         self,
         name: str,
         inventory: "Inventory",
         groups,
-        executor=get_execution_connector("ssh"),
+        connector_cls=get_execution_connector("ssh"),
     ):
         self.inventory = inventory
         self.groups = groups
-        self.executor = executor
+        self.connector_cls = connector_cls
         self.name = name
 
         self.loop_position = []
 
         self.connector_data = {}
-        self.current_op_global_kwargs = {}
-
-        # Fact data store
-        # TODO: how to not have Any here?
-        self.facts: Dict[str, Any] = {}
-        self.facts_lock = BoundedSemaphore()
 
         # Append only list of operation hashes as called on this host, used to
         # generate a DAG to create the final operation order.
-        self.op_hash_order: List[str] = []
+        self.op_hash_order: list[str] = []
 
         # Create the (waterfall data: override, host, group, global)
         self.data = HostData(
             self,
             lambda: inventory.get_override_data(),
             lambda: inventory.get_host_data(name),
             lambda: inventory.get_groups_data(groups),
             lambda: inventory.get_data(),
             # @deploy function data are default values, so come last
             self.get_deploy_data,
         )
 
+    def init(self, state: "State") -> None:
+        self.state = state
+        self.connector = self.connector_cls(state, self)
+
+        longest_name_len = max([len(host.name) for host in self.inventory])
+        padding_diff = longest_name_len - len(self.name)
+        self.print_prefix_padding = "".join(" " for _ in range(0, padding_diff))
+
     def __str__(self):
         return "{0}".format(self.name)
 
     def __repr__(self):
         return "Host({0})".format(self.name)
 
     @property
-    def connected(self) -> bool:
-        return self.connection is not None
-
-    @property
     def host_data(self):
         return self.inventory.get_host_data(self.name)
 
     @property
     def group_data(self):
         return self.inventory.get_groups_data(self.groups)
 
     @property
-    def print_prefix(self):
+    def print_prefix(self) -> str:
         if self.nested_executing_op_hash:
-            return "{0}[{1}] {2} ".format(
+            return "{0}[{1}] {2}{3} ".format(
                 click.style(""),  # reset
                 click.style(self.name, bold=True),
                 click.style("nested", "blue"),
+                self.print_prefix_padding,
             )
 
-        return "{0}[{1}] ".format(
+        return "{0}[{1}]{2} ".format(
             click.style(""),  # reset
             click.style(self.name, bold=True),
+            self.print_prefix_padding,
         )
 
-    def style_print_prefix(self, *args, **kwargs):
-        return "{0}[{1}] ".format(
+    def style_print_prefix(self, *args, **kwargs) -> str:
+        return "{0}[{1}]{2} ".format(
             click.style(""),  # reset
             click.style(self.name, *args, **kwargs),
+            self.print_prefix_padding,
         )
 
+    def log(self, message, log_func=logger.info):
+        log_func(f"{self.print_prefix}{message}")
+
+    def log_styled(self, message, log_func=logger.info, **kwargs):
+        message_styled = click.style(message, **kwargs)
+        self.log(message_styled, log_func=log_func)
+
     def get_deploy_data(self):
         if self.current_deploy_data:
             return self.current_deploy_data
-
         return {}
 
     def noop(self, description):
         """
         Log a description for a noop operation.
         """
 
         handler = logger.info if self.state.print_noop_info else logger.debug
         handler("{0}noop: {1}".format(self.print_prefix, description))
 
+    def when(self, condition: Callable[[], bool]):
+        return self.deploy(
+            "",
+            cast("AllArguments", {"_if": [condition]}),
+            {},
+            in_deploy=False,
+        )
+
+    def arguments(self, **arguments: Unpack["AllArguments"]):
+        return self.deploy("", arguments, {}, in_deploy=False)
+
     @contextmanager
-    def deploy(self, name: str, kwargs, data, in_deploy: bool = True):
+    def deploy(
+        self,
+        name: str,
+        kwargs: Optional["AllArguments"],
+        data: Optional[dict],
+        in_deploy: bool = True,
+    ):
         """
         Wraps a group of operations as a deploy, this should not be used
         directly, instead use ``pyinfra.api.deploy.deploy``.
         """
 
         # Handle nested deploy names
         if self.current_deploy_name:
@@ -215,14 +259,21 @@
         # Store the previous values
         old_in_deploy = self.in_deploy
         old_deploy_name = self.current_deploy_name
         old_deploy_kwargs = self.current_deploy_kwargs
         old_deploy_data = self.current_deploy_data
         self.in_deploy = in_deploy
 
+        # Combine any old _ifs with the new ones
+        if old_deploy_kwargs and kwargs:
+            old_ifs = old_deploy_kwargs["_if"]
+            new_ifs = kwargs["_if"]
+            if old_ifs and new_ifs:
+                kwargs["_if"] = old_ifs + new_ifs
+
         # Set the new values
         self.current_deploy_name = name
         self.current_deploy_kwargs = kwargs
         self.current_deploy_data = data
         logger.debug(
             "Starting deploy %s (args=%r, data=%r)",
             name,
@@ -241,60 +292,82 @@
         logger.debug(
             "Reset deploy to %s (args=%r, data=%r)",
             old_deploy_name,
             old_deploy_kwargs,
             old_deploy_data,
         )
 
-    # Host facts
-    #
+    @memoize
+    def _get_temp_directory(self):
+        temp_directory = self.state.config.TEMP_DIR
 
-    def get_fact(self, name_or_cls, *args, **kwargs):
-        """
-        Get a fact for this host, reading from the cache if present.
-        """
-        return get_host_fact(self.state, self, name_or_cls, args=args, kwargs=kwargs)
+        if temp_directory is None:
+            # Unfortunate, but very hard to avoid, circular dependency, this method is memoized so
+            # performance isn't a concern.
+            from pyinfra.facts.server import TmpDir
 
-    def reload_fact(self, name_or_cls, *args, **kwargs):
-        """
-        Get a fact for this host without using any cached value, always re-fetch the fact data
-        from the host and then cache it.
-        """
-        return reload_host_fact(self.state, self, name_or_cls, args=args, kwargs=kwargs)
+            temp_directory = self.get_fact(TmpDir)
+
+        if not temp_directory:
+            temp_directory = self.state.config.DEFAULT_TEMP_DIR
+
+        return temp_directory
 
-    def create_fact(self, name_or_cls, data=None, kwargs=None):
+    def get_temp_filename(self, hash_key: Optional[str] = None, hash_filename: bool = True):
         """
-        Create a new fact for this host in the fact cache.
+        Generate a temporary filename for this deploy.
         """
-        return create_host_fact(self.state, self, name_or_cls, data, kwargs=kwargs)
 
-    def delete_fact(self, name_or_cls, kwargs=None):
+        temp_directory = self._get_temp_directory()
+
+        if not hash_key:
+            hash_key = str(uuid4())
+
+        if hash_filename:
+            hash_key = sha1_hash(hash_key)
+
+        return "{0}/pyinfra-{1}".format(temp_directory, hash_key)
+
+    # Host facts
+    #
+
+    T = TypeVar("T")
+
+    @overload
+    def get_fact(self, name_or_cls: Type[FactBase[T]], *args, **kwargs) -> T:
+        ...
+
+    @overload
+    def get_fact(self, name_or_cls: Type[ShortFactBase[T]], *args, **kwargs) -> T:
+        ...
+
+    def get_fact(self, name_or_cls, *args, **kwargs):
         """
-        Remove an existing fact for this host in the fact cache.
+        Get a fact for this host, reading from the cache if present.
         """
-        return delete_host_fact(self.state, self, name_or_cls, kwargs=kwargs)
+        return get_host_fact(self.state, self, name_or_cls, args=args, kwargs=kwargs)
 
     # Connector proxy
     #
 
     def _check_state(self):
         if not self.state:
             raise TypeError("Cannot call this function with no state!")
 
     def connect(self, reason=None, show_errors: bool = True, raise_exceptions: bool = False):
         """
         Connect to the host using it's configured connector.
         """
 
         self._check_state()
-        if not self.connection:
+        if not self.connected:
             self.state.trigger_callbacks("host_before_connect", self)
 
             try:
-                self.connection = self.executor.connect(self.state, self)
+                self.connector.connect()
             except ConnectError as e:
                 if show_errors:
                     log_message = "{0}{1}".format(
                         self.print_prefix,
                         click.style(e.args[0], "red"),
                     )
                     logger.error(log_message)
@@ -312,63 +385,55 @@
                     log_message = "{0}{1}".format(
                         log_message,
                         " ({0})".format(reason),
                     )
 
                 logger.info(log_message)
                 self.state.trigger_callbacks("host_connect", self)
-
-        return self.connection
+                self.connected = True
 
     def disconnect(self):
         """
         Disconnect from the host using it's configured connector.
         """
         self._check_state()
 
-        # Disconnect is an optional function for executors if needed
-        disconnect_func = getattr(self.executor, "disconnect", None)
+        # Disconnect is an optional function for connectors if needed
+        disconnect_func = getattr(self.connector, "disconnect", None)
         if disconnect_func:
-            return disconnect_func(self.state, self)
+            return disconnect_func()
 
         # TODO: consider whether this should be here!
         remove_any_sudo_askpass_file(self)
 
         self.state.trigger_callbacks("host_disconnect", self)
 
-    def run_shell_command(self, *args, **kwargs):
+    def run_shell_command(self, *args, **kwargs) -> tuple[bool, CommandOutput]:
         """
         Low level method to execute a shell command on the host via it's configured connector.
         """
         self._check_state()
-        return self.executor.run_shell_command(self.state, self, *args, **kwargs)
+        return self.connector.run_shell_command(*args, **kwargs)
 
-    def put_file(self, *args, **kwargs):
+    def put_file(self, *args, **kwargs) -> bool:
         """
         Low level method to upload a file to the host via it's configured connector.
         """
         self._check_state()
-        return self.executor.put_file(self.state, self, *args, **kwargs)
+        return self.connector.put_file(*args, **kwargs)
 
-    def get_file(self, *args, **kwargs):
+    def get_file(self, *args, **kwargs) -> bool:
         """
         Low level method to download a file from the host via it's configured connector.
         """
         self._check_state()
-        return self.executor.get_file(self.state, self, *args, **kwargs)
+        return self.connector.get_file(*args, **kwargs)
 
-    # Rsync - optional executor specific ability
+    # Rsync - optional connector specific ability
 
-    def check_can_rsync(self):
-        check_can_rsync_func = getattr(self.executor, "check_can_rsync", None)
-        if check_can_rsync_func:
-            return check_can_rsync_func(self)
-
-        raise NotImplementedError(
-            "The {0} connector does not support rsync!".format(
-                self.executor.__name__,
-            ),
-        )
+    def check_can_rsync(self) -> None:
+        self._check_state()
+        return self.connector.check_can_rsync()
 
-    def rsync(self, *args, **kwargs):
+    def rsync(self, *args, **kwargs) -> bool:
         self._check_state()
-        return self.executor.rsync(self.state, self, *args, **kwargs)
+        return self.connector.rsync(*args, **kwargs)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/inventory.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/inventory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from __future__ import annotations
+
 from collections import defaultdict
-from typing import TYPE_CHECKING, Any, Iterator, List
+from typing import TYPE_CHECKING, Any, Iterator
 
 from .connectors import get_all_connectors, get_execution_connectors
 from .exceptions import NoConnectorError, NoGroupError, NoHostError
 from .host import Host
 
 if TYPE_CHECKING:
     from pyinfra.api.state import State
 
 
-def extract_name_data(names: List[Any]):
+def extract_name_data(names: list[Any]):
     for name in names:
         data = {}
 
         if isinstance(name, tuple):
             data = name[1]
             name = name[0]
 
@@ -34,32 +36,32 @@
     """
 
     state: "State"
 
     def __init__(self, names_data, override_data=None, **groups):
         # Setup basics
         self.groups = defaultdict(list)  # lists of Host objects
-        self.host_data = defaultdict(dict)  # dict of name -> data
-        self.group_data = defaultdict(dict)  # dict of name -> data
+        self.host_data: dict[str, dict] = defaultdict(dict)  # dict of name -> data
+        self.group_data: dict[str, dict] = defaultdict(dict)  # dict of name -> data
         self.override_data = override_data or {}
 
         names, data = names_data
 
         # Assign global data
         self.data = data
 
         # Create the actual host instances and groups
-        self.hosts = self.make_hosts_and_groups(names, groups)
+        self.make_hosts_and_groups(names, groups)
 
-    def make_hosts_and_groups(self, names, groups):
+    def make_hosts_and_groups(self, names, groups) -> None:
         all_connectors = get_all_connectors()
         execution_connectors = get_execution_connectors()
 
         # Map name -> data
-        name_to_data = defaultdict(dict)
+        name_to_data: dict[str, dict] = defaultdict(dict)
         # Map name -> group names
         name_to_group_names = defaultdict(list)
 
         for group_name, (group_names, group_data) in groups.items():
             # Assign group data
             self.group_data[group_name] = group_data
 
@@ -69,22 +71,22 @@
                 name_to_group_names[name].append(group_name)
 
         # Build all/top-level host data - *before* we expand any inventory
         # connectors.
         for name, data in extract_name_data(names):
             name_to_data[name].update(data)
 
-        # Now, use the above to fill self.host_data and populate names_executors
-        names_executors = []
+        # Now, use the above to fill self.host_data and populate names_connectors
+        names_connectors = []
 
         for name, _ in extract_name_data(names):
             host_data = name_to_data[name]
 
             # Default to executing commands with the ssh connector
-            executor = execution_connectors["ssh"]
+            connector_cls = execution_connectors["ssh"]
 
             if name[0] == "@":
                 connector_name = name[1:]
                 arg_string = None
 
                 if "/" in connector_name:
                     connector_name, arg_string = connector_name.split("/", 1)
@@ -92,54 +94,54 @@
                 if connector_name not in get_all_connectors():
                     raise NoConnectorError(
                         "Invalid connector: {0}".format(connector_name),
                     )
 
                 # Execution connector? Simple, just set it for their host
                 if connector_name in execution_connectors:
-                    executor = execution_connectors[connector_name]
+                    connector_cls = execution_connectors[connector_name]
 
                 names_data = all_connectors[connector_name].make_names_data(arg_string)
                 connector_inventory_name = name
             else:
                 names_data = [(name, {}, [])]
                 connector_inventory_name = None
 
             for sub_name, sub_data, sub_groups in names_data:
                 # Update any connector data with a copy of the host data (so that
                 # host data can override connector data).
                 sub_data.update(host_data.copy())
 
                 # Assign the name/data/groups from the connector
                 self.host_data[sub_name] = sub_data
-                names_executors.append((sub_name, executor))
+                names_connectors.append((sub_name, connector_cls))
                 name_to_group_names[sub_name].extend(sub_groups)
 
                 # If we have a connector inventory name, copy any groups attached
                 # to the newly generated host name.
                 if connector_inventory_name:
                     name_to_group_names[sub_name].extend(
                         name_to_group_names[connector_inventory_name],
                     )
 
         # Now we can actually make Host instances
         hosts: dict[str, "Host"] = {}
 
-        for name, executor in names_executors:
+        for name, connector_cls in names_connectors:
             host_groups = name_to_group_names[name]
 
-            host = Host(name, inventory=self, groups=host_groups, executor=executor)
+            host = Host(name, inventory=self, groups=host_groups, connector_cls=connector_cls)
             hosts[name] = host
 
             # And push into any groups
             for group_name in host_groups:
                 if host not in self.groups[group_name]:
                     self.groups[group_name].append(host)
 
-        return hosts
+        self.hosts = hosts
 
     def __len__(self) -> int:
         """
         Returns the number of inventory hosts.
         """
 
         return len(self.hosts)
@@ -237,17 +239,7 @@
 
         data = {}
 
         for group in groups:
             data.update(self.get_group_data(group))
 
         return data
-
-    def get_deploy_data(self):
-        """
-        Gets any default data attached to the current deploy, if any.
-        """
-
-        if self.state and self.state.deploy_data:
-            return self.state.deploy_data
-
-        return {}
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/operation.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/operation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,151 @@
 """
 Operations are the core of pyinfra. The ``@operation`` wrapper intercepts calls
 to the function and instead diff against the remote server, outputting commands
 to the deploy state. This is then run later by pyinfra's ``__main__`` or the
 :doc:`./pyinfra.api.operations` module.
 """
 
+from __future__ import annotations
+
 from functools import wraps
+from inspect import signature
+from io import StringIO
 from types import FunctionType
-from typing import TYPE_CHECKING
+from typing import Any, Callable, Generator, Iterator, Optional, cast
+
+from typing_extensions import ParamSpec
 
 import pyinfra
 from pyinfra import context, logger
 from pyinfra.context import ctx_host, ctx_state
 
-from .arguments import get_execution_kwarg_keys, pop_global_arguments
-from .command import StringCommand
+from .arguments import EXECUTION_KWARG_KEYS, AllArguments, pop_global_arguments
+from .arguments_typed import PyinfraOperation
+from .command import PyinfraCommand, StringCommand
 from .exceptions import OperationValueError, PyinfraError
 from .host import Host
 from .operations import run_host_op
+from .state import State, StateOperationHostData, StateOperationMeta
 from .util import (
-    get_args_kwargs_spec,
     get_call_location,
+    get_file_sha1,
     get_operation_order_from_stack,
     log_operation_start,
     make_hash,
-    memoize,
 )
 
-if TYPE_CHECKING:
-    from pyinfra.api.state import State
-
 op_meta_default = object()
 
 
 class OperationMeta:
-    combined_output_lines = None
-
-    def __init__(self, hash=None, commands=None):
-        # Wrap all the attributes
-        commands = commands or []
-        self.commands = commands
-        self.hash = hash
+    _hash: str
 
-        # Changed flag = did we do anything?
-        self.changed = len(self.commands) > 0
+    _combined_output_lines = None
+    _commands: Optional[list[Any]] = None
+    _maybe_is_change: Optional[bool] = False
+    _success: Optional[bool] = None
+
+    def __init__(self, hash, is_change: Optional[bool]):
+        self._hash = hash
+        self._maybe_is_change = is_change
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """
         Return Operation object as a string.
         """
 
+        if self._commands is not None:
+            return (
+                "OperationMeta(executed=True, "
+                f"success={self.did_succeed}, hash={self._hash}, commands={len(self._commands)})"
+            )
         return (
-            f"OperationMeta(commands={len(self.commands)}, "
-            f"changed={self.changed}, hash={self.hash})"
+            "OperationMeta(executed=False, "
+            f"maybeChange={self._maybe_is_change}, hash={self._hash})"
         )
 
-    def set_combined_output_lines(self, combined_output_lines):
-        self.combined_output_lines = combined_output_lines
+    # Completion & status checks
+    def set_complete(
+        self,
+        success: bool,
+        commands: list[Any],
+        combined_output_lines,
+    ) -> None:
+        if self.is_complete():
+            raise RuntimeError("Cannot complete an already complete operation")
+        self._success = success
+        self._commands = commands
+        self._combined_output_lines = combined_output_lines
+
+    def is_complete(self) -> bool:
+        return self._success is not None
+
+    def _raise_if_not_complete(self) -> None:
+        if not self.is_complete():
+            raise RuntimeError("Cannot evaluate operation result before execution")
 
-    def _get_lines(self, types=("stdout", "stderr")):
-        if self.combined_output_lines is None:
-            raise AttributeError("Output is not available until operations have been executed")
+    def _did_change(self) -> bool:
+        return bool(self._success and len(self._commands or []) > 0)
+
+    @property
+    def did_change(self):
+        return context.host.when(self._did_change)
 
-        return [line for type_, line in self.combined_output_lines if type_ in types]
+    @property
+    def did_not_change(self):
+        return context.host.when(lambda: not self._did_change())
+
+    def did_succeed(self) -> bool:
+        self._raise_if_not_complete()
+        return self._success is True
+
+    def did_error(self) -> bool:
+        self._raise_if_not_complete()
+        return self._success is False
+
+    # TODO: deprecated, remove in v4
+    @property
+    def changed(self) -> bool:
+        if self.is_complete():
+            return self._did_change()
+
+        if self._maybe_is_change is not None:
+            return self._maybe_is_change
+
+        op_data = context.state.get_op_data_for_host(context.host, self._hash)
+        cmd_gen = op_data.command_generator
+        for _ in cmd_gen():
+            return True
+        return False
+
+    # Output lines
+    def _get_lines(self, types=("stdout", "stderr")):
+        self._raise_if_not_complete()
+        assert self._combined_output_lines is not None
+        return [line for type_, line in self._combined_output_lines if type_ in types]
 
     @property
     def stdout_lines(self):
         return self._get_lines(types=("stdout",))
 
     @property
     def stderr_lines(self):
         return self._get_lines(types=("stderr",))
 
     @property
-    def stdout(self):
+    def stdout(self) -> str:
         return "\n".join(self.stdout_lines)
 
     @property
-    def stderr(self):
+    def stderr(self) -> str:
         return "\n".join(self.stderr_lines)
 
 
-def add_op(state: "State", op_func, *args, **kwargs):
+def add_op(state: State, op_func, *args, **kwargs):
     """
     Prepare & add an operation to ``pyinfra.state`` by executing it on all hosts.
 
     Args:
         state (``pyinfra.api.State`` obj): the deploy state to add the operation
         to op_func (function): the operation function from one of the modules,
         ie ``server.user``
@@ -108,178 +168,176 @@
         for op_host in hosts:
             with ctx_host.use(op_host):
                 results[op_host] = op_func(*args, **kwargs)
 
     return results
 
 
-@memoize
-def show_state_host_arguments_warning(call_location):
-    logger.warning(
-        (
-            "{0}:\n\tLegacy operation function detected! Operations should no longer define "
-            "`state` and `host` arguments."
-        ).format(call_location),
-    )
+P = ParamSpec("P")
 
 
 def operation(
-    func=None,
-    pipeline_facts=None,
     is_idempotent: bool = True,
-    idempotent_notice=None,
-    frame_offset: int = 1,
-):
+    idempotent_notice: Optional[str] = None,
+    is_deprecated: bool = False,
+    deprecated_for: Optional[str] = None,
+    _set_in_op: bool = True,
+) -> Callable[[Callable[P, Generator]], PyinfraOperation[P]]:
     """
     Decorator that takes a simple module function and turn it into the internal
     operation representation that consists of a list of commands + options
     (sudo, (sudo|su)_user, env).
     """
 
-    # If not decorating, return function with config attached
-    if func is None:
+    def decorator(f: Callable[P, Generator]) -> PyinfraOperation[P]:
+        f.is_idempotent = is_idempotent  # type: ignore[attr-defined]
+        f.idempotent_notice = idempotent_notice  # type: ignore[attr-defined]
+        f.is_deprecated = is_deprecated  # type: ignore[attr-defined]
+        f.deprecated_for = deprecated_for  # type: ignore[attr-defined]
+        return _wrap_operation(f, _set_in_op=_set_in_op)
+
+    return decorator
 
-        def decorator(f):
-            f.pipeline_facts = pipeline_facts
-            f.is_idempotent = is_idempotent
-            f.idempotent_notice = idempotent_notice
-            return operation(f, frame_offset=2)
-
-        return decorator
-
-    # Check whether an operation is "legacy" - ie contains state=None, host=None kwargs
-    # TODO: remove this in v3
-    is_legacy = False
-    args, kwargs = get_args_kwargs_spec(func)
-    if all(key in kwargs and kwargs[key] is None for key in ("state", "host")):
-        show_state_host_arguments_warning(get_call_location(frame_offset=frame_offset))
-        is_legacy = True
-    func.is_legacy = is_legacy
 
-    # Actually decorate!
+def _wrap_operation(func: Callable[P, Generator], _set_in_op: bool = True) -> PyinfraOperation[P]:
     @wraps(func)
-    def decorated_func(*args, **kwargs):
+    def decorated_func(*args: P.args, **kwargs: P.kwargs) -> OperationMeta:
         state = context.state
         host = context.host
 
+        if host.in_op:
+            raise Exception(
+                "Operation called within another operation, this is not allowed! Use the `_inner` "
+                + "function to call the underlying operation."
+            )
+
+        if func.is_deprecated:  # type: ignore[attr-defined]
+            if func.deprecated_for:  # type: ignore[attr-defined]
+                logger.warning(
+                    f"The {get_operation_name_from_func(func)} operation is "
+                    + f"deprecated, please use: {func.deprecated_for}",  # type: ignore[attr-defined] # noqa
+                )
+            else:
+                logger.warning(f"The {get_operation_name_from_func(func)} operation is deprecated")
+
         # Configure operation
         #
         # Get the meta kwargs (globals that apply to all hosts)
-        global_kwargs, global_kwarg_keys = pop_global_arguments(kwargs)
-
-        # If this op is being called inside another, just return here
-        # (any unwanted/op-related kwargs removed above).
-        if host.in_op:
-            if global_kwarg_keys:
-                _error_msg = "Nested operation called with global arguments: {0} ({1})".format(
-                    global_kwarg_keys,
-                    get_call_location(),
-                )
-                raise PyinfraError(_error_msg)
-            return func(*args, **kwargs) or []
+        global_arguments, global_argument_keys = pop_global_arguments(kwargs)
 
-        kwargs = _solve_legacy_operation_arguments(func, state, host, kwargs)
-        names, add_args = _generate_operation_name(func, host, kwargs, global_kwargs)
-        op_order, op_hash = _solve_operation_consistency(names, state, host)
+        names, add_args = generate_operation_name(func, host, kwargs, global_arguments)
+        op_order, op_hash = solve_operation_consistency(names, state, host)
 
         # Ensure shared (between servers) operation meta, mutates state
-        op_meta = _ensure_shared_op_meta(state, op_hash, op_order, global_kwargs, names)
+        op_meta = ensure_shared_op_meta(state, op_hash, op_order, global_arguments, names)
 
         # Attach normal args, if we're auto-naming this operation
         if add_args:
-            op_meta = _attach_args(op_meta, args, kwargs)
+            op_meta = attach_args(op_meta, args, kwargs)
 
         # Check if we're actually running the operation on this host
         # Run once and we've already added meta for this op? Stop here.
-        if op_meta["run_once"]:
+        if op_meta.global_arguments["_run_once"]:
             has_run = False
             for ops in state.ops.values():
                 if op_hash in ops:
                     has_run = True
                     break
 
             if has_run:
-                return OperationMeta(op_hash)
-
-        # "Run" operation
-        #
+                return OperationMeta(op_hash, is_change=False)
 
-        # Otherwise, flag as in-op and run it to get the commands
-        host.in_op = True
-        host.current_op_hash = op_hash
-        host.current_op_global_kwargs = global_kwargs
-
-        # Convert to list as the result may be a generator
-        commands = func(*args, **kwargs)
-        commands = [  # convert any strings -> StringCommand's
-            StringCommand(command.strip()) if isinstance(command, str) else command
-            for command in commands
-        ]
-
-        host.in_op = False
-        host.current_op_hash = None
-        host.current_op_global_kwargs = None
+        # "Run" operation - here we make a generator that will yield out actual commands to execute
+        # and, if we're diff-ing, we then iterate the generator now to determine if any changes
+        # *would* be made based on the *current* remote state.
+
+        def command_generator() -> Iterator[PyinfraCommand]:
+            # Check global _if_ argument function and do nothing if returns False
+            if state.is_executing:
+                _ifs = global_arguments.get("_if")
+                if _ifs and not all(_if() for _if in _ifs):
+                    return
+
+            host.in_op = _set_in_op
+            host.current_op_hash = op_hash
+            host.current_op_global_arguments = global_arguments
+
+            try:
+                for command in func(*args, **kwargs):
+                    if isinstance(command, str):
+                        command = StringCommand(command.strip())
+                    yield command
+            finally:
+                host.in_op = False
+                host.current_op_hash = None
+                host.current_op_global_arguments = None
+
+        op_is_change = None
+        if state.should_check_for_changes():
+            op_is_change = False
+            for _ in command_generator():
+                op_is_change = True
+                break
+        else:
+            # If not calling the op function to check for change we still want to ensure the args
+            # are valid, so use Signature.bind to trigger any TypeError.
+            signature(func).bind(*args, **kwargs)
 
         # Add host-specific operation data to state, this mutates state
-        operation_meta = _update_state_meta(state, host, commands, op_hash, op_meta, global_kwargs)
+        host_meta = state.get_meta_for_host(host)
+        host_meta.ops += 1
+        if op_is_change:
+            host_meta.ops_change += 1
+        else:
+            host_meta.ops_no_change += 1
 
-        # Return result meta for use in deploy scripts
-        return operation_meta
+        operation_meta = OperationMeta(op_hash, op_is_change)
 
-    decorated_func._pyinfra_op = func  # type: ignore
-    return decorated_func
+        # Add the server-relevant commands
+        op_data = StateOperationHostData(command_generator, global_arguments, operation_meta)
+        state.set_op_data_for_host(host, op_hash, op_data)
 
+        # If we're already in the execution phase, execute this operation immediately
+        if state.is_executing:
+            execute_immediately(state, host, op_hash)
 
-def _solve_legacy_operation_arguments(op_func, state, host, kwargs):
-    """
-    Solve legacy operation arguments.
-    """
+        # Return result meta for use in deploy scripts
+        return operation_meta
 
-    # If this is a legacy operation function (ie - state & host arg kwargs), ensure that state
-    # and host are included as kwargs.
+    decorated_func._inner = func  # type: ignore[attr-defined]
+    return cast(PyinfraOperation[P], decorated_func)
 
-    # Legacy operation arguments
-    if op_func.is_legacy:
-        if "state" not in kwargs:
-            kwargs["state"] = state
-        if "host" not in kwargs:
-            kwargs["host"] = host
-    # If not legacy, pop off any state/host kwargs that may come from legacy @deploy functions
-    else:
-        kwargs.pop("state", None)
-        kwargs.pop("host", None)
 
-    return kwargs
+def get_operation_name_from_func(func):
+    if func.__module__:
+        module_bits = func.__module__.split(".")
+        module_name = module_bits[-1]
+        return "{0}.{1}".format(module_name, func.__name__)
+    else:
+        return func.__name__
 
 
-def _generate_operation_name(func, host, kwargs, global_kwargs):
+def generate_operation_name(func, host, kwargs, global_arguments):
     # Generate an operation name if needed (Module/Operation format)
-    name = global_kwargs.get("name")
+    name = global_arguments.get("name")
     add_args = False
     if name:
         names = {name}
     else:
         add_args = True
-
-        if func.__module__:
-            module_bits = func.__module__.split(".")
-            module_name = module_bits[-1]
-            name = "{0}/{1}".format(module_name.title(), func.__name__.title())
-        else:
-            name = func.__name__
-
+        name = get_operation_name_from_func(func)
         names = {name}
 
     if host.current_deploy_name:
         names = {"{0} | {1}".format(host.current_deploy_name, name) for name in names}
 
     return names, add_args
 
 
-def _solve_operation_consistency(names, state, host):
+def solve_operation_consistency(names, state, host):
     # Operation order is used to tie-break available nodes in the operation DAG, in CLI mode
     # we use stack call order so this matches as defined by the user deploy code.
     if pyinfra.is_cli:
         op_order = get_operation_order_from_stack(state)
     # In API mode we just increase the order for each host
     else:
         op_order = [len(host.op_hash_order)]
@@ -306,89 +364,59 @@
 
     op_order = tuple(op_order)
     logger.debug(f"Adding operation, {names}, opOrder={op_order}, opHash={op_hash}")
     return op_order, op_hash
 
 
 # NOTE: this function mutates state.op_meta for this hash
-def _ensure_shared_op_meta(state, op_hash, op_order, global_kwargs, names):
-    op_meta = state.op_meta.setdefault(
-        op_hash,
-        {
-            "names": set(),
-            "args": [],
-            "op_order": op_order,
-        },
-    )
-
-    for key in get_execution_kwarg_keys():
-        global_value = global_kwargs.pop(key)
-        op_meta_value = op_meta.get(key, op_meta_default)
+def ensure_shared_op_meta(
+    state: State,
+    op_hash: str,
+    op_order: tuple[int, ...],
+    global_arguments: AllArguments,
+    names: set[str],
+):
+    op_meta = state.op_meta.setdefault(op_hash, StateOperationMeta(op_order))
+
+    for key in EXECUTION_KWARG_KEYS:
+        global_value = global_arguments.pop(key)  # type: ignore[misc]
+        op_meta_value = op_meta.global_arguments.get(key, op_meta_default)
 
         if op_meta_value is not op_meta_default and global_value != op_meta_value:
             raise OperationValueError("Cannot have different values for `{0}`.".format(key))
 
-        op_meta[key] = global_value
+        op_meta.global_arguments[key] = global_value  # type: ignore[literal-required]
 
     # Add any new names to the set
-    op_meta["names"].update(names)
+    op_meta.names.update(names)
 
     return op_meta
 
 
-def _execute_immediately(state, host, op_data, op_meta, op_hash):
-    logger.warning(
-        f"Note: nested operations are currently in beta ({get_call_location()})\n"
-        "    More information: "
-        "https://docs.pyinfra.com/en/2.x/using-operations.html#nested-operations",
-    )
-    op_data["parent_op_hash"] = host.executing_op_hash
+def execute_immediately(state, host, op_hash):
+    op_meta = state.get_op_meta(op_hash)
+    op_data = state.get_op_data_for_host(host, op_hash)
+    op_data.parent_op_hash = host.executing_op_hash
     log_operation_start(op_meta, op_types=["nested"], prefix="")
     run_host_op(state, host, op_hash)
 
 
-def _attach_args(op_meta, args, kwargs):
-    for arg in args:
-        if isinstance(arg, FunctionType):
-            arg = arg.__name__
+def _get_arg_value(arg):
+    if isinstance(arg, FunctionType):
+        return arg.__name__
+    if isinstance(arg, StringIO):
+        return f"StringIO(hash={get_file_sha1(arg)})"
+    return arg
+
 
-        if arg not in op_meta["args"]:
-            op_meta["args"].append(arg)
+def attach_args(op_meta, args, kwargs):
+    for arg in args:
+        if arg not in op_meta.args:
+            op_meta.args.append(str(_get_arg_value(arg)))
 
     # Attach keyword args
     for key, value in kwargs.items():
-        if isinstance(value, FunctionType):
-            value = value.__name__
-
-        arg = "=".join((str(key), str(value)))
-        if arg not in op_meta["args"]:
-            op_meta["args"].append(arg)
+        arg = "=".join((str(key), str(_get_arg_value(value))))
+        if arg not in op_meta.args:
+            op_meta.args.append(arg)
 
     return op_meta
-
-
-# NOTE: this function mutates state.meta for this host
-def _update_state_meta(state, host, commands, op_hash, op_meta, global_kwargs):
-    # We're doing some commands, meta/ops++
-    state.meta[host]["ops"] += 1
-    state.meta[host]["commands"] += len(commands)
-
-    if commands:
-        state.meta[host]["ops_change"] += 1
-    else:
-        state.meta[host]["ops_no_change"] += 1
-
-    operation_meta = OperationMeta(op_hash, commands)
-
-    # Add the server-relevant commands
-    op_data = {
-        "commands": commands,
-        "global_kwargs": global_kwargs,
-        "operation_meta": operation_meta,
-    }
-    state.set_op_data(host, op_hash, op_data)
-
-    # If we're already in the execution phase, execute this operation immediately
-    if state.is_executing:
-        _execute_immediately(state, host, op_data, op_meta, op_hash)
-
-    return operation_meta
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/operations.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,223 +1,186 @@
+from __future__ import annotations
+
 import traceback
 from itertools import product
 from socket import error as socket_error, timeout as timeout_error
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional, cast
 
 import click
 import gevent
 from paramiko import SSHException
 
-import pyinfra
 from pyinfra import logger
-from pyinfra.context import ctx_host
+from pyinfra.connectors.util import CommandOutput, OutputLine
+from pyinfra.context import ctx_host, ctx_state
 from pyinfra.progress import progress_spinner
 
-from .arguments import get_executor_kwarg_keys
+from .arguments import CONNECTOR_ARGUMENT_KEYS, ConnectorArguments
 from .command import FunctionCommand, PyinfraCommand, StringCommand
 from .exceptions import PyinfraError
 from .util import (
     format_exception,
     log_error_or_warning,
     log_host_command_error,
     log_operation_start,
-    memoize,
     print_host_combined_output,
 )
 
 if TYPE_CHECKING:
     from .inventory import Host
     from .state import State
 
 
-@memoize
-def show_pre_or_post_condition_warning(condition_name):
-    logger.warning("The `{0}` argument is in beta!".format(condition_name))
+# Run a single host operation
+#
 
 
-def run_host_op(state: "State", host: "Host", op_hash):
+def run_host_op(state: "State", host: "Host", op_hash: str) -> Optional[bool]:
     state.trigger_callbacks("operation_host_start", host, op_hash)
 
     if op_hash not in state.ops[host]:
         logger.info("{0}{1}".format(host.print_prefix, click.style("Skipped", "blue")))
         return True
 
-    op_data = state.get_op_data(host, op_hash)
-    global_kwargs = op_data["global_kwargs"]
-
     op_meta = state.get_op_meta(op_hash)
-
-    ignore_errors = global_kwargs["ignore_errors"]
-    continue_on_error = global_kwargs["continue_on_error"]
-
-    logger.debug("Starting operation %r on %s", op_meta["names"], host)
-
-    executor_kwarg_keys = get_executor_kwarg_keys()
-    base_executor_kwargs = {
-        key: global_kwargs[key] for key in executor_kwarg_keys if key in global_kwargs
-    }
-
-    def _run_shell_command(command, executor_kwargs):
-        status = False
-        combined_output_lines = []
-
-        try:
-            status, combined_output_lines = command.execute(state, host, executor_kwargs)
-        except (timeout_error, socket_error, SSHException) as e:
-            log_host_command_error(
-                host,
-                e,
-                timeout=global_kwargs["timeout"],
-            )
-
-        # If we failed and have no already printed the stderr, print it
-        if status is False and not state.print_output:
-            print_host_combined_output(host, combined_output_lines)
-
-        return status, combined_output_lines
-
-    def run_condition(condition_name: str) -> bool:
-        condition_value = global_kwargs[condition_name]
-        if not condition_value:
-            return True
-
-        show_pre_or_post_condition_warning(condition_name)
-
-        _shell_command_status, _ = _run_shell_command(
-            StringCommand(condition_value),
-            base_executor_kwargs,
-        )
-
-        if _shell_command_status:
-            return True
-
-        _log_msg = f"{condition_name} failed: {condition_value}"
-        log_error_or_warning(host, ignore_errors, description=_log_msg)
-
-        if ignore_errors:
-            return True
-
-        state.trigger_callbacks("operation_host_error", host, op_hash)
-        return False
-
-    if not run_condition("precondition"):
-        return False
-
-    state.ops_run.add(op_hash)
+    logger.debug("Starting operation %r on %s", op_meta.names, host)
 
     if host.executing_op_hash is None:
         host.executing_op_hash = op_hash
     else:
         host.nested_executing_op_hash = op_hash
 
-    return_status = False
+    try:
+        return _run_host_op(state, host, op_hash)
+    finally:
+        if host.nested_executing_op_hash:
+            host.nested_executing_op_hash = None
+        else:
+            host.executing_op_hash = None
+
+
+def _run_host_op(state: "State", host: "Host", op_hash: str) -> Optional[bool]:
+    op_data = state.get_op_data_for_host(host, op_hash)
+    global_arguments = op_data.global_arguments
+
+    ignore_errors = global_arguments["_ignore_errors"]
+    continue_on_error = global_arguments["_continue_on_error"]
+    timeout = global_arguments.get("_timeout", 0)
+
+    executor_kwarg_keys = CONNECTOR_ARGUMENT_KEYS
+    # See: https://github.com/python/mypy/issues/10371
+    base_connector_arguments: ConnectorArguments = cast(
+        ConnectorArguments,
+        {key: global_arguments[key] for key in executor_kwarg_keys if key in global_arguments},  # type: ignore[literal-required] # noqa
+    )
+
     did_error = False
     executed_commands = 0
-    all_combined_output_lines = []
+    commands = []
+    all_combined_output_lines: list[OutputLine] = []
 
-    for i, command in enumerate(op_data["commands"]):
+    for command in op_data.command_generator():
+        commands.append(command)
 
         status = False
 
-        executor_kwargs = base_executor_kwargs.copy()
-        executor_kwargs.update(command.executor_kwargs)
-
-        # Now we attempt to execute the command
-        #
+        connector_arguments = base_connector_arguments.copy()
+        connector_arguments.update(command.connector_arguments)
 
         if not isinstance(command, PyinfraCommand):
             raise TypeError("{0} is an invalid pyinfra command!".format(command))
 
         if isinstance(command, FunctionCommand):
             try:
-                status = command.execute(state, host, executor_kwargs)
-            except Exception as e:  # Custom functions could do anything, so expect anything!
-                _formatted_exc = format_exception(e)
-                _error_msg = "Unexpected error in Python callback: {0}".format(_formatted_exc)
-                _error_msg_styled = click.style(_error_msg, "red")
-                _error_log = "{0}{1}".format(host.print_prefix, _error_msg_styled)
+                status = command.execute(state, host, connector_arguments)
+            except Exception as e:
+                # Custom functions could do anything, so expect anything!
                 logger.warning(traceback.format_exc())
-                logger.error(_error_log)
+                host.log_styled(
+                    f"Unexpected error in Python callback: {format_exception(e)}",
+                    fg="red",
+                    log_func=logger.warning,
+                )
 
         elif isinstance(command, StringCommand):
-            status, combined_output_lines = _run_shell_command(command, executor_kwargs)
+            combined_output_lines = CommandOutput([])
+            try:
+                status, combined_output_lines = command.execute(
+                    state,
+                    host,
+                    connector_arguments,
+                )
+            except (timeout_error, socket_error, SSHException) as e:
+                log_host_command_error(host, e, timeout=timeout)
             all_combined_output_lines.extend(combined_output_lines)
+            # If we failed and have not already printed the stderr, print it
+            if status is False and not state.print_output:
+                print_host_combined_output(host, combined_output_lines)
 
         else:
             try:
-                status = command.execute(state, host, executor_kwargs)
+                status = command.execute(state, host, connector_arguments)
             except (timeout_error, socket_error, SSHException, IOError) as e:
-                _timeout = global_kwargs["timeout"]
-                log_host_command_error(host, e, timeout=_timeout)
+                log_host_command_error(host, e, timeout=timeout)
 
         # Break the loop to trigger a failure
         if status is False:
+            did_error = True
             if continue_on_error is True:
-                did_error = True
                 continue
             break
 
         executed_commands += 1
-        state.results[host]["commands"] += 1
 
-    # Commands didn't break, so count our successes & return True!
-    else:
-        if not run_condition("postcondition"):
-            return False
+    # Handle results
+    #
 
-        if not did_error:
-            return_status = True
+    op_success = return_status = not did_error
+    host_results = state.get_results_for_host(host)
 
-    if return_status is True:
-        state.results[host]["ops"] += 1
-        state.results[host]["success_ops"] += 1
+    if did_error is False:
+        host_results.ops += 1
+        host_results.success_ops += 1
 
-        _status_log = "Success" if len(op_data["commands"]) > 0 else "No changes"
+        _status_log = "Success" if executed_commands > 0 else "No changes"
         _click_log_status = click.style(_status_log, "green")
         logger.info("{0}{1}".format(host.print_prefix, _click_log_status))
 
-        # Trigger any success handler
-        if global_kwargs["on_success"]:
-            global_kwargs["on_success"](state, host, op_hash)
-
         state.trigger_callbacks("operation_host_success", host, op_hash)
     else:
         if ignore_errors:
-            state.results[host]["ignored_error_ops"] += 1
+            host_results.ignored_error_ops += 1
         else:
-            state.results[host]["error_ops"] += 1
+            host_results.error_ops += 1
 
         if executed_commands:
-            state.results[host]["partial_ops"] += 1
+            host_results.partial_ops += 1
 
-        _command_description = f"executed {executed_commands}/{len(op_data['commands'])} commands"
+        _command_description = f"executed {executed_commands} commands"
         log_error_or_warning(host, ignore_errors, _command_description, continue_on_error)
 
-        # Always trigger any error handler
-        if global_kwargs["on_error"]:
-            global_kwargs["on_error"](state, host, op_hash)
-
         # Ignored, op "completes" w/ ignored error
         if ignore_errors:
-            state.results[host]["ops"] += 1
+            host_results.ops += 1
+            return_status = True
 
         # Unignored error -> False
         state.trigger_callbacks("operation_host_error", host, op_hash)
 
-        if ignore_errors:
-            return_status = True
+    op_data.operation_meta.set_complete(
+        op_success,
+        commands,
+        all_combined_output_lines,
+    )
 
-    op_data["operation_meta"].set_combined_output_lines(all_combined_output_lines)
+    return return_status
 
-    if host.nested_executing_op_hash:
-        host.nested_executing_op_hash = None
-    else:
-        host.executing_op_hash = None
 
-    return return_status
+# Run all operations strategies
+#
 
 
 def _run_host_op_with_context(state: "State", host: "Host", op_hash: str):
     with ctx_host.use(host):
         return run_host_op(state, host, op_hash)
 
 
@@ -237,22 +200,19 @@
         # Trigger CLI progress if provided
         if progress:
             progress((host, op_hash))
 
         if result is False:
             raise PyinfraError(
                 "Error in operation {0} on {1}".format(
-                    ", ".join(op_meta["names"]),
+                    ", ".join(op_meta.names),
                     host,
                 ),
             )
 
-        if pyinfra.is_cli:
-            click.echo(err=True)
-
 
 def _run_serial_ops(state: "State"):
     """
     Run all ops for all servers, one server at a time.
     """
 
     for host in list(state.inventory.iter_active_hosts()):
@@ -298,33 +258,32 @@
     state.trigger_callbacks("operation_start", op_hash)
 
     op_meta = state.get_op_meta(op_hash)
     log_operation_start(op_meta)
 
     failed_hosts = set()
 
-    if op_meta["serial"]:
+    if op_meta.global_arguments["_serial"]:
         with progress_spinner(state.inventory.iter_active_hosts()) as progress:
             # For each host, run the op
             for host in state.inventory.iter_active_hosts():
                 result = _run_host_op_with_context(state, host, op_hash)
                 progress(host)
 
                 if not result:
                     failed_hosts.add(host)
 
     else:
         # Start with the whole inventory in one batch
         batches = [list(state.inventory.iter_active_hosts())]
 
         # If parallel set break up the inventory into a series of batches
-        if op_meta["parallel"]:
-            parallel = op_meta["parallel"]
+        parallel = op_meta.global_arguments["_parallel"]
+        if parallel:
             hosts = list(state.inventory.iter_active_hosts())
-
             batches = [hosts[i : i + parallel] for i in range(0, len(hosts), parallel)]
 
         for batch in batches:
             with progress_spinner(batch) as progress:
                 # Spawn greenlet for each host
                 if state.pool is None:
                     raise PyinfraError("No pool found on state.")
@@ -342,17 +301,14 @@
                 for greenlet, host in greenlet_to_host.items():
                     if not greenlet.get():
                         failed_hosts.add(host)
 
     # Now all the batches/hosts are complete, fail any failures
     state.fail_hosts(failed_hosts)
 
-    if pyinfra.is_cli:
-        click.echo(err=True)
-
     state.trigger_callbacks("operation_end", op_hash)
 
 
 def run_ops(state: "State", serial: bool = False, no_wait: bool = False):
     """
     Runs all operations across all servers in a configurable manner.
 
@@ -361,19 +317,18 @@
         serial (boolean): whether to run operations host by host
         no_wait (boolean): whether to wait for all hosts between operations
     """
 
     # Flag state as deploy in process
     state.is_executing = True
 
-    # Run all ops, but server by server
-    if serial:
-        _run_serial_ops(state)
-
-    # Run all the ops on each server in parallel (not waiting at each operation)
-    elif no_wait:
-        _run_no_wait_ops(state)
-
-    # Default: run all ops in order, waiting at each for all servers to complete
-    else:
-        for op_hash in state.get_op_order():
-            _run_single_op(state, op_hash)
+    with ctx_state.use(state):
+        # Run all ops, but server by server
+        if serial:
+            _run_serial_ops(state)
+        # Run all the ops on each server in parallel (not waiting at each operation)
+        elif no_wait:
+            _run_no_wait_ops(state)
+        # Default: run all ops in order, waiting at each for all servers to complete
+        else:
+            for op_hash in state.get_op_order():
+                _run_single_op(state, op_hash)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/state.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/state.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-from contextlib import contextmanager
+from __future__ import annotations
+
+from collections import defaultdict
+from dataclasses import dataclass
+from enum import IntEnum
 from graphlib import CycleError, TopologicalSorter
 from multiprocessing import cpu_count
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set
-from uuid import uuid4
+from typing import TYPE_CHECKING, Callable, Iterator, Optional
 
 from gevent.pool import Pool
 from paramiko import PKey
 
 from pyinfra import logger
 
 from .config import Config
 from .exceptions import PyinfraError
-from .util import sha1_hash
 
 if TYPE_CHECKING:
+    from pyinfra.api.arguments import AllArguments
+    from pyinfra.api.command import PyinfraCommand
     from pyinfra.api.host import Host
     from pyinfra.api.inventory import Inventory
+    from pyinfra.api.operation import OperationMeta
 
 
 # Work out the max parallel we can achieve with the open files limit of the user/process,
 # take 10 for opening Python files and /3 for ~3 files per host during op runs.
 # See: https://github.com/Fizzadar/pyinfra/issues/44
 try:
     from resource import RLIMIT_NOFILE, getrlimit
@@ -73,14 +78,66 @@
         pass
 
     @staticmethod
     def operation_end(state: "State", op_hash):
         pass
 
 
+class StateStage(IntEnum):
+    # Setup - collect inventory & data
+    Setup = 1
+    # Connect - connect to the inventory
+    Connect = 2
+    # Prepare - detect operation changes
+    Prepare = 3
+    # Execute - execute operations
+    Execute = 4
+    # Disconnect - disconnect from the inventory
+    Disconnect = 5
+
+
+class StateOperationMeta:
+    names: set[str]
+    args: list[str]
+    op_order: tuple[int, ...]
+    global_arguments: "AllArguments"
+
+    def __init__(self, op_order: tuple[int, ...]):
+        self.op_order = op_order
+        self.names = set()
+        self.args = []
+        self.global_arguments = {}  # type: ignore
+
+
+@dataclass
+class StateOperationHostData:
+    command_generator: Callable[[], Iterator["PyinfraCommand"]]
+    global_arguments: "AllArguments"
+    operation_meta: "OperationMeta"
+    parent_op_hash: Optional[str] = None
+
+
+class StateHostMeta:
+    ops = 0
+    ops_change = 0
+    ops_no_change = 0
+    op_hashes: set[str]
+
+    def __init__(self):
+        self.op_hashes = set()
+
+
+class StateHostResults:
+    ops = 0
+    success_ops = 0
+    error_ops = 0
+    ignored_error_ops = 0
+    partial_ops = 0
+
+
 class State:
     """
     Manages state for a pyinfra deploy.
     """
 
     initialised: bool = False
 
@@ -89,43 +146,65 @@
 
     # A pyinfra.api.Config
     config: "Config"
 
     # Main gevent pool
     pool: "Pool"
 
+    # Current stage this state is in
+    current_stage: StateStage = StateStage.Setup
+    # Warning counters by stage
+    stage_warnings: dict[StateStage, int] = defaultdict(int)
+
     # Whether we are executing operations (ie hosts are all ready)
     is_executing: bool = False
 
+    # Whether we should check for operation changes as part of the operation ordering phase, this
+    # allows us to guesstimate which ops will result in changes on which hosts.
+    check_for_changes: bool = True
+
     print_noop_info: bool = False  # print "[host] noop: reason for noop"
     print_fact_info: bool = False  # print "loaded fact X"
     print_input: bool = False
     print_fact_input: bool = False
     print_output: bool = False
     print_fact_output: bool = False
 
     # Used in CLI
     cwd: Optional[str] = None  # base directory for locating files/templates/etc
     current_deploy_filename: Optional[str] = None
     current_exec_filename: Optional[str] = None
     current_op_file_number: int = 0
+    should_raise_failed_hosts: Optional[Callable[["State"], bool]] = None
 
     def __init__(
-        self, inventory: Optional["Inventory"] = None, config: Optional["Config"] = None, **kwargs
+        self,
+        inventory: Optional["Inventory"] = None,
+        config: Optional["Config"] = None,
+        check_for_changes: bool = True,
+        **kwargs,
     ):
-        """Initializes the state, the main Pyinfra
+        """
+        Initializes the state, the main Pyinfra
 
         Args:
             inventory (Optional[Inventory], optional): The inventory. Defaults to None.
             config (Optional[Config], optional): The config object. Defaults to None.
         """
+        self.check_for_changes = check_for_changes
+
         if inventory:
             self.init(inventory, config, **kwargs)
 
-    def init(self, inventory: "Inventory", config: Optional["Config"], initial_limit=None):
+    def init(
+        self,
+        inventory: "Inventory",
+        config: Optional["Config"],
+        initial_limit=None,
+    ):
         # Config validation
         #
 
         # If no config, create one using the defaults
         if config is None:
             config = Config()
 
@@ -146,112 +225,86 @@
                     "    Max recommended value: {2}"
                 ).format(config.PARALLEL, nofile_limit, MAX_PARALLEL),
             )
 
         # Actually initialise the state object
         #
 
-        self.callback_handlers: List[BaseStateCallback] = []
+        self.callback_handlers: list[BaseStateCallback] = []
 
         # Setup greenlet pools
         self.pool = Pool(config.PARALLEL)
         self.fact_pool = Pool(config.PARALLEL)
 
         # Private keys
-        self.private_keys: Dict[str, PKey] = {}
+        self.private_keys: dict[str, PKey] = {}
 
         # Assign inventory/config
         self.inventory = inventory
         self.config = config
 
         # Hosts we've activated at any time
-        self.activated_hosts: Set["Host"] = set()
+        self.activated_hosts: set["Host"] = set()
         # Active hosts that *haven't* failed yet
-        self.active_hosts: Set["Host"] = set()
+        self.active_hosts: set["Host"] = set()
         # Hosts that have failed
-        self.failed_hosts: Set["Host"] = set()
+        self.failed_hosts: set["Host"] = set()
 
         # Limit hosts changes dynamically to limit operations to a subset of hosts
-        self.limit_hosts: List["Host"] = initial_limit
+        self.limit_hosts: list["Host"] = initial_limit
 
         # Op basics
-        self.op_meta: Dict[str, dict] = {}  # maps operation hash -> names/etc
-        self.ops_run: Set[str] = set()  # list of ops which have been started/run
+        self.op_meta: dict[str, StateOperationMeta] = {}  # maps operation hash -> names/etc
 
         # Op dict for each host
-        self.ops: Dict["Host", dict] = {host: {} for host in inventory}
-
-        # Facts dict for each host
-        self.facts: Dict["Host", Any] = {host: {} for host in inventory}
+        self.ops: dict["Host", dict[str, StateOperationHostData]] = {host: {} for host in inventory}
 
         # Meta dict for each host
-        self.meta = {
-            host: {
-                "ops": 0,  # one function call in a deploy file
-                "ops_change": 0,
-                "ops_no_change": 0,
-                "commands": 0,  # actual # of commands to run
-                "op_hashes": set(),
-            }
-            for host in inventory
-        }
+        self.meta: dict["Host", StateHostMeta] = {host: StateHostMeta() for host in inventory}
 
         # Results dict for each host
-        self.results = {
-            host: {
-                "ops": 0,  # success_ops + failed ops w/ignore_errors
-                "success_ops": 0,
-                "error_ops": 0,
-                "ignored_error_ops": 0,
-                "partial_ops": 0,  # operations that had an error, but did do something
-                "commands": 0,
-            }
-            for host in inventory
+        self.results: dict["Host", StateHostResults] = {
+            host: StateHostResults() for host in inventory
         }
 
         # Assign state back references to inventory & config
         inventory.state = config.state = self
         for host in inventory:
-            host.state = self
+            host.init(self)
 
         self.initialised = True
 
-    def to_dict(self):
-        return {
-            "op_order": self.get_op_order(),
-            "ops": self.ops,
-            "facts": self.facts,
-            "meta": self.meta,
-            "results": self.results,
-        }
+    def set_stage(self, stage: StateStage) -> None:
+        if stage < self.current_stage:
+            raise Exception("State stage cannot go backwards!")
+        self.current_stage = stage
+
+    def increment_warning_counter(self) -> None:
+        self.stage_warnings[self.current_stage] += 1
+
+    def get_warning_counter(self) -> int:
+        return self.stage_warnings[self.current_stage]
+
+    def should_check_for_changes(self):
+        return self.check_for_changes
 
     def add_callback_handler(self, handler):
         if not isinstance(handler, BaseStateCallback):
             raise TypeError(
                 ("{0} is not a valid callback handler (use `BaseStateCallback`)").format(handler),
             )
         self.callback_handlers.append(handler)
 
     def trigger_callbacks(self, method_name: str, *args, **kwargs):
         for handler in self.callback_handlers:
             func = getattr(handler, method_name)
             func(self, *args, **kwargs)
 
-    @contextmanager
-    def preserve_loop_order(self, items):
-        logger.warning(
-            (
-                "Using `state.preserve_loop_order` is not longer required for operations to be "
-                "executed in correct loop order and can be safely removed."
-            ),
-        )
-        yield lambda: items
-
     def get_op_order(self):
-        ts = TopologicalSorter()
+        ts: TopologicalSorter = TopologicalSorter()
 
         for host in self.inventory:
             for i, op_hash in enumerate(host.op_hash_order):
                 if not i:
                     ts.add(op_hash)
                 else:
                     ts.add(op_hash, host.op_hash_order[i - 1])
@@ -271,28 +324,43 @@
             )
 
         while ts.is_active():
             # Ensure that where we have multiple different operations that can be executed in any
             # dependency order we order them by line numbers.
             node_group = sorted(
                 ts.get_ready(),
-                key=lambda op_hash: self.op_meta[op_hash]["op_order"],
+                key=lambda op_hash: self.op_meta[op_hash].op_order,
             )
             ts.done(*node_group)
             final_op_order.extend(node_group)
 
         return final_op_order
 
-    def get_op_meta(self, op_hash: str):
+    def get_op_meta(self, op_hash: str) -> StateOperationMeta:
         return self.op_meta[op_hash]
 
-    def get_op_data(self, host: "Host", op_hash: str):
+    def get_meta_for_host(self, host: "Host") -> StateHostMeta:
+        return self.meta[host]
+
+    def get_results_for_host(self, host: "Host") -> StateHostResults:
+        return self.results[host]
+
+    def get_op_data_for_host(
+        self,
+        host: "Host",
+        op_hash: str,
+    ) -> StateOperationHostData:
         return self.ops[host][op_hash]
 
-    def set_op_data(self, host: "Host", op_hash: str, op_data):
+    def set_op_data_for_host(
+        self,
+        host: "Host",
+        op_hash: str,
+        op_data: StateOperationHostData,
+    ):
         self.ops[host][op_hash] = op_data
 
     def activate_host(self, host: "Host"):
         """
         Flag a host as active.
         """
 
@@ -332,14 +400,17 @@
         if not active_hosts:
             raise PyinfraError("No hosts remaining!")
 
         if self.config.FAIL_PERCENT is not None:
             percent_failed = (1 - len(active_hosts) / activated_count) * 100
 
             if percent_failed > self.config.FAIL_PERCENT:
+                if self.should_raise_failed_hosts and self.should_raise_failed_hosts(self) is False:
+                    return
+
                 raise PyinfraError(
                     "Over {0}% of hosts failed ({1}%)".format(
                         self.config.FAIL_PERCENT,
                         int(round(percent_failed)),
                     ),
                 )
 
@@ -349,20 +420,7 @@
         """
 
         limit_hosts = self.limit_hosts
 
         if not isinstance(limit_hosts, list):
             return True
         return host in limit_hosts
-
-    def get_temp_filename(self, hash_key: Optional[str] = None, hash_filename: bool = True):
-        """
-        Generate a temporary filename for this deploy.
-        """
-
-        if not hash_key:
-            hash_key = str(uuid4())
-
-        if hash_filename:
-            hash_key = sha1_hash(hash_key)
-
-        return "{0}/pyinfra-{1}".format(self.config.TEMP_DIR, hash_key)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/api/util.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/api/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,38 @@
+from __future__ import annotations
+
 from functools import wraps
 from hashlib import sha1
-from inspect import getframeinfo, getfullargspec, stack
+from inspect import getframeinfo, stack
+from io import BytesIO, StringIO
 from os import getcwd, path, stat
 from socket import error as socket_error, timeout as timeout_error
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple
+from typing import IO, TYPE_CHECKING, Any, Callable, Dict, List, Optional, Type, Union
 
 import click
 from jinja2 import Environment, FileSystemLoader, StrictUndefined
 from paramiko import SSHException
+from typeguard import TypeCheckError, check_type
 
 import pyinfra
 from pyinfra import logger
 
 if TYPE_CHECKING:
     from pyinfra.api.host import Host
-    from pyinfra.api.state import State
+    from pyinfra.api.state import State, StateOperationMeta
+    from pyinfra.connectors.util import CommandOutput
 
 # 64kb chunks
 BLOCKSIZE = 65536
 
 # Caches
 TEMPLATES: Dict[Any, Any] = {}
 FILE_SHAS: Dict[Any, Any] = {}
 
-PYINFRA_API_DIR = path.dirname(__file__)
+PYINFRA_INSTALL_DIR = path.normpath(path.join(path.dirname(__file__), ".."))
 
 
 def get_file_path(state: "State", filename: str):
     if path.isabs(filename):
         return filename
 
     assert state.cwd is not None, "Cannot use `get_file_path` with no `state.cwd` set"
@@ -35,36 +40,14 @@
 
     if state.current_exec_filename and (filename.startswith("./") or filename.startswith(".\\")):
         relative_to = path.dirname(state.current_exec_filename)
 
     return path.join(relative_to, filename)
 
 
-def get_args_kwargs_spec(func: Callable[..., Any]) -> Tuple[List, Dict]:
-    args: List[Any] = []
-    kwargs: Dict[Any, Any] = {}
-
-    argspec = getfullargspec(func)
-    if not argspec.args:
-        return args, kwargs
-
-    if argspec.defaults:
-        kwargs = dict(
-            zip(
-                argspec.args[-len(argspec.defaults) :],
-                argspec.defaults,
-            ),
-        )
-        args = argspec.args[: -len(argspec.defaults)]
-    else:
-        args = argspec.args
-
-    return args, kwargs
-
-
 def get_kwargs_str(kwargs: Dict[Any, Any]):
     if not kwargs:
         return ""
 
     items = [
         "{0}={1}".format(key, value)
         for key, value in sorted(kwargs.items())
@@ -80,22 +63,22 @@
         return value
 
 
 def memoize(func: Callable[..., Any]):
     @wraps(func)
     def wrapper(*args, **kwargs):
         key = "{0}{1}".format(args, kwargs)
-        if key in wrapper.cache:
-            return wrapper.cache[key]
+        if key in wrapper.cache:  # type: ignore[attr-defined]
+            return wrapper.cache[key]  # type: ignore[attr-defined]
 
         value = func(*args, **kwargs)
-        wrapper.cache[key] = value
+        wrapper.cache[key] = value  # type: ignore[attr-defined]
         return value
 
-    wrapper.cache = {}  # type: ignore
+    wrapper.cache = {}  # type: ignore[attr-defined]
     return wrapper
 
 
 def get_call_location(frame_offset: int = 1):
     frame = get_caller_frameinfo(frame_offset=frame_offset)  # escape *this* function
     relpath = frame.filename
 
@@ -142,15 +125,15 @@
 
     if pyinfra.is_cli:
         line_numbers.append(state.current_op_file_number)
 
     for stack_item in stack_items[i:]:
         frame = getframeinfo(stack_item[0])
 
-        if frame.filename.startswith(PYINFRA_API_DIR):
+        if frame.filename.startswith(PYINFRA_INSTALL_DIR):
             continue
 
         line_numbers.append(frame.lineno)
 
     del stack_items
 
     return line_numbers
@@ -179,75 +162,67 @@
 
     if cache_key:
         TEMPLATES[cache_key] = template
 
     return template
 
 
-def sha1_hash(string: str):
+def sha1_hash(string: str) -> str:
     """
     Return the SHA1 of the input string.
     """
 
     hasher = sha1()
     hasher.update(string.encode("utf-8"))
     return hasher.hexdigest()
 
 
-def format_exception(e):
-    return "{0}{1}".format(e.__class__.__name__, e.args)
+def format_exception(e: Exception) -> str:
+    return f"{e.__class__.__name__}{e.args}"
 
 
-def print_host_combined_output(host: "Host", combined_output_lines):
-    for type_, line in combined_output_lines:
-        if type_ == "stderr":
-            logger.error(
-                "{0}{1}".format(
-                    host.print_prefix,
-                    click.style(line, "red"),
-                ),
-            )
+def print_host_combined_output(host: "Host", output: "CommandOutput") -> None:
+    for line in output:
+        if line.buffer_name == "stderr":
+            logger.error(f"{host.print_prefix}{click.style(line.line, 'red')}")
         else:
-            logger.error(
-                "{0}{1}".format(
-                    host.print_prefix,
-                    line,
-                ),
-            )
+            logger.error(f"{host.print_prefix}{line.line}")
 
 
-def log_operation_start(op_meta: Dict, op_types: Optional[List] = None, prefix: str = "--> "):
+def log_operation_start(
+    op_meta: "StateOperationMeta", op_types: Optional[List] = None, prefix: str = "--> "
+) -> None:
     op_types = op_types or []
-    if op_meta["serial"]:
+    if op_meta.global_arguments["_serial"]:
         op_types.append("serial")
-    if op_meta["run_once"]:
+    if op_meta.global_arguments["_run_once"]:
         op_types.append("run once")
 
     args = ""
-    if op_meta["args"]:
-        args = "({0})".format(", ".join(str(arg) for arg in op_meta["args"]))
+    if op_meta.args:
+        args = "({0})".format(", ".join(str(arg) for arg in op_meta.args))
 
     logger.info(
         "{0} {1} {2}".format(
             click.style(
                 "{0}Starting{1}operation:".format(
                     prefix,
                     " {0} ".format(", ".join(op_types)) if op_types else " ",
                 ),
                 "blue",
             ),
-            click.style(", ".join(op_meta["names"]), bold=True),
+            click.style(", ".join(op_meta.names), bold=True),
             args,
         ),
     )
 
 
 def log_error_or_warning(
     host: "Host", ignore_errors: bool, description: str = "", continue_on_error: bool = False
-):
+) -> None:
     log_func = logger.error
     log_color = "red"
     log_text = "Error: " if description else "Error"
 
     if ignore_errors:
         log_func = logger.warning
         log_color = "yellow"
@@ -262,15 +237,15 @@
             host.print_prefix,
             click.style(log_text, log_color),
             description,
         ),
     )
 
 
-def log_host_command_error(host: "Host", e, timeout: int = 0):
+def log_host_command_error(host: "Host", e: Exception, timeout: int = 0) -> None:
     if isinstance(e, timeout_error):
         logger.error(
             "{0}{1}".format(
                 host.print_prefix,
                 click.style(
                     "Command timed out after {0}s".format(
                         timeout,
@@ -346,52 +321,59 @@
 
 class get_file_io:
     """
     Given either a filename or an existing IO object, this context processor
     will open and close filenames, and leave IO objects alone.
     """
 
-    close = False
+    filename_or_io: Union[str, IO[Any]]
+    mode: str
+
+    _close: bool = False
+    _file_io: IO[Any]
 
     def __init__(self, filename_or_io, mode="rb"):
         if not (
             # Check we can be read
             hasattr(filename_or_io, "read")
             # Or we're a filename
             or isinstance(filename_or_io, str)
         ):
             raise TypeError(
                 "Invalid filename or IO object: {0}".format(
                     filename_or_io,
                 ),
             )
 
+        # Convert any StringIO/BytesIO to the other to match the desired mode
+        if isinstance(filename_or_io, StringIO) and mode == "rb":
+            filename_or_io.seek(0)
+            filename_or_io = BytesIO(filename_or_io.read().encode())
+        if isinstance(filename_or_io, BytesIO) and mode == "r":
+            filename_or_io.seek(0)
+            filename_or_io = StringIO(filename_or_io.read().decode())
+
         self.filename_or_io = filename_or_io
         self.mode = mode
 
     def __enter__(self):
-        # If we have a read attribute, just use the object as-is
-        if hasattr(self.filename_or_io, "read"):
-            file_io = self.filename_or_io
-
-        # Otherwise, assume a filename and open it up
-        else:
+        if isinstance(self.filename_or_io, str):
             file_io = open(self.filename_or_io, self.mode)
-
-            # Attach to self for closing on __exit__
-            self.file_io = file_io
-            self.close = True
+            self._file_io = file_io
+            self._close = True
+        else:
+            file_io = self.filename_or_io
 
         # Ensure we're at the start of the file
         file_io.seek(0)
         return file_io
 
     def __exit__(self, type, value, traceback):
-        if self.close:
-            self.file_io.close()
+        if self._close:
+            self._file_io.close()
 
     @property
     def cache_key(self):
         # If we're a filename, cache against that - we don't cache in-memory
         # file objects.
         if isinstance(self.filename_or_io, str):
             return self.filename_or_io
@@ -430,7 +412,19 @@
 def get_path_permissions_mode(pathname: str):
     """
     Get the permissions (bits) of a path as an integer.
     """
 
     mode_octal = oct(stat(pathname).st_mode)
     return mode_octal[-3:]
+
+
+def raise_if_bad_type(
+    value: Any,
+    type_: Type,
+    exception: type[Exception],
+    message_prefix: str,
+):
+    try:
+        check_type(value, type_)
+    except TypeCheckError as e:
+        raise exception(f"{message_prefix}: {e}")
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/chroot.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/chroot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,212 +1,203 @@
 import os
 from tempfile import mkstemp
 from typing import TYPE_CHECKING, Optional
 
 import click
+from typing_extensions import Unpack
 
 from pyinfra import local, logger
 from pyinfra.api import QuoteString, StringCommand
-from pyinfra.api.connectors import BaseConnectorMeta
 from pyinfra.api.exceptions import ConnectError, InventoryError, PyinfraError
 from pyinfra.api.util import get_file_io, memoize
 from pyinfra.progress import progress_spinner
 
-from .local import run_shell_command as run_local_shell_command
-from .util import make_unix_command_for_host
+from .base import BaseConnector
+from .local import LocalConnector
+from .util import extract_control_arguments, make_unix_command_for_host
 
 if TYPE_CHECKING:
+    from pyinfra.api.arguments import ConnectorArguments
     from pyinfra.api.host import Host
     from pyinfra.api.state import State
 
 
-class Meta(BaseConnectorMeta):
-    handles_execution = True
-
-
 @memoize
 def show_warning():
     logger.warning("The @chroot connector is in beta!")
 
 
-def make_names_data(directory: Optional[str] = None):
-    if not directory:
-        raise InventoryError("No directory provided!")
-
-    show_warning()
-
-    yield "@chroot/{0}".format(directory), {
-        "chroot_directory": "/{0}".format(directory.lstrip("/")),
-    }, ["@chroot"]
-
-
-def connect(state: "State", host: "Host"):
-    chroot_directory = host.data.chroot_directory
-
-    try:
-        with progress_spinner({"chroot run"}):
-            local.shell(
-                "chroot {0} ls".format(chroot_directory),
-                splitlines=True,
-            )
-    except PyinfraError as e:
-        raise ConnectError(e.args[0])
-
-    host.connector_data["chroot_directory"] = chroot_directory
-    return True
-
-
-def run_shell_command(
-    state: "State",
-    host: "Host",
-    command,
-    get_pty: bool = False,
-    timeout=None,
-    stdin=None,
-    success_exit_codes=None,
-    print_output: bool = False,
-    print_input: bool = False,
-    return_combined_output: bool = False,
-    **command_kwargs,
-):
-    chroot_directory = host.connector_data["chroot_directory"]
-
-    command = make_unix_command_for_host(state, host, command, **command_kwargs)
-    command = QuoteString(command)
-
-    logger.debug("--> Running chroot command on (%s): %s", chroot_directory, command)
-
-    chroot_command = StringCommand(
-        "chroot",
-        chroot_directory,
-        "sh",
-        "-c",
+class ChrootConnector(BaseConnector):
+    """
+    The chroot connector allows you to execute operations within another root.
+    """
+
+    handles_execution = True
+
+    local: LocalConnector
+
+    def __init__(self, state: "State", host: "Host"):
+        super().__init__(state, host)
+        self.local = LocalConnector(state, host)
+
+    @staticmethod
+    def make_names_data(name: Optional[str] = None):
+        if not name:
+            raise InventoryError("No directory provided!")
+
+        show_warning()
+
+        yield "@chroot/{0}".format(name), {
+            "chroot_directory": "/{0}".format(name.lstrip("/")),
+        }, ["@chroot"]
+
+    def connect(self) -> None:
+        self.local.connect()
+
+        chroot_directory = self.host.data.chroot_directory
+
+        try:
+            with progress_spinner({"chroot run"}):
+                local.shell(
+                    "chroot {0} ls".format(chroot_directory),
+                    splitlines=True,
+                )
+        except PyinfraError as e:
+            raise ConnectError(e.args[0])
+
+        self.host.connector_data["chroot_directory"] = chroot_directory
+
+    def run_shell_command(
+        self,
         command,
-    )
+        print_output: bool = False,
+        print_input: bool = False,
+        **command_arguments: Unpack["ConnectorArguments"],
+    ):
+        local_arguments = extract_control_arguments(command_arguments)
 
-    return run_local_shell_command(
-        state,
-        host,
-        chroot_command,
-        timeout=timeout,
-        stdin=stdin,
-        success_exit_codes=success_exit_codes,
-        print_output=print_output,
-        print_input=print_input,
-        return_combined_output=return_combined_output,
-    )
-
-
-def put_file(
-    state: "State",
-    host: "Host",
-    filename_or_io,
-    remote_filename,
-    remote_temp_filename=None,  # ignored
-    print_output: bool = False,
-    print_input: bool = False,
-    **kwargs,  # ignored (sudo/etc)
-):
-
-    _, temp_filename = mkstemp()
-
-    try:
-        # Load our file or IO object and write it to the temporary file
-        with get_file_io(filename_or_io) as file_io:
-            with open(temp_filename, "wb") as temp_f:
-                data = file_io.read()
-
-                if isinstance(data, str):
-                    data = data.encode()
+        chroot_directory = self.host.connector_data["chroot_directory"]
 
-                temp_f.write(data)
+        command = make_unix_command_for_host(self.state, self.host, command, **command_arguments)
+        command = QuoteString(command)
 
-        chroot_directory = host.connector_data["chroot_directory"]
+        logger.debug("--> Running chroot command on (%s): %s", chroot_directory, command)
 
-        chroot_command = "cp {0} {1}/{2}".format(
-            temp_filename,
+        chroot_command = StringCommand(
+            "chroot",
             chroot_directory,
-            remote_filename,
+            "sh",
+            "-c",
+            command,
         )
 
-        status, _, stderr = run_local_shell_command(
-            state,
-            host,
+        return self.local.run_shell_command(
             chroot_command,
             print_output=print_output,
             print_input=print_input,
+            **local_arguments,
         )
-    finally:
-        os.remove(temp_filename)
 
-    if not status:
-        raise IOError("\n".join(stderr))
+    def put_file(
+        self,
+        filename_or_io,
+        remote_filename,
+        remote_temp_filename=None,  # ignored
+        print_output: bool = False,
+        print_input: bool = False,
+        **kwargs,  # ignored (sudo/etc)
+    ):
+        _, temp_filename = mkstemp()
+
+        try:
+            # Load our file or IO object and write it to the temporary file
+            with get_file_io(filename_or_io) as file_io:
+                with open(temp_filename, "wb") as temp_f:
+                    data = file_io.read()
+
+                    if isinstance(data, str):
+                        data = data.encode()
+
+                    temp_f.write(data)
+
+            chroot_directory = self.host.connector_data["chroot_directory"]
+            chroot_command = StringCommand(
+                "cp",
+                temp_filename,
+                f"{chroot_directory}/{remote_filename}",
+            )
 
-    if print_output:
-        click.echo(
-            "{0}file uploaded to chroot: {1}".format(
-                host.print_prefix,
-                remote_filename,
-            ),
-            err=True,
-        )
+            status, output = self.local.run_shell_command(
+                chroot_command,
+                print_output=print_output,
+                print_input=print_input,
+            )
+        finally:
+            os.remove(temp_filename)
 
-    return status
+        if not status:
+            raise IOError(output.stderr)
 
+        if print_output:
+            click.echo(
+                "{0}file uploaded to chroot: {1}".format(
+                    self.host.print_prefix,
+                    remote_filename,
+                ),
+                err=True,
+            )
 
-def get_file(
-    state: "State",
-    host: "Host",
-    remote_filename,
-    filename_or_io,
-    remote_temp_filename=None,  # ignored
-    print_output: bool = False,
-    print_input: bool = False,
-    **kwargs,  # ignored (sudo/etc)
-):
-
-    _, temp_filename = mkstemp()
-
-    try:
-        chroot_directory = host.connector_data["chroot_directory"]
-        chroot_command = "cp {0}/{1} {2}".format(
-            chroot_directory,
-            remote_filename,
-            temp_filename,
-        )
+        return status
 
-        status, _, stderr = run_local_shell_command(
-            state,
-            host,
-            chroot_command,
-            print_output=print_output,
-            print_input=print_input,
-        )
+    def get_file(
+        self,
+        remote_filename,
+        filename_or_io,
+        remote_temp_filename=None,  # ignored
+        print_output: bool = False,
+        print_input: bool = False,
+        **kwargs,  # ignored (sudo/etc)
+    ):
+        _, temp_filename = mkstemp()
+
+        try:
+            chroot_directory = self.host.connector_data["chroot_directory"]
+            chroot_command = StringCommand(
+                "cp",
+                f"{chroot_directory}/{remote_filename}",
+                temp_filename,
+            )
 
-        # Load the temporary file and write it to our file or IO object
-        with open(temp_filename, encoding="utf-8") as temp_f:
-            with get_file_io(filename_or_io, "wb") as file_io:
-                data = temp_f.read()
-                data_bytes: bytes
-
-                if isinstance(data, str):
-                    data_bytes = data.encode()
-                else:
-                    data_bytes = data
-
-                file_io.write(data_bytes)
-    finally:
-        os.remove(temp_filename)
-
-    if not status:
-        raise IOError("\n".join(stderr))
-
-    if print_output:
-        click.echo(
-            "{0}file downloaded from chroot: {1}".format(
-                host.print_prefix,
-                remote_filename,
-            ),
-            err=True,
-        )
+            status, output = self.local.run_shell_command(
+                chroot_command,
+                print_output=print_output,
+                print_input=print_input,
+            )
+
+            # Load the temporary file and write it to our file or IO object
+            with open(temp_filename, encoding="utf-8") as temp_f:
+                with get_file_io(filename_or_io, "wb") as file_io:
+                    data = temp_f.read()
+                    data_bytes: bytes
+
+                    if isinstance(data, str):
+                        data_bytes = data.encode()
+                    else:
+                        data_bytes = data
+
+                    file_io.write(data_bytes)
+        finally:
+            os.remove(temp_filename)
+
+        if not status:
+            raise IOError(output.stderr)
+
+        if print_output:
+            click.echo(
+                "{0}file downloaded from chroot: {1}".format(
+                    self.host.print_prefix,
+                    remote_filename,
+                ),
+                err=True,
+            )
 
-    return status
+        return status
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/docker.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/docker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,305 +1,295 @@
-"""
-The ``@docker`` connector allows you to build Docker images, or modify running
-Docker containers, using ``pyinfra``. You can pass either an image name or
-existing container ID:
-
-+ Image - will create a container from the image, execute operations and save
-    into a new image
-+ Existing container ID - will simply execute operations against the container,
-    leaving it up afterwards
-
-
-.. code:: shell
-
-    # A Docker base image must be provided
-    pyinfra @docker/alpine:3.8 ...
-
-    # pyinfra can run on multiple Docker images in parallel
-    pyinfra @docker/alpine:3.8,@docker/ubuntu:bionic ...
-
-    # Execute against a running container
-    pyinfra @docker/2beb8c15a1b1 ...
-"""
+from __future__ import annotations
 
 import json
 import os
 from tempfile import mkstemp
 from typing import TYPE_CHECKING
 
 import click
+from typing_extensions import TypedDict, Unpack
 
 from pyinfra import local, logger
 from pyinfra.api import QuoteString, StringCommand
-from pyinfra.api.connectors import BaseConnectorMeta
 from pyinfra.api.exceptions import ConnectError, InventoryError, PyinfraError
 from pyinfra.api.util import get_file_io
 from pyinfra.progress import progress_spinner
 
-from .local import run_shell_command as run_local_shell_command
-from .util import make_unix_command_for_host
+from .base import BaseConnector, DataMeta
+from .local import LocalConnector
+from .util import CommandOutput, extract_control_arguments, make_unix_command_for_host
 
 if TYPE_CHECKING:
+    from pyinfra.api.arguments import ConnectorArguments
     from pyinfra.api.host import Host
     from pyinfra.api.state import State
 
 
-class Meta(BaseConnectorMeta):
-    handles_execution: bool = True
-    keys_prefix: str = "docker"
-
-    class DataKeys:
-        identifier = "ID of container or image to target"
-        container_id = "ID of container to target, overrides ``docker_identifier``"
-
-
-DATA_KEYS = Meta.keys()
-
+class ConnectorData(TypedDict):
+    docker_identifier: str
 
-def make_names_data(identifier=None):
-    if not identifier:
-        raise InventoryError("No docker base ID provided!")
 
-    yield (
-        "@docker/{0}".format(identifier),
-        {DATA_KEYS.identifier: identifier},
-        ["@docker"],
-    )
+connector_data_meta: dict[str, DataMeta] = {
+    "docker_identifier": DataMeta("ID of container or image to start from"),
+}
 
 
-def _find_start_docker_container(container_id):
+def _find_start_docker_container(container_id) -> tuple[str, bool]:
     docker_info = local.shell("docker container inspect {0}".format(container_id))
+    assert isinstance(docker_info, str)
     docker_info = json.loads(docker_info)[0]
     if docker_info["State"]["Running"] is False:
         logger.info("Starting stopped container: {0}".format(container_id))
         local.shell("docker container start {0}".format(container_id))
+        return container_id, False
+    return container_id, True
 
 
 def _start_docker_image(image_name):
     try:
         return local.shell(
             "docker run -d {0} tail -f /dev/null".format(image_name),
             splitlines=True,
         )[
             -1
         ]  # last line is the container ID
     except PyinfraError as e:
         raise ConnectError(e.args[0])
 
 
-def connect(state: "State", host: "Host"):
-    docker_container_id = host.data.get(DATA_KEYS.container_id)
-    if docker_container_id:  # user can provide a docker_container_id
-        host.connector_data["docker_container_no_disconnect"] = True
-        host.connector_data["docker_container_id"] = docker_container_id
-        return True
+class DockerConnector(BaseConnector):
+    """
+    The docker connector allows you to build Docker images or modify running
+    Docker containers. You can pass either an image name or existing container ID:
 
-    docker_identifier = getattr(host.data, DATA_KEYS.identifier)
-    with progress_spinner({"prepare docker container"}):
-        try:
-            # Check if the provided @docker/X is an existing container ID
-            _find_start_docker_container(docker_identifier)
-        except PyinfraError:
-            container_id = _start_docker_image(docker_identifier)
-        else:
-            container_id = docker_identifier
-            host.connector_data["docker_container_no_disconnect"] = True
+    + Image - will create a new container from the image, execute operations \
+        against it, save into a new Docker image and remove the container
+    + Existing container ID - will execute operations against the running \
+        container, leaving it running
 
-    host.connector_data["docker_container_id"] = container_id
-    return True
+    .. code:: shell
 
+        # A Docker base image must be provided
+        pyinfra @docker/alpine:3.8 ...
 
-def disconnect(state, host):
-    container_id = host.connector_data["docker_container_id"]
+        # pyinfra can run on multiple Docker images in parallel
+        pyinfra @docker/alpine:3.8,@docker/ubuntu:bionic ...
 
-    if host.connector_data.get("docker_container_no_disconnect"):
-        logger.info(
-            "{0}docker build complete, container left running: {1}".format(
-                host.print_prefix,
-                click.style(container_id, bold=True),
-            ),
-        )
-        return
+        # Execute against a running container
+        pyinfra @docker/2beb8c15a1b1 ...
+    """
+
+    handles_execution = True
 
-    with progress_spinner({"docker commit"}):
-        image_id = local.shell("docker commit {0}".format(container_id), splitlines=True)[-1][
-            7:19
-        ]  # last line is the image ID, get sha256:[XXXXXXXXXX]...
-
-    with progress_spinner({"docker rm"}):
-        local.shell(
-            "docker rm -f {0}".format(container_id),
+    data_cls = ConnectorData
+    data_meta = connector_data_meta
+    data: ConnectorData
+
+    local: LocalConnector
+
+    container_id: str
+    no_stop: bool = False
+
+    def __init__(self, state: "State", host: "Host"):
+        super().__init__(state, host)
+        self.local = LocalConnector(state, host)
+
+    @staticmethod
+    def make_names_data(name=None):
+        if not name:
+            raise InventoryError("No docker base ID provided!")
+
+        yield (
+            "@docker/{0}".format(name),
+            {"docker_identifier": name},
+            ["@docker"],
         )
 
-    logger.info(
-        "{0}docker build complete, image ID: {1}".format(
-            host.print_prefix,
-            click.style(image_id, bold=True),
-        ),
-    )
-
-
-def run_shell_command(
-    state: "State",
-    host: "Host",
-    command,
-    get_pty=False,
-    timeout=None,
-    stdin=None,
-    success_exit_codes=None,
-    print_output=False,
-    print_input=False,
-    return_combined_output=False,
-    **command_kwargs,
-):
-    container_id = host.connector_data["docker_container_id"]
-
-    command = make_unix_command_for_host(state, host, command, **command_kwargs)
-    command = QuoteString(command)
-
-    docker_flags = "-it" if get_pty else "-i"
-    docker_command = StringCommand(
-        "docker",
-        "exec",
-        docker_flags,
-        container_id,
-        "sh",
-        "-c",
-        command,
-    )
-
-    return run_local_shell_command(
-        state,
-        host,
-        docker_command,
-        timeout=timeout,
-        stdin=stdin,
-        success_exit_codes=success_exit_codes,
-        print_output=print_output,
-        print_input=print_input,
-        return_combined_output=return_combined_output,
-    )
-
-
-def put_file(
-    state: "State",
-    host: "Host",
-    filename_or_io,
-    remote_filename,
-    remote_temp_filename=None,  # ignored
-    print_output=False,
-    print_input=False,
-    **kwargs,  # ignored (sudo/etc)
-):
-    """
-    Upload a file/IO object to the target Docker container by copying it to a
-    temporary location and then uploading it into the container using ``docker cp``.
-    """
+    def connect(self) -> None:
+        self.local.connect()
 
-    fd, temp_filename = mkstemp()
+        docker_identifier = self.data["docker_identifier"]
+        with progress_spinner({"prepare docker container"}):
+            try:
+                self.container_id, was_running = _find_start_docker_container(docker_identifier)
+                if was_running:
+                    self.no_stop = True
+            except PyinfraError:
+                self.container_id = _start_docker_image(docker_identifier)
+
+    def disconnect(self):
+        container_id = self.container_id
+
+        if self.no_stop:
+            logger.info(
+                "{0}docker build complete, container left running: {1}".format(
+                    self.host.print_prefix,
+                    click.style(container_id, bold=True),
+                ),
+            )
+            return
+
+        with progress_spinner({"docker commit"}):
+            image_id = local.shell("docker commit {0}".format(container_id), splitlines=True)[-1][
+                7:19
+            ]  # last line is the image ID, get sha256:[XXXXXXXXXX]...
+
+        with progress_spinner({"docker rm"}):
+            local.shell(
+                "docker rm -f {0}".format(container_id),
+            )
 
-    try:
-        # Load our file or IO object and write it to the temporary file
-        with get_file_io(filename_or_io) as file_io:
-            with open(temp_filename, "wb") as temp_f:
-                data = file_io.read()
-
-                if isinstance(data, str):
-                    data = data.encode()
-
-                temp_f.write(data)
-
-        docker_id = host.connector_data["docker_container_id"]
-        docker_command = "docker cp {0} {1}:{2}".format(
-            temp_filename,
-            docker_id,
-            remote_filename,
+        logger.info(
+            "{0}docker build complete, image ID: {1}".format(
+                self.host.print_prefix,
+                click.style(image_id, bold=True),
+            ),
         )
 
-        status, _, stderr = run_local_shell_command(
-            state,
-            host,
+    def run_shell_command(
+        self,
+        command: StringCommand,
+        print_output: bool = False,
+        print_input: bool = False,
+        **arguments: Unpack["ConnectorArguments"],
+    ) -> tuple[bool, CommandOutput]:
+        local_arguments = extract_control_arguments(arguments)
+
+        container_id = self.container_id
+
+        command = make_unix_command_for_host(self.state, self.host, command, **arguments)
+        command = StringCommand(QuoteString(command))
+
+        docker_flags = "-it" if local_arguments.get("_get_pty") else "-i"
+        docker_command = StringCommand(
+            "docker",
+            "exec",
+            docker_flags,
+            container_id,
+            "sh",
+            "-c",
+            command,
+        )
+
+        return self.local.run_shell_command(
             docker_command,
             print_output=print_output,
             print_input=print_input,
+            **local_arguments,
         )
-    finally:
-        os.close(fd)
-        os.remove(temp_filename)
-
-    if not status:
-        raise IOError("\n".join(stderr))
-
-    if print_output:
-        click.echo(
-            "{0}file uploaded to container: {1}".format(
-                host.print_prefix,
-                remote_filename,
-            ),
-            err=True,
-        )
-
-    return status
-
 
-def get_file(
-    state: "State",
-    host: "Host",
-    remote_filename,
-    filename_or_io,
-    remote_temp_filename=None,  # ignored
-    print_output=False,
-    print_input=False,
-    **kwargs,  # ignored (sudo/etc)
-):
-    """
-    Download a file from the target Docker container by copying it to a temporary
-    location and then reading that into our final file/IO object.
-    """
+    def put_file(
+        self,
+        filename_or_io,
+        remote_filename,
+        remote_temp_filename=None,  # ignored
+        print_output=False,
+        print_input=False,
+        **kwargs,  # ignored (sudo/etc)
+    ) -> bool:
+        """
+        Upload a file/IO object to the target Docker container by copying it to a
+        temporary location and then uploading it into the container using ``docker cp``.
+        """
 
-    fd, temp_filename = mkstemp()
+        fd, temp_filename = mkstemp()
 
-    try:
-        docker_id = host.connector_data["docker_container_id"]
-        docker_command = "docker cp {0}:{1} {2}".format(
-            docker_id,
-            remote_filename,
-            temp_filename,
-        )
+        try:
+            # Load our file or IO object and write it to the temporary file
+            with get_file_io(filename_or_io) as file_io:
+                with open(temp_filename, "wb") as temp_f:
+                    data = file_io.read()
+
+                    if isinstance(data, str):
+                        data = data.encode()
+
+                    temp_f.write(data)
+
+            docker_command = StringCommand(
+                "docker",
+                "cp",
+                temp_filename,
+                f"{self.container_id}:{remote_filename}",
+            )
+
+            status, output = self.local.run_shell_command(
+                docker_command,
+                print_output=print_output,
+                print_input=print_input,
+            )
+        finally:
+            os.close(fd)
+            os.remove(temp_filename)
+
+        if not status:
+            raise IOError(output.stderr)
+
+        if print_output:
+            click.echo(
+                "{0}file uploaded to container: {1}".format(
+                    self.host.print_prefix,
+                    remote_filename,
+                ),
+                err=True,
+            )
+
+        return status
+
+    def get_file(
+        self,
+        remote_filename,
+        filename_or_io,
+        remote_temp_filename=None,  # ignored
+        print_output=False,
+        print_input=False,
+        **kwargs,  # ignored (sudo/etc)
+    ) -> bool:
+        """
+        Download a file from the target Docker container by copying it to a temporary
+        location and then reading that into our final file/IO object.
+        """
 
-        status, _, stderr = run_local_shell_command(
-            state,
-            host,
-            docker_command,
-            print_output=print_output,
-            print_input=print_input,
-        )
+        fd, temp_filename = mkstemp()
 
-        # Load the temporary file and write it to our file or IO object
-        with open(temp_filename, encoding="utf-8") as temp_f:
-            with get_file_io(filename_or_io, "wb") as file_io:
-                data = temp_f.read()
-                data_bytes: bytes
-
-                if isinstance(data, str):
-                    data_bytes = data.encode()
-                else:
-                    data_bytes = data
-
-                file_io.write(data_bytes)
-    finally:
-        os.close(fd)
-        os.remove(temp_filename)
-
-    if not status:
-        raise IOError("\n".join(stderr))
-
-    if print_output:
-        click.echo(
-            "{0}file downloaded from container: {1}".format(
-                host.print_prefix,
-                remote_filename,
-            ),
-            err=True,
-        )
+        try:
+            docker_command = StringCommand(
+                "docker",
+                "cp",
+                f"{self.container_id}:{remote_filename}",
+                temp_filename,
+            )
+
+            status, output = self.local.run_shell_command(
+                docker_command,
+                print_output=print_output,
+                print_input=print_input,
+            )
+
+            # Load the temporary file and write it to our file or IO object
+            with open(temp_filename, encoding="utf-8") as temp_f:
+                with get_file_io(filename_or_io, "wb") as file_io:
+                    data = temp_f.read()
+                    data_bytes: bytes
+
+                    if isinstance(data, str):
+                        data_bytes = data.encode()
+                    else:
+                        data_bytes = data
+
+                    file_io.write(data_bytes)
+        finally:
+            os.close(fd)
+            os.remove(temp_filename)
+
+        if not status:
+            raise IOError(output.stderr)
+
+        if print_output:
+            click.echo(
+                "{0}file downloaded from container: {1}".format(
+                    self.host.print_prefix,
+                    remote_filename,
+                ),
+                err=True,
+            )
 
-    return status
+        return status
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/dockerssh.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/dockerssh.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,313 +1,291 @@
-"""
-**Note**: this connector is in beta!
-
-The ``@dockerssh`` connector allows you to run commands on Docker containers on a remote machine.
-
-.. code:: shell
-
-    # A Docker base image must be provided
-    pyinfra @dockerssh/remotehost:alpine:3.8 ...
-
-    # pyinfra can run on multiple Docker images in parallel
-    pyinfra @dockerssh/remotehost:alpine:3.8,@dockerssh/remotehost:ubuntu:bionic ...
-"""
-
 import os
 from tempfile import mkstemp
 from typing import TYPE_CHECKING
 
 import click
+from typing_extensions import Unpack
 
 from pyinfra import logger
 from pyinfra.api import QuoteString, StringCommand
-from pyinfra.api.connectors import BaseConnectorMeta
 from pyinfra.api.exceptions import ConnectError, InventoryError, PyinfraError
 from pyinfra.api.util import get_file_io, memoize
 from pyinfra.progress import progress_spinner
 
-from . import ssh
-from .util import make_unix_command_for_host
+from .base import BaseConnector
+from .ssh import SSHConnector
+from .util import extract_control_arguments, make_unix_command_for_host
 
 if TYPE_CHECKING:
+    from pyinfra.api.arguments import ConnectorArguments
     from pyinfra.api.host import Host
     from pyinfra.api.state import State
 
 
-class Meta(BaseConnectorMeta):
-    handles_execution = True
+@memoize
+def show_warning():
+    logger.warning("The @dockerssh connector is in beta!")
 
 
-def remote_remove(
-    state: "State", host: "Host", filename, print_output: bool = False, print_input: bool = False
-):
+class DockerSSHConnector(BaseConnector):
     """
-    Deletes a file on a remote machine over ssh.
-    """
-    remove_status, _, remove_stderr = ssh.run_shell_command(
-        state,
-        host,
-        "rm -f {0}".format(filename),
-        print_output=print_output,
-        print_input=print_input,
-    )
+    **Note**: this connector is in beta!
 
-    if not remove_status:
-        raise IOError("\n".join(remove_stderr))
+    The ``@dockerssh`` connector allows you to run commands on Docker containers \
+    on a remote machine.
 
+    .. code:: shell
 
-@memoize
-def show_warning():
-    logger.warning("The @dockerssh connector is in beta!")
+        # A Docker base image must be provided
+        pyinfra @dockerssh/remotehost:alpine:3.8 ...
 
+        # pyinfra can run on multiple Docker images in parallel
+        pyinfra @dockerssh/remotehost:alpine:3.8,@dockerssh/remotehost:ubuntu:bionic ...
+    """
 
-def make_names_data(host_image_str):
-    try:
-        hostname, image = host_image_str.split(":", 1)
-    except (AttributeError, ValueError):  # failure to parse the host_image_str
-        raise InventoryError("No ssh host or docker base image provided!")
-
-    if not image:
-        raise InventoryError("No docker base image provided!")
-
-    show_warning()
-
-    yield (
-        "@dockerssh/{0}:{1}".format(hostname, image),
-        {"ssh_hostname": hostname, "docker_image": image},
-        ["@dockerssh"],
-    )
-
-
-def connect(state: "State", host: "Host"):
-    if not host.connection:
-        host.connection = ssh.connect(state, host)
-
-    if "docker_container_id" in host.host_data:  # user can provide a docker_container_id
-        return host.connection
-
-    try:
-        with progress_spinner({"docker run"}):
-            # last line is the container ID
-            status, stdout, stderr = ssh.run_shell_command(
-                state,
-                host,
-                "docker run -d {0} tail -f /dev/null".format(host.data.docker_image),
-            )
-            if not status:
-                raise IOError("\n".join(stderr))
-            container_id = stdout[-1]
-
-    except PyinfraError as e:
-        host.connection = None  # fail connection
-        raise ConnectError(e.args[0])
-
-    host.host_data["docker_container_id"] = container_id
-    return host.connection
-
-
-def disconnect(state: "State", host: "Host"):
-    container_id = host.host_data["docker_container_id"][:12]
-
-    with progress_spinner({"docker commit"}):
-        image_id = ssh.run_shell_command(state, host, "docker commit {0}".format(container_id))[1][
-            -1
-        ][
-            7:19
-        ]  # last line is the image ID, get sha256:[XXXXXXXXXX]...
-
-    with progress_spinner({"docker rm"}):
-        ssh.run_shell_command(
-            state,
-            host,
-            "docker rm -f {0}".format(container_id),
+    handles_execution = True
+
+    ssh: SSHConnector
+
+    def __init__(self, state: "State", host: "Host"):
+        super().__init__(state, host)
+        self.ssh = SSHConnector(state, host)
+
+    @staticmethod
+    def make_names_data(name):
+        try:
+            hostname, image = name.split(":", 1)
+        except (AttributeError, ValueError):  # failure to parse the name
+            raise InventoryError("No ssh host or docker base image provided!")
+
+        if not image:
+            raise InventoryError("No docker base image provided!")
+
+        show_warning()
+
+        yield (
+            "@dockerssh/{0}:{1}".format(hostname, image),
+            {"ssh_hostname": hostname, "docker_image": image},
+            ["@dockerssh"],
         )
 
-    logger.info(
-        "{0}docker build complete, image ID: {1}".format(
-            host.print_prefix,
-            click.style(image_id, bold=True),
-        ),
-    )
-
-
-def run_shell_command(
-    state: "State",
-    host: "Host",
-    command,
-    get_pty: bool = False,
-    timeout=None,
-    stdin=None,
-    success_exit_codes=None,
-    print_output: bool = False,
-    print_input: bool = False,
-    return_combined_output=False,
-    **command_kwargs,
-):
-    container_id = host.host_data["docker_container_id"]
-
-    # Don't sudo/su in Docker - is this the right thing to do? Makes deploys that
-    # target SSH systems work w/Docker out of the box (ie most docker commands
-    # are run as root).
-    for key in ("sudo", "su_user"):
-        command_kwargs.pop(key, None)
-
-    command = make_unix_command_for_host(state, host, command, **command_kwargs)
-    command = QuoteString(command)
-
-    docker_flags = "-it" if get_pty else "-i"
-    docker_command = StringCommand(
-        "docker",
-        "exec",
-        docker_flags,
-        container_id,
-        "sh",
-        "-c",
-        command,
-    )
+    def connect(self) -> None:
+        self.ssh.connect()
 
-    return ssh.run_shell_command(
-        state,
-        host,
-        docker_command,
-        timeout=timeout,
-        stdin=stdin,
-        success_exit_codes=success_exit_codes,
-        print_output=print_output,
-        print_input=print_input,
-        return_combined_output=return_combined_output,
-    )
-
-
-def put_file(
-    state: "State",
-    host: "Host",
-    filename_or_io,
-    remote_filename,
-    remote_temp_filename=None,
-    print_output: bool = False,
-    print_input: bool = False,
-    **kwargs,  # ignored (sudo/etc)
-):
-    """
-    Upload a file/IO object to the target Docker container by copying it to a
-    temporary location and then uploading it into the container using ``docker cp``.
-    """
+        if "docker_container_id" in self.host.host_data:  # user can provide a docker_container_id
+            return
 
-    fd, local_temp_filename = mkstemp()
-    remote_temp_filename = remote_temp_filename or state.get_temp_filename(local_temp_filename)
+        try:
+            with progress_spinner({"docker run"}):
+                # last line is the container ID
+                status, output = self.ssh.run_shell_command(
+                    StringCommand(
+                        "docker",
+                        "run",
+                        "-d",
+                        self.host.data.docker_image,
+                        "tail",
+                        "-f",
+                        "/dev/null",
+                    ),
+                )
+                if not status:
+                    raise IOError(output.stderr)
+                container_id = output.stdout_lines[-1]
+
+        except PyinfraError as e:
+            raise ConnectError(e.args[0])
+
+        self.host.host_data["docker_container_id"] = container_id
+
+    def disconnect(self) -> None:
+        container_id = self.host.host_data["docker_container_id"][:12]
+
+        with progress_spinner({"docker commit"}):
+            _, output = self.ssh.run_shell_command(StringCommand("docker", "commit", container_id))
+
+            # Last line is the image ID, get sha256:[XXXXXXXXXX]...
+            image_id = output.stdout_lines[-1][7:19]
+
+        with progress_spinner({"docker rm"}):
+            self.ssh.run_shell_command(
+                StringCommand("docker", "rm", "-f", container_id),
+            )
+
+        logger.info(
+            "{0}docker build complete, image ID: {1}".format(
+                self.host.print_prefix,
+                click.style(image_id, bold=True),
+            ),
+        )
 
-    # Load our file or IO object and write it to the temporary file
-    with get_file_io(filename_or_io) as file_io:
-        with open(local_temp_filename, "wb") as temp_f:
-            data = file_io.read()
-
-            if isinstance(data, str):
-                data = data.encode()
-
-            temp_f.write(data)
-
-    # upload file to remote server
-    ssh_status = ssh.put_file(state, host, local_temp_filename, remote_temp_filename)
-    if not ssh_status:
-        raise IOError("Failed to copy file over ssh")
-
-    try:
-        docker_id = host.host_data["docker_container_id"]
-        docker_command = "docker cp {0} {1}:{2}".format(
-            remote_temp_filename,
-            docker_id,
-            remote_filename,
+    def run_shell_command(
+        self,
+        command,
+        print_output: bool = False,
+        print_input: bool = False,
+        **arguments: Unpack["ConnectorArguments"],
+    ):
+        local_arguments = extract_control_arguments(arguments)
+
+        container_id = self.host.host_data["docker_container_id"]
+
+        command = make_unix_command_for_host(self.state, self.host, command, **arguments)
+        command = QuoteString(command)
+
+        docker_flags = "-it" if local_arguments.get("_get_pty") else "-i"
+        docker_command = StringCommand(
+            "docker",
+            "exec",
+            docker_flags,
+            container_id,
+            "sh",
+            "-c",
+            command,
         )
 
-        status, _, stderr = ssh.run_shell_command(
-            state,
-            host,
+        return self.ssh.run_shell_command(
             docker_command,
             print_output=print_output,
             print_input=print_input,
+            **local_arguments,
         )
-    finally:
-        os.close(fd)
-        os.remove(local_temp_filename)
-        remote_remove(
-            state,
-            host,
-            local_temp_filename,
-            print_output=print_output,
-            print_input=print_input,
+
+    def put_file(
+        self,
+        filename_or_io,
+        remote_filename,
+        remote_temp_filename=None,
+        print_output: bool = False,
+        print_input: bool = False,
+        **kwargs,  # ignored (sudo/etc)
+    ):
+        """
+        Upload a file/IO object to the target Docker container by copying it to a
+        temporary location and then uploading it into the container using ``docker cp``.
+        """
+
+        fd, local_temp_filename = mkstemp()
+        remote_temp_filename = remote_temp_filename or self.host.get_temp_filename(
+            local_temp_filename
         )
 
-    if not status:
-        raise IOError("\n".join(stderr))
+        # Load our file or IO object and write it to the temporary file
+        with get_file_io(filename_or_io) as file_io:
+            with open(local_temp_filename, "wb") as temp_f:
+                data = file_io.read()
+
+                if isinstance(data, str):
+                    data = data.encode()
+
+                temp_f.write(data)
+
+        # upload file to remote server
+        ssh_status = self.ssh.put_file(local_temp_filename, remote_temp_filename)
+        if not ssh_status:
+            raise IOError("Failed to copy file over ssh")
+
+        try:
+            docker_id = self.host.host_data["docker_container_id"]
+            docker_command = StringCommand(
+                "docker",
+                "cp",
+                remote_temp_filename,
+                f"{docker_id}:{remote_filename}",
+            )
 
-    if print_output:
-        click.echo(
-            "{0}file uploaded to container: {1}".format(
-                host.print_prefix,
-                remote_filename,
-            ),
-            err=True,
-        )
+            status, output = self.ssh.run_shell_command(
+                docker_command,
+                print_output=print_output,
+                print_input=print_input,
+            )
+        finally:
+            os.close(fd)
+            os.remove(local_temp_filename)
+            self.remote_remove(
+                local_temp_filename,
+                print_output=print_output,
+                print_input=print_input,
+            )
 
-    return status
+        if not status:
+            raise IOError(output.stderr)
 
+        if print_output:
+            click.echo(
+                "{0}file uploaded to container: {1}".format(
+                    self.host.print_prefix,
+                    remote_filename,
+                ),
+                err=True,
+            )
 
-def get_file(
-    state: "State",
-    host: "Host",
-    remote_filename,
-    filename_or_io,
-    remote_temp_filename=None,
-    print_output: bool = False,
-    print_input: bool = False,
-    **kwargs,  # ignored (sudo/etc)
-):
-    """
-    Download a file from the target Docker container by copying it to a temporary
-    location and then reading that into our final file/IO object.
-    """
+        return status
 
-    remote_temp_filename = remote_temp_filename or state.get_temp_filename(remote_filename)
+    def get_file(
+        self,
+        remote_filename,
+        filename_or_io,
+        remote_temp_filename=None,
+        print_output: bool = False,
+        print_input: bool = False,
+        **kwargs,  # ignored (sudo/etc)
+    ):
+        """
+        Download a file from the target Docker container by copying it to a temporary
+        location and then reading that into our final file/IO object.
+        """
+
+        remote_temp_filename = remote_temp_filename or self.host.get_temp_filename(remote_filename)
+
+        try:
+            docker_id = self.host.host_data["docker_container_id"]
+            docker_command = StringCommand(
+                "docker",
+                "cp",
+                f"{docker_id}:{remote_filename}",
+                remote_temp_filename,
+            )
 
-    try:
-        docker_id = host.host_data["docker_container_id"]
-        docker_command = "docker cp {0}:{1} {2}".format(
-            docker_id,
-            remote_filename,
-            remote_temp_filename,
-        )
+            status, output = self.ssh.run_shell_command(
+                docker_command,
+                print_output=print_output,
+                print_input=print_input,
+            )
 
-        status, _, stderr = ssh.run_shell_command(
-            state,
-            host,
-            docker_command,
-            print_output=print_output,
-            print_input=print_input,
-        )
+            ssh_status = self.ssh.get_file(remote_temp_filename, filename_or_io)
+        finally:
+            self.remote_remove(
+                remote_temp_filename,
+                print_output=print_output,
+                print_input=print_input,
+            )
 
-        ssh_status = ssh.get_file(state, host, remote_temp_filename, filename_or_io)
-    finally:
-        remote_remove(
-            state,
-            host,
-            remote_temp_filename,
-            print_output=print_output,
-            print_input=print_input,
-        )
+        if not ssh_status:
+            raise IOError("failed to copy file over ssh")
 
-    if not ssh_status:
-        raise IOError("failed to copy file over ssh")
+        if not status:
+            raise IOError(output.stderr)
 
-    if not status:
-        raise IOError("\n".join(stderr))
+        if print_output:
+            click.echo(
+                "{0}file downloaded from container: {1}".format(
+                    self.host.print_prefix,
+                    remote_filename,
+                ),
+                err=True,
+            )
 
-    if print_output:
-        click.echo(
-            "{0}file downloaded from container: {1}".format(
-                host.print_prefix,
-                remote_filename,
-            ),
-            err=True,
+        return status
+
+    def remote_remove(self, filename, print_output: bool = False, print_input: bool = False):
+        """
+        Deletes a file on a remote machine over ssh.
+        """
+        remove_status, output = self.ssh.run_shell_command(
+            StringCommand("rm", "-f", filename),
+            print_output=print_output,
+            print_input=print_input,
         )
 
-    return status
+        if not remove_status:
+            raise IOError(output.stderr)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/local.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/local.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,244 +1,232 @@
-"""
-The ``@local`` connector executes changes on the local machine using subprocesses.
-"""
-
 import os
 from distutils.spawn import find_executable
 from tempfile import mkstemp
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Tuple
 
 import click
+from typing_extensions import Unpack
 
 from pyinfra import logger
 from pyinfra.api.command import QuoteString, StringCommand
-from pyinfra.api.connectors import BaseConnectorMeta
 from pyinfra.api.exceptions import InventoryError
 from pyinfra.api.util import get_file_io
 
+from .base import BaseConnector
 from .util import (
+    CommandOutput,
     execute_command_with_sudo_retry,
     make_unix_command_for_host,
     run_local_process,
-    split_combined_output,
 )
 
 if TYPE_CHECKING:
-    from pyinfra.api.host import Host
-    from pyinfra.api.state import State
-
-
-class Meta(BaseConnectorMeta):
-    handles_execution = True
+    from pyinfra.api.arguments import ConnectorArguments
 
 
-def make_names_data(_=None):
-    if _ is not None:
-        raise InventoryError("Cannot have more than one @local")
-
-    yield "@local", {}, ["@local"]
-
-
-def connect(state: "State", host: "Host"):
-    return True
-
-
-def run_shell_command(
-    state: "State",
-    host: "Host",
-    command,
-    get_pty: bool = False,  # ignored
-    timeout=None,
-    stdin=None,
-    success_exit_codes=None,
-    print_output: bool = False,
-    print_input: bool = False,
-    return_combined_output: bool = False,
-    **command_kwargs,
-):
+class LocalConnector(BaseConnector):
     """
-    Execute a command on the local machine.
+    The ``@local`` connector executes changes on the local machine using
+    subprocesses. **This connector is only compatible with MacOS & Linux hosts**.
 
-    Args:
-        state (``pyinfra.api.State`` object): state object for this command
-        host (``pyinfra.api.Host`` object): the target host
-        command (string): actual command to execute
-        sudo (boolean): whether to wrap the command with sudo
-        sudo_user (string): user to sudo to
-        env (dict): environment variables to set
-        timeout (int): timeout for this command to complete before erroring
-
-    Returns:
-        tuple: (exit_code, stdout, stderr)
-        stdout and stderr are both lists of strings from each buffer.
-    """
-
-    def execute_command():
-        unix_command = make_unix_command_for_host(state, host, command, **command_kwargs)
-        actual_command = unix_command.get_raw_value()
-
-        logger.debug("--> Running command on localhost: %s", unix_command)
-
-        if print_input:
-            click.echo("{0}>>> {1}".format(host.print_prefix, unix_command), err=True)
-
-        return run_local_process(
-            actual_command,
-            stdin=stdin,
-            timeout=timeout,
-            print_output=print_output,
-            print_prefix=host.print_prefix,
-        )
+    Examples:
 
-    return_code, combined_output = execute_command_with_sudo_retry(
-        host,
-        command_kwargs,
-        execute_command,
-    )
-
-    if success_exit_codes:
-        status = return_code in success_exit_codes
-    else:
-        status = return_code == 0
+    .. code::
 
-    if return_combined_output:
-        return status, combined_output
-
-    stdout, stderr = split_combined_output(combined_output)
-    return status, stdout, stderr
-
-
-def put_file(
-    state: "State",
-    host: "Host",
-    filename_or_io,
-    remote_filename,
-    remote_temp_filename=None,  # ignored
-    print_output: bool = False,
-    print_input: bool = False,
-    **command_kwargs,
-):
+        # Install nginx
+        pyinfra inventory.py apt.packages nginx update=true _sudo=true
     """
-    Upload a local file or IO object by copying it to a temporary directory
-    and then writing it to the upload location.
-    """
-
-    _, temp_filename = mkstemp()
 
-    try:
-        # Load our file or IO object and write it to the temporary file
-        with get_file_io(filename_or_io) as file_io:
-            with open(temp_filename, "wb") as temp_f:
-                data = file_io.read()
-
-                if isinstance(data, str):
-                    data = data.encode()
-
-                temp_f.write(data)
-
-        # Copy the file using `cp` such that we support sudo/su
-        status, _, stderr = run_shell_command(
-            state,
-            host,
-            StringCommand("cp", temp_filename, QuoteString(remote_filename)),
-            print_output=print_output,
-            print_input=print_input,
-            **command_kwargs,
-        )
+    handles_execution = True
 
-        if not status:
-            raise IOError("\n".join(stderr))
-    finally:
-        os.remove(temp_filename)
-
-    if print_output:
-        click.echo(
-            "{0}file copied: {1}".format(host.print_prefix, remote_filename),
-            err=True,
+    @staticmethod
+    def make_names_data(name=None):
+        if name is not None:
+            raise InventoryError("Cannot have more than one @local")
+
+        yield "@local", {}, ["@local"]
+
+    def run_shell_command(
+        self,
+        command: StringCommand,
+        print_output: bool = False,
+        print_input: bool = False,
+        **arguments: Unpack["ConnectorArguments"],
+    ) -> Tuple[bool, CommandOutput]:
+        """
+        Execute a command on the local machine.
+
+        Args:
+            command (StringCommand): actual command to execute
+            print_output (bool): whether to print command output
+            print_input (bool): whether to print command input
+            arguments: (ConnectorArguments): connector global arguments
+
+        Returns:
+            tuple: (bool, CommandOutput)
+            Bool indicating success and CommandOutput with stdout/stderr lines.
+        """
+
+        arguments.pop("_get_pty", False)
+        _timeout = arguments.pop("_timeout", None)
+        _stdin = arguments.pop("_stdin", None)
+        _success_exit_codes = arguments.pop("_success_exit_codes", None)
+
+        def execute_command() -> Tuple[int, CommandOutput]:
+            unix_command = make_unix_command_for_host(self.state, self.host, command, **arguments)
+            actual_command = unix_command.get_raw_value()
+
+            logger.debug("--> Running command on localhost: %s", unix_command)
+
+            if print_input:
+                click.echo("{0}>>> {1}".format(self.host.print_prefix, unix_command), err=True)
+
+            return run_local_process(
+                actual_command,
+                stdin=_stdin,
+                timeout=_timeout,
+                print_output=print_output,
+                print_prefix=self.host.print_prefix,
+            )
+
+        return_code, combined_output = execute_command_with_sudo_retry(
+            self.host,
+            arguments,
+            execute_command,
         )
 
-    return status
-
-
-def get_file(
-    state: "State",
-    host: "Host",
-    remote_filename,
-    filename_or_io,
-    remote_temp_filename=None,  # ignored
-    print_output: bool = False,
-    print_input: bool = False,
-    **command_kwargs,
-):
-    """
-    Download a local file by copying it to a temporary location and then writing
-    it to our filename or IO object.
-    """
+        if _success_exit_codes:
+            status = return_code in _success_exit_codes
+        else:
+            status = return_code == 0
 
-    _, temp_filename = mkstemp()
+        return status, combined_output
 
-    try:
-        # Copy the file using `cp` such that we support sudo/su
-        status, _, stderr = run_shell_command(
-            state,
-            host,
-            "cp {0} {1}".format(remote_filename, temp_filename),
+    def put_file(
+        self,
+        filename_or_io,
+        remote_filename,
+        remote_temp_filename=None,  # ignored
+        print_output: bool = False,
+        print_input: bool = False,
+        **arguments,
+    ) -> bool:
+        """
+        Upload a local file or IO object by copying it to a temporary directory
+        and then writing it to the upload location.
+
+        Returns:
+            bool: Indicating success or failure
+        """
+
+        _, temp_filename = mkstemp()
+
+        try:
+            # Load our file or IO object and write it to the temporary file
+            with get_file_io(filename_or_io) as file_io:
+                with open(temp_filename, "wb") as temp_f:
+                    data = file_io.read()
+
+                    if isinstance(data, str):
+                        data = data.encode()
+
+                    temp_f.write(data)
+
+            # Copy the file using `cp` such that we support sudo/su
+            status, output = self.run_shell_command(
+                StringCommand("cp", temp_filename, QuoteString(remote_filename)),
+                print_output=print_output,
+                print_input=print_input,
+                **arguments,
+            )
+
+            if not status:
+                raise IOError(output.stderr)
+        finally:
+            os.remove(temp_filename)
+
+        if print_output:
+            click.echo(
+                "{0}file copied: {1}".format(self.host.print_prefix, remote_filename),
+                err=True,
+            )
+
+        return status
+
+    def get_file(
+        self,
+        remote_filename,
+        filename_or_io,
+        remote_temp_filename=None,  # ignored
+        print_output: bool = False,
+        print_input: bool = False,
+        **arguments,
+    ) -> bool:
+        """
+        Download a local file by copying it to a temporary location and then writing
+        it to our filename or IO object.
+
+        Returns:
+            bool: Indicating success or failure
+        """
+
+        _, temp_filename = mkstemp()
+
+        try:
+            # Copy the file using `cp` such that we support sudo/su
+            status, output = self.run_shell_command(
+                StringCommand("cp", remote_filename, temp_filename),
+                print_output=print_output,
+                print_input=print_input,
+                **arguments,
+            )
+
+            if not status:
+                raise IOError(output.stderr)
+
+            # Load our file or IO object and write it to the temporary file
+            with open(temp_filename, encoding="utf-8") as temp_f:
+                with get_file_io(filename_or_io, "wb") as file_io:
+                    data_bytes: bytes
+
+                    data = temp_f.read()
+                    if isinstance(data, str):
+                        data_bytes = data.encode()
+                    else:
+                        data_bytes = data
+
+                    file_io.write(data_bytes)
+        finally:
+            os.remove(temp_filename)
+
+        if print_output:
+            click.echo(
+                "{0}file copied: {1}".format(self.host.print_prefix, remote_filename),
+                err=True,
+            )
+
+        return True
+
+    def check_can_rsync(self):
+        if not find_executable("rsync"):
+            raise NotImplementedError("The `rsync` binary is not available on this system.")
+
+    def rsync(
+        self,
+        src,
+        dest,
+        flags,
+        print_output: bool = False,
+        print_input: bool = False,
+        **arguments,
+    ) -> bool:
+        status, output = self.run_shell_command(
+            StringCommand("rsync", " ".join(flags), src, dest),
             print_output=print_output,
             print_input=print_input,
-            **command_kwargs,
+            **arguments,
         )
 
         if not status:
-            raise IOError("\n".join(stderr))
-
-        # Load our file or IO object and write it to the temporary file
-        with open(temp_filename, encoding="utf-8") as temp_f:
-            with get_file_io(filename_or_io, "wb") as file_io:
-                data_bytes: bytes
-
-                data = temp_f.read()
-                if isinstance(data, str):
-                    data_bytes = data.encode()
-                else:
-                    data_bytes = data
-
-                file_io.write(data_bytes)
-    finally:
-        os.remove(temp_filename)
-
-    if print_output:
-        click.echo(
-            "{0}file copied: {1}".format(host.print_prefix, remote_filename),
-            err=True,
-        )
-
-    return True
-
-
-def check_can_rsync(host):
-    if not find_executable("rsync"):
-        raise NotImplementedError("The `rsync` binary is not available on this system.")
-
-
-def rsync(
-    state: "State",
-    host: "Host",
-    src,
-    dest,
-    flags,
-    print_output: bool = False,
-    print_input: bool = False,
-    **command_kwargs,
-):
-    status, _, stderr = run_shell_command(
-        state,
-        host,
-        "rsync {0} {1} {2}".format(" ".join(flags), src, dest),
-        print_output=print_output,
-        print_input=print_input,
-        **command_kwargs,
-    )
-
-    if not status:
-        raise IOError("\n".join(stderr))
+            raise IOError(output.stderr)
 
-    return True
+        return True
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/mech.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/vagrant.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,186 +1,180 @@
-"""
-The ``@mech`` connector reads the current mech status and generates an inventory
-for any running VMs.
-
-.. code:: python
-
-    # Run on all hosts
-    pyinfra @mech ...
-
-    # Run on a specific VM
-    pyinfra @mech/my-vm-name ...
-
-    # Run on multiple named VMs
-    pyinfra @mech/my-vm-name,@mech/another-vm-name ...
-"""
-
 import json
 from os import path
 from queue import Queue
 from threading import Thread
 
 from pyinfra import local, logger
 from pyinfra.api.exceptions import InventoryError
 from pyinfra.api.util import memoize
 from pyinfra.progress import progress_spinner
 
+from .base import BaseConnector
 
-def _get_mech_ssh_config(queue, progress, target):
+
+def _get_vagrant_ssh_config(queue, progress, target):
     logger.debug("Loading SSH config for %s", target)
 
-    # Note: We have to work-around the fact that "mech ssh-config somehost"
-    # does not return the correct "Host" value. When "mech" fixes this
-    # issue we can simply this code.
-    lines = local.shell(
-        "mech ssh-config {0}".format(target),
-        splitlines=True,
+    queue.put(
+        local.shell(
+            "vagrant ssh-config {0}".format(target),
+            splitlines=True,
+        ),
     )
 
-    newlines = []
-    for line in lines:
-        if line.startswith("Host "):
-            newlines.append("Host " + target)
-        else:
-            newlines.append(line)
-
-    queue.put(newlines)
-
     progress(target)
 
 
 @memoize
-def get_mech_config(limit=None):
-    logger.info("Getting Mech config...")
+def get_vagrant_config(limit=None):
+    logger.info("Getting Vagrant config...")
 
     if limit and not isinstance(limit, (list, tuple)):
         limit = [limit]
 
-    # Note: There is no "--machine-readable" option to 'mech status'
-    with progress_spinner({"mech ls"}) as progress:
+    with progress_spinner({"vagrant status"}) as progress:
         output = local.shell(
-            "mech ls",
+            "vagrant status --machine-readable",
             splitlines=True,
         )
-        progress("mech ls")
+        progress("vagrant status")
 
     targets = []
 
     for line in output:
-
-        address = ""
-
-        data = line.split()
-        target = data[0]
-
-        if len(data) == 5:
-            address = data[1]
+        line = line.strip()
+        _, target, type_, data = line.split(",", 3)
 
         # Skip anything not in the limit
         if limit is not None and target not in limit:
             continue
 
-        # For each vm that has an address, fetch it's SSH config in a thread
-        if address != "" and address[0].isdigit():
+        # For each running container - fetch it's SSH config in a thread - this
+        # is because Vagrant *really* slow to run each command.
+        if type_ == "state" and data == "running":
             targets.append(target)
 
     threads = []
-    config_queue = Queue()
+    config_queue = Queue()  # type: ignore
 
     with progress_spinner(targets) as progress:
         for target in targets:
             thread = Thread(
-                target=_get_mech_ssh_config,
+                target=_get_vagrant_ssh_config,
                 args=(config_queue, progress, target),
             )
             threads.append(thread)
             thread.start()
 
     for thread in threads:
         thread.join()
 
     queue_items = list(config_queue.queue)
 
     lines = []
     for output in queue_items:
-        lines.extend(output)
+        lines.extend([ln.strip() for ln in output])
 
     return lines
 
 
 @memoize
-def get_mech_options():
-    if path.exists("@mech.json"):
-        with open("@mech.json", "r", encoding="utf-8") as f:
+def get_vagrant_options():
+    if path.exists("@vagrant.json"):
+        with open("@vagrant.json", "r", encoding="utf-8") as f:
             return json.loads(f.read())
     return {}
 
 
 def _make_name_data(host):
-    mech_options = get_mech_options()
-    mech_host = host["Host"]
+    vagrant_options = get_vagrant_options()
+    vagrant_host = host["Host"]
 
     data = {
         "ssh_hostname": host["HostName"],
     }
 
     for config_key, data_key in (
         ("Port", "ssh_port"),
         ("User", "ssh_user"),
         ("IdentityFile", "ssh_key"),
     ):
         if config_key in host:
             data[data_key] = host[config_key]
 
     # Update any configured JSON data
-    if mech_host in mech_options.get("data", {}):
-        data.update(mech_options["data"][mech_host])
+    if vagrant_host in vagrant_options.get("data", {}):
+        data.update(vagrant_options["data"][vagrant_host])
 
     # Work out groups
-    groups = mech_options.get("groups", {}).get(mech_host, [])
+    groups = vagrant_options.get("groups", {}).get(vagrant_host, [])
 
-    if "@mech" not in groups:
-        groups.append("@mech")
+    if "@vagrant" not in groups:
+        groups.append("@vagrant")
 
-    return "@mech/{0}".format(host["Host"]), data, groups
+    return "@vagrant/{0}".format(host["Host"]), data, groups
 
 
-def make_names_data(limit=None):
-    mech_ssh_info = get_mech_config(limit)
+class VagrantInventoryConnector(BaseConnector):
+    """
+    The ``@vagrant`` connector reads the current Vagrant status and generates an
+    inventory for any running VMs.
 
-    logger.debug("Got Mech SSH info: \n%s", mech_ssh_info)
+    .. code:: shell
 
-    hosts = []
-    current_host = None
+        # Run on all hosts
+        pyinfra @vagrant ...
 
-    for line in mech_ssh_info:
-        if not line:
-            if current_host:
-                hosts.append(_make_name_data(current_host))
+        # Run on a specific VM
+        pyinfra @vagrant/my-vm-name ...
 
-            current_host = None
-            continue
+        # Run on multiple named VMs
+        pyinfra @vagrant/my-vm-name,@vagrant/another-vm-name ...
+    """
+
+    @staticmethod
+    def make_names_data(name=None):
+        vagrant_ssh_info = get_vagrant_config(name)
+
+        logger.debug("Got Vagrant SSH info: \n%s", vagrant_ssh_info)
+
+        hosts = []
+        current_host = None
+
+        for line in vagrant_ssh_info:
+            # Vagrant outputs an empty line between each host
+            if not line:
+                if current_host:
+                    hosts.append(_make_name_data(current_host))
+
+                current_host = None
+                continue
 
-        key, value = line.strip().split(" ", 1)
+            key, value = line.split(" ", 1)
 
-        if key == "Host":
-            if current_host:
-                hosts.append(_make_name_data(current_host))
+            if key == "Host":
+                if current_host:
+                    hosts.append(_make_name_data(current_host))
 
-            # Set the new host
-            current_host = {
-                key: value,
-            }
+                # Set the new host
+                current_host = {
+                    key: value,
+                }
 
-        elif current_host:
-            current_host[key] = value
+            elif current_host:
+                current_host[key] = value
 
-        else:
-            logger.debug("Extra Mech SSH key/value (%s=%s)", key, value)
+            else:
+                logger.debug("Extra Vagrant SSH key/value (%s=%s)", key, value)
 
-    if current_host:
-        hosts.append(_make_name_data(current_host))
+        if current_host:
+            hosts.append(_make_name_data(current_host))
 
-    if not hosts:
-        raise InventoryError("No running Mech instances found!")
+        if not hosts:
+            if name:
+                raise InventoryError(
+                    "No running Vagrant instances matching `{0}` found!".format(name)
+                )
+            raise InventoryError("No running Vagrant instances found!")
 
-    return hosts
+        for host in hosts:
+            yield host
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/ssh.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/ssh.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,687 +1,624 @@
-"""
-Connect to hosts over SSH. This is the default connector and all targets default
-to this meaning you do not need to specify it - ie the following two commands
-are identical:
-
-.. code:: shell
-
-    pyinfra my-host.net ...
-    pyinfra @ssh/my-host.net ...
-"""
+from __future__ import annotations
+
 import shlex
 from distutils.spawn import find_executable
-from getpass import getpass
-from os import path
+from random import uniform
 from socket import error as socket_error, gaierror
-from typing import TYPE_CHECKING, Type, Union
+from time import sleep
+from typing import TYPE_CHECKING, Any, Iterable, Optional, Tuple
 
 import click
-from paramiko import (
-    AuthenticationException,
-    BadHostKeyException,
-    DSSKey,
-    ECDSAKey,
-    Ed25519Key,
-    PasswordRequiredException,
-    RSAKey,
-    SFTPClient,
-    SSHException,
-)
+from paramiko import AuthenticationException, BadHostKeyException, SFTPClient, SSHException
+from typing_extensions import TypedDict, Unpack
 
-import pyinfra
 from pyinfra import logger
 from pyinfra.api.command import QuoteString, StringCommand
-from pyinfra.api.connectors import BaseConnectorMeta
-from pyinfra.api.exceptions import ConnectError, PyinfraError
+from pyinfra.api.exceptions import ConnectError
 from pyinfra.api.util import get_file_io, memoize
 
+from .base import BaseConnector, DataMeta
+from .ssh_util import get_private_key, raise_connect_error
 from .sshuserclient import SSHClient
 from .util import (
+    CommandOutput,
     execute_command_with_sudo_retry,
     make_unix_command_for_host,
-    read_buffers_into_queue,
+    read_output_buffers,
     run_local_process,
-    split_combined_output,
     write_stdin,
 )
 
 if TYPE_CHECKING:
-    from pyinfra.api.host import Host
-    from pyinfra.api.state import State
+    from pyinfra.api.arguments import ConnectorArguments
 
 
-class Meta(BaseConnectorMeta):
-    handles_execution = True
-    keys_prefix = "ssh"
-
-    class DataKeys:
-        hostname = "SSH hostname"
-        port = "SSH port"
-
-        user = "User to SSH as"
-        password = "Password to use for authentication"
-        key = "Key file to use for authentication"
-        key_password = "Key file password"
-
-        allow_agent = "Allow using SSH agent"
-        look_for_keys = "Allow looking up users keys"
-
-        forward_agent = "Enable SSH forward agent"
-        config_file = "Custom SSH config file"
-        known_hosts_file = "Custom SSH known hosts file"
-        strict_host_key_checking = "Override strict host keys check setting"
-
-        paramiko_connect_kwargs = (
-            "Override keyword arguments passed into paramiko's `SSHClient.connect`"
-        )
-
+class ConnectorData(TypedDict):
+    ssh_hostname: str
+    ssh_port: int
+    ssh_user: str
+    ssh_password: str
+    ssh_key: str
+    ssh_key_password: str
+
+    ssh_allow_agent: bool
+    ssh_look_for_keys: bool
+    ssh_forward_agent: bool
+
+    ssh_config_file: str
+    ssh_known_hosts_file: str
+    ssh_strict_host_key_checking: str
+
+    ssh_paramiko_connect_kwargs: dict
+
+    ssh_connect_retries: int
+    ssh_connect_retry_min_delay: float
+    ssh_connect_retry_max_delay: float
+
+
+connector_data_meta: dict[str, DataMeta] = {
+    "ssh_hostname": DataMeta("SSH hostname"),
+    "ssh_port": DataMeta("SSH port"),
+    "ssh_user": DataMeta("SSH user"),
+    "ssh_password": DataMeta("SSH password"),
+    "ssh_key": DataMeta("SSH key filename"),
+    "ssh_key_password": DataMeta("SSH key password"),
+    "ssh_allow_agent": DataMeta(
+        "Whether to use any active SSH agent",
+        True,
+    ),
+    "ssh_look_for_keys": DataMeta(
+        "Whether to look for private keys",
+        True,
+    ),
+    "ssh_forward_agent": DataMeta(
+        "Whether to enable SSH forward agent",
+        False,
+    ),
+    "ssh_config_file": DataMeta("SSH config filename"),
+    "ssh_known_hosts_file": DataMeta("SSH known_hosts filename"),
+    "ssh_strict_host_key_checking": DataMeta(
+        "SSH strict host key checking",
+        "accept-new",
+    ),
+    "ssh_paramiko_connect_kwargs": DataMeta(
+        "Override keyword arguments passed into Paramiko's ``SSHClient.connect``"
+    ),
+    "ssh_connect_retries": DataMeta("Number of tries to connect via ssh", 0),
+    "ssh_connect_retry_min_delay": DataMeta(
+        "Lower bound for random delay between retries",
+        0.1,
+    ),
+    "ssh_connect_retry_max_delay": DataMeta(
+        "Upper bound for random delay between retries",
+        0.5,
+    ),
+}
 
-DATA_KEYS = Meta.keys()
-
-
-def make_names_data(hostname):
-    yield "@ssh/{0}".format(hostname), {DATA_KEYS.hostname: hostname}, []
 
+class SSHConnector(BaseConnector):
+    """
+    Connect to hosts over SSH. This is the default connector and all targets default
+    to this meaning you do not need to specify it - ie the following two commands
+    are identical:
 
-def _raise_connect_error(host: "Host", message, data):
-    message = "{0} ({1})".format(message, data)
-    raise ConnectError(message)
+    .. code:: shell
 
+        pyinfra my-host.net ...
+        pyinfra @ssh/my-host.net ...
+    """
 
-def _load_private_key_file(filename: str, key_filename: str, key_password: str):
-    exception: Union[PyinfraError, SSHException] = PyinfraError("Invalid key: {0}".format(filename))
+    __examples_doc__ = """
+    An inventory file (``inventory.py``) containing a single SSH target with SSH
+    forward agent enabled:
+
+    .. code:: python
+
+        hosts = [
+            ("my-host.net", {"ssh_forward_agent": True}),
+        ]
+
+    Multiple hosts sharing the same SSH username:
+
+    .. code:: python
+
+        hosts = (
+            [
+                "my-host-1.net",
+                "my-host-2.net",
+            ],
+            {
+                "ssh_username": "ssh-user",
+            },
+        )
+    """
 
-    key_cls: Union[Type[RSAKey], Type[DSSKey], Type[ECDSAKey], Type[Ed25519Key]]
+    handles_execution = True
 
-    for key_cls in (RSAKey, DSSKey, ECDSAKey, Ed25519Key):
-        try:
-            return key_cls.from_private_key_file(
-                filename=filename,
+    data_cls = ConnectorData
+    data_meta = connector_data_meta
+    data: ConnectorData
+
+    client: Optional[SSHClient] = None
+
+    @staticmethod
+    def make_names_data(name):
+        yield "@ssh/{0}".format(name), {"ssh_hostname": name}, []
+
+    def make_paramiko_kwargs(self) -> dict[str, Any]:
+        kwargs = {
+            "allow_agent": False,
+            "look_for_keys": False,
+            "hostname": self.data["ssh_hostname"] or self.host.name,
+            # Overrides of SSH config via pyinfra host data
+            "_pyinfra_ssh_forward_agent": self.data["ssh_forward_agent"],
+            "_pyinfra_ssh_config_file": self.data["ssh_config_file"],
+            "_pyinfra_ssh_known_hosts_file": self.data["ssh_known_hosts_file"],
+            "_pyinfra_ssh_strict_host_key_checking": self.data["ssh_strict_host_key_checking"],
+            "_pyinfra_ssh_paramiko_connect_kwargs": self.data["ssh_paramiko_connect_kwargs"],
+        }
+
+        for key, value in (
+            ("username", self.data["ssh_user"]),
+            ("port", int(self.data["ssh_port"] or 0)),
+            ("timeout", self.state.config.CONNECT_TIMEOUT),
+        ):
+            if value:
+                kwargs[key] = value
+
+        # Password auth (boo!)
+        ssh_password = self.data["ssh_password"]
+        if ssh_password:
+            kwargs["password"] = ssh_password
+
+        # Key auth!
+        ssh_key = self.data["ssh_key"]
+        if ssh_key:
+            kwargs["pkey"] = get_private_key(
+                self.state,
+                key_filename=ssh_key,
+                key_password=self.data["ssh_key_password"],
             )
 
-        except PasswordRequiredException:
-            if not key_password:
-                # If password is not provided, but we're in CLI mode, ask for it. I'm not a
-                # huge fan of having CLI specific code in here, but it doesn't really fit
-                # anywhere else without duplicating lots of key related code into cli.py.
-                if pyinfra.is_cli:
-                    key_password = getpass(
-                        "Enter password for private key: {0}: ".format(
-                            key_filename,
-                        ),
-                    )
-
-                # API mode and no password? We can't continue!
-                else:
-                    raise PyinfraError(
-                        "Private key file ({0}) is encrypted, set ssh_key_password to "
-                        "use this key".format(key_filename),
-                    )
+        # No key or password, so let's have paramiko look for SSH agents and user keys
+        # unless disabled by the user.
+        else:
+            kwargs["allow_agent"] = self.data["ssh_allow_agent"]
+            kwargs["look_for_keys"] = self.data["ssh_look_for_keys"]
 
-            try:
-                return key_cls.from_private_key_file(
-                    filename=filename,
-                    password=key_password,
-                )
-            except SSHException as e:  # key does not match key_cls type
-                exception = e
-        except SSHException as e:  # key does not match key_cls type
-            exception = e
-    raise exception
-
-
-def _get_private_key(state: "State", key_filename: str, key_password: str):
-    if key_filename in state.private_keys:
-        return state.private_keys[key_filename]
-
-    ssh_key_filenames = [
-        # Global from executed directory
-        path.expanduser(key_filename),
-    ]
-
-    if state.cwd:
-        # Relative to the CWD
-        path.join(state.cwd, key_filename)
-
-    key = None
-    key_file_exists = False
-
-    for filename in ssh_key_filenames:
-        if not path.isfile(filename):
-            continue
+        return kwargs
 
-        key_file_exists = True
+    def connect(self) -> None:
+        retries = self.data["ssh_connect_retries"]
 
         try:
-            key = _load_private_key_file(filename, key_filename, key_password)
-            break
-        except SSHException:
-            pass
-
-    # No break, so no key found
-    if not key:
-        if not key_file_exists:
-            raise PyinfraError("No such private key file: {0}".format(key_filename))
-        raise PyinfraError("Invalid private key file: {0}".format(key_filename))
-
-    # Load any certificate, names from OpenSSH:
-    # https://github.com/openssh/openssh-portable/blob/049297de975b92adcc2db77e3fb7046c0e3c695d/ssh-keygen.c#L2453  # noqa: E501
-    for certificate_filename in (
-        "{0}-cert.pub".format(key_filename),
-        "{0}.pub".format(key_filename),
-    ):
-        if path.isfile(certificate_filename):
-            key.load_certificate(certificate_filename)
-
-    state.private_keys[key_filename] = key
-    return key
-
-
-def _make_paramiko_kwargs(state: "State", host: "Host"):
-    kwargs = {
-        "allow_agent": False,
-        "look_for_keys": False,
-        "hostname": host.data.get(DATA_KEYS.hostname, host.name),
-        # Overrides of SSH config via pyinfra host data
-        "_pyinfra_ssh_forward_agent": host.data.get(DATA_KEYS.forward_agent),
-        "_pyinfra_ssh_config_file": host.data.get(DATA_KEYS.config_file),
-        "_pyinfra_ssh_known_hosts_file": host.data.get(DATA_KEYS.known_hosts_file),
-        "_pyinfra_ssh_strict_host_key_checking": host.data.get(DATA_KEYS.strict_host_key_checking),
-        "_pyinfra_ssh_paramiko_connect_kwargs": host.data.get(DATA_KEYS.paramiko_connect_kwargs),
-    }
-
-    for key, value in (
-        ("username", host.data.get(DATA_KEYS.user)),
-        ("port", int(host.data.get(DATA_KEYS.port, 0))),
-        ("timeout", state.config.CONNECT_TIMEOUT),
-    ):
-        if value:
-            kwargs[key] = value
-
-    # Password auth (boo!)
-    ssh_password = host.data.get(DATA_KEYS.password)
-    if ssh_password:
-        kwargs["password"] = ssh_password
-
-    # Key auth!
-    ssh_key = host.data.get(DATA_KEYS.key)
-    if ssh_key:
-        kwargs["pkey"] = _get_private_key(
-            state,
-            key_filename=ssh_key,
-            key_password=host.data.get(DATA_KEYS.key_password),
-        )
-
-    # No key or password, so let's have paramiko look for SSH agents and user keys
-    # unless disabled by the user.
-    else:
-        kwargs["allow_agent"] = host.data.get(DATA_KEYS.allow_agent, True)
-        kwargs["look_for_keys"] = host.data.get(DATA_KEYS.look_for_keys, True)
+            while True:
+                try:
+                    return self._connect()
+                except (SSHException, gaierror, socket_error, EOFError):
+                    if retries == 0:
+                        raise
+                    retries -= 1
+                    min_delay = self.data["ssh_connect_retry_min_delay"]
+                    max_delay = self.data["ssh_connect_retry_max_delay"]
+                    sleep(uniform(min_delay, max_delay))
+        except SSHException as e:
+            raise_connect_error(self.host, "SSH error", e)
+        except gaierror as e:
+            raise_connect_error(self.host, "Could not resolve hostname", e)
+        except socket_error as e:
+            raise_connect_error(self.host, "Could not connect", e)
+        except EOFError as e:
+            raise_connect_error(self.host, "EOF error", e)
+
+    def _connect(self) -> None:
+        """
+        Connect to a single host. Returns the SSH client if successful. Stateless by
+        design so can be run in parallel.
+        """
+
+        kwargs = self.make_paramiko_kwargs()
+        hostname = kwargs.pop("hostname")
+        logger.debug("Connecting to: %s (%r)", hostname, kwargs)
 
-    return kwargs
+        self.client = SSHClient()
 
+        try:
+            self.client.connect(hostname, **kwargs)
+        except AuthenticationException as e:
+            auth_kwargs = {}
+
+            for key, value in kwargs.items():
+                if key in ("username", "password"):
+                    auth_kwargs[key] = value
+                    continue
 
-def connect(state: "State", host: "Host"):
-    """
-    Connect to a single host. Returns the SSH client if successful. Stateless by
-    design so can be run in parallel.
-    """
-
-    kwargs = _make_paramiko_kwargs(state, host)
-    logger.debug("Connecting to: %s (%r)", host.name, kwargs)
-
-    hostname = kwargs.pop("hostname")
-
-    try:
-        # Create new client & connect to the host
-        client = SSHClient()
-        client.connect(hostname, **kwargs)
-        return client
-
-    except AuthenticationException as e:
-        auth_kwargs = {}
+                if key == "pkey" and value:
+                    auth_kwargs["key"] = self.data["ssh_key"]
 
-        for key, value in kwargs.items():
-            if key in ("username", "password"):
-                auth_kwargs[key] = value
-                continue
+            auth_args = ", ".join(
+                "{0}={1}".format(key, value) for key, value in auth_kwargs.items()
+            )
 
-            if key == "pkey" and value:
-                auth_kwargs["key"] = host.data.get(DATA_KEYS.key)
+            raise_connect_error(self.host, "Authentication error ({0})".format(auth_args), e)
 
-        auth_args = ", ".join("{0}={1}".format(key, value) for key, value in auth_kwargs.items())
+        except BadHostKeyException as e:
+            remove_entry = e.hostname
+            port = self.client._ssh_config.get("port", 22)
+            if port != 22:
+                remove_entry = f"[{e.hostname}]:{port}"
+
+            logger.warning("WARNING: REMOTE HOST IDENTIFICATION HAS CHANGED!")
+            logger.warning(
+                ("Someone could be eavesdropping on you right now " "(man-in-the-middle attack)!"),
+            )
+            logger.warning("If this is expected, you can remove the bad key using:")
+            logger.warning(f"    ssh-keygen -R {remove_entry}")
 
-        _raise_connect_error(host, "Authentication error ({0})".format(auth_args), e)
+            raise_connect_error(
+                self.host,
+                "SSH host key error",
+                f"Host key for {e.hostname} does not match.",
+            )
 
-    except BadHostKeyException as e:
-        remove_entry = e.hostname
-        port = client._ssh_config.get("port", 22)
-        if port != 22:
-            remove_entry = f"[{e.hostname}]:{port}"
+    def run_shell_command(
+        self,
+        command: StringCommand,
+        print_output: bool = False,
+        print_input: bool = False,
+        **arguments: Unpack["ConnectorArguments"],
+    ) -> Tuple[bool, CommandOutput]:
+        """
+        Execute a command on the specified host.
+
+        Args:
+            state (``pyinfra.api.State`` obj): state object for this command
+            hostname (string): hostname of the target
+            command (string): actual command to execute
+            sudo (boolean): whether to wrap the command with sudo
+            sudo_user (string): user to sudo to
+            get_pty (boolean): whether to get a PTY before executing the command
+            env (dict): environment variables to set
+            timeout (int): timeout for this command to complete before erroring
+
+        Returns:
+            tuple: (exit_code, stdout, stderr)
+            stdout and stderr are both lists of strings from each buffer.
+        """
+
+        _get_pty = arguments.pop("_get_pty", False)
+        _timeout = arguments.pop("_timeout", None)
+        _stdin = arguments.pop("_stdin", None)
+        _success_exit_codes = arguments.pop("_success_exit_codes", None)
+
+        def execute_command() -> Tuple[int, CommandOutput]:
+            unix_command = make_unix_command_for_host(self.state, self.host, command, **arguments)
+            actual_command = unix_command.get_raw_value()
+
+            logger.debug(
+                "Running command on %s: (pty=%s) %s",
+                self.host.name,
+                _get_pty,
+                unix_command,
+            )
 
-        logger.warning("WARNING: REMOTE HOST IDENTIFICATION HAS CHANGED!")
-        logger.warning(
-            ("Someone could be eavesdropping on you right now " "(man-in-the-middle attack)!"),
-        )
-        logger.warning("If this is expected, you can remove the bad key using:")
-        logger.warning(f"    ssh-keygen -R {remove_entry}")
+            if print_input:
+                click.echo("{0}>>> {1}".format(self.host.print_prefix, unix_command), err=True)
 
-        _raise_connect_error(
-            host,
-            "SSH host key error",
-            f"Host key for {e.hostname} does not match.",
-        )
+            # Run it! Get stdout, stderr & the underlying channel
+            assert self.client is not None
+            stdin_buffer, stdout_buffer, stderr_buffer = self.client.exec_command(
+                actual_command,
+                get_pty=_get_pty,
+            )
 
-    except SSHException as e:
-        _raise_connect_error(host, "SSH error", e)
+            if _stdin:
+                write_stdin(_stdin, stdin_buffer)
 
-    except gaierror:
-        _raise_connect_error(host, "Could not resolve hostname", hostname)
+            combined_output = read_output_buffers(
+                stdout_buffer,
+                stderr_buffer,
+                timeout=_timeout,
+                print_output=print_output,
+                print_prefix=self.host.print_prefix,
+            )
 
-    except socket_error as e:
-        _raise_connect_error(host, "Could not connect", e)
+            logger.debug("Waiting for exit status...")
+            exit_status = stdout_buffer.channel.recv_exit_status()
+            logger.debug("Command exit status: %i", exit_status)
+
+            return exit_status, combined_output
+
+        return_code, combined_output = execute_command_with_sudo_retry(
+            self.host,
+            arguments,
+            execute_command,
+        )
+
+        if _success_exit_codes:
+            status = return_code in _success_exit_codes
+        else:
+            status = return_code == 0
 
-    except EOFError as e:
-        _raise_connect_error(host, "EOF error", e)
-
-
-def run_shell_command(
-    state: "State",
-    host: "Host",
-    command,
-    get_pty: bool = False,
-    timeout=None,
-    stdin=None,
-    success_exit_codes=None,
-    print_output: bool = False,
-    print_input: bool = False,
-    return_combined_output: bool = False,
-    **command_kwargs,
-):
-    """
-    Execute a command on the specified host.
+        return status, combined_output
 
-    Args:
-        state (``pyinfra.api.State`` obj): state object for this command
-        hostname (string): hostname of the target
-        command (string): actual command to execute
-        sudo (boolean): whether to wrap the command with sudo
-        sudo_user (string): user to sudo to
-        get_pty (boolean): whether to get a PTY before executing the command
-        env (dict): environment variables to set
-        timeout (int): timeout for this command to complete before erroring
-
-    Returns:
-        tuple: (exit_code, stdout, stderr)
-        stdout and stderr are both lists of strings from each buffer.
-    """
+    @memoize
+    def get_sftp_connection(self):
+        assert self.client is not None
+        transport = self.client.get_transport()
+        assert transport is not None, "No transport"
+        try:
+            return SFTPClient.from_transport(transport)
+        except SSHException as e:
+            raise ConnectError(
+                (
+                    "Unable to establish SFTP connection. Check that the SFTP subsystem "
+                    "for the SSH service at {0} is enabled."
+                ).format(self.host),
+            ) from e
+
+    def _get_file(self, remote_filename: str, filename_or_io):
+        with get_file_io(filename_or_io, "wb") as file_io:
+            sftp = self.get_sftp_connection()
+            sftp.getfo(remote_filename, file_io)
+
+    def get_file(
+        self,
+        remote_filename: str,
+        filename_or_io,
+        remote_temp_filename=None,
+        print_output: bool = False,
+        print_input: bool = False,
+        **arguments: Unpack["ConnectorArguments"],
+    ) -> bool:
+        """
+        Download a file from the remote host using SFTP. Supports download files
+        with sudo by copying to a temporary directory with read permissions,
+        downloading and then removing the copy.
+        """
+
+        _sudo = arguments.get("_sudo", False)
+        _su_user = arguments.get("_su_user", None)
+
+        if _sudo or _su_user:
+            # Get temp file location
+            temp_file = remote_temp_filename or self.host.get_temp_filename(remote_filename)
+
+            # Copy the file to the tempfile location and add read permissions
+            command = StringCommand(
+                "cp", remote_filename, temp_file, "&&", "chmod", "+r", temp_file
+            )
 
-    def execute_command():
-        unix_command = make_unix_command_for_host(state, host, command, **command_kwargs)
-        actual_command = unix_command.get_raw_value()
-
-        logger.debug(
-            "Running command on %s: (pty=%s) %s",
-            host.name,
-            get_pty,
-            unix_command,
-        )
+            copy_status, output = self.run_shell_command(
+                command,
+                print_output=print_output,
+                print_input=print_input,
+                **arguments,
+            )
 
-        if print_input:
-            click.echo("{0}>>> {1}".format(host.print_prefix, unix_command), err=True)
+            if copy_status is False:
+                logger.error("File download copy temp error: {0}".format(output.stderr))
+                return False
 
-        # Run it! Get stdout, stderr & the underlying channel
-        stdin_buffer, stdout_buffer, stderr_buffer = host.connection.exec_command(
-            actual_command,
-            get_pty=get_pty,
-        )
+            try:
+                self._get_file(temp_file, filename_or_io)
 
-        if stdin:
-            write_stdin(stdin, stdin_buffer)
+            # Ensure that, even if we encounter an error, we (attempt to) remove the
+            # temporary copy of the file.
+            finally:
+                remove_status, output = self.run_shell_command(
+                    StringCommand("rm", "-f", temp_file),
+                    print_output=print_output,
+                    print_input=print_input,
+                    **arguments,
+                )
 
-        combined_output = read_buffers_into_queue(
-            stdout_buffer,
-            stderr_buffer,
-            timeout=timeout,
-            print_output=print_output,
-            print_prefix=host.print_prefix,
-        )
+            if remove_status is False:
+                logger.error("File download remove temp error: {0}".format(output.stderr))
+                return False
 
-        logger.debug("Waiting for exit status...")
-        exit_status = stdout_buffer.channel.recv_exit_status()
-        logger.debug("Command exit status: %i", exit_status)
-
-        return exit_status, combined_output
-
-    return_code, combined_output = execute_command_with_sudo_retry(
-        host,
-        command_kwargs,
-        execute_command,
-    )
-
-    if success_exit_codes:
-        status = return_code in success_exit_codes
-    else:
-        status = return_code == 0
+        else:
+            self._get_file(remote_filename, filename_or_io)
 
-    if return_combined_output:
-        return status, combined_output
+        if print_output:
+            click.echo(
+                "{0}file downloaded: {1}".format(self.host.print_prefix, remote_filename),
+                err=True,
+            )
 
-    stdout, stderr = split_combined_output(combined_output)
-    return status, stdout, stderr
+        return True
 
+    def _put_file(self, filename_or_io, remote_location):
+        logger.debug("Attempting upload of %s to %s", filename_or_io, remote_location)
 
-@memoize
-def _get_sftp_connection(host: "Host"):
-    assert host.connection is not None
-    transport = host.connection.get_transport()
-
-    try:
-        return SFTPClient.from_transport(transport)
-    except SSHException as e:
-        raise ConnectError(
-            (
-                "Unable to establish SFTP connection. Check that the SFTP subsystem "
-                "for the SSH service at {0} is enabled."
-            ).format(host),
-        ) from e
-
-
-def _get_file(host: "Host", remote_filename: str, filename_or_io):
-    with get_file_io(filename_or_io, "wb") as file_io:
-        sftp = _get_sftp_connection(host)
-        sftp.getfo(remote_filename, file_io)
-
-
-def get_file(
-    state: "State",
-    host: "Host",
-    remote_filename: str,
-    filename_or_io,
-    remote_temp_filename=None,
-    sudo: bool = False,
-    sudo_user=None,
-    su_user=None,
-    print_output: bool = False,
-    print_input: bool = False,
-    **command_kwargs,
-):
-    """
-    Download a file from the remote host using SFTP. Supports download files
-    with sudo by copying to a temporary directory with read permissions,
-    downloading and then removing the copy.
-    """
+        attempts = 0
+        last_e = None
 
-    if sudo or su_user:
-        # Get temp file location
-        temp_file = remote_temp_filename or state.get_temp_filename(remote_filename)
-
-        # Copy the file to the tempfile location and add read permissions
-        command = "cp {0} {1} && chmod +r {0}".format(remote_filename, temp_file)
-
-        copy_status, _, stderr = run_shell_command(
-            state,
-            host,
-            command,
-            sudo=sudo,
-            sudo_user=sudo_user,
-            su_user=su_user,
-            print_output=print_output,
-            print_input=print_input,
-            **command_kwargs,
-        )
+        while attempts < 3:
+            try:
+                with get_file_io(filename_or_io) as file_io:
+                    sftp = self.get_sftp_connection()
+                    sftp.putfo(file_io, remote_location)
+                return
+            except OSError as e:
+                logger.warning(f"Failed to upload file, retrying: {e}")
+                attempts += 1
+                last_e = e
+
+        if last_e is not None:
+            raise last_e
+
+    def put_file(
+        self,
+        filename_or_io,
+        remote_filename,
+        remote_temp_filename=None,
+        print_output: bool = False,
+        print_input: bool = False,
+        **arguments: Unpack["ConnectorArguments"],
+    ) -> bool:
+        """
+        Upload file-ios to the specified host using SFTP. Supports uploading files
+        with sudo by uploading to a temporary directory then moving & chowning.
+        """
+
+        original_arguments = arguments.copy()
+
+        _sudo = arguments.pop("_sudo", False)
+        _sudo_user = arguments.pop("_sudo_user", False)
+        _doas = arguments.pop("_doas", False)
+        _doas_user = arguments.pop("_doas_user", False)
+        _su_user = arguments.pop("_su_user", None)
+
+        # sudo/su are a little more complicated, as you can only sftp with the SSH
+        # user connected, so upload to tmp and copy/chown w/sudo and/or su_user
+        if _sudo or _doas or _su_user:
+            # Get temp file location
+            temp_file = remote_temp_filename or self.host.get_temp_filename(remote_filename)
+            self._put_file(filename_or_io, temp_file)
+
+            # Make sure our sudo/su user can access the file
+            other_user = _su_user or _sudo_user or _doas_user
+            if other_user:
+                status, output = self.run_shell_command(
+                    StringCommand("setfacl", "-m", f"u:{other_user}:r", temp_file),
+                    print_output=print_output,
+                    print_input=print_input,
+                    **arguments,
+                )
 
-        if copy_status is False:
-            logger.error("File download copy temp error: {0}".format("\n".join(stderr)))
-            return False
+                if status is False:
+                    logger.error("Error on handover to sudo/su user: {0}".format(output.stderr))
+                    return False
 
-        try:
-            _get_file(host, temp_file, filename_or_io)
+            # Execute run_shell_command w/sudo, etc
+            command = StringCommand("cp", temp_file, QuoteString(remote_filename))
 
-        # Ensure that, even if we encounter an error, we (attempt to) remove the
-        # temporary copy of the file.
-        finally:
-            remove_status, _, stderr = run_shell_command(
-                state,
-                host,
-                "rm -f {0}".format(temp_file),
-                sudo=sudo,
-                sudo_user=sudo_user,
-                su_user=su_user,
+            status, output = self.run_shell_command(
+                command,
                 print_output=print_output,
                 print_input=print_input,
-                **command_kwargs,
+                **original_arguments,
             )
 
-        if remove_status is False:
-            logger.error("File download remove temp error: {0}".format("\n".join(stderr)))
-            return False
-
-    else:
-        _get_file(host, remote_filename, filename_or_io)
-
-    if print_output:
-        click.echo(
-            "{0}file downloaded: {1}".format(host.print_prefix, remote_filename),
-            err=True,
-        )
-
-    return True
-
-
-def _put_file(host: "Host", filename_or_io, remote_location):
-    logger.debug("Attempting upload of %s to %s", filename_or_io, remote_location)
-
-    attempts = 0
-    last_e = None
+            if status is False:
+                logger.error("File upload error: {0}".format(output.stderr))
+                return False
 
-    while attempts < 3:
-        try:
-            with get_file_io(filename_or_io) as file_io:
-                sftp = _get_sftp_connection(host)
-                sftp.putfo(file_io, remote_location)
-            return
-        except OSError as e:
-            logger.warning(f"Failed to upload file, retrying: {e}")
-            attempts += 1
-            last_e = e
-
-    if last_e is not None:
-        raise last_e
-
-
-def put_file(
-    state: "State",
-    host: "Host",
-    filename_or_io,
-    remote_filename,
-    remote_temp_filename=None,
-    sudo: bool = False,
-    sudo_user=None,
-    doas: bool = False,
-    doas_user=None,
-    su_user=None,
-    print_output: bool = False,
-    print_input: bool = False,
-    **command_kwargs,
-):
-    """
-    Upload file-ios to the specified host using SFTP. Supports uploading files
-    with sudo by uploading to a temporary directory then moving & chowning.
-    """
+            # Delete the temporary file now that we've successfully copied it
+            command = StringCommand("rm", "-f", temp_file)
 
-    # sudo/su are a little more complicated, as you can only sftp with the SSH
-    # user connected, so upload to tmp and copy/chown w/sudo and/or su_user
-    if sudo or doas or su_user:
-        # Get temp file location
-        temp_file = remote_temp_filename or state.get_temp_filename(remote_filename)
-        _put_file(host, filename_or_io, temp_file)
-
-        # Make sure our sudo/su user can access the file
-        if su_user:
-            command = StringCommand("setfacl", "-m", "u:{0}:r".format(su_user), temp_file)
-        elif sudo_user:
-            command = StringCommand("setfacl", "-m", "u:{0}:r".format(sudo_user), temp_file)
-        elif doas_user:
-            command = StringCommand("setfacl", "-m", "u:{0}:r".format(doas_user), temp_file)
-
-        if su_user or sudo_user or doas_user:
-            status, _, stderr = run_shell_command(
-                state,
-                host,
+            status, output = self.run_shell_command(
                 command,
-                sudo=False,
                 print_output=print_output,
                 print_input=print_input,
-                **command_kwargs,
+                **arguments,
             )
 
             if status is False:
-                logger.error("Error on handover to sudo/su user: {0}".format("\n".join(stderr)))
+                logger.error("Unable to remove temporary file: {0}".format(output.stderr))
                 return False
 
-        # Execute run_shell_command w/sudo and/or su_user
-        command = StringCommand("cp", temp_file, QuoteString(remote_filename))
+        # No sudo and no su_user, so just upload it!
+        else:
+            self._put_file(filename_or_io, remote_filename)
+
+        if print_output:
+            click.echo(
+                "{0}file uploaded: {1}".format(self.host.print_prefix, remote_filename),
+                err=True,
+            )
 
-        status, _, stderr = run_shell_command(
-            state,
-            host,
-            command,
-            sudo=sudo,
-            sudo_user=sudo_user,
-            doas=doas,
-            doas_user=doas_user,
-            su_user=su_user,
-            print_output=print_output,
-            print_input=print_input,
-            **command_kwargs,
-        )
+        return True
 
-        if status is False:
-            logger.error("File upload error: {0}".format("\n".join(stderr)))
-            return False
-
-        # Delete the temporary file now that we've successfully copied it
-        command = StringCommand("rm", "-f", temp_file)
-
-        status, _, stderr = run_shell_command(
-            state,
-            host,
-            command,
-            sudo=False,
-            doas=False,
-            print_output=print_output,
-            print_input=print_input,
-            **command_kwargs,
-        )
+    def check_can_rsync(self):
+        if self.data["ssh_key_password"]:
+            raise NotImplementedError(
+                "Rsync does not currently work with SSH keys needing passwords."
+            )
 
-        if status is False:
-            logger.error("Unable to remove temporary file: {0}".format("\n".join(stderr)))
-            return False
-
-    # No sudo and no su_user, so just upload it!
-    else:
-        _put_file(host, filename_or_io, remote_filename)
-
-    if print_output:
-        click.echo(
-            "{0}file uploaded: {1}".format(host.print_prefix, remote_filename),
-            err=True,
-        )
+        if self.data["ssh_password"]:
+            raise NotImplementedError("Rsync does not currently work with SSH passwords.")
+
+        if not find_executable("rsync"):
+            raise NotImplementedError("The `rsync` binary is not available on this system.")
+
+    def rsync(
+        self,
+        src: str,
+        dest: str,
+        flags: Iterable[str],
+        print_output: bool = False,
+        print_input: bool = False,
+        **arguments: Unpack["ConnectorArguments"],
+    ):
+        _sudo = arguments.pop("_sudo", False)
+        _sudo_user = arguments.pop("_sudo_user", False)
 
-    return True
+        hostname = self.data["ssh_hostname"] or self.host.name
+        user = self.data["ssh_user"]
+        if user:
+            user = "{0}@".format(user)
+
+        ssh_flags = []
+        # To avoid asking for interactive input, specify BatchMode=yes
+        ssh_flags.append("-o BatchMode=yes")
+
+        known_hosts_file = self.data["ssh_known_hosts_file"]
+        if known_hosts_file:
+            ssh_flags.append(
+                '-o \\"UserKnownHostsFile={0}\\"'.format(shlex.quote(known_hosts_file))
+            )  # never trust users
+
+        strict_host_key_checking = self.data["ssh_strict_host_key_checking"]
+        if strict_host_key_checking:
+            ssh_flags.append(
+                '-o \\"StrictHostKeyChecking={0}\\"'.format(shlex.quote(strict_host_key_checking))
+            )
+
+        ssh_config_file = self.data["ssh_config_file"]
+        if ssh_config_file:
+            ssh_flags.append("-F {0}".format(shlex.quote(ssh_config_file)))
+
+        port = self.data["ssh_port"]
+        if port:
+            ssh_flags.append("-p {0}".format(port))
+
+        ssh_key = self.data["ssh_key"]
+        if ssh_key:
+            ssh_flags.append("-i {0}".format(ssh_key))
+
+        remote_rsync_command = "rsync"
+        if _sudo:
+            remote_rsync_command = "sudo rsync"
+            if _sudo_user:
+                remote_rsync_command = "sudo -u {0} rsync".format(_sudo_user)
+
+        rsync_command = (
+            "rsync {rsync_flags} "
+            '--rsh "ssh {ssh_flags}" '
+            "--rsync-path '{remote_rsync_command}' "
+            "{src} {user}{hostname}:{dest}"
+        ).format(
+            rsync_flags=" ".join(flags),
+            ssh_flags=" ".join(ssh_flags),
+            remote_rsync_command=remote_rsync_command,
+            user=user,
+            hostname=hostname,
+            src=src,
+            dest=dest,
+        )
 
+        if print_input:
+            click.echo("{0}>>> {1}".format(self.host.print_prefix, rsync_command), err=True)
 
-def check_can_rsync(host: "Host"):
-    if host.data.get(DATA_KEYS.key_password):
-        raise NotImplementedError("Rsync does not currently work with SSH keys needing passwords.")
-
-    if host.data.get(DATA_KEYS.password):
-        raise NotImplementedError("Rsync does not currently work with SSH passwords.")
-
-    if not find_executable("rsync"):
-        raise NotImplementedError("The `rsync` binary is not available on this system.")
-
-
-def rsync(
-    state: "State",
-    host: "Host",
-    src: str,
-    dest: str,
-    flags,
-    print_output: bool = False,
-    print_input: bool = False,
-    sudo: bool = False,
-    sudo_user=None,
-    **ignored_kwargs,
-):
-    hostname = host.data.get(DATA_KEYS.hostname, host.name)
-    user = host.data.get(DATA_KEYS.user, "")
-    if user:
-        user = "{0}@".format(user)
-
-    ssh_flags = []
-    # To avoid asking for interactive input, specify BatchMode=yes
-    ssh_flags.append("-o BatchMode=yes")
-
-    known_hosts_file = host.data.get(DATA_KEYS.known_hosts_file, "")
-    if known_hosts_file:
-        ssh_flags.append(
-            '-o \\"UserKnownHostsFile={0}\\"'.format(shlex.quote(known_hosts_file))
-        )  # never trust users
-
-    strict_host_key_checking = host.data.get(DATA_KEYS.strict_host_key_checking, "")
-    if strict_host_key_checking:
-        ssh_flags.append(
-            '-o \\"StrictHostKeyChecking={0}\\"'.format(shlex.quote(strict_host_key_checking))
+        return_code, output = run_local_process(
+            rsync_command,
+            print_output=print_output,
+            print_prefix=self.host.print_prefix,
         )
 
-    ssh_config_file = host.data.get(DATA_KEYS.config_file, "")
-    if ssh_config_file:
-        ssh_flags.append("-F {0}".format(shlex.quote(ssh_config_file)))
-
-    port = host.data.get(DATA_KEYS.port)
-    if port:
-        ssh_flags.append("-p {0}".format(port))
-
-    ssh_key = host.data.get(DATA_KEYS.key)
-    if ssh_key:
-        ssh_flags.append("-i {0}".format(ssh_key))
-
-    remote_rsync_command = "rsync"
-    if sudo:
-        remote_rsync_command = "sudo rsync"
-        if sudo_user:
-            remote_rsync_command = "sudo -u {0} rsync".format(sudo_user)
-
-    rsync_command = (
-        "rsync {rsync_flags} "
-        '--rsh "ssh {ssh_flags}" '
-        "--rsync-path '{remote_rsync_command}' "
-        "{src} {user}{hostname}:{dest}"
-    ).format(
-        rsync_flags=" ".join(flags),
-        ssh_flags=" ".join(ssh_flags),
-        remote_rsync_command=remote_rsync_command,
-        user=user,
-        hostname=hostname,
-        src=src,
-        dest=dest,
-    )
-
-    if print_input:
-        click.echo("{0}>>> {1}".format(host.print_prefix, rsync_command), err=True)
-
-    return_code, combined_output = run_local_process(
-        rsync_command,
-        print_output=print_output,
-        print_prefix=host.print_prefix,
-    )
-
-    status = return_code == 0
-
-    if not status:
-        _, stderr = split_combined_output(combined_output)
-        raise IOError("\n".join(stderr))
+        status = return_code == 0
+        if not status:
+            raise IOError(output.stderr)
 
-    return True
+        return True
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/sshuserclient/client.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/sshuserclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,34 +162,36 @@
         self._ssh_config = config
         super().connect(hostname, **config)
 
         if _pyinfra_ssh_forward_agent is not None:
             forward_agent = _pyinfra_ssh_forward_agent
 
         if forward_agent:
-            # Enable SSH forwarding
-            session = self.get_transport().open_session()
+            transport = self.get_transport()
+            assert transport is not None, "No transport"
+            session = transport.open_session()
             AgentRequestHandler(session)
 
     def gateway(self, hostname, host_port, target, target_port):
         transport = self.get_transport()
+        assert transport is not None, "No transport"
         return transport.open_channel(
             "direct-tcpip",
             (target, target_port),
             (hostname, host_port),
         )
 
     def parse_config(
         self,
         hostname,
         initial_cfg=None,
         ssh_config_file=None,
         strict_host_key_checking=None,
     ):
-        cfg = {"port": 22}
+        cfg: dict = {"port": 22}
         cfg.update(initial_cfg or {})
 
         forward_agent = False
         missing_host_key_policy = get_missing_host_key_policy(strict_host_key_checking)
         host_keys_file = path.expanduser("~/.ssh/known_hosts")  # OpenSSH default
 
         ssh_config = get_ssh_config(ssh_config_file)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/sshuserclient/config.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/sshuserclient/config.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/connectors/terraform.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/connectors/terraform.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,16 @@
-"""
-.. warning::
-    This connector is in alpha and may change in future releases.
-
-Generate one or more SSH hosts from a Terraform output variable. The variable
-must be a list of hostnames or IP addresses that ``pyinfra`` can connect to
-over SSH. Currently there is no support for specifying SSH user/pass/port/key
-from Terraform, these must be provided via ``pyinfra`` group data or ``--data``
-CLI flags.
-
-Output is fetched from a flattened JSON dictionary output from ``terraform output
--json``. For example the following object:
-
-.. code:: json
-
-    {
-      "server_group": {
-        "value": {
-          "server_group_node_ips": [
-            "1.2.3.4",
-            "1.2.3.5",
-            "1.2.3.6"
-          ]
-        }
-      }
-    }
-
-The IP list ``server_group_node_ips`` would be used like so:
-
-.. code:: python
-
-    pyinfra @terraform/server_group.value.server_group_node_ips ...
-"""
-
 import json
 
 from pyinfra import local, logger
 from pyinfra.api.exceptions import InventoryError
 from pyinfra.api.util import memoize
 from pyinfra.progress import progress_spinner
 
+from .base import BaseConnector
+
 
 @memoize
 def show_warning():
     logger.warning("The @terraform connector is in alpha!")
 
 
 def _flatten_dict_gen(d, parent_key, sep):
@@ -54,47 +22,101 @@
             yield new_key, v
 
 
 def _flatten_dict(d: dict, parent_key: str = "", sep: str = "."):
     return dict(_flatten_dict_gen(d, parent_key, sep))
 
 
-def make_names_data(output_key=None):
-    show_warning()
+class TerraformInventoryConnector(BaseConnector):
+    """
+    Generate one or more SSH hosts from a Terraform output variable. The variable
+    must be a list of hostnames or dictionaries.
+
+    Output is fetched from a flattened JSON dictionary output from ``terraform output
+    -json``. For example the following object:
+
+    .. code:: json
+
+        {
+          "server_group": {
+            "value": {
+              "server_group_node_ips": [
+                "1.2.3.4",
+                "1.2.3.5",
+                "1.2.3.6"
+              ]
+            }
+          }
+        }
 
-    if not output_key:
-        raise InventoryError("No Terraform output key!")
+    The IP list ``server_group_node_ips`` would be used like so:
 
-    with progress_spinner({"fetch terraform output"}):
-        tf_output_raw = local.shell("terraform output -json")
+    .. code:: sh
 
-    tf_output = json.loads(tf_output_raw)
-    tf_output = _flatten_dict(tf_output)
-
-    tf_output_value = tf_output.get(output_key)
-    if tf_output_value is None:
-        raise InventoryError(f"No Terraform output with key: `{output_key}`")
-
-    if not isinstance(tf_output_value, list):
-        raise InventoryError(
-            "Invalid Terraform output type, should be `list`, got "
-            f"`{type(tf_output_value).__name__}`",
-        )
-
-    for ssh_target in tf_output_value:
-        if isinstance(ssh_target, dict):
-            name = ssh_target.pop("name", ssh_target.get("ssh_hostname"))
-            if name is None:
-                raise InventoryError(
-                    "Invalid Terraform list item, missing `name` or `ssh_hostname` keys",
-                )
-            yield f"@terraform/{name}", ssh_target, ["@terraform"]
+        pyinfra @terraform/server_group.value.server_group_node_ips ...
 
-        elif isinstance(ssh_target, str):
-            data = {"ssh_hostname": ssh_target}
-            yield f"@terraform/{ssh_target}", data, ["@terraform"]
+    You can also specify dictionaries to include extra data with hosts:
 
-        else:
+    .. code:: json
+
+        {
+          "server_group": {
+            "value": {
+              "server_group_node_ips": [
+                {
+                    "ssh_hostname": "1.2.3.4",
+                    "ssh_user": "ssh-user"
+                },
+                {
+                    "ssh_hostname": "1.2.3.5",
+                    "ssh_user": "ssh-user"
+                }
+              ]
+            }
+          }
+        }
+
+    """
+
+    @staticmethod
+    def make_names_data(name=None):
+        show_warning()
+
+        if not name:
+            name = ""
+
+        with progress_spinner({"fetch terraform output"}):
+            tf_output_raw = local.shell("terraform output -json")
+
+        assert isinstance(tf_output_raw, str)
+        tf_output = json.loads(tf_output_raw)
+        tf_output = _flatten_dict(tf_output)
+
+        tf_output_value = tf_output.get(name)
+        if tf_output_value is None:
+            keys = "\n".join(f"   - {k}" for k in tf_output.keys())
+            raise InventoryError(f"No Terraform output with key: `{name}`, valid keys:\n{keys}")
+
+        if not isinstance(tf_output_value, list):
             raise InventoryError(
-                "Invalid Terraform list item, should be `dict` or `str` got "
-                f"`{type(ssh_target).__name__}`",
+                "Invalid Terraform output type, should be `list`, got "
+                f"`{type(tf_output_value).__name__}`",
             )
+
+        for ssh_target in tf_output_value:
+            if isinstance(ssh_target, dict):
+                name = ssh_target.pop("name", ssh_target.get("ssh_hostname"))
+                if name is None:
+                    raise InventoryError(
+                        "Invalid Terraform list item, missing `name` or `ssh_hostname` keys",
+                    )
+                yield f"@terraform/{name}", ssh_target, ["@terraform"]
+
+            elif isinstance(ssh_target, str):
+                data = {"ssh_hostname": ssh_target}
+                yield f"@terraform/{ssh_target}", data, ["@terraform"]
+
+            else:
+                raise InventoryError(
+                    "Invalid Terraform list item, should be `dict` or `str` got "
+                    f"`{type(ssh_target).__name__}`",
+                )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/context.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 The `ContextObject` and `ContextManager` provide context specific variables that
 are imported and used throughout pyinfra and end user deploy code (CLI mode).
 
 These variables always represent the current executing pyinfra context.
 """
 from contextlib import contextmanager
+from types import ModuleType
 from typing import TYPE_CHECKING
 
 from gevent.local import local
 
 if TYPE_CHECKING:
     from pyinfra.api.config import Config
     from pyinfra.api.host import Host
     from pyinfra.api.inventory import Inventory
     from pyinfra.api.state import State
 
 
 class container:
-    pass
+    module = None
 
 
 class ContextObject:
     _container_cls = container
-    _base_cls = None
+    _base_cls: ModuleType
 
     def __init__(self):
         self._container = self._container_cls()
         self._container.module = None
 
     def _get_module(self):
         return self._container.module
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/apt.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/apt.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/brew.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/brew.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/cargo.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/cargo.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/choco.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/choco.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     .. code:: python
 
         {
             "package_name": ["version"],
         }
     """
 
-    command = "choco list --local-only"
+    command = "choco list"
     shell_executable = "ps"
 
     default = dict
 
     def process(self, output):
         return parse_packages(CHOCO_REGEX, output)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/deb.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/deb.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 
 class DebPackage(FactBase):
     """
     Returns information on a .deb archive or installed package.
     """
 
     _regexes = {
-        "name": r"^Package: ({0})$".format(DEB_PACKAGE_NAME_REGEX),
-        "version": r"^Version: ({0})$".format(DEB_PACKAGE_VERSION_REGEX),
+        "name": r"^Package:\s+({0})$".format(DEB_PACKAGE_NAME_REGEX),
+        "version": r"^Version:\s+({0})$".format(DEB_PACKAGE_VERSION_REGEX),
     }
 
     requires_command = "dpkg"
 
     def command(self, name):
         return "! test -e {0} && (dpkg -s {0} 2>/dev/null || true) || dpkg -I {0}".format(name)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/dnf.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/dnf.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/docker.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/docker.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from pyinfra.api import FactBase
 
 
 class DockerFactBase(FactBase):
     abstract = True
 
+    docker_type: str
     requires_command = "docker"
 
     def process(self, output):
         output = "".join(output)
         return json.loads(output)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/files.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 The files facts provide information about the filesystem and it's contents on the target host.
 """
 
 import re
 import stat
 from datetime import datetime
-from typing import List, Tuple
+from typing import TYPE_CHECKING, List, Optional, Tuple, Union
+
+from typing_extensions import Literal, NotRequired, TypedDict
 
 from pyinfra.api.command import QuoteString, make_formatted_string_command
 from pyinfra.api.facts import FactBase
 from pyinfra.api.util import try_int
 
 LINUX_STAT_COMMAND = "stat -c 'user=%U group=%G mode=%A atime=%X mtime=%Y ctime=%Z size=%s %N'"
 BSD_STAT_COMMAND = "stat -f 'user=%Su group=%Sg mode=%Sp atime=%a mtime=%m ctime=%c size=%z %N%SY'"
@@ -60,15 +62,33 @@
             if char == c:
                 out |= m
                 break
 
     return int(oct(out)[2:])
 
 
-class File(FactBase):
+def _parse_datetime(value: str) -> Optional[datetime]:
+    value = try_int(value)
+    if isinstance(value, int):
+        return datetime.utcfromtimestamp(value)
+    return None
+
+
+class FileDict(TypedDict):
+    mode: int
+    size: Union[int, str]
+    atime: Optional[datetime]
+    mtime: Optional[datetime]
+    ctime: Optional[datetime]
+    user: str
+    group: str
+    link_target: NotRequired[str]
+
+
+class File(FactBase[Union[FileDict, Literal[False], None]]):
     """
     Returns information about a file on the remote system:
 
     .. code:: python
 
         {
             "user": "pyinfra",
@@ -94,44 +114,31 @@
                 "( {linux_stat_command} {0} 2> /dev/null || {bsd_stat_command} {0} )"
             ),
             QuoteString(path),
             linux_stat_command=LINUX_STAT_COMMAND,
             bsd_stat_command=BSD_STAT_COMMAND,
         )
 
-    def process(self, output):
+    def process(self, output) -> Union[FileDict, Literal[False], None]:
         match = re.match(STAT_REGEX, output[0])
         if not match:
             return None
 
-        data = {}
-        path_type = None
-
-        for key, value in (
-            ("user", match.group(1)),
-            ("group", match.group(2)),
-            ("mode", match.group(3)),
-            ("atime", match.group(4)),
-            ("mtime", match.group(5)),
-            ("ctime", match.group(6)),
-            ("size", match.group(7)),
-        ):
-            if key == "mode":
-                path_type = FLAG_TO_TYPE[value[0]]
-                value = _parse_mode(value[1:])
-
-            elif key == "size":
-                value = try_int(value)
-
-            elif key in ("atime", "mtime", "ctime"):
-                value = try_int(value)
-                if isinstance(value, int):
-                    value = datetime.utcfromtimestamp(value)
+        mode = match.group(3)
+        path_type = FLAG_TO_TYPE[mode[0]]
 
-            data[key] = value
+        data: FileDict = {
+            "user": match.group(1),
+            "group": match.group(2),
+            "mode": _parse_mode(mode[1:]),
+            "atime": _parse_datetime(match.group(4)),
+            "mtime": _parse_datetime(match.group(5)),
+            "ctime": _parse_datetime(match.group(6)),
+            "size": try_int(match.group(7)),
+        }
 
         if path_type != self.type:
             return False
 
         if path_type == "link":
             filename = match.group(8)
             filename, target = filename.split(" -> ")
@@ -201,15 +208,21 @@
     If the path exists but is not a socket:
         returns ``False``
     """
 
     type = "socket"
 
 
-class HashFileFactBase(FactBase):
+if TYPE_CHECKING:
+    FactBaseOptionalStr = FactBase[Optional[str]]
+else:
+    FactBaseOptionalStr = FactBase
+
+
+class HashFileFactBase(FactBaseOptionalStr):
     _raw_cmd: str
     _regexes: Tuple[str, str]
 
     def __init_subclass__(cls, digits: int, cmds: List[str], **kwargs) -> None:
         super().__init_subclass__(**kwargs)
 
         raw_hash_cmds = ["%s {0} 2> /dev/null" % cmd for cmd in cmds]
@@ -225,21 +238,22 @@
             r"^%s\s+\(%%s\)\s+=\s+([a-fA-F0-9]{%d})$" % (hash_name, digits),
         )
 
     def command(self, path):
         self.path = path
         return make_formatted_string_command(self._raw_cmd, QuoteString(path))
 
-    def process(self, output):
+    def process(self, output) -> Optional[str]:
         output = output[0]
         escaped_path = re.escape(self.path)
         for regex in self._regexes:
             matches = re.match(regex % escaped_path, output)
             if matches:
                 return matches.group(1)
+        return None
 
 
 class Sha1File(HashFileFactBase, digits=40, cmds=["sha1sum", "shasum", "sha1"]):
     """
     Returns a SHA1 hash of a file. Works with both sha1sum and sha1. Returns
     ``None`` if the file doest not exist.
     """
@@ -290,14 +304,15 @@
 
         return output
 
 
 class FindFilesBase(FactBase):
     abstract = True
     default = list
+    type_flag: str
 
     @staticmethod
     def process(output):
         return output
 
     def command(self, path, quote_path=True):
         return make_formatted_string_command(
@@ -341,15 +356,14 @@
     def command(self, path):
         return make_formatted_string_command(
             "! test -e {0} || stat -f %Sf {0}",
             QuoteString(path),
         )
 
     def process(self, output):
-
         return [flag for flag in output[0].split(",") if len(flag) > 0] if len(output) == 1 else []
 
 
 MARKER_DEFAULT = "# {mark} PYINFRA BLOCK"
 MARKER_BEGIN_DEFAULT = "BEGIN"
 MARKER_END_DEFAULT = "END"
 EXISTS = "__pyinfra_exists_"
@@ -377,15 +391,14 @@
     # if markers aren't found, awk will return 0 and produce no output but we need to
     # distinguish between "markers not found" and "markers found but nothing between them"
     # for the former we use the empty list (created the call to default) and for the latter
     # the list with a single empty string.
     default = list
 
     def command(self, path, marker=None, begin=None, end=None):
-
         self.path = path
         start = (marker or MARKER_DEFAULT).format(mark=begin or MARKER_BEGIN_DEFAULT)
         end = (marker or MARKER_DEFAULT).format(mark=end or MARKER_END_DEFAULT)
         if start == end:
             raise ValueError(f"delimiters for block must be different but found only '{start}'")
 
         backstop = make_formatted_string_command(
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/git.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/git.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 
 from pyinfra.api.facts import FactBase
 
 
 class GitBranch(FactBase):
     requires_command = "git"
@@ -25,15 +27,15 @@
         if repo is None:
             return "git config --global -l || true"
 
         return "! test -d {0} || (cd {0} && git config --local -l)".format(repo)
 
     @staticmethod
     def process(output):
-        items = {}
+        items: dict[str, list[str]] = {}
 
         for line in output:
             key, value = line.split("=", 1)
             items.setdefault(key, []).append(value)
 
         return items
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/gpg.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/gpg.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                     current_key = key_details
                     current_subkey = None
                 elif current_key:
                     current_subkey = key_details
 
             elif current_subkey or current_key:
                 target = current_subkey or current_key
-
+                assert target is not None
                 if bits[0] == "fpr":
                     target["fingerprint"] = bits[9]  # fingerprint = field 10
                 elif bits[0] == "uid":
                     target["uid_hash"] = bits[7]
                     target["uid"] = bits[9]
 
         if current_key:
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/hardware.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/hardware.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 
 from pyinfra.api import FactBase, ShortFactBase
 
 
 class Cpus(FactBase):
     """
@@ -93,164 +95,199 @@
                     "used_percent": matches.group(5),
                     "mount": matches.group(6),
                 }
 
         return devices
 
 
-nettools_1_regexes = [
-    (
-        r"^inet addr:([0-9\.]+).+Bcast:([0-9\.]+).+Mask:([0-9\.]+)$",
-        ("ipv4", "address", "broadcast", "netmask"),
-    ),
-    (
-        r"^inet6 addr: ([0-9a-z:]+)\/([0-9]+) Scope:Global",
-        ("ipv6", "address", "mask_bits"),
-    ),
-]
-
-nettools_2_regexes = [
-    (
-        r"^inet ([0-9\.]+)\s+netmask ([0-9\.fx]+)(?:\s+broadcast ([0-9\.]+))?$",
-        ("ipv4", "address", "netmask", "broadcast"),
-    ),
-    (
-        r"^inet6 ([0-9a-z:]+)\s+prefixlen ([0-9]+)",
-        ("ipv6", "address", "mask_bits"),
-    ),
-]
-
-iproute2_regexes = [
-    (
-        r"^inet ([0-9\.]+)\/([0-9]{1,2})(?:\s+brd ([0-9\.]+))?",
-        ("ipv4", "address", "mask_bits", "broadcast"),
-    ),
-    (
-        r"^inet6 ([0-9a-z:]+)\/([0-9]{1,3})",
-        ("ipv6", "address", "mask_bits"),
-    ),
-]
-
-
-def _parse_regexes(regexes, lines):
-    data = {
-        "ipv4": {},
-        "ipv6": {},
-    }
-
-    for line in lines:
-        for regex, groups in regexes:
-            matches = re.match(regex, line)
-            if matches:
-                ip_data = {}
-
-                for i, group in enumerate(groups[1:]):
-                    ip_data[group] = matches.group(i + 1)
-
-                if "mask_bits" in ip_data:
-                    ip_data["mask_bits"] = int(ip_data["mask_bits"])
-
-                target_group = data[groups[0]]
-                if target_group.get("address"):
-                    target_group.setdefault("additional_ips", []).append(ip_data)
-                else:
-                    target_group.update(ip_data)
-
-                break
-
-    return data
-
-
 class NetworkDevices(FactBase):
     """
     Gets & returns a dict of network devices. See the ``ipv4_addresses`` and
     ``ipv6_addresses`` facts for easier-to-use shortcuts to get device addresses.
 
     .. code:: python
-
-        {
-            "eth0": {
-                "ipv4": {
-                    "address": "127.0.0.1",
-                    "broadcast": "127.0.0.13",
-                    # Only one of these will exist:
-                    "netmask": "255.255.255.255",
-                    "mask_bits": 32,
-                },
-                "ipv6": {
-                    "address": "fe80::a00:27ff:fec3:36f0",
-                    "mask_bits": 64,
-                    "additional_ips": [{
-                        "address": "fe80::",
-                        "mask_bits": 128,
-                    }],
-                }
+        "enp1s0": {
+            "ether": "12:34:56:78:9A:BC",
+            "mtu": 1500,
+            "state": "UP",
+            "ipv4": {
+                "address": "192.168.1.100",
+                "mask_bits": 24,
+                "netmask": "255.255.255.0"
+            },
+            "ipv6": {
+                "address": "2001:db8:85a3::8a2e:370:7334",
+                "mask_bits": 64,
+                "additional_ips": [
+                    {
+                        "address": "fe80::1234:5678:9abc:def0",
+                        "mask_bits": 64
+                    }
+                ]
+            }
+        },
+        "incusbr0": {
+            "ether": "DE:AD:BE:EF:CA:FE",
+            "mtu": 1500,
+            "state": "UP",
+            "ipv4": {
+                "address": "10.0.0.1",
+                "mask_bits": 24,
+                "netmask": "255.255.255.0"
             },
+            "ipv6": {
+                "address": "fe80::dead:beef:cafe:babe",
+                "mask_bits": 64,
+                "additional_ips": [
+                    {
+                        "address": "2001:db8:1234:5678::1",
+                        "mask_bits": 64
+                    }
+                ]
+            }
+        },
+        "lo": {
+            "mtu": 65536,
+            "state": "UP",
+            "ipv6": {
+                "address": "::1",
+                "mask_bits": 128
+            }
+        },
+        "veth98806fd6": {
+            "ether": "AA:BB:CC:DD:EE:FF",
+            "mtu": 1500,
+            "state": "UP"
+        },
+        "vethda29df81": {
+            "ether": "11:22:33:44:55:66",
+            "mtu": 1500,
+            "state": "UP"
+        },
+        "wlo1": {
+            "ether": "77:88:99:AA:BB:CC",
+            "mtu": 1500,
+            "state": "UNKNOWN"
         }
     """
 
-    command = "ip addr show 2> /dev/null || ifconfig"
+    command = "ip addr show 2> /dev/null || ifconfig -a"
     default = dict
 
     # Definition of valid interface names for Linux:
     # https://git.kernel.org/pub/scm/linux/kernel/git/stable/linux.git/tree/net/core/dev.c?h=v5.1.3#n1020
-    _start_regexes = [
-        (
-            r"^([^/: \s]+)\s+Link encap:",
-            lambda lines: _parse_regexes(nettools_1_regexes, lines),
-        ),
-        (
-            r"^([^/: \s]+): flags=",
-            lambda lines: _parse_regexes(nettools_2_regexes, lines),
-        ),
-        (
-            r"^[0-9]+: ([^/: \s]+): ",
-            lambda lines: _parse_regexes(iproute2_regexes, lines),
-        ),
-    ]
-
     def process(self, output):
-        devices = {}
+        def mask(value):
+            try:
+                if value.startswith("0x"):
+                    mask_bits = bin(int(value, 16)).count("1")
+                else:
+                    mask_bits = int(value)
+                netmask = ".".join(
+                    str((0xFFFFFFFF << (32 - b) >> mask_bits) & 0xFF) for b in (24, 16, 8, 0)
+                )
+            except ValueError:
+                mask_bits = sum(bin(int(x)).count("1") for x in value.split("."))
+                netmask = value
 
-        # Store current matches (start lines), the handler and any lines
-        matches = None
-        handler = None
-        line_buffer = []
+            return mask_bits, netmask
 
-        for line in output:
-            line = line.strip()
+        # Strip lines and merge them as a block of text
+        output = "\n".join(map(str.strip, output))
 
-            matched = False
+        # Splitting the output into sections per network device
+        device_sections = re.split(r"\n(?=\d+: \w|\w+:.*mtu.*)", output)
 
-            # Look for start lines
-            for regex, new_handler in self._start_regexes:
-                new_matches = re.match(regex, line)
-
-                # If we find a start line
-                if new_matches:
-                    matched = True
-
-                    # Assign any current matches with current handler, reset buffer
-                    if matches:
-                        devices[matches.group(1)] = handler(line_buffer)
-                        line_buffer = []
-
-                    # Set new matches/handler
-                    matches = new_matches
-                    handler = new_handler
+        # Dictionary to hold all device information
+        all_devices = {}
+
+        for section in device_sections:
+            # Extracting the device name
+            device_name_match = re.match(r"^(?:\d+: )?([\w@]+):", section)
+            if not device_name_match:
+                continue
+            device_name = device_name_match.group(1)
+
+            # Regular expressions to match different parts of the output
+            ether_re = re.compile(r"([0-9A-Fa-f:]{17})")
+            mtu_re = re.compile(r"mtu (\d+)")
+            ipv4_re = (
+                re.compile(
+                    r"inet (\d+\.\d+\.\d+\.\d+)/(\d+)(?: brd (\d+\.\d+\.\d+\.\d+))"
+                ),  # ip a output,
+                re.compile(
+                    r"inet (\d+\.\d+\.\d+\.\d+)\s+netmask\s+((?:\d+\.\d+\.\d+\.\d+)|(?:[0-9a-fA-FxX]+))(?:\s+broadcast\s+(\d+\.\d+\.\d+\.\d+))"  # noqa: E501
+                ),  # ifconfig -a output
+            )
+
+            # Parsing the output
+            ether = ether_re.search(section)
+            mtu = mtu_re.search(section)
+
+            # Building the result dictionary for the device
+            device_info = {}
+            if ether:
+                device_info["ether"] = ether.group(1)
+            if mtu:
+                device_info["mtu"] = int(mtu.group(1))
+
+            device_info["state"] = (
+                "UP" if "UP" in section else "DOWN" if "DOWN" in section else "UNKNOWN"
+            )
+
+            # IPv4 Addresses
+            for ipv4_re_ in ipv4_re:
+                ipv4_matches = ipv4_re_.findall(section)
+                if ipv4_matches:
                     break
 
-            if not matched:
-                line_buffer.append(line)
+            if ipv4_matches:
+                ipv4_info = []
+                for ipv4 in ipv4_matches:
+                    address = ipv4[0]
+                    mask_value = ipv4[1]
+                    mask_bits, netmask = mask(mask_value)
+                    broadcast = ipv4[2] if len(ipv4) == 3 else None
+
+                    ipv4_info.append(
+                        {
+                            "address": address,
+                            "mask_bits": mask_bits,
+                            "netmask": netmask,
+                            "broadcast": broadcast,
+                        },
+                    )
+                device_info["ipv4"] = ipv4_info[0]
+                if len(ipv4_matches) > 1:
+                    device_info["ipv4"]["additional_ips"] = ipv4_info[1:]  # type: ignore[index]
+
+            # IPv6 Addresses
+            ipv6_re = (
+                re.compile(r"inet6\s+([0-9a-fA-F:]+)/(\d+)"),
+                re.compile(r"inet6\s+([0-9a-fA-F:]+)\s+prefixlen\s+(\d+)"),
+            )
+
+            for ipv6_re_ in ipv6_re:
+                ipv6_matches = ipv6_re_.findall(section)
+                if ipv6_matches:
+                    break
 
-        # Handle any left over matches
-        if matches:
-            devices[matches.group(1)] = handler(line_buffer)
+            if ipv6_matches:
+                ipv6_info = []
+                for ipv6 in ipv6_matches:
+                    address = ipv6[0]
+                    mask_bits = ipv6[1] or ipv6[2]
+                    ipv6_info.append({"address": address, "mask_bits": int(mask_bits)})
+                device_info["ipv6"] = ipv6_info[0]
+                if len(ipv6_matches) > 1:
+                    device_info["ipv6"]["additional_ips"] = ipv6_info[1:]  # type: ignore[index]
 
-        return devices
+            all_devices[device_name] = device_info
+
+        return all_devices
 
 
 class Ipv4Addrs(ShortFactBase):
     """
     Gets & returns a dictionary of network interface -> list of IPv4 addresses.
 
     .. code:: python
@@ -269,15 +306,15 @@
     def process_data(self, data):
         host_to_ips = {}
 
         for interface, details in data.items():
             ips = []
 
             ip_details = details.get(self.ip_type)
-            if not ip_details:
+            if not ip_details or not ip_details.get("address"):
                 continue
 
             ips.append(ip_details["address"])
             if "additional_ips" in ip_details:
                 ips.extend([ip["address"] for ip in ip_details["additional_ips"]])
 
             host_to_ips[interface] = ips
@@ -328,15 +365,15 @@
     ip_type = "ipv4"
 
     def process_data(self, data):
         addresses = {}
 
         for interface, details in data.items():
             ip_details = details.get(self.ip_type)
-            if not ip_details:
+            if not ip_details or not ip_details.get("address"):
                 continue  # pragma: no cover
 
             addresses[interface] = ip_details["address"]
 
         return addresses
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/iptables.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/iptables.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pyinfra.api import FactBase
 
 # Mapping for iptables code arguments to variable names
 IPTABLES_ARGS = {
     "-A": "chain",
     "-j": "jump",
     # Boolean matches
@@ -23,24 +25,24 @@
     """
     Parse one iptables rule. Returns a dict where each iptables code argument
     is mapped to a name using IPTABLES_ARGS.
     """
 
     bits = line.split()
 
-    definition = {}
+    definition: dict = {}
 
     key = None
-    args = []
+    args: list[str] = []
     not_arg = False
 
     def add_args():
         arg_string = " ".join(args)
 
-        if key in IPTABLES_ARGS:
+        if key and key in IPTABLES_ARGS:
             definition_key = "not_{0}".format(IPTABLES_ARGS[key]) if not_arg else IPTABLES_ARGS[key]
             definition[definition_key] = arg_string
         else:
             definition.setdefault("extras", []).extend((key, arg_string))
 
     for bit in bits:
         if bit == "!":
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/launchd.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/launchd.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/mysql.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/mysql.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from pyinfra.api import FactBase, MaskString, QuoteString, StringCommand
 from pyinfra.api.util import try_int
 
 from .util.databases import parse_columns_and_rows
 
 
 def make_mysql_command(
-    database=None,
-    user=None,
-    password=None,
-    host=None,
-    port=None,
+    database: str = None,
+    user: str = None,
+    password: str = None,
+    host: str = None,
+    port: int = None,
     executable="mysql",
 ):
     target_bits = [executable]
 
     if database:
         target_bits.append(database)
 
@@ -33,15 +33,15 @@
 
     if port:
         target_bits.append("-P{0}".format(port))
 
     return StringCommand(*target_bits)
 
 
-def make_execute_mysql_command(command, ignore_errors=False, **mysql_kwargs):
+def make_execute_mysql_command(command: str, ignore_errors=False, **mysql_kwargs):
     commands_bits = [
         make_mysql_command(**mysql_kwargs),
         "-Be",
         QuoteString(command),  # quote this whole item as a single shell argument
     ]
 
     if ignore_errors:
@@ -49,14 +49,15 @@
 
     return StringCommand(*commands_bits)
 
 
 class MysqlFactBase(FactBase):
     abstract = True
 
+    mysql_command: str
     requires_command = "mysql"
     ignore_errors = False
 
     def command(
         self,
         # Details for speaking to MySQL via `mysql` CLI via `mysql` CLI
         mysql_user=None,
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/npm.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/npm.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/openrc.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/openrc.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/pacman.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/pacman.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/pip.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/pip.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/postgresql.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/postgres.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from __future__ import annotations
+
 from pyinfra.api import FactBase, MaskString, QuoteString, StringCommand
 from pyinfra.api.util import try_int
 
 from .util.databases import parse_columns_and_rows
 
 
 def make_psql_command(
-    database=None,
-    user=None,
-    password=None,
-    host=None,
-    port=None,
+    database: str = None,
+    user: str = None,
+    password: str = None,
+    host: str = None,
+    port: str = None,
     executable="psql",
-):
-    target_bits = []
+) -> StringCommand:
+    target_bits: list[str] = []
 
     if password:
         target_bits.append(MaskString('PGPASSWORD="{0}"'.format(password)))
 
     target_bits.append(executable)
 
     if database:
@@ -38,17 +40,18 @@
     return StringCommand(
         make_psql_command(**psql_kwargs),
         "-Ac",
         QuoteString(command),  # quote this whole item as a single shell argument
     )
 
 
-class PostgresqlFactBase(FactBase):
+class PostgresFactBase(FactBase):
     abstract = True
 
+    psql_command: str
     requires_command = "psql"
 
     def command(
         self,
         psql_user=None,
         psql_password=None,
         psql_host=None,
@@ -59,15 +62,15 @@
             user=psql_user,
             password=psql_password,
             host=psql_host,
             port=psql_port,
         )
 
 
-class PostgresqlRoles(PostgresqlFactBase):
+class PostgresRoles(PostgresFactBase):
     """
     Returns a dict of PostgreSQL roles and data:
 
     .. code:: python
 
         {
             "pyinfra": {
@@ -111,15 +114,15 @@
                     details[key] = value == "t"
 
             users[details.pop("name")] = details
 
         return users
 
 
-class PostgresqlDatabases(PostgresqlFactBase):
+class PostgresDatabases(PostgresFactBase):
     """
     Returns a dict of PostgreSQL databases and metadata:
 
     .. code:: python
 
         {
             "pyinfra_stuff": {
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/rpm.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/rpm.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/selinux.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/selinux.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 from collections import defaultdict
 
 from pyinfra.api import FactBase
 
 FIELDS = ["user", "role", "type", "level"]  # order is significant, do not change
 
@@ -90,15 +92,15 @@
     # example output: amqp_port_t                    tcp      15672, 5671-5672  # noqa: SC100
     _regex = re.compile(r"^([\w_]+)\s+(\w+)\s+([\w\-,\s]+)$")
 
     def command(self):
         return "semanage port -ln"
 
     def process(self, output):
-        labels = defaultdict(dict)
+        labels: dict[str, dict] = defaultdict(dict)
         for line in output:
             m = SEPorts._regex.match(line)
             if m is None:  # something went wrong
                 continue
             if m.group(1) == "unreserved_port_t":  # these cover the entire space
                 continue
             for item in m.group(3).split(","):
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/server.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+from __future__ import annotations
+
 import os
 import re
 import shutil
 from datetime import datetime
 from tempfile import mkdtemp
+from typing import Dict, List, NewType, Optional, Union
 
 from dateutil.parser import parse as parse_date
 from distro import distro
+from typing_extensions import NotRequired, TypedDict
 
 from pyinfra.api import FactBase, ShortFactBase
 from pyinfra.api.util import try_int
 
 ISO_DATE_FORMAT = "%Y-%m-%dT%H:%M:%S%z"
 
 
@@ -33,14 +37,22 @@
     """
     Returns the path environment variable of the current user.
     """
 
     command = "echo $PATH"
 
 
+class TmpDir(FactBase):
+    """
+    Returns the temporary directory of the current server, if configured.
+    """
+
+    command = "echo $TMPDIR"
+
+
 class Hostname(FactBase):
     """
     Returns the current hostname of the server.
     """
 
     command = "uname -n"
 
@@ -58,90 +70,96 @@
     Returns the kernel version according to ``uname``.
     """
 
     command = "uname -r"
 
 
 # Deprecated/renamed -> Kernel
-class Os(FactBase):
+class Os(FactBase[str]):
     """
     Returns the OS name according to ``uname``.
 
     .. warning::
         This fact is deprecated/renamed, please use the ``server.Kernel`` fact.
     """
 
     command = "uname -s"
 
 
 # Deprecated/renamed -> KernelVersion
-class OsVersion(FactBase):
+class OsVersion(FactBase[str]):
     """
     Returns the OS version according to ``uname``.
 
     .. warning::
         This fact is deprecated/renamed, please use the ``server.KernelVersion`` fact.
     """
 
     command = "uname -r"
 
 
-class Arch(FactBase):
+class Arch(FactBase[str]):
     """
     Returns the system architecture according to ``uname``.
     """
 
     # ``uname -p`` is not portable and returns ``unknown`` on Debian.
     # ``uname -m`` works on most Linux and BSD systems.
     command = "uname -m"
 
 
-class Command(FactBase):
+class Command(FactBase[str]):
     """
     Returns the raw output lines of a given command.
     """
 
     @staticmethod
     def command(command):
         return command
 
 
-class Which(FactBase):
+class Which(FactBase[Optional[str]]):
     """
     Returns the path of a given command, if available.
     """
 
     @staticmethod
     def command(command):
         return "which {0} || true".format(command)
 
 
-class Date(FactBase):
+class Date(FactBase[datetime]):
     """
     Returns the current datetime on the server.
     """
 
     command = f"date +'{ISO_DATE_FORMAT}'"
     default = datetime.now
 
     @staticmethod
-    def process(output):
+    def process(output) -> datetime:
         return datetime.strptime(output[0], ISO_DATE_FORMAT)
 
 
-class MacosVersion(FactBase):
+class MacosVersion(FactBase[str]):
     """
     Returns the installed MacOS version.
     """
 
     command = "sw_vers -productVersion"
     requires_command = "sw_vers"
 
 
-class Mounts(FactBase):
+class MountsDict(TypedDict):
+    device: str
+    type: str
+    options: list[str]
+
+
+class Mounts(FactBase[Dict[str, MountsDict]]):
     """
     Returns a dictionary of mounted filesystems and information.
 
     .. code:: python
 
         {
             "/": {
@@ -155,16 +173,16 @@
         }
     """
 
     command = "mount"
     default = dict
 
     @staticmethod
-    def process(output):
-        devices = {}
+    def process(output) -> dict[str, MountsDict]:
+        devices: dict[str, MountsDict] = {}
 
         for line in output:
             is_map = False
             if line.startswith("map "):
                 line = line[4:]
                 is_map = True
 
@@ -281,18 +299,23 @@
             "fs.inode-state": [
                 44565,
                 360,
             ],
         }
     """
 
-    command = "sysctl -a"
     default = dict
 
     @staticmethod
+    def command(keys=None):
+        if keys is None:
+            return "sysctl -a"
+        return f"sysctl {' '.join(keys)}"
+
+    @staticmethod
     def process(output):
         sysctls = {}
 
         for line in output:
             key = values = None
 
             if "=" in line:
@@ -313,34 +336,47 @@
                         values = values[0]
 
                 sysctls[key] = values
 
         return sysctls
 
 
-class Groups(FactBase):
+class Groups(FactBase[List[str]]):
     """
     Returns a list of groups on the system.
     """
 
     command = "cat /etc/group"
     default = list
 
     @staticmethod
-    def process(output):
-        groups = []
+    def process(output) -> list[str]:
+        groups: list[str] = []
 
         for line in output:
             if ":" in line:
                 groups.append(line.split(":")[0])
 
         return groups
 
 
-class Crontab(FactBase):
+CrontabCommand = NewType("CrontabCommand", int)
+
+
+class CrontabDict(TypedDict):
+    minute: NotRequired[Union[int, str]]
+    hour: NotRequired[Union[int, str]]
+    month: NotRequired[Union[int, str]]
+    day_of_month: NotRequired[Union[int, str]]
+    day_of_week: NotRequired[Union[int, str]]
+    comments: Optional[list[str]]
+    special_time: NotRequired[str]
+
+
+class Crontab(FactBase[Dict[CrontabCommand, CrontabDict]]):
     """
     Returns a dictionary of cron command -> execution time.
 
     .. code:: python
 
         {
             "/path/to/command": {
@@ -364,15 +400,15 @@
     def command(user=None):
         if user:
             return "crontab -l -u {0} || true".format(user)
         return "crontab -l || true"
 
     @staticmethod
     def process(output):
-        crons = {}
+        crons: dict[Command, CrontabDict] = {}
         current_comments = []
 
         for line in output:
             line = line.strip()
             if not line or line.startswith("#"):
                 current_comments.append(line)
                 continue
@@ -413,35 +449,37 @@
                 "groups": [
                     "other",
                     "groups"
                 ],
                 "uid": user_id,
                 "gid": main_user_group_id,
                 "lastlog": last_login_time,
+                "password": encrypted_password,
             },
         }
     """
 
     command = """
         for i in `cat /etc/passwd | cut -d: -f1`; do
             ENTRY=`grep ^$i: /etc/passwd`;
             LASTLOG_RAW=`(lastlog -u $i 2> /dev/null || lastlogin $i 2> /dev/null)`;
             LASTLOG=`echo $LASTLOG_RAW | grep ^$i | tr -s ' '`;
-            echo "$ENTRY|`id -gn $i`|`id -Gn $i`|$LASTLOG";
+            PASSWORD=`grep ^$i: /etc/shadow | cut -d: -f2`;
+            echo "$ENTRY|`id -gn $i`|`id -Gn $i`|$LASTLOG|$PASSWORD";
         done
     """.strip()
 
     default = dict
 
     def process(self, output):
         users = {}
         rex = r"[A-Z][a-z]{2} [A-Z][a-z]{2} {1,2}\d+ .+$"
 
         for line in output:
-            entry, group, user_groups, lastlog = line.split("|")
+            entry, group, user_groups, lastlog, password = line.rsplit("|", 4)
 
             if entry:
                 # Parse out the comment/home/shell
                 entries = entry.split(":")
 
                 # Parse groups
                 groups = []
@@ -466,20 +504,28 @@
                     "shell": entries[6] or None,
                     "group": group,
                     "groups": groups,
                     "uid": int(entries[2]),
                     "gid": int(entries[3]),
                     "lastlog": raw_login_time,
                     "login_time": login_time,
+                    "password": password,
                 }
 
         return users
 
 
-class LinuxDistribution(FactBase):
+class LinuxDistributionDict(TypedDict):
+    name: Optional[str]
+    major: Optional[int]
+    minor: Optional[int]
+    release_meta: Dict
+
+
+class LinuxDistribution(FactBase[LinuxDistributionDict]):
     """
     Returns a dict of the Linux distribution version. Ubuntu, Debian, CentOS,
     Fedora & Gentoo currently. Also contains any key/value items located in
     release files.
 
     .. code:: python
 
@@ -509,23 +555,23 @@
         "opensuse": "openSUSE",
         "rhel": "RedHat",
         "ubuntu": "Ubuntu",
         "debian": "Debian",
     }
 
     @staticmethod
-    def default():
+    def default() -> LinuxDistributionDict:
         return {
             "name": None,
             "major": None,
             "minor": None,
             "release_meta": {},
         }
 
-    def process(self, output):
+    def process(self, output) -> LinuxDistributionDict:
         parts = {}
         for part in "\n".join(output).strip().split("---"):
             if not part.strip():
                 continue
             try:
                 filename, content = part.strip().split("\n", 1)
                 parts[filename] = content
@@ -571,61 +617,65 @@
 
         finally:
             shutil.rmtree(temp_root)
 
         return release_info
 
 
-class LinuxName(ShortFactBase):
+class LinuxName(ShortFactBase[str]):
     """
     Returns the name of the Linux distribution. Shortcut for
     ``host.get_fact(LinuxDistribution)['name']``.
     """
 
     fact = LinuxDistribution
 
     @staticmethod
     def process_data(data):
         return data["name"]
 
 
-class Selinux(FactBase):
+class SelinuxDict(TypedDict):
+    mode: Optional[str]
+
+
+class Selinux(FactBase[SelinuxDict]):
     """
     Discovers the SELinux related facts on the target host.
 
     .. code:: python
 
         {
             "mode": "enabled",
         }
     """
 
     command = "sestatus"
     requires_command = "sestatus"
 
     @staticmethod
-    def default():
+    def default() -> SelinuxDict:
         return {
             "mode": None,
         }
 
-    def process(self, output):
+    def process(self, output) -> SelinuxDict:
         selinux_info = self.default()
 
         match = re.match(r"^SELinux status:\s+(\S+)", "\n".join(output))
 
         if not match:
             return selinux_info
 
         selinux_info["mode"] = match.group(1)
 
         return selinux_info
 
 
-class LinuxGui(FactBase):
+class LinuxGui(FactBase[List[str]]):
     """
     Returns a list of available Linux GUIs.
     """
 
     command = "ls /usr/bin/*session || true"
     default = list
 
@@ -633,47 +683,129 @@
         "/usr/bin/gnome-session": "GNOME",
         "/usr/bin/mate-session": "MATE",
         "/usr/bin/lxsession": "LXDE",
         "/usr/bin/plasma_session": "KDE Plasma",
         "/usr/bin/xfce4-session": "XFCE 4",
     }
 
-    def process(self, output):
+    def process(self, output) -> list[str]:
         gui_names = []
 
         for line in output:
             gui_name = self.known_gui_binaries.get(line)
             if gui_name:
                 gui_names.append(gui_name)
 
         return gui_names
 
 
-class HasGui(ShortFactBase):
+class HasGui(ShortFactBase[bool]):
     """
     Returns a boolean indicating the remote side has GUI capabilities. Linux only.
     """
 
     fact = LinuxGui
 
     @staticmethod
-    def process_data(data):
+    def process_data(data) -> bool:
         return len(data) > 0
 
 
-class Locales(FactBase):
+class Locales(FactBase[List[str]]):
     """
     Returns installed locales on the target host.
 
     .. code:: python
 
         ["C.UTF-8", "en_US.UTF-8"]
     """
 
     command = "locale -a"
     requires_command = "locale"
     default = list
 
-    def process(self, output):
+    def process(self, output) -> list[str]:
         # replace utf8 with UTF-8 to match names in /etc/locale.gen
         # return a list of enabled locales
         return [line.replace("utf8", "UTF-8") for line in output]
+
+
+class SecurityLimits(FactBase):
+    """
+    Returns a list of security limits on the target host.
+
+    .. code:: python
+
+        [
+            {
+                "domain": "*",
+                "limit_type": "soft",
+                "item": "nofile",
+                "value": "1048576"
+            },
+            {
+                "domain": "*",
+                "limit_type": "hard",
+                "item": "nofile",
+                "value": "1048576"
+            },
+            {
+                "domain": "root",
+                "limit_type": "soft",
+                "item": "nofile",
+                "value": "1048576"
+            },
+            {
+                "domain": "root",
+                "limit_type": "hard",
+                "item": "nofile",
+                "value": "1048576"
+            },
+            {
+                "domain": "*",
+                "limit_type": "soft",
+                "item": "memlock",
+                "value": "unlimited"
+            },
+            {
+                "domain": "*",
+                "limit_type": "hard",
+                "item": "memlock",
+                "value": "unlimited"
+            },
+            {
+                "domain": "root",
+                "limit_type": "soft",
+                "item": "memlock",
+                "value": "unlimited"
+            },
+            {
+                "domain": "root",
+                "limit_type": "hard",
+                "item": "memlock",
+                "value": "unlimited"
+            }
+        ]
+    """
+
+    command = "cat /etc/security/limits.conf"
+    default = list
+
+    def process(self, output):
+        limits = []
+
+        for line in output:
+            if line.startswith("#") or not len(line.strip()):
+                continue
+
+            domain, limit_type, item, value = line.split()
+
+            limits.append(
+                {
+                    "domain": domain,
+                    "limit_type": limit_type,
+                    "item": item,
+                    "value": value,
+                },
+            )
+
+        return limits
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/snap.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/snap.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/systemd.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/systemd.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
+from typing import Dict, Iterable
 
-from pyinfra.api import FactBase
+from pyinfra.api import FactBase, FactTypeError, QuoteString, StringCommand
 
 # Valid unit names consist of a "name prefix" and a dot and a suffix specifying the unit type.
 # The "unit prefix" must consist of one or more valid characters
 # (ASCII letters, digits, ":", "-", "_", ".", and "\").
 # The total length of the unit name including the suffix must not exceed 256 characters.
 # The type suffix must be one of
 # ".service", ".socket", ".device", ".mount", ".automount",
@@ -17,29 +18,27 @@
     r"[a-zA-Z0-9\:\-\_\.\\\@]+\."
     r"(?:service|socket|device|mount|automount|swap|target|path|timer|slice|scope)"
 )
 
 
 def _make_systemctl_cmd(user_mode=False, machine=None, user_name=None):
     # base command for normal and user mode
-    systemctl_cmd = "systemctl --user" if user_mode else "systemctl"
+    systemctl_cmd = ["systemctl --user"] if user_mode else ["systemctl"]
 
     # add user and machine flag if given in args
     if machine is not None:
         if user_name is not None:
-            machine_opt = "--machine={1}@{0}".format(machine, user_name)
+            systemctl_cmd.append("--machine={1}@{0}".format(machine, user_name))
         else:
-            machine_opt = "--machine={0}".format(machine)
+            systemctl_cmd.append("--machine={0}".format(machine))
 
-        systemctl_cmd = "{0} {1}".format(systemctl_cmd, machine_opt)
+    return StringCommand(*systemctl_cmd)
 
-    return systemctl_cmd
 
-
-class SystemdStatus(FactBase):
+class SystemdStatus(FactBase[Dict[str, bool]]):
     """
     Returns a dictionary map of systemd units to booleans indicating whether they are active.
 
     + user_mode: whether to use user mode
     + machine: machine name
 
     .. code:: python
@@ -54,25 +53,43 @@
     requires_command = "systemctl"
 
     default = dict
 
     state_key = "SubState"
     state_values = ["running", "waiting", "exited"]
 
-    def command(self, user_mode=False, machine=None, user_name=None):
+    def command(self, user_mode=False, machine=None, user_name=None, services=None):
         fact_cmd = _make_systemctl_cmd(
             user_mode=user_mode,
             machine=machine,
             user_name=user_name,
         )
 
-        return f"{fact_cmd} show --all --property Id --property {self.state_key} '*'"
+        if services is None:
+            service_strs = [QuoteString("*")]
+        elif isinstance(services, str):
+            service_strs = [QuoteString(services)]
+        elif isinstance(services, Iterable):
+            service_strs = [QuoteString(s) for s in services]
+        else:
+            raise FactTypeError(f"Invalid type passed for services argument: {type(services)}")
+
+        return StringCommand(
+            fact_cmd,
+            "show",
+            "--all",
+            "--property",
+            "Id",
+            "--property",
+            self.state_key,
+            *service_strs,
+        )
 
-    def process(self, output):
-        services = {}
+    def process(self, output) -> Dict[str, bool]:
+        services: Dict[str, bool] = {}
 
         current_unit = None
         for line in output:
             line = line.strip()
 
             try:
                 key, value = line.split("=", 1)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/upstart.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/upstart.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/util/__init__.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/util/databases.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/util/databases.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/util/win_files.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/util/win_files.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/vzctl.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/vzctl.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/yum.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/yum.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/facts/zypper.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/facts/zypper.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/local.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/local.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import click
 
 import pyinfra
 from pyinfra import config, host, logger, state
 from pyinfra.api.exceptions import PyinfraError
 from pyinfra.api.util import get_file_path
-from pyinfra.connectors.util import run_local_process, split_combined_output
+from pyinfra.connectors.util import run_local_process
 from pyinfra.context import ctx_state
 
 
 def include(filename: str):
     """
     Executes a local python file within the ``pyinfra.state.cwd``
     directory.
@@ -72,25 +72,24 @@
 
     for command in commands:
         print_prefix = "localhost: "
 
         if print_input:
             click.echo("{0}>>> {1}".format(print_prefix, command), err=True)
 
-        return_code, combined_output = run_local_process(
+        return_code, output = run_local_process(
             command,
             print_output=print_output,
             print_prefix=print_prefix,
         )
-        stdout, stderr = split_combined_output(combined_output)
 
         if return_code > 0 and not ignore_errors:
             raise PyinfraError(
-                "Local command failed: {0}\n{1}".format(command, stderr),
+                "Local command failed: {0}\n{1}".format(command, output.stderr),
             )
 
-        all_stdout.extend(stdout)
+        all_stdout.extend(output.stdout_lines)
 
     if not splitlines:
         return "\n".join(all_stdout)
 
     return all_stdout
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/apk.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/apk.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,32 +19,32 @@
 
     if available:
         yield "apk upgrade --available"
     else:
         yield "apk upgrade"
 
 
-_upgrade = upgrade  # noqa: E305
+_upgrade = upgrade._inner  # noqa: E305
 
 
 @operation(is_idempotent=False)
 def update():
     """
     Updates apk repositories.
     """
 
     yield "apk update"
 
 
-_update = update  # noqa: E305
+_update = update._inner  # noqa: E305
 
 
-@operation
+@operation()
 def packages(
-    packages=None,
+    packages: str | list[str] = None,
     present=True,
     latest=False,
     update=False,
     upgrade=False,
 ):
     """
     Add/remove/update apk packages.
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/apt.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/apt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 Manage apt packages and repositories.
 """
 
-from datetime import datetime, timedelta
+from datetime import timedelta
 from urllib.parse import urlparse
 
-from pyinfra import host, state
+from pyinfra import host
 from pyinfra.api import OperationError, operation
 from pyinfra.facts.apt import AptKeys, AptSources, parse_apt_repo
 from pyinfra.facts.deb import DebPackage, DebPackages
 from pyinfra.facts.files import File
 from pyinfra.facts.gpg import GpgKey
 from pyinfra.facts.server import Date
 
 from . import files
 from .util.packaging import ensure_packages
 
 APT_UPDATE_FILENAME = "/var/lib/apt/periodic/update-success-stamp"
 
 
-def noninteractive_apt(command, force=False):
+def noninteractive_apt(command: str, force=False):
     args = ["DEBIAN_FRONTEND=noninteractive apt-get -y"]
 
     if force:
         args.append("--force-yes")
 
     args.extend(
         (
@@ -32,16 +32,16 @@
             command,
         ),
     )
 
     return " ".join(args)
 
 
-@operation
-def key(src=None, keyserver=None, keyid=None):
+@operation()
+def key(src: str = None, keyserver: str = None, keyid: str = None):
     """
     Add apt gpg keys with ``apt-key``.
 
     + src: filename or URL
     + keyserver: URL of keyserver to fetch key from
     + keyid: key ID or list of key IDs when using keyserver
 
@@ -74,18 +74,14 @@
         if not keyid or not all(kid in existing_keys for kid in keyid):
             # If URL, wget the key to stdout and pipe into apt-key, because the "adv"
             # apt-key passes to gpg which doesn't always support https!
             if urlparse(src).scheme:
                 yield "(wget -O - {0} || curl -sSLf {0}) | apt-key add -".format(src)
             else:
                 yield "apt-key add {0}".format(src)
-
-            if keyid:
-                for kid in keyid:
-                    existing_keys[kid] = {}
         else:
             host.noop("All keys from {0} are already available in the apt keychain".format(src))
 
     if keyserver:
         if not keyid:
             raise OperationError("`keyid` must be provided with `keyserver`")
 
@@ -94,26 +90,24 @@
 
         needed_keys = sorted(set(keyid) - set(existing_keys.keys()))
         if needed_keys:
             yield "apt-key adv --keyserver {0} --recv-keys {1}".format(
                 keyserver,
                 " ".join(needed_keys),
             )
-            for kid in keyid:
-                existing_keys[kid] = {}
         else:
             host.noop(
                 "Keys {0} are already available in the apt keychain".format(
                     ", ".join(keyid),
                 ),
             )
 
 
-@operation
-def repo(src, present=True, filename=None):
+@operation()
+def repo(src: str, present=True, filename: str = None):
     """
     Add/remove apt repositories.
 
     + src: apt source string eg ``deb http://X hardy main``
     + present: whether the repo should exist on the system
     + filename: optional filename to use ``/etc/apt/sources.list.d/<filename>.list``. By
       default uses ``/etc/apt/sources.list``.
@@ -140,43 +134,39 @@
     is_present = False
     repo = parse_apt_repo(src)
     if repo and repo in apt_sources:
         is_present = True
 
     # Doesn't exist and we want it
     if not is_present and present:
-        yield from files.line(
-            filename,
-            src,
+        yield from files.line._inner(
+            path=filename,
+            line=src,
             escape_regex_characters=True,
         )
-        apt_sources.append(repo)
 
     # Exists and we don't want it
     elif is_present and not present:
-        yield from files.line(
-            filename,
-            src,
+        yield from files.line._inner(
+            path=filename,
+            line=src,
             present=False,
-            assume_present=True,
             escape_regex_characters=True,
         )
-        apt_sources.remove(repo)
-
     else:
         host.noop(
             'apt repo "{0}" {1}'.format(
                 src,
                 "exists" if present else "does not exist",
             ),
         )
 
 
 @operation(is_idempotent=False)
-def ppa(src, present=True):
+def ppa(src: str, present=True):
     """
     Add/remove Ubuntu ppa repositories.
 
     + src: the PPA name (full ppa:user/repo format)
     + present: whether it should exist
 
     Note:
@@ -197,16 +187,16 @@
     if present:
         yield 'apt-add-repository -y "{0}"'.format(src)
 
     if not present:
         yield 'apt-add-repository -y --remove "{0}"'.format(src)
 
 
-@operation
-def deb(src, present=True, force=False):
+@operation()
+def deb(src: str, present=True, force=False):
     """
     Add/remove ``.deb`` file packages.
 
     + src: filename or URL of the ``.deb`` file
     + present: whether or not the package should exist on the system
     + force: whether to force the package install by passing `--force-yes` to apt
 
@@ -230,18 +220,18 @@
     """
 
     original_src = src
 
     # If source is a url
     if urlparse(src).scheme:
         # Generate a temp filename
-        temp_filename = state.get_temp_filename(src)
+        temp_filename = host.get_temp_filename(src)
 
         # Ensure it's downloaded
-        yield from files.download(src, temp_filename)
+        yield from files.download._inner(src=src, dest=temp_filename)
 
         # Override the source with the downloaded file
         src = temp_filename
 
     # Check for file .deb information (if file is present)
     info = host.get_fact(DebPackage, name=src)
     current_packages = host.get_fact(DebPackages)
@@ -262,40 +252,36 @@
             # Install .deb file - ignoring failure (on unmet dependencies)
             yield "dpkg --force-confdef --force-confold -i {0} 2> /dev/null || true".format(src)
             # Attempt to install any missing dependencies
             yield "{0} -f".format(noninteractive_apt("install", force=force))
             # Now reinstall, and critically configure, the package - if there are still
             # missing deps, now we error
             yield "dpkg --force-confdef --force-confold -i {0}".format(src)
-
-            if info:
-                current_packages[info["name"]] = [info.get("version")]
         else:
             host.noop("deb {0} is installed".format(original_src))
 
     # Package exists but we don't want?
     if not present:
         if exists:
             yield "{0} {1}".format(
                 noninteractive_apt("remove", force=force),
                 info["name"],
             )
-            current_packages.pop(info["name"])
         else:
             host.noop("deb {0} is not installed".format(original_src))
 
 
 @operation(
     is_idempotent=False,
     idempotent_notice=(
         "This operation will always execute commands "
         "unless the ``cache_time`` argument is provided."
     ),
 )
-def update(cache_time=None):
+def update(cache_time: int = None):
     """
     Updates apt repositories.
 
     + cache_time: cache updates for this many seconds
 
     **Example:**
 
@@ -322,22 +308,14 @@
     yield "apt-get update"
 
     # Some apt systems (Debian) have the /var/lib/apt/periodic directory, but
     # don't bother touching anything in there - so pyinfra does it, enabling
     # cache_time to work.
     if cache_time:
         yield "touch {0}".format(APT_UPDATE_FILENAME)
-        if cache_info is None:
-            host.create_fact(
-                File,
-                kwargs={"path": APT_UPDATE_FILENAME},
-                data={"mtime": datetime.utcnow()},
-            )
-        else:
-            cache_info["mtime"] = datetime.utcnow()
 
 
 _update = update  # noqa: E305
 
 
 @operation(is_idempotent=False)
 def upgrade(auto_remove: bool = False):
@@ -386,27 +364,27 @@
             name="Upgrade apt packages using dist-upgrade",
         )
     """
 
     yield noninteractive_apt("dist-upgrade")
 
 
-@operation
+@operation()
 def packages(
-    packages=None,
+    packages: str | list[str] = None,
     present=True,
     latest=False,
     update=False,
-    cache_time=None,
+    cache_time: int = None,
     upgrade=False,
     force=False,
     no_recommends=False,
     allow_downgrades=False,
-    extra_install_args=None,
-    extra_uninstall_args=None,
+    extra_install_args: str = None,
+    extra_uninstall_args: str = None,
 ):
     """
     Install/remove/update packages & update apt.
 
     + packages: list of packages to ensure
     + present: whether the packages should be installed
     + latest: whether to upgrade packages without a specified version
@@ -450,37 +428,37 @@
             name="Install kernel headers",
             packages=[f"linux-headers-{host.get_fact(OsVersion)}"],
             update=True,
         )
     """
 
     if update:
-        yield from _update(cache_time=cache_time)
+        yield from _update._inner(cache_time=cache_time)
 
     if upgrade:
-        yield from _upgrade()
+        yield from _upgrade._inner()
 
-    install_command = ["install"]
+    install_command_args = ["install"]
     if no_recommends is True:
-        install_command.append("--no-install-recommends")
+        install_command_args.append("--no-install-recommends")
     if allow_downgrades:
-        install_command.append("--allow-downgrades")
+        install_command_args.append("--allow-downgrades")
 
-    upgrade_command = " ".join(install_command)
+    upgrade_command = " ".join(install_command_args)
 
     if extra_install_args:
-        install_command.append(extra_install_args)
+        install_command_args.append(extra_install_args)
 
-    install_command = " ".join(install_command)
+    install_command = " ".join(install_command_args)
 
-    uninstall_command = ["remove"]
+    uninstall_command_args = ["remove"]
     if extra_uninstall_args:
-        uninstall_command.append(extra_uninstall_args)
+        uninstall_command_args.append(extra_uninstall_args)
 
-    uninstall_command = " ".join(uninstall_command)
+    uninstall_command = " ".join(uninstall_command_args)
 
     # Compare/ensure packages are present/not
     yield from ensure_packages(
         host,
         packages,
         host.get_fact(DebPackages),
         present,
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/brew.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/brew.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Manage brew packages on mac/OSX. See https://brew.sh/
 """
 
+import urllib
+
 from pyinfra import host
-from pyinfra.api import operation
+from pyinfra.api import Host, operation
 from pyinfra.facts.brew import BrewCasks, BrewPackages, BrewTaps, BrewVersion, new_cask_cli
 
 from .util.packaging import ensure_packages
 
 
 @operation(is_idempotent=False)
 def update():
@@ -29,17 +31,17 @@
 
     yield "brew upgrade"
 
 
 _upgrade = upgrade  # noqa: E305
 
 
-@operation
+@operation()
 def packages(
-    packages=None,
+    packages: str | list[str] = None,
     present=True,
     latest=False,
     update=False,
     upgrade=False,
 ):
     """
     Add/remove/update brew packages.
@@ -69,53 +71,48 @@
             name="Install latest Vim",
             packages=["vim"],
             latest=True,
         )
     """
 
     if update:
-        yield from _update()
+        yield from _update._inner()
 
     if upgrade:
-        yield from _upgrade()
+        yield from _upgrade._inner()
 
     yield from ensure_packages(
         host,
         packages,
         host.get_fact(BrewPackages),
         present,
         install_command="brew install",
         uninstall_command="brew uninstall",
         upgrade_command="brew upgrade",
         version_join="@",
         latest=latest,
     )
 
 
-def cask_args(host):
+def cask_args():
     return ("", " --cask") if new_cask_cli(host.get_fact(BrewVersion)) else ("cask ", "")
 
 
-@operation(
-    is_idempotent=False,
-    pipeline_facts={"brew_version": ""},
-)
+@operation(is_idempotent=False)
 def cask_upgrade():
     """
     Upgrades all brew casks.
     """
 
-    yield "brew %supgrade%s" % cask_args(host)
+    yield "brew %supgrade%s" % cask_args()
 
 
-@operation(
-    pipeline_facts={"brew_version": ""},
-)
+@operation()
 def casks(
-    casks=None,
+    casks: str | list[str] = None,
     present=True,
     latest=False,
     upgrade=False,
 ):
     """
     Add/remove/update brew casks.
 
@@ -137,66 +134,96 @@
             upgrade=True,
             latest=True,
         )
 
     """
 
     if upgrade:
-        yield from cask_upgrade()
+        yield from cask_upgrade._inner()
 
-    args = cask_args(host)
+    args = cask_args()
 
     yield from ensure_packages(
         host,
         casks,
         host.get_fact(BrewCasks),
         present,
         install_command="brew %sinstall%s" % args,
         uninstall_command="brew %suninstall%s" % args,
         upgrade_command="brew %supgrade%s" % args,
         version_join="@",
         latest=latest,
     )
 
 
-@operation
-def tap(src, present=True):
+@operation()
+def tap(src: str = None, present=True, url: str = None):
     """
     Add/remove brew taps.
 
     + src: the name of the tap
     + present: whether this tap should be present or not
+    + url: the url of the tap. See https://docs.brew.sh/Taps
 
     **Examples:**
 
     .. code:: python
 
         brew.tap(
             name="Add a brew tap",
             src="includeos/includeos",
         )
 
+        # Just url is equivalent to
+        # `brew tap kptdev/kpt https://github.com/kptdev/kpt`
+        brew.tap(
+            url="https://github.com/kptdev/kpt",
+        )
+
+        # src and url is equivalent to
+        # `brew tap example/project https://github.example.com/project`
+        brew.tap(
+            src="example/project",
+            url="https://github.example.com/project",
+        )
+
         # Multiple taps
         for tap in ["includeos/includeos", "ktr0731/evans"]:
             brew.tap(
                 name={f"Add brew tap {tap}"},
                 src=tap,
             )
 
     """
 
+    if not (src or url):
+        host.noop("no tap was specified")
+        return
+
+    src = src or urllib.parse.urlparse(url).path.strip("/")
+
+    if len(src.split("/")) != 2:
+        host.noop("src '{0}' doesn't have two components.".format(src))
+        return
+
     taps = host.get_fact(BrewTaps)
-    is_tapped = src in taps
+    already_tapped = src in taps
+
+    if present and already_tapped:
+        host.noop("tap {0} already exists".format(src))
+        return
+
+    if already_tapped:
+        yield "brew untap {0}".format(src)
+        return
+
+    if not present:
+        host.noop("tap {0} does not exist".format(src))
+        return
+
+    cmd = "brew tap {0}".format(src)
+
+    if url is not None:
+        cmd = " ".join([cmd, url])
 
-    if present:
-        if is_tapped:
-            host.noop("tap {0} already exists".format(src))
-        else:
-            yield "brew tap {0}".format(src)
-            taps.append(src)
-
-    elif not present:
-        if is_tapped:
-            yield "brew untap {0}".format(src)
-            taps.remove(src)
-        else:
-            host.noop("tap {0} does not exist".format(src))
+    yield cmd
+    return
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/bsdinit.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/bsdinit.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from pyinfra.facts.bsdinit import RcdStatus
 from pyinfra.facts.server import Os
 
 from . import files
 from .util.service import handle_service_control
 
 
-@operation
+@operation()
 def service(
-    service,
+    service: str,
     running=True,
     restarted=False,
     reloaded=False,
-    command=None,
-    enabled=None,
+    command: str = None,
+    enabled: bool = None,
 ):
     """
     Manage the state of BSD init services.
 
     + service: name of the service to manage
     + running: whether the service should be running
     + restarted: whether the service should be restarted
@@ -45,13 +45,13 @@
         reloaded,
         command,
         status_argument=status_argument,
     )
 
     # BSD init is simple, just add/remove <service>_enabled="YES"
     if isinstance(enabled, bool):
-        yield from files.line(
-            "/etc/rc.conf.local",
-            "^{0}_enable=".format(service),
+        yield from files.line._inner(
+            path="/etc/rc.conf.local",
+            line="^{0}_enable=".format(service),
             replace='{0}_enable="YES"'.format(service),
             present=enabled,
         )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/cargo.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/cargo.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from pyinfra import host
 from pyinfra.api import operation
 from pyinfra.facts.cargo import CargoPackages
 
 from .util.packaging import ensure_packages
 
 
-@operation
-def packages(packages=None, present=True, latest=False):
+@operation()
+def packages(packages: str | list[str] = None, present=True, latest=False):
     """
     Install/remove/update cargo packages.
 
     + packages: list of packages to ensure
     + present: whether the packages should be present
     + latest: whether to upgrade packages without a specified version
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/choco.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/choco.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from pyinfra import host
 from pyinfra.api import operation
 from pyinfra.facts.choco import ChocoPackages
 
 from .util.packaging import ensure_packages
 
 
-@operation
-def packages(packages=None, present=True, latest=False):
+@operation()
+def packages(packages: str | list[str] = None, present=True, latest=False):
     """
     Add/remove/update ``choco`` packages.
 
     + packages: list of packages to ensure
     + present: whether the packages should be installed
     + latest: whether to upgrade packages without a specified version
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/dnf.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/yum.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,214 +1,211 @@
 """
-Manage dnf packages and repositories. Note that dnf package names are case-sensitive.
+Manage yum packages and repositories. Note that yum package names are case-sensitive.
 """
 
 from pyinfra import host, state
 from pyinfra.api import operation
 from pyinfra.facts.rpm import RpmPackageProvides, RpmPackages
 
-from . import files
 from .util.packaging import ensure_packages, ensure_rpm, ensure_yum_repo
 
 
 @operation(is_idempotent=False)
-def key(src):
+def key(src: str):
     """
-    Add dnf gpg keys with ``rpm``.
+    Add yum gpg keys with ``rpm``.
 
-    + key: filename or URL
+    + src: filename or URL
 
     Note:
-        always returns one command, not idempotent
+        always returns one command, not state checking
 
     **Example:**
 
     .. code:: python
 
         linux_id = host.get_fact(LinuxDistribution)["release_meta"].get("ID")
-        dnf.key(
+        yum.key(
             name="Add the Docker CentOS gpg key",
             src=f"https://download.docker.com/linux/{linux_id}/gpg",
         )
 
     """
 
     yield "rpm --import {0}".format(src)
 
 
-@operation
+@operation()
 def repo(
-    src,
+    src: str,
     present=True,
-    baseurl=None,
-    description=None,
+    baseurl: str = None,
+    description: str = None,
     enabled=True,
     gpgcheck=True,
-    gpgkey=None,
+    gpgkey: str = None,
 ):
-    # NOTE: if updating this docstring also update `yum.repo`
+    # NOTE: if updating this docstring also update `dnf.repo`
     """
-    Add/remove/update dnf repositories.
+    Add/remove/update yum repositories.
 
-    + name: URL or name for the ``.repo``   file
+    + src: URL or name for the ``.repo``   file
     + present: whether the ``.repo`` file should be present
     + baseurl: the baseurl of the repo (if ``name`` is not a URL)
     + description: optional verbose description
     + enabled: whether this repo is enabled
     + gpgcheck: whether set ``gpgcheck=1``
     + gpgkey: the URL to the gpg key for this repo
 
     ``Baseurl``/``description``/``gpgcheck``/``gpgkey``:
-        These are only valid when ``name`` is a filename (ie not a URL). This is
+        These are only valid when ``src`` is a filename (ie not a URL). This is
         for manual construction of repository files. Use a URL to download and
         install remote repository files.
 
     **Examples:**
 
     .. code:: python
 
         # Download a repository file
-        dnf.rpm(
+        yum.repo(
             name="Install Docker-CE repo via URL",
             src="https://download.docker.com/linux/centos/docker-ce.repo",
         )
 
         # Create the repository file from baseurl/etc
-        dnf.repo(
+        yum.repo(
             name="Add the Docker CentOS repo",
             src="DockerCE",
             baseurl="https://download.docker.com/linux/centos/7/$basearch/stable",
         )
     """
 
     yield from ensure_yum_repo(
-        state,
         host,
-        files,
         src,
         baseurl,
         present,
         description,
         enabled,
         gpgcheck,
         gpgkey,
     )
 
 
-@operation
-def rpm(src, present=True):
-    # NOTE: if updating this docstring also update `yum.rpm`
+@operation()
+def rpm(src: str, present=True):
+    # NOTE: if updating this docstring also update `dnf.rpm`
     """
     Add/remove ``.rpm`` file packages.
 
     + src: filename or URL of the ``.rpm`` package
     + present: whether ore not the package should exist on the system
 
     URL sources with ``present=False``:
         If the ``.rpm`` file isn't downloaded, pyinfra can't remove any existing
         package as the file won't exist until mid-deploy.
 
     **Example:**
 
     .. code:: python
 
-        major_centos_version = host.get_fact(LinuxDistribution)["major"]
+        major_version = host.get_fact(LinuxDistribution)["major"]
         dnf.rpm(
            name="Install EPEL rpm to enable EPEL repo",
-           src=f"https://dl.fedoraproject.org/pub/epel/epel-release-latest-{major_centos_version}.noarch.rpm",
+           src=f"https://dl.fedoraproject.org/pub/epel/epel-release-latest-{major_version}.noarch.rpm",
         )
     """
 
-    yield from ensure_rpm(state, host, files, src, present, "dnf")
+    yield from ensure_rpm(host, src, present, "yum")
 
 
 @operation(is_idempotent=False)
 def update():
     """
-    Updates all dnf packages.
+    Updates all yum packages.
     """
 
-    yield "dnf update -y"
+    yield "yum update -y"
 
 
-_update = update  # noqa: E305 (for use below where update is a kwarg)
+_update = update._inner  # noqa: E305 (for use below where update is a kwarg)
 
 
-@operation
+@operation()
 def packages(
-    packages=None,
+    packages: str | list[str] = None,
     present=True,
     latest=False,
     update=False,
     clean=False,
     nobest=False,
-    extra_install_args=None,
-    extra_uninstall_args=None,
+    extra_install_args: str = None,
+    extra_uninstall_args: str = None,
 ):
     """
-    Install/remove/update dnf packages & updates.
+    Install/remove/update yum packages & updates.
 
     + packages: list of packages to ensure
     + present: whether the packages should be installed
     + latest: whether to upgrade packages without a specified version
-    + update: run ``dnf update`` before installing packages
-    + clean: run ``dnf clean`` before installing packages
+    + update: run ``yum update`` before installing packages
+    + clean: run ``yum clean all`` before installing packages
     + nobest: add the no best option to install
-    + extra_install_args: additional arguments to the dnf install command
-    + extra_uninstall_args: additional arguments to the dnf uninstall command
+    + extra_install_args: additional arguments to the yum install command
+    + extra_uninstall_args: additional arguments to the yum uninstall command
 
     Versions:
         Package versions can be pinned as follows: ``<pkg>=<version>``
 
     **Examples:**
 
     .. code:: python
 
         # Update package list and install packages
-        dnf.packages(
-            name='Install Vim and Vim enhanced',
+        yum.packages(
+            name="Install Vim and Vim enhanced",
             packages=["vim-enhanced", "vim"],
             update=True,
         )
 
         # Install the latest versions of packages (always check)
-        dnf.packages(
+        yum.packages(
             name="Install latest Vim",
             packages=["vim"],
             latest=True,
         )
     """
 
     if clean:
-        yield "dnf clean all"
+        yield "yum clean all"
 
     if update:
         yield from _update()
 
-    install_command = ["dnf", "install", "-y"]
+    install_command = ["yum", "install", "-y"]
 
     if nobest:
         install_command.append("--nobest")
 
     if extra_install_args:
         install_command.append(extra_install_args)
 
-    uninstall_command = ["dnf", "remove", "-y"]
+    uninstall_command = ["yum", "remove", "-y"]
 
     if extra_uninstall_args:
         uninstall_command.append(extra_uninstall_args)
 
     yield from ensure_packages(
         host,
         packages,
         host.get_fact(RpmPackages),
         present,
         install_command=" ".join(install_command),
         uninstall_command=" ".join(uninstall_command),
-        upgrade_command="dnf update -y",
+        upgrade_command="yum update -y",
         version_join="=",
         latest=latest,
         expand_package_fact=lambda package: host.get_fact(
             RpmPackageProvides,
             name=package,
         ),
     )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/files.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """
 The files operations handles filesystem state, file uploads and template generation.
 """
 
+from __future__ import annotations
+
 import os
 import posixpath
 import sys
 import traceback
 from datetime import timedelta
 from fnmatch import fnmatch
 from io import StringIO
+from typing import IO, Any, Union
 
 from jinja2 import TemplateRuntimeError, TemplateSyntaxError, UndefinedError
 
-import pyinfra
 from pyinfra import host, logger, state
 from pyinfra.api import (
     FileDownloadCommand,
     FileUploadCommand,
     OperationError,
     OperationTypeError,
+    OperationValueError,
     QuoteString,
     RsyncCommand,
     StringCommand,
     operation,
 )
 from pyinfra.api.command import make_formatted_string_command
 from pyinfra.api.util import (
@@ -49,30 +52,29 @@
 )
 from pyinfra.facts.server import Date, Which
 
 from .util import files as file_utils
 from .util.files import adjust_regex, ensure_mode_int, get_timestamp, sed_replace, unix_path_join
 
 
-@operation(
-    pipeline_facts={"file": "dest"},
-)
+@operation()
 def download(
-    src,
-    dest,
-    user=None,
-    group=None,
-    mode=None,
-    cache_time=None,
+    src: str,
+    dest: str,
+    user: str = None,
+    group: str = None,
+    mode: str = None,
+    cache_time: int = None,
     force=False,
-    sha256sum=None,
-    sha1sum=None,
-    md5sum=None,
-    headers=None,
+    sha256sum: str = None,
+    sha1sum: str = None,
+    md5sum: str = None,
+    headers: dict[str, str] = None,
     insecure=False,
+    proxy: str = None,
 ):
     """
     Download files from remote locations using ``curl`` or ``wget``.
 
     + src: source URL of the file
     + dest: where to save the file
     + user: user to own the files
@@ -81,28 +83,28 @@
     + cache_time: if the file exists already, re-download after this time (in seconds)
     + force: always download the file, even if it already exists
     + sha256sum: sha256 hash to checksum the downloaded file against
     + sha1sum: sha1 hash to checksum the downloaded file against
     + md5sum: md5 hash to checksum the downloaded file against
     + headers: optional dictionary of headers to set for the HTTP request
     + insecure: disable SSL verification for the HTTP request
+    + proxy: simple HTTP proxy through which we can download files, form `http://<yourproxy>:<port>`
 
     **Example:**
 
     .. code:: python
 
         files.download(
             name="Download the Docker repo file",
             src="https://download.docker.com/linux/centos/docker-ce.repo",
             dest="/etc/yum.repos.d/docker-ce.repo",
         )
     """
 
     info = host.get_fact(File, path=dest)
-    host_datetime = host.get_fact(Date).replace(tzinfo=None)
 
     # Destination is a directory?
     if info is False:
         raise OperationError(
             "Destination {0} already exists and is not a file".format(dest),
         )
 
@@ -133,18 +135,24 @@
 
         if md5sum:
             if md5sum != host.get_fact(Md5File, path=dest):
                 download = True
 
     # If we download, always do user/group/mode as SSH user may be different
     if download:
-        temp_file = state.get_temp_filename(dest)
+        temp_file = host.get_temp_filename(dest)
+
+        curl_args: list[Union[str, StringCommand]] = ["-sSLf"]
+        wget_args: list[Union[str, StringCommand]] = ["-q"]
+
+        if proxy:
+            curl_args.append(f"--proxy {proxy}")
+            wget_args.append("-e use_proxy=yes")
+            wget_args.append(f"-e http_proxy={proxy}")
 
-        curl_args = ["-sSLf"]
-        wget_args = ["-q"]
         if insecure:
             curl_args.append("--insecure")
             wget_args.append("--no-check-certificate")
 
         if headers:
             for key, value in headers.items():
                 header_arg = StringCommand("--header", QuoteString(f"{key}: {value}"))
@@ -207,61 +215,40 @@
                     "(( md5sum {0} 2> /dev/null || md5 {0} ) | grep {1}) "
                     "|| ( echo {2} && exit 1 )"
                 ),
                 QuoteString(dest),
                 md5sum,
                 QuoteString("MD5 did not match!"),
             )
-
-        host.create_fact(
-            File,
-            kwargs={"path": dest},
-            data={"mode": mode, "group": group, "user": user, "mtime": host_datetime},
-        )
-
-        # Remove any checksum facts as we don't know the correct values
-        for value, fact_cls in (
-            (sha1sum, Sha1File),
-            (sha256sum, Sha256File),
-            (md5sum, Md5File),
-        ):
-            fact_kwargs = {"path": dest}
-            if value:
-                host.create_fact(fact_cls, kwargs=fact_kwargs, data=value)
-            else:
-                host.delete_fact(fact_cls, kwargs=fact_kwargs)
-
     else:
         host.noop("file {0} has already been downloaded".format(dest))
 
 
-@operation
+@operation()
 def line(
-    path,
-    line,
+    path: str,
+    line: str,
     present=True,
-    replace=None,
-    flags=None,
+    replace: str = None,
+    flags: list[str] = None,
     backup=False,
     interpolate_variables=False,
     escape_regex_characters=False,
-    assume_present=False,
     ensure_newline=False,
 ):
     """
     Ensure lines in files using grep to locate and sed to replace.
 
     + path: target remote file to edit
     + line: string or regex matching the target line
     + present: whether the line should be in the file
     + replace: text to replace entire matching lines when ``present=True``
     + flags: list of flags to pass to sed when replacing/deleting
     + backup: whether to backup the file (see below)
     + interpolate_variables: whether to interpolate variables in ``replace``
-    + assume_present: whether to assume a matching line already exists in the file
     + escape_regex_characters: whether to escape regex characters from the matching line
     + ensure_newline: ensures that the appended line is on a new line
 
     Regex line matching:
         Unless line matches a line (starts with ^, ends $), pyinfra will wrap it such that
         it does, like: ``^.*LINE.*$``. This means we don't swap parts of lines out. To
         change bits of lines, see ``files.replace``.
@@ -340,23 +327,20 @@
     # # put any matches on either side.
     # if not match_line.startswith("^"):
     #     match_line = "^.*{0}".format(match_line)
     # if not match_line.endswith("$"):
     #     match_line = "{0}.*$".format(match_line)
 
     # Is there a matching line in this file?
-    if assume_present:
-        present_lines = [line]
-    else:
-        present_lines = host.get_fact(
-            FindInFile,
-            path=path,
-            pattern=match_line,
-            interpolate_variables=interpolate_variables,
-        )
+    present_lines = host.get_fact(
+        FindInFile,
+        path=path,
+        pattern=match_line,
+        interpolate_variables=interpolate_variables,
+    )
 
     # If replace present, use that over the matching line
     if replace:
         line = replace
     # We must provide some kind of replace to sed_replace_command below
     else:
         replace = ""
@@ -393,104 +377,62 @@
         flags=flags,
         backup=backup,
         interpolate_variables=interpolate_variables,
     )
 
     # No line and we want it, append it
     if not present_lines and present:
-        # If the file does not exist - it *might* be created, so we handle it
-        # dynamically with a little script.
-        if present_lines is None:
-            yield make_formatted_string_command(
-                """
-                    if [ -f '{target}' ]; then
-                        ( grep {match_line} '{target}' && \
-                        {sed_replace_command}) 2> /dev/null || \
-                        {echo_command} ;
-                    else
-                        {echo_command} ;
-                    fi
-                """,
-                target=QuoteString(path),
-                match_line=QuoteString(match_line),
-                echo_command=echo_command,
-                sed_replace_command=sed_replace_command,
+        # If we're doing replacement, only append if the *replacement* line
+        # does not exist (as we are appending the replacement).
+        if replace:
+            # Ensure replace explicitly matches a whole line
+            replace_line = replace
+            if not replace_line.startswith("^"):
+                replace_line = f"^{replace_line}"
+            if not replace_line.endswith("$"):
+                replace_line = f"{replace_line}$"
+
+            present_lines = host.get_fact(
+                FindInFile,
+                path=path,
+                pattern=replace_line,
+                interpolate_variables=interpolate_variables,
             )
 
-        # File exists but has no matching lines - append it.
+        if not present_lines:
+            yield echo_command
         else:
-            # If we're doing replacement, only append if the *replacement* line
-            # does not exist (as we are appending the replacement).
-            if replace:
-                # Ensure replace explicitly matches a whole line
-                replace_line = replace
-                if not replace_line.startswith("^"):
-                    replace_line = f"^{replace_line}"
-                if not replace_line.endswith("$"):
-                    replace_line = f"{replace_line}$"
-
-                present_lines = host.get_fact(
-                    FindInFile,
-                    path=path,
-                    pattern=replace_line,
-                    interpolate_variables=interpolate_variables,
-                )
-
-            if not present_lines:
-                yield echo_command
-            else:
-                host.noop('line "{0}" exists in {1}'.format(replace or line, path))
-
-        host.create_fact(
-            FindInFile,
-            kwargs={
-                "path": path,
-                "pattern": match_line,
-                "interpolate_variables": interpolate_variables,
-            },
-            data=[replace or line],
-        )
+            host.noop('line "{0}" exists in {1}'.format(replace or line, path))
 
     # Line(s) exists and we want to remove them, replace with nothing
     elif present_lines and not present:
         yield sed_replace(
             path,
             match_line,
             "",
             flags=flags,
             backup=backup,
             interpolate_variables=interpolate_variables,
         )
 
-        host.delete_fact(
-            FindInFile,
-            kwargs={
-                "path": path,
-                "pattern": match_line,
-                "interpolate_variables": interpolate_variables,
-            },
-        )
-
     # Line(s) exists and we have want to ensure they're correct
     elif present_lines and present:
         # If any of lines are different, sed replace them
         if replace and any(line != replace for line in present_lines):
             yield sed_replace_command
-            del present_lines[:]  # TODO: use .clear() when py3+
-            present_lines.append(replace)
         else:
             host.noop('line "{0}" exists in {1}'.format(replace or line, path))
 
 
-@operation
+@operation()
 def replace(
-    path,
-    text=None,
-    replace=None,
-    flags=None,
+    path: str,
+    text: str = None,
+    replace: str = None,
+    flags: list[str] = None,
     backup=False,
     interpolate_variables=False,
     match=None,  # deprecated
 ):
     """
     Replace contents of a file using ``sed``.
 
@@ -547,40 +489,29 @@
             path,
             text,
             replace,
             flags=flags,
             backup=backup,
             interpolate_variables=interpolate_variables,
         )
-        host.create_fact(
-            FindInFile,
-            kwargs={
-                "path": path,
-                "pattern": text,
-                "interpolate_variables": interpolate_variables,
-            },
-            data=[],
-        )
     else:
         host.noop('string "{0}" does not exist in {1}'.format(text, path))
 
 
-@operation(
-    pipeline_facts={"find_files": "destination"},
-)
+@operation()
 def sync(
-    src,
-    dest,
-    user=None,
-    group=None,
-    mode=None,
-    dir_mode=None,
+    src: str,
+    dest: str,
+    user: str = None,
+    group: str = None,
+    mode: str = None,
+    dir_mode: str = None,
     delete=False,
-    exclude=None,
-    exclude_dir=None,
+    exclude: str | list[str] | tuple[str] = None,
+    exclude_dir: str | list[str] | tuple[str] = None,
     add_deploy_dir=True,
 ):
     """
     Syncs a local directory with a remote one, with delete support. Note that delete will
     remove extra files on the remote side, but not extra directories.
 
     + src: local directory to sync
@@ -668,35 +599,35 @@
     # Ensure the destination directory - if the destination is a link, ensure
     # the link target is a directory.
     dest_to_ensure = dest
     dest_link_info = host.get_fact(Link, path=dest)
     if dest_link_info:
         dest_to_ensure = dest_link_info["link_target"]
 
-    yield from directory(
-        dest_to_ensure,
+    yield from directory._inner(
+        path=dest_to_ensure,
         user=user,
         group=group,
         mode=dir_mode or get_path_permissions_mode(src),
     )
 
     # Ensure any remote dirnames
     for dir_path_curr, dir_mode_curr in ensure_dirnames:
-        yield from directory(
-            unix_path_join(dest, dir_path_curr),
+        yield from directory._inner(
+            path=unix_path_join(dest, dir_path_curr),
             user=user,
             group=group,
             mode=dir_mode or dir_mode_curr,
         )
 
     # Put each file combination
     for local_filename, remote_filename in put_files:
-        yield from put(
-            local_filename,
-            remote_filename,
+        yield from put._inner(
+            src=local_filename,
+            dest=remote_filename,
             user=user,
             group=group,
             mode=mode or get_path_permissions_mode(local_filename),
             add_deploy_dir=False,
             create_remote_dir=False,  # handled above
         )
 
@@ -706,73 +637,71 @@
         wanted_filenames = set([remote_filename for _, remote_filename in put_files])
         files_to_delete = remote_filenames - wanted_filenames
         for filename in files_to_delete:
             # Should we exclude this file?
             if exclude and any(fnmatch(filename, match) for match in exclude):
                 continue
 
-            yield from file(filename, present=False)
+            yield from file._inner(path=filename, present=False)
 
 
 @memoize
 def show_rsync_warning():
     logger.warning("The `files.rsync` operation is in alpha!")
 
 
 @operation(is_idempotent=False)
-def rsync(src, dest, flags=["-ax", "--delete"]):
+def rsync(src: str, dest: str, flags: list[str] = None):
     """
     Use ``rsync`` to sync a local directory to the remote system. This operation will actually call
     the ``rsync`` binary on your system.
 
     .. important::
         The ``files.rsync`` operation is in alpha, and only supported using SSH
         or ``@local`` connectors. When using the SSH connector, rsync will automatically use the
         StrictHostKeyChecking setting, config and known_hosts file (when specified).
 
     .. caution::
         When using SSH, the ``files.rsync`` operation only supports the ``sudo`` and ``sudo_user``
         global arguments.
     """
 
+    if flags is None:
+        flags = ["-ax", "--delete"]
     show_rsync_warning()
 
     try:
         host.check_can_rsync()
     except NotImplementedError as e:
         raise OperationError(*e.args)
 
     yield RsyncCommand(src, dest, flags)
 
 
-def _create_remote_dir(state, host, remote_filename, user, group):
+def _create_remote_dir(remote_filename, user, group):
     # Always use POSIX style path as local might be Windows, remote always *nix
     remote_dirname = posixpath.dirname(remote_filename)
     if remote_dirname:
-        yield from directory(
+        yield from directory._inner(
             path=remote_dirname,
             user=user,
             group=group,
             _no_check_owner_mode=True,  # don't check existing user/mode
             _no_fail_on_link=True,  # don't fail if the path is a link
         )
 
 
 @operation(
     # We don't (currently) cache the local state, so there's nothing we can
     # update to flag the local file as present.
     is_idempotent=False,
-    pipeline_facts={
-        "file": "src",
-        "sha1_file": "src",
-    },
 )
 def get(
-    src,
-    dest,
+    src: str,
+    dest: str,
     add_deploy_dir=True,
     create_local_dir=False,
     force=False,
 ):
     """
     Download a file from the remote system.
 
@@ -805,42 +734,37 @@
         if not os.path.exists(local_pathname):
             os.makedirs(local_pathname)
 
     remote_file = host.get_fact(File, path=src)
 
     # No remote file, so assume exists and download it "blind"
     if not remote_file or force:
-        yield FileDownloadCommand(src, dest, remote_temp_filename=state.get_temp_filename(dest))
+        yield FileDownloadCommand(src, dest, remote_temp_filename=host.get_temp_filename(dest))
 
     # No local file, so always download
     elif not os.path.exists(dest):
-        yield FileDownloadCommand(src, dest, remote_temp_filename=state.get_temp_filename(dest))
+        yield FileDownloadCommand(src, dest, remote_temp_filename=host.get_temp_filename(dest))
 
     # Remote file exists - check if it matches our local
     else:
         local_sum = get_file_sha1(dest)
         remote_sum = host.get_fact(Sha1File, path=src)
 
         # Check sha1sum, upload if needed
         if local_sum != remote_sum:
-            yield FileDownloadCommand(src, dest, remote_temp_filename=state.get_temp_filename(dest))
+            yield FileDownloadCommand(src, dest, remote_temp_filename=host.get_temp_filename(dest))
 
 
-@operation(
-    pipeline_facts={
-        "file": "dest",
-        "sha1_file": "dest",
-    },
-)
+@operation()
 def put(
-    src,
-    dest,
-    user=None,
-    group=None,
-    mode=None,
+    src: str | IO[Any],
+    dest: str,
+    user: str = None,
+    group: str = None,
+    mode: str = None,
     add_deploy_dir=True,
     create_remote_dir=True,
     force=False,
     assume_exists=False,
 ):
     """
     Upload a local file, or file-like object, to the remote system.
@@ -920,27 +844,27 @@
                 ),
             )
     else:
         mode = ensure_mode_int(mode)
 
     remote_file = host.get_fact(File, path=dest)
 
-    if not remote_file and host.get_fact(Directory, path=dest):
+    if not remote_file and bool(host.get_fact(Directory, path=dest)):
         dest = unix_path_join(dest, os.path.basename(src))
         remote_file = host.get_fact(File, path=dest)
 
     if create_remote_dir:
-        yield from _create_remote_dir(state, host, dest, user, group)
+        yield from _create_remote_dir(dest, user, group)
 
     # No remote file, always upload and user/group/mode if supplied
     if not remote_file or force:
         yield FileUploadCommand(
             local_file,
             dest,
-            remote_temp_filename=state.get_temp_filename(dest),
+            remote_temp_filename=host.get_temp_filename(dest),
         )
 
         if user or group:
             yield file_utils.chown(dest, user, group)
 
         if mode:
             yield file_utils.chmod(dest, mode)
@@ -950,15 +874,15 @@
         remote_sum = host.get_fact(Sha1File, path=dest)
 
         # Check sha1sum, upload if needed
         if local_sum != remote_sum:
             yield FileUploadCommand(
                 local_file,
                 dest,
-                remote_temp_filename=state.get_temp_filename(dest),
+                remote_temp_filename=host.get_temp_filename(dest),
             )
 
             if user or group:
                 yield file_utils.chown(dest, user, group)
 
             if mode:
                 yield file_utils.chmod(dest, mode)
@@ -975,25 +899,25 @@
             if (user and remote_file["user"] != user) or (group and remote_file["group"] != group):
                 yield file_utils.chown(dest, user, group)
                 changed = True
 
             if not changed:
                 host.noop("file {0} is already uploaded".format(dest))
 
-    # Now we've uploaded the file and ensured user/group/mode, update the relevant fact data
-    host.create_fact(Sha1File, kwargs={"path": dest}, data=local_sum)
-    host.create_fact(
-        File,
-        kwargs={"path": dest},
-        data={"user": user, "group": group, "mode": mode},
-    )
 
-
-@operation
-def template(src, dest, user=None, group=None, mode=None, create_remote_dir=True, **data):
+@operation()
+def template(
+    src: str | IO[Any],
+    dest: str,
+    user: str = None,
+    group: str = None,
+    mode: str = None,
+    create_remote_dir=True,
+    **data,
+):
     '''
     Generate a template using jinja2 and write it to the remote system.
 
     + src: template filename or IO-like object
     + dest: remote filename
     + user: user to own the files
     + group: group to own the files
@@ -1067,24 +991,22 @@
     if not hasattr(src, "read") and state.cwd:
         src = os.path.join(state.cwd, src)
 
     # Ensure host/state/inventory are available inside templates (if not set)
     data.setdefault("host", host)
     data.setdefault("state", state)
     data.setdefault("inventory", state.inventory)
-    data.setdefault("facts", pyinfra.facts)
 
     # Render and make file-like it's output
     try:
         output = get_template(src).render(data)
     except (TemplateRuntimeError, TemplateSyntaxError, UndefinedError) as e:
-        trace_frames = traceback.extract_tb(sys.exc_info()[2])
         trace_frames = [
             frame
-            for frame in trace_frames
+            for frame in traceback.extract_tb(sys.exc_info()[2])
             if frame[2] in ("template", "<module>", "top-level template code")
         ]  # thank you https://github.com/saltstack/salt/blob/master/salt/utils/templates.py
 
         line_number = trace_frames[-1][1]
 
         # Quickly read the line in question and one above/below for nicer debugging
         with open(src, "r") as f:
@@ -1100,20 +1022,20 @@
                 e,
                 "\n".join(relevant_lines),
             ),
         )
 
     output_file = StringIO(output)
     # Set the template attribute for nicer debugging
-    output_file.template = src
+    output_file.template = src  # type: ignore[attr-defined]
 
     # Pass to the put function
-    yield from put(
-        output_file,
-        dest,
+    yield from put._inner(
+        src=output_file,
+        dest=dest,
         user=user,
         group=group,
         mode=mode,
         add_deploy_dir=False,
         create_remote_dir=create_remote_dir,
     )
 
@@ -1135,37 +1057,33 @@
             yield StringCommand("mv", QuoteString(path), QuoteString(backup_path))
         else:
             yield StringCommand("rm", "-rf", QuoteString(path))
     else:
         raise OperationError("{0} exists and is not a {1}".format(path, fs_type))
 
 
-@operation(
-    pipeline_facts={"link": "path"},
-)
+@operation()
 def link(
-    path,
-    target=None,
+    path: str,
+    target: str = None,
     present=True,
-    assume_present=False,
-    user=None,
-    group=None,
+    user: str = None,
+    group: str = None,
     symbolic=True,
     create_remote_dir=True,
     force=False,
     force_backup=True,
-    force_backup_dir=None,
+    force_backup_dir: str = None,
 ):
     """
     Add/remove/update links.
 
     + path: the name of the link
     + target: the file/directory the link points to
     + present: whether the link should exist
-    + assume_present: whether to assume the link exists
     + user: user to own the link
     + group: group to own the link
     + symbolic: whether to make a symbolic link (vs hard link)
     + create_remote_dir: create the remote directory if it doesn't exist
     + force: if the target exists and is not a file, move or remove it and continue
     + force_backup: set to ``False`` to remove any existing non-file when ``force=True``
     + force_backup_dir: directory to move any backup to when ``force=True``
@@ -1184,145 +1102,94 @@
     .. code:: python
 
         files.link(
             name="Create link /etc/issue2 that points to /etc/issue",
             path="/etc/issue2",
             target="/etc/issue",
         )
-
-
-        # Complex example demonstrating the assume_present option
-        from pyinfra.operations import apt, files
-
-        install_nginx = apt.packages(
-            name="Install nginx",
-            packages=["nginx"],
-        )
-
-        files.link(
-            name="Remove default nginx site",
-            path="/etc/nginx/sites-enabled/default",
-            present=False,
-            assume_present=install_nginx.changed,
-        )
     """
 
     path = _validate_path(path)
 
     if present and not target:
         raise OperationError("If present is True target must be provided")
 
     info = host.get_fact(Link, path=path)
 
-    # Not a link?
-    if info is False:
+    if info is False:  # not a link
         yield from _raise_or_remove_invalid_path(
             "link",
             path,
             force,
             force_backup,
             force_backup_dir,
         )
         info = None
 
     add_args = ["ln"]
     if symbolic:
         add_args.append("-s")
 
-    add_cmd = StringCommand(" ".join(add_args), QuoteString(target), QuoteString(path))
     remove_cmd = StringCommand("rm", "-f", QuoteString(path))
 
-    # No link and we want it
-    if not assume_present and info is None and present:
+    if not present:
+        if info:
+            yield remove_cmd
+        else:
+            host.noop("link {link} does not exist")
+        return
+
+    assert target is not None  # appease typing QuoteString below
+    add_cmd = StringCommand(" ".join(add_args), QuoteString(target), QuoteString(path))
+
+    if info is None:  # create
         if create_remote_dir:
-            yield from _create_remote_dir(state, host, path, user, group)
+            yield from _create_remote_dir(path, user, group)
 
         yield add_cmd
 
         if user or group:
             yield file_utils.chown(path, user, group, dereference=False)
 
-        host.create_fact(
-            Link,
-            kwargs={"path": path},
-            data={"link_target": target, "group": group, "user": user},
-        )
-
-    # It exists and we don't want it
-    elif (assume_present or info) and not present:
-        yield remove_cmd
-        host.delete_fact(Link, kwargs={"path": path})
-
-    # Exists and want to ensure it's state
-    elif (assume_present or info) and present:
-        if assume_present and not info:
-            info = {"link_target": None, "group": None, "user": None}
-            host.create_fact(Link, kwargs={"path": path}, data=info)
-
-        # If we have an absolute path - prepend to any non-absolute values from the fact
-        # and/or the source.
-        if os.path.isabs(path):
-            link_dirname = os.path.dirname(path)
-
-            if not os.path.isabs(target):
-                target = os.path.normpath(unix_path_join(link_dirname, target))
-
-            if info and not os.path.isabs(info["link_target"]):
-                info["link_target"] = os.path.normpath(
-                    unix_path_join(link_dirname, info["link_target"]),
-                )
-
+    else:  # edit
         changed = False
 
         # If the target is wrong, remove & recreate the link
         if not info or info["link_target"] != target:
             changed = True
             yield remove_cmd
             yield add_cmd
-            info["link_target"] = target
 
         # Check user/group
-        if (
-            (not info and (user or group))
-            or (user and info["user"] != user)
-            or (group and info["group"] != group)
-        ):
+        if (user and info["user"] != user) or (group and info["group"] != group):
             yield file_utils.chown(path, user, group, dereference=False)
             changed = True
-            if user:
-                info["user"] = user
-            if group:
-                info["group"] = group
 
         if not changed:
             host.noop("link {0} already exists".format(path))
 
 
-@operation(
-    pipeline_facts={"file": "path"},
-)
+@operation()
 def file(
-    path,
+    path: str,
     present=True,
-    assume_present=False,
-    user=None,
-    group=None,
-    mode=None,
+    user: str = None,
+    group: str = None,
+    mode: str = None,
     touch=False,
     create_remote_dir=True,
     force=False,
     force_backup=True,
-    force_backup_dir=None,
+    force_backup_dir: str = None,
 ):
     """
     Add/remove/update files.
 
     + path: name/path of the remote file
     + present: whether the file should exist
-    + assume_present: whether to assume the file exists
     + user: user to own the files
     + group: group to own the files
     + mode: permissions of the files as an integer, eg: 755
     + touch: whether to touch the file
     + create_remote_dir: create the remote directory if it doesn't exist
     + force: if the target exists and is not a file, move or remove it and continue
     + force_backup: set to ``False`` to remove any existing non-file when ``force=True``
@@ -1350,106 +1217,82 @@
     """
 
     path = _validate_path(path)
 
     mode = ensure_mode_int(mode)
     info = host.get_fact(File, path=path)
 
-    # Not a file?!
-    if info is False:
+    if info is False:  # not a file
         yield from _raise_or_remove_invalid_path(
             "file",
             path,
             force,
             force_backup,
             force_backup_dir,
         )
         info = None
 
-    # Doesn't exist & we want it
-    if not assume_present and info is None and present:
+    if not present:
+        if info:
+            yield StringCommand("rm", "-f", QuoteString(path))
+        else:
+            host.noop("file {0} does not exist")
+        return
+
+    if info is None:  # create
         if create_remote_dir:
-            yield from _create_remote_dir(state, host, path, user, group)
+            yield from _create_remote_dir(path, user, group)
 
         yield StringCommand("touch", QuoteString(path))
 
         if mode:
             yield file_utils.chmod(path, mode)
         if user or group:
             yield file_utils.chown(path, user, group)
 
-        host.create_fact(
-            File,
-            kwargs={"path": path},
-            data={"mode": mode, "group": group, "user": user},
-        )
-
-    # It exists and we don't want it
-    elif (assume_present or info) and not present:
-        yield StringCommand("rm", "-f", QuoteString(path))
-        host.delete_fact(File, kwargs={"path": path})
-
-    # It exists & we want to ensure its state
-    elif (assume_present or info) and present:
-        if assume_present and not info:
-            info = {"mode": None, "group": None, "user": None}
-            host.create_fact(File, kwargs={"path": path}, data=info)
-
+    else:  # update
         changed = False
 
         if touch:
             changed = True
             yield StringCommand("touch", QuoteString(path))
 
         # Check mode
         if mode and (not info or info["mode"] != mode):
             yield file_utils.chmod(path, mode)
-            info["mode"] = mode
             changed = True
 
         # Check user/group
-        if (
-            (not info and (user or group))
-            or (user and info["user"] != user)
-            or (group and info["group"] != group)
-        ):
+        if (user and info["user"] != user) or (group and info["group"] != group):
             yield file_utils.chown(path, user, group)
             changed = True
-            if user:
-                info["user"] = user
-            if group:
-                info["group"] = group
 
         if not changed:
             host.noop("file {0} already exists".format(path))
 
 
-@operation(
-    pipeline_facts={"directory": "path"},
-)
+@operation()
 def directory(
-    path,
+    path: str,
     present=True,
-    assume_present=False,
-    user=None,
-    group=None,
-    mode=None,
+    user: str = None,
+    group: str = None,
+    mode: str = None,
     recursive=False,
     force=False,
     force_backup=True,
-    force_backup_dir=None,
+    force_backup_dir: str = None,
     _no_check_owner_mode=False,
     _no_fail_on_link=False,
 ):
     """
     Add/remove/update directories.
 
     + path: path of the remote folder
     + present: whether the folder should exist
-    + assume_present: whether to assume the directory exists
     + user: user to own the folder
     + group: group to own the folder
     + mode: permissions of the folder
     + recursive: recursively apply user/group/mode
     + force: if the target exists and is not a file, move or remove it and continue
     + force_backup: set to ``False`` to remove any existing non-file when ``force=True``
     + force_backup_dir: directory to move any backup to when ``force=True``
@@ -1480,81 +1323,61 @@
     """
 
     path = _validate_path(path)
 
     mode = ensure_mode_int(mode)
     info = host.get_fact(Directory, path=path)
 
-    # Not a directory?!
-    if info is False:
+    if info is False:  # not a directory
         if _no_fail_on_link and host.get_fact(Link, path=path):
             host.noop("directory {0} already exists (as a link)".format(path))
             return
         yield from _raise_or_remove_invalid_path(
             "directory",
             path,
             force,
             force_backup,
             force_backup_dir,
         )
         info = None
 
-    # Doesn't exist & we want it
-    if not assume_present and info is None and present:
+    if not present:
+        if info:
+            yield StringCommand("rm", "-rf", QuoteString(path))
+        else:
+            host.noop("directory {0} does not exist")
+        return
+
+    if info is None:  # create
         yield StringCommand("mkdir", "-p", QuoteString(path))
         if mode:
             yield file_utils.chmod(path, mode, recursive=recursive)
         if user or group:
             yield file_utils.chown(path, user, group, recursive=recursive)
 
-        host.create_fact(
-            Directory,
-            kwargs={"path": path},
-            data={"mode": mode, "group": group, "user": user},
-        )
-
-    # It exists and we don't want it
-    elif (assume_present or info) and not present:
-        yield StringCommand("rm", "-rf", QuoteString(path))
-        host.delete_fact(Directory, kwargs={"path": path})
-
-    # It exists & we want to ensure its state
-    elif (assume_present or info) and present:
-        if assume_present and not info:
-            info = {"mode": None, "group": None, "user": None}
-            host.create_fact(Directory, kwargs={"path": path}, data=info)
-
+    else:  # update
         if _no_check_owner_mode:
             return
 
         changed = False
 
         if mode and (not info or info["mode"] != mode):
             yield file_utils.chmod(path, mode, recursive=recursive)
-            info["mode"] = mode
             changed = True
 
-        if (
-            (not info and (user or group))
-            or (user and info["user"] != user)
-            or (group and info["group"] != group)
-        ):
+        if (user and info["user"] != user) or (group and info["group"] != group):
             yield file_utils.chown(path, user, group, recursive=recursive)
             changed = True
-            if user:
-                info["user"] = user
-            if group:
-                info["group"] = group
 
         if not changed:
             host.noop("directory {0} already exists".format(path))
 
 
-@operation(pipeline_facts={"flags": "path"})
-def flags(path, flags=None, present=True):
+@operation()
+def flags(path: str, flags: list[str] = None, present=True):
     """
     Set/clear file flags.
 
     + path: path of the remote folder
     + flags: a list of the file flags to be set or cleared
     + present: whether the flags should be set or cleared
 
@@ -1587,43 +1410,34 @@
         current_set = set(host.get_fact(Flags, path=path))
         to_change = list(set(flags) - current_set) if present else list(current_set & set(flags))
 
         if len(to_change) > 0:
             prefix = "" if present else "no"
             new_flags = ",".join([prefix + flag for flag in sorted(to_change)])
             yield StringCommand("chflags", new_flags, QuoteString(path))
-            host.create_fact(
-                Flags,
-                kwargs={"path": path},
-                data=list(current_set | set(to_change))
-                if present
-                else list(current_set - set(to_change)),
-            )
         else:
             host.noop(
                 f'\'{path}\' already has \'{",".join(flags)}\' {"set" if present else "clear"}',
             )
 
 
-@operation(
-    pipeline_facts={"file": "path"},
-)
+@operation()
 def block(
-    path,
-    content=None,
+    path: str,
+    content: str = None,
     present=True,
-    line=None,
+    line: str = None,
     backup=False,
     escape_regex_characters=False,
     try_prevent_shell_expansion=False,
     before=False,
     after=False,
-    marker=None,
-    begin=None,
-    end=None,
+    marker: str = None,
+    begin: str = None,
+    end: str = None,
 ):
     """
     Ensure content, surrounded by the appropriate markers, is present (or not) in the file.
 
     + path: target remote file
     + content: what should be present in the file (between markers).
     + present: whether the content should be present in the file
@@ -1704,15 +1518,15 @@
 
     mark_1 = (marker or MARKER_DEFAULT).format(mark=begin or MARKER_BEGIN_DEFAULT)
     mark_2 = (marker or MARKER_DEFAULT).format(mark=end or MARKER_END_DEFAULT)
 
     # standard awk doesn't have an "in-place edit" option so we write to a tempfile and
     # if edits were successful move to dest i.e. we do: <out_prep> ... do some work ... <real_out>
     q_path = QuoteString(path)
-    out_prep = 'OUT="$(TMPDIR=/tmp mktemp -t pyinfra.XXXXXX)" && '
+    out_prep = StringCommand('OUT="$(TMPDIR=/tmp mktemp -t pyinfra.XXXXXX)" && ')
     if backup:
         out_prep = StringCommand(
             "cp",
             q_path,
             QuoteString(f"{path}.{get_timestamp()}"),
             "&&",
             out_prep,
@@ -1732,20 +1546,24 @@
         q_path,
     )
 
     current = host.get_fact(Block, path=path, marker=marker, begin=begin, end=end)
     cmd = None
     if present:
         if not content:
-            raise ValueError("'content' must be supplied when 'present' == True")
+            raise OperationValueError("'content' must be supplied when 'present' == True")
         if line:
             if before == after:
-                raise ValueError("only one of 'before' or 'after' used when 'line` is specified")
+                raise OperationValueError(
+                    "only one of 'before' or 'after' used when 'line` is specified"
+                )
         elif before != after:
-            raise ValueError("'line' must be supplied or 'before' and 'after' must be equal")
+            raise OperationValueError(
+                "'line' must be supplied or 'before' and 'after' must be equal"
+            )
         if isinstance(content, str):
             # convert string to list of lines
             content = content.split("\n")
         if try_prevent_shell_expansion and any("'" in line for line in content):
             logger.warning("content contains single quotes, shell expansion prevention may fail")
 
         the_block = "\n".join([mark_1, *content, mark_2])
@@ -1755,40 +1573,37 @@
             redirect = ">" if (current is None) else ">>"
             stdin = "- " if ((current == []) and before) else ""
             # here = hex(random.randint(0, 2147483647))
             here = "PYINFRAHERE"
             cmd = StringCommand(
                 f"cat {stdin}{redirect}",
                 q_path,
-                f"<<{here}"
-                if not try_prevent_shell_expansion
-                else f"<<'{here}'",
-                f"\n{the_block}\n{here}"
+                f"<<{here}" if not try_prevent_shell_expansion else f"<<'{here}'",
+                f"\n{the_block}\n{here}",
             )
         elif current == []:  # markers not found and have a pattern to match (not start or end)
             regex = adjust_regex(line, escape_regex_characters)
             print_before = "{ print }" if before else ""
             print_after = "{ print }" if after else ""
             prog = (
                 'awk \'BEGIN {x=ARGV[2]; ARGV[2]=""} '
                 f"{print_after} f!=1 && /{regex}/ {{ print x; f=1}} "
                 f"END {{if (f==0) print ARGV[2] }} {print_before}'"
             )
             cmd = StringCommand(
                 out_prep,
-                prog, q_path,
-                f'"{the_block}"'
-                if not try_prevent_shell_expansion
-                else f"'{the_block}'",
+                prog,
+                q_path,
+                f'"{the_block}"' if not try_prevent_shell_expansion else f"'{the_block}'",
                 "> $OUT &&",
-                real_out
+                real_out,
             )
         else:
             if (len(current) != len(content)) or (
-                    not all(lines[0] == lines[1] for lines in zip(content, current))
+                not all(lines[0] == lines[1] for lines in zip(content, current))
             ):  # marked_block found but text is different
                 prog = (
                     'awk \'BEGIN {{f=1; x=ARGV[2]; ARGV[2]=""}}'
                     f"/{mark_1}/ {{print; print x; f=0}} /{mark_2}/ {{print; f=1; next}} f'"
                 )
                 cmd = StringCommand(
                     out_prep,
@@ -1801,26 +1616,17 @@
                     real_out,
                 )
             else:
                 host.noop("content already present")
 
         if cmd:
             yield cmd
-            host.create_fact(
-                Block,
-                kwargs={"path": path, "marker": marker, "begin": begin, "end": end},
-                data=content,
-            )
     else:  # remove the marked_block
         if content:
             logger.warning("'content' ignored when removing a marked_block")
         if current is None:
             host.noop("no remove required: file did not exist")
         elif current == []:
             host.noop("no remove required: markers not found")
         else:
-            cmd = f"awk '/{mark_1}/,/{mark_2}/ {{next}} 1'"
+            cmd = StringCommand(f"awk '/{mark_1}/,/{mark_2}/ {{next}} 1'")
             yield StringCommand(out_prep, cmd, q_path, "> $OUT &&", real_out)
-            host.delete_fact(
-                Block,
-                kwargs={"path": path, "marker": marker, "begin": begin, "end": end},
-            )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/gem.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/gem.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from pyinfra import host
 from pyinfra.api import operation
 from pyinfra.facts.gem import GemPackages
 
 from .util.packaging import ensure_packages
 
 
-@operation
-def packages(packages=None, present=True, latest=False):
+@operation()
+def packages(packages: str | list[str] = None, present=True, latest=False):
     """
     Add/remove/update gem packages.
 
     + packages: list of packages to ensure
     + present: whether the packages should be installed
     + latest: whether to upgrade packages without a specified version
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/git.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/git.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 from pyinfra.facts.files import Directory, File
 from pyinfra.facts.git import GitBranch, GitConfig, GitTrackingBranch
 
 from . import files, ssh
 from .util.files import chown, unix_path_join
 
 
-@operation(
-    pipeline_facts={"git_config": "repo"},
-)
-def config(key, value, multi_value=False, repo=None):
+@operation()
+def config(key: str, value: str, multi_value=False, repo: str = None):
     """
     Manage git config for a repository or globally.
 
     + key: the key of the config to ensure
     + value: the value this key should have
     + multi_value: Add the value rather than set it for settings that can have multiple values
     + repo: specify the git repo path to edit local config (defaults to global)
@@ -50,35 +48,31 @@
     if repo is None:
         base_command = "git config --global"
     else:
         base_command = "cd {0} && git config --local".format(repo)
 
     if not multi_value and existing_config.get(key) != [value]:
         yield '{0} {1} "{2}"'.format(base_command, key, value)
-        existing_config[key] = [value]
 
     elif multi_value and value not in existing_config.get(key, []):
         yield '{0} --add {1} "{2}"'.format(base_command, key, value)
-        existing_config.setdefault(key, []).append(value)
 
     else:
         host.noop("git config {0} is set to {1}".format(key, value))
 
 
-@operation(
-    pipeline_facts={"git_branch": "target"},
-)
+@operation()
 def repo(
-    src,
-    dest,
-    branch=None,
+    src: str,
+    dest: str,
+    branch: str = None,
     pull=True,
     rebase=False,
-    user=None,
-    group=None,
+    user: str = None,
+    group: str = None,
     ssh_keyscan=False,
     update_submodules=False,
     recursive_submodules=False,
 ):
     """
     Clone/pull git repositories.
 
@@ -101,23 +95,23 @@
             name="Clone repo",
             src="https://github.com/Fizzadar/pyinfra.git",
             dest="/usr/local/src/pyinfra",
         )
     """
 
     # Ensure our target directory exists
-    yield from files.directory(dest)
+    yield from files.directory._inner(dest)
 
     # Do we need to scan for the remote host key?
     if ssh_keyscan:
         # Attempt to parse the domain from the git repository
         domain = re.match(r"^[a-zA-Z0-9]+@([0-9a-zA-Z\.\-]+)", src)
 
         if domain:
-            yield from ssh.keyscan(domain.group(1))
+            yield from ssh.keyscan._inner(domain.group(1))
         else:
             raise OperationError(
                 "Could not parse domain (to SSH keyscan) from: {0}".format(src),
             )
 
     # Store git commands for directory prefix
     git_commands = []
@@ -126,29 +120,19 @@
 
     # Cloning new repo?
     if not is_repo:
         if branch:
             git_commands.append("clone {0} --branch {1} .".format(src, branch))
         else:
             git_commands.append("clone {0} .".format(src))
-
-        host.create_fact(GitBranch, kwargs={"repo": dest}, data=branch)
-        host.create_fact(
-            Directory,
-            kwargs={"path": git_dir},
-            data={"user": user, "group": group},
-        )
-
     # Ensuring existing repo
     else:
         if branch and host.get_fact(GitBranch, repo=dest) != branch:
             git_commands.append("fetch")  # fetch to ensure we have the branch locally
             git_commands.append("checkout {0}".format(branch))
-            host.create_fact(GitBranch, kwargs={"repo": dest}, data=branch)
-
         if pull:
             if rebase:
                 git_commands.append("pull --rebase")
             else:
                 git_commands.append("pull")
 
     if update_submodules:
@@ -167,27 +151,27 @@
     # Apply any user or group if we did anything
     if git_commands and (user or group):
         yield chown(dest, user, group, recursive=True)
 
 
 @operation()
 def worktree(
-    worktree,
-    repo=None,
+    worktree: str,
+    repo: str = None,
     detached=False,
-    new_branch=None,
-    commitish=None,
+    new_branch: str = None,
+    commitish: str = None,
     pull=True,
     rebase=False,
-    from_remote_branch=None,
+    from_remote_branch: tuple[str, str] = None,
     present=True,
     assume_repo_exists=False,
     force=False,
-    user=None,
-    group=None,
+    user: str = None,
+    group: str = None,
 ):
     """
     Manage git worktrees.
 
     + worktree: git working tree directory
     + repo: git main repository directory
     + detached: create a working tree with a detached HEAD
@@ -289,15 +273,14 @@
             present=False,
             force=True,
         )
     """
 
     # Doesn't exist & we want it
     if not host.get_fact(Directory, path=worktree) and present:
-
         # be sure that `repo` is a GIT repository
         if not assume_repo_exists and not host.get_fact(
             Directory,
             path=unix_path_join(repo, ".git"),
         ):
             raise OperationError(
                 "The following folder is not a valid GIT repository : {0}".format(repo),
@@ -317,33 +300,25 @@
 
         yield " ".join(command_parts)
 
         # Apply any user or group
         if user or group:
             yield chown(worktree, user, group, recursive=True)
 
-        host.create_fact(Directory, kwargs={"path": worktree}, data={"user": user, "group": group})
-        host.create_fact(GitTrackingBranch, kwargs={"repo": worktree}, data=new_branch)
-
     # It exists and we don't want it
     elif host.get_fact(Directory, path=worktree) and not present:
-
         command = "cd {0} && git worktree remove .".format(worktree)
 
         if force:
             command += " --force"
 
         yield command
 
-        host.delete_fact(Directory, kwargs={"path": worktree})
-        host.create_fact(GitTrackingBranch, kwargs={"repo": worktree})
-
     # It exists and we still want it => pull/rebase it
     elif host.get_fact(Directory, path=worktree) and present:
-
         # pull the worktree only if it's already linked to a tracking branch or
         # if a remote branch is set
         if host.get_fact(GitTrackingBranch, repo=worktree) or from_remote_branch:
             command = "cd {0} && git pull".format(worktree)
 
             if rebase:
                 command += " --rebase"
@@ -355,19 +330,19 @@
                         '("origin", "master")',
                     )
                 command += " {0} {1}".format(*from_remote_branch)
 
             yield command
 
 
-@operation
+@operation()
 def bare_repo(
-    path,
-    user=None,
-    group=None,
+    path: str,
+    user: str = None,
+    group: str = None,
     present=True,
 ):
     """
     Create bare git repositories.
 
     + path: path to the folder
     + present: whether the bare repository should exist
@@ -380,26 +355,20 @@
 
         git.bare_repo(
             name="Create bare repo",
             path="/home/git/test.git",
         )
     """
 
-    yield from files.directory(path, present=present)
+    yield from files.directory._inner(path, present=present)
 
     if present:
         head_filename = unix_path_join(path, "HEAD")
         head_file = host.get_fact(File, path=head_filename)
 
         if not head_file:
             yield "git init --bare {0}".format(path)
             if user or group:
                 yield chown(path, user, group, recursive=True)
         else:
             if (user and head_file["user"] != user) or (group and head_file["group"] != group):
                 yield chown(path, user, group, recursive=True)
-
-        host.create_fact(
-            File,
-            kwargs={"path": head_filename},
-            data={"user": user, "group": group, "mode": None},
-        )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/iptables.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/iptables.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 from pyinfra import host
 from pyinfra.api import operation
 from pyinfra.api.exceptions import OperationError
 from pyinfra.facts.iptables import Ip6tablesChains, Ip6tablesRules, IptablesChains, IptablesRules
 
 
-@operation
+@operation()
 def chain(
-    chain,
+    chain: str,
     present=True,
     table="filter",
-    policy=None,
+    policy: str = None,
     version=4,
 ):
     """
     Add/remove/update iptables chains.
 
     + chain: the name of the chain
     + present: whether the chain should exist
@@ -37,60 +37,57 @@
 
     command = "iptables" if version == 4 else "ip6tables"
     command = "{0} -t {1}".format(command, table)
 
     if not present:
         if chain in chains:
             yield "{0} -X {1}".format(command, chain)
-            chains.pop(chain)
         else:
             host.noop("iptables chain {0} does not exist".format(chain))
         return
 
     if present:
         if chain not in chains:
             yield "{0} -N {1}".format(command, chain)
-            chains[chain] = None  # policy will be set below
         else:
             host.noop("iptables chain {0} exists".format(chain))
 
         if policy:
             if chain not in chains or chains[chain] != policy:
                 yield "{0} -P {1} {2}".format(command, chain, policy)
-                chains[chain] = policy
 
 
-@operation
+@operation()
 def rule(
-    chain,
-    jump,
-    present=True,
-    table="filter",
-    append=True,
-    version=4,
+    chain: str,
+    jump: str,
+    present: bool = True,
+    table: str = "filter",
+    append: bool = True,
+    version: int = 4,
     # Core iptables filter arguments
-    protocol=None,
-    not_protocol=None,
-    source=None,
-    not_source=None,
-    destination=None,
-    not_destination=None,
-    in_interface=None,
-    not_in_interface=None,
-    out_interface=None,
-    not_out_interface=None,
+    protocol: str = None,
+    not_protocol: str = None,
+    source: str = None,
+    not_source: str = None,
+    destination: str = None,
+    not_destination: str = None,
+    in_interface: str = None,
+    not_in_interface: str = None,
+    out_interface: str = None,
+    not_out_interface: str = None,
     # After-rule arguments
-    to_destination=None,
-    to_source=None,
-    to_ports=None,
-    log_prefix=None,
+    to_destination: str = None,
+    to_source: str = None,
+    to_ports: int = None,
+    log_prefix: str = None,
     # Extras and extra shortcuts
-    destination_port=None,
-    source_port=None,
-    extras="",
+    destination_port: int = None,
+    source_port: int = None,
+    extras: str = "",
 ):
     """
     Add/remove iptables rules.
 
     + chain: the chain this rule should live in
     + jump: the target of the rule
     + table: the iptables table this rule should belong to
@@ -262,26 +259,32 @@
 
         if protocol:
             args.extend(("-p", protocol))
 
         if source:
             args.extend(("-s", source))
 
+        if destination:
+            args.extend(("-d", destination))
+
         if in_interface:
             args.extend(("-i", in_interface))
 
         if out_interface:
             args.extend(("-o", out_interface))
 
         if not_protocol:
             args.extend(("!", "-p", not_protocol.lower()))
 
         if not_source:
             args.extend(("!", "-s", not_source))
 
+        if not_destination:
+            args.extend(("!", "-d", not_destination))
+
         if not_in_interface:
             args.extend(("!", "-i", not_in_interface))
 
         if not_out_interface:
             args.extend(("!", "-o", not_out_interface))
 
         if extras:
@@ -300,12 +303,7 @@
             args.extend(("--to-source", to_source))
 
         if to_ports:
             args.extend(("--to-ports", to_ports))
 
         # Build the final iptables command
         yield " ".join(args)
-
-        if action == "-D":
-            rules.remove(definition)
-        else:
-            rules.append(definition)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/launchd.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/openrc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 """
-Manage launchd services.
+Manage OpenRC init services.
 """
 
 from pyinfra import host
 from pyinfra.api import operation
-from pyinfra.facts.launchd import LaunchdStatus
+from pyinfra.facts.openrc import OpenrcEnabled, OpenrcStatus
 
 from .util.service import handle_service_control
 
 
-@operation
+@operation()
 def service(
-    service,
+    service: str,
     running=True,
     restarted=False,
-    command=None,
+    reloaded=False,
+    command: str = None,
+    enabled: bool = None,
+    runlevel="default",
 ):
     """
-    Manage the state of systemd managed services.
+    Manage the state of OpenRC services.
 
     + service: name of the service to manage
     + running: whether the service should be running
     + restarted: whether the service should be restarted
-    + command: custom command to pass like: ``launchctl <command> <service>``
+    + reloaded: whether the service should be reloaded
+    + command: custom command to pass like: ``rc-service <service> <command>``
     + enabled: whether this service should be enabled/disabled on boot
+    + runlevel: runlevel to manage services for
     """
 
-    was_running = host.get_fact(LaunchdStatus).get(service, None)
-
     yield from handle_service_control(
         host,
         service,
-        host.get_fact(LaunchdStatus),
-        "launchctl {1} {0}",
-        # No support for restart/reload/command
+        host.get_fact(OpenrcStatus, runlevel=runlevel),
+        "rc-service {0} {1}",
         running,
-        None,
-        None,
-        None,
+        restarted,
+        reloaded,
+        command,
     )
 
-    # No restart command, so just stop/start
-    if restarted and was_running:
-        yield "launchctl stop {0}".format(service)
-        yield "launchctl start {0}".format(service)
+    if isinstance(enabled, bool):
+        openrc_enabled = host.get_fact(OpenrcEnabled, runlevel=runlevel)
+        is_enabled = openrc_enabled.get(service, False)
+
+        if enabled and not is_enabled:
+            yield "rc-update add {0}".format(service)
+            openrc_enabled[service] = True
+
+        if not enabled and is_enabled:
+            yield "rc-update del {0}".format(service)
+            openrc_enabled[service] = False
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/lxd.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/lxd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 The LXD modules manage LXD containers
 """
+from typing import Any
 
 from pyinfra import host
 from pyinfra.api import operation
 from pyinfra.facts.lxd import LxdContainers
 
 
-def get_container_named(name, containers):
+def get_container_named(name: str, containers: list[dict[str, Any]]) -> dict[str, Any] | None:
     for container in containers:
         if container["name"] == name:
             return container
-    else:
-        return None
+        else:
+            return None
 
 
-@operation
+@operation()
 def container(
-    id,
+    id: str,
     present=True,
     image="ubuntu:16.04",
 ):
     """
     Add/remove LXD containers.
 
     Note: does not check if an existing container is based on the specified
@@ -49,25 +50,17 @@
     if not present:
         if container:
             if container["status"] == "Running":
                 yield "lxc stop {0}".format(id)
 
             # Command to remove the container:
             yield "lxc delete {0}".format(id)
-
-            current_containers.remove(container)
         else:
             host.noop("container {0} does not exist".format(id))
 
     # Container doesn't exist and we want it
     if present:
         if not container:
             # Command to create the container:
             yield "lxc launch {image} {id} < /dev/null".format(id=id, image=image)
-            current_containers.append(
-                {
-                    "name": id,
-                    "image": image,
-                },
-            )
         else:
             host.noop("container {0} exists".format(id))
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/mysql.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,21 @@
     make_execute_mysql_command,
     make_mysql_command,
 )
 
 
 @operation(is_idempotent=False)
 def sql(
-    sql,
-    database=None,
+    sql: str,
+    database: str = None,
     # Details for speaking to MySQL via `mysql` CLI
-    mysql_user=None,
-    mysql_password=None,
-    mysql_host=None,
-    mysql_port=None,
+    mysql_user: str = None,
+    mysql_password: str = None,
+    mysql_host: str = None,
+    mysql_port: int = None,
 ):
     """
     Execute arbitrary SQL against MySQL.
 
     + sql: SQL command(s) to execute
     + database: optional database to open the connection with
     + mysql_*: global module arguments, see above
@@ -48,36 +48,36 @@
         user=mysql_user,
         password=mysql_password,
         host=mysql_host,
         port=mysql_port,
     )
 
 
-@operation
+@operation()
 def user(
-    user,
-    present=True,
-    user_hostname="localhost",
-    password=None,
-    privileges=None,
+    user: str,
+    present: bool = True,
+    user_hostname: str = "localhost",
+    password: str = None,
+    privileges: str | list[str] = None,
     # MySQL REQUIRE SSL/TLS options
-    require=None,  # SSL or X509
-    require_cipher=False,
-    require_issuer=False,
-    require_subject=False,
+    require: str = None,  # SSL or X509
+    require_cipher: str = None,
+    require_issuer: str = None,
+    require_subject: str = None,
     # MySQL WITH resource limit options
-    max_connections=None,
-    max_queries_per_hour=None,
-    max_updates_per_hour=None,
-    max_connections_per_hour=None,
+    max_connections: int = None,
+    max_queries_per_hour: int = None,
+    max_updates_per_hour: int = None,
+    max_connections_per_hour: int = None,
     # Details for speaking to MySQL via `mysql` CLI via `mysql` CLI
-    mysql_user=None,
-    mysql_password=None,
-    mysql_host=None,
-    mysql_port=None,
+    mysql_user: str = None,
+    mysql_password: str = None,
+    mysql_host: str = None,
+    mysql_port: int = None,
 ):
     """
     Add/remove/update MySQL users.
 
     + user: the name of the user
     + present: whether the user should exist or not
     + user_hostname: the hostname of the user
@@ -158,30 +158,18 @@
             yield make_execute_mysql_command(
                 'DROP USER "{0}"@"{1}"'.format(user, user_hostname),
                 user=mysql_user,
                 password=mysql_password,
                 host=mysql_host,
                 port=mysql_port,
             )
-            current_users.pop(user_host)
         else:
             host.noop("mysql user {0}@{1} does not exist".format(user, user_hostname))
         return
 
-    new_or_updated_user_fact = {
-        "ssl_type": "ANY" if require == "SSL" else require,
-        "ssl_cipher": require_cipher,
-        "x509_issuer": require_issuer,
-        "x509_subject": require_subject,
-        "max_user_connections": max_connections,
-        "max_questions": max_queries_per_hour,
-        "max_updates": max_updates_per_hour,
-        "max_connections": max_connections_per_hour,
-    }
-
     if present and not is_present:
         sql_bits = ['CREATE USER "{0}"@"{1}"'.format(user, user_hostname)]
         if password:
             sql_bits.append(MaskString('IDENTIFIED BY "{0}"'.format(password)))
 
         if require == "SSL":
             sql_bits.append("REQUIRE SSL")
@@ -220,16 +208,14 @@
             StringCommand(*sql_bits),
             user=mysql_user,
             password=mysql_password,
             host=mysql_host,
             port=mysql_port,
         )
 
-        current_users[user_host] = new_or_updated_user_fact
-
     if present and is_present:
         current_user = current_users.get(user_host)
 
         alter_bits = []
 
         if require == "SSL":
             if current_user["ssl_type"] != "ANY":
@@ -273,52 +259,51 @@
             yield make_execute_mysql_command(
                 StringCommand(*sql_bits),
                 user=mysql_user,
                 password=mysql_password,
                 host=mysql_host,
                 port=mysql_port,
             )
-            current_user.update(new_or_updated_user_fact)
         else:
             host.noop("mysql user {0}@{1} exists".format(user, user_hostname))
 
     # If we're here either the user exists or we just created them; either way
     # now we can check any privileges are set.
     if privileges:
-        yield from _privileges(
+        yield from _privileges._inner(
             user,
             privileges,
             user_hostname=user_hostname,
             mysql_user=mysql_user,
             mysql_password=mysql_password,
             mysql_host=mysql_host,
             mysql_port=mysql_port,
         )
 
 
-@operation
+@operation()
 def database(
-    database,
+    database: str,
     # Desired database settings
-    present=True,
-    collate=None,
-    charset=None,
-    user=None,
-    user_hostname="localhost",
-    user_privileges="ALL",
+    present: bool = True,
+    collate: str = None,
+    charset: str = None,
+    user: str = None,
+    user_hostname: str = "localhost",
+    user_privileges: str | list[str] = "ALL",
     # Details for speaking to MySQL via `mysql` CLI
-    mysql_user=None,
-    mysql_password=None,
-    mysql_host=None,
-    mysql_port=None,
+    mysql_user: str = None,
+    mysql_password: str = None,
+    mysql_host: str = None,
+    mysql_port: int = None,
 ):
     """
     Add/remove MySQL databases.
 
-    + name: the name of the database
+    + database: the name of the database
     + present: whether the database should exist or not
     + collate: the collate to use when creating the database
     + charset: the charset to use when creating the database
     + user: MySQL user to grant privileges on this database to
     + user_hostname: the hostname of the MySQL user to grant
     + user_privileges: privileges to grant to any specified user
     + mysql_*: global module arguments, see above
@@ -355,15 +340,14 @@
             yield make_execute_mysql_command(
                 "DROP DATABASE `{0}`".format(database),
                 user=mysql_user,
                 password=mysql_password,
                 host=mysql_host,
                 port=mysql_port,
             )
-            current_databases.pop(database)
         else:
             host.noop("mysql database {0} does not exist".format(database))
         return
 
     # We want the database but it doesn't exist
     if present and not is_present:
         sql_bits = ["CREATE DATABASE `{0}`".format(database)]
@@ -377,49 +361,45 @@
         yield make_execute_mysql_command(
             " ".join(sql_bits),
             user=mysql_user,
             password=mysql_password,
             host=mysql_host,
             port=mysql_port,
         )
-        current_databases[database] = {
-            "collate": collate,
-            "charset": charset,
-        }
     else:
         host.noop("mysql database {0} exists".format(database))
 
     # Ensure any user privileges for this database
     if user and user_privileges:
-        yield from privileges(
+        yield from privileges._inner(
             user,
             user_hostname=user_hostname,
             privileges=user_privileges,
             database=database,
             mysql_user=mysql_user,
             mysql_password=mysql_password,
             mysql_host=mysql_host,
             mysql_port=mysql_port,
         )
 
 
-@operation
+@operation()
 def privileges(
-    user,
-    privileges,
+    user: str,
+    privileges: str | list[str],
     user_hostname="localhost",
     database="*",
     table="*",
     flush=True,
     with_grant_option=False,
     # Details for speaking to MySQL via `mysql` CLI
-    mysql_user=None,
-    mysql_password=None,
-    mysql_host=None,
-    mysql_port=None,
+    mysql_user: str = None,
+    mysql_password: str = None,
+    mysql_host: str = None,
+    mysql_port: int = None,
 ):
     """
     Add/remove MySQL privileges for a user, either global, database or table specific.
 
     + user: name of the user to manage privileges for
     + privileges: list of privileges the user should have (see also: ``with_grant_option`` argument)
     + user_hostname: the hostname of the user
@@ -500,17 +480,14 @@
         )
 
     # Find / revoke any privileges that exist that do not match the desired state
     privileges_to_revoke = existing_privileges.difference(privileges)
     # Find / grant any privileges that we want but do not exist
     privileges_to_grant = privileges - existing_privileges
 
-    user_grants[database_table] -= privileges_to_revoke
-    user_grants[database_table].update(privileges_to_grant)
-
     if privileges_to_grant:
         # We will grant something on this table, no need to revoke "USAGE" as it will be overridden
         privileges_to_revoke.discard("USAGE")
 
     if privileges_to_revoke:
         if {"ALL", "GRANT OPTION"} == privileges_to_revoke:
             # This specific case is identified as the alternative syntax for revoke (without ON).
@@ -543,21 +520,21 @@
 
 
 _privileges = privileges  # noqa: E305 (for use where kwarg is the same)
 
 
 @operation(is_idempotent=False)
 def dump(
-    dest,
-    database=None,
+    dest: str,
+    database: str = None,
     # Details for speaking to MySQL via `mysql` CLI
-    mysql_user=None,
-    mysql_password=None,
-    mysql_host=None,
-    mysql_port=None,
+    mysql_user: str = None,
+    mysql_password: str = None,
+    mysql_host: str = None,
+    mysql_port: int = None,
 ):
     """
     Dump a MySQL database into a ``.sql`` file. Requires ``mysqldump``.
 
     + dest: name of the file to dump the SQL to
     + database: name of the database to dump
     + mysql_*: global module arguments, see above
@@ -584,21 +561,21 @@
         ),
         dest,
     )
 
 
 @operation(is_idempotent=False)
 def load(
-    src,
-    database=None,
+    src: str,
+    database: str = None,
     # Details for speaking to MySQL via `mysql` CLI
-    mysql_user=None,
-    mysql_password=None,
-    mysql_host=None,
-    mysql_port=None,
+    mysql_user: str = None,
+    mysql_password: str = None,
+    mysql_host: str = None,
+    mysql_port: int = None,
 ):
     """
     Load ``.sql`` file into a database.
 
     + src: the filename to read from
     + database: name of the database to import into
     + mysql_*: global module arguments, see above
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/npm.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/npm.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from pyinfra import host
 from pyinfra.api import operation
 from pyinfra.facts.npm import NpmPackages
 
 from .util.packaging import ensure_packages
 
 
-@operation
-def packages(packages=None, present=True, latest=False, directory=None):
+@operation()
+def packages(packages: str | list[str] = None, present=True, latest=False, directory: str = None):
     """
     Install/remove/update npm packages.
 
     + packages: list of packages to ensure
     + present: whether the packages should be present
     + latest: whether to upgrade packages without a specified version
     + directory: directory to manage packages for, defaults to global
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/openrc.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/upstart.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,66 @@
 """
-Manage OpenRC init services.
+Manage upstart services.
 """
 
+from io import StringIO
+
 from pyinfra import host
 from pyinfra.api import operation
-from pyinfra.facts.openrc import OpenrcEnabled, OpenrcStatus
+from pyinfra.facts.upstart import UpstartStatus
 
+from . import files
 from .util.service import handle_service_control
 
 
-@operation
+@operation()
 def service(
-    service,
+    service: str,
     running=True,
     restarted=False,
     reloaded=False,
-    command=None,
-    enabled=None,
-    runlevel="default",
+    command: str = None,
+    enabled: bool = None,
 ):
     """
-    Manage the state of OpenRC services.
+    Manage the state of upstart managed services.
 
     + service: name of the service to manage
     + running: whether the service should be running
     + restarted: whether the service should be restarted
     + reloaded: whether the service should be reloaded
-    + command: custom command to pass like: ``rc-service <service> <command>``
+    + command: custom command to pass like: ``/etc/rc.d/<service> <command>``
     + enabled: whether this service should be enabled/disabled on boot
-    + runlevel: runlevel to manage services for
+
+    Enabling/disabling services:
+        Upstart jobs define runlevels in their config files - as such there is no way to
+        edit/list these without fiddling with the config. So pyinfra simply manages the
+        existence of a ``/etc/init/<service>.override`` file, and sets its content to
+        "manual" to disable automatic start of services.
     """
 
     yield from handle_service_control(
         host,
         service,
-        host.get_fact(OpenrcStatus, runlevel=runlevel),
-        "rc-service {0} {1}",
+        host.get_fact(UpstartStatus),
+        "initctl {1} {0}",
         running,
         restarted,
         reloaded,
         command,
     )
 
-    if isinstance(enabled, bool):
-        openrc_enabled = host.get_fact(OpenrcEnabled, runlevel=runlevel)
-        is_enabled = openrc_enabled.get(service, False)
-
-        if enabled and not is_enabled:
-            yield "rc-update add {0}".format(service)
-            openrc_enabled[service] = True
-
-        if not enabled and is_enabled:
-            yield "rc-update del {0}".format(service)
-            openrc_enabled[service] = False
+    # Upstart jobs are setup w/runlevels etc in their config files, so here we just check
+    # there's no override file.
+    if enabled is True:
+        yield from files.file._inner(
+            path="/etc/init/{0}.override".format(service),
+            present=False,
+        )
+
+    # Set the override file to "manual" to disable automatic start
+    elif enabled is False:
+        file = StringIO("manual\n")
+        yield from files.put._inner(
+            src=file,
+            dest="/etc/init/{0}.override".format(service),
+        )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/pacman.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/pacman.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,32 +14,32 @@
     """
     Upgrades all pacman packages.
     """
 
     yield "pacman --noconfirm -Su"
 
 
-_upgrade = upgrade  # noqa: E305
+_upgrade = upgrade._inner  # noqa: E305
 
 
 @operation(is_idempotent=False)
 def update():
     """
     Updates pacman repositories.
     """
 
     yield "pacman -Sy"
 
 
-_update = update  # noqa: E305
+_update = update._inner  # noqa: E305
 
 
-@operation
+@operation()
 def packages(
-    packages=None,
+    packages: str | list[str] = None,
     present=True,
     update=False,
     upgrade=False,
 ):
     """
     Add/remove pacman packages.
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/pip.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/pip.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from pyinfra.facts.files import File
 from pyinfra.facts.pip import PipPackages
 
 from . import files
 from .util.packaging import ensure_packages
 
 
-@operation
+@operation()
 def virtualenv(
-    path,
-    python=None,
+    path: str,
+    python: str = None,
     venv=False,
     site_packages=False,
     always_copy=False,
     present=True,
 ):
     """
     Add/remove Python virtualenvs.
@@ -42,15 +42,15 @@
 
     # Check for *contents* of a virtualenv, ie don't accept an empty directory
     # as a valid virtualenv but ensure the activate script exists.
     activate_script_path = "{0}/bin/activate".format(path)
 
     if present is False:
         if host.get_fact(File, path=activate_script_path):
-            yield from files.directory(path, present=False)
+            yield from files.directory._inner(path, present=False)
         else:
             host.noop("virtualenv {0} does not exist".format(path))
 
     if present:
         if not host.get_fact(File, path=activate_script_path):
             # Create missing virtualenv
             command = ["virtualenv"]
@@ -68,31 +68,25 @@
                 command.append("--always-copy")
             elif always_copy and venv:
                 command.append("--copies")
 
             command.append(path)
 
             yield " ".join(command)
-
-            host.create_fact(
-                File,
-                kwargs={"path": activate_script_path},
-                data={"user": None, "group": None},
-            )
         else:
             host.noop("virtualenv {0} exists".format(path))
 
 
-_virtualenv = virtualenv  # noqa
+_virtualenv = virtualenv._inner  # noqa
 
 
-@operation
+@operation()
 def venv(
-    path,
-    python=None,
+    path: str,
+    python: str = None,
     site_packages=False,
     always_copy=False,
     present=True,
 ):
     """
     Add/remove Python virtualenvs.
 
@@ -107,34 +101,34 @@
 
         pip.venv(
             name="Create a virtualenv",
             path="/usr/local/bin/venv",
         )
     """
 
-    yield from virtualenv(
+    yield from _virtualenv(
         venv=True,
         path=path,
         python=python,
         site_packages=site_packages,
         always_copy=always_copy,
         present=present,
     )
 
 
-@operation
+@operation()
 def packages(
-    packages=None,
+    packages: str | list[str] = None,
     present=True,
     latest=False,
-    requirements=None,
+    requirements: str = None,
     pip="pip",
-    virtualenv=None,
-    virtualenv_kwargs=None,
-    extra_install_args=None,
+    virtualenv: str = None,
+    virtualenv_kwargs: dict = None,
+    extra_install_args: str = None,
 ):
     """
     Install/remove/update pip packages.
 
     + packages: list of packages to ensure
     + present: whether the packages should be installed
     + latest: whether to upgrade packages without a specified version
@@ -169,32 +163,37 @@
     if virtualenv:
         yield from _virtualenv(virtualenv, **virtualenv_kwargs)
 
         # And update pip path
         virtualenv = virtualenv.rstrip("/")
         pip = "{0}/bin/{1}".format(virtualenv, pip)
 
-    install_command = [pip, "install"]
+    install_command_args = [pip, "install"]
     if extra_install_args:
-        install_command.append(extra_install_args)
-    install_command = " ".join(install_command)
+        install_command_args.append(extra_install_args)
+    install_command = " ".join(install_command_args)
 
     uninstall_command = " ".join([pip, "uninstall", "--yes"])
 
     # (un)Install requirements
     if requirements is not None:
         if present:
             yield "{0} -r {1}".format(install_command, requirements)
         else:
             yield "{0} -r {1}".format(uninstall_command, requirements)
 
     # Handle passed in packages
     if packages:
         current_packages = host.get_fact(PipPackages, pip=pip)
 
+        # PEP-0426 states that Python packages should be compared using lowercase, so lowercase both
+        # the input packages and the fact packages before comparison.
+        packages = [pkg.lower() for pkg in packages]
+        current_packages = {pkg.lower(): versions for pkg, versions in current_packages.items()}
+
         yield from ensure_packages(
             host,
             packages,
             current_packages,
             present,
             install_command=install_command,
             uninstall_command=uninstall_command,
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/pkg.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/pkg.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from pyinfra.facts.files import File
 from pyinfra.facts.pkg import PkgPackages
 from pyinfra.facts.server import Arch, Os, OsVersion, Which
 
 from .util.packaging import ensure_packages
 
 
-@operation
-def packages(packages=None, present=True, pkg_path=None):
+@operation()
+def packages(packages: str | list[str] = None, present=True, pkg_path: str = None):
     """
     Install/remove/update pkg packages. This will use ``pkg ...`` where available
     (FreeBSD) and the ``pkg_*`` variants elsewhere.
 
     + packages: list of packages to ensure
     + present: whether the packages should be installed
     + pkg_path: the PKG_PATH environment variable to set
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/pkgin.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/pkgin.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,32 +14,32 @@
     """
     Upgrades all pkgin packages.
     """
 
     yield "pkgin -y upgrade"
 
 
-_upgrade = upgrade  # noqa: E305
+_upgrade = upgrade._inner  # noqa: E305
 
 
 @operation(is_idempotent=False)
 def update():
     """
     Updates pkgin repositories.
     """
 
     yield "pkgin -y update"
 
 
-_update = update  # noqa: E305
+_update = update._inner  # noqa: E305
 
 
-@operation
+@operation()
 def packages(
-    packages=None,
+    packages: str | list[str] = None,
     present=True,
     latest=False,
     update=False,
     upgrade=False,
 ):
     """
     Add/remove/update pkgin packages.
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/postgresql.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/postgres.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,58 +9,33 @@
     + ``psql_host``: the hostname of the server to connect to
     + ``psql_port``: the port of the server to connect to
 
 See example/postgresql.py for detailed example
 
 """
 
-from pyinfra import host, logger
+from pyinfra import host
 from pyinfra.api import MaskString, StringCommand, operation
-from pyinfra.facts.postgresql import (
-    PostgresqlDatabases,
-    PostgresqlRoles,
+from pyinfra.facts.postgres import (
+    PostgresDatabases,
+    PostgresRoles,
     make_execute_psql_command,
     make_psql_command,
 )
 
-LEGACY_ARG_MAP = {
-    "postgresql_user": "psql_user",
-    "postgresql_password": "psql_password",
-    "postgresql_host": "psql_host",
-    "postgresql_port": "psql_port",
-}
-
-
-def _translate_legacy_args(func):
-    def decorated_func(*args, **kwargs):
-        for legacy_key, key in LEGACY_ARG_MAP.items():
-            if legacy_key in kwargs:
-                kwargs[key] = kwargs.pop(legacy_key)
-                logger.warning(
-                    (
-                        f"The `{legacy_key}` has been replaced "
-                        f"by `{key}` in `postgresql.*` operations."
-                    ),
-                )
-        return func(*args, **kwargs)
-
-    decorated_func._pyinfra_op = func
-    return decorated_func
-
 
 @operation(is_idempotent=False)
-@_translate_legacy_args
 def sql(
-    sql,
-    database=None,
+    sql: str,
+    database: str = None,
     # Details for speaking to PostgreSQL via `psql` CLI
-    psql_user=None,
-    psql_password=None,
-    psql_host=None,
-    psql_port=None,
+    psql_user: str = None,
+    psql_password: str = None,
+    psql_host: str = None,
+    psql_port: int = None,
 ):
     """
     Execute arbitrary SQL against PostgreSQL.
 
     + sql: SQL command(s) to execute
     + database: optional database to execute against
     + psql_*: global module arguments, see above
@@ -72,32 +47,31 @@
         user=psql_user,
         password=psql_password,
         host=psql_host,
         port=psql_port,
     )
 
 
-@operation
-@_translate_legacy_args
+@operation()
 def role(
-    role,
+    role: str,
     present=True,
-    password=None,
+    password: str = None,
     login=True,
     superuser=False,
     inherit=False,
     createdb=False,
     createrole=False,
     replication=False,
-    connection_limit=None,
+    connection_limit: int = None,
     # Details for speaking to PostgreSQL via `psql` CLI
-    psql_user=None,
-    psql_password=None,
-    psql_host=None,
-    psql_port=None,
+    psql_user: str = None,
+    psql_password: str = None,
+    psql_host: str = None,
+    psql_port: int = None,
 ):
     """
     Add/remove PostgreSQL roles.
 
     + role: name of the role
     + present: whether the role should be present or absent
     + password: the password for the role
@@ -127,15 +101,15 @@
             login=True,
             sudo_user="postgres",
         )
 
     """
 
     roles = host.get_fact(
-        PostgresqlRoles,
+        PostgresRoles,
         psql_user=psql_user,
         psql_password=psql_password,
         psql_host=psql_host,
         psql_port=psql_port,
     )
 
     is_present = role in roles
@@ -146,15 +120,14 @@
             yield make_execute_psql_command(
                 'DROP ROLE "{0}"'.format(role),
                 user=psql_user,
                 password=psql_password,
                 host=psql_host,
                 port=psql_port,
             )
-            roles.pop(role)
         else:
             host.noop("postgresql role {0} does not exist".format(role))
         return
 
     # If we want the user and they don't exist
     if not is_present:
         sql_bits = ['CREATE ROLE "{0}"'.format(role)]
@@ -179,40 +152,34 @@
         yield make_execute_psql_command(
             StringCommand(*sql_bits),
             user=psql_user,
             password=psql_password,
             host=psql_host,
             port=psql_port,
         )
-        roles[role] = {
-            "super": superuser,
-            "createdb": createdb,
-            "createrole": createrole,
-        }
     else:
         host.noop("postgresql role {0} exists".format(role))
 
 
-@operation
-@_translate_legacy_args
+@operation()
 def database(
-    database,
+    database: str,
     present=True,
-    owner=None,
-    template=None,
-    encoding=None,
-    lc_collate=None,
-    lc_ctype=None,
-    tablespace=None,
-    connection_limit=None,
+    owner: str = None,
+    template: str = None,
+    encoding: str = None,
+    lc_collate: str = None,
+    lc_ctype: str = None,
+    tablespace: str = None,
+    connection_limit: int = None,
     # Details for speaking to PostgreSQL via `psql` CLI
-    psql_user=None,
-    psql_password=None,
-    psql_host=None,
-    psql_port=None,
+    psql_user: str = None,
+    psql_password: str = None,
+    psql_host: str = None,
+    psql_port: int = None,
 ):
     """
     Add/remove PostgreSQL databases.
 
     + name: name of the database
     + present: whether the database should exist or not
     + owner: the PostgreSQL role that owns the database
@@ -240,15 +207,15 @@
             encoding="UTF8",
             sudo_user="postgres",
         )
 
     """
 
     current_databases = host.get_fact(
-        PostgresqlDatabases,
+        PostgresDatabases,
         psql_user=psql_user,
         psql_password=psql_password,
         psql_host=psql_host,
         psql_port=psql_port,
     )
 
     is_present = database in current_databases
@@ -258,15 +225,14 @@
             yield make_execute_psql_command(
                 'DROP DATABASE "{0}"'.format(database),
                 user=psql_user,
                 password=psql_password,
                 host=psql_host,
                 port=psql_port,
             )
-            current_databases.pop(database)
         else:
             host.noop("postgresql database {0} does not exist".format(database))
         return
 
     # We want the database but it doesn't exist
     if present and not is_present:
         sql_bits = ['CREATE DATABASE "{0}"'.format(database)]
@@ -286,36 +252,27 @@
         yield make_execute_psql_command(
             StringCommand(*sql_bits),
             user=psql_user,
             password=psql_password,
             host=psql_host,
             port=psql_port,
         )
-        current_databases[database] = {
-            "template": template,
-            "encoding": encoding,
-            "lc_collate": lc_collate,
-            "lc_ctype": lc_ctype,
-            "tablespace": tablespace,
-            "connection_limit": connection_limit,
-        }
     else:
         host.noop("postgresql database {0} exists".format(database))
 
 
 @operation(is_idempotent=False)
-@_translate_legacy_args
 def dump(
-    dest,
-    database=None,
+    dest: str,
+    database: str = None,
     # Details for speaking to PostgreSQL via `psql` CLI
-    psql_user=None,
-    psql_password=None,
-    psql_host=None,
-    psql_port=None,
+    psql_user: str = None,
+    psql_password: str = None,
+    psql_host: str = None,
+    psql_port: int = None,
 ):
     """
     Dump a PostgreSQL database into a ``.sql`` file. Requires ``pg_dump``.
 
     + dest: name of the file to dump the SQL to
     + database: name of the database to dump
     + psql_*: global module arguments, see above
@@ -344,23 +301,22 @@
         ),
         ">",
         dest,
     )
 
 
 @operation(is_idempotent=False)
-@_translate_legacy_args
 def load(
-    src,
-    database=None,
+    src: str,
+    database: str = None,
     # Details for speaking to PostgreSQL via `psql` CLI
-    psql_user=None,
-    psql_password=None,
-    psql_host=None,
-    psql_port=None,
+    psql_user: str = None,
+    psql_password: str = None,
+    psql_host: str = None,
+    psql_port: int = None,
 ):
     """
     Load ``.sql`` file into a database.
 
     + src: the filename to read from
     + database: name of the database to import into
     + psql_*: global module arguments, see above
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/puppet.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/puppet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pyinfra.api import operation
 
 
 @operation(is_idempotent=False)
-def agent(server=None, port=None):
+def agent(server: str = None, port: int = None):
     """
     Run puppet agent
 
     + server: master server URL
     + port: puppet master port
 
     Note: Either 'USE_SUDO_LOGIN=True' or 'USE_SU_LOGIN=True'
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/python.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/python.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """
 The Python module allows you to execute Python code within the context of a deploy.
 """
 
-from inspect import getfullargspec
+from typing import Callable
 
-from pyinfra import logger
 from pyinfra.api import FunctionCommand, operation
-from pyinfra.api.util import get_call_location
 
 
-@operation(is_idempotent=False)
-def call(function, *args, **kwargs):
+@operation(is_idempotent=False, _set_in_op=False)
+def call(function: Callable, *args, **kwargs):
     """
     Execute a Python function within a deploy.
 
     + function: the function to execute
     + args: arguments to pass to the function
     + kwargs: keyword arguments to pass to the function
 
@@ -39,28 +37,19 @@
             name="Run my_callback function",
             function=my_callback,
             hello="world",
         )
 
     """
 
-    argspec = getfullargspec(function)
-    if "state" in argspec.args and "host" in argspec.args:
-        logger.warning(
-            "Callback functions used in `python.call` operations no "
-            f"longer take `state` and `host` arguments: {get_call_location(frame_offset=3)}",
-        )
-
-    kwargs.pop("state", None)
-    kwargs.pop("host", None)
     yield FunctionCommand(function, args, kwargs)
 
 
-@operation(is_idempotent=False)
-def raise_exception(exception, *args, **kwargs):
+@operation(is_idempotent=False, _set_in_op=False)
+def raise_exception(exception: Exception, *args, **kwargs):
     """
     Raise a Python exception within a deploy.
 
     + exception: the exception class to raise
     + args: arguments passed to the exception creation
     + kwargs: keyword arguments passed to the exception creation
 
@@ -74,10 +63,8 @@
             message="This is not implemented",
         )
     """
 
     def raise_exc(*args, **kwargs):  # pragma: no cover
         raise exception(*args, **kwargs)
 
-    kwargs.pop("state", None)
-    kwargs.pop("host", None)
     yield FunctionCommand(raise_exc, args, kwargs)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/selinux.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/selinux.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 """
 Provides operations to set SELinux file contexts, booleans and port types.
 """
+from enum import Enum
+
 from pyinfra import host
-from pyinfra.api import QuoteString, StringCommand, operation
+from pyinfra.api import OperationValueError, QuoteString, StringCommand, operation
 from pyinfra.facts.selinux import FileContext, FileContextMapping, SEBoolean, SEPort, SEPorts
 from pyinfra.facts.server import Which
 
 
-@operation(
-    pipeline_facts={"seboolean": "bool_name"},
-)
-def boolean(bool_name, value, persistent=False):
+class Boolean(Enum):
+    ON = "on"
+    OFF = "off"
+
+
+class Protocol(Enum):
+    UDP = "udp"
+    TCP = "tcp"
+    SCTP = "sctp"
+    DCCP = "dccp"
+
+
+@operation()
+def boolean(bool_name: str, value: Boolean, persistent=False):
     """
     Set the specified SELinux boolean to the desired state.
 
     + boolean: name of an SELinux boolean
-    + state: 'on' or 'off'
+    + value: desired state of the boolean
     + persistent: whether to write updated policy or not
 
     Note: This operation requires root privileges.
 
     **Example:**
 
     .. code:: python
 
         selinux.boolean(
             name='Allow Apache to connect to LDAP server',
             'httpd_can_network_connect',
-            'on',
+            Boolean.ON,
             persistent=True
         )
     """
-    _valid_states = ["on", "off"]
 
-    if value not in _valid_states:
-        raise ValueError(
-            f'\'value\' must be one of \'{",".join(_valid_states)}\' but found \'{value}\'',
-        )
+    if value in ["on", "off"]:  # compatibility with the old version
+        pass
+    elif value is Boolean.ON:
+        value = "on"
+    elif value is Boolean.OFF:
+        value = "off"
+    else:
+        raise OperationValueError(f"Invalid value '{value}' for boolean operation")
 
     if host.get_fact(SEBoolean, boolean=bool_name) != value:
         persist = "-P " if persistent else ""
         yield StringCommand("setsebool", f"{persist}{bool_name}", value)
-        host.create_fact(SEBoolean, kwargs={"boolean": bool_name}, data=value)
     else:
         host.noop(f"boolean '{bool_name}' already had the value '{value}'")
 
 
-@operation(
-    pipeline_facts={"filecontext": "path"},
-)
-def file_context(path, se_type):
+@operation()
+def file_context(path: str, se_type: str):
     """
     Set the SELinux type for the specified path to the specified value.
 
     + path: the target path (expression) for the context
     + se_type: the SELinux type for the given target
 
     **Example:**
@@ -66,27 +78,20 @@
             'httpd_sys_content_t'
         )
     """
 
     current = host.get_fact(FileContext, path=path) or {}
     if se_type != current.get("type", ""):
         yield StringCommand("chcon", "-t", se_type, QuoteString(path))
-        host.create_fact(
-            FileContext,
-            kwargs={"path": path},
-            data=dict(current, **{"type": se_type}),
-        )
     else:
         host.noop(f"file_context: '{path}' already had type '{se_type}'")
 
 
-@operation(
-    pipeline_facts={"filecontextmapping": "target"},
-)
-def file_context_mapping(target, se_type=None, present=True):
+@operation()
+def file_context_mapping(target: str, se_type: str = None, present=True):
     """
     Set the SELinux file context mapping for paths matching the target.
 
     + target: the target path (expression) for the context
     + se_type: the SELinux type for the given target
     + present: whether to add or remove the target -> context mapping
 
@@ -104,38 +109,29 @@
             se_type='httpd_sys_content_t'
         )
     """
     if present and (se_type is None):
         raise ValueError("se_type must have a valid value if present is set")
 
     current = host.get_fact(FileContextMapping, target=target)
-    kwargs = {"target": target}
     if present:
         option = "-a" if len(current) == 0 else ("-m" if current.get("type") != se_type else "")
         if option != "":
             yield StringCommand("semanage", "fcontext", option, "-t", se_type, QuoteString(target))
-            host.create_fact(
-                FileContextMapping,
-                kwargs=kwargs,
-                data=dict(current, **{"type": se_type}),
-            )
         else:
             host.noop(f"mapping for '{target}' -> '{se_type}' already present")
     else:
         if len(current) > 0:
             yield StringCommand("semanage", "fcontext", "-d", QuoteString(target))
-            host.create_fact(FileContextMapping, kwargs=kwargs, data={})
         else:
             host.noop(f"no existing mapping for '{target}'")
 
 
-@operation(
-    pipeline_facts={"which": "sepolicy"},
-)
-def port(protocol, port_num, se_type=None, present=True):
+@operation()
+def port(protocol: Protocol, port_num: int, se_type: str = None, present=True):
     """
     Set the SELinux type for the specified protocol and port.
 
     + protocol: the protocol: (udp|tcp|sctp|dccp)
     + port: the port
     + se_type: the SELinux type for the given port
     + present: whether to add or remove the SELinux type for the port
@@ -144,20 +140,23 @@
 
     **Example:**
 
     .. code:: python
 
         selinux.port(
             name='Allow Apache to provide service on port 2222',
-            'tcp',
+            Protocol.TCP,
             2222,
             'http_port_t',
         )
     """
 
+    if protocol is Protocol:
+        protocol = protocol.value
+
     if present and (se_type is None):
         raise ValueError("se_type must have a valid value if present is set")
 
     new_type = se_type if present else ""
     direct_get = len(host.get_fact(Which, command=SEPort.requires_command) or "") > 0
     if direct_get:
         current = host.get_fact(SEPort, protocol=protocol, port=port_num)
@@ -174,13 +173,11 @@
     else:
         if current != "":
             yield StringCommand("semanage", "port", "-d", "-p", protocol, port_num)
         else:
             host.noop(f"setype for '{protocol}/{port_num}' is already unset")
 
     if (present and (option != "")) or (not present and (current != "")):
-        if direct_get:
-            host.create_fact(SEPort, kwargs={"protocol": protocol, "port": port_num}, data=new_type)
-        else:
+        if not direct_get:
             if protocol not in port_info:
                 port_info[protocol] = {}
             port_info[protocol][str(port_num)] = new_type
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/server.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 import shlex
 from io import StringIO
 from itertools import filterfalse, tee
 from os import path
 from time import sleep
+from typing import TYPE_CHECKING
 
 from pyinfra import host, logger, state
 from pyinfra.api import FunctionCommand, OperationError, StringCommand, operation
 from pyinfra.api.util import try_int
 from pyinfra.connectors.util import remove_any_sudo_askpass_file
 from pyinfra.facts.files import Directory, FindInFile, Link
 from pyinfra.facts.server import (
@@ -42,14 +43,17 @@
     upstart,
     xbps,
     yum,
     zypper,
 )
 from .util.files import chmod, sed_replace
 
+if TYPE_CHECKING:
+    from pyinfra.api.arguments_typed import PyinfraOperation
+
 
 @operation(is_idempotent=False)
 def reboot(delay=10, interval=1, reboot_timeout=300):
     """
     Reboot the server and wait for reconnection.
 
     + delay: number of seconds to wait before attempting reconnect
@@ -71,15 +75,15 @@
     # not) we'll error if we don't clean this up now. Will simply be re-uploaded if
     # needed later.
     def remove_any_askpass_file(state, host):
         remove_any_sudo_askpass_file(host)
 
     yield FunctionCommand(remove_any_askpass_file, (), {})
 
-    yield StringCommand("reboot", success_exit_codes=[0, -1])  # -1 being error/disconnected
+    yield StringCommand("reboot", _success_exit_codes=[0, -1])  # -1 being error/disconnected
 
     def wait_and_reconnect(state, host):  # pragma: no cover
         sleep(delay)
         max_retries = round(reboot_timeout / interval)
 
         host.connection = None  # remove the connection object
         retries = 0
@@ -131,15 +135,15 @@
         done
     """.format(
         port,
     )
 
 
 @operation(is_idempotent=False)
-def shell(commands):
+def shell(commands: str | list[str]):
     """
     Run raw shell code on server during a deploy. If the command would
     modify data that would be in a fact, the fact would not be updated
     since facts are only run at the start of a deploy.
 
     + commands: command or list of commands to execute on the remote server
 
@@ -158,15 +162,15 @@
         commands = [commands]
 
     for command in commands:
         yield command
 
 
 @operation(is_idempotent=False)
-def script(src, args=()):
+def script(src: str, args=()):
     """
     Upload and execute a local script on the remote host.
 
     + src: local script filename to upload & execute
     + args: iterable to pass as arguments to the script
 
     **Example:**
@@ -183,23 +187,23 @@
         server.script(
             name="Hello",
             src="files/hello.bash",
             args=("do-something", "with-this"),
         )
     """
 
-    temp_file = state.get_temp_filename()
-    yield from files.put(src, temp_file)
+    temp_file = host.get_temp_filename()
+    yield from files.put._inner(src=src, dest=temp_file)
 
     yield chmod(temp_file, "+x")
     yield StringCommand(temp_file, *args)
 
 
 @operation(is_idempotent=False)
-def script_template(src, args=(), **data):
+def script_template(src: str, args=(), **data):
     """
     Generate, upload and execute a local script template on the remote host.
 
     + src: local script template filename
 
     **Example:**
 
@@ -213,23 +217,23 @@
         server.script_template(
             name="Hello from script",
             src="templates/hello2.bash.j2",
             some_var=some_var,
         )
     """
 
-    temp_file = state.get_temp_filename("{0}{1}".format(src, data))
-    yield from files.template(src, temp_file, **data)
+    temp_file = host.get_temp_filename("{0}{1}".format(src, data))
+    yield from files.template._inner(src, temp_file, **data)
 
     yield chmod(temp_file, "+x")
     yield StringCommand(temp_file, *args)
 
 
-@operation
-def modprobe(module, present=True, force=False):
+@operation()
+def modprobe(module: str, present=True, force=False):
     """
     Load/unload kernel modules.
 
     + module: name of the module to manage
     + present: whether the module should be loaded or not
     + force: whether to force any add/remove modules
 
@@ -255,41 +259,37 @@
     args = ""
     if force:
         args = " -f"
 
     # Module is loaded and we don't want it?
     if not present and present_mods:
         yield "modprobe{0} -r -a {1}".format(args, " ".join(present_mods))
-        for mod in present_mods:
-            modules.pop(mod)
 
     # Module isn't loaded and we want it?
     elif present and missing_mods:
         yield "modprobe{0} -a {1}".format(args, " ".join(missing_mods))
-        for mod in missing_mods:
-            modules[mod] = {}
 
     else:
         host.noop(
             "{0} {1} {2} {3}".format(
                 "modules" if len(list_value) > 1 else "module",
                 "/".join(list_value),
                 "are" if len(list_value) > 1 else "is",
                 "loaded" if present else "not loaded",
             ),
         )
 
 
-@operation
+@operation()
 def mount(
-    path,
+    path: str,
     mounted=True,
-    options=None,
-    device=None,
-    fs_type=None,
+    options: list[str] = None,
+    device: str = None,
+    fs_type: str = None,
     # TODO: do we want to manage fstab here?
     # update_fstab=False,
 ):
     """
     Manage mounted filesystems.
 
     + path: the path of the mounted filesystem
@@ -318,41 +318,37 @@
         if options_string:
             args.extend(["-o", options_string])
         if device:
             args.append(device)
         args.append(path)
 
         yield StringCommand("mount", *args)
-        # Should we update facts with fs_type, device, etc?
-        mounts[path] = {"options": options}
 
     # Want no mount but mounted?
     elif mounted is False and is_mounted:
         yield "umount {0}".format(path)
-        mounts.pop(path)
 
     # Want mount and is mounted! Check the options
     elif is_mounted and mounted and options:
         mounted_options = mounts[path]["options"]
         needed_options = set(options) - set(mounted_options)
         if needed_options:
             yield "mount -o remount,{0} {1}".format(options_string, path)
-            mounts[path]["options"] = options
 
     else:
         host.noop(
             "filesystem {0} is {1}".format(
                 path,
                 "mounted" if mounted else "not mounted",
             ),
         )
 
 
-@operation
-def hostname(hostname, hostname_file=None):
+@operation()
+def hostname(hostname: str, hostname_file: str = None):
     """
     Set the system hostname using ``hostnamectl`` or ``hostname`` on older systems.
 
     + hostname: the hostname that should be set
     + hostname_file: the file that permanently sets the hostname
 
     Hostname file:
@@ -375,45 +371,43 @@
     """
 
     current_hostname = host.get_fact(Hostname)
 
     if host.get_fact(Which, command="hostnamectl"):
         if current_hostname != hostname:
             yield "hostnamectl set-hostname {0}".format(hostname)
-            host.create_fact(Hostname, data=hostname)
         else:
             host.noop("hostname is set")
         return
 
     if hostname_file is None:
         os = host.get_fact(Os)
 
         if os == "Linux":
             hostname_file = "/etc/hostname"
         elif os == "OpenBSD":
             hostname_file = "/etc/myname"
 
     if current_hostname != hostname:
         yield "hostname {0}".format(hostname)
-        host.create_fact(Hostname, data=hostname)
     else:
         host.noop("hostname is set")
 
     if hostname_file:
         # Create a whole new hostname file
         file = StringIO("{0}\n".format(hostname))
 
         # And ensure it exists
-        yield from files.put(file, hostname_file)
+        yield from files.put._inner(src=file, dest=hostname_file)
 
 
-@operation
+@operation()
 def sysctl(
-    key,
-    value,
+    key: str,
+    value: str,
     persist=False,
     persist_file="/etc/sysctl.conf",
 ):
     """
     Edit sysctl configuration.
 
     + key: name of the sysctl setting to ensure
@@ -433,43 +427,42 @@
         )
     """
 
     string_value = " ".join(["{0}".format(v) for v in value]) if isinstance(value, list) else value
 
     value = [try_int(v) for v in value] if isinstance(value, list) else try_int(value)
 
-    existing_sysctls = host.get_fact(Sysctl)
-
+    existing_sysctls = host.get_fact(Sysctl, keys=[key])
     existing_value = existing_sysctls.get(key)
+
     if not existing_value or existing_value != value:
         yield "sysctl {0}='{1}'".format(key, string_value)
-        existing_sysctls[key] = value
     else:
         host.noop("sysctl {0} is set to {1}".format(key, string_value))
 
     if persist:
-        yield from files.line(
+        yield from files.line._inner(
             path=persist_file,
             line="{0}[[:space:]]*=[[:space:]]*{1}".format(key, string_value),
             replace="{0} = {1}".format(key, string_value),
         )
 
 
-@operation
+@operation()
 def service(
-    service,
+    service: str,
     running=True,
     restarted=False,
     reloaded=False,
-    command=None,
-    enabled=None,
+    command: str = None,
+    enabled: bool = None,
 ):
     """
     Manage the state of services. This command checks for the presence of all the
-    Linux init systems ``pyinfra`` can handle and executes the relevant operation.
+    Linux init systems pyinfra can handle and executes the relevant operation.
 
     + service: name of the service to manage
     + running: whether the service should be running
     + restarted: whether the service should be restarted
     + reloaded: whether the service should be reloaded
     + command: custom command execute
     + enabled: whether this service should be enabled/disabled on boot
@@ -481,14 +474,16 @@
         server.service(
             name="Enable open-vm-tools service",
             service="open-vm-tools",
             enabled=True,
         )
     """
 
+    service_operation: "PyinfraOperation"
+
     if host.get_fact(Which, command="systemctl"):
         service_operation = systemd.service
 
     elif host.get_fact(Which, command="rc-service"):
         service_operation = openrc.service
 
     elif host.get_fact(Which, command="initctl"):
@@ -499,54 +494,56 @@
         or host.get_fact(Link, path="/etc/init.d")
         or host.get_fact(Directory, path="/etc/init.d")
     ):
         service_operation = sysvinit.service
 
     # NOTE: important that we are not Linux here because /etc/rc.d will exist but checking it's
     # contents may trigger things (like a reboot: https://github.com/Fizzadar/pyinfra/issues/819)
-    elif host.get_fact(Os) != "Linux" and host.get_fact(Directory, path="/etc/rc.d"):
+    elif host.get_fact(Os) != "Linux" and bool(host.get_fact(Directory, path="/etc/rc.d")):
         service_operation = bsdinit.service
 
     else:
         raise OperationError(
             ("No init system found " "(no systemctl, initctl, /etc/init.d or /etc/rc.d found)"),
         )
 
-    yield from service_operation(
-        service,
+    yield from service_operation._inner(
+        service=service,
         running=running,
         restarted=restarted,
         reloaded=reloaded,
         command=command,
         enabled=enabled,
     )
 
 
-@operation
+@operation()
 def packages(
-    packages,
+    packages: str | list[str],
     present=True,
 ):
     """
     Add or remove system packages. This command checks for the presence of all the
-    system package managers ``pyinfra`` can handle and executes the relevant operation.
+    system package managers pyinfra can handle and executes the relevant operation.
 
     + packages: list of packages to ensure
     + present: whether the packages should be installed
 
     **Example:**
 
     .. code:: python
 
         server.packages(
             name="Install Vim and vimpager",
             packages=["vimpager", "vim"],
         )
     """
 
+    package_operation: "PyinfraOperation"
+
     # TODO: improve this - use LinuxDistribution fact + mapping with fallback below?
     # Here to be preferred on openSUSE which also provides aptitude
     # See: https://github.com/Fizzadar/pyinfra/issues/799
     if host.get_fact(Which, command="zypper"):
         package_operation = zypper.packages
 
     elif host.get_fact(Which, command="apk"):
@@ -577,29 +574,29 @@
         raise OperationError(
             (
                 "No system package manager found "
                 "(no apk, apt, brew, dnf, pacman, pkg, xbps, yum or zypper found)"
             ),
         )
 
-    yield from package_operation(packages=packages, present=present)
+    yield from package_operation._inner(packages=packages, present=present)
 
 
-@operation
+@operation()
 def crontab(
-    command,
+    command: str,
     present=True,
-    user=None,
-    cron_name=None,
+    user: str = None,
+    cron_name: str = None,
     minute="*",
     hour="*",
     month="*",
     day_of_week="*",
     day_of_month="*",
-    special_time=None,
+    special_time: str = None,
     interpolate_variables=False,
 ):
     """
     Add/remove/update crontab entries.
 
     + command: the command for the cron
     + present: whether this cron command should exist
@@ -653,23 +650,25 @@
 
     existing_crontab = crontab.get(command)
     existing_crontab_command = command
     existing_crontab_match = command
 
     if not existing_crontab and cron_name:  # find the crontab by name if provided
         for cmd, details in crontab.items():
+            if not details["comments"]:
+                continue
             if name_comment in details["comments"]:
                 existing_crontab = details
                 existing_crontab_match = cmd
                 existing_crontab_command = cmd
 
     exists = existing_crontab is not None
 
     edit_commands = []
-    temp_filename = state.get_temp_filename()
+    temp_filename = host.get_temp_filename()
 
     if special_time:
         new_crontab_line = "{0} {1}".format(special_time, command)
     else:
         new_crontab_line = "{minute} {hour} {day_of_month} {month} {day_of_week} {command}".format(
             minute=minute,
             hour=hour,
@@ -709,14 +708,15 @@
                 shlex.quote(new_crontab_line),
                 temp_filename,
             ),
         )
 
     # We have the cron and it exists, do it's details? If not, replace the line
     elif present and exists:
+        assert existing_crontab is not None
         if any(
             (
                 special_time != existing_crontab.get("special_time"),
                 minute != existing_crontab.get("minute"),
                 hour != existing_crontab.get("hour"),
                 month != existing_crontab.get("month"),
                 day_of_week != existing_crontab.get("day_of_week"),
@@ -744,39 +744,25 @@
 
         # Now yield any edits
         for edit_command in edit_commands:
             yield edit_command
 
         # Finally, use the tempfile to write a new crontab
         yield "crontab {0} {1}".format(" ".join(crontab_args), temp_filename)
-
-        # Update the crontab fact
-        if present:
-            crontab[command] = {
-                "special_time": special_time,
-                "minute": minute,
-                "hour": hour,
-                "month": month,
-                "day_of_week": day_of_week,
-                "day_of_month": day_of_month,
-                "comments": [cron_name] if cron_name else [],
-            }
-        else:
-            crontab.pop(command)
     else:
         host.noop(
             "crontab {0} {1}".format(
                 command,
                 "exists" if present else "does not exist",
             ),
         )
 
 
-@operation
-def group(group, present=True, system=False, gid=None):
+@operation()
+def group(group: str, present=True, system=False, gid: int = None):
     """
     Add/remove system groups.
 
     + group: name of the group to ensure
     + present: whether the group should be present or not
     + system: whether to create a system group
     + gid: use a specific groupid number
@@ -807,15 +793,14 @@
 
     # Group exists but we don't want them?
     if not present and is_present:
         if os_type == "FreeBSD":
             yield "pw groupdel -n {0}".format(group)
         else:
             yield "groupdel {0}".format(group)
-        groups.remove(group)
 
     # Group doesn't exist and we want it?
     elif present and not is_present:
         args = []
 
         # BSD doesn't do system users
         if system and "BSD" not in host.get_fact(Os):
@@ -833,49 +818,49 @@
                 args.append("--gid {0}".format(gid))
 
         # Groups are often added by other operations (package installs), so check
         # for the group at runtime before adding.
         group_add_command = "groupadd"
         if os_type == "FreeBSD":
             group_add_command = "pw groupadd"
-        yield "grep '^{0}:' /etc/group || {2} {1}".format(group, " ".join(args), group_add_command)
-        groups.append(group)
+        yield "{0} {1}".format(group_add_command, " ".join(args))
 
 
-@operation
+@operation()
 def user_authorized_keys(
-    user,
-    public_keys,
-    group=None,
+    user: str,
+    public_keys: str | list[str],
+    group: str = None,
     delete_keys=False,
-    authorized_key_directory=None,
-    authorized_key_filename=None,
+    authorized_key_directory: str = None,
+    authorized_key_filename: str = None,
 ):
     """
     Manage `authorized_keys` of system users.
 
     + user: name of the user to ensure
     + public_keys: list of public keys to attach to this user, ``home`` must be specified
     + group: the users primary group
     + delete_keys: whether to remove any keys not specified in ``public_keys``
 
     Public keys:
         These can be provided as strings containing the public key or as a path to
-        a public key file which ``pyinfra`` will read.
+        a public key file which pyinfra will read.
 
     **Examples:**
 
     .. code:: python
 
         server.user_authorized_keys(
             name="Ensure user has a public key",
             user="kevin",
             public_keys=["ed25519..."],
         )
     """
+
     if not authorized_key_directory:
         authorized_key_directory = f"/home/{user}/.ssh/"
     if not authorized_key_filename:
         authorized_key_filename = "authorized_keys"
 
     if isinstance(public_keys, str):
         public_keys = [public_keys]
@@ -885,23 +870,23 @@
         if state.cwd:
             try_path = path.join(state.cwd, key)
 
         if path.exists(try_path):
             with open(try_path, "r") as f:
                 return f.read().strip()
 
-        return key
+        return key.strip()
 
     public_keys = list(map(read_any_pub_key_file, public_keys))
 
     # Ensure .ssh directory
     # note that this always outputs commands unless the SSH user has access to the
     # authorized_keys file, ie the SSH user is the user defined in this function
-    yield from files.directory(
-        authorized_key_directory,
+    yield from files.directory._inner(
+        path=authorized_key_directory,
         user=user,
         group=group or user,
         mode=700,
     )
 
     authorized_key_file = f"{authorized_key_directory}/{authorized_key_filename}"
 
@@ -910,53 +895,54 @@
         keys_file = StringIO(
             "{0}\n".format(
                 "\n".join(public_keys),
             ),
         )
 
         # And ensure it exists
-        yield from files.put(
+        yield from files.put._inner(
             src=keys_file,
             dest=authorized_key_file,
             user=user,
             group=group or user,
             mode=600,
         )
 
     else:
         # Ensure authorized_keys exists
-        yield from files.file(
+        yield from files.file._inner(
             path=authorized_key_file,
             user=user,
             group=group or user,
             mode=600,
         )
 
         # And every public key is present
         for key in public_keys:
-            yield from files.line(path=authorized_key_file, line=key, ensure_newline=True)
+            yield from files.line._inner(path=authorized_key_file, line=key, ensure_newline=True)
 
 
-@operation
+@operation()
 def user(
-    user,
+    user: str,
     present=True,
-    home=None,
-    shell=None,
-    group=None,
-    groups=None,
-    public_keys=None,
+    home: str = None,
+    shell: str = None,
+    group: str = None,
+    groups: list[str] = None,
+    public_keys: str | list[str] = None,
     delete_keys=False,
     ensure_home=True,
     create_home=False,
     system=False,
-    uid=None,
-    comment=None,
+    uid: int = None,
+    comment: str = None,
     add_deploy_dir=True,
     unique=True,
+    password: str = None,
 ):
     """
     Add/remove/update system users & their ssh `authorized_keys`.
 
     + user: name of the user to ensure
     + present: whether this user should exist
     + home: the users home directory
@@ -968,24 +954,25 @@
     + ensure_home: whether to ensure the ``home`` directory exists
     + create_home: whether to new user create home directories from the system skeleton
     + system: whether to create a system account
     + uid: use a specific userid number
     + comment: the user GECOS comment
     + add_deploy_dir: any public_key filenames are relative to the deploy directory
     + unique: prevent creating users with duplicate UID
+    + password: set the encrypted password for the user
 
     Home directory:
         When ``ensure_home`` or ``public_keys`` are provided, ``home`` defaults to
         ``/home/{name}``. When ``create_home`` is ``True`` any newly created users
         will be created with the ``-m`` flag to build a new home directory from the
         systems skeleton directory.
 
     Public keys:
         These can be provided as strings containing the public key or as a path to
-        a public key file which ``pyinfra`` will read.
+        a public key file which pyinfra will read.
 
     **Examples:**
 
     .. code:: python
 
         server.user(
             name="Ensure user is removed",
@@ -1023,15 +1010,14 @@
     # User not wanted?
     if not present:
         if existing_user:
             if os_type == "FreeBSD":
                 yield "pw userdel -n {0}".format(user)
             else:
                 yield "userdel {0}".format(user)
-            users.pop(user)
         return
 
     # User doesn't exist but we want them?
     if present and existing_user is None:
         # Fix the case where a group of the same name already exists, tell useradd to use this
         # group rather than failing trying to create it.
         if not group and user in existing_groups:
@@ -1065,41 +1051,38 @@
             args.append("-c '{0}'".format(comment))
 
         if not unique:
             args.append("-o")
 
         if create_home:
             args.append("-m")
+        else:
+            args.append("-M")
+
+        if password:
+            args.append("-p '{0}'".format(password))
 
         # Users are often added by other operations (package installs), so check
         # for the user at runtime before adding.
-
         add_user_command = "useradd"
         if os_type == "FreeBSD":
             add_user_command = "pw useradd"
-            yield "grep '^{2}:' /etc/passwd || {0} -n {2} {1}".format(
+            yield "{0} -n {2} {1}".format(
                 add_user_command,
                 " ".join(args),
                 user,
             )
         else:
-            yield "grep '^{2}:' /etc/passwd || {0} {1} {2}".format(
+            yield "{0} {1} {2}".format(
                 add_user_command,
                 " ".join(args),
                 user,
             )
-        users[user] = {
-            "comment": comment,
-            "home": home,
-            "shell": shell,
-            "group": group,
-            "groups": groups,
-        }
 
-    # User exists and we want them, check home/shell/keys
+    # User exists and we want them, check home/shell/keys/password
     else:
         args = []
 
         # Check homedir
         if home and existing_user["home"] != home:
             args.append("-d {0}".format(home))
 
@@ -1114,14 +1097,17 @@
         # Check secondary groups, if defined
         if groups and set(existing_user["groups"]) != set(groups):
             args.append("-G {0}".format(",".join(groups)))
 
         if comment and existing_user["comment"] != comment:
             args.append("-c '{0}'".format(comment))
 
+        if password and existing_user["password"] != password:
+            args.append("-p '{0}'".format(password))
+
         # Need to mod the user?
         if args:
             if os_type == "FreeBSD":
                 yield "pw usermod -n {1} {0}".format(" ".join(args), user)
             else:
                 yield "usermod {0} {1}".format(" ".join(args), user)
             if comment:
@@ -1130,40 +1116,42 @@
                 existing_user["home"] = home
             if shell:
                 existing_user["shell"] = shell
             if group:
                 existing_user["group"] = group
             if groups:
                 existing_user["groups"] = groups
+            if password:
+                existing_user["password"] = password
 
     # Ensure home directory ownership
     if ensure_home:
-        yield from files.directory(
-            home,
+        yield from files.directory._inner(
+            path=home,
             user=user,
             group=group or user,
             # Don't fail if the home directory exists as a link
             _no_fail_on_link=True,
         )
 
     # Add SSH keys
     if public_keys is not None:
-        yield from user_authorized_keys(
-            user,
-            public_keys,
+        yield from user_authorized_keys._inner(
+            user=user,
+            public_keys=public_keys,
             group=group,
             delete_keys=delete_keys,
             authorized_key_directory="{0}/.ssh".format(home),
             authorized_key_filename=None,
         )
 
 
-@operation
+@operation()
 def locale(
-    locale,
+    locale: str,
     present=True,
 ):
     """
     Enable/Disable locale.
 
     + locale: name of the locale to enable/disable
     + present: whether this locale should be present or not
@@ -1204,24 +1192,61 @@
 
     matching_line = matching_lines[0]
 
     # Remove locale
     if not present and locale in locales:
         logger.debug(f"Removing locale {locale}")
 
-        yield from files.line(
+        yield from files.line._inner(
             path=locales_definitions_file, line=f"^{matching_line}$", replace=f"# {matching_line}"
         )
 
         yield "locale-gen"
 
     # Add locale
     if present and locale not in locales:
         logger.debug(f"Adding locale {locale}")
 
-        yield from files.replace(
+        yield from files.replace._inner(
             path=locales_definitions_file,
             text=f"^{matching_line}$",
             replace=f"{matching_line}".replace("# ", ""),
         )
 
         yield "locale-gen"
+
+
+@operation()
+def security_limit(
+    domain: str,
+    limit_type: str,
+    item: str,
+    value: int,
+):
+    """
+    Edit /etc/security/limits.conf configuration.
+
+    + domain: the domain (user, group, or wildcard) for the limit
+    + limit_type: the type of limit (hard or soft)
+    + item: the item to limit (e.g., nofile, nproc)
+    + value: the value for the limit
+
+    **Example:**
+
+    .. code:: python
+
+        security_limit(
+            name="Set nofile limit for all users",
+            domain='*',
+            limit_type='soft',
+            item='nofile',
+            value=1024,
+        )
+    """
+
+    line_format = f"{domain}\t{limit_type}\t{item}\t{value}"
+
+    yield from files.line._inner(
+        path="/etc/security/limits.conf",
+        line=f"^{domain}[[:space:]]+{limit_type}[[:space:]]+{item}",
+        replace=line_format,
+    )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/snap.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/snap.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 
 from pyinfra import host
 from pyinfra.api import operation
 from pyinfra.facts.snap import SnapPackage, SnapPackages
 
 
-@operation
+@operation()
 def package(
-    packages=None,
+    packages: str | list[str] = None,
     channel="latest/stable",
     classic=False,
     present=True,
 ):
     """
     Install/remove a snap package
 
@@ -87,22 +87,20 @@
                 if pkg_info and "channel" in pkg_info and channel != pkg_info["channel"]:
                     refresh_packages.append(package)
                     pkg_info["channel"] = channel
 
             else:
                 # we don't want it
                 remove_packages.append(package)
-                snap_packages.remove(package)
 
         # it's not installed
         if package not in snap_packages:
             # we want it
             if present:
                 install_packages.append(package)
-                snap_packages.append(package)
 
             # we don't want it
             else:
                 host.noop(f"snap package {package} is not installed")
 
     install_cmd = ["snap", "install"]
     if classic:
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/ssh.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/ssh.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 Execute commands and up/download files *from* the remote host.
 
 Eg: ``pyinfra -> inventory-host.net <-> another-host.net``
 """
 
 import shlex
 
-from pyinfra import host, state
+from pyinfra import host
 from pyinfra.api import OperationError, operation
 from pyinfra.facts.files import File, FindInFile
 from pyinfra.facts.server import Home
 
 from . import files
 
 
-@operation
-def keyscan(hostname, force=False, port=22):
+@operation()
+def keyscan(hostname: str, force=False, port=22):
     """
     Check/add hosts to the ``~/.ssh/known_hosts`` file.
 
     + hostname: hostname that should have a key in ``known_hosts``
     + force: if the key already exists, remove and rescan
 
     **Example:**
@@ -30,54 +30,44 @@
             name="Set add server two to known_hosts on one",
             hostname="two.example.com",
         )
     """
 
     homedir = host.get_fact(Home)
 
-    yield from files.directory(
+    yield from files.directory._inner(
         "{0}/.ssh".format(homedir),
         mode=700,
     )
 
     hostname_present = host.get_fact(
         FindInFile,
         path="{0}/.ssh/known_hosts".format(homedir),
         pattern=hostname,
     )
 
-    did_keyscan = False
     keyscan_command = "ssh-keyscan -p {0} {1} >> {2}/.ssh/known_hosts".format(
         port,
         hostname,
         homedir,
     )
 
     if not hostname_present:
         yield keyscan_command
-        did_keyscan = True
 
     elif force:
         yield "ssh-keygen -R {0}".format(hostname)
         yield keyscan_command
-        did_keyscan = True
 
     else:
         host.noop("host key for {0} already exists".format(hostname))
 
-    if did_keyscan:
-        host.create_fact(
-            FindInFile,
-            kwargs={"path": "{0}/.ssh/known_hosts".format(homedir), "pattern": hostname},
-            data=["{0} unknown unknown".format(hostname)],
-        )
-
 
 @operation(is_idempotent=False)
-def command(hostname, command, user=None, port=22):
+def command(hostname: str, command: str, user: str = None, port=22):
     """
     Execute commands on other servers over SSH.
 
     + hostname: the hostname to connect to
     + command: the command to execute
     + user: connect with this user
     + port: connect to this port
@@ -101,19 +91,19 @@
         connection_target = "@".join((user, hostname))
 
     yield "ssh -p {0} {1} {2}".format(port, connection_target, command)
 
 
 @operation(is_idempotent=False)
 def upload(
-    hostname,
-    filename,
-    remote_filename=None,
+    hostname: str,
+    filename: str,
+    remote_filename: str = None,
     port=22,
-    user=None,
+    user: str = None,
     use_remote_sudo=False,
     ssh_keyscan=False,
 ):
     """
     Upload files to other servers using ``scp``.
 
     + hostname: hostname to upload to
@@ -129,56 +119,56 @@
 
     # Figure out where we're connecting (host or user@host)
     connection_target = hostname
     if user:
         connection_target = "@".join((user, hostname))
 
     if ssh_keyscan:
-        yield from keyscan(hostname)
+        yield from keyscan._inner(hostname)
 
     # If we're not using sudo on the remote side, just scp the file over
     if not use_remote_sudo:
         yield "scp -P {0} {1} {2}:{3}".format(
             port,
             filename,
             connection_target,
             remote_filename,
         )
 
     else:
         # Otherwise - we need a temporary location for the file
-        temp_remote_filename = state.get_temp_filename()
+        temp_remote_filename = host.get_temp_filename()
 
         # scp it to the temporary location
         upload_cmd = "scp -P {0} {1} {2}:{3}".format(
             port,
             filename,
             connection_target,
             temp_remote_filename,
         )
 
         yield upload_cmd
 
         # And sudo sudo to move it
-        yield from command(
+        yield from command._inner(
             hostname=hostname,
             command="sudo mv {0} {1}".format(temp_remote_filename, remote_filename),
             port=port,
             user=user,
         )
 
 
-@operation
+@operation()
 def download(
-    hostname,
-    filename,
-    local_filename=None,
+    hostname: str,
+    filename: str,
+    local_filename: str = None,
     force=False,
     port=22,
-    user=None,
+    user: str = None,
     ssh_keyscan=False,
 ):
     """
     Download files from other servers using ``scp``.
 
     + hostname: hostname to upload to
     + filename: file to download
@@ -209,21 +199,16 @@
 
     # Figure out where we're connecting (host or user@host)
     connection_target = hostname
     if user:
         connection_target = "@".join((user, hostname))
 
     if ssh_keyscan:
-        yield from keyscan(hostname)
+        yield from keyscan._inner(hostname)
 
     # Download the file with scp
     yield "scp -P {0} {1}:{2} {3}".format(
         port,
         connection_target,
         filename,
         local_filename,
     )
-    host.create_fact(
-        File,
-        kwargs={"path": local_filename},
-        data={"mode": None, "group": None, "user": user, "mtime": None},
-    )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/systemd.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/systemd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 """
 Manage systemd services.
 """
 
 from pyinfra import host
-from pyinfra.api import operation
+from pyinfra.api import StringCommand, operation
 from pyinfra.facts.systemd import SystemdEnabled, SystemdStatus, _make_systemctl_cmd
 
 from .util.service import handle_service_control
 
 
 @operation(is_idempotent=False)
-def daemon_reload(user_mode=False, machine=None, user_name=None):
+def daemon_reload(user_mode=False, machine: str = None, user_name: str = None):
     """
     Reload the systemd daemon to read unit file changes.
 
     + user_mode: whether to use per-user systemd (systemctl --user) or not
     + machine: the machine name to connect to
     + user_name: connect to a specific user's systemd session
     """
 
     systemctl_cmd = _make_systemctl_cmd(
         user_mode=user_mode,
         machine=machine,
         user_name=user_name,
     )
 
-    yield "{0} daemon-reload".format(systemctl_cmd)
+    yield StringCommand(systemctl_cmd, "daemon-reload")
 
 
-_daemon_reload = daemon_reload  # noqa: E305
+_daemon_reload = daemon_reload._inner  # noqa: E305
 
 
-@operation
+@operation()
 def service(
-    service,
+    service: str,
     running=True,
     restarted=False,
     reloaded=False,
-    command=None,
-    enabled=None,
+    command: str = None,
+    enabled: bool = None,
     daemon_reload=False,
     user_mode=False,
-    machine=None,
-    user_name=None,
+    machine: str = None,
+    user_name: str = None,
 ):
     """
     Manage the state of systemd managed units.
 
     + service: name of the systemd unit to manage
     + running: whether the unit should be running
     + restarted: whether the unit should be restarted
@@ -113,33 +113,33 @@
         host,
         service,
         host.get_fact(
             SystemdStatus,
             user_mode=user_mode,
             machine=machine,
             user_name=user_name,
+            services=[service],
         ),
-        " ".join([systemctl_cmd, "{1}", "{0}"]),
+        " ".join([systemctl_cmd.get_raw_value(), "{1}", "{0}"]),
         running,
         restarted,
         reloaded,
         command,
     )
 
     if isinstance(enabled, bool):
         systemd_enabled = host.get_fact(
             SystemdEnabled,
             user_mode=user_mode,
             machine=machine,
             user_name=user_name,
+            services=[service],
         )
         is_enabled = systemd_enabled.get(service, False)
 
         # Isn't enabled and want enabled?
         if not is_enabled and enabled is True:
             yield "{0} enable {1}".format(systemctl_cmd, service)
-            systemd_enabled[service] = True
 
         # Is enabled and want disabled?
         elif is_enabled and enabled is False:
             yield "{0} disable {1}".format(systemctl_cmd, service)
-            systemd_enabled[service] = False
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/sysvinit.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/sysvinit.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from pyinfra.facts.server import LinuxDistribution
 from pyinfra.facts.sysvinit import InitdStatus
 
 from . import files
 from .util.service import handle_service_control
 
 
-@operation
+@operation()
 def service(
-    service,
+    service: str,
     running=True,
     restarted=False,
     reloaded=False,
-    enabled=None,
-    command=None,
+    enabled: bool = None,
+    command: str = None,
 ):
     """
     Manage the state of SysV Init (/etc/init.d) services.
 
     + service: name of the service to manage
     + running: whether the service should be running
     + restarted: whether the service should be restarted
@@ -71,44 +71,35 @@
             path="/etc/rc*.d/S*{0}".format(service),
             quote_path=False,  # enable path glob matching
         )
 
         # If no links exist, attempt to enable the service using distro-specific commands
         if enabled is True and not start_links:
             distro = host.get_fact(LinuxDistribution).get("name")
-            did_add = False
 
             if distro in ("Ubuntu", "Debian"):
                 yield "update-rc.d {0} defaults".format(service)
-                did_add = True
 
             elif distro in ("CentOS", "Fedora", "Red Hat Enterprise Linux"):
                 yield "chkconfig {0} --add".format(service)
                 yield "chkconfig {0} on".format(service)
-                did_add = True
 
             elif distro == "Gentoo":
                 yield "rc-update add {0} default".format(service)
-                did_add = True
-
-            # Add a single start link to the fact if we executed a command
-            if did_add:
-                start_links.append("/etc/rc0.d/S20{0}".format(service))
 
         # Remove any /etc/rcX.d/<service> start links
         elif enabled is False:
             # No state checking, just blindly remove any that exist
             for link in start_links:
                 yield "rm -f {0}".format(link)
-                start_links.remove(link)
 
 
-@operation
+@operation()
 def enable(
-    service,
+    service: str,
     start_priority=20,
     stop_priority=80,
     start_levels=(2, 3, 4, 5),
     stop_levels=(0, 1, 6),
 ):
     """
     Manually enable /etc/init.d scripts by creating /etc/rcX.d/Y links.
@@ -138,11 +129,11 @@
         links.append("/etc/rc{0}.d/S{1}{2}".format(level, start_priority, service))
 
     for level in stop_levels:
         links.append("/etc/rc{0}.d/K{1}{2}".format(level, stop_priority, service))
 
     # Ensure all the new links exist
     for link in links:
-        yield from files.link(
+        yield from files.link._inner(
             path=link,
             target="/etc/init.d/{0}".format(service),
         )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/util/files.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/util/files.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import re
 from datetime import datetime
 
 from pyinfra.api import QuoteString, StringCommand
 
 
-def unix_path_join(*parts):
-    parts = list(parts)
+def unix_path_join(*path_parts) -> str:
+    parts = list(path_parts)
     parts[0:-1] = [part.rstrip("/") for part in parts[0:-1]]
     return "/".join(parts)
 
 
-def ensure_mode_int(mode):
+def ensure_mode_int(mode: str | int | None) -> int | str | None:
     # Already an int (/None)?
     if isinstance(mode, int) or mode is None:
         return mode
 
     try:
         # Try making an int ('700' -> 700)
         return int(mode)
@@ -22,26 +22,26 @@
     except (TypeError, ValueError):
         pass
 
     # Return as-is (ie +x which we don't need to normalise, it always gets run)
     return mode
 
 
-def get_timestamp():
+def get_timestamp() -> str:
     return datetime.now().strftime("%y%m%d%H%M")
 
 
 def sed_replace(
-    filename,
-    line,
-    replace,
-    flags=None,
+    filename: str,
+    line: str,
+    replace: str,
+    flags: list[str] = None,
     backup=False,
     interpolate_variables=False,
-):
+) -> StringCommand:
     flags = "".join(flags) if flags else ""
 
     line = line.replace("/", r"\/")
     replace = str(replace)
     replace = replace.replace("/", r"\/")
     replace = replace.replace("&", r"\&")
     backup_extension = get_timestamp()
@@ -69,25 +69,27 @@
     if not backup:  # if we're not backing up, remove the file *if* sed succeeds
         backup_filename = "{0}.{1}".format(filename, backup_extension)
         sed_command = StringCommand(sed_command, "&&", "rm", "-f", QuoteString(backup_filename))
 
     return sed_command
 
 
-def chmod(target, mode, recursive=False):
+def chmod(target: str, mode: str, recursive=False) -> StringCommand:
     args = ["chmod"]
     if recursive:
         args.append("-R")
 
     args.append("{0}".format(mode))
 
     return StringCommand(" ".join(args), QuoteString(target))
 
 
-def chown(target, user, group=None, recursive=False, dereference=True):
+def chown(
+    target: str, user: str, group: str = None, recursive=False, dereference=True
+) -> StringCommand:
     command = "chown"
     user_group = None
 
     if user and group:
         user_group = "{0}:{1}".format(user, group)
 
     elif user:
@@ -103,15 +105,15 @@
 
     if not dereference:
         args.append("-h")
 
     return StringCommand(" ".join(args), user_group, QuoteString(target))
 
 
-def adjust_regex(line, escape_regex_characters):
+def adjust_regex(line: str, escape_regex_characters: bool) -> str:
     """
     Ensure the regex starts with '^' and ends with '$' and escape regex characters if requested
     """
     match_line = line
 
     if escape_regex_characters:
         match_line = re.sub(r"([\.\\\+\*\?\[\^\]\$\(\)\{\}\-])", r"\\\1", match_line)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/util/packaging.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/util/packaging.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import shlex
 from collections import defaultdict
 from io import StringIO
+from typing import Callable
 from urllib.parse import urlparse
 
+from pyinfra.api import Host, State
 from pyinfra.facts.files import File
 from pyinfra.facts.rpm import RpmPackage
+from pyinfra.operations import files
 
 
 def _package_name(package):
     if isinstance(package, list):
         return package[0]
     return package
 
@@ -39,104 +42,103 @@
 
     if match_any:
         return any(checks), package_name_to_versions
     return all(checks), package_name_to_versions
 
 
 def ensure_packages(
-    host,
-    packages,
-    current_packages,
-    present,
-    install_command,
-    uninstall_command,
+    host: Host,
+    packages_to_ensure: str | list[str],
+    current_packages_to_versions: dict[str, set[str]],
+    present: bool,
+    install_command: str,
+    uninstall_command: str,
     latest=False,
-    upgrade_command=None,
-    version_join=None,
-    expand_package_fact=None,
+    upgrade_command: str = None,
+    version_join: str = None,
+    expand_package_fact: Callable[[str], list[str]] = None,
 ):
     """
     Handles this common scenario:
 
     + We have a list of packages(/versions) to ensure
     + We have a map of existing package -> versions
     + We have the common command bits (install, uninstall, version "joiner")
     + Outputs commands to ensure our desired packages/versions
     + Optionally upgrades packages w/o specified version when present
 
     Args:
-        packages (list): list of packages or package/versions
-        current_packages (fact): fact returning dict of package names -> version
-        present (bool): whether packages should exist or not
-        install_command (str): command to prefix to list of packages to install
-        uninstall_command (str): as above for uninstalling packages
-        latest (bool): whether to upgrade installed packages when present
-        upgrade_command (str): as above for upgrading
-        version_join (str): the package manager specific "joiner", ie ``=`` for \
+        host: host object
+        packages_to_ensure: list of packages or package/versions
+        current_packages_to_versions: fact returning dict of package names -> version
+        present: whether packages should exist or not
+        install_command: command to prefix to list of packages to install
+        uninstall_command: as above for uninstalling packages
+        latest: whether to upgrade installed packages when present
+        upgrade_command: as above for upgrading
+        version_join: the package manager specific "joiner", ie ``=`` for \
             ``<apt_pkg>=<version>``
+        expand_package_fact: fact returning packages providing a capability \
+            (ie ``yum whatprovides``)
     """
 
-    if packages is None:
+    if packages_to_ensure is None:
         return
 
-    if isinstance(packages, str):
-        packages = [packages]
+    if isinstance(packages_to_ensure, str):
+        packages_to_ensure = [packages_to_ensure]
 
     if version_join:
-        packages = [
+        packages_to_ensure = [
             package[0] if len(package) == 1 else package
-            for package in [package.rsplit(version_join, 1) for package in packages]
+            for package in [package.rsplit(version_join, 1) for package in packages_to_ensure]
         ]
 
     diff_packages = []
-    diff_expanded_packages = {}
-
     upgrade_packages = []
 
     if present is True:
-        for package in packages:
+        for package in packages_to_ensure:
             has_package, expanded_packages = _has_package(
                 package,
-                current_packages,
+                current_packages_to_versions,
                 expand_package_fact,
             )
 
             if not has_package:
                 diff_packages.append(package)
-                diff_expanded_packages[_package_name(package)] = expanded_packages
             else:
                 # Present packages w/o version specified - for upgrade if latest
                 if isinstance(package, str):
                     upgrade_packages.append(package)
 
                 if not latest:
                     pkg_name = _package_name(package)
-                    if pkg_name in current_packages:
+                    if pkg_name in current_packages_to_versions:
                         host.noop(
                             "package {0} is installed ({1})".format(
                                 package,
-                                ", ".join(current_packages[pkg_name]),
+                                ", ".join(current_packages_to_versions[pkg_name]),
                             ),
                         )
                     else:
                         host.noop("package {0} is installed".format(package))
 
     if present is False:
-        for package in packages:
+        for package in packages_to_ensure:
             # String version, just check if existing
             has_package, expanded_packages = _has_package(
                 package,
-                current_packages,
+                current_packages_to_versions,
                 expand_package_fact,
                 match_any=True,
             )
 
             if has_package:
                 diff_packages.append(package)
-                diff_expanded_packages[_package_name(package)] = expanded_packages
             else:
                 host.noop("package {0} is not installed".format(package))
 
     if diff_packages:
         command = install_command if present else uninstall_command
 
         joined_packages = [
@@ -145,45 +147,31 @@
         ]
 
         yield "{0} {1}".format(
             command,
             " ".join([shlex.quote(pkg) for pkg in joined_packages]),
         )
 
-        for package in diff_packages:  # add/remove from current packages
-            pkg_name = _package_name(package)
-            version = "unknown"
-            if isinstance(package, list):
-                version = package[1]
-
-            if present:
-                current_packages[pkg_name] = [version]
-                current_packages.update(diff_expanded_packages.get(pkg_name, {}))
-            else:
-                current_packages.pop(pkg_name, None)
-                for name in diff_expanded_packages.get(pkg_name, {}):
-                    current_packages.pop(name, None)
-
     if latest and upgrade_command and upgrade_packages:
         yield "{0} {1}".format(
             upgrade_command,
             " ".join([shlex.quote(pkg) for pkg in upgrade_packages]),
         )
 
 
-def ensure_rpm(state, host, files, source, present, package_manager_command):
+def ensure_rpm(host: Host, source: str, present: bool, package_manager_command: str):
     original_source = source
 
     # If source is a url
     if urlparse(source).scheme:
         # Generate a temp filename (with .rpm extension to please yum)
-        temp_filename = "{0}.rpm".format(state.get_temp_filename(source))
+        temp_filename = "{0}.rpm".format(host.get_temp_filename(source))
 
         # Ensure it's downloaded
-        yield from files.download(source, temp_filename)
+        yield from files.download._inner(src=source, dest=temp_filename)
 
         # Override the source with the downloaded file
         source = temp_filename
 
     # Check for file .rpm information
     info = host.get_fact(RpmPackage, name=source)
     exists = False
@@ -195,69 +183,63 @@
             exists = True
 
     # Package does not exist and we want?
     if present and not exists:
         # If we had info, always install
         if info:
             yield "rpm -i {0}".format(source)
-            host.create_fact(RpmPackage, kwargs={"name": info["name"]}, data=info)
-
         # This happens if we download the package mid-deploy, so we have no info
         # but also don't know if it's installed. So check at runtime, otherwise
         # the install will fail.
         else:
             yield "rpm -q `rpm -qp {0}` 2> /dev/null || rpm -i {0}".format(source)
 
     # Package exists but we don't want?
     elif exists and not present:
         yield "{0} remove -y {1}".format(package_manager_command, info["name"])
-        host.delete_fact(RpmPackage, kwargs={"name": info["name"]})
-
     else:
         host.noop(
             "rpm {0} is {1}".format(
                 original_source,
                 "installed" if present else "not installed",
             ),
         )
 
 
 def ensure_yum_repo(
-    state,
-    host,
-    files,
-    name_or_url,
-    baseurl,
-    present,
-    description,
-    enabled,
-    gpgcheck,
-    gpgkey,
+    host: Host,
+    name_or_url: str,
+    baseurl: str,
+    present: bool,
+    description: str,
+    enabled: bool,
+    gpgcheck: bool,
+    gpgkey: str,
     repo_directory="/etc/yum.repos.d/",
-    type_=None,
+    type_: str = None,
 ):
     url = None
     url_parts = urlparse(name_or_url)
     if url_parts.scheme:
         url = name_or_url
         name_or_url = url_parts.path.split("/")[-1]
         if name_or_url.endswith(".repo"):
             name_or_url = name_or_url[:-5]
 
     filename = "{0}{1}.repo".format(repo_directory, name_or_url)
 
     # If we don't want the repo, just remove any existing file
     if not present:
-        yield from files.file(filename, present=False)
+        yield from files.file._inner(path=filename, present=False)
         return
 
     # If we're a URL, download the repo if it doesn't exist
     if url:
         if not host.get_fact(File, path=filename):
-            yield from files.download(url, filename)
+            yield from files.download._inner(src=url, dest=filename)
         return
 
     # Description defaults to name
     description = description or name_or_url
 
     # Build the repo file from string
     repo_lines = [
@@ -272,11 +254,11 @@
         repo_lines.append("type={0}".format(type_))
 
     if gpgkey:
         repo_lines.append("gpgkey={0}".format(gpgkey))
 
     repo_lines.append("")
     repo = "\n".join(repo_lines)
-    repo = StringIO(repo)
+    repo_file = StringIO(repo)
 
     # Ensure this is the file on the server
-    yield from files.put(repo, filename)
+    yield from files.put._inner(src=repo_file, dest=filename)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/util/service.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/util/service.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,42 @@
+from pyinfra.api import Host
+
+
 def handle_service_control(
-    host,
-    name,
-    statuses,
-    formatter,
-    running,
-    restarted,
-    reloaded,
-    command,
+    host: Host,
+    name: str,
+    statuses: dict[str, bool],
+    formatter: str,
+    running: bool = None,
+    restarted: bool = None,
+    reloaded: bool = None,
+    command: str = None,
     status_argument="status",
 ):
     status = statuses.get(name, None)
 
-    # If we don't know the status, we need to check if it's up before starting
-    # and/or restarting/reloading
-    if status is None:
-        yield (
-            "if ({status_command}); then "
-            "({stop_command}); ({restart_command}); ({reload_command}); "
-            "else ({start_command}); fi"
-        ).format(
-            status_command=formatter.format(name, status_argument),
-            start_command=(formatter.format(name, "start") if running is True else "true"),
-            stop_command=(formatter.format(name, "stop") if running is False else "true"),
-            restart_command=(formatter.format(name, "restart") if restarted else "true"),
-            reload_command=(formatter.format(name, "reload") if reloaded else "true"),
-        )
-        statuses[name] = running
-
-    else:
-        # Need down but running
-        if running is False:
-            if status:
-                yield formatter.format(name, "stop")
-                statuses[name] = False
-            else:
-                host.noop("service {0} is stopped".format(name))
-
-        # Need running but down
-        if running is True:
-            if not status:
-                yield formatter.format(name, "start")
-                statuses[name] = True
-            else:
-                host.noop("service {0} is running".format(name))
-
-        # Only restart if the service is already running
-        if restarted and status:
-            yield formatter.format(name, "restart")
-
-        # Only reload if the service is already reloaded
-        if reloaded and status:
-            yield formatter.format(name, "reload")
+    # Need down but running
+    if running is False:
+        if status:
+            yield formatter.format(name, "stop")
+        else:
+            host.noop("service {0} is stopped".format(name))
+
+    # Need running but down
+    if running is True:
+        if not status:
+            yield formatter.format(name, "start")
+        else:
+            host.noop("service {0} is running".format(name))
+
+    # Only restart if the service is already running
+    if restarted and status:
+        yield formatter.format(name, "restart")
+
+    # Only reload if the service is already reloaded
+    if reloaded and status:
+        yield formatter.format(name, "reload")
 
     # Always execute arbitrary commands as these may or may not rely on the service
     # being up or down
     if command:
         yield formatter.format(name, command)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/vzctl.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/vzctl.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from pyinfra import host
 from pyinfra.api import OperationError, operation
 from pyinfra.facts.vzctl import OpenvzContainers
 
 
 @operation(is_idempotent=False)
-def start(ctid, force=False):
+def start(ctid: str, force=False):
     """
     Start OpenVZ containers.
 
     + ctid: CTID of the container to start
     + force: whether to force container start
     """
 
@@ -21,74 +21,74 @@
     if force:
         args.append("--force")
 
     yield "vzctl start {0}".format(" ".join(args))
 
 
 @operation(is_idempotent=False)
-def stop(ctid):
+def stop(ctid: str):
     """
     Stop OpenVZ containers.
 
     + ctid: CTID of the container to stop
     """
 
     args = ["{0}".format(ctid)]
 
     yield "vzctl stop {0}".format(" ".join(args))
 
 
 @operation(is_idempotent=False)
-def restart(ctid, force=False):
+def restart(ctid: str, force=False):
     """
     Restart OpenVZ containers.
 
     + ctid: CTID of the container to restart
     + force: whether to force container start
     """
 
-    yield from stop(ctid)
-    yield from start(ctid, force=force)
+    yield from stop._inner(ctid=ctid)
+    yield from start._inner(ctid=ctid, force=force)
 
 
 @operation(is_idempotent=False)
-def mount(ctid):
+def mount(ctid: str):
     """
     Mount OpenVZ container filesystems.
 
     + ctid: CTID of the container to mount
     """
 
     yield "vzctl mount {0}".format(ctid)
 
 
 @operation(is_idempotent=False)
-def unmount(ctid):
+def unmount(ctid: str):
     """
     Unmount OpenVZ container filesystems.
 
     + ctid: CTID of the container to unmount
     """
 
     yield "vzctl umount {0}".format(ctid)
 
 
 @operation(is_idempotent=False)
-def delete(ctid):
+def delete(ctid: str):
     """
     Delete OpenVZ containers.
 
     + ctid: CTID of the container to delete
     """
 
     yield "vzctl delete {0}".format(ctid)
 
 
 @operation(is_idempotent=False)
-def create(ctid, template=None):
+def create(ctid: str, template: str = None):
     """
     Create OpenVZ containers.
 
     + ctid: CTID of the container to create
     """
 
     # Check we don't already have a container with this CTID
@@ -103,15 +103,15 @@
     if template:
         args.append("--ostemplate {0}".format(template))
 
     yield "vzctl create {0}".format(" ".join(args))
 
 
 @operation(is_idempotent=False)
-def set(ctid, save=True, **settings):
+def set(ctid: str, save=True, **settings):
     """
     Set OpenVZ container details.
 
     + ctid: CTID of the container to set
     + save: whether to save the changes
     + settings: settings/arguments to apply to the container
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/xbps.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/xbps.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,32 +14,32 @@
     """
     Upgrades all XBPS packages.
     """
 
     yield "xbps-install -y -u"
 
 
-_upgrade = upgrade  # noqa: E305
+_upgrade = upgrade._inner  # noqa: E305
 
 
 @operation(is_idempotent=False)
 def update():
     """
     Update XBPS repositories.
     """
 
     yield "xbps-install -S"
 
 
-_update = update  # noqa: E305
+_update = update._inner  # noqa: E305
 
 
-@operation
+@operation()
 def packages(
-    packages=None,
+    packages: str | list[str] = None,
     present=True,
     update=False,
     upgrade=False,
 ):
     """
     Install/remove/update XBPS packages.
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/yum.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/dnf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,214 +1,211 @@
 """
-Manage yum packages and repositories. Note that yum package names are case-sensitive.
+Manage dnf packages and repositories. Note that dnf package names are case-sensitive.
 """
 
 from pyinfra import host, state
 from pyinfra.api import operation
 from pyinfra.facts.rpm import RpmPackageProvides, RpmPackages
 
-from . import files
 from .util.packaging import ensure_packages, ensure_rpm, ensure_yum_repo
 
 
 @operation(is_idempotent=False)
-def key(src):
+def key(src: str):
     """
-    Add yum gpg keys with ``rpm``.
+    Add dnf gpg keys with ``rpm``.
 
-    + src: filename or URL
+    + key: filename or URL
 
     Note:
-        always returns one command, not state checking
+        always returns one command, not idempotent
 
     **Example:**
 
     .. code:: python
 
         linux_id = host.get_fact(LinuxDistribution)["release_meta"].get("ID")
-        yum.key(
+        dnf.key(
             name="Add the Docker CentOS gpg key",
             src=f"https://download.docker.com/linux/{linux_id}/gpg",
         )
 
     """
 
     yield "rpm --import {0}".format(src)
 
 
-@operation
+@operation()
 def repo(
-    src,
+    src: str,
     present=True,
-    baseurl=None,
-    description=None,
+    baseurl: str = None,
+    description: str = None,
     enabled=True,
     gpgcheck=True,
-    gpgkey=None,
+    gpgkey: str = None,
 ):
-    # NOTE: if updating this docstring also update `dnf.repo`
+    # NOTE: if updating this docstring also update `yum.repo`
     """
-    Add/remove/update yum repositories.
+    Add/remove/update dnf repositories.
 
     + src: URL or name for the ``.repo``   file
     + present: whether the ``.repo`` file should be present
     + baseurl: the baseurl of the repo (if ``name`` is not a URL)
     + description: optional verbose description
     + enabled: whether this repo is enabled
     + gpgcheck: whether set ``gpgcheck=1``
     + gpgkey: the URL to the gpg key for this repo
 
     ``Baseurl``/``description``/``gpgcheck``/``gpgkey``:
-        These are only valid when ``src`` is a filename (ie not a URL). This is
+        These are only valid when ``name`` is a filename (ie not a URL). This is
         for manual construction of repository files. Use a URL to download and
         install remote repository files.
 
     **Examples:**
 
     .. code:: python
 
         # Download a repository file
-        yum.repo(
+        dnf.rpm(
             name="Install Docker-CE repo via URL",
             src="https://download.docker.com/linux/centos/docker-ce.repo",
         )
 
         # Create the repository file from baseurl/etc
-        yum.repo(
+        dnf.repo(
             name="Add the Docker CentOS repo",
             src="DockerCE",
             baseurl="https://download.docker.com/linux/centos/7/$basearch/stable",
         )
     """
 
     yield from ensure_yum_repo(
-        state,
         host,
-        files,
         src,
         baseurl,
         present,
         description,
         enabled,
         gpgcheck,
         gpgkey,
     )
 
 
-@operation
-def rpm(src, present=True):
-    # NOTE: if updating this docstring also update `dnf.rpm`
+@operation()
+def rpm(src: str, present=True):
+    # NOTE: if updating this docstring also update `yum.rpm`
     """
     Add/remove ``.rpm`` file packages.
 
     + src: filename or URL of the ``.rpm`` package
     + present: whether ore not the package should exist on the system
 
     URL sources with ``present=False``:
         If the ``.rpm`` file isn't downloaded, pyinfra can't remove any existing
         package as the file won't exist until mid-deploy.
 
     **Example:**
 
     .. code:: python
 
-        major_version = host.get_fact(LinuxDistribution)["major"]
+        major_centos_version = host.get_fact(LinuxDistribution)["major"]
         dnf.rpm(
            name="Install EPEL rpm to enable EPEL repo",
-           src=f"https://dl.fedoraproject.org/pub/epel/epel-release-latest-{major_version}.noarch.rpm",
+           src=f"https://dl.fedoraproject.org/pub/epel/epel-release-latest-{major_centos_version}.noarch.rpm",
         )
     """
 
-    yield from ensure_rpm(state, host, files, src, present, "yum")
+    yield from ensure_rpm(host, src, present, "dnf")
 
 
 @operation(is_idempotent=False)
 def update():
     """
-    Updates all yum packages.
+    Updates all dnf packages.
     """
 
-    yield "yum update -y"
+    yield "dnf update -y"
 
 
-_update = update  # noqa: E305 (for use below where update is a kwarg)
+_update = update._inner  # noqa: E305 (for use below where update is a kwarg)
 
 
-@operation
+@operation()
 def packages(
-    packages=None,
+    packages: str | list[str] = None,
     present=True,
     latest=False,
     update=False,
     clean=False,
     nobest=False,
-    extra_install_args=None,
-    extra_uninstall_args=None,
+    extra_install_args: str = None,
+    extra_uninstall_args: str = None,
 ):
     """
-    Install/remove/update yum packages & updates.
+    Install/remove/update dnf packages & updates.
 
-    + packages: list of packages to ensure
+    + packages: packages to ensure
     + present: whether the packages should be installed
     + latest: whether to upgrade packages without a specified version
-    + update: run ``yum update`` before installing packages
-    + clean: run ``yum clean all`` before installing packages
+    + update: run ``dnf update`` before installing packages
+    + clean: run ``dnf clean`` before installing packages
     + nobest: add the no best option to install
-    + extra_install_args: additional arguments to the yum install command
-    + extra_uninstall_args: additional arguments to the yum uninstall command
+    + extra_install_args: additional arguments to the dnf install command
+    + extra_uninstall_args: additional arguments to the dnf uninstall command
 
     Versions:
         Package versions can be pinned as follows: ``<pkg>=<version>``
 
     **Examples:**
 
     .. code:: python
 
         # Update package list and install packages
-        yum.packages(
-            name="Install Vim and Vim enhanced",
+        dnf.packages(
+            name='Install Vim and Vim enhanced',
             packages=["vim-enhanced", "vim"],
             update=True,
         )
 
         # Install the latest versions of packages (always check)
-        yum.packages(
+        dnf.packages(
             name="Install latest Vim",
             packages=["vim"],
             latest=True,
         )
     """
 
     if clean:
-        yield "yum clean all"
+        yield "dnf clean all"
 
     if update:
         yield from _update()
 
-    install_command = ["yum", "install", "-y"]
+    install_command = ["dnf", "install", "-y"]
 
     if nobest:
         install_command.append("--nobest")
 
     if extra_install_args:
         install_command.append(extra_install_args)
 
-    uninstall_command = ["yum", "remove", "-y"]
+    uninstall_command = ["dnf", "remove", "-y"]
 
     if extra_uninstall_args:
         uninstall_command.append(extra_uninstall_args)
 
     yield from ensure_packages(
         host,
         packages,
         host.get_fact(RpmPackages),
         present,
         install_command=" ".join(install_command),
         uninstall_command=" ".join(uninstall_command),
-        upgrade_command="yum update -y",
+        upgrade_command="dnf update -y",
         version_join="=",
         latest=latest,
         expand_package_fact=lambda package: host.get_fact(
             RpmPackageProvides,
             name=package,
         ),
     )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/operations/zypper.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/operations/zypper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from pyinfra import host, state
 from pyinfra.api import operation
 from pyinfra.facts.rpm import RpmPackages
 
-from . import files
 from .util.packaging import ensure_packages, ensure_rpm, ensure_yum_repo
 from .yum import key as yum_key
 
 key = yum_key
 
 
-@operation
+@operation()
 def repo(
     src,
     baseurl=None,
     present=True,
     description=None,
     enabled=True,
     gpgcheck=True,
@@ -52,30 +51,28 @@
             name="Install container virtualization repo",
             src=="Virtualization:containers (openSUSE_Tumbleweed)",
             baseurl="https://download.opensuse.org/repositories/Virtualization:/containers/openSUSE_Tumbleweed/",
         )
     """
 
     yield from ensure_yum_repo(
-        state,
         host,
-        files,
         src,
         baseurl,
         present,
         description,
         enabled,
         gpgcheck,
         gpgkey,
         type_=type,
         repo_directory="/etc/zypp/repos.d/",
     )
 
 
-@operation
+@operation()
 def rpm(src, present=True):
     # NOTE: if updating this docstring also update `dnf.rpm`
     """
     Add/remove ``.rpm`` file packages.
 
     + src: filename or URL of the ``.rpm`` package
     + present: whether ore not the package should exist on the system
@@ -90,40 +87,40 @@
 
         zypper.rpm(
            name="Install task from rpm",
            src="https://github.com/go-task/task/releases/download/v2.8.1/task_linux_amd64.rpm",
         )
     """
 
-    yield from ensure_rpm(state, host, files, src, present, "zypper --non-interactive")
+    yield from ensure_rpm(host, src, present, "zypper --non-interactive")
 
 
 @operation(is_idempotent=False)
 def update():
     """
     Updates all zypper packages.
     """
 
     yield "zypper update -y"
 
 
-_update = update  # noqa: E305 (for use below where update is a kwarg)
+_update = update._inner  # noqa: E305 (for use below where update is a kwarg)
 
 
-@operation
+@operation()
 def packages(
-    packages=None,
+    packages: str | list[str] = None,
     present=True,
     latest=False,
     update=False,
     clean=False,
-    extra_global_install_args=None,
-    extra_install_args=None,
-    extra_global_uninstall_args=None,
-    extra_uninstall_args=None,
+    extra_global_install_args: str = None,
+    extra_install_args: str = None,
+    extra_global_uninstall_args: str = None,
+    extra_uninstall_args: str = None,
 ):
     """
     Install/remove/update zypper packages & updates.
 
     + packages: list of packages to ensure
     + present: whether the packages should be installed
     + latest: whether to upgrade packages without a specified version
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra/progress.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra/progress.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/__main__.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 # Set CLI mode
 pyinfra.is_cli = True
 
 # Don't write out deploy.pyc/config.pyc etc
 sys.dont_write_bytecode = True
 
+sys.path.append(".")
+
 # Shut it click
 click.disable_unicode_literals_warning = True  # type: ignore
 
 # Force line buffering
 sys.stdout = os.fdopen(sys.stdout.fileno(), "w", 1)
 sys.stderr = os.fdopen(sys.stderr.fileno(), "w", 1)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/commands.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+from __future__ import annotations
+
 import json
 
+from pyinfra.api.facts import FactBase
+
 from .exceptions import CliError
 from .util import parse_cli_arg, try_import_module_attribute
 
 
 def get_func_and_args(commands):
     operation_name = commands[0]
 
@@ -28,34 +32,35 @@
         for key, value in [arg.split("=", 1) for arg in operation_args if "=" in arg]
     }
 
     return op, (args, kwargs)
 
 
 def get_facts_and_args(commands):
-    facts = []
+    facts: list[tuple[FactBase, tuple, dict]] = []
 
     current_fact = None
 
     for command in commands:
         if "=" in command:
             if not current_fact:
                 raise CliError("Invalid fact commands: `{0}`".format(commands))
 
             key, value = command.split("=", 1)
-            current_fact[2][key] = value
+            current_fact[2][key] = parse_cli_arg(value)
             continue
 
         if current_fact:
             facts.append(current_fact)
             current_fact = None
 
         if "." not in command:
             raise CliError(f"Invalid fact: `{command}`, should be in the format `module.cls`")
 
         fact_cls = try_import_module_attribute(command, prefix="pyinfra.facts")
+        assert fact_cls is not None
         current_fact = (fact_cls, (), {})
 
     if current_fact:
         facts.append(current_fact)
 
     return facts
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/inventory.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/inventory.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+import socket
 from collections import defaultdict
 from os import listdir, path
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar, Union
 
 from pyinfra import logger
 from pyinfra.api.inventory import Inventory
@@ -81,18 +83,31 @@
 
 def make_inventory(
     inventory: str,
     override_data=None,
     cwd: Optional[str] = None,
     group_data_directories=None,
 ):
-    # First, try loading the inventory as if it's a Python import function
-    try:
-        inventory_func = try_import_module_attribute(inventory)
-    except (CliError, ValueError):
+    inventory_func = None
+
+    # (Un)fortunately the CLI is pretty flexible for inventory inputs; we support a single hostname,
+    # a Python module.function import or a Python file path. All of these are kind of similar, and
+    # we want error handling to be a good user experience.
+    # Thus, we'll check for everything but also drop a warning to the console if the inventory looks
+    # like either an import or hostname but neither works.
+    if re.match("[a-zA-Z0-9\\._]+[\\.:][a-zA-Z0-9_]+", inventory):
+        # First, try loading the inventory as if it's a Python import function
+        inventory_func = try_import_module_attribute(inventory, raise_for_none=False)
+        if inventory_func is None:
+            try:
+                socket.gethostbyname(inventory)
+            except socket.gaierror:
+                logger.warning(f"{inventory} is neither a valid Python import or hostname.")
+
+    if inventory_func is None:
         # If not an import, load as if from the filesystem *or* comma separated list, which also
         # loads any all.py group data files (imported functions do not load group data).
         return make_inventory_from_files(inventory, override_data, cwd, group_data_directories)
     else:
         return make_inventory_from_func(inventory_func, override_data)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/main.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 from pyinfra import __version__, logger, state
 from pyinfra.api import Config, State
 from pyinfra.api.connect import connect_all, disconnect_all
 from pyinfra.api.exceptions import NoGroupError, PyinfraError
 from pyinfra.api.facts import get_facts
 from pyinfra.api.operations import run_ops
+from pyinfra.api.state import StateStage
 from pyinfra.api.util import get_kwargs_str
 from pyinfra.context import ctx_config, ctx_inventory, ctx_state
 from pyinfra.operations import server
 
 from .commands import get_facts_and_args, get_func_and_args
-from .exceptions import CliError, UnexpectedExternalError, UnexpectedInternalError
+from .exceptions import CliError, UnexpectedExternalError, UnexpectedInternalError, WrappedError
 from .inventory import make_inventory
 from .log import setup_logging
 from .prints import (
     print_facts,
     print_inventory,
     print_meta,
     print_results,
-    print_state_facts,
     print_state_operations,
     print_support_info,
 )
 from .util import exec_file, load_deploy_file, load_func, parse_cli_arg
 from .virtualenv import init_virtualenv
 
 
@@ -40,15 +40,15 @@
     sys.exit(0)
 
 
 def _print_support(ctx, param, value):
     if not value:
         return
 
-    click.echo("--> Support information:", err=True)
+    logger.info("--> Support information:")
     print_support_info()
     ctx.exit()
 
 
 @click.command()
 @click.argument("inventory", nargs=1, type=click.Path(exists=False))
 @click.argument("operations", nargs=-1, required=True, type=click.Path(exists=False))
@@ -61,14 +61,23 @@
 @click.option(
     "--dry",
     is_flag=True,
     default=False,
     help="Don't execute operations on the target hosts.",
 )
 @click.option(
+    "-y",
+    "--yes",
+    is_flag=True,
+    default=False,
+    help="Execute operations immediately on hosts without prompt or checking for changes.",
+    envvar="PYINFRA_YES",
+    show_envvar=True,
+)
+@click.option(
     "--limit",
     help="Restrict the target hosts by name and group name.",
     multiple=True,
 )
 @click.option("--fail-percent", type=int, help="% of hosts that need to fail before exiting early.")
 @click.option(
     "--data",
@@ -128,19 +137,14 @@
 @click.option(
     "--ssh-key-password",
     "--key-password",
     "ssh_key_password",
     help="SSH Private key password.",
 )
 @click.option("--ssh-password", "--password", "ssh_password", help="SSH password.")
-# WinRM connector args
-@click.option("--winrm-username", help="WINRM user to connect as.")
-@click.option("--winrm-password", help="WINRM password.")
-@click.option("--winrm-port", help="WINRM port to connect to.")
-@click.option("--winrm-transport", help="WINRM transport for use.")
 # Eager commands (pyinfra --support)
 @click.option(
     "--support",
     is_flag=True,
     is_eager=True,
     callback=_print_support,
     help="Print useful information for support and exit.",
@@ -152,15 +156,21 @@
     default=False,
     help="Hide most pyinfra output.",
 )
 @click.option(
     "--debug",
     is_flag=True,
     default=False,
-    help="Print debug info.",
+    help="Print debug logs from pyinfra.",
+)
+@click.option(
+    "--debug-all",
+    is_flag=True,
+    default=False,
+    help="Print debug logs from all packages including pyinfra.",
 )
 @click.option(
     "--debug-facts",
     is_flag=True,
     default=False,
     help="Print facts after generating operations and exit.",
 )
@@ -212,34 +222,25 @@
     \b
     # Debug the inventory hosts and data
     pyinfra INVENTORY debug-inventory
     """
 
     try:
         _main(*args, **kwargs)
-
-    except PyinfraError as e:
-        # Re-raise any internal exceptions that aren't handled by click as
-        # CliErrors which are.
-        if not isinstance(e, click.ClickException):
-            message = getattr(e, "message", e.args[0])
-            raise CliError(message)
-
-        raise
-
-    except UnexpectedExternalError:
-        # Pass unexpected external exceptions through as-is
+    except (CliError, UnexpectedExternalError):
         raise
-
+    except PyinfraError as e:
+        # Re-raise "expected" pyinfra exceptions with our click exception wrapper
+        raise WrappedError(e)
     except Exception as e:
         # Re-raise any unexpected internal exceptions as UnexpectedInternalError
         raise UnexpectedInternalError(e)
-
     finally:
         if ctx_state.isset() and state.initialised:
+            logger.info("--> Disconnecting from hosts...")
             # Triggers any executor disconnect requirements
             disconnect_all(state)
 
 
 class CliCommands:
     DEBUG_INVENTORY = "DEBUG_INVENTORY"
     FACT = "FACT"
@@ -254,55 +255,53 @@
     verbosity: int,
     chdir: str,
     ssh_user,
     ssh_port: int,
     ssh_key,
     ssh_key_password: str,
     ssh_password: str,
-    winrm_username: str,
-    winrm_password: str,
-    winrm_port,
-    winrm_transport,
     shell_executable,
     sudo: bool,
     sudo_user: str,
     use_sudo_password: bool,
     su_user: str,
     parallel: int,
     fail_percent: int,
     data,
     group_data,
     config_filename: str,
     dry: bool,
+    yes: bool,
     limit: Iterable,
     no_wait: bool,
     serial: bool,
     quiet: bool,
     debug: bool,
+    debug_all: bool,
     debug_facts: bool,
     debug_operations: bool,
-    support: bool = None,
+    support: bool = False,
 ):
     # Setup working directory
     #
     if chdir:
         os_chdir(chdir)
 
     # Setup logging & Bootstrap/Venv
     #
-    _setup_log_level(debug, quiet)
+    _setup_log_level(debug, debug_all)
     init_virtualenv()
 
     # Check operations are valid and setup commands
     #
     original_operations, operations, command, chdir = _validate_operations(operations, chdir)
 
     # Setup state, config & inventory
     #
-    state = _setup_state(verbosity, quiet)
+    state = _setup_state(verbosity, quiet, yes)
     config = Config()
     ctx_config.set(config)
 
     # Update Config & Override Data
     #
     config = _set_config(
         config,
@@ -310,32 +309,31 @@
         sudo,
         sudo_user,
         use_sudo_password,
         su_user,
         parallel,
         shell_executable,
         fail_percent,
-        quiet,
+        yes,
     )
     override_data = _set_override_data(
         data,
         ssh_user,
         ssh_key,
         ssh_key_password,
         ssh_port,
         ssh_password,
-        winrm_username,
-        winrm_password,
-        winrm_port,
-        winrm_transport,
     )
 
+    if yes is False:
+        _set_fail_prompts(state, config)
+
     # Load up the inventory from the filesystem
     #
-    echo_msg("--> Loading inventory...", quiet)
+    logger.info("--> Loading inventory...")
     inventory = make_inventory(
         inventory,
         cwd=state.cwd,
         override_data=override_data,
         group_data_directories=group_data,
     )
     ctx_inventory.set(inventory)
@@ -348,63 +346,104 @@
 
     if command == CliCommands.DEBUG_INVENTORY:
         print_inventory(state)
         _exit()
 
     # Connect to the hosts & start handling the user commands
     #
-    echo_msg("--> Connecting to hosts...", quiet)
+    logger.info("--> Connecting to hosts...")
+    state.set_stage(StateStage.Connect)
     connect_all(state)
-    state, config = _handle_commands(state, config, command, original_operations, operations, quiet)
+
+    logger.info("--> Preparing operations...")
+    state.set_stage(StateStage.Prepare)
+    can_diff, state, config = _handle_commands(
+        state, config, command, original_operations, operations
+    )
 
     # Print proposed changes, execute unless --dry, and exit
     #
-    echo_msg("--> Proposed changes:", quiet)
-    print_meta(state)
+    if can_diff:
+        if yes:
+            logger.info("--> Skipping change detection")
+        else:
+            logger.info("--> Detected changes:")
+            print_meta(state)
 
     # If --debug-facts or --debug-operations, print and exit
     if debug_facts or debug_operations:
-        if debug_facts:
-            print_state_facts(state)
-
         if debug_operations:
             print_state_operations(state)
 
         _exit()
 
     if dry:
         _exit()
 
-    echo_msg(quiet=quiet)
-    echo_msg("--> Beginning operation run...", quiet)
+    if (
+        can_diff
+        and not yes
+        and not _do_confirm("Detected changes displayed above, skip this step with -y")
+    ):
+        _exit()
 
+    logger.info("--> Beginning operation run...")
+    state.set_stage(StateStage.Execute)
     run_ops(state, serial=serial, no_wait=no_wait)
 
-    echo_msg("--> Results:", quiet)
+    logger.info("--> Results:")
+    state.set_stage(StateStage.Disconnect)
     print_results(state)
     _exit()
 
 
+def _do_confirm(msg: str) -> bool:
+    click.echo(err=True)
+    click.echo(f"    {msg}", err=True)
+    warning_count = state.get_warning_counter()
+    if warning_count > 0:
+        click.secho(
+            f"    {warning_count} warnings shown during change detection, see above",
+            fg="yellow",
+            err=True,
+        )
+    confirm_msg = "    Press enter to execute..."
+    click.echo(confirm_msg, err=True, nl=False)
+    v = input()
+    if v:
+        click.echo(f"    Unexpected user input: {v}", err=True)
+        return False
+    # Go up, clear the line, go up again - as if the confirmation statement was never here!
+    click.echo(
+        "\033[1A{0}\033[1A".format("".join(" " for _ in range(len(confirm_msg)))),
+        err=True,
+        nl=False,
+    )
+    click.echo(err=True)
+    return True
+
+
 # Setup
 #
-def _setup_log_level(debug, quiet):
+def _setup_log_level(debug, debug_all):
     if not debug and not sys.warnoptions:
         warnings.simplefilter("ignore")
 
     log_level = logging.INFO
-    if debug:
+    if debug or debug_all:
         log_level = logging.DEBUG
-    elif quiet:
-        log_level = logging.WARNING
 
-    setup_logging(log_level)
+    other_log_level = None
+    if debug_all:
+        other_log_level = logging.DEBUG
 
+    setup_logging(log_level, other_log_level)
 
-def _validate_operations(operations, chdir):
 
+def _validate_operations(operations, chdir):
     # Make a copy before we overwrite
     original_operations = operations
 
     # Debug (print) inventory + group data
     if operations[0] == "debug-inventory":
         command = CliCommands.DEBUG_INVENTORY
 
@@ -463,57 +502,58 @@
                 operations,
             ),
         )
 
     return original_operations, operations, command, chdir
 
 
-def _set_verbosity(state, verbosity, quiet):
+def _set_verbosity(state, verbosity):
     if verbosity > 0:
         state.print_fact_info = True
         state.print_noop_info = True
 
     if verbosity > 1:
         state.print_input = state.print_fact_input = True
 
     if verbosity > 2:
         state.print_output = state.print_fact_output = True
 
     return state
 
 
-def _setup_state(verbosity, quiet):
+def _setup_state(verbosity, quiet, yes):
     cwd = getcwd()
     if cwd not in sys.path:  # ensure cwd is present in sys.path
         sys.path.append(cwd)
 
-    state = State()
+    state = State(check_for_changes=not yes)
     state.cwd = cwd
     ctx_state.set(state)
 
-    state = _set_verbosity(state, verbosity, quiet)
+    state = _set_verbosity(state, verbosity)
     return state
 
 
 def _set_config(
     config,
     config_filename,
     sudo,
     sudo_user,
     use_sudo_password,
     su_user,
     parallel,
     shell_executable,
     fail_percent,
-    quiet,
+    yes,
 ):
-    echo_msg("--> Loading config...", quiet)
+    logger.info("--> Loading config...")
 
     # Load up any config.py from the filesystem
-    config_filename = path.join(state.cwd, config_filename)
+    if state.cwd:
+        config_filename = path.join(state.cwd, config_filename)
     if path.exists(config_filename):
         exec_file(config_filename)
 
     # Lock the current config, this allows us to restore this version after
     # executing deploy files that may alter them.
     config.lock_current_state()
 
@@ -544,18 +584,14 @@
 def _set_override_data(
     data,
     ssh_user,
     ssh_key,
     ssh_key_password,
     ssh_port,
     ssh_password,
-    winrm_username,
-    winrm_password,
-    winrm_port,
-    winrm_transport,
 ):
     override_data = {}
 
     for arg in data:
         key, value = arg.split("=", 1)
         override_data[key] = value
 
@@ -563,25 +599,34 @@
 
     for key, value in (
         ("ssh_user", ssh_user),
         ("ssh_key", ssh_key),
         ("ssh_key_password", ssh_key_password),
         ("ssh_port", ssh_port),
         ("ssh_password", ssh_password),
-        ("winrm_username", winrm_username),
-        ("winrm_password", winrm_password),
-        ("winrm_port", winrm_port),
-        ("winrm_transport", winrm_transport),
     ):
         if value:
             override_data[key] = value
 
     return override_data
 
 
+def _set_fail_prompts(state: State, config: Config) -> None:
+    # Set fail percent to zero, meaning we'll raise an exception for any fail,
+    # and we can capture + prompt the user to continue/exit.
+    config.FAIL_PERCENT = 0
+
+    def should_raise_failed_hosts(state: State) -> bool:
+        if state.current_stage == StateStage.Connect:
+            return not _do_confirm("One of more hosts failed to connect, continue?")
+        return not _do_confirm("One of more hosts failed, continue?")
+
+    state.should_raise_failed_hosts = should_raise_failed_hosts
+
+
 def _apply_inventory_limit(inventory, limit):
     initial_limit = None
     if limit:
         all_limit_hosts = []
 
         for limiter in limit:
             try:
@@ -596,35 +641,42 @@
         initial_limit = list(set(all_limit_hosts))
 
     return initial_limit
 
 
 # Operations Execution
 #
-def _handle_commands(state, config, command, original_operations, operations, quiet):
-
+def _handle_commands(state, config, command, original_operations, operations):
     if command is CliCommands.FACT:
-        state, fact_data = _run_fact_operations(state, config, operations, quiet)
+        state, fact_data = _run_fact_operations(state, config, operations)
         print_facts(fact_data)
         _exit()
 
+    can_diff = True
+
     if command == CliCommands.SHELL:
-        state = _run_exec_operations(state, config, operations, quiet)
+        state = _prepare_exec_operations(state, config, operations)
+        can_diff = False
 
     elif command == CliCommands.DEPLOY_FILES:
-        state, config, operations = _run_deploy_operations(state, config, operations, quiet)
+        state, config, operations = _prepare_deploy_operations(state, config, operations)
 
     elif command == CliCommands.FUNC:
-        state, kwargs = _run_func_operations(state, config, operations, original_operations, quiet)
+        state, kwargs = _prepare_func_operations(
+            state,
+            config,
+            operations,
+            original_operations,
+        )
 
-    return state, config
+    return can_diff, state, config
 
 
-def _run_fact_operations(state, config, operations, quiet):
-    echo_msg("--> Gathering facts...", quiet)
+def _run_fact_operations(state, config, operations):
+    logger.info("--> Gathering facts...")
 
     state.print_fact_info = True
     fact_data = {}
 
     for i, command in enumerate(operations):
         fact_cls, args, kwargs = command
         fact_key = fact_cls.name
@@ -644,26 +696,26 @@
             )
         except PyinfraError:
             pass
 
     return state, fact_data
 
 
-def _run_exec_operations(state, config, operations, quiet):
+def _prepare_exec_operations(state, config, operations):
     state.print_output = True
     load_func(
         state,
         server.shell,
         " ".join(operations),
     )
     return state
 
 
-def _run_deploy_operations(state, config, operations, quiet):
-    echo_msg("--> Preparing Operations...", quiet)
+def _prepare_deploy_operations(state, config, operations):
+    logger.info("--> Preparing Operations...")
 
     # Number of "steps" to make = number of files * number of hosts
     for i, filename in enumerate(operations):
         _log_styled_msg = click.style(filename, bold=True)
         logger.info("Loading: {0}".format(_log_styled_msg))
 
         state.current_op_file_number = i
@@ -671,25 +723,16 @@
 
         # Remove any config changes introduced by the deploy file & any includes
         config.reset_locked_state()
 
     return state, config, operations
 
 
-def _run_func_operations(state, config, operations, original_operations, quiet):
-    echo_msg("--> Preparing operation...", quiet)
+def _prepare_func_operations(state, config, operations, original_operations):
+    logger.info("--> Preparing operation...")
 
     op, args = operations
     args, kwargs = args
 
     load_func(state, op, *args, **kwargs)
 
     return state, kwargs
-
-
-# Utils
-#
-def echo_msg(msg=None, quiet=None):
-    if not quiet:
-        click.echo(err=True)
-    if msg:
-        click.echo(msg, err=True)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/prints.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/prints.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 import platform
 import re
 import sys
 from typing import TYPE_CHECKING, Callable, Dict, Iterator, List, Tuple, Union
 
 import click
@@ -46,20 +48,14 @@
 
 
 def jsonify(data, *args, **kwargs):
     data = _stringify_host_keys(data)
     return json.dumps(data, *args, **kwargs)
 
 
-def print_state_facts(state: "State"):
-    click.echo(err=True)
-    click.echo("--> Facts:", err=True)
-    click.echo(jsonify(state.facts, indent=4, default=json_encode), err=True)
-
-
 def print_state_operations(state: "State"):
     state_ops = {host: ops for host, ops in state.ops.items() if state.is_host_in_limit(host)}
 
     click.echo(err=True)
     click.echo("--> Operations:", err=True)
     click.echo(jsonify(state_ops, indent=4, default=json_encode), err=True)
     click.echo(err=True)
@@ -72,15 +68,15 @@
     for op_hash in state.get_op_order():
         meta = state.op_meta[op_hash]
         hosts = set(host for host, operations in state.ops.items() if op_hash in operations)
 
         click.echo(
             "    {0} (names={1}, hosts={2})".format(
                 op_hash,
-                meta["names"],
+                meta.names,
                 hosts,
             ),
             err=True,
         )
 
 
 def print_groups_by_comparison(print_items, comparator=lambda item: item[0]):
@@ -157,30 +153,30 @@
         ),
         err=True,
     )
 
 
 def print_rows(rows):
     # Go through the rows and work out all the widths in each column
-    column_widths = []
+    row_column_widths: list[list[int]] = []
 
     for _, columns in rows:
         if isinstance(columns, str):
             continue
 
         for i, column in enumerate(columns):
-            if i >= len(column_widths):
-                column_widths.append([])
+            if i >= len(row_column_widths):
+                row_column_widths.append([])
 
             # Length of the column (with ansi codes removed)
             width = len(_strip_ansi(column.strip()))
-            column_widths[i].append(width)
+            row_column_widths[i].append(width)
 
     # Get the max width of each column and add 4 padding spaces
-    column_widths = [max(widths) + 4 for widths in column_widths]
+    column_widths = [max(widths) + 4 for widths in row_column_widths]
 
     # Now print each column, keeping text justified to the widths above
     for func, columns in rows:
         line = columns
 
         if not isinstance(columns, str):
             justified = []
@@ -198,69 +194,123 @@
                 )
 
             line = "".join(justified)
 
         func(line)
 
 
-def print_meta(state: "State"):
-    group_combinations = _get_group_combinations(state.inventory.iter_activated_hosts())
-    rows: List[Tuple[Callable, Union[List[str], str]]] = []
+def truncate(text, max_length):
+    if len(text) <= max_length:
+        return text
 
-    for i, (groups, hosts) in enumerate(group_combinations.items(), 1):
-        if not hosts:
-            continue
+    text = text[: max_length - 3]
+    return f"{text}..."
 
-        if groups:
-            rows.append(
-                (
-                    logger.info,
-                    "Groups: {0}".format(
-                        click.style(" / ".join(groups), bold=True),
+
+def pretty_op_name(op_meta):
+    name = list(op_meta.names)[0]
+
+    if op_meta.args:
+        name = "{0} ({1})".format(name, ", ".join(str(arg) for arg in op_meta.args))
+
+    return name
+
+
+def print_meta(state: "State"):
+    rows: List[Tuple[Callable, Union[List[str], str]]] = [
+        (logger.info, ["Operation", "Change", "Conditional Change"]),
+    ]
+
+    for op_hash in state.get_op_order():
+        hosts_in_op = []
+        hosts_maybe_in_op = []
+        for host in state.inventory.iter_activated_hosts():
+            if op_hash in state.ops[host]:
+                op_data = state.get_op_data_for_host(host, op_hash)
+                if op_data.operation_meta._maybe_is_change:
+                    if op_data.global_arguments["_if"]:
+                        hosts_maybe_in_op.append(host.name)
+                    else:
+                        hosts_in_op.append(host.name)
+
+        rows.append(
+            (
+                logger.info,
+                [
+                    pretty_op_name(state.op_meta[op_hash]),
+                    "-"
+                    if len(hosts_in_op) == 0
+                    else "{0} ({1})".format(
+                        len(hosts_in_op),
+                        truncate(", ".join(sorted(hosts_in_op)), 48),
                     ),
-                ),
+                    "-"
+                    if len(hosts_maybe_in_op) == 0
+                    else "{0} ({1})".format(
+                        len(hosts_maybe_in_op),
+                        truncate(", ".join(sorted(hosts_maybe_in_op)), 48),
+                    ),
+                ],
             )
-        else:
-            rows.append((logger.info, "Ungrouped:"))
+        )
 
-        for host in hosts:
-            meta = state.meta[host]
+    print_rows(rows)
 
-            # Didn't connect to this host?
-            if host not in state.activated_hosts:
-                rows.append(
-                    (
-                        logger.info,
-                        [
-                            host.style_print_prefix("red", bold=True),
-                            click.style("No connection", "red"),
-                        ],
-                    ),
-                )
+
+def print_results(state: "State"):
+    rows: List[Tuple[Callable, Union[List[str], str]]] = [
+        (logger.info, ["Operation", "Hosts", "Success", "Error", "No Change"]),
+    ]
+
+    for op_hash in state.get_op_order():
+        hosts_in_op = 0
+        hosts_in_op_success: list[str] = []
+        hosts_in_op_error: list[str] = []
+        hosts_in_op_no_attempt: list[str] = []
+        for host in state.inventory.iter_activated_hosts():
+            if op_hash not in state.ops[host]:
                 continue
 
-            rows.append(
-                (
-                    logger.info,
-                    [
-                        host.print_prefix,
-                        "Operations: {0}".format(meta["ops"]),
-                        "Change: {0}".format(meta["ops_change"]),
-                        "No change: {0}".format(meta["ops_no_change"]),
-                    ],
-                ),
-            )
+            hosts_in_op += 1
 
-        if i != len(group_combinations):
-            rows.append((lambda m: click.echo(m, err=True), []))
+            result = state.ops[host][op_hash].operation_meta.did_succeed()
+            if result is True:
+                hosts_in_op_success.append(host.name)
+            elif result is False:
+                hosts_in_op_error.append(host.name)
+            else:
+                hosts_in_op_no_attempt.append(host.name)
+
+        # if not hosts_in_op:
+        #     continue
+
+        row = [
+            pretty_op_name(state.op_meta[op_hash]),
+            str(hosts_in_op),
+        ]
+
+        if hosts_in_op_success:
+            row.append(f"{len(hosts_in_op_success)}")
+        else:
+            row.append("-")
+        if hosts_in_op_error:
+            row.append(f"{len(hosts_in_op_error)}")
+        else:
+            row.append("-")
+        if hosts_in_op_no_attempt:
+            row.append(f"{len(hosts_in_op_no_attempt)}")
+        else:
+            row.append("-")
+
+        rows.append((logger.info, row))
 
     print_rows(rows)
 
 
-def print_results(state: "State"):
+def get_fucked(state: "State"):
     group_combinations = _get_group_combinations(state.inventory.iter_activated_hosts())
     rows: List[Tuple[Callable, Union[List[str], str]]] = []
 
     for i, (groups, hosts) in enumerate(group_combinations.items(), 1):
         if not hosts:
             continue
 
@@ -289,26 +339,26 @@
                     ),
                 )
                 continue
 
             results = state.results[host]
 
             meta = state.meta[host]
-            success_ops = results["success_ops"]
-            partial_ops = results["partial_ops"]
+            success_ops = results.success_ops
+            partial_ops = results.partial_ops
             # TODO: type meta object
-            changed_ops = success_ops - meta["ops_no_change"]  # type: ignore
-            error_ops = results["error_ops"]
-            ignored_error_ops = results["ignored_error_ops"]
+            changed_ops = success_ops - meta.ops_no_change  # type: ignore
+            error_ops = results.error_ops
+            ignored_error_ops = results.ignored_error_ops
 
             host_args = ("green",)
             host_kwargs = {}
 
             # If all ops got complete
-            if results["ops"] == meta["ops"]:
+            if results.ops == meta.ops:
                 # We had some errors - but we ignored them - so "warning" color
                 if error_ops != 0:
                     host_args = ("yellow",)
 
             # Ops did not complete!
             else:
                 host_args = ("red",)
@@ -324,15 +374,15 @@
 
             rows.append(
                 (
                     logger.info,
                     [
                         host.style_print_prefix(*host_args, **host_kwargs),
                         changed_str,
-                        "No change: {0}".format(click.style(f"{meta['ops_no_change']}", bold=True)),
+                        "No change: {0}".format(click.style(f"{meta.ops_no_change}", bold=True)),
                         error_str,
                     ],
                 ),
             )
 
         if i != len(group_combinations):
             rows.append((lambda m: click.echo(m, err=True), []))
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/util.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,42 @@
+from __future__ import annotations
+
 import json
 import os
 from datetime import datetime
 from importlib import import_module
+from importlib.util import find_spec
 from io import IOBase
 from os import path
 from pathlib import Path
-from types import FunctionType, ModuleType
-from typing import TYPE_CHECKING, Callable
+from types import CodeType, FunctionType, ModuleType
+from typing import Callable
 
 import click
 import gevent
 
 from pyinfra import logger, state
 from pyinfra.api.command import PyinfraCommand
 from pyinfra.api.exceptions import PyinfraError
 from pyinfra.api.host import HostData
 from pyinfra.api.operation import OperationMeta
+from pyinfra.api.state import (
+    State,
+    StateHostMeta,
+    StateHostResults,
+    StateOperationHostData,
+    StateOperationMeta,
+)
 from pyinfra.context import ctx_config, ctx_host
 from pyinfra.progress import progress_spinner
 
 from .exceptions import CliError, UnexpectedExternalError
 
-if TYPE_CHECKING:
-    from pyinfra.api.state import State
-
 # Cache for compiled Python deploy code
-PYTHON_CODES = {}
+PYTHON_CODES: dict[str, CodeType] = {}
 
 
 def is_subdir(child, parent):
     child = path.realpath(child)
     parent = path.realpath(parent)
     relative = path.relpath(child, start=parent)
     return not relative.startswith(os.pardir)
@@ -41,45 +48,55 @@
     """
 
     old_current_exec_filename = state.current_exec_filename
     state.current_exec_filename = filename
 
     if filename not in PYTHON_CODES:
         with open(filename, "r", encoding="utf-8") as f:
-            code = f.read()
+            code_str = f.read()
 
-        code = compile(code, filename, "exec")
+        code = compile(code_str, filename, "exec")
         PYTHON_CODES[filename] = code
 
     # Create some base attributes for our "module"
-    data = {
-        "__file__": filename,
-    }
+    data = {"__file__": filename}
 
     # Execute the code with locals/globals going into the dict above
     try:
         exec(PYTHON_CODES[filename], data)
+    except PyinfraError:
+        # Raise pyinfra errors as-is
+        raise
     except Exception as e:
-        if isinstance(e, (PyinfraError, UnexpectedExternalError)):
-            raise
+        # Wrap & re-raise errors in user code so we highlight filename/etc
         raise UnexpectedExternalError(e, filename)
+    finally:
+        state.current_exec_filename = old_current_exec_filename
 
-    state.current_exec_filename = old_current_exec_filename
     return data
 
 
 def json_encode(obj):
     # pyinfra types
     if isinstance(obj, HostData):
         return obj.dict()
 
     if isinstance(obj, PyinfraCommand):
         return repr(obj)
 
-    if isinstance(obj, OperationMeta):
+    if isinstance(
+        obj,
+        (
+            OperationMeta,
+            StateOperationMeta,
+            StateOperationHostData,
+            StateHostMeta,
+            StateHostResults,
+        ),
+    ):
         return repr(obj)
 
     # Python types
     if isinstance(obj, ModuleType):
         return "Module: {0}".format(obj.__name__)
 
     if isinstance(obj, FunctionType):
@@ -129,36 +146,50 @@
         return json.loads(arg)
     except ValueError:
         pass
 
     return arg
 
 
-def try_import_module_attribute(path, prefix=None):
-    mod_path, attr_name = path.rsplit(".", 1)
-    module = None
+def try_import_module_attribute(path, prefix=None, raise_for_none=True):
+    if ":" in path:
+        # Allow a.module.name:function syntax
+        mod_path, attr_name = path.rsplit(":", 1)
+    else:
+        # And also a.module.name.function
+        mod_path, attr_name = path.rsplit(".", 1)
 
+    possible_modules = [mod_path]
     if prefix:
-        full_path = f"{prefix}.{mod_path}"
+        possible_modules.append(f"{prefix}.{mod_path}")
+
+    module = None
+
+    for possible in possible_modules:
         try:
-            module = import_module(full_path)
-        except (ModuleNotFoundError, ImportError):
-            pass
-    else:
-        full_path = mod_path
+            # First use find_spec which checks if the possible module exists *without* importing
+            # it, thus any import errors it contains still get properly raised to the user.
+            spec = find_spec(possible)
+        except ModuleNotFoundError:
+            continue
+        else:
+            if spec is not None:
+                module = import_module(possible)
+                break
 
     if module is None:
-        try:
-            module = import_module(mod_path)
-        except (ModuleNotFoundError, ImportError):
-            raise CliError(f"No such module: {full_path}")
+        if raise_for_none:
+            raise CliError(f"No such module: {possible_modules[-1]}")
+        return
 
     attr = getattr(module, attr_name, None)
     if attr is None:
-        raise CliError(f"No such attribute in module {full_path}: {attr_name}")
+        if raise_for_none:
+            raise CliError(f"No such attribute in module {possible_modules[-1]}: {attr_name}")
+        return
 
     return attr
 
 
 def _parallel_load_hosts(state: "State", callback: Callable, name: str):
     def load_file(local_host):
         try:
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_cli/virtualenv.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_cli/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_forked_by_stone_w4tch3r.egg-info/PKG-INFO` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_forked_by_stone_w4tch3r.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 696e  : 2.1.Name: pyin
-00000020: 6672 612d 666f 726b 6564 2d62 792d 7374  fra-forked-by-st
+00000020: 6672 615f 666f 726b 6564 5f62 795f 7374  fra_forked_by_st
 00000030: 6f6e 652d 7734 7463 6833 720a 5665 7273  one-w4tch3r.Vers
-00000040: 696f 6e3a 2030 2e31 2e31 0a53 756d 6d61  ion: 0.1.1.Summa
+00000040: 696f 6e3a 2030 2e33 2e30 0a53 756d 6d61  ion: 0.3.0.Summa
 00000050: 7279 3a20 4375 7374 6f6d 2076 6572 7369  ry: Custom versi
 00000060: 6f6e 2066 6f72 2064 6576 656c 6f70 696e  on for developin
 00000070: 6720 7079 696e 6672 610a 486f 6d65 2d70  g pyinfra.Home-p
 00000080: 6167 653a 2068 7474 7073 3a2f 2f70 7969  age: https://pyi
 00000090: 6e66 7261 2e63 6f6d 0a41 7574 686f 723a  nfra.com.Author:
 000000a0: 2073 746f 6e65 2d77 3474 6368 3372 0a41   stone-w4tch3r.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2031 3030  uthor-email: 100
@@ -44,483 +44,462 @@
 000002b0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
 000002c0: 6e64 6570 656e 6465 6e74 0a43 6c61 7373  ndependent.Class
 000002d0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
 000002e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 000002f0: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
 00000300: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
 00000310: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000320: 7974 686f 6e20 3a3a 2033 2e36 0a43 6c61  ython :: 3.6.Cla
+00000320: 7974 686f 6e20 3a3a 2033 2e37 0a43 6c61  ython :: 3.7.Cla
 00000330: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
 00000340: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000350: 2050 7974 686f 6e20 3a3a 2033 2e37 0a43   Python :: 3.7.C
+00000350: 2050 7974 686f 6e20 3a3a 2033 2e38 0a43   Python :: 3.8.C
 00000360: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
 00000370: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000380: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+00000380: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
 00000390: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
 000003a0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 000003b0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000003c0: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
-000003d0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000003e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000003f0: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
-00000400: 3a20 546f 7069 6320 3a3a 2053 7973 7465  : Topic :: Syste
-00000410: 6d20 3a3a 2053 7973 7465 6d73 2041 646d  m :: Systems Adm
-00000420: 696e 6973 7472 6174 696f 6e0a 436c 6173  inistration.Clas
+000003c0: 2e31 300a 436c 6173 7369 6669 6572 3a20  .10.Classifier: 
+000003d0: 546f 7069 6320 3a3a 2053 7973 7465 6d20  Topic :: System 
+000003e0: 3a3a 2053 7973 7465 6d73 2041 646d 696e  :: Systems Admin
+000003f0: 6973 7472 6174 696f 6e0a 436c 6173 7369  istration.Classi
+00000400: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
+00000410: 7973 7465 6d20 3a3a 2049 6e73 7461 6c6c  ystem :: Install
+00000420: 6174 696f 6e2f 5365 7475 700a 436c 6173  ation/Setup.Clas
 00000430: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
-00000440: 2053 7973 7465 6d20 3a3a 2049 6e73 7461   System :: Insta
-00000450: 6c6c 6174 696f 6e2f 5365 7475 700a 436c  llation/Setup.Cl
-00000460: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00000470: 3a3a 2055 7469 6c69 7469 6573 0a44 6573  :: Utilities.Des
-00000480: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-00000490: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-000004a0: 646f 776e 0a4c 6963 656e 7365 2d46 696c  down.License-Fil
-000004b0: 653a 204c 4943 454e 5345 2e6d 640a 5265  e: LICENSE.md.Re
-000004c0: 7175 6972 6573 2d44 6973 743a 2067 6576  quires-Dist: gev
-000004d0: 656e 743e 3d31 2e35 0a52 6571 7569 7265  ent>=1.5.Require
-000004e0: 732d 4469 7374 3a20 7061 7261 6d69 6b6f  s-Dist: paramiko
-000004f0: 3c34 2c3e 3d32 2e37 0a52 6571 7569 7265  <4,>=2.7.Require
-00000500: 732d 4469 7374 3a20 636c 6963 6b3e 320a  s-Dist: click>2.
-00000510: 5265 7175 6972 6573 2d44 6973 743a 206a  Requires-Dist: j
-00000520: 696e 6a61 323c 342c 3e32 0a52 6571 7569  inja2<4,>2.Requi
-00000530: 7265 732d 4469 7374 3a20 7079 7468 6f6e  res-Dist: python
-00000540: 2d64 6174 6575 7469 6c3c 332c 3e32 0a52  -dateutil<3,>2.R
-00000550: 6571 7569 7265 732d 4469 7374 3a20 7365  equires-Dist: se
-00000560: 7475 7074 6f6f 6c73 0a52 6571 7569 7265  tuptools.Require
-00000570: 732d 4469 7374 3a20 636f 6e66 6967 7061  s-Dist: configpa
-00000580: 7273 6572 0a52 6571 7569 7265 732d 4469  rser.Requires-Di
-00000590: 7374 3a20 7079 7769 6e72 6d0a 5265 7175  st: pywinrm.Requ
-000005a0: 6972 6573 2d44 6973 743a 2064 6973 7472  ires-Dist: distr
-000005b0: 6f3c 322c 3e3d 312e 360a 5265 7175 6972  o<2,>=1.6.Requir
-000005c0: 6573 2d44 6973 743a 2067 7261 7068 6c69  es-Dist: graphli
-000005d0: 625f 6261 636b 706f 7274 3b20 7079 7468  b_backport; pyth
-000005e0: 6f6e 5f76 6572 7369 6f6e 203c 2022 332e  on_version < "3.
-000005f0: 3922 0a50 726f 7669 6465 732d 4578 7472  9".Provides-Extr
-00000600: 613a 2074 6573 740a 5265 7175 6972 6573  a: test.Requires
-00000610: 2d44 6973 743a 2070 7979 616d 6c3b 2065  -Dist: pyyaml; e
-00000620: 7874 7261 203d 3d20 2274 6573 7422 0a52  xtra == "test".R
-00000630: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
-00000640: 7465 7374 3d3d 372e 302e 313b 2070 7974  test==7.0.1; pyt
-00000650: 686f 6e5f 7665 7273 696f 6e20 3c3d 2022  hon_version <= "
-00000660: 332e 3622 2061 6e64 2065 7874 7261 203d  3.6" and extra =
-00000670: 3d20 2274 6573 7422 0a52 6571 7569 7265  = "test".Require
-00000680: 732d 4469 7374 3a20 636f 7665 7261 6765  s-Dist: coverage
-00000690: 3d3d 362e 323b 2070 7974 686f 6e5f 7665  ==6.2; python_ve
-000006a0: 7273 696f 6e20 3c3d 2022 332e 3622 2061  rsion <= "3.6" a
-000006b0: 6e64 2065 7874 7261 203d 3d20 2274 6573  nd extra == "tes
-000006c0: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
-000006d0: 3a20 7079 7465 7374 3d3d 372e 322e 303b  : pytest==7.2.0;
-000006e0: 2070 7974 686f 6e5f 7665 7273 696f 6e20   python_version 
-000006f0: 3e20 2233 2e36 2220 616e 6420 6578 7472  > "3.6" and extr
-00000700: 6120 3d3d 2022 7465 7374 220a 5265 7175  a == "test".Requ
-00000710: 6972 6573 2d44 6973 743a 2063 6f76 6572  ires-Dist: cover
-00000720: 6167 653d 3d36 2e35 3b20 7079 7468 6f6e  age==6.5; python
-00000730: 5f76 6572 7369 6f6e 203e 2022 332e 3622  _version > "3.6"
-00000740: 2061 6e64 2065 7874 7261 203d 3d20 2274   and extra == "t
-00000750: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
-00000760: 7374 3a20 7079 7465 7374 2d63 6f76 3d3d  st: pytest-cov==
-00000770: 342e 302e 303b 2065 7874 7261 203d 3d20  4.0.0; extra == 
-00000780: 2274 6573 7422 0a52 6571 7569 7265 732d  "test".Requires-
-00000790: 4469 7374 3a20 626c 6163 6b3d 3d32 322e  Dist: black==22.
-000007a0: 332e 303b 2065 7874 7261 203d 3d20 2274  3.0; extra == "t
-000007b0: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
-000007c0: 7374 3a20 6973 6f72 743d 3d35 2e31 302e  st: isort==5.10.
-000007d0: 313b 2065 7874 7261 203d 3d20 2274 6573  1; extra == "tes
-000007e0: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
-000007f0: 3a20 666c 616b 6538 3d3d 342e 302e 313b  : flake8==4.0.1;
-00000800: 2065 7874 7261 203d 3d20 2274 6573 7422   extra == "test"
-00000810: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000820: 666c 616b 6538 2d62 6c61 636b 3d3d 302e  flake8-black==0.
-00000830: 332e 303b 2065 7874 7261 203d 3d20 2274  3.0; extra == "t
-00000840: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
-00000850: 7374 3a20 666c 616b 6538 2d69 736f 7274  st: flake8-isort
-00000860: 3d3d 342e 312e 313b 2065 7874 7261 203d  ==4.1.1; extra =
-00000870: 3d20 2274 6573 7422 0a52 6571 7569 7265  = "test".Require
-00000880: 732d 4469 7374 3a20 6d79 7079 3d3d 302e  s-Dist: mypy==0.
-00000890: 3937 313b 2065 7874 7261 203d 3d20 2274  971; extra == "t
-000008a0: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
-000008b0: 7374 3a20 7479 7065 732d 6372 7970 746f  st: types-crypto
-000008c0: 6772 6170 6879 3b20 6578 7472 6120 3d3d  graphy; extra ==
-000008d0: 2022 7465 7374 220a 5265 7175 6972 6573   "test".Requires
-000008e0: 2d44 6973 743a 2074 7970 6573 2d70 6172  -Dist: types-par
-000008f0: 616d 696b 6f3b 2065 7874 7261 203d 3d20  amiko; extra == 
-00000900: 2274 6573 7422 0a52 6571 7569 7265 732d  "test".Requires-
-00000910: 4469 7374 3a20 7479 7065 732d 7079 7468  Dist: types-pyth
-00000920: 6f6e 2d64 6174 6575 7469 6c3b 2065 7874  on-dateutil; ext
-00000930: 7261 203d 3d20 2274 6573 7422 0a52 6571  ra == "test".Req
-00000940: 7569 7265 732d 4469 7374 3a20 7479 7065  uires-Dist: type
-00000950: 732d 5079 5941 4d4c 3b20 6578 7472 6120  s-PyYAML; extra 
-00000960: 3d3d 2022 7465 7374 220a 5265 7175 6972  == "test".Requir
-00000970: 6573 2d44 6973 743a 2074 7970 6573 2d73  es-Dist: types-s
-00000980: 6574 7570 746f 6f6c 733b 2065 7874 7261  etuptools; extra
-00000990: 203d 3d20 2274 6573 7422 0a50 726f 7669   == "test".Provi
-000009a0: 6465 732d 4578 7472 613a 2064 6f63 730a  des-Extra: docs.
-000009b0: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-000009c0: 7969 6e66 7261 2d67 757a 7a6c 655f 7370  yinfra-guzzle_sp
-000009d0: 6869 6e78 5f74 6865 6d65 3d3d 302e 3134  hinx_theme==0.14
-000009e0: 3b20 6578 7472 6120 3d3d 2022 646f 6373  ; extra == "docs
-000009f0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000a00: 2072 6563 6f6d 6d6f 6e6d 6172 6b3d 3d30   recommonmark==0
-00000a10: 2e35 2e30 3b20 6578 7472 6120 3d3d 2022  .5.0; extra == "
-00000a20: 646f 6373 220a 5265 7175 6972 6573 2d44  docs".Requires-D
-00000a30: 6973 743a 2073 7068 696e 783d 3d32 2e32  ist: sphinx==2.2
-00000a40: 2e31 3b20 6578 7472 6120 3d3d 2022 646f  .1; extra == "do
-00000a50: 6373 220a 5265 7175 6972 6573 2d44 6973  cs".Requires-Dis
-00000a60: 743a 2064 6f63 7574 696c 733d 3d30 2e31  t: docutils==0.1
-00000a70: 372e 313b 2065 7874 7261 203d 3d20 2264  7.1; extra == "d
-00000a80: 6f63 7322 0a50 726f 7669 6465 732d 4578  ocs".Provides-Ex
-00000a90: 7472 613a 2064 6576 0a52 6571 7569 7265  tra: dev.Require
-00000aa0: 732d 4469 7374 3a20 7079 7961 6d6c 3b20  s-Dist: pyyaml; 
-00000ab0: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
-00000ac0: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
-00000ad0: 7465 7374 3d3d 372e 302e 313b 2070 7974  test==7.0.1; pyt
-00000ae0: 686f 6e5f 7665 7273 696f 6e20 3c3d 2022  hon_version <= "
-00000af0: 332e 3622 2061 6e64 2065 7874 7261 203d  3.6" and extra =
+00000440: 2055 7469 6c69 7469 6573 0a44 6573 6372   Utilities.Descr
+00000450: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
+00000460: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
+00000470: 776e 0a4c 6963 656e 7365 2d46 696c 653a  wn.License-File:
+00000480: 204c 4943 454e 5345 2e6d 640a 5265 7175   LICENSE.md.Requ
+00000490: 6972 6573 2d44 6973 743a 2067 6576 656e  ires-Dist: geven
+000004a0: 743e 3d31 2e35 0a52 6571 7569 7265 732d  t>=1.5.Requires-
+000004b0: 4469 7374 3a20 7061 7261 6d69 6b6f 3c34  Dist: paramiko<4
+000004c0: 2c3e 3d32 2e37 0a52 6571 7569 7265 732d  ,>=2.7.Requires-
+000004d0: 4469 7374 3a20 636c 6963 6b3e 320a 5265  Dist: click>2.Re
+000004e0: 7175 6972 6573 2d44 6973 743a 206a 696e  quires-Dist: jin
+000004f0: 6a61 323c 342c 3e32 0a52 6571 7569 7265  ja2<4,>2.Require
+00000500: 732d 4469 7374 3a20 7079 7468 6f6e 2d64  s-Dist: python-d
+00000510: 6174 6575 7469 6c3c 332c 3e32 0a52 6571  ateutil<3,>2.Req
+00000520: 7569 7265 732d 4469 7374 3a20 7365 7475  uires-Dist: setu
+00000530: 7074 6f6f 6c73 0a52 6571 7569 7265 732d  ptools.Requires-
+00000540: 4469 7374 3a20 636f 6e66 6967 7061 7273  Dist: configpars
+00000550: 6572 0a52 6571 7569 7265 732d 4469 7374  er.Requires-Dist
+00000560: 3a20 7079 7769 6e72 6d0a 5265 7175 6972  : pywinrm.Requir
+00000570: 6573 2d44 6973 743a 2074 7970 6567 7561  es-Dist: typegua
+00000580: 7264 0a52 6571 7569 7265 732d 4469 7374  rd.Requires-Dist
+00000590: 3a20 6469 7374 726f 3c32 2c3e 3d31 2e36  : distro<2,>=1.6
+000005a0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000005b0: 6772 6170 686c 6962 5f62 6163 6b70 6f72  graphlib_backpor
+000005c0: 743b 2070 7974 686f 6e5f 7665 7273 696f  t; python_versio
+000005d0: 6e20 3c20 2233 2e39 220a 5265 7175 6972  n < "3.9".Requir
+000005e0: 6573 2d44 6973 743a 2074 7970 696e 672d  es-Dist: typing-
+000005f0: 6578 7465 6e73 696f 6e73 3b20 7079 7468  extensions; pyth
+00000600: 6f6e 5f76 6572 7369 6f6e 203c 2022 332e  on_version < "3.
+00000610: 3131 220a 5072 6f76 6964 6573 2d45 7874  11".Provides-Ext
+00000620: 7261 3a20 7465 7374 0a52 6571 7569 7265  ra: test.Require
+00000630: 732d 4469 7374 3a20 7079 7465 7374 3d3d  s-Dist: pytest==
+00000640: 372e 322e 303b 2065 7874 7261 203d 3d20  7.2.0; extra == 
+00000650: 2274 6573 7422 0a52 6571 7569 7265 732d  "test".Requires-
+00000660: 4469 7374 3a20 636f 7665 7261 6765 3d3d  Dist: coverage==
+00000670: 362e 353b 2065 7874 7261 203d 3d20 2274  6.5; extra == "t
+00000680: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
+00000690: 7374 3a20 7079 7465 7374 2d63 6f76 3d3d  st: pytest-cov==
+000006a0: 342e 302e 303b 2065 7874 7261 203d 3d20  4.0.0; extra == 
+000006b0: 2274 6573 7422 0a52 6571 7569 7265 732d  "test".Requires-
+000006c0: 4469 7374 3a20 626c 6163 6b3d 3d32 322e  Dist: black==22.
+000006d0: 332e 303b 2065 7874 7261 203d 3d20 2274  3.0; extra == "t
+000006e0: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
+000006f0: 7374 3a20 6973 6f72 743d 3d35 2e31 302e  st: isort==5.10.
+00000700: 313b 2065 7874 7261 203d 3d20 2274 6573  1; extra == "tes
+00000710: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
+00000720: 3a20 666c 616b 6538 3d3d 342e 302e 313b  : flake8==4.0.1;
+00000730: 2065 7874 7261 203d 3d20 2274 6573 7422   extra == "test"
+00000740: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000750: 666c 616b 6538 2d62 6c61 636b 3d3d 302e  flake8-black==0.
+00000760: 332e 303b 2065 7874 7261 203d 3d20 2274  3.0; extra == "t
+00000770: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
+00000780: 7374 3a20 666c 616b 6538 2d69 736f 7274  st: flake8-isort
+00000790: 3d3d 342e 312e 313b 2065 7874 7261 203d  ==4.1.1; extra =
+000007a0: 3d20 2274 6573 7422 0a52 6571 7569 7265  = "test".Require
+000007b0: 732d 4469 7374 3a20 6d79 7079 3b20 6578  s-Dist: mypy; ex
+000007c0: 7472 6120 3d3d 2022 7465 7374 220a 5265  tra == "test".Re
+000007d0: 7175 6972 6573 2d44 6973 743a 2074 7970  quires-Dist: typ
+000007e0: 6573 2d63 7279 7074 6f67 7261 7068 793b  es-cryptography;
+000007f0: 2065 7874 7261 203d 3d20 2274 6573 7422   extra == "test"
+00000800: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000810: 7479 7065 732d 7061 7261 6d69 6b6f 3b20  types-paramiko; 
+00000820: 6578 7472 6120 3d3d 2022 7465 7374 220a  extra == "test".
+00000830: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
+00000840: 7970 6573 2d70 7974 686f 6e2d 6461 7465  ypes-python-date
+00000850: 7574 696c 3b20 6578 7472 6120 3d3d 2022  util; extra == "
+00000860: 7465 7374 220a 5265 7175 6972 6573 2d44  test".Requires-D
+00000870: 6973 743a 2074 7970 6573 2d50 7959 414d  ist: types-PyYAM
+00000880: 4c3b 2065 7874 7261 203d 3d20 2274 6573  L; extra == "tes
+00000890: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
+000008a0: 3a20 7479 7065 732d 7365 7475 7074 6f6f  : types-setuptoo
+000008b0: 6c73 3b20 6578 7472 6120 3d3d 2022 7465  ls; extra == "te
+000008c0: 7374 220a 5072 6f76 6964 6573 2d45 7874  st".Provides-Ext
+000008d0: 7261 3a20 646f 6373 0a52 6571 7569 7265  ra: docs.Require
+000008e0: 732d 4469 7374 3a20 7079 696e 6672 612d  s-Dist: pyinfra-
+000008f0: 6775 7a7a 6c65 5f73 7068 696e 785f 7468  guzzle_sphinx_th
+00000900: 656d 653d 3d30 2e31 353b 2065 7874 7261  eme==0.15; extra
+00000910: 203d 3d20 2264 6f63 7322 0a52 6571 7569   == "docs".Requi
+00000920: 7265 732d 4469 7374 3a20 6d79 7374 2d70  res-Dist: myst-p
+00000930: 6172 7365 723d 3d32 2e30 2e30 3b20 6578  arser==2.0.0; ex
+00000940: 7472 6120 3d3d 2022 646f 6373 220a 5265  tra == "docs".Re
+00000950: 7175 6972 6573 2d44 6973 743a 2073 7068  quires-Dist: sph
+00000960: 696e 783d 3d36 2e32 2e31 3b20 6578 7472  inx==6.2.1; extr
+00000970: 6120 3d3d 2022 646f 6373 220a 5072 6f76  a == "docs".Prov
+00000980: 6964 6573 2d45 7874 7261 3a20 6465 760a  ides-Extra: dev.
+00000990: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+000009a0: 7974 6573 743d 3d37 2e32 2e30 3b20 6578  ytest==7.2.0; ex
+000009b0: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+000009c0: 7569 7265 732d 4469 7374 3a20 636f 7665  uires-Dist: cove
+000009d0: 7261 6765 3d3d 362e 353b 2065 7874 7261  rage==6.5; extra
+000009e0: 203d 3d20 2264 6576 220a 5265 7175 6972   == "dev".Requir
+000009f0: 6573 2d44 6973 743a 2070 7974 6573 742d  es-Dist: pytest-
+00000a00: 636f 763d 3d34 2e30 2e30 3b20 6578 7472  cov==4.0.0; extr
+00000a10: 6120 3d3d 2022 6465 7622 0a52 6571 7569  a == "dev".Requi
+00000a20: 7265 732d 4469 7374 3a20 626c 6163 6b3d  res-Dist: black=
+00000a30: 3d32 322e 332e 303b 2065 7874 7261 203d  =22.3.0; extra =
+00000a40: 3d20 2264 6576 220a 5265 7175 6972 6573  = "dev".Requires
+00000a50: 2d44 6973 743a 2069 736f 7274 3d3d 352e  -Dist: isort==5.
+00000a60: 3130 2e31 3b20 6578 7472 6120 3d3d 2022  10.1; extra == "
+00000a70: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
+00000a80: 7374 3a20 666c 616b 6538 3d3d 342e 302e  st: flake8==4.0.
+00000a90: 313b 2065 7874 7261 203d 3d20 2264 6576  1; extra == "dev
+00000aa0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000ab0: 2066 6c61 6b65 382d 626c 6163 6b3d 3d30   flake8-black==0
+00000ac0: 2e33 2e30 3b20 6578 7472 6120 3d3d 2022  .3.0; extra == "
+00000ad0: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
+00000ae0: 7374 3a20 666c 616b 6538 2d69 736f 7274  st: flake8-isort
+00000af0: 3d3d 342e 312e 313b 2065 7874 7261 203d  ==4.1.1; extra =
 00000b00: 3d20 2264 6576 220a 5265 7175 6972 6573  = "dev".Requires
-00000b10: 2d44 6973 743a 2063 6f76 6572 6167 653d  -Dist: coverage=
-00000b20: 3d36 2e32 3b20 7079 7468 6f6e 5f76 6572  =6.2; python_ver
-00000b30: 7369 6f6e 203c 3d20 2233 2e36 2220 616e  sion <= "3.6" an
-00000b40: 6420 6578 7472 6120 3d3d 2022 6465 7622  d extra == "dev"
-00000b50: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000b60: 7079 7465 7374 3d3d 372e 322e 303b 2070  pytest==7.2.0; p
-00000b70: 7974 686f 6e5f 7665 7273 696f 6e20 3e20  ython_version > 
-00000b80: 2233 2e36 2220 616e 6420 6578 7472 6120  "3.6" and extra 
-00000b90: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
-00000ba0: 732d 4469 7374 3a20 636f 7665 7261 6765  s-Dist: coverage
-00000bb0: 3d3d 362e 353b 2070 7974 686f 6e5f 7665  ==6.5; python_ve
-00000bc0: 7273 696f 6e20 3e20 2233 2e36 2220 616e  rsion > "3.6" an
-00000bd0: 6420 6578 7472 6120 3d3d 2022 6465 7622  d extra == "dev"
-00000be0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000bf0: 7079 7465 7374 2d63 6f76 3d3d 342e 302e  pytest-cov==4.0.
-00000c00: 303b 2065 7874 7261 203d 3d20 2264 6576  0; extra == "dev
-00000c10: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000c20: 2062 6c61 636b 3d3d 3232 2e33 2e30 3b20   black==22.3.0; 
-00000c30: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
-00000c40: 6571 7569 7265 732d 4469 7374 3a20 6973  equires-Dist: is
-00000c50: 6f72 743d 3d35 2e31 302e 313b 2065 7874  ort==5.10.1; ext
-00000c60: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
-00000c70: 6972 6573 2d44 6973 743a 2066 6c61 6b65  ires-Dist: flake
-00000c80: 383d 3d34 2e30 2e31 3b20 6578 7472 6120  8==4.0.1; extra 
-00000c90: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
-00000ca0: 732d 4469 7374 3a20 666c 616b 6538 2d62  s-Dist: flake8-b
-00000cb0: 6c61 636b 3d3d 302e 332e 303b 2065 7874  lack==0.3.0; ext
-00000cc0: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
-00000cd0: 6972 6573 2d44 6973 743a 2066 6c61 6b65  ires-Dist: flake
-00000ce0: 382d 6973 6f72 743d 3d34 2e31 2e31 3b20  8-isort==4.1.1; 
-00000cf0: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
-00000d00: 6571 7569 7265 732d 4469 7374 3a20 6d79  equires-Dist: my
-00000d10: 7079 3d3d 302e 3937 313b 2065 7874 7261  py==0.971; extra
-00000d20: 203d 3d20 2264 6576 220a 5265 7175 6972   == "dev".Requir
-00000d30: 6573 2d44 6973 743a 2074 7970 6573 2d63  es-Dist: types-c
-00000d40: 7279 7074 6f67 7261 7068 793b 2065 7874  ryptography; ext
-00000d50: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
-00000d60: 6972 6573 2d44 6973 743a 2074 7970 6573  ires-Dist: types
-00000d70: 2d70 6172 616d 696b 6f3b 2065 7874 7261  -paramiko; extra
-00000d80: 203d 3d20 2264 6576 220a 5265 7175 6972   == "dev".Requir
-00000d90: 6573 2d44 6973 743a 2074 7970 6573 2d70  es-Dist: types-p
-00000da0: 7974 686f 6e2d 6461 7465 7574 696c 3b20  ython-dateutil; 
-00000db0: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
-00000dc0: 6571 7569 7265 732d 4469 7374 3a20 7479  equires-Dist: ty
-00000dd0: 7065 732d 5079 5941 4d4c 3b20 6578 7472  pes-PyYAML; extr
-00000de0: 6120 3d3d 2022 6465 7622 0a52 6571 7569  a == "dev".Requi
-00000df0: 7265 732d 4469 7374 3a20 7479 7065 732d  res-Dist: types-
-00000e00: 7365 7475 7074 6f6f 6c73 3b20 6578 7472  setuptools; extr
-00000e10: 6120 3d3d 2022 6465 7622 0a52 6571 7569  a == "dev".Requi
-00000e20: 7265 732d 4469 7374 3a20 7079 696e 6672  res-Dist: pyinfr
-00000e30: 612d 6775 7a7a 6c65 5f73 7068 696e 785f  a-guzzle_sphinx_
-00000e40: 7468 656d 653d 3d30 2e31 343b 2065 7874  theme==0.14; ext
-00000e50: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
-00000e60: 6972 6573 2d44 6973 743a 2072 6563 6f6d  ires-Dist: recom
-00000e70: 6d6f 6e6d 6172 6b3d 3d30 2e35 2e30 3b20  monmark==0.5.0; 
-00000e80: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
-00000e90: 6571 7569 7265 732d 4469 7374 3a20 7370  equires-Dist: sp
-00000ea0: 6869 6e78 3d3d 322e 322e 313b 2065 7874  hinx==2.2.1; ext
-00000eb0: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
-00000ec0: 6972 6573 2d44 6973 743a 2064 6f63 7574  ires-Dist: docut
-00000ed0: 696c 733d 3d30 2e31 372e 313b 2065 7874  ils==0.17.1; ext
-00000ee0: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
-00000ef0: 6972 6573 2d44 6973 743a 2077 6865 656c  ires-Dist: wheel
-00000f00: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
-00000f10: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000f20: 7477 696e 653b 2065 7874 7261 203d 3d20  twine; extra == 
-00000f30: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
-00000f40: 6973 743a 2069 7079 7468 6f6e 3b20 6578  ist: ipython; ex
-00000f50: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
-00000f60: 7569 7265 732d 4469 7374 3a20 6970 6462  uires-Dist: ipdb
-00000f70: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
-00000f80: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000f90: 6970 6462 706c 7567 696e 3b20 6578 7472  ipdbplugin; extr
-00000fa0: 6120 3d3d 2022 6465 7622 0a52 6571 7569  a == "dev".Requi
-00000fb0: 7265 732d 4469 7374 3a20 666c 616b 6538  res-Dist: flake8
-00000fc0: 2d73 7065 6c6c 6368 6563 6b3d 3d30 2e31  -spellcheck==0.1
-00000fd0: 322e 313b 2065 7874 7261 203d 3d20 2264  2.1; extra == "d
-00000fe0: 6576 220a 5265 7175 6972 6573 2d44 6973  ev".Requires-Dis
-00000ff0: 743a 2072 6564 6261 726f 6e3b 2065 7874  t: redbaron; ext
-00001000: 7261 203d 3d20 2264 6576 220a 5072 6f76  ra == "dev".Prov
-00001010: 6964 6573 2d45 7874 7261 3a20 616e 7369  ides-Extra: ansi
-00001020: 626c 650a 5265 7175 6972 6573 2d44 6973  ble.Requires-Dis
-00001030: 743a 2070 7979 616d 6c3b 2065 7874 7261  t: pyyaml; extra
-00001040: 203d 3d20 2261 6e73 6962 6c65 220a 0a3c   == "ansible"..<
-00001050: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00001060: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
-00001070: 7474 7073 3a2f 2f70 7969 6e66 7261 2e63  ttps://pyinfra.c
-00001080: 6f6d 223e 0a20 2020 2020 2020 203c 696d  om">.        <im
-00001090: 6720 7372 633d 2268 7474 7073 3a2f 2f70  g src="https://p
-000010a0: 7969 6e66 7261 2e63 6f6d 2f73 7461 7469  yinfra.com/stati
-000010b0: 632f 6c6f 676f 5f72 6561 646d 652e 706e  c/logo_readme.pn
-000010c0: 6722 2061 6c74 3d22 7079 696e 6672 6122  g" alt="pyinfra"
-000010d0: 202f 3e0a 2020 2020 3c2f 613e 0a3c 2f70   />.    </a>.</p
-000010e0: 3e0a 0a3c 7020 616c 6967 6e3d 2263 656e  >..<p align="cen
-000010f0: 7465 7222 3e0a 2020 2020 3c65 6d3e 7079  ter">.    <em>py
-00001100: 696e 6672 6120 6175 746f 6d61 7465 7320  infra automates 
-00001110: 696e 6672 6173 7472 7563 7475 7265 2075  infrastructure u
-00001120: 7369 6e67 2050 7974 686f 6e2e 2049 74e2  sing Python. It.
-00001130: 8099 7320 6661 7374 2061 6e64 2073 6361  ..s fast and sca
-00001140: 6c65 7320 6672 6f6d 206f 6e65 2073 6572  les from one ser
-00001150: 7665 7220 746f 2074 686f 7573 616e 6473  ver to thousands
-00001160: 2e20 4772 6561 7420 666f 7220 6164 2d68  . Great for ad-h
-00001170: 6f63 2063 6f6d 6d61 6e64 2065 7865 6375  oc command execu
-00001180: 7469 6f6e 2c20 7365 7276 6963 6520 6465  tion, service de
-00001190: 706c 6f79 6d65 6e74 2c20 636f 6e66 6967  ployment, config
-000011a0: 7572 6174 696f 6e20 6d61 6e61 6765 6d65  uration manageme
-000011b0: 6e74 2061 6e64 206d 6f72 652e 3c2f 656d  nt and more.</em
-000011c0: 3e0a 3c2f 703e 0a0a 2d2d 2d0a 0a3c 7020  >.</p>..---..<p 
-000011d0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-000011e0: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-000011f0: 7073 3a2f 2f64 6f63 732e 7079 696e 6672  ps://docs.pyinfr
-00001200: 612e 636f 6d22 3e3c 7374 726f 6e67 3e44  a.com"><strong>D
-00001210: 6f63 756d 656e 7461 7469 6f6e 3c2f 7374  ocumentation</st
-00001220: 726f 6e67 3e3c 2f61 3e20 2672 4172 723b  rong></a> &rArr;
-00001230: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-00001240: 7470 733a 2f2f 646f 6373 2e70 7969 6e66  tps://docs.pyinf
-00001250: 7261 2e63 6f6d 2f70 6167 652f 6765 7474  ra.com/page/gett
-00001260: 696e 672d 7374 6172 7465 642e 6874 6d6c  ing-started.html
-00001270: 223e 3c73 7472 6f6e 673e 4765 7474 696e  "><strong>Gettin
-00001280: 6720 5374 6172 7465 643c 2f73 7472 6f6e  g Started</stron
-00001290: 673e 3c2f 613e 2026 6275 6c6c 3b0a 2020  g></a> &bull;.  
-000012a0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-000012b0: 3a2f 2f64 6f63 732e 7079 696e 6672 612e  ://docs.pyinfra.
-000012c0: 636f 6d2f 7061 6765 2f65 7861 6d70 6c65  com/page/example
-000012d0: 732e 6874 6d6c 223e 3c73 7472 6f6e 673e  s.html"><strong>
-000012e0: 4578 616d 706c 6573 3c2f 7374 726f 6e67  Examples</strong
-000012f0: 3e3c 2f61 3e20 2662 756c 6c3b 0a20 2020  ></a> &bull;.   
-00001300: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00001310: 2f2f 646f 6373 2e70 7969 6e66 7261 2e63  //docs.pyinfra.c
-00001320: 6f6d 2f70 6167 652f 7375 7070 6f72 742e  om/page/support.
-00001330: 6874 6d6c 223e 3c73 7472 6f6e 673e 4865  html"><strong>He
-00001340: 6c70 2026 2053 7570 706f 7274 3c2f 7374  lp & Support</st
-00001350: 726f 6e67 3e3c 2f61 3e20 2662 756c 6c3b  rong></a> &bull;
-00001360: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-00001370: 7470 733a 2f2f 646f 6373 2e70 7969 6e66  tps://docs.pyinf
-00001380: 7261 2e63 6f6d 2f70 6167 652f 636f 6e74  ra.com/page/cont
-00001390: 7269 6275 7469 6e67 2e68 746d 6c22 3e3c  ributing.html"><
-000013a0: 7374 726f 6e67 3e43 6f6e 7472 6962 7574  strong>Contribut
-000013b0: 696e 673c 2f73 7472 6f6e 673e 3c2f 613e  ing</strong></a>
-000013c0: 0a3c 2f70 3e0a 0a3c 7020 616c 6967 6e3d  .</p>..<p align=
-000013d0: 2263 656e 7465 7222 3e0a 2020 2020 4368  "center">.    Ch
-000013e0: 6174 2026 7241 7272 3b0a 2020 2020 3c61  at &rArr;.    <a
-000013f0: 2068 7265 663d 2268 7474 7073 3a2f 2f6d   href="https://m
-00001400: 6174 7269 782e 746f 2f23 2f23 7079 696e  atrix.to/#/#pyin
-00001410: 6672 613a 6d61 7472 6978 2e6f 7267 223e  fra:matrix.org">
-00001420: 3c73 7472 6f6e 673e 3c63 6f64 653e 2370  <strong><code>#p
-00001430: 7969 6e66 7261 3c2f 636f 6465 3e20 6f6e  yinfra</code> on
-00001440: 204d 6174 7269 783c 2f73 7472 6f6e 673e   Matrix</strong>
-00001450: 3c2f 613e 0a3c 2f70 3e0a 0a2d 2d2d 0a0a  </a>.</p>..---..
-00001460: 5768 7920 7079 696e 6672 613f 2044 6573  Why pyinfra? Des
-00001470: 6967 6e20 6665 6174 7572 6573 2069 6e63  ign features inc
-00001480: 6c75 6465 3a0a 0a2b 20f0 9f9a 8020 2a2a  lude:..+ .... **
-00001490: 5375 7065 7220 6661 7374 2a2a 2065 7865  Super fast** exe
-000014a0: 6375 7469 6f6e 206f 7665 7220 7468 6f75  cution over thou
-000014b0: 7361 6e64 7320 6f66 2068 6f73 7473 2077  sands of hosts w
-000014c0: 6974 6820 7072 6564 6963 7461 626c 6520  ith predictable 
-000014d0: 7065 7266 6f72 6d61 6e63 652e 0a2b 20f0  performance..+ .
-000014e0: 9f9a a820 2a2a 496e 7374 616e 7420 6465  ... **Instant de
-000014f0: 6275 6767 696e 672a 2a20 7769 7468 2072  bugging** with r
-00001500: 6561 6c74 696d 6520 7374 6469 6e2f 7374  ealtime stdin/st
-00001510: 646f 7574 2f73 7464 6572 7220 6f75 7470  dout/stderr outp
-00001520: 7574 2028 602d 7676 7660 292e 0a2b 20f0  ut (`-vvv`)..+ .
-00001530: 9f94 8420 2a2a 4964 656d 706f 7465 6e74  ... **Idempotent
-00001540: 206f 7065 7261 7469 6f6e 732a 2a20 7468   operations** th
-00001550: 6174 2065 6e61 626c 6520 6469 6666 7320  at enable diffs 
-00001560: 616e 6420 6472 7920 7275 6e73 2062 6566  and dry runs bef
-00001570: 6f72 6520 6d61 6b69 6e67 2063 6861 6e67  ore making chang
-00001580: 6573 2e0a 2b20 f09f 93a6 202a 2a45 7874  es..+ .... **Ext
-00001590: 656e 6461 626c 652a 2a20 7769 7468 2074  endable** with t
-000015a0: 6865 2065 6e74 6972 6520 5079 7468 6f6e  he entire Python
-000015b0: 2070 6163 6b61 6765 2065 636f 7379 7374   package ecosyst
-000015c0: 656d 2e0a 2b20 f09f 92bb 202a 2a41 6765  em..+ .... **Age
-000015d0: 6e74 6c65 7373 2065 7865 6375 7469 6f6e  ntless execution
-000015e0: 2a2a 2061 6761 696e 7374 2061 6e79 7468  ** against anyth
-000015f0: 696e 6720 7769 7468 2073 6865 6c6c 2061  ing with shell a
-00001600: 6363 6573 732e 0a2b 20f0 9f94 8c20 2a2a  ccess..+ .... **
-00001610: 496e 7465 6772 6174 6564 2a2a 2077 6974  Integrated** wit
-00001620: 6820 636f 6e6e 6563 746f 7273 2066 6f72  h connectors for
-00001630: 2044 6f63 6b65 722c 2054 6572 7261 666f   Docker, Terrafo
-00001640: 726d 2c20 5661 6772 616e 7420 616e 6420  rm, Vagrant and 
-00001650: 6d6f 7265 2e0a 0a3c 696d 6720 7769 6474  more...<img widt
-00001660: 683d 2231 3030 2522 2073 7263 3d22 6874  h="100%" src="ht
-00001670: 7470 733a 2f2f 7079 696e 6672 612e 636f  tps://pyinfra.co
-00001680: 6d2f 7374 6174 6963 2f65 7861 6d70 6c65  m/static/example
-00001690: 5f64 6570 6c6f 792e 6769 6622 202f 3e0a  _deploy.gif" />.
-000016a0: 0a23 2320 5175 6963 6b73 7461 7274 0a0a  .## Quickstart..
-000016b0: 496e 7374 616c 6c20 7079 696e 6672 6120  Install pyinfra 
-000016c0: 7769 7468 2060 7069 7060 3a0a 0a60 6060  with `pip`:..```
-000016d0: 0a70 6970 2069 6e73 7461 6c6c 2070 7969  .pip install pyi
-000016e0: 6e66 7261 0a60 6060 0a0a 4e6f 7720 796f  nfra.```..Now yo
-000016f0: 7520 6361 6e20 6578 6563 7574 6520 636f  u can execute co
-00001700: 6d6d 616e 6473 206f 6e20 686f 7374 7320  mmands on hosts 
-00001710: 7669 6120 5353 483a 0a0a 6060 6073 680a  via SSH:..```sh.
-00001720: 7079 696e 6672 6120 6d79 2d73 6572 7665  pyinfra my-serve
-00001730: 722e 6e65 7420 6578 6563 202d 2d20 6563  r.net exec -- ec
-00001740: 686f 2022 6865 6c6c 6f20 776f 726c 6422  ho "hello world"
-00001750: 0a60 6060 0a0a 4f72 2074 6172 6765 7420  .```..Or target 
-00001760: 446f 636b 6572 2063 6f6e 7461 696e 6572  Docker container
-00001770: 732c 2074 6865 206c 6f63 616c 206d 6163  s, the local mac
-00001780: 6869 6e65 2c20 616e 6420 6f74 6865 7220  hine, and other 
-00001790: 5b63 6f6e 6e65 6374 6f72 735d 2868 7474  [connectors](htt
-000017a0: 7073 3a2f 2f64 6f63 732e 7079 696e 6672  ps://docs.pyinfr
-000017b0: 612e 636f 6d2f 7061 6765 2f63 6f6e 6e65  a.com/page/conne
-000017c0: 6374 6f72 732e 6874 6d6c 293a 0a0a 6060  ctors.html):..``
-000017d0: 6073 680a 7079 696e 6672 6120 4064 6f63  `sh.pyinfra @doc
-000017e0: 6b65 722f 7562 756e 7475 2065 7865 6320  ker/ubuntu exec 
-000017f0: 2d2d 2065 6368 6f20 2248 656c 6c6f 2077  -- echo "Hello w
-00001800: 6f72 6c64 220a 7079 696e 6672 6120 406c  orld".pyinfra @l
-00001810: 6f63 616c 2065 7865 6320 2d2d 2065 6368  ocal exec -- ech
-00001820: 6f20 2248 656c 6c6f 2077 6f72 6c64 220a  o "Hello world".
-00001830: 6060 600a 0a41 7320 7765 6c6c 2061 7320  ```..As well as 
-00001840: 6578 6563 7574 696e 6720 636f 6d6d 616e  executing comman
-00001850: 6473 2079 6f75 2063 616e 2064 6566 696e  ds you can defin
-00001860: 6520 7374 6174 6520 7573 696e 6720 5b6f  e state using [o
-00001870: 7065 7261 7469 6f6e 735d 2868 7474 7073  perations](https
-00001880: 3a2f 2f64 6f63 732e 7079 696e 6672 612e  ://docs.pyinfra.
-00001890: 636f 6d2f 7061 6765 2f6f 7065 7261 7469  com/page/operati
-000018a0: 6f6e 732e 6874 6d6c 293a 0a0a 6060 6073  ons.html):..```s
-000018b0: 680a 2320 496e 7374 616c 6c20 6966 746f  h.# Install ifto
-000018c0: 7020 6170 7420 7061 636b 6167 6520 6966  p apt package if
-000018d0: 206e 6f74 2070 7265 7365 6e74 0a70 7969   not present.pyi
-000018e0: 6e66 7261 2040 646f 636b 6572 2f75 6275  nfra @docker/ubu
-000018f0: 6e74 7520 6170 742e 7061 636b 6167 6573  ntu apt.packages
-00001900: 2069 6674 6f70 2075 7064 6174 653d 7472   iftop update=tr
-00001910: 7565 205f 7375 646f 3d74 7275 650a 6060  ue _sudo=true.``
-00001920: 600a 0a57 6869 6368 2063 616e 2074 6865  `..Which can the
-00001930: 6e20 6265 2073 6176 6564 2061 7320 6120  n be saved as a 
-00001940: 5079 7468 6f6e 2066 696c 6520 6c69 6b65  Python file like
-00001950: 2060 6465 706c 6f79 2e70 7960 3a0a 0a0a   `deploy.py`:...
-00001960: 6060 6070 790a 6672 6f6d 2070 7969 6e66  ```py.from pyinf
-00001970: 7261 2e6f 7065 7261 7469 6f6e 7320 696d  ra.operations im
-00001980: 706f 7274 2061 7074 0a0a 6170 742e 7061  port apt..apt.pa
-00001990: 636b 6167 6573 280a 2020 2020 6e61 6d65  ckages(.    name
-000019a0: 3d22 456e 7375 7265 2069 6674 6f70 2069  ="Ensure iftop i
-000019b0: 7320 696e 7374 616c 6c65 6422 2c0a 2020  s installed",.  
-000019c0: 2020 7061 636b 6167 6573 3d5b 2769 6674    packages=['ift
-000019d0: 6f70 275d 2c0a 2020 2020 7570 6461 7465  op'],.    update
-000019e0: 3d54 7275 652c 0a20 2020 205f 7375 646f  =True,.    _sudo
-000019f0: 3d54 7275 652c 0a29 0a60 6060 0a0a 5468  =True,.).```..Th
-00001a00: 6520 686f 7374 7320 6361 6e20 616c 736f  e hosts can also
-00001a10: 2062 6520 7361 7665 6420 696e 2061 2066   be saved in a f
-00001a20: 696c 652c 2066 6f72 2065 7861 6d70 6c65  ile, for example
-00001a30: 2060 696e 7665 6e74 6f72 792e 7079 603a   `inventory.py`:
-00001a40: 0a0a 6060 6070 790a 7461 7267 6574 7320  ..```py.targets 
-00001a50: 3d20 5b22 4064 6f63 6b65 722f 7562 756e  = ["@docker/ubun
-00001a60: 7475 222c 2022 6d79 2d74 6573 742d 7365  tu", "my-test-se
-00001a70: 7276 6572 2e6e 6574 225d 0a60 6060 0a0a  rver.net"].```..
-00001a80: 0a41 6e64 2065 7865 6375 7465 6420 746f  .And executed to
-00001a90: 6765 7468 6572 3a0a 0a60 6060 7368 0a70  gether:..```sh.p
-00001aa0: 7969 6e66 7261 2069 6e76 656e 746f 7279  yinfra inventory
-00001ab0: 2e70 7920 6465 706c 6f79 2e70 790a 6060  .py deploy.py.``
-00001ac0: 600a 0a4e 6f77 2079 6f75 206b 6e6f 7720  `..Now you know 
-00001ad0: 7468 6520 6275 696c 6469 6e67 2062 6c6f  the building blo
-00001ae0: 636b 7320 6f66 2070 7969 6e66 7261 2120  cks of pyinfra! 
-00001af0: 4279 2063 6f6d 6269 6e69 6e67 2069 6e76  By combining inv
-00001b00: 656e 746f 7279 2c20 6f70 6572 6174 696f  entory, operatio
-00001b10: 6e73 2061 6e64 2050 7974 686f 6e20 636f  ns and Python co
-00001b20: 6465 2079 6f75 2063 616e 2064 6570 6c6f  de you can deplo
-00001b30: 7920 616e 7974 6869 6e67 2e0a 0a53 6565  y anything...See
-00001b40: 2074 6865 206d 6f72 6520 6465 7461 696c   the more detail
-00001b50: 6564 205b 6765 7474 696e 6720 7374 6172  ed [getting star
-00001b60: 7465 645d 2868 7474 7073 3a2f 2f64 6f63  ted](https://doc
-00001b70: 732e 7079 696e 6672 612e 636f 6d2f 7061  s.pyinfra.com/pa
-00001b80: 6765 2f67 6574 7469 6e67 2d73 7461 7274  ge/getting-start
-00001b90: 6564 2e68 746d 6c29 206f 7220 5b75 7369  ed.html) or [usi
-00001ba0: 6e67 206f 7065 7261 7469 6f6e 735d 2868  ng operations](h
-00001bb0: 7474 7073 3a2f 2f64 6f63 732e 7079 696e  ttps://docs.pyin
-00001bc0: 6672 612e 636f 6d2f 7061 6765 2f75 7369  fra.com/page/usi
-00001bd0: 6e67 2d6f 7065 7261 7469 6f6e 732e 6874  ng-operations.ht
-00001be0: 6d6c 2920 6775 6964 6573 2e20 5365 6520  ml) guides. See 
-00001bf0: 686f 7720 746f 2075 7365 205b 696e 7665  how to use [inve
-00001c00: 6e74 6f72 7920 2620 6461 7461 5d28 6874  ntory & data](ht
-00001c10: 7470 733a 2f2f 646f 6373 2e70 7969 6e66  tps://docs.pyinf
-00001c20: 7261 2e63 6f6d 2f70 6167 652f 696e 7665  ra.com/page/inve
-00001c30: 6e74 6f72 792d 6461 7461 2e68 746d 6c29  ntory-data.html)
-00001c40: 2c20 5b67 6c6f 6261 6c20 6172 6775 6d65  , [global argume
-00001c50: 6e74 735d 2868 7474 7073 3a2f 2f64 6f63  nts](https://doc
-00001c60: 732e 7079 696e 6672 612e 636f 6d2f 7061  s.pyinfra.com/pa
-00001c70: 6765 2f61 7267 756d 656e 7473 2e68 746d  ge/arguments.htm
-00001c80: 6c29 2061 6e64 205b 7468 6520 434c 495d  l) and [the CLI]
-00001c90: 2868 7474 7073 3a2f 2f64 6f63 732e 7079  (https://docs.py
-00001ca0: 696e 6672 612e 636f 6d2f 7061 6765 2f63  infra.com/page/c
-00001cb0: 6c69 2e68 746d 6c29 206f 7220 6368 6563  li.html) or chec
-00001cc0: 6b20 6f75 7420 7468 6520 5b64 6f63 756d  k out the [docum
-00001cd0: 656e 7465 6420 6578 616d 706c 6573 5d28  ented examples](
-00001ce0: 6874 7470 733a 2f2f 646f 6373 2e70 7969  https://docs.pyi
-00001cf0: 6e66 7261 2e63 6f6d 2f70 6167 652f 6578  nfra.com/page/ex
-00001d00: 616d 706c 6573 2e68 746d 6c29 2e0a 0a2d  amples.html)...-
-00001d10: 2d2d 0a0a 3c70 2061 6c69 676e 3d22 6365  --..<p align="ce
-00001d20: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
-00001d30: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
-00001d40: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
-00001d50: 2f70 7969 6e66 7261 223e 3c69 6d67 2061  /pyinfra"><img a
-00001d60: 6c74 3d22 5079 5049 2076 6572 7369 6f6e  lt="PyPI version
-00001d70: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00001d80: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00001d90: 7069 2f76 2f70 7969 6e66 7261 3f63 6f6c  pi/v/pyinfra?col
-00001da0: 6f72 3d62 6c75 6522 3e3c 2f61 3e0a 2020  or=blue"></a>.  
-00001db0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00001dc0: 3a2f 2f70 6570 792e 7465 6368 2f70 726f  ://pepy.tech/pro
-00001dd0: 6a65 6374 2f70 7969 6e66 7261 223e 3c69  ject/pyinfra"><i
-00001de0: 6d67 2061 6c74 3d22 5079 5069 2064 6f77  mg alt="PyPi dow
-00001df0: 6e6c 6f61 6473 2220 7372 633d 2268 7474  nloads" src="htt
-00001e00: 7073 3a2f 2f70 6570 792e 7465 6368 2f62  ps://pepy.tech/b
-00001e10: 6164 6765 2f70 7969 6e66 7261 223e 3c2f  adge/pyinfra"></
-00001e20: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
-00001e30: 6874 7470 733a 2f2f 646f 6373 2e70 7969  https://docs.pyi
-00001e40: 6e66 7261 2e63 6f6d 223e 3c69 6d67 2061  nfra.com"><img a
-00001e50: 6c74 3d22 446f 6373 2073 7461 7475 7322  lt="Docs status"
-00001e60: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00001e70: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
-00001e80: 6875 622f 6163 7469 6f6e 732f 776f 726b  hub/actions/work
-00001e90: 666c 6f77 2f73 7461 7475 732f 4669 7a7a  flow/status/Fizz
-00001ea0: 6164 6172 2f70 7969 6e66 7261 2f64 6f63  adar/pyinfra/doc
-00001eb0: 732e 796d 6c3f 6272 616e 6368 3d32 2e78  s.yml?branch=2.x
-00001ec0: 223e 3c2f 613e 0a20 2020 203c 6120 6872  "></a>.    <a hr
-00001ed0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00001ee0: 7562 2e63 6f6d 2f46 697a 7a61 6461 722f  ub.com/Fizzadar/
-00001ef0: 7079 696e 6672 612f 6163 7469 6f6e 733f  pyinfra/actions?
-00001f00: 7175 6572 793d 776f 726b 666c 6f77 2533  query=workflow%3
-00001f10: 4125 3232 4578 6563 7574 652b 7465 7374  A%22Execute+test
-00001f20: 7325 3232 223e 3c69 6d67 2061 6c74 3d22  s%22"><img alt="
-00001f30: 4578 6563 7574 6520 7465 7374 7320 7374  Execute tests st
-00001f40: 6174 7573 2220 7372 633d 2268 7474 7073  atus" src="https
-00001f50: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00001f60: 6f2f 6769 7468 7562 2f61 6374 696f 6e73  o/github/actions
-00001f70: 2f77 6f72 6b66 6c6f 772f 7374 6174 7573  /workflow/status
-00001f80: 2f46 697a 7a61 6461 722f 7079 696e 6672  /Fizzadar/pyinfr
-00001f90: 612f 7465 7374 2e79 6d6c 3f62 7261 6e63  a/test.yml?branc
-00001fa0: 683d 322e 7822 3e3c 2f61 3e0a 2020 2020  h=2.x"></a>.    
-00001fb0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001fc0: 2f63 6f64 6563 6f76 2e69 6f2f 6769 7468  /codecov.io/gith
-00001fd0: 7562 2f46 697a 7a61 6461 722f 7079 696e  ub/Fizzadar/pyin
-00001fe0: 6672 6122 3e3c 696d 6720 616c 743d 2243  fra"><img alt="C
-00001ff0: 6f64 6563 6f76 2043 6f76 6572 6167 6522  odecov Coverage"
-00002000: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00002010: 672e 7368 6965 6c64 732e 696f 2f63 6f64  g.shields.io/cod
-00002020: 6563 6f76 2f63 2f67 682f 4669 7a7a 6164  ecov/c/gh/Fizzad
-00002030: 6172 2f70 7969 6e66 7261 223e 3c2f 613e  ar/pyinfra"></a>
-00002040: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-00002050: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002060: 2f46 697a 7a61 6461 722f 7079 696e 6672  /Fizzadar/pyinfr
-00002070: 612f 626c 6f62 2f32 2e78 2f4c 4943 454e  a/blob/2.x/LICEN
-00002080: 5345 2e6d 6422 3e3c 696d 6720 616c 743d  SE.md"><img alt=
-00002090: 224d 4954 204c 6963 656e 7365 6422 2073  "MIT Licensed" s
-000020a0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-000020b0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-000020c0: 6c2f 7079 696e 6672 6122 3e3c 2f61 3e0a  l/pyinfra"></a>.
-000020d0: 3c2f 703e 0a                             </p>.
+00000b10: 2d44 6973 743a 206d 7970 793b 2065 7874  -Dist: mypy; ext
+00000b20: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+00000b30: 6972 6573 2d44 6973 743a 2074 7970 6573  ires-Dist: types
+00000b40: 2d63 7279 7074 6f67 7261 7068 793b 2065  -cryptography; e
+00000b50: 7874 7261 203d 3d20 2264 6576 220a 5265  xtra == "dev".Re
+00000b60: 7175 6972 6573 2d44 6973 743a 2074 7970  quires-Dist: typ
+00000b70: 6573 2d70 6172 616d 696b 6f3b 2065 7874  es-paramiko; ext
+00000b80: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+00000b90: 6972 6573 2d44 6973 743a 2074 7970 6573  ires-Dist: types
+00000ba0: 2d70 7974 686f 6e2d 6461 7465 7574 696c  -python-dateutil
+00000bb0: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
+00000bc0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000bd0: 7479 7065 732d 5079 5941 4d4c 3b20 6578  types-PyYAML; ex
+00000be0: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+00000bf0: 7569 7265 732d 4469 7374 3a20 7479 7065  uires-Dist: type
+00000c00: 732d 7365 7475 7074 6f6f 6c73 3b20 6578  s-setuptools; ex
+00000c10: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+00000c20: 7569 7265 732d 4469 7374 3a20 7079 696e  uires-Dist: pyin
+00000c30: 6672 612d 6775 7a7a 6c65 5f73 7068 696e  fra-guzzle_sphin
+00000c40: 785f 7468 656d 653d 3d30 2e31 353b 2065  x_theme==0.15; e
+00000c50: 7874 7261 203d 3d20 2264 6576 220a 5265  xtra == "dev".Re
+00000c60: 7175 6972 6573 2d44 6973 743a 206d 7973  quires-Dist: mys
+00000c70: 742d 7061 7273 6572 3d3d 322e 302e 303b  t-parser==2.0.0;
+00000c80: 2065 7874 7261 203d 3d20 2264 6576 220a   extra == "dev".
+00000c90: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
+00000ca0: 7068 696e 783d 3d36 2e32 2e31 3b20 6578  phinx==6.2.1; ex
+00000cb0: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+00000cc0: 7569 7265 732d 4469 7374 3a20 7768 6565  uires-Dist: whee
+00000cd0: 6c3b 2065 7874 7261 203d 3d20 2264 6576  l; extra == "dev
+00000ce0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000cf0: 2074 7769 6e65 3b20 6578 7472 6120 3d3d   twine; extra ==
+00000d00: 2022 6465 7622 0a52 6571 7569 7265 732d   "dev".Requires-
+00000d10: 4469 7374 3a20 6970 7974 686f 6e3b 2065  Dist: ipython; e
+00000d20: 7874 7261 203d 3d20 2264 6576 220a 5265  xtra == "dev".Re
+00000d30: 7175 6972 6573 2d44 6973 743a 2069 7064  quires-Dist: ipd
+00000d40: 623b 2065 7874 7261 203d 3d20 2264 6576  b; extra == "dev
+00000d50: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000d60: 2069 7064 6270 6c75 6769 6e3b 2065 7874   ipdbplugin; ext
+00000d70: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+00000d80: 6972 6573 2d44 6973 743a 2066 6c61 6b65  ires-Dist: flake
+00000d90: 382d 7370 656c 6c63 6865 636b 3d3d 302e  8-spellcheck==0.
+00000da0: 3132 2e31 3b20 6578 7472 6120 3d3d 2022  12.1; extra == "
+00000db0: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
+00000dc0: 7374 3a20 7265 6462 6172 6f6e 3b20 6578  st: redbaron; ex
+00000dd0: 7472 6120 3d3d 2022 6465 7622 0a0a 3c70  tra == "dev"..<p
+00000de0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000df0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000e00: 7470 733a 2f2f 7079 696e 6672 612e 636f  tps://pyinfra.co
+00000e10: 6d22 3e0a 2020 2020 2020 2020 3c69 6d67  m">.        <img
+00000e20: 2073 7263 3d22 6874 7470 733a 2f2f 7079   src="https://py
+00000e30: 696e 6672 612e 636f 6d2f 7374 6174 6963  infra.com/static
+00000e40: 2f6c 6f67 6f5f 7265 6164 6d65 2e70 6e67  /logo_readme.png
+00000e50: 2220 616c 743d 2270 7969 6e66 7261 2220  " alt="pyinfra" 
+00000e60: 2f3e 0a20 2020 203c 2f61 3e0a 3c2f 703e  />.    </a>.</p>
+00000e70: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00000e80: 6572 223e 0a20 2020 203c 7374 726f 6e67  er">.    <strong
+00000e90: 3e4e 6f74 653a 2074 6869 7320 6973 2074  >Note: this is t
+00000ea0: 6865 2076 3320 6272 616e 6368 2c20 7768  he v3 branch, wh
+00000eb0: 6963 6820 6973 2063 7572 7265 6e74 6c79  ich is currently
+00000ec0: 2069 6e20 6265 7461 2e20 3c61 2068 7265   in beta. <a hre
+00000ed0: 663d 2268 7474 7073 3a2f 2f64 6f63 732e  f="https://docs.
+00000ee0: 7079 696e 6672 612e 636f 6d2f 656e 2f6e  pyinfra.com/en/n
+00000ef0: 6578 7422 3e53 6565 2074 6865 2064 6f63  ext">See the doc
+00000f00: 7320 666f 7220 7633 3c2f 613e 2e20 4966  s for v3</a>. If
+00000f10: 206e 6565 6465 6420 7468 6520 3c61 2068   needed the <a h
+00000f20: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000f30: 6875 622e 636f 6d2f 7079 696e 6672 612d  hub.com/pyinfra-
+00000f40: 6465 762f 7079 696e 6672 612f 7472 6565  dev/pyinfra/tree
+00000f50: 2f32 2e78 2f22 3e32 2e78 2062 7261 6e63  /2.x/">2.x branc
+00000f60: 6820 6973 2068 6572 653c 2f61 3e2c 2062  h is here</a>, b
+00000f70: 7574 2069 7320 696e 2062 7567 6669 7820  ut is in bugfix 
+00000f80: 6f6e 6c79 206d 6f64 652e 3c2f 7374 726f  only mode.</stro
+00000f90: 6e67 3e0a 3c2f 703e 0a0a 3c70 2061 6c69  ng>.</p>..<p ali
+00000fa0: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
+00000fb0: 203c 656d 3e70 7969 6e66 7261 2061 7574   <em>pyinfra aut
+00000fc0: 6f6d 6174 6573 2069 6e66 7261 7374 7275  omates infrastru
+00000fd0: 6374 7572 6520 7573 696e 6720 5079 7468  cture using Pyth
+00000fe0: 6f6e 2e20 4974 e280 9973 2066 6173 7420  on. It...s fast 
+00000ff0: 616e 6420 7363 616c 6573 2066 726f 6d20  and scales from 
+00001000: 6f6e 6520 7365 7276 6572 2074 6f20 7468  one server to th
+00001010: 6f75 7361 6e64 732e 2047 7265 6174 2066  ousands. Great f
+00001020: 6f72 2061 642d 686f 6320 636f 6d6d 616e  or ad-hoc comman
+00001030: 6420 6578 6563 7574 696f 6e2c 2073 6572  d execution, ser
+00001040: 7669 6365 2064 6570 6c6f 796d 656e 742c  vice deployment,
+00001050: 2063 6f6e 6669 6775 7261 7469 6f6e 206d   configuration m
+00001060: 616e 6167 656d 656e 7420 616e 6420 6d6f  anagement and mo
+00001070: 7265 2e3c 2f65 6d3e 0a3c 2f70 3e0a 0a2d  re.</em>.</p>..-
+00001080: 2d2d 0a0a 3c70 2061 6c69 676e 3d22 6365  --..<p align="ce
+00001090: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
+000010a0: 6566 3d22 6874 7470 733a 2f2f 646f 6373  ef="https://docs
+000010b0: 2e70 7969 6e66 7261 2e63 6f6d 223e 3c73  .pyinfra.com"><s
+000010c0: 7472 6f6e 673e 446f 6375 6d65 6e74 6174  trong>Documentat
+000010d0: 696f 6e3c 2f73 7472 6f6e 673e 3c2f 613e  ion</strong></a>
+000010e0: 2026 7241 7272 3b0a 2020 2020 3c61 2068   &rArr;.    <a h
+000010f0: 7265 663d 2268 7474 7073 3a2f 2f64 6f63  ref="https://doc
+00001100: 732e 7079 696e 6672 612e 636f 6d2f 7061  s.pyinfra.com/pa
+00001110: 6765 2f67 6574 7469 6e67 2d73 7461 7274  ge/getting-start
+00001120: 6564 2e68 746d 6c22 3e3c 7374 726f 6e67  ed.html"><strong
+00001130: 3e47 6574 7469 6e67 2053 7461 7274 6564  >Getting Started
+00001140: 3c2f 7374 726f 6e67 3e3c 2f61 3e20 2662  </strong></a> &b
+00001150: 756c 6c3b 0a20 2020 203c 6120 6872 6566  ull;.    <a href
+00001160: 3d22 6874 7470 733a 2f2f 646f 6373 2e70  ="https://docs.p
+00001170: 7969 6e66 7261 2e63 6f6d 2f70 6167 652f  yinfra.com/page/
+00001180: 6578 616d 706c 6573 2e68 746d 6c22 3e3c  examples.html"><
+00001190: 7374 726f 6e67 3e45 7861 6d70 6c65 733c  strong>Examples<
+000011a0: 2f73 7472 6f6e 673e 3c2f 613e 2026 6275  /strong></a> &bu
+000011b0: 6c6c 3b0a 2020 2020 3c61 2068 7265 663d  ll;.    <a href=
+000011c0: 2268 7474 7073 3a2f 2f64 6f63 732e 7079  "https://docs.py
+000011d0: 696e 6672 612e 636f 6d2f 7061 6765 2f73  infra.com/page/s
+000011e0: 7570 706f 7274 2e68 746d 6c22 3e3c 7374  upport.html"><st
+000011f0: 726f 6e67 3e48 656c 7020 2620 5375 7070  rong>Help & Supp
+00001200: 6f72 743c 2f73 7472 6f6e 673e 3c2f 613e  ort</strong></a>
+00001210: 2026 6275 6c6c 3b0a 2020 2020 3c61 2068   &bull;.    <a h
+00001220: 7265 663d 2268 7474 7073 3a2f 2f64 6f63  ref="https://doc
+00001230: 732e 7079 696e 6672 612e 636f 6d2f 7061  s.pyinfra.com/pa
+00001240: 6765 2f63 6f6e 7472 6962 7574 696e 672e  ge/contributing.
+00001250: 6874 6d6c 223e 3c73 7472 6f6e 673e 436f  html"><strong>Co
+00001260: 6e74 7269 6275 7469 6e67 3c2f 7374 726f  ntributing</stro
+00001270: 6e67 3e3c 2f61 3e0a 3c2f 703e 0a0a 3c70  ng></a>.</p>..<p
+00001280: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00001290: 0a20 2020 2043 6861 7420 2672 4172 723b  .    Chat &rArr;
+000012a0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+000012b0: 7470 733a 2f2f 6d61 7472 6978 2e74 6f2f  tps://matrix.to/
+000012c0: 232f 2370 7969 6e66 7261 3a6d 6174 7269  #/#pyinfra:matri
+000012d0: 782e 6f72 6722 3e3c 7374 726f 6e67 3e3c  x.org"><strong><
+000012e0: 636f 6465 3e23 7079 696e 6672 613c 2f63  code>#pyinfra</c
+000012f0: 6f64 653e 206f 6e20 4d61 7472 6978 3c2f  ode> on Matrix</
+00001300: 7374 726f 6e67 3e3c 2f61 3e0a 3c2f 703e  strong></a>.</p>
+00001310: 0a0a 2d2d 2d0a 0a57 6879 2070 7969 6e66  ..---..Why pyinf
+00001320: 7261 3f20 4465 7369 676e 2066 6561 7475  ra? Design featu
+00001330: 7265 7320 696e 636c 7564 653a 0a0a 2b20  res include:..+ 
+00001340: f09f 9a80 202a 2a53 7570 6572 2066 6173  .... **Super fas
+00001350: 742a 2a20 6578 6563 7574 696f 6e20 6f76  t** execution ov
+00001360: 6572 2074 686f 7573 616e 6473 206f 6620  er thousands of 
+00001370: 686f 7374 7320 7769 7468 2070 7265 6469  hosts with predi
+00001380: 6374 6162 6c65 2070 6572 666f 726d 616e  ctable performan
+00001390: 6365 2e0a 2b20 f09f 9aa8 202a 2a49 6e73  ce..+ .... **Ins
+000013a0: 7461 6e74 2064 6562 7567 6769 6e67 2a2a  tant debugging**
+000013b0: 2077 6974 6820 7265 616c 7469 6d65 2073   with realtime s
+000013c0: 7464 696e 2f73 7464 6f75 742f 7374 6465  tdin/stdout/stde
+000013d0: 7272 206f 7574 7075 7420 2860 2d76 7676  rr output (`-vvv
+000013e0: 6029 2e0a 2b20 f09f 9484 202a 2a49 6465  `)..+ .... **Ide
+000013f0: 6d70 6f74 656e 7420 6f70 6572 6174 696f  mpotent operatio
+00001400: 6e73 2a2a 2074 6861 7420 656e 6162 6c65  ns** that enable
+00001410: 2064 6966 6673 2061 6e64 2064 7279 2072   diffs and dry r
+00001420: 756e 7320 6265 666f 7265 206d 616b 696e  uns before makin
+00001430: 6720 6368 616e 6765 732e 0a2b 20f0 9f93  g changes..+ ...
+00001440: a620 2a2a 4578 7465 6e64 6162 6c65 2a2a  . **Extendable**
+00001450: 2077 6974 6820 7468 6520 656e 7469 7265   with the entire
+00001460: 2050 7974 686f 6e20 7061 636b 6167 6520   Python package 
+00001470: 6563 6f73 7973 7465 6d2e 0a2b 20f0 9f92  ecosystem..+ ...
+00001480: bb20 2a2a 4167 656e 746c 6573 7320 6578  . **Agentless ex
+00001490: 6563 7574 696f 6e2a 2a20 6167 6169 6e73  ecution** agains
+000014a0: 7420 616e 7974 6869 6e67 2077 6974 6820  t anything with 
+000014b0: 7368 656c 6c20 6163 6365 7373 2e0a 2b20  shell access..+ 
+000014c0: f09f 948c 202a 2a49 6e74 6567 7261 7465  .... **Integrate
+000014d0: 642a 2a20 7769 7468 2063 6f6e 6e65 6374  d** with connect
+000014e0: 6f72 7320 666f 7220 446f 636b 6572 2c20  ors for Docker, 
+000014f0: 5465 7272 6166 6f72 6d2c 2056 6167 7261  Terraform, Vagra
+00001500: 6e74 2061 6e64 206d 6f72 652e 0a0a 3c69  nt and more...<i
+00001510: 6d67 2077 6964 7468 3d22 3130 3025 2220  mg width="100%" 
+00001520: 7372 633d 2268 7474 7073 3a2f 2f70 7969  src="https://pyi
+00001530: 6e66 7261 2e63 6f6d 2f73 7461 7469 632f  nfra.com/static/
+00001540: 6578 616d 706c 655f 6465 706c 6f79 2e67  example_deploy.g
+00001550: 6966 2220 2f3e 0a0a 2323 2051 7569 636b  if" />..## Quick
+00001560: 7374 6172 740a 0a49 6e73 7461 6c6c 2070  start..Install p
+00001570: 7969 6e66 7261 2077 6974 6820 6070 6970  yinfra with `pip
+00001580: 603a 0a0a 6060 600a 7069 7020 696e 7374  `:..```.pip inst
+00001590: 616c 6c20 7079 696e 6672 610a 6060 600a  all pyinfra.```.
+000015a0: 0a4e 6f77 2079 6f75 2063 616e 2065 7865  .Now you can exe
+000015b0: 6375 7465 2063 6f6d 6d61 6e64 7320 6f6e  cute commands on
+000015c0: 2068 6f73 7473 2076 6961 2053 5348 3a0a   hosts via SSH:.
+000015d0: 0a60 6060 7368 0a70 7969 6e66 7261 206d  .```sh.pyinfra m
+000015e0: 792d 7365 7276 6572 2e6e 6574 2065 7865  y-server.net exe
+000015f0: 6320 2d2d 2065 6368 6f20 2268 656c 6c6f  c -- echo "hello
+00001600: 2077 6f72 6c64 220a 6060 600a 0a4f 7220   world".```..Or 
+00001610: 7461 7267 6574 2044 6f63 6b65 7220 636f  target Docker co
+00001620: 6e74 6169 6e65 7273 2c20 7468 6520 6c6f  ntainers, the lo
+00001630: 6361 6c20 6d61 6368 696e 652c 2061 6e64  cal machine, and
+00001640: 206f 7468 6572 205b 636f 6e6e 6563 746f   other [connecto
+00001650: 7273 5d28 6874 7470 733a 2f2f 646f 6373  rs](https://docs
+00001660: 2e70 7969 6e66 7261 2e63 6f6d 2f70 6167  .pyinfra.com/pag
+00001670: 652f 636f 6e6e 6563 746f 7273 2e68 746d  e/connectors.htm
+00001680: 6c29 3a0a 0a60 6060 7368 0a70 7969 6e66  l):..```sh.pyinf
+00001690: 7261 2040 646f 636b 6572 2f75 6275 6e74  ra @docker/ubunt
+000016a0: 7520 6578 6563 202d 2d20 6563 686f 2022  u exec -- echo "
+000016b0: 4865 6c6c 6f20 776f 726c 6422 0a70 7969  Hello world".pyi
+000016c0: 6e66 7261 2040 6c6f 6361 6c20 6578 6563  nfra @local exec
+000016d0: 202d 2d20 6563 686f 2022 4865 6c6c 6f20   -- echo "Hello 
+000016e0: 776f 726c 6422 0a60 6060 0a0a 4173 2077  world".```..As w
+000016f0: 656c 6c20 6173 2065 7865 6375 7469 6e67  ell as executing
+00001700: 2063 6f6d 6d61 6e64 7320 796f 7520 6361   commands you ca
+00001710: 6e20 6465 6669 6e65 2073 7461 7465 2075  n define state u
+00001720: 7369 6e67 205b 6f70 6572 6174 696f 6e73  sing [operations
+00001730: 5d28 6874 7470 733a 2f2f 646f 6373 2e70  ](https://docs.p
+00001740: 7969 6e66 7261 2e63 6f6d 2f70 6167 652f  yinfra.com/page/
+00001750: 6f70 6572 6174 696f 6e73 2e68 746d 6c29  operations.html)
+00001760: 3a0a 0a60 6060 7368 0a23 2049 6e73 7461  :..```sh.# Insta
+00001770: 6c6c 2069 6674 6f70 2061 7074 2070 6163  ll iftop apt pac
+00001780: 6b61 6765 2069 6620 6e6f 7420 7072 6573  kage if not pres
+00001790: 656e 740a 7079 696e 6672 6120 4064 6f63  ent.pyinfra @doc
+000017a0: 6b65 722f 7562 756e 7475 2061 7074 2e70  ker/ubuntu apt.p
+000017b0: 6163 6b61 6765 7320 6966 746f 7020 7570  ackages iftop up
+000017c0: 6461 7465 3d74 7275 6520 5f73 7564 6f3d  date=true _sudo=
+000017d0: 7472 7565 0a60 6060 0a0a 5768 6963 6820  true.```..Which 
+000017e0: 6361 6e20 7468 656e 2062 6520 7361 7665  can then be save
+000017f0: 6420 6173 2061 2050 7974 686f 6e20 6669  d as a Python fi
+00001800: 6c65 206c 696b 6520 6064 6570 6c6f 792e  le like `deploy.
+00001810: 7079 603a 0a0a 0a60 6060 7079 0a66 726f  py`:...```py.fro
+00001820: 6d20 7079 696e 6672 612e 6f70 6572 6174  m pyinfra.operat
+00001830: 696f 6e73 2069 6d70 6f72 7420 6170 740a  ions import apt.
+00001840: 0a61 7074 2e70 6163 6b61 6765 7328 0a20  .apt.packages(. 
+00001850: 2020 206e 616d 653d 2245 6e73 7572 6520     name="Ensure 
+00001860: 6966 746f 7020 6973 2069 6e73 7461 6c6c  iftop is install
+00001870: 6564 222c 0a20 2020 2070 6163 6b61 6765  ed",.    package
+00001880: 733d 5b27 6966 746f 7027 5d2c 0a20 2020  s=['iftop'],.   
+00001890: 2075 7064 6174 653d 5472 7565 2c0a 2020   update=True,.  
+000018a0: 2020 5f73 7564 6f3d 5472 7565 2c0a 290a    _sudo=True,.).
+000018b0: 6060 600a 0a54 6865 2068 6f73 7473 2063  ```..The hosts c
+000018c0: 616e 2061 6c73 6f20 6265 2073 6176 6564  an also be saved
+000018d0: 2069 6e20 6120 6669 6c65 2c20 666f 7220   in a file, for 
+000018e0: 6578 616d 706c 6520 6069 6e76 656e 746f  example `invento
+000018f0: 7279 2e70 7960 3a0a 0a60 6060 7079 0a74  ry.py`:..```py.t
+00001900: 6172 6765 7473 203d 205b 2240 646f 636b  argets = ["@dock
+00001910: 6572 2f75 6275 6e74 7522 2c20 226d 792d  er/ubuntu", "my-
+00001920: 7465 7374 2d73 6572 7665 722e 6e65 7422  test-server.net"
+00001930: 5d0a 6060 600a 0a0a 416e 6420 6578 6563  ].```...And exec
+00001940: 7574 6564 2074 6f67 6574 6865 723a 0a0a  uted together:..
+00001950: 6060 6073 680a 7079 696e 6672 6120 696e  ```sh.pyinfra in
+00001960: 7665 6e74 6f72 792e 7079 2064 6570 6c6f  ventory.py deplo
+00001970: 792e 7079 0a60 6060 0a0a 4e6f 7720 796f  y.py.```..Now yo
+00001980: 7520 6b6e 6f77 2074 6865 2062 7569 6c64  u know the build
+00001990: 696e 6720 626c 6f63 6b73 206f 6620 7079  ing blocks of py
+000019a0: 696e 6672 6121 2042 7920 636f 6d62 696e  infra! By combin
+000019b0: 696e 6720 696e 7665 6e74 6f72 792c 206f  ing inventory, o
+000019c0: 7065 7261 7469 6f6e 7320 616e 6420 5079  perations and Py
+000019d0: 7468 6f6e 2063 6f64 6520 796f 7520 6361  thon code you ca
+000019e0: 6e20 6465 706c 6f79 2061 6e79 7468 696e  n deploy anythin
+000019f0: 672e 0a0a 5365 6520 7468 6520 6d6f 7265  g...See the more
+00001a00: 2064 6574 6169 6c65 6420 5b67 6574 7469   detailed [getti
+00001a10: 6e67 2073 7461 7274 6564 5d28 6874 7470  ng started](http
+00001a20: 733a 2f2f 646f 6373 2e70 7969 6e66 7261  s://docs.pyinfra
+00001a30: 2e63 6f6d 2f70 6167 652f 6765 7474 696e  .com/page/gettin
+00001a40: 672d 7374 6172 7465 642e 6874 6d6c 2920  g-started.html) 
+00001a50: 6f72 205b 7573 696e 6720 6f70 6572 6174  or [using operat
+00001a60: 696f 6e73 5d28 6874 7470 733a 2f2f 646f  ions](https://do
+00001a70: 6373 2e70 7969 6e66 7261 2e63 6f6d 2f70  cs.pyinfra.com/p
+00001a80: 6167 652f 7573 696e 672d 6f70 6572 6174  age/using-operat
+00001a90: 696f 6e73 2e68 746d 6c29 2067 7569 6465  ions.html) guide
+00001aa0: 732e 2053 6565 2068 6f77 2074 6f20 7573  s. See how to us
+00001ab0: 6520 5b69 6e76 656e 746f 7279 2026 2064  e [inventory & d
+00001ac0: 6174 615d 2868 7474 7073 3a2f 2f64 6f63  ata](https://doc
+00001ad0: 732e 7079 696e 6672 612e 636f 6d2f 7061  s.pyinfra.com/pa
+00001ae0: 6765 2f69 6e76 656e 746f 7279 2d64 6174  ge/inventory-dat
+00001af0: 612e 6874 6d6c 292c 205b 676c 6f62 616c  a.html), [global
+00001b00: 2061 7267 756d 656e 7473 5d28 6874 7470   arguments](http
+00001b10: 733a 2f2f 646f 6373 2e70 7969 6e66 7261  s://docs.pyinfra
+00001b20: 2e63 6f6d 2f70 6167 652f 6172 6775 6d65  .com/page/argume
+00001b30: 6e74 732e 6874 6d6c 2920 616e 6420 5b74  nts.html) and [t
+00001b40: 6865 2043 4c49 5d28 6874 7470 733a 2f2f  he CLI](https://
+00001b50: 646f 6373 2e70 7969 6e66 7261 2e63 6f6d  docs.pyinfra.com
+00001b60: 2f70 6167 652f 636c 692e 6874 6d6c 2920  /page/cli.html) 
+00001b70: 6f72 2063 6865 636b 206f 7574 2074 6865  or check out the
+00001b80: 205b 646f 6375 6d65 6e74 6564 2065 7861   [documented exa
+00001b90: 6d70 6c65 735d 2868 7474 7073 3a2f 2f64  mples](https://d
+00001ba0: 6f63 732e 7079 696e 6672 612e 636f 6d2f  ocs.pyinfra.com/
+00001bb0: 7061 6765 2f65 7861 6d70 6c65 732e 6874  page/examples.ht
+00001bc0: 6d6c 292e 0a0a 2d2d 2d0a 0a3c 7020 616c  ml)...---..<p al
+00001bd0: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00001be0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00001bf0: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+00001c00: 7267 2f70 7970 692f 7079 696e 6672 6122  rg/pypi/pyinfra"
+00001c10: 3e3c 696d 6720 616c 743d 2250 7950 4920  ><img alt="PyPI 
+00001c20: 7665 7273 696f 6e22 2073 7263 3d22 6874  version" src="ht
+00001c30: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00001c40: 732e 696f 2f70 7970 692f 762f 7079 696e  s.io/pypi/v/pyin
+00001c50: 6672 613f 636f 6c6f 723d 626c 7565 223e  fra?color=blue">
+00001c60: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
+00001c70: 3d22 6874 7470 733a 2f2f 7065 7079 2e74  ="https://pepy.t
+00001c80: 6563 682f 7072 6f6a 6563 742f 7079 696e  ech/project/pyin
+00001c90: 6672 6122 3e3c 696d 6720 616c 743d 2250  fra"><img alt="P
+00001ca0: 7950 6920 646f 776e 6c6f 6164 7322 2073  yPi downloads" s
+00001cb0: 7263 3d22 6874 7470 733a 2f2f 7065 7079  rc="https://pepy
+00001cc0: 2e74 6563 682f 6261 6467 652f 7079 696e  .tech/badge/pyin
+00001cd0: 6672 6122 3e3c 2f61 3e0a 2020 2020 3c61  fra"></a>.    <a
+00001ce0: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+00001cf0: 6f63 732e 7079 696e 6672 612e 636f 6d22  ocs.pyinfra.com"
+00001d00: 3e3c 696d 6720 616c 743d 2244 6f63 7320  ><img alt="Docs 
+00001d10: 7374 6174 7573 2220 7372 633d 2268 7474  status" src="htt
+00001d20: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00001d30: 2e69 6f2f 6769 7468 7562 2f61 6374 696f  .io/github/actio
+00001d40: 6e73 2f77 6f72 6b66 6c6f 772f 7374 6174  ns/workflow/stat
+00001d50: 7573 2f46 697a 7a61 6461 722f 7079 696e  us/Fizzadar/pyin
+00001d60: 6672 612f 646f 6373 2e79 6d6c 3f62 7261  fra/docs.yml?bra
+00001d70: 6e63 683d 322e 7822 3e3c 2f61 3e0a 2020  nch=2.x"></a>.  
+00001d80: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00001d90: 3a2f 2f67 6974 6875 622e 636f 6d2f 4669  ://github.com/Fi
+00001da0: 7a7a 6164 6172 2f70 7969 6e66 7261 2f61  zzadar/pyinfra/a
+00001db0: 6374 696f 6e73 3f71 7565 7279 3d77 6f72  ctions?query=wor
+00001dc0: 6b66 6c6f 7725 3341 2532 3245 7865 6375  kflow%3A%22Execu
+00001dd0: 7465 2b74 6573 7473 2532 3222 3e3c 696d  te+tests%22"><im
+00001de0: 6720 616c 743d 2245 7865 6375 7465 2074  g alt="Execute t
+00001df0: 6573 7473 2073 7461 7475 7322 2073 7263  ests status" src
+00001e00: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00001e10: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00001e20: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00001e30: 2f73 7461 7475 732f 4669 7a7a 6164 6172  /status/Fizzadar
+00001e40: 2f70 7969 6e66 7261 2f74 6573 742e 796d  /pyinfra/test.ym
+00001e50: 6c3f 6272 616e 6368 3d32 2e78 223e 3c2f  l?branch=2.x"></
+00001e60: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00001e70: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+00001e80: 696f 2f67 6974 6875 622f 4669 7a7a 6164  io/github/Fizzad
+00001e90: 6172 2f70 7969 6e66 7261 223e 3c69 6d67  ar/pyinfra"><img
+00001ea0: 2061 6c74 3d22 436f 6465 636f 7620 436f   alt="Codecov Co
+00001eb0: 7665 7261 6765 2220 7372 633d 2268 7474  verage" src="htt
+00001ec0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00001ed0: 2e69 6f2f 636f 6465 636f 762f 632f 6768  .io/codecov/c/gh
+00001ee0: 2f46 697a 7a61 6461 722f 7079 696e 6672  /Fizzadar/pyinfr
+00001ef0: 6122 3e3c 2f61 3e0a 2020 2020 3c61 2068  a"></a>.    <a h
+00001f00: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00001f10: 6875 622e 636f 6d2f 4669 7a7a 6164 6172  hub.com/Fizzadar
+00001f20: 2f70 7969 6e66 7261 2f62 6c6f 622f 322e  /pyinfra/blob/2.
+00001f30: 782f 4c49 4345 4e53 452e 6d64 223e 3c69  x/LICENSE.md"><i
+00001f40: 6d67 2061 6c74 3d22 4d49 5420 4c69 6365  mg alt="MIT Lice
+00001f50: 6e73 6564 2220 7372 633d 2268 7474 7073  nsed" src="https
+00001f60: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00001f70: 6f2f 7079 7069 2f6c 2f70 7969 6e66 7261  o/pypi/l/pyinfra
+00001f80: 223e 3c2f 613e 0a3c 2f70 3e0a            "></a>.</p>.
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/pyinfra_forked_by_stone_w4tch3r.egg-info/SOURCES.txt` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/pyinfra_forked_by_stone_w4tch3r.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,40 +10,39 @@
 pyinfra/context.py
 pyinfra/local.py
 pyinfra/progress.py
 pyinfra/py.typed
 pyinfra/version.py
 pyinfra/api/__init__.py
 pyinfra/api/arguments.py
+pyinfra/api/arguments_typed.py
 pyinfra/api/command.py
 pyinfra/api/config.py
 pyinfra/api/connect.py
 pyinfra/api/connectors.py
 pyinfra/api/deploy.py
 pyinfra/api/exceptions.py
 pyinfra/api/facts.py
 pyinfra/api/host.py
 pyinfra/api/inventory.py
 pyinfra/api/operation.py
 pyinfra/api/operations.py
 pyinfra/api/state.py
 pyinfra/api/util.py
 pyinfra/connectors/__init__.py
-pyinfra/connectors/ansible.py
+pyinfra/connectors/base.py
 pyinfra/connectors/chroot.py
 pyinfra/connectors/docker.py
 pyinfra/connectors/dockerssh.py
 pyinfra/connectors/local.py
-pyinfra/connectors/mech.py
 pyinfra/connectors/ssh.py
+pyinfra/connectors/ssh_util.py
 pyinfra/connectors/terraform.py
 pyinfra/connectors/util.py
 pyinfra/connectors/vagrant.py
-pyinfra/connectors/winrm.py
-pyinfra/connectors/pyinfrawinrmsession/__init__.py
 pyinfra/connectors/sshuserclient/__init__.py
 pyinfra/connectors/sshuserclient/client.py
 pyinfra/connectors/sshuserclient/config.py
 pyinfra/facts/__init__.py
 pyinfra/facts/apk.py
 pyinfra/facts/apt.py
 pyinfra/facts/brew.py
@@ -64,25 +63,24 @@
 pyinfra/facts/mysql.py
 pyinfra/facts/npm.py
 pyinfra/facts/openrc.py
 pyinfra/facts/pacman.py
 pyinfra/facts/pip.py
 pyinfra/facts/pkg.py
 pyinfra/facts/pkgin.py
+pyinfra/facts/postgres.py
 pyinfra/facts/postgresql.py
 pyinfra/facts/rpm.py
 pyinfra/facts/selinux.py
 pyinfra/facts/server.py
 pyinfra/facts/snap.py
 pyinfra/facts/systemd.py
 pyinfra/facts/sysvinit.py
 pyinfra/facts/upstart.py
 pyinfra/facts/vzctl.py
-pyinfra/facts/windows.py
-pyinfra/facts/windows_files.py
 pyinfra/facts/xbps.py
 pyinfra/facts/yum.py
 pyinfra/facts/zypper.py
 pyinfra/facts/util/__init__.py
 pyinfra/facts/util/databases.py
 pyinfra/facts/util/packaging.py
 pyinfra/facts/util/win_files.py
@@ -103,27 +101,26 @@
 pyinfra/operations/mysql.py
 pyinfra/operations/npm.py
 pyinfra/operations/openrc.py
 pyinfra/operations/pacman.py
 pyinfra/operations/pip.py
 pyinfra/operations/pkg.py
 pyinfra/operations/pkgin.py
+pyinfra/operations/postgres.py
 pyinfra/operations/postgresql.py
 pyinfra/operations/puppet.py
 pyinfra/operations/python.py
 pyinfra/operations/selinux.py
 pyinfra/operations/server.py
 pyinfra/operations/snap.py
 pyinfra/operations/ssh.py
 pyinfra/operations/systemd.py
 pyinfra/operations/sysvinit.py
 pyinfra/operations/upstart.py
 pyinfra/operations/vzctl.py
-pyinfra/operations/windows.py
-pyinfra/operations/windows_files.py
 pyinfra/operations/xbps.py
 pyinfra/operations/yum.py
 pyinfra/operations/zypper.py
 pyinfra/operations/util/__init__.py
 pyinfra/operations/util/files.py
 pyinfra/operations/util/packaging.py
 pyinfra/operations/util/service.py
@@ -162,19 +159,16 @@
 tests/test_cli/test_cli.py
 tests/test_cli/test_cli_deploy.py
 tests/test_cli/test_cli_exceptions.py
 tests/test_cli/test_cli_util.py
 tests/test_cli/test_context_objects.py
 tests/test_cli/util.py
 tests/test_connectors/__init__.py
-tests/test_connectors/test_ansible.py
 tests/test_connectors/test_chroot.py
 tests/test_connectors/test_docker.py
 tests/test_connectors/test_dockerssh.py
 tests/test_connectors/test_local.py
-tests/test_connectors/test_mech.py
 tests/test_connectors/test_ssh.py
 tests/test_connectors/test_sshuserclient.py
 tests/test_connectors/test_terraform.py
 tests/test_connectors/test_util.py
-tests/test_connectors/test_vagrant.py
-tests/test_connectors/test_winrm.py
+tests/test_connectors/test_vagrant.py
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/setup.cfg` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/setup.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,50 +23,46 @@
     "paramiko>=2.7,<4",  # 2.7 (2019) adds OpenSSH key format + Match SSH config
     "click>2",
     "jinja2>2,<4",
     "python-dateutil>2,<3",
     "setuptools",
     "configparser",
     "pywinrm",
+    "typeguard",
     "distro>=1.6,<2",
     # Backport of graphlib used for DAG operation ordering
     'graphlib_backport ; python_version < "3.9"',
+    # Backport of typing for Unpack (added 3.11)
+    'typing-extensions ; python_version < "3.11"',
 )
 
-ANSIBLE_REQUIRES = ("pyyaml",)  # extras for parsing Ansible inventory
-
-TEST_REQUIRES = ANSIBLE_REQUIRES + (
+TEST_REQUIRES = (
     # Unit testing
-    # TODO: drop Python 3.6 support
-    'pytest==7.0.1 ; python_version <= "3.6"',
-    'coverage==6.2 ; python_version <= "3.6"',
-    'pytest==7.2.0 ; python_version > "3.6"',
-    'coverage==6.5 ; python_version > "3.6"',
+    "pytest==7.2.0",
+    "coverage==6.5",
     "pytest-cov==4.0.0",
     # Formatting & linting
     "black==22.3.0",
     "isort==5.10.1",
     "flake8==4.0.1",
     "flake8-black==0.3.0",
     "flake8-isort==4.1.1",
     # Typing
-    "mypy==0.971",
+    "mypy",
     "types-cryptography",
     "types-paramiko",
     "types-python-dateutil",
     "types-PyYAML",
     "types-setuptools",
 )
 
 DOCS_REQUIRES = (
-    "pyinfra-guzzle_sphinx_theme==0.14",
-    "recommonmark==0.5.0",
-    "sphinx==2.2.1",
-    # Pinned to fix: https://github.com/sphinx-doc/sphinx/issues/9727
-    "docutils==0.17.1",
+    "pyinfra-guzzle_sphinx_theme==0.15",
+    "myst-parser==2.0.0",
+    "sphinx==6.2.1",
 )
 
 DEV_REQUIRES = (
     TEST_REQUIRES
     + DOCS_REQUIRES
     + (
         # Releasing
@@ -115,44 +111,40 @@
             "Documentation": "https://docs.pyinfra.com",
             "GitHub": "https://github.com/stone-w4tch3r/pyinfra_fork",
         },
         packages=find_packages(exclude=["tests", "docs"]),
         entry_points={
             "console_scripts": ("pyinfra=pyinfra_cli.__main__:execute_pyinfra",),
             "pyinfra.connectors": [
-                "ansible = pyinfra.connectors.ansible",
-                "chroot = pyinfra.connectors.chroot",
-                "docker = pyinfra.connectors.docker",
-                "local = pyinfra.connectors.local",
-                "mech = pyinfra.connectors.mech",
-                "ssh = pyinfra.connectors.ssh",
-                "dockerssh = pyinfra.connectors.dockerssh",
-                "vagrant = pyinfra.connectors.vagrant",
-                "winrm = pyinfra.connectors.winrm",
-                "terraform = pyinfra.connectors.terraform",
+                "chroot = pyinfra.connectors.chroot:ChrootConnector",
+                "docker = pyinfra.connectors.docker:DockerConnector",
+                "local = pyinfra.connectors.local:LocalConnector",
+                "ssh = pyinfra.connectors.ssh:SSHConnector",
+                "dockerssh = pyinfra.connectors.dockerssh:DockerSSHConnector",
+                # Inventory only connectors
+                "terraform = pyinfra.connectors.terraform:TerraformInventoryConnector",
+                "vagrant = pyinfra.connectors.vagrant:VagrantInventoryConnector",
             ],
         },
         install_requires=INSTALL_REQUIRES,
         extras_require={
             "test": TEST_REQUIRES,
             "docs": DOCS_REQUIRES,
             "dev": DEV_REQUIRES,
-            "ansible": ANSIBLE_REQUIRES,
         },
         include_package_data=True,
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Environment :: Console",
             "Intended Audience :: Developers",
             "Intended Audience :: System Administrators",
             "Intended Audience :: Information Technology",
             "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent",
             "Programming Language :: Python :: 3",
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Topic :: System :: Systems Administration",
             "Topic :: System :: Installation/Setup",
             "Topic :: Utilities",
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from unittest import TestCase
+from unittest.mock import patch
 
 from paramiko import SSHException
 
 from pyinfra.api import Config, State
 from pyinfra.api.connect import connect_all
 from pyinfra.api.exceptions import NoGroupError, NoHostError, PyinfraError
 
@@ -56,14 +57,15 @@
             inventory.get_host("i-dont-exist")
 
         with self.assertRaises(NoGroupError):
             inventory.get_group("i-dont-exist")
 
 
 class TestStateApi(PatchSSHTestCase):
+    @patch("pyinfra.connectors.base.raise_if_bad_type", lambda *args, **kwargs: None)
     def test_fail_percent(self):
         inventory = make_inventory(
             (
                 "somehost",
                 ("thinghost", {"ssh_hostname": SSHException}),
                 "anotherhost",
             ),
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_command.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_command.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_config.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_config.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_deploys.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_deploys.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,60 +20,56 @@
         state.print_output = True
         state.print_input = True
         state.print_fact_info = True
         state.print_noop_info = True
 
         connect_all(state)
 
-        @deploy
+        @deploy()
         def test_deploy(state=None, host=None):
             server.shell(commands=["echo first command"])
             server.shell(commands=["echo second command"])
 
         add_deploy(state, test_deploy)
 
         op_order = state.get_op_order()
 
         # Ensure we have an op
         assert len(op_order) == 2
 
+        # Ensure run ops works
+        run_ops(state)
+
         first_op_hash = op_order[0]
-        assert state.op_meta[first_op_hash]["names"] == {"test_deploy | Server/Shell"}
-        assert state.ops[somehost][first_op_hash]["commands"] == [
+        assert state.op_meta[first_op_hash].names == {"test_deploy | server.shell"}
+        assert state.ops[somehost][first_op_hash].operation_meta._commands == [
             StringCommand("echo first command"),
         ]
-        assert state.ops[anotherhost][first_op_hash]["commands"] == [
+        assert state.ops[anotherhost][first_op_hash].operation_meta._commands == [
             StringCommand("echo first command"),
         ]
 
         second_op_hash = op_order[1]
-        assert state.op_meta[second_op_hash]["names"] == {"test_deploy | Server/Shell"}
-        assert state.ops[somehost][second_op_hash]["commands"] == [
+        assert state.op_meta[second_op_hash].names == {"test_deploy | server.shell"}
+        assert state.ops[somehost][second_op_hash].operation_meta._commands == [
             StringCommand("echo second command"),
         ]
-        assert state.ops[anotherhost][second_op_hash]["commands"] == [
+        assert state.ops[anotherhost][second_op_hash].operation_meta._commands == [
             StringCommand("echo second command"),
         ]
 
-        # Ensure run ops works
-        run_ops(state)
-
         # Ensure ops completed OK
-        assert state.results[somehost]["success_ops"] == 2
-        assert state.results[somehost]["ops"] == 2
-        assert state.results[anotherhost]["success_ops"] == 2
-        assert state.results[anotherhost]["ops"] == 2
+        assert state.results[somehost].success_ops == 2
+        assert state.results[somehost].ops == 2
+        assert state.results[anotherhost].success_ops == 2
+        assert state.results[anotherhost].ops == 2
 
         # And w/o errors
-        assert state.results[somehost]["error_ops"] == 0
-        assert state.results[anotherhost]["error_ops"] == 0
-
-        # And with the different modes
-        run_ops(state, serial=True)
-        run_ops(state, no_wait=True)
+        assert state.results[somehost].error_ops == 0
+        assert state.results[anotherhost].error_ops == 0
 
         disconnect_all(state)
 
     def test_nested_deploy(self):
         inventory = make_inventory()
         somehost = inventory.get_host("somehost")
 
@@ -83,43 +79,46 @@
         state.print_output = True
         state.print_input = True
         state.print_fact_info = True
         state.print_noop_info = True
 
         connect_all(state)
 
-        @deploy
+        @deploy()
         def test_nested_deploy():
             server.shell(commands=["echo nested command"])
 
-        @deploy
+        @deploy()
         def test_deploy():
             server.shell(commands=["echo first command"])
             test_nested_deploy()
             server.shell(commands=["echo second command"])
 
         add_deploy(state, test_deploy)
 
         op_order = state.get_op_order()
 
         # Ensure we have an op
         assert len(op_order) == 3
 
+        # Ensure run ops works
+        run_ops(state)
+
         first_op_hash = op_order[0]
-        assert state.op_meta[first_op_hash]["names"] == {"test_deploy | Server/Shell"}
-        assert state.ops[somehost][first_op_hash]["commands"] == [
+        assert state.op_meta[first_op_hash].names == {"test_deploy | server.shell"}
+        assert state.ops[somehost][first_op_hash].operation_meta._commands == [
             StringCommand("echo first command"),
         ]
 
         second_op_hash = op_order[1]
-        assert state.op_meta[second_op_hash]["names"] == {
-            "test_deploy | test_nested_deploy | Server/Shell",
+        assert state.op_meta[second_op_hash].names == {
+            "test_deploy | test_nested_deploy | server.shell",
         }
-        assert state.ops[somehost][second_op_hash]["commands"] == [
+        assert state.ops[somehost][second_op_hash].operation_meta._commands == [
             StringCommand("echo nested command"),
         ]
 
         third_op_hash = op_order[2]
-        assert state.op_meta[third_op_hash]["names"] == {"test_deploy | Server/Shell"}
-        assert state.ops[somehost][third_op_hash]["commands"] == [
+        assert state.op_meta[third_op_hash].names == {"test_deploy | server.shell"}
+        assert state.ops[somehost][third_op_hash].operation_meta._commands == [
             StringCommand("echo second command"),
         ]
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_facts.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_facts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,354 +1,316 @@
 from unittest.mock import MagicMock, patch
 
 from pyinfra.api import Config, State
-from pyinfra.api.arguments import get_executor_kwarg_keys, pop_global_arguments
+from pyinfra.api.arguments import CONNECTOR_ARGUMENT_KEYS, pop_global_arguments
 from pyinfra.api.connect import connect_all
 from pyinfra.api.exceptions import PyinfraError
 from pyinfra.api.facts import get_facts
+from pyinfra.connectors.util import CommandOutput, OutputLine
 from pyinfra.facts.server import Arch, Command
 
 from ..paramiko_util import PatchSSHTestCase
 from ..util import make_inventory
 
 
 def _get_executor_defaults(state, host):
     global_argument_defaults, _ = pop_global_arguments({}, state=state, host=host)
     return {
         key: value
         for key, value in global_argument_defaults.items()
-        if key in get_executor_kwarg_keys()
+        if key in CONNECTOR_ARGUMENT_KEYS
     }
 
 
 class TestFactsApi(PatchSSHTestCase):
     def test_get_fact(self):
         inventory = make_inventory(hosts=("anotherhost",))
         state = State(inventory, Config())
 
         anotherhost = inventory.get_host("anotherhost")
 
         connect_all(state)
 
-        with patch("pyinfra.connectors.ssh.run_shell_command") as fake_run_command:
-            fake_run_command.return_value = MagicMock(), [("stdout", "some-output")]
+        with patch("pyinfra.connectors.ssh.SSHConnector.run_shell_command") as fake_run_command:
+            fake_run_command.return_value = True, CommandOutput(
+                [OutputLine("stdout", "some-output")]
+            )
             fact_data = get_facts(state, Command, ("yes",))
 
         assert fact_data == {anotherhost: "some-output"}
 
         fake_run_command.assert_called_with(
-            state,
-            anotherhost,
             "yes",
             print_input=False,
             print_output=False,
-            return_combined_output=True,
             **_get_executor_defaults(state, anotherhost),
         )
 
     def test_get_fact_current_op_global_arguments(self):
         inventory = make_inventory(hosts=("anotherhost",))
         state = State(inventory, Config())
 
         anotherhost = inventory.get_host("anotherhost")
 
         connect_all(state)
-        anotherhost.current_op_global_kwargs = {
-            "sudo": True,
-            "sudo_user": "someuser",
-            "use_sudo_password": True,
-            "su_user": "someuser",
-            "timeout": 10,
-            "env": {"HELLO": "WORLD"},
+        anotherhost.current_op_global_arguments = {
+            "_sudo": True,
+            "_sudo_user": "someuser",
+            "_su_user": "someuser",
+            "_timeout": 10,
+            "_env": {"HELLO": "WORLD"},
         }
 
-        with patch("pyinfra.connectors.ssh.run_shell_command") as fake_run_command:
-            fake_run_command.return_value = MagicMock(), [("stdout", "some-output")]
+        with patch("pyinfra.connectors.ssh.SSHConnector.run_shell_command") as fake_run_command:
+            fake_run_command.return_value = True, CommandOutput(
+                [OutputLine("stdout", "some-output")]
+            )
             fact_data = get_facts(state, Command, ("yes",))
 
         assert fact_data == {anotherhost: "some-output"}
 
         defaults = _get_executor_defaults(state, anotherhost)
-        defaults.update(anotherhost.current_op_global_kwargs)
+        defaults.update(anotherhost.current_op_global_arguments)
 
         fake_run_command.assert_called_with(
-            state,
-            anotherhost,
             "yes",
             print_input=False,
             print_output=False,
-            return_combined_output=True,
             **defaults,
         )
 
     def test_get_fact_error(self):
         inventory = make_inventory(hosts=("anotherhost",))
         state = State(inventory, Config())
 
         anotherhost = inventory.get_host("anotherhost")
 
         connect_all(state)
 
-        with patch("pyinfra.connectors.ssh.run_shell_command") as fake_run_command:
+        with patch("pyinfra.connectors.ssh.SSHConnector.run_shell_command") as fake_run_command:
             fake_run_command.return_value = False, MagicMock()
 
             with self.assertRaises(PyinfraError) as context:
                 get_facts(state, Command, ("fail command",))
 
         assert context.exception.args[0] == "No hosts remaining!"
 
         fake_run_command.assert_called_with(
-            state,
-            anotherhost,
             "fail command",
             print_input=False,
             print_output=False,
-            return_combined_output=True,
             **_get_executor_defaults(state, anotherhost),
         )
 
     def test_get_fact_error_ignore(self):
         inventory = make_inventory(hosts=("anotherhost",))
         state = State(inventory, Config())
 
         anotherhost = inventory.get_host("anotherhost")
 
         connect_all(state)
-        anotherhost.current_op_global_kwargs = {
-            "ignore_errors": True,
+        anotherhost.in_op = True
+        anotherhost.current_op_global_arguments = {
+            "_ignore_errors": True,
         }
 
-        with patch("pyinfra.connectors.ssh.run_shell_command") as fake_run_command:
+        with patch("pyinfra.connectors.ssh.SSHConnector.run_shell_command") as fake_run_command:
             fake_run_command.return_value = False, MagicMock()
             fact_data = get_facts(state, Command, ("fail command",))
 
         assert fact_data == {anotherhost: None}
 
         fake_run_command.assert_called_with(
-            state,
-            anotherhost,
             "fail command",
             print_input=False,
             print_output=False,
-            return_combined_output=True,
             **_get_executor_defaults(state, anotherhost),
         )
 
     def test_get_fact_executor_override_arguments(self):
         inventory = make_inventory(hosts=("anotherhost",))
         state = State(inventory, Config())
 
         anotherhost = inventory.get_host("anotherhost")
 
         connect_all(state)
 
-        with patch("pyinfra.connectors.ssh.run_shell_command") as fake_run_command:
-            fake_run_command.return_value = MagicMock(), [("stdout", "some-output")]
+        with patch("pyinfra.connectors.ssh.SSHConnector.run_shell_command") as fake_run_command:
+            fake_run_command.return_value = MagicMock(), CommandOutput(
+                [OutputLine("stdout", "some-output")]
+            )
             fact_data = get_facts(state, Command, ("yes",), {"_sudo": True})
 
         assert fact_data == {anotherhost: "some-output"}
 
         defaults = _get_executor_defaults(state, anotherhost)
-        defaults["sudo"] = True
+        defaults["_sudo"] = True
 
         fake_run_command.assert_called_with(
-            state,
-            anotherhost,
             "yes",
             print_input=False,
             print_output=False,
-            return_combined_output=True,
             **defaults,
         )
 
     def test_get_fact_executor_host_data_arguments(self):
         inventory = make_inventory(hosts=("anotherhost",))
         state = State(inventory, Config())
 
         anotherhost = inventory.get_host("anotherhost")
         anotherhost.data._sudo = True
 
         connect_all(state)
 
-        with patch("pyinfra.connectors.ssh.run_shell_command") as fake_run_command:
-            fake_run_command.return_value = MagicMock(), [("stdout", "some-output")]
+        with patch("pyinfra.connectors.ssh.SSHConnector.run_shell_command") as fake_run_command:
+            fake_run_command.return_value = True, CommandOutput(
+                [OutputLine("stdout", "some-output")]
+            )
             fact_data = get_facts(state, Command, ("yes",))
 
         assert fact_data == {anotherhost: "some-output"}
 
         defaults = _get_executor_defaults(state, anotherhost)
-        defaults["sudo"] = True
+        defaults["_sudo"] = True
 
         fake_run_command.assert_called_with(
-            state,
-            anotherhost,
             "yes",
             print_input=False,
             print_output=False,
-            return_combined_output=True,
             **defaults,
         )
 
     def test_get_fact_executor_mixed_arguments(self):
         inventory = make_inventory(hosts=("anotherhost",))
         state = State(inventory, Config())
 
         anotherhost = inventory.get_host("anotherhost")
         anotherhost.data._sudo = True
         anotherhost.data._sudo_user = "this-should-be-overridden"
         anotherhost.data._su_user = "this-should-be-overridden"
 
-        anotherhost.current_op_global_kwargs = {
-            "su_user": "override-su-user",
+        anotherhost.current_op_global_arguments = {
+            "_su_user": "override-su-user",
         }
 
         connect_all(state)
 
-        with patch("pyinfra.connectors.ssh.run_shell_command") as fake_run_command:
-            fake_run_command.return_value = MagicMock(), [("stdout", "some-output")]
+        with patch("pyinfra.connectors.ssh.SSHConnector.run_shell_command") as fake_run_command:
+            fake_run_command.return_value = True, CommandOutput(
+                [OutputLine("stdout", "some-output")]
+            )
             fact_data = get_facts(
                 state,
                 Command,
                 args=("yes",),
                 kwargs={"_sudo_user": "override-sudo-user"},
             )
 
         assert fact_data == {anotherhost: "some-output"}
 
         defaults = _get_executor_defaults(state, anotherhost)
-        defaults["sudo"] = True
-        defaults["sudo_user"] = "override-sudo-user"
-        defaults["su_user"] = "override-su-user"
+        defaults["_sudo"] = True
+        defaults["_sudo_user"] = "override-sudo-user"
+        defaults["_su_user"] = "override-su-user"
 
         fake_run_command.assert_called_with(
-            state,
-            anotherhost,
             "yes",
             print_input=False,
             print_output=False,
-            return_combined_output=True,
             **defaults,
         )
 
-    def test_get_fact_cached(self):
-        inventory = make_inventory(hosts=("anotherhost",))
-        state = State(inventory, Config())
-
-        fact_hash = "a-fact-hash"
-        cached_fact = {"this is a cached fact"}
-        anotherhost = inventory.get_host("anotherhost")
-        anotherhost.facts[fact_hash] = cached_fact
-
-        connect_all(state)
-
-        with patch("pyinfra.connectors.ssh.run_shell_command") as fake_run_command:
-            fake_run_command.return_value = MagicMock(), [("stdout", "some-output")]
-            fact_data = get_facts(
-                state,
-                Command,
-                args=("yes",),
-                kwargs={"_sudo": True},
-                fact_hash=fact_hash,
-            )
-
-        assert fact_data == {anotherhost: cached_fact}
-        fake_run_command.assert_not_called()
-
     def test_get_fact_no_args(self):
         inventory = make_inventory(hosts=("host-1",))
         state = State(inventory, Config())
 
         connect_all(state)
 
         host_1 = inventory.get_host("host-1")
         defaults = _get_executor_defaults(state, host_1)
 
-        with patch("pyinfra.connectors.ssh.run_shell_command") as fake_run_command:
-            fake_run_command.return_value = MagicMock(), [("stdout", "some-output")]
+        with patch("pyinfra.connectors.ssh.SSHConnector.run_shell_command") as fake_run_command:
+            fake_run_command.return_value = MagicMock(), CommandOutput(
+                [OutputLine("stdout", "some-output")]
+            )
             fact_data = get_facts(state, Arch)
 
         assert fact_data == {host_1: "some-output"}
         fake_run_command.assert_called_with(
-            state,
-            host_1,
             Arch.command,
             print_input=False,
             print_output=False,
-            return_combined_output=True,
             **defaults,
         )
 
 
 class TestHostFactsApi(PatchSSHTestCase):
     def test_get_host_fact(self):
         inventory = make_inventory(hosts=("host-1",))
         state = State(inventory, Config())
 
         connect_all(state)
 
         host_1 = inventory.get_host("host-1")
         defaults = _get_executor_defaults(state, host_1)
 
-        with patch("pyinfra.connectors.ssh.run_shell_command") as fake_run_command:
-            fake_run_command.return_value = MagicMock(), [("stdout", "some-output")]
+        with patch("pyinfra.connectors.ssh.SSHConnector.run_shell_command") as fake_run_command:
+            fake_run_command.return_value = MagicMock(), CommandOutput(
+                [OutputLine("stdout", "some-output")]
+            )
             fact_data = host_1.get_fact(Command, command="echo hello world")
 
         assert fact_data == "some-output"
         fake_run_command.assert_called_with(
-            state,
-            host_1,
             "echo hello world",
             print_input=False,
             print_output=False,
-            return_combined_output=True,
             **defaults,
         )
 
     def test_get_host_fact_sudo(self):
         inventory = make_inventory(hosts=("host-1",))
         state = State(inventory, Config())
 
         connect_all(state)
 
         host_1 = inventory.get_host("host-1")
         defaults = _get_executor_defaults(state, host_1)
-        defaults["sudo"] = True
+        defaults["_sudo"] = True
 
-        with patch("pyinfra.connectors.ssh.run_shell_command") as fake_run_command:
-            fake_run_command.return_value = MagicMock(), [("stdout", "some-output")]
+        with patch("pyinfra.connectors.ssh.SSHConnector.run_shell_command") as fake_run_command:
+            fake_run_command.return_value = MagicMock(), CommandOutput(
+                [OutputLine("stdout", "some-output")]
+            )
             fact_data = host_1.get_fact(Command, command="echo hello world", _sudo=True)
 
         assert fact_data == "some-output"
         fake_run_command.assert_called_with(
-            state,
-            host_1,
             "echo hello world",
             print_input=False,
             print_output=False,
-            return_combined_output=True,
             **defaults,
         )
 
     def test_get_host_fact_sudo_no_args(self):
         inventory = make_inventory(hosts=("host-1",))
         state = State(inventory, Config())
 
         connect_all(state)
 
         host_1 = inventory.get_host("host-1")
         defaults = _get_executor_defaults(state, host_1)
-        defaults["sudo"] = True
+        defaults["_sudo"] = True
 
-        with patch("pyinfra.connectors.ssh.run_shell_command") as fake_run_command:
-            fake_run_command.return_value = MagicMock(), [("stdout", "some-output")]
+        with patch("pyinfra.connectors.ssh.SSHConnector.run_shell_command") as fake_run_command:
+            fake_run_command.return_value = MagicMock(), CommandOutput(
+                [OutputLine("stdout", "some-output")]
+            )
             fact_data = host_1.get_fact(Arch, _sudo=True)
 
         assert fact_data == "some-output"
         fake_run_command.assert_called_with(
-            state,
-            host_1,
             Arch.command,
             print_input=False,
             print_output=False,
-            return_combined_output=True,
             **defaults,
         )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_host.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_host.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_inventory.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_inventory.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_api/test_api_operations.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_api/test_api_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,29 +14,30 @@
     State,
     StringCommand,
 )
 from pyinfra.api.connect import connect_all, disconnect_all
 from pyinfra.api.exceptions import PyinfraError
 from pyinfra.api.operation import OperationMeta, add_op
 from pyinfra.api.operations import run_ops
+from pyinfra.api.state import StateOperationMeta
 from pyinfra.context import ctx_host, ctx_state
 from pyinfra.operations import files, python, server
 
 from ..paramiko_util import FakeBuffer, FakeChannel, PatchSSHTestCase
 from ..util import make_inventory
 
 
 class TestOperationMeta(TestCase):
     def test_operation_meta_repr_no_change(self):
-        op_meta = OperationMeta("hash", [])
-        assert repr(op_meta) == "OperationMeta(commands=0, changed=False, hash=hash)"
+        op_meta = OperationMeta("hash", False)
+        assert repr(op_meta) == "OperationMeta(executed=False, maybeChange=False, hash=hash)"
 
     def test_operation_meta_repr_changes(self):
-        op_meta = OperationMeta("hash", ["a-command"])
-        assert repr(op_meta) == "OperationMeta(commands=1, changed=True, hash=hash)"
+        op_meta = OperationMeta("hash", True)
+        assert repr(op_meta) == "OperationMeta(executed=False, maybeChange=True, hash=hash)"
 
 
 class TestOperationsApi(PatchSSHTestCase):
     def test_op(self):
         inventory = make_inventory()
         somehost = inventory.get_host("somehost")
         anotherhost = inventory.get_host("anotherhost")
@@ -56,93 +57,68 @@
             state,
             files.file,
             "/var/log/pyinfra.log",
             user="pyinfra",
             group="pyinfra",
             mode="644",
             create_remote_dir=False,
-            sudo=True,
-            sudo_user="test_sudo",
-            su_user="test_su",
-            ignore_errors=True,
-            env={
+            _sudo=True,
+            _sudo_user="test_sudo",
+            _su_user="test_su",
+            _ignore_errors=True,
+            _env={
                 "TEST": "what",
             },
         )
 
         op_order = state.get_op_order()
 
         # Ensure we have an op
         assert len(op_order) == 1
 
         first_op_hash = op_order[0]
 
         # Ensure the op name
-        assert state.op_meta[first_op_hash]["names"] == {"Files/File"}
+        assert state.op_meta[first_op_hash].names == {"files.file"}
+
+        # Ensure the global kwargs (same for both hosts)
+        somehost_global_arguments = state.ops[somehost][first_op_hash].global_arguments
+        assert somehost_global_arguments["_sudo"] is True
+        assert somehost_global_arguments["_sudo_user"] == "test_sudo"
+        assert somehost_global_arguments["_su_user"] == "test_su"
+        assert somehost_global_arguments["_ignore_errors"] is True
+
+        anotherhost_global_arguments = state.ops[anotherhost][first_op_hash].global_arguments
+        assert anotherhost_global_arguments["_sudo"] is True
+        assert anotherhost_global_arguments["_sudo_user"] == "test_sudo"
+        assert anotherhost_global_arguments["_su_user"] == "test_su"
+        assert anotherhost_global_arguments["_ignore_errors"] is True
+
+        # Ensure run ops works
+        run_ops(state)
 
         # Ensure the commands
-        assert state.ops[somehost][first_op_hash]["commands"] == [
+        assert state.ops[somehost][first_op_hash].operation_meta._commands == [
             StringCommand("touch /var/log/pyinfra.log"),
             StringCommand("chmod 644 /var/log/pyinfra.log"),
             StringCommand("chown pyinfra:pyinfra /var/log/pyinfra.log"),
         ]
 
-        # Ensure the global kwargs (same for both hosts)
-        somehost_global_kwargs = state.ops[somehost][first_op_hash]["global_kwargs"]
-        assert somehost_global_kwargs["sudo"] is True
-        assert somehost_global_kwargs["sudo_user"] == "test_sudo"
-        assert somehost_global_kwargs["su_user"] == "test_su"
-        assert somehost_global_kwargs["ignore_errors"] is True
-
-        anotherhost_global_kwargs = state.ops[anotherhost][first_op_hash]["global_kwargs"]
-        assert anotherhost_global_kwargs["sudo"] is True
-        assert anotherhost_global_kwargs["sudo_user"] == "test_sudo"
-        assert anotherhost_global_kwargs["su_user"] == "test_su"
-        assert anotherhost_global_kwargs["ignore_errors"] is True
-
-        # Ensure run ops works
-        run_ops(state)
-
         # Ensure ops completed OK
-        assert state.results[somehost]["success_ops"] == 1
-        assert state.results[somehost]["ops"] == 1
-        assert state.results[anotherhost]["success_ops"] == 1
-        assert state.results[anotherhost]["ops"] == 1
+        assert state.results[somehost].success_ops == 1
+        assert state.results[somehost].ops == 1
+        assert state.results[anotherhost].success_ops == 1
+        assert state.results[anotherhost].ops == 1
 
         # And w/o errors
-        assert state.results[somehost]["error_ops"] == 0
-        assert state.results[anotherhost]["error_ops"] == 0
-
-        # And with the different modes
-        run_ops(state, serial=True)
-        run_ops(state, no_wait=True)
+        assert state.results[somehost].error_ops == 0
+        assert state.results[anotherhost].error_ops == 0
 
         disconnect_all(state)
 
-    # def test_op_call_direct_falls(self):
-    #     inventory = make_inventory()
-    #     somehost = inventory.get_host('somehost')
-    #     state = State(inventory, Config())
-
-    #     # Enable printing on this test to catch any exceptions in the formatting
-    #     state.print_output = True
-    #     state.print_input = True
-    #     state.print_fact_info = True
-    #     state.print_noop_info = True
-
-    #     connect_all(state)
-
-    #     with self.assertRaises(PyinfraError) as context:
-    #         server.shell(commands='echo hi')
-
-    #     assert context.exception.args[0] == (
-    #         'Operation order number not provided in API mode - '
-    #         'you must use `add_op` to add operations.'
-    #     )
-
     @patch("pyinfra.api.util.open", mock_open(read_data="test!"), create=True)
     @patch("pyinfra.operations.files.os.path.isfile", lambda *args, **kwargs: True)
     def test_file_upload_op(self):
         inventory = make_inventory()
 
         state = State(inventory, Config())
         connect_all(state)
@@ -158,67 +134,67 @@
 
         # And with sudo
         add_op(
             state,
             files.put,
             src="files/file.txt",
             dest="/home/vagrant/file.txt",
-            sudo=True,
-            sudo_user="pyinfra",
+            _sudo=True,
+            _sudo_user="pyinfra",
         )
 
         # And with su
         add_op(
             state,
             files.put,
             src="files/file.txt",
             dest="/home/vagrant/file.txt",
-            sudo=True,
-            su_user="pyinfra",
+            _sudo=True,
+            _su_user="pyinfra",
         )
 
         op_order = state.get_op_order()
 
         # Ensure we have all ops
         assert len(op_order) == 3
 
         first_op_hash = op_order[0]
         second_op_hash = op_order[1]
 
         # Ensure first op is the right one
-        assert state.op_meta[first_op_hash]["names"] == {"First op name"}
+        assert state.op_meta[first_op_hash].names == {"First op name"}
 
         somehost = inventory.get_host("somehost")
         anotherhost = inventory.get_host("anotherhost")
 
-        # Ensure first op has the right (upload) command
-        assert state.ops[somehost][first_op_hash]["commands"] == [
-            StringCommand("mkdir -p /home/vagrant"),
-            FileUploadCommand("files/file.txt", "/home/vagrant/file.txt"),
-        ]
-
         # Ensure second op has sudo/sudo_user
-        assert state.ops[somehost][second_op_hash]["global_kwargs"]["sudo"] is True
-        assert state.ops[somehost][second_op_hash]["global_kwargs"]["sudo_user"] == "pyinfra"
+        assert state.ops[somehost][second_op_hash].global_arguments["_sudo"] is True
+        assert state.ops[somehost][second_op_hash].global_arguments["_sudo_user"] == "pyinfra"
 
         # Ensure third has su_user
-        assert state.ops[somehost][op_order[2]]["global_kwargs"]["su_user"] == "pyinfra"
+        assert state.ops[somehost][op_order[2]].global_arguments["_su_user"] == "pyinfra"
 
         # Check run ops works
         run_ops(state)
 
+        # Ensure first op used the right (upload) command
+        assert state.ops[somehost][first_op_hash].operation_meta._commands == [
+            StringCommand("mkdir -p /home/vagrant"),
+            FileUploadCommand("files/file.txt", "/home/vagrant/file.txt"),
+        ]
+
         # Ensure ops completed OK
-        assert state.results[somehost]["success_ops"] == 3
-        assert state.results[somehost]["ops"] == 3
-        assert state.results[anotherhost]["success_ops"] == 3
-        assert state.results[anotherhost]["ops"] == 3
+        assert state.results[somehost].success_ops == 3
+        assert state.results[somehost].ops == 3
+        assert state.results[anotherhost].success_ops == 3
+        assert state.results[anotherhost].ops == 3
 
         # And w/o errors
-        assert state.results[somehost]["error_ops"] == 0
-        assert state.results[anotherhost]["error_ops"] == 0
+        assert state.results[somehost].error_ops == 0
+        assert state.results[anotherhost].error_ops == 0
 
     def test_file_download_op(self):
         inventory = make_inventory()
 
         state = State(inventory, Config())
         connect_all(state)
 
@@ -232,33 +208,33 @@
             )
 
         op_order = state.get_op_order()
 
         assert len(op_order) == 1
 
         first_op_hash = op_order[0]
-        assert state.op_meta[first_op_hash]["names"] == {"First op name"}
+        assert state.op_meta[first_op_hash].names == {"First op name"}
 
         somehost = inventory.get_host("somehost")
         anotherhost = inventory.get_host("anotherhost")
 
+        with patch("pyinfra.api.util.open", mock_open(read_data="test!"), create=True):
+            run_ops(state)
+
         # Ensure first op has the right (upload) command
-        assert state.ops[somehost][first_op_hash]["commands"] == [
+        assert state.ops[somehost][first_op_hash].operation_meta._commands == [
             FileDownloadCommand("/home/vagrant/file.txt", "files/file.txt"),
         ]
 
-        with patch("pyinfra.api.util.open", mock_open(read_data="test!"), create=True):
-            run_ops(state)
-
-        assert state.results[somehost]["success_ops"] == 1
-        assert state.results[somehost]["ops"] == 1
-        assert state.results[anotherhost]["success_ops"] == 1
-        assert state.results[anotherhost]["ops"] == 1
-        assert state.results[somehost]["error_ops"] == 0
-        assert state.results[anotherhost]["error_ops"] == 0
+        assert state.results[somehost].success_ops == 1
+        assert state.results[somehost].ops == 1
+        assert state.results[anotherhost].success_ops == 1
+        assert state.results[anotherhost].ops == 1
+        assert state.results[somehost].error_ops == 0
+        assert state.results[anotherhost].error_ops == 0
 
     def test_function_call_op(self):
         inventory = make_inventory()
         state = State(inventory, Config())
         connect_all(state)
 
         is_called = []
@@ -279,63 +255,61 @@
 
     def test_run_once_serial_op(self):
         inventory = make_inventory()
         state = State(inventory, Config())
         connect_all(state)
 
         # Add a run once op
-        add_op(state, server.shell, 'echo "hi"', run_once=True, serial=True)
+        add_op(state, server.shell, 'echo "hi"', _run_once=True, _serial=True)
 
         # Ensure it's added to op_order
         assert len(state.get_op_order()) == 1
 
         somehost = inventory.get_host("somehost")
         anotherhost = inventory.get_host("anotherhost")
 
         # Ensure between the two hosts we only run the one op
         assert len(state.ops[somehost]) + len(state.ops[anotherhost]) == 1
 
         # Check run works
         run_ops(state)
 
-        assert (
-            state.results[somehost]["success_ops"] + state.results[anotherhost]["success_ops"]
-        ) == 1
+        assert (state.results[somehost].success_ops + state.results[anotherhost].success_ops) == 1
 
+    @patch("pyinfra.connectors.ssh.SSHConnector.check_can_rsync", lambda _: True)
     def test_rsync_op(self):
         inventory = make_inventory(hosts=("somehost",))
         state = State(inventory, Config())
         connect_all(state)
 
-        with patch("pyinfra.connectors.ssh.check_can_rsync"):
-            add_op(state, files.rsync, "src", "dest", sudo=True, sudo_user="root")
+        add_op(state, files.rsync, "src", "dest", _sudo=True, _sudo_user="root")
 
         assert len(state.get_op_order()) == 1
 
         with patch("pyinfra.connectors.ssh.run_local_process") as fake_run_local_process:
             fake_run_local_process.return_value = 0, []
             run_ops(state)
 
         fake_run_local_process.assert_called_with(
             (
                 "rsync -ax --delete --rsh "
-                '"ssh -o BatchMode=yes"'
+                '"ssh -o BatchMode=yes -o \\"StrictHostKeyChecking=accept-new\\""'
                 " --rsync-path 'sudo -u root rsync' src vagrant@somehost:dest"
             ),
             print_output=False,
             print_prefix=inventory.get_host("somehost").print_prefix,
         )
 
+    @patch("pyinfra.connectors.ssh.SSHConnector.check_can_rsync", lambda _: True)
     def test_rsync_op_with_strict_host_key_checking_disabled(self):
         inventory = make_inventory(hosts=(("somehost", {"ssh_strict_host_key_checking": "no"}),))
         state = State(inventory, Config())
         connect_all(state)
 
-        with patch("pyinfra.connectors.ssh.check_can_rsync"):
-            add_op(state, files.rsync, "src", "dest", sudo=True, sudo_user="root")
+        add_op(state, files.rsync, "src", "dest", _sudo=True, _sudo_user="root")
 
         assert len(state.get_op_order()) == 1
 
         with patch("pyinfra.connectors.ssh.run_local_process") as fake_run_local_process:
             fake_run_local_process.return_value = 0, []
             run_ops(state)
 
@@ -345,14 +319,15 @@
                 '"ssh -o BatchMode=yes -o \\"StrictHostKeyChecking=no\\""'
                 " --rsync-path 'sudo -u root rsync' src vagrant@somehost:dest"
             ),
             print_output=False,
             print_prefix=inventory.get_host("somehost").print_prefix,
         )
 
+    @patch("pyinfra.connectors.ssh.SSHConnector.check_can_rsync", lambda _: True)
     def test_rsync_op_with_strict_host_key_checking_disabled_and_custom_config_file(self):
         inventory = make_inventory(
             hosts=(
                 (
                     "somehost",
                     {
                         "ssh_strict_host_key_checking": "no",
@@ -360,16 +335,15 @@
                     },
                 ),
             )
         )
         state = State(inventory, Config())
         connect_all(state)
 
-        with patch("pyinfra.connectors.ssh.check_can_rsync"):
-            add_op(state, files.rsync, "src", "dest", sudo=True, sudo_user="root")
+        add_op(state, files.rsync, "src", "dest", _sudo=True, _sudo_user="root")
 
         assert len(state.get_op_order()) == 1
 
         with patch("pyinfra.connectors.ssh.run_local_process") as fake_run_local_process:
             fake_run_local_process.return_value = 0, []
             run_ops(state)
 
@@ -380,34 +354,35 @@
                 '-o \\"StrictHostKeyChecking=no\\" -F /home/me/ssh_test_config"'
                 " --rsync-path 'sudo -u root rsync' src vagrant@somehost:dest"
             ),
             print_output=False,
             print_prefix=inventory.get_host("somehost").print_prefix,
         )
 
+    @patch("pyinfra.connectors.ssh.SSHConnector.check_can_rsync", lambda _: True)
     def test_rsync_op_with_sanitized_custom_config_file(self):
         inventory = make_inventory(
             hosts=(("somehost", {"ssh_config_file": "/home/me/ssh_test_config && echo hi"}),)
         )
         state = State(inventory, Config())
         connect_all(state)
 
-        with patch("pyinfra.connectors.ssh.check_can_rsync"):
-            add_op(state, files.rsync, "src", "dest", sudo=True, sudo_user="root")
+        add_op(state, files.rsync, "src", "dest", _sudo=True, _sudo_user="root")
 
         assert len(state.get_op_order()) == 1
 
         with patch("pyinfra.connectors.ssh.run_local_process") as fake_run_local_process:
             fake_run_local_process.return_value = 0, []
             run_ops(state)
 
         fake_run_local_process.assert_called_with(
             (
                 "rsync -ax --delete --rsh "
-                "\"ssh -o BatchMode=yes -F '/home/me/ssh_test_config && echo hi'\""
+                '"ssh -o BatchMode=yes -o \\"StrictHostKeyChecking=accept-new\\" '
+                "-F '/home/me/ssh_test_config && echo hi'\""
                 " --rsync-path 'sudo -u root rsync' src vagrant@somehost:dest"
             ),
             print_output=False,
             print_prefix=inventory.get_host("somehost").print_prefix,
         )
 
     def test_rsync_op_failure(self):
@@ -426,22 +401,24 @@
 
         state = State(inventory, Config())
 
         class NoSetDefaultDict(defaultdict):
             def setdefault(self, key, _):
                 return self[key]
 
-        state.op_meta = NoSetDefaultDict(lambda: {"serial": True})
+        op_meta_item = StateOperationMeta(tuple())
+        op_meta_item.global_arguments = {"_serial": True}
+        state.op_meta = NoSetDefaultDict(lambda: op_meta_item)
 
         connect_all(state)
 
         with self.assertRaises(OperationValueError) as context:
-            add_op(state, files.file, "/var/log/pyinfra.log", serial=False)
+            add_op(state, files.file, "/var/log/pyinfra.log", _serial=False)
 
-        assert context.exception.args[0] == "Cannot have different values for `serial`."
+        assert context.exception.args[0] == "Cannot have different values for `_serial`."
 
 
 class TestNestedOperationsApi(PatchSSHTestCase):
     def test_nested_op_api(self):
         inventory = make_inventory()
         state = State(inventory, Config())
 
@@ -452,101 +429,86 @@
         ctx_state.set(state)
         ctx_host.set(somehost)
 
         pyinfra.is_cli = True
 
         try:
             outer_result = server.shell(commands="echo outer")
-            assert outer_result.combined_output_lines is None
+            assert outer_result._combined_output_lines is None
 
             def callback():
                 inner_result = server.shell(commands="echo inner")
-                assert inner_result.combined_output_lines is not None
+                assert inner_result._combined_output_lines is not None
 
             python.call(function=callback)
 
             assert len(state.get_op_order()) == 2
 
             run_ops(state)
 
             assert len(state.get_op_order()) == 3
-            assert state.results[somehost]["success_ops"] == 3
-            assert outer_result.combined_output_lines is not None
+            assert state.results[somehost].success_ops == 3
+            assert outer_result._combined_output_lines is not None
 
             disconnect_all(state)
         finally:
             pyinfra.is_cli = False
 
 
 class TestOperationFailures(PatchSSHTestCase):
     def test_full_op_fail(self):
         inventory = make_inventory()
         state = State(inventory, Config())
         connect_all(state)
 
         add_op(state, server.shell, 'echo "hi"')
 
-        with patch("pyinfra.connectors.ssh.run_shell_command") as fake_run_command:
+        with patch("pyinfra.connectors.ssh.SSHConnector.run_shell_command") as fake_run_command:
             fake_channel = FakeChannel(1)
             fake_run_command.return_value = (
                 False,
                 FakeBuffer("", fake_channel),
             )
 
             with self.assertRaises(PyinfraError) as e:
                 run_ops(state)
 
             assert e.exception.args[0] == "No hosts remaining!"
 
             somehost = inventory.get_host("somehost")
 
             # Ensure the op was not flagged as success
-            assert state.results[somehost]["success_ops"] == 0
+            assert state.results[somehost].success_ops == 0
             # And was flagged asn an error
-            assert state.results[somehost]["error_ops"] == 1
+            assert state.results[somehost].error_ops == 1
 
     def test_ignore_errors_op_fail(self):
         inventory = make_inventory()
         state = State(inventory, Config())
         connect_all(state)
 
-        add_op(state, server.shell, 'echo "hi"', ignore_errors=True)
+        add_op(state, server.shell, 'echo "hi"', _ignore_errors=True)
 
-        with patch("pyinfra.connectors.ssh.run_shell_command") as fake_run_command:
+        with patch("pyinfra.connectors.ssh.SSHConnector.run_shell_command") as fake_run_command:
             fake_channel = FakeChannel(1)
             fake_run_command.return_value = (
                 False,
                 FakeBuffer("", fake_channel),
             )
 
             # This should run OK
             run_ops(state)
 
         somehost = inventory.get_host("somehost")
 
         # Ensure the op was added to results
-        assert state.results[somehost]["ops"] == 1
-        assert state.results[somehost]["ignored_error_ops"] == 1
+        assert state.results[somehost].ops == 1
+        assert state.results[somehost].ignored_error_ops == 1
         # But not as a success
-        assert state.results[somehost]["success_ops"] == 0
-
-    # def test_no_invalid_op_call(self):
-    #     inventory = make_inventory()
-    #     state = State(inventory, Config())
-    #     connect_all(state)
-    #     ctx_state.set(state)
-
-    #     state.in_op = True
-    #     with self.assertRaises(PyinfraError):
-    #         server.user('user')
-
-    #     state.in_op = False
-    #     state.in_deploy = True
-    #     with self.assertRaises(PyinfraError):
-    #         server.user('user')
+        assert state.results[somehost].success_ops == 0
 
 
 class TestOperationOrdering(PatchSSHTestCase):
     # In CLI mode, pyinfra uses *line numbers* to order operations as defined by
     # the user. This makes reasoning about user-written deploys simple and easy
     # to understand.
     def test_cli_op_line_numbers(self):
@@ -563,26 +525,27 @@
         for name in ("anotherhost", "somehost"):
             ctx_host.set(inventory.get_host(name))
             server.shell("echo hi")  # note this is called twice but on *the same line*
 
         # Add op to just the second host - using the context modules such that
         # it replicates a deploy file.
         ctx_host.set(inventory.get_host("anotherhost"))
-        first_context_hash = server.user("anotherhost_user").hash
+        first_context_hash = server.user("anotherhost_user")._hash
 
         # Add op to just the first host - using the context modules such that
         # it replicates a deploy file.
         ctx_host.set(inventory.get_host("somehost"))
-        second_context_hash = server.user("somehost_user").hash
+        second_context_hash = server.user("somehost_user")._hash
 
         ctx_state.reset()
         ctx_host.reset()
 
         pyinfra.is_cli = False
 
+        print(state.ops)
         # Ensure there are two ops
         op_order = state.get_op_order()
         assert len(op_order) == 3
 
         # And that the two ops above were called in the expected order
         assert op_order[1] == first_context_hash
         assert op_order[2] == second_context_hash
@@ -598,83 +561,20 @@
         inventory = make_inventory()
         state = State(inventory, Config())
         connect_all(state)
 
         another_host = inventory.get_host("anotherhost")
 
         def add_another_op():
-            return add_op(state, server.shell, "echo second-op")[another_host].hash
+            return add_op(state, server.shell, "echo second-op")[another_host]._hash
 
-        first_op_hash = add_op(state, server.shell, "echo first-op")[another_host].hash
+        first_op_hash = add_op(state, server.shell, "echo first-op")[another_host]._hash
         second_op_hash = add_another_op()  # note `add_op` will be called on an earlier line
 
         op_order = state.get_op_order()
         assert len(op_order) == 2
 
         assert op_order[0] == first_op_hash
         assert op_order[1] == second_op_hash
 
 
 this_filename = path.join("tests", "test_api", "test_api_operations.py")
-
-
-# class TestOperationExceptions(TestCase):
-#     def test_add_op_rejects_cli(self):
-#         pyinfra.is_cli = True
-
-#         with self.assertRaises(PyinfraError) as context:
-#             add_op(None, server.shell)
-#         call_line = getframeinfo(currentframe()).lineno - 1
-
-#         pyinfra.is_cli = False
-
-#         assert context.exception.args[0] == (
-#             '`add_op` should not be called when pyinfra is executing in CLI mode! '
-#             '(line {0} in {1})'.format(call_line, this_filename)
-#         )
-
-#     def test_op_call_rejects_no_cli(self):
-#         with self.assertRaises(PyinfraError) as context:
-#             server.shell()
-#         call_line = getframeinfo(currentframe()).lineno - 1
-
-#         assert context.exception.args[0] == (
-#             'API operation called without state/host: '
-#             'server.shell (line {0} in {1})'.format(call_line, this_filename)
-#         )
-
-#     def test_op_call_rejects_in_op(self):
-#         state = FakeState()
-
-#         pyinfra.is_cli = True
-#         ctx_state.set(state)
-
-#         with self.assertRaises(PyinfraError) as context:
-#             server.shell()
-#         call_line = getframeinfo(currentframe()).lineno - 1
-
-#         pyinfra.is_cli = False
-#         ctx_state.reset()
-
-#         assert context.exception.args[0] == (
-#             'Nested operation called without state/host: '
-#             'server.shell (line {0} in {1})'.format(call_line, this_filename)
-#         )
-
-#     def test_op_call_rejects_in_deploy(self):
-#         state = FakeState()
-#         state.in_op = False
-
-#         pyinfra.is_cli = True
-#         ctx_state.set(state)
-
-#         with self.assertRaises(PyinfraError) as context:
-#             server.shell()
-#         call_line = getframeinfo(currentframe()).lineno - 1
-
-#         pyinfra.is_cli = False
-#         ctx_state.reset()
-
-#         assert context.exception.args[0] == (
-#             'Nested deploy operation called without state/host: '
-#             'server.shell (line {0} in {1})'.format(call_line, this_filename)
-#         )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_cli/test_cli.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_cli/test_cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from os import path
 from unittest import TestCase
 
-from pyinfra.context import ctx_state
 from pyinfra_cli.main import _main
 
 from ..paramiko_util import PatchSSHTestCase
 from .util import run_cli
 
 
 class TestCliEagerFlags(TestCase):
@@ -13,121 +12,93 @@
         result = run_cli("--version")
         assert result.exit_code == 0, result.stdout
 
         result = run_cli("--help")
         assert result.exit_code == 0, result.stdout
 
 
-class TestDeployCli(PatchSSHTestCase):
-    def setUp(self):
-        ctx_state.reset()
-
-    def test_invalid_deploy(self):
-        result = run_cli(
-            "@local",
-            "not-a-file.py",
-        )
-        assert result.exit_code == 1, result.stdout
-        assert "No deploy file: not-a-file.py" in result.stdout
-
-
 class TestOperationCli(PatchSSHTestCase):
     def test_invalid_operation_module(self):
         result = run_cli(
-            path.join("tests", "deploy", "inventories", "inventory.py"),
+            path.join("tests", "test_cli", "deploy", "inventories", "inventory.py"),
             "not_a_module.shell",
         )
         assert result.exit_code == 1, result.stdout
         assert "No such module: not_a_module"
 
     def test_invalid_operation_function(self):
         result = run_cli(
-            path.join("tests", "deploy", "inventories", "inventory.py"),
+            path.join("tests", "test_cli", "deploy", "inventories", "inventory.py"),
             "server.not_an_operation",
         )
         assert result.exit_code == 1, result.stdout
         assert "No such operation: server.not_an_operation"
 
     def test_deploy_operation(self):
         result = run_cli(
-            path.join("tests", "deploy", "inventories", "inventory.py"),
+            "-y",
+            path.join("tests", "test_cli", "deploy", "inventories", "inventory.py"),
             "server.shell",
             "echo hi",
         )
         assert result.exit_code == 0, result.stdout
 
     def test_deploy_operation_with_all(self):
         result = run_cli(
-            path.join("tests", "deploy", "inventory_all.py"),
+            "-y",
+            path.join("tests", "test_cli", "deploy", "inventory_all.py"),
             "server.shell",
             "echo hi",
         )
         assert result.exit_code == 0, result.stdout
 
     def test_deploy_operation_json_args(self):
         result = run_cli(
-            path.join("tests", "deploy", "inventory_all.py"),
+            "-y",
+            path.join("tests", "test_cli", "deploy", "inventory_all.py"),
             "server.shell",
             '[["echo hi"], {}]',
         )
         assert result.exit_code == 0, result.stdout
 
 
 class TestFactCli(PatchSSHTestCase):
     def test_get_fact(self):
         result = run_cli(
-            path.join("tests", "deploy", "inventories", "inventory.py"),
+            path.join("tests", "test_cli", "deploy", "inventories", "inventory.py"),
             "fact",
             "server.Os",
         )
         assert result.exit_code == 0, result.stdout
         assert '"somehost": null' in result.stdout
 
     def test_get_fact_with_kwargs(self):
         result = run_cli(
-            path.join("tests", "deploy", "inventories", "inventory.py"),
+            path.join("tests", "test_cli", "deploy", "inventories", "inventory.py"),
             "fact",
             "files.File",
             "path=.",
         )
         assert result.exit_code == 0, result.stdout
         assert '"somehost": null' in result.stdout
 
-    def test_invalid_fact_module(self):
-        result = run_cli(
-            path.join("tests", "deploy", "inventories", "inventory.py"),
-            "fact",
-            "not_a_module.NotAFact",
-        )
-        assert result.exit_code == 1, result.stdout
-        assert "No such module: pyinfra.facts.not_a_module" in result.stdout
-
-    def test_invalid_fact_class(self):
-        result = run_cli(
-            path.join("tests", "deploy", "inventories", "inventory.py"),
-            "fact",
-            "server.NotAFact",
-        )
-        assert result.exit_code == 1, result.stdout
-        assert "No such attribute in module pyinfra.facts.server: NotAFact" in result.stdout
-
 
 class TestExecCli(PatchSSHTestCase):
     def test_exec_command(self):
         result = run_cli(
-            path.join("tests", "deploy", "inventories", "inventory.py"),
+            path.join("tests", "test_cli", "deploy", "inventories", "inventory.py"),
             "exec",
             "--",
             "echo hi",
         )
         assert result.exit_code == 0, result.stdout
 
     def test_exec_command_with_options(self):
         result = run_cli(
-            path.join("tests", "deploy", "inventories", "inventory.py"),
+            path.join("tests", "test_cli", "deploy", "inventories", "inventory.py"),
             "exec",
             "--sudo",
             "--sudo-user",
             "pyinfra",
             "--su-user",
             "pyinfrawhat",
             "--port",
@@ -137,45 +108,45 @@
             "--",
             "echo hi",
         )
         assert result.exit_code == 0, result.stdout
 
     def test_exec_command_with_serial(self):
         result = run_cli(
-            path.join("tests", "deploy", "inventories", "inventory.py"),
+            path.join("tests", "test_cli", "deploy", "inventories", "inventory.py"),
             "exec",
             "--serial",
             "--",
             "echo hi",
         )
         assert result.exit_code == 0, result.stdout
 
     def test_exec_command_with_no_wait(self):
         result = run_cli(
-            path.join("tests", "deploy", "inventories", "inventory.py"),
+            path.join("tests", "test_cli", "deploy", "inventories", "inventory.py"),
             "exec",
             "--no-wait",
             "--",
             "echo hi",
         )
         assert result.exit_code == 0, result.stdout
 
     def test_exec_command_with_debug_operations(self):
         result = run_cli(
-            path.join("tests", "deploy", "inventories", "inventory.py"),
+            path.join("tests", "test_cli", "deploy", "inventories", "inventory.py"),
             "exec",
             "--debug-operations",
             "--",
             "echo hi",
         )
         assert result.exit_code == 0, result.stdout
 
     def test_exec_command_with_debug_facts(self):
         result = run_cli(
-            path.join("tests", "deploy", "inventories", "inventory.py"),
+            path.join("tests", "test_cli", "deploy", "inventories", "inventory.py"),
             "exec",
             "--debug-facts",
             "--",
             "echo hi",
         )
         assert result.exit_code == 0, result.stdout
 
@@ -202,23 +173,21 @@
                 sudo=False,
                 sudo_user=None,
                 use_sudo_password=False,
                 su_user=None,
                 parallel=None,
                 fail_percent=0,
                 dry=False,
+                yes=True,
                 limit=None,
                 no_wait=False,
                 serial=False,
-                winrm_username=None,
-                winrm_password=None,
-                winrm_port=None,
-                winrm_transport=None,
                 shell_executable=None,
                 quiet=False,
                 data=tuple(),
                 debug=False,
                 debug_facts=False,
+                debug_all=False,
                 debug_operations=False,
                 config_filename="config.py",
             )
             assert e.args == (0,)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_cli/test_cli_deploy.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_cli/test_cli_deploy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,40 @@
 from os import path
 from random import shuffle
 
-from pyinfra import inventory, state
+from pyinfra import state
 from pyinfra.context import ctx_state
 
 from ..paramiko_util import PatchSSHTestCase
 from .util import run_cli
 
 
-class TestCliDeploy(PatchSSHTestCase):
-    def test_interdependent_deploy(self):
-        ctx_state.reset()
-
-        result = run_cli(
-            "somehost",
-            path.join("tests", "deploy", "deploy_interdependent.py"),
-            f'--chdir={path.join("tests", "deploy")}',
+class TestCliDeployState(PatchSSHTestCase):
+    def _run_cli(self, hosts, filename):
+        return run_cli(
+            "-y",
+            ",".join(hosts),
+            path.join("tests", "test_cli", "deploy", filename),
+            f'--chdir={path.join("tests", "test_cli", "deploy")}',
         )
-        assert result.exit_code == 0, result.stdout
-
-        # Check every operation had commands/changes - this ensures that each
-        # combo (add/remove/add) always had changes.
-        for host, ops in state.ops.items():
-            for _, op in ops.items():
-                assert len(op["commands"]) > 0
-
 
-class TestCliDeployState(PatchSSHTestCase):
     def _assert_op_data(self, correct_op_name_and_host_names):
         op_order = state.get_op_order()
 
         assert len(correct_op_name_and_host_names) == len(
             op_order,
         ), "Incorrect number of operations detected"
 
         for i, (correct_op_name, correct_host_names) in enumerate(
             correct_op_name_and_host_names,
         ):
             op_hash = op_order[i]
             op_meta = state.op_meta[op_hash]
 
-            assert list(op_meta["names"])[0] == correct_op_name
+            assert list(op_meta.names)[0] == correct_op_name
 
             for host in state.inventory:
                 if correct_host_names is True or host.name in correct_host_names:
                     self.assertIn(op_hash, host.op_hash_order)
                 else:
                     self.assertNotIn(op_hash, host.op_hash_order)
 
@@ -88,19 +78,15 @@
         # hosts - ensuring that the ordering has no effect on the operation order.
         for _ in range(3):
             ctx_state.reset()
 
             hosts = ["somehost", "anotherhost", "someotherhost"]
             shuffle(hosts)
 
-            result = run_cli(
-                ",".join(hosts),
-                path.join("tests", "deploy", "deploy.py"),
-                f'--chdir={path.join("tests", "deploy")}',
-            )
+            result = self._run_cli(hosts, "deploy.py")
             assert result.exit_code == 0, result.stdout
 
             self._assert_op_data(correct_op_name_and_host_names)
 
     def test_random_deploy(self):
         correct_op_name_and_host_names = [
             ("First main operation", True),
@@ -117,23 +103,11 @@
         # hosts - ensuring that the ordering has no effect on the operation order.
         for _ in range(3):
             ctx_state.reset()
 
             hosts = ["somehost", "anotherhost", "someotherhost"]
             shuffle(hosts)
 
-            result = run_cli(
-                ",".join(hosts),
-                path.join("tests", "deploy", "deploy_random.py"),
-                f'--chdir={path.join("tests", "deploy")}',
-            )
+            result = self._run_cli(hosts, "deploy_random.py")
             assert result.exit_code == 0, result.stdout
 
             self._assert_op_data(correct_op_name_and_host_names)
-
-            for hostname, expected_fact_count in (
-                ("somehost", 2),
-                ("anotherhost", 0),
-                ("someotherhost", 1),
-            ):
-                host = inventory.get_host(hostname)
-                assert len(host.facts) == expected_fact_count
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_cli/test_cli_util.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_cli/test_cli_util.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_cli/test_context_objects.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_cli/test_context_objects.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_chroot.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_chroot.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,19 +59,19 @@
         host = inventory.get_host("@chroot/not-a-chroot")
         host.connect()
 
         command = "echo hoi"
         self.fake_popen_mock().returncode = 0
         out = host.run_shell_command(
             command,
-            stdin="hello",
-            get_pty=True,
+            _stdin="hello",
+            _get_pty=True,
             print_output=True,
         )
-        assert len(out) == 3
+        assert len(out) == 2
         assert out[0] is True
 
         command = make_unix_command(command).get_raw_value()
         command = shlex.quote(command)
         docker_command = "chroot /not-a-chroot sh -c {0}".format(command)
         shell_command = make_unix_command(docker_command).get_raw_value()
 
@@ -89,30 +89,30 @@
         connect_all(state)
 
         host = inventory.get_host("@chroot/not-a-chroot")
 
         command = "echo hoi"
         self.fake_popen_mock().returncode = 1
 
-        out = host.run_shell_command(command, success_exit_codes=[1])
-        assert len(out) == 3
+        out = host.run_shell_command(command, _success_exit_codes=[1])
+        assert len(out) == 2
         assert out[0] is True
 
     def test_run_shell_command_error(self):
         inventory = make_inventory(hosts=("@chroot/not-a-chroot",))
         state = State(inventory, Config())
         connect_all(state)
 
         host = inventory.get_host("@chroot/not-a-chroot")
 
         command = "echo hoi"
         self.fake_popen_mock().returncode = 1
 
         out = host.run_shell_command(command)
-        assert len(out) == 3
+        assert len(out) == 2
         assert out[0] is False
 
     def test_put_file(self):
         inventory = make_inventory(hosts=("@chroot/not-a-chroot",))
         state = State(inventory, Config())
         connect_all(state)
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_docker.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_docker.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,19 +79,19 @@
         command = "echo hi"
         self.fake_popen_mock().returncode = 0
 
         host = inventory.get_host("@docker/not-an-image")
         host.connect()
         out = host.run_shell_command(
             command,
-            stdin="hello",
-            get_pty=True,
+            _stdin="hello",
+            _get_pty=True,
             print_output=True,
         )
-        assert len(out) == 3
+        assert len(out) == 2
         assert out[0] is True
 
         command = make_unix_command(command).get_raw_value()
         command = shlex.quote(command)
         docker_command = "docker exec -it containerid sh -c {0}".format(command)
         shell_command = make_unix_command(docker_command).get_raw_value()
 
@@ -108,15 +108,15 @@
         State(inventory, Config())
 
         command = "echo hi"
         self.fake_popen_mock().returncode = 1
 
         host = inventory.get_host("@docker/not-an-image")
         host.connect()
-        out = host.run_shell_command(command, success_exit_codes=[1])
+        out = host.run_shell_command(command, _success_exit_codes=[1])
         assert out[0] is True
 
     def test_run_shell_command_error(self):
         inventory = make_inventory(hosts=("@docker/not-an-image",))
         state = State(inventory, Config())
 
         command = "echo hi"
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_dockerssh.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_dockerssh.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,68 +3,61 @@
 import shlex
 from unittest import TestCase
 from unittest.mock import MagicMock, mock_open, patch
 
 from pyinfra.api import Config, State
 from pyinfra.api.connect import connect_all
 from pyinfra.api.exceptions import InventoryError, PyinfraError
-from pyinfra.connectors.util import make_unix_command
+from pyinfra.connectors.util import CommandOutput, OutputLine, make_unix_command
 
 from ..util import make_inventory
 
 
 def fake_ssh_docker_shell(
-    state,
-    host,
+    self,
     command,
-    get_pty=False,
-    timeout=None,
-    stdin=None,
-    success_exit_codes=None,
     print_output=False,
     print_input=False,
-    return_combined_output=False,
-    use_sudo_password=False,
     **command_kwargs,
 ):
-    if host.data.ssh_hostname not in ("somehost", "anotherhost"):
-        raise PyinfraError("Invalid host", host.data.ssh_hostname)
+    if str(command) == "docker run -d not-an-image tail -f /dev/null":
+        return (True, CommandOutput([OutputLine("stdout", "containerid")]))
 
-    if command == "docker run -d not-an-image tail -f /dev/null":
-        return (True, ["containerid"], [])
+    if str(command) == "docker commit containerid":
+        return (True, CommandOutput([OutputLine("stdout", "sha256:blahsomerandomstringdata")]))
 
-    if command == "docker commit containerid":
-        return (True, ["sha256:blahsomerandomstringdata"], [])
-
-    if command == "docker rm -f containerid":
-        return (True, [], [])
+    if str(command) == "docker rm -f containerid":
+        return (True, CommandOutput([]))
 
     if str(command).startswith("rm -f"):
-        return (True, [], [])
+        return (True, CommandOutput([]))
+
+    if "$TMPDIR" in str(command):
+        return (True, CommandOutput([]))
 
     # This is a bit messy. But it's easier than trying to swap out a mock
     # when it needs to be used...
     if fake_ssh_docker_shell.custom_command:
-        custom_command, status, stdout, stderr = fake_ssh_docker_shell.custom_command
+        custom_command, status, output = fake_ssh_docker_shell.custom_command
         if str(command) == custom_command:
             fake_ssh_docker_shell.ran_custom_command = True
-            return (status, stdout, stderr)
+            return (status, output)
 
     raise PyinfraError("Invalid Command: {0}".format(command))
 
 
 def get_docker_command(command):
     shell_command = make_unix_command(command).get_raw_value()
     shell_command = shlex.quote(shell_command)
     docker_command = "docker exec -it containerid sh -c {0}".format(shell_command)
     return docker_command
 
 
-@patch("pyinfra.connectors.ssh.connect", MagicMock())
-@patch("pyinfra.connectors.ssh.run_shell_command", fake_ssh_docker_shell)
+@patch("pyinfra.connectors.ssh.SSHConnector.connect", MagicMock())
+@patch("pyinfra.connectors.ssh.SSHConnector.run_shell_command", fake_ssh_docker_shell)
 @patch("pyinfra.api.util.open", mock_open(read_data="test!"), create=True)
 class TestDockerSSHConnector(TestCase):
     def setUp(self):
         # reset custom command for shell
         fake_ssh_docker_shell.custom_command = None
         fake_ssh_docker_shell.ran_custom_command = False
 
@@ -118,145 +111,140 @@
 
     def test_run_shell_command(self):
         inventory = make_inventory(hosts=("@dockerssh/somehost:not-an-image",))
         State(inventory, Config())
 
         command = "echo hi"
 
-        fake_ssh_docker_shell.custom_command = [get_docker_command(command), True, [], []]
+        fake_ssh_docker_shell.custom_command = [get_docker_command(command), True, []]
 
         host = inventory.get_host("@dockerssh/somehost:not-an-image")
         host.connect()
         out = host.run_shell_command(
             command,
-            stdin="hello",
-            get_pty=True,
+            _stdin="hello",
+            _get_pty=True,
             print_output=True,
         )
-        assert len(out) == 3
+        assert len(out) == 2
         assert out[0] is True
         assert fake_ssh_docker_shell.ran_custom_command
 
     def test_run_shell_command_error(self):
         inventory = make_inventory(hosts=("@dockerssh/somehost:not-an-image",))
         state = State(inventory, Config())
 
         command = "echo hi"
-        fake_ssh_docker_shell.custom_command = [get_docker_command(command), False, [], []]
+        fake_ssh_docker_shell.custom_command = [get_docker_command(command), False, []]
 
         host = inventory.get_host("@dockerssh/somehost:not-an-image")
         host.connect(state)
-        out = host.run_shell_command(command, get_pty=True)
+        out = host.run_shell_command(command, _get_pty=True)
         assert out[0] is False
         assert fake_ssh_docker_shell.ran_custom_command
 
     @patch("pyinfra.connectors.dockerssh.mkstemp", lambda: (None, "local_tempfile"))
     @patch("pyinfra.connectors.docker.os.close", lambda f: None)
-    @patch("pyinfra.connectors.dockerssh.ssh.put_file")
+    @patch("pyinfra.connectors.ssh.SSHConnector.put_file")
     def test_put_file(self, fake_put_file):
         fake_ssh_docker_shell.custom_command = [
             "docker cp remote_tempfile containerid:not-another-file",
             True,
             [],
-            [],
         ]
 
         inventory = make_inventory(hosts=("@dockerssh/somehost:not-an-image",))
-        state = State(inventory, Config())
-        state.get_temp_filename = lambda _: "remote_tempfile"
+        State(inventory, Config())
 
         host = inventory.get_host("@dockerssh/somehost:not-an-image")
+        host.get_temp_filename = lambda _: "remote_tempfile"
         host.connect()
 
         host.put_file("not-a-file", "not-another-file", print_output=True)
 
         # ensure copy from local to remote host
-        fake_put_file.assert_called_with(state, host, "local_tempfile", "remote_tempfile")
+        fake_put_file.assert_called_with("local_tempfile", "remote_tempfile")
 
         # ensure copy from remote host to remote docker container
         assert fake_ssh_docker_shell.ran_custom_command
 
-    @patch("pyinfra.connectors.dockerssh.ssh.put_file")
+    @patch("pyinfra.connectors.ssh.SSHConnector.put_file")
     def test_put_file_error(self, fake_put_file):
         inventory = make_inventory(hosts=("@dockerssh/somehost:not-an-image",))
-        state = State(inventory, Config())
-        state.get_temp_filename = lambda _: "remote_tempfile"
+        State(inventory, Config())
 
         host = inventory.get_host("@dockerssh/somehost:not-an-image")
+        host.get_temp_filename = lambda _: "remote_tempfile"
         host.connect()
 
         # SSH error
         fake_put_file.return_value = False
         with self.assertRaises(IOError):
             host.put_file("not-a-file", "not-another-file", print_output=True)
 
         # docker copy error
         fake_ssh_docker_shell.custom_command = [
             "docker cp remote_tempfile containerid:not-another-file",
             False,
-            [],
-            ["docker error"],
+            CommandOutput([OutputLine("stderr", "docker error")]),
         ]
         fake_put_file.return_value = True
 
         with self.assertRaises(IOError) as e:
             host.put_file("not-a-file", "not-another-file", print_output=True)
         assert str(e.exception) == "docker error"
 
-    @patch("pyinfra.connectors.dockerssh.ssh.get_file")
+    @patch("pyinfra.connectors.ssh.SSHConnector.get_file")
     def test_get_file(self, fake_get_file):
         fake_ssh_docker_shell.custom_command = [
             "docker cp containerid:not-a-file remote_tempfile",
             True,
             [],
-            [],
         ]
 
         inventory = make_inventory(hosts=("@dockerssh/somehost:not-an-image",))
-        state = State(inventory, Config())
-        state.get_temp_filename = lambda _: "remote_tempfile"
+        State(inventory, Config())
 
         host = inventory.get_host("@dockerssh/somehost:not-an-image")
+        host.get_temp_filename = lambda _: "remote_tempfile"
         host.connect()
 
         host.get_file("not-a-file", "not-another-file", print_output=True)
 
         # ensure copy from local to remote host
-        fake_get_file.assert_called_with(state, host, "remote_tempfile", "not-another-file")
+        fake_get_file.assert_called_with("remote_tempfile", "not-another-file")
 
         # ensure copy from remote host to remote docker container
         assert fake_ssh_docker_shell.ran_custom_command
 
-    @patch("pyinfra.connectors.dockerssh.ssh.get_file")
+    @patch("pyinfra.connectors.ssh.SSHConnector.get_file")
     def test_get_file_error(self, fake_get_file):
         fake_ssh_docker_shell.custom_command = [
             "docker cp containerid:not-a-file remote_tempfile",
             False,
-            [],
-            ["docker error"],
+            CommandOutput([OutputLine("stderr", "docker error")]),
         ]
 
         inventory = make_inventory(hosts=("@dockerssh/somehost:not-an-image",))
-        state = State(inventory, Config())
-        state.get_temp_filename = lambda _: "remote_tempfile"
+        State(inventory, Config())
 
         host = inventory.get_host("@dockerssh/somehost:not-an-image")
+        host.get_temp_filename = lambda _: "remote_tempfile"
         host.connect()
 
         fake_get_file.return_value = True
         with self.assertRaises(IOError) as ex:
             host.get_file("not-a-file", "not-another-file", print_output=True)
 
         assert str(ex.exception) == "docker error"
 
         # SSH error
         fake_ssh_docker_shell.custom_command = [
             "docker cp containerid:not-a-file remote_tempfile",
             True,
             [],
-            [],
         ]
         fake_get_file.return_value = False
         with self.assertRaises(IOError) as ex:
             host.get_file("not-a-file", "not-another-file", print_output=True)
 
         assert str(ex.exception) == "failed to copy file over ssh"
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_local.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,26 +41,25 @@
         inventory = make_inventory(hosts=("@local",))
         State(inventory, Config())
         host = inventory.get_host("@local")
 
         command = "echo Šablony"
         self.fake_popen_mock().returncode = 0
 
-        out = host.run_shell_command(command, stdin="hello", print_output=True)
-        assert len(out) == 3
+        out = host.run_shell_command(command, _stdin="hello", print_output=True)
+        assert len(out) == 2
 
-        status, stdout, stderr = out
+        status, output = out
         assert status is True
         self.fake_popen_mock().stdin.write.assert_called_with(b"hello\n")
 
         combined_out = host.run_shell_command(
             command,
-            stdin="hello",
+            _stdin="hello",
             print_output=True,
-            return_combined_output=True,
         )
         assert len(combined_out) == 2
 
         shell_command = make_unix_command(command).get_raw_value()
         self.fake_popen_mock.assert_called_with(
             shell_command,
             shell=True,
@@ -75,17 +74,17 @@
         State(inventory, Config())
         host = inventory.get_host("@local")
 
         command = StringCommand("echo", MaskString("top-secret-stuff"))
         self.fake_popen_mock().returncode = 0
 
         out = host.run_shell_command(command, print_output=True, print_input=True)
-        assert len(out) == 3
+        assert len(out) == 2
 
-        status, stdout, stderr = out
+        status, output = out
         assert status is True
 
         self.fake_popen_mock.assert_called_with(
             "sh -c 'echo top-secret-stuff'",
             shell=True,
             stdout=PIPE,
             stderr=PIPE,
@@ -101,28 +100,28 @@
         inventory = make_inventory(hosts=("@local",))
         State(inventory, Config())
         host = inventory.get_host("@local")
 
         command = "echo hi"
         self.fake_popen_mock().returncode = 1
 
-        out = host.run_shell_command(command, success_exit_codes=[1])
-        assert len(out) == 3
+        out = host.run_shell_command(command, _success_exit_codes=[1])
+        assert len(out) == 2
         assert out[0] is True
 
     def test_run_shell_command_error(self):
         inventory = make_inventory(hosts=("@local",))
         State(inventory, Config())
         host = inventory.get_host("@local")
 
         command = "echo hi"
         self.fake_popen_mock().returncode = 1
 
         out = host.run_shell_command(command)
-        assert len(out) == 3
+        assert len(out) == 2
         assert out[0] is False
 
     def test_put_file(self):
         inventory = make_inventory(hosts=("@local",))
         State(inventory, Config())
 
         host = inventory.get_host("@local")
@@ -206,15 +205,15 @@
         inventory = make_inventory(hosts=("@local",))
         State(inventory, Config())
         host = inventory.get_host("@local")
 
         command = "echo Šablony"
         self.fake_popen_mock().returncode = 0
 
-        host.run_shell_command(command, stdin=["hello", "abc"], print_output=True)
+        host.run_shell_command(command, _stdin=["hello", "abc"], print_output=True)
         self.fake_popen_mock().stdin.write.assert_has_calls(
             [
                 call(b"hello\n"),
                 call(b"abc\n"),
             ],
         )
 
@@ -222,14 +221,14 @@
         inventory = make_inventory(hosts=("@local",))
         State(inventory, Config())
         host = inventory.get_host("@local")
 
         command = "echo Šablony"
         self.fake_popen_mock().returncode = 0
 
-        host.run_shell_command(command, stdin=StringIO("hello\nabc"), print_output=True)
+        host.run_shell_command(command, _stdin=StringIO("hello\nabc"), print_output=True)
         self.fake_popen_mock().stdin.write.assert_has_calls(
             [
                 call(b"hello\n"),
                 call(b"abc\n"),
             ],
         )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_ssh.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_ssh.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from paramiko import AuthenticationException, PasswordRequiredException, SSHException
 
 import pyinfra
 from pyinfra.api import Config, MaskString, State, StringCommand
 from pyinfra.api.connect import connect_all
 from pyinfra.api.exceptions import ConnectError, PyinfraError
-from pyinfra.connectors.ssh import _get_sftp_connection
 
 from ..util import make_inventory
 
 
 def make_raise_exception_function(cls, *args, **kwargs):
     def handler(*a, **kw):
         raise cls(*args, **kwargs)
@@ -24,15 +23,14 @@
 
 @patch("pyinfra.connectors.ssh.SSHClient.get_transport", MagicMock())
 @patch("pyinfra.connectors.ssh.open", mock_open(read_data="test!"), create=True)
 class TestSSHConnector(TestCase):
     def setUp(self):
         self.fake_connect_patch = patch("pyinfra.connectors.ssh.SSHClient.connect")
         self.fake_connect_mock = self.fake_connect_patch.start()
-        _get_sftp_connection.cache = {}
 
     def tearDown(self):
         self.fake_connect_patch.stop()
 
     def test_connect_all(self):
         inventory = make_inventory()
         state = State(inventory, Config())
@@ -54,16 +52,16 @@
         assert somehost.data.ssh_password == "test"
 
         state = State(inventory, Config())
         connect_all(state)
 
         assert len(state.active_hosts) == 2
 
-    @patch("pyinfra.connectors.ssh.path.isfile", lambda *args, **kwargs: True)
-    @patch("pyinfra.connectors.ssh.RSAKey.from_private_key_file")
+    @patch("pyinfra.connectors.ssh_util.path.isfile", lambda *args, **kwargs: True)
+    @patch("pyinfra.connectors.ssh_util.RSAKey.from_private_key_file")
     def test_connect_exceptions(self, fake_key_open):
         for exception_class in (
             AuthenticationException,
             SSHException,
             gaierror,
             socket_error,
             EOFError,
@@ -79,16 +77,16 @@
 
     # SSH key tests
     #
 
     def test_connect_with_rsa_ssh_key(self):
         state = State(make_inventory(hosts=(("somehost", {"ssh_key": "testkey"}),)), Config())
 
-        with patch("pyinfra.connectors.ssh.path.isfile", lambda *args, **kwargs: True), patch(
-            "pyinfra.connectors.ssh.RSAKey.from_private_key_file",
+        with patch("pyinfra.connectors.ssh_util.path.isfile", lambda *args, **kwargs: True), patch(
+            "pyinfra.connectors.ssh_util.RSAKey.from_private_key_file",
         ) as fake_key_open:
             fake_key = MagicMock()
             fake_key_open.return_value = fake_key
 
             connect_all(state)
 
             # Check the key was created properly
@@ -100,18 +98,18 @@
             self.fake_connect_mock.assert_called_with(
                 "somehost",
                 allow_agent=False,
                 look_for_keys=False,
                 pkey=fake_key,
                 timeout=10,
                 username="vagrant",
-                _pyinfra_ssh_forward_agent=None,
+                _pyinfra_ssh_forward_agent=False,
                 _pyinfra_ssh_config_file=None,
                 _pyinfra_ssh_known_hosts_file=None,
-                _pyinfra_ssh_strict_host_key_checking=None,
+                _pyinfra_ssh_strict_host_key_checking="accept-new",
                 _pyinfra_ssh_paramiko_connect_kwargs=None,
             )
 
         # Check that loading the same key again is cached in the state
         second_state = State(
             make_inventory(hosts=(("somehost", {"ssh_key": "testkey"}),)),
             Config(),
@@ -124,16 +122,16 @@
         state = State(
             make_inventory(
                 hosts=(("somehost", {"ssh_key": "testkey", "ssh_key_password": "testpass"}),),
             ),
             Config(),
         )
 
-        with patch("pyinfra.connectors.ssh.path.isfile", lambda *args, **kwargs: True), patch(
-            "pyinfra.connectors.ssh.RSAKey.from_private_key_file",
+        with patch("pyinfra.connectors.ssh_util.path.isfile", lambda *args, **kwargs: True), patch(
+            "pyinfra.connectors.ssh_util.RSAKey.from_private_key_file",
         ) as fake_key_open:
             fake_key = MagicMock()
 
             def fake_key_open_fail(*args, **kwargs):
                 if "password" not in kwargs:
                     raise PasswordRequiredException()
                 return fake_key
@@ -146,19 +144,19 @@
             fake_key_open.assert_called_with(filename="testkey", password="testpass")
             # Check the certificate file was then loaded
             fake_key.load_certificate.assert_called_with("testkey.pub")
 
     def test_connect_with_rsa_ssh_key_password_from_prompt(self):
         state = State(make_inventory(hosts=(("somehost", {"ssh_key": "testkey"}),)), Config())
 
-        with patch("pyinfra.connectors.ssh.path.isfile", lambda *args, **kwargs: True), patch(
-            "pyinfra.connectors.ssh.getpass",
+        with patch("pyinfra.connectors.ssh_util.path.isfile", lambda *args, **kwargs: True), patch(
+            "pyinfra.connectors.ssh_util.getpass",
             lambda *args, **kwargs: "testpass",
         ), patch(
-            "pyinfra.connectors.ssh.RSAKey.from_private_key_file",
+            "pyinfra.connectors.ssh_util.RSAKey.from_private_key_file",
         ) as fake_key_open:
             fake_key = MagicMock()
 
             def fake_key_open_fail(*args, **kwargs):
                 if "password" not in kwargs:
                     raise PasswordRequiredException()
                 return fake_key
@@ -173,16 +171,16 @@
             fake_key_open.assert_called_with(filename="testkey", password="testpass")
             # Check the certificate file was then loaded
             fake_key.load_certificate.assert_called_with("testkey.pub")
 
     def test_connect_with_rsa_ssh_key_missing_password(self):
         state = State(make_inventory(hosts=(("somehost", {"ssh_key": "testkey"}),)), Config())
 
-        with patch("pyinfra.connectors.ssh.path.isfile", lambda *args, **kwargs: True), patch(
-            "pyinfra.connectors.ssh.RSAKey.from_private_key_file",
+        with patch("pyinfra.connectors.ssh_util.path.isfile", lambda *args, **kwargs: True), patch(
+            "pyinfra.connectors.ssh_util.RSAKey.from_private_key_file",
         ) as fake_key_open:
             fake_key_open.side_effect = make_raise_exception_function(PasswordRequiredException)
 
             fake_key = MagicMock()
             fake_key_open.return_value = fake_key
 
             with self.assertRaises(PyinfraError) as e:
@@ -199,25 +197,25 @@
             ),
             Config(),
         )
 
         fake_fail_from_private_key_file = MagicMock()
         fake_fail_from_private_key_file.side_effect = make_raise_exception_function(SSHException)
 
-        with patch("pyinfra.connectors.ssh.path.isfile", lambda *args, **kwargs: True), patch(
-            "pyinfra.connectors.ssh.DSSKey.from_private_key_file",
+        with patch("pyinfra.connectors.ssh_util.path.isfile", lambda *args, **kwargs: True), patch(
+            "pyinfra.connectors.ssh_util.DSSKey.from_private_key_file",
             fake_fail_from_private_key_file,
         ), patch(
-            "pyinfra.connectors.ssh.ECDSAKey.from_private_key_file",
+            "pyinfra.connectors.ssh_util.ECDSAKey.from_private_key_file",
             fake_fail_from_private_key_file,
         ), patch(
-            "pyinfra.connectors.ssh.Ed25519Key.from_private_key_file",
+            "pyinfra.connectors.ssh_util.Ed25519Key.from_private_key_file",
             fake_fail_from_private_key_file,
         ), patch(
-            "pyinfra.connectors.ssh.RSAKey.from_private_key_file",
+            "pyinfra.connectors.ssh_util.RSAKey.from_private_key_file",
         ) as fake_key_open:
 
             def fake_key_open_fail(*args, **kwargs):
                 if "password" not in kwargs:
                     raise PasswordRequiredException
                 raise SSHException
 
@@ -232,18 +230,18 @@
             assert e.exception.args[0] == "Invalid private key file: testkey"
 
         assert fake_fail_from_private_key_file.call_count == 3
 
     def test_connect_with_dss_ssh_key(self):
         state = State(make_inventory(hosts=(("somehost", {"ssh_key": "testkey"}),)), Config())
 
-        with patch("pyinfra.connectors.ssh.path.isfile", lambda *args, **kwargs: True), patch(
-            "pyinfra.connectors.ssh.RSAKey.from_private_key_file",
+        with patch("pyinfra.connectors.ssh_util.path.isfile", lambda *args, **kwargs: True), patch(
+            "pyinfra.connectors.ssh_util.RSAKey.from_private_key_file",
         ) as fake_rsa_key_open, patch(
-            "pyinfra.connectors.ssh.DSSKey.from_private_key_file",
+            "pyinfra.connectors.ssh_util.DSSKey.from_private_key_file",
         ) as fake_key_open:  # noqa
             fake_rsa_key_open.side_effect = make_raise_exception_function(SSHException)
 
             fake_key = MagicMock()
             fake_key_open.return_value = fake_key
 
             connect_all(state)
@@ -255,18 +253,18 @@
             self.fake_connect_mock.assert_called_with(
                 "somehost",
                 allow_agent=False,
                 look_for_keys=False,
                 pkey=fake_key,
                 timeout=10,
                 username="vagrant",
-                _pyinfra_ssh_forward_agent=None,
+                _pyinfra_ssh_forward_agent=False,
                 _pyinfra_ssh_config_file=None,
                 _pyinfra_ssh_known_hosts_file=None,
-                _pyinfra_ssh_strict_host_key_checking=None,
+                _pyinfra_ssh_strict_host_key_checking="accept-new",
                 _pyinfra_ssh_paramiko_connect_kwargs=None,
             )
 
         # Check that loading the same key again is cached in the state
         second_state = State(
             make_inventory(hosts=(("somehost", {"ssh_key": "testkey"}),)),
             Config(),
@@ -279,18 +277,18 @@
         state = State(
             make_inventory(
                 hosts=(("somehost", {"ssh_key": "testkey", "ssh_key_password": "testpass"}),),
             ),
             Config(),
         )
 
-        with patch("pyinfra.connectors.ssh.path.isfile", lambda *args, **kwargs: True), patch(
-            "pyinfra.connectors.ssh.RSAKey.from_private_key_file",
+        with patch("pyinfra.connectors.ssh_util.path.isfile", lambda *args, **kwargs: True), patch(
+            "pyinfra.connectors.ssh_util.RSAKey.from_private_key_file",
         ) as fake_rsa_key_open, patch(
-            "pyinfra.connectors.ssh.DSSKey.from_private_key_file",
+            "pyinfra.connectors.ssh_util.DSSKey.from_private_key_file",
         ) as fake_dss_key_open:  # noqa
 
             def fake_rsa_key_open_fail(*args, **kwargs):
                 if "password" not in kwargs:
                     raise PasswordRequiredException
                 raise SSHException
 
@@ -314,18 +312,18 @@
             self.fake_connect_mock.assert_called_with(
                 "somehost",
                 allow_agent=False,
                 look_for_keys=False,
                 pkey=fake_dss_key,
                 timeout=10,
                 username="vagrant",
-                _pyinfra_ssh_forward_agent=None,
+                _pyinfra_ssh_forward_agent=False,
                 _pyinfra_ssh_config_file=None,
                 _pyinfra_ssh_known_hosts_file=None,
-                _pyinfra_ssh_strict_host_key_checking=None,
+                _pyinfra_ssh_strict_host_key_checking="accept-new",
                 _pyinfra_ssh_paramiko_connect_kwargs=None,
             )
 
         # Check that loading the same key again is cached in the state
         second_state = State(
             make_inventory(hosts=(("somehost", {"ssh_key": "testkey"}),)),
             Config(),
@@ -358,26 +356,25 @@
         State(inventory, Config())
         host = inventory.get_host("somehost")
         host.connect()
 
         command = "echo Šablony"
         fake_stdout.channel.recv_exit_status.return_value = 0
 
-        out = host.run_shell_command(command, stdin="hello", print_output=True)
-        assert len(out) == 3
+        out = host.run_shell_command(command, _stdin="hello", print_output=True)
+        assert len(out) == 2
 
-        status, stdout, stderr = out
+        status, output = out
         assert status is True
         fake_stdin.write.assert_called_with(b"hello\n")
 
         combined_out = host.run_shell_command(
             command,
-            stdin="hello",
+            _stdin="hello",
             print_output=True,
-            return_combined_output=True,
         )
         assert len(combined_out) == 2
 
         fake_ssh.exec_command.assert_called_with("sh -c 'echo Šablony'", get_pty=False)
 
     @patch("pyinfra.connectors.ssh.click")
     @patch("pyinfra.connectors.ssh.SSHClient")
@@ -393,17 +390,17 @@
         host = inventory.get_host("somehost")
         host.connect()
 
         command = StringCommand("echo", MaskString("top-secret-stuff"))
         fake_stdout.channel.recv_exit_status.return_value = 0
 
         out = host.run_shell_command(command, print_output=True, print_input=True)
-        assert len(out) == 3
+        assert len(out) == 2
 
-        status, stdout, stderr = out
+        status, output = out
         assert status is True
 
         fake_ssh.exec_command.assert_called_with(
             "sh -c 'echo top-secret-stuff'",
             get_pty=False,
         )
 
@@ -424,16 +421,16 @@
         State(inventory, Config())
         host = inventory.get_host("somehost")
         host.connect()
 
         command = "echo hi"
         fake_stdout.channel.recv_exit_status.return_value = 1
 
-        out = host.run_shell_command(command, success_exit_codes=[1])
-        assert len(out) == 3
+        out = host.run_shell_command(command, _success_exit_codes=[1])
+        assert len(out) == 2
         assert out[0] is True
 
     @patch("pyinfra.connectors.ssh.SSHClient")
     def test_run_shell_command_error(self, fake_ssh_client):
         fake_ssh = MagicMock()
         fake_stdout = MagicMock()
         fake_ssh.exec_command.return_value = MagicMock(), fake_stdout, MagicMock()
@@ -445,57 +442,19 @@
         host = inventory.get_host("somehost")
         host.connect(state)
 
         command = "echo hi"
         fake_stdout.channel.recv_exit_status.return_value = 1
 
         out = host.run_shell_command(command)
-        assert len(out) == 3
+        assert len(out) == 2
         assert out[0] is False
 
     @patch("pyinfra.connectors.util.getpass")
     @patch("pyinfra.connectors.ssh.SSHClient")
-    def test_run_shell_command_sudo_password_prompt(
-        self,
-        fake_ssh_client,
-        fake_getpass,
-    ):
-        fake_ssh = MagicMock()
-        fake_stdout = MagicMock()
-        fake_ssh.exec_command.return_value = MagicMock(), fake_stdout, MagicMock()
-
-        fake_ssh_client.return_value = fake_ssh
-        fake_getpass.return_value = "password"
-
-        inventory = make_inventory(hosts=("somehost",))
-        State(inventory, Config())
-        host = inventory.get_host("somehost")
-        host.connect()
-
-        command = "echo Šablony"
-        fake_stdout.__iter__.return_value = ["/tmp/pyinfra-sudo-askpass-XXXXXXXXXXXX"]
-        fake_stdout.channel.recv_exit_status.return_value = 0
-
-        out = host.run_shell_command(command, sudo=True, use_sudo_password=True, print_output=True)
-        assert len(out) == 3
-
-        status, stdout, stderr = out
-        assert status is True
-
-        fake_ssh.exec_command.assert_called_with(
-            (
-                "env SUDO_ASKPASS=/tmp/pyinfra-sudo-askpass-XXXXXXXXXXXX "
-                "PYINFRA_SUDO_PASSWORD=password "
-                "sudo -H -A -k sh -c 'echo Šablony'"
-            ),
-            get_pty=False,
-        )
-
-    @patch("pyinfra.connectors.util.getpass")
-    @patch("pyinfra.connectors.ssh.SSHClient")
     def test_run_shell_command_sudo_password_automatic_prompt(
         self,
         fake_ssh_client,
         fake_getpass,
     ):
         fake_ssh = MagicMock()
         first_fake_stdout = MagicMock()
@@ -520,18 +479,18 @@
         host.connect()
 
         command = "echo Šablony"
         first_fake_stdout.channel.recv_exit_status.return_value = 1
         second_fake_stdout.channel.recv_exit_status.return_value = 0
         third_fake_stdout.channel.recv_exit_status.return_value = 0
 
-        out = host.run_shell_command(command, sudo=True, print_output=True)
-        assert len(out) == 3
+        out = host.run_shell_command(command, _sudo=True, print_output=True)
+        assert len(out) == 2
 
-        status, stdout, stderr = out
+        status, output = out
         assert status is True
 
         fake_ssh.exec_command.assert_any_call(("sudo -H -n sh -c 'echo Šablony'"), get_pty=False)
 
         fake_ssh.exec_command.assert_called_with(
             (
                 "env SUDO_ASKPASS=/tmp/pyinfra-sudo-askpass-XXXXXXXXXXXX "
@@ -541,21 +500,21 @@
             get_pty=False,
         )
 
     # SSH file put/get tests
     #
 
     @patch("pyinfra.connectors.ssh.SSHClient")
-    @patch("pyinfra.connectors.util._get_sudo_password")
+    @patch("pyinfra.connectors.util.getpass")
     def test_run_shell_command_retry_for_sudo_password(
         self,
-        fake_get_sudo_password,
+        fake_getpass,
         fake_ssh_client,
     ):
-        fake_get_sudo_password.return_value = "PASSWORD"
+        fake_getpass.return_value = "PASSWORD"
 
         fake_ssh = MagicMock()
         fake_stdin = MagicMock()
         fake_stdout = MagicMock()
         fake_stderr = ["sudo: a password is required"]
         fake_ssh.exec_command.return_value = fake_stdin, fake_stdout, fake_stderr
 
@@ -567,21 +526,21 @@
         host.connect(state)
         host.connector_data["sudo_askpass_path"] = "/tmp/pyinfra-sudo-askpass-XXXXXXXXXXXX"
 
         command = "echo hi"
         return_values = [1, 0]  # return 0 on the second call
         fake_stdout.channel.recv_exit_status.side_effect = lambda: return_values.pop(0)
 
-        out = host.run_shell_command(command)
-        assert len(out) == 3
+        out = host.run_shell_command(command, _sudo=True)
+        assert len(out) == 2
         assert out[0] is True
-        assert fake_get_sudo_password.called
+        assert fake_getpass.called
         fake_ssh.exec_command.assert_called_with(
             "env SUDO_ASKPASS=/tmp/pyinfra-sudo-askpass-XXXXXXXXXXXX "
-            "PYINFRA_SUDO_PASSWORD=PASSWORD sh -c 'echo hi'",
+            "PYINFRA_SUDO_PASSWORD=PASSWORD sudo -H -A -k sh -c 'echo hi'",
             get_pty=False,
         )
 
     # SSH file put/get tests
     #
 
     @patch("pyinfra.connectors.ssh.SSHClient")
@@ -620,16 +579,16 @@
 
         fake_open = mock_open(read_data="test!")
         with patch("pyinfra.api.util.open", fake_open, create=True):
             status = host.put_file(
                 "not-a-file",
                 "not another file",
                 print_output=True,
-                sudo=True,
-                sudo_user="ubuntu",
+                _sudo=True,
+                _sudo_user="ubuntu",
             )
 
         assert status is True
 
         fake_ssh_client().exec_command.assert_has_calls(
             [
                 call(
@@ -671,16 +630,16 @@
 
         fake_open = mock_open(read_data="test!")
         with patch("pyinfra.api.util.open", fake_open, create=True):
             status = host.put_file(
                 "not-a-file",
                 "not another file",
                 print_output=True,
-                doas=True,
-                doas_user="ubuntu",
+                _doas=True,
+                _doas_user="ubuntu",
             )
 
         assert status is True
 
         fake_ssh_client().exec_command.assert_has_calls(
             [
                 call(
@@ -722,15 +681,15 @@
 
         fake_open = mock_open(read_data="test!")
         with patch("pyinfra.api.util.open", fake_open, create=True):
             status = host.put_file(
                 "not-a-file",
                 "not-another-file",
                 print_output=True,
-                su_user="centos",
+                _su_user="centos",
             )
 
         assert status is False
 
         fake_ssh_client().exec_command.assert_called_with(
             (
                 "sh -c 'setfacl -m u:centos:r "
@@ -759,15 +718,15 @@
 
         fake_open = mock_open(read_data="test!")
         with patch("pyinfra.api.util.open", fake_open, create=True):
             status = host.put_file(
                 "not-a-file",
                 "not-another-file",
                 print_output=True,
-                su_user="centos",
+                _su_user="centos",
             )
 
         assert status is False
 
         fake_ssh_client().exec_command.assert_any_call(
             (
                 "sh -c 'setfacl -m u:centos:r "
@@ -804,16 +763,16 @@
 
         fake_open = mock_open(read_data="test!")
         with patch("pyinfra.api.util.open", fake_open, create=True):
             status = host.put_file(
                 "not-a-file",
                 "not another file",
                 print_output=True,
-                sudo=True,
-                sudo_user="ubuntu",
+                _sudo=True,
+                _sudo_user="ubuntu",
                 remote_temp_filename="/a-different-tempfile",
             )
 
         assert status is True
 
         fake_ssh_client().exec_command.assert_called_with(
             ("sh -c 'rm -f " "/a-different-tempfile'"),
@@ -861,26 +820,26 @@
 
         fake_open = mock_open(read_data="test!")
         with patch("pyinfra.api.util.open", fake_open, create=True):
             status = host.get_file(
                 "not-a-file",
                 "not-another-file",
                 print_output=True,
-                sudo=True,
-                sudo_user="ubuntu",
+                _sudo=True,
+                _sudo_user="ubuntu",
             )
 
         assert status is True
 
         fake_ssh_client().exec_command.assert_has_calls(
             [
                 call(
                     (
                         "sudo -H -n -u ubuntu sh -c 'cp not-a-file "
-                        "/tmp/pyinfra-e9c0d3c8ffca943daa0e75511b0a09c84b59c508 && chmod +r not-a-file'"  # noqa
+                        "/tmp/pyinfra-e9c0d3c8ffca943daa0e75511b0a09c84b59c508 && chmod +r /tmp/pyinfra-e9c0d3c8ffca943daa0e75511b0a09c84b59c508'"  # noqa
                     ),
                     get_pty=False,
                 ),
                 call(
                     (
                         "sudo -H -n -u ubuntu sh -c 'rm -f "
                         "/tmp/pyinfra-e9c0d3c8ffca943daa0e75511b0a09c84b59c508'"
@@ -906,26 +865,26 @@
         stdout_mock.channel.recv_exit_status.return_value = 1
         fake_ssh_client().exec_command.return_value = MagicMock(), stdout_mock, MagicMock()
 
         status = host.get_file(
             "not-a-file",
             "not-another-file",
             print_output=True,
-            sudo=True,
-            sudo_user="ubuntu",
+            _sudo=True,
+            _sudo_user="ubuntu",
         )
 
         assert status is False
 
         fake_ssh_client().exec_command.assert_has_calls(
             [
                 call(
                     (
                         "sudo -H -n -u ubuntu sh -c 'cp not-a-file "
-                        "/tmp/pyinfra-e9c0d3c8ffca943daa0e75511b0a09c84b59c508 && chmod +r not-a-file'"  # noqa
+                        "/tmp/pyinfra-e9c0d3c8ffca943daa0e75511b0a09c84b59c508 && chmod +r /tmp/pyinfra-e9c0d3c8ffca943daa0e75511b0a09c84b59c508'"  # noqa
                     ),
                     get_pty=False,
                 ),
             ],
         )
 
     @patch("pyinfra.connectors.ssh.SSHClient")
@@ -942,26 +901,26 @@
 
         fake_open = mock_open(read_data="test!")
         with patch("pyinfra.api.util.open", fake_open, create=True):
             status = host.get_file(
                 "not-a-file",
                 "not-another-file",
                 print_output=True,
-                sudo=True,
-                sudo_user="ubuntu",
+                _sudo=True,
+                _sudo_user="ubuntu",
             )
 
         assert status is False
 
         fake_ssh_client().exec_command.assert_has_calls(
             [
                 call(
                     (
                         "sudo -H -n -u ubuntu sh -c 'cp not-a-file "
-                        "/tmp/pyinfra-e9c0d3c8ffca943daa0e75511b0a09c84b59c508 && chmod +r not-a-file'"  # noqa
+                        "/tmp/pyinfra-e9c0d3c8ffca943daa0e75511b0a09c84b59c508 && chmod +r /tmp/pyinfra-e9c0d3c8ffca943daa0e75511b0a09c84b59c508'"  # noqa
                     ),
                     get_pty=False,
                 ),
                 call(
                     (
                         "sudo -H -n -u ubuntu sh -c 'rm -f "
                         "/tmp/pyinfra-e9c0d3c8ffca943daa0e75511b0a09c84b59c508'"
@@ -990,26 +949,26 @@
 
         fake_open = mock_open(read_data="test!")
         with patch("pyinfra.api.util.open", fake_open, create=True):
             status = host.get_file(
                 "not-a-file",
                 "not-another-file",
                 print_output=True,
-                su_user="centos",
+                _su_user="centos",
             )
 
         assert status is True
 
         fake_ssh_client().exec_command.assert_has_calls(
             [
                 call(
                     (
                         "su centos -c 'sh -c '\"'\"'cp not-a-file "
                         "/tmp/pyinfra-e9c0d3c8ffca943daa0e75511b0a09c84b59c508 && chmod +r "
-                        "not-a-file'\"'\"''"
+                        "/tmp/pyinfra-e9c0d3c8ffca943daa0e75511b0a09c84b59c508'\"'\"''"
                     ),
                     get_pty=False,
                 ),
                 call(
                     (
                         "su centos -c 'sh -c '\"'\"'rm -f "
                         "/tmp/pyinfra-e9c0d3c8ffca943daa0e75511b0a09c84b59c508'\"'\"''"
@@ -1038,7 +997,59 @@
         with patch("pyinfra.api.util.open", fake_open, create=True):
             with self.assertRaises(ConnectError):
                 host.put_file(
                     "not-a-file",
                     "not-another-file",
                     print_output=True,
                 )
+
+    @patch("pyinfra.connectors.ssh.SSHClient")
+    @patch("time.sleep")
+    def test_ssh_connect_fail_retry(self, fake_sleep, fake_ssh_client):
+        for exception_class in (
+            SSHException,
+            gaierror,
+            socket_error,
+            EOFError,
+        ):
+            inventory = make_inventory(
+                hosts=("unresposivehost",), override_data={"ssh_connect_retries": 1}
+            )
+            State(inventory, Config())
+
+            unresposivehost = inventory.get_host("unresposivehost")
+            assert unresposivehost.data.ssh_connect_retries == 1
+
+            fake_ssh = MagicMock()
+            fake_ssh.connect.side_effect = exception_class()
+            fake_ssh_client.return_value = fake_ssh
+
+            with self.assertRaises(ConnectError):
+                unresposivehost.connect(show_errors=False, raise_exceptions=True)
+            assert fake_sleep.called_once()
+            assert fake_ssh_client.connect.called_twice()
+
+    @patch("pyinfra.connectors.ssh.SSHClient")
+    @patch("time.sleep")
+    def test_ssh_connect_fail_success(self, fake_sleep, fake_ssh_client):
+        for exception_class in (
+            SSHException,
+            gaierror,
+            socket_error,
+            EOFError,
+        ):
+            inventory = make_inventory(
+                hosts=("unresposivehost",), override_data={"ssh_connect_retries": 1}
+            )
+            State(inventory, Config())
+
+            unresposivehost = inventory.get_host("unresposivehost")
+            assert unresposivehost.data.ssh_connect_retries == 1
+
+            connection = MagicMock()
+            fake_ssh = MagicMock()
+            fake_ssh.connect.side_effect = [exception_class(), connection]
+            fake_ssh_client.return_value = fake_ssh
+
+            unresposivehost.connect(show_errors=False, raise_exceptions=True)
+            assert fake_sleep.called_once()
+            assert fake_ssh_client.connect.called_twice()
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_sshuserclient.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_sshuserclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 Include other_file
 """
 
 SSH_CONFIG_OTHER_FILE = """
 Host 192.168.1.1
     User "otheruser"
-    ProxyCommand None
+    # ProxyCommand None # Commented to get test passing with Paramiko > 3
     ForwardAgent yes
     UserKnownHostsFile ~/.ssh/test3
 """
 
 SSH_CONFIG_OTHER_FILE_PROXYJUMP = """
 Host 192.168.1.2
     User "otheruser"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_terraform.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_terraform.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,72 +1,75 @@
 import json
 from unittest import TestCase
 from unittest.mock import patch
 
 from pyinfra.api.exceptions import InventoryError
-from pyinfra.connectors.terraform import make_names_data
+from pyinfra.connectors.terraform import TerraformInventoryConnector
 
 
-class TestVagrantConnector(TestCase):
-    def test_make_names_data_no_output_key(self):
-        with self.assertRaises(InventoryError) as context:
-            list(make_names_data())
-
-        assert context.exception.args[0] == "No Terraform output key!"
-
+class TestTerraformConnector(TestCase):
     @patch("pyinfra.connectors.terraform.local.shell")
     def test_make_names_data_no_output(self, fake_shell):
-        fake_shell.return_value = json.dumps({})
+        fake_shell.return_value = json.dumps(
+            {
+                "hello": {
+                    "world": [],
+                },
+            },
+        )
 
         with self.assertRaises(InventoryError) as context:
-            list(make_names_data("output_key"))
+            list(TerraformInventoryConnector.make_names_data("output_key"))
 
-        assert context.exception.args[0] == "No Terraform output with key: `output_key`"
+        assert (
+            context.exception.args[0]
+            == "No Terraform output with key: `output_key`, valid keys:\n   - hello.world"
+        )
 
     @patch("pyinfra.connectors.terraform.local.shell")
     def test_make_names_data_invalid_output(self, fake_shell):
         fake_shell.return_value = json.dumps({"output_key": "wrongvalue"})
 
         with self.assertRaises(InventoryError) as context:
-            list(make_names_data("output_key"))
+            list(TerraformInventoryConnector.make_names_data("output_key"))
 
         assert (
             context.exception.args[0]
             == "Invalid Terraform output type, should be `list`, got `str`"
         )
 
     @patch("pyinfra.connectors.terraform.local.shell")
     def test_make_names_data_dict_invalid_item(self, fake_shell):
         fake_shell.return_value = json.dumps({"output_key": [None]})
 
         with self.assertRaises(InventoryError) as context:
-            list(make_names_data("output_key"))
+            list(TerraformInventoryConnector.make_names_data("output_key"))
 
         assert (
             context.exception.args[0]
             == "Invalid Terraform list item, should be `dict` or `str` got `NoneType`"
         )
 
     @patch("pyinfra.connectors.terraform.local.shell")
     def test_make_names_data(self, fake_shell):
         fake_shell.return_value = json.dumps({"output_key": ["somehost"]})
-        data = list(make_names_data("output_key"))
+        data = list(TerraformInventoryConnector.make_names_data("output_key"))
 
         assert data == [
             (
                 "@terraform/somehost",
                 {"ssh_hostname": "somehost"},
                 ["@terraform"],
             ),
         ]
 
     @patch("pyinfra.connectors.terraform.local.shell")
     def test_make_names_data_nested(self, fake_shell):
         fake_shell.return_value = json.dumps({"output_key": {"nested_key": ["somehost"]}})
-        data = list(make_names_data("output_key.nested_key"))
+        data = list(TerraformInventoryConnector.make_names_data("output_key.nested_key"))
 
         assert data == [
             (
                 "@terraform/somehost",
                 {"ssh_hostname": "somehost"},
                 ["@terraform"],
             ),
@@ -75,15 +78,15 @@
     @patch("pyinfra.connectors.terraform.local.shell")
     def test_make_names_data_dict(self, fake_shell):
         host = {
             "name": "a name",
             "ssh_hostname": "hostname",
         }
         fake_shell.return_value = json.dumps({"output_key": [host]})
-        data = list(make_names_data("output_key"))
+        data = list(TerraformInventoryConnector.make_names_data("output_key"))
 
         assert data == [
             (
                 "@terraform/a name",
                 {"ssh_hostname": "hostname"},
                 ["@terraform"],
             ),
@@ -93,13 +96,13 @@
     def test_make_names_data_dict_no_name(self, fake_shell):
         host = {
             "not_a_name": "hostname",
         }
         fake_shell.return_value = json.dumps({"output_key": [host]})
 
         with self.assertRaises(InventoryError) as context:
-            list(make_names_data("output_key"))
+            list(TerraformInventoryConnector.make_names_data("output_key"))
 
         assert (
             context.exception.args[0]
             == "Invalid Terraform list item, missing `name` or `ssh_hostname` keys"
         )
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_util.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,134 +1,112 @@
 # encoding: utf-8
 
 from unittest import TestCase
 
 from pyinfra.api import Config, State
-from pyinfra.connectors.util import (
-    make_unix_command,
-    make_unix_command_for_host,
-    split_combined_output,
-)
+from pyinfra.connectors.util import make_unix_command, make_unix_command_for_host
 
 from ..util import make_inventory
 
 
-class TestConnectorUtil(TestCase):
-    def test_split_combined_output_works(self):
-        results = split_combined_output(
-            [
-                ("stdout", "stdout1"),
-                ("stdout", "stdout2"),
-                ("stderr", "stderr1"),
-                ("stdout", "stdout3"),
-            ],
-        )
-
-        assert results == (["stdout1", "stdout2", "stdout3"], ["stderr1"])
-
-    def test_split_combined_output_raises(self):
-        with self.assertRaises(ValueError):
-            split_combined_output(["nope", ""])
-
-
 class TestMakeUnixCommandConnectorUtil(TestCase):
     def test_command(self):
         command = make_unix_command("echo Šablony")
         assert command.get_raw_value() == "sh -c 'echo Šablony'"
 
     def test_doas_command(self):
-        command = make_unix_command("uptime", doas=True)
+        command = make_unix_command("uptime", _doas=True)
         assert command.get_raw_value() == "doas -n sh -c uptime"
 
     def test_doas_user_command(self):
-        command = make_unix_command("uptime", doas=True, doas_user="pyinfra")
+        command = make_unix_command("uptime", _doas=True, _doas_user="pyinfra")
         assert command.get_raw_value() == "doas -n -u pyinfra sh -c uptime"
 
     def test_sudo_command(self):
-        command = make_unix_command("uptime", sudo=True)
+        command = make_unix_command("uptime", _sudo=True)
         assert command.get_raw_value() == "sudo -H -n sh -c uptime"
 
     def test_sudo_multi_arg_command(self):
-        command = make_unix_command("echo hi", sudo=True, preserve_sudo_env=True)
+        command = make_unix_command("echo hi", _sudo=True, _preserve_sudo_env=True)
         assert command.get_raw_value() == "sudo -H -n -E sh -c 'echo hi'"
 
     def test_sudo_preserve_env_command(self):
-        command = make_unix_command("uptime", sudo=True, preserve_sudo_env=True)
+        command = make_unix_command("uptime", _sudo=True, _preserve_sudo_env=True)
         assert command.get_raw_value() == "sudo -H -n -E sh -c uptime"
 
     def test_use_sudo_login_command(self):
-        command = make_unix_command("uptime", sudo=True, use_sudo_login=True)
+        command = make_unix_command("uptime", _sudo=True, _use_sudo_login=True)
         assert command.get_raw_value() == "sudo -H -n -i sh -c uptime"
 
     def test_sudo_user_command(self):
-        command = make_unix_command("uptime", sudo=True, sudo_user="pyinfra")
+        command = make_unix_command("uptime", _sudo=True, _sudo_user="pyinfra")
         assert command.get_raw_value() == "sudo -H -n -u pyinfra sh -c uptime"
 
     def test_su_command(self):
-        command = make_unix_command("uptime", su_user="pyinfra")
+        command = make_unix_command("uptime", _su_user="pyinfra")
         assert command.get_raw_value() == "su pyinfra -c 'sh -c uptime'"
 
     def test_su_multi_arg_command(self):
-        command = make_unix_command("echo hi", su_user="pyinfra")
+        command = make_unix_command("echo hi", _su_user="pyinfra")
         assert command.get_raw_value() == "su pyinfra -c 'sh -c '\"'\"'echo hi'\"'\"''"
 
     def test_use_su_login_command(self):
-        command = make_unix_command("uptime", su_user="pyinfra", use_su_login=True)
+        command = make_unix_command("uptime", _su_user="pyinfra", _use_su_login=True)
         assert command.get_raw_value() == "su -l pyinfra -c 'sh -c uptime'"
 
     def test_preserve_su_env_command(self):
-        command = make_unix_command("uptime", su_user="pyinfra", preserve_su_env=True)
+        command = make_unix_command("uptime", _su_user="pyinfra", _preserve_su_env=True)
         assert command.get_raw_value() == "su -m pyinfra -c 'sh -c uptime'"
 
     def test_su_shell_command(self):
-        command = make_unix_command("uptime", su_user="pyinfra", su_shell="bash")
+        command = make_unix_command("uptime", _su_user="pyinfra", _su_shell="bash")
         assert command.get_raw_value() == "su -s `which bash` pyinfra -c 'sh -c uptime'"
 
     def test_command_env(self):
         command = make_unix_command(
             "uptime",
-            env={
+            _env={
                 "key": "value",
                 "anotherkey": "anothervalue",
             },
         )
         assert command.get_raw_value() in [
             'sh -c \'export "key=value" "anotherkey=anothervalue" && uptime\'',
             'sh -c \'export "anotherkey=anothervalue" "key=value" && uptime\'',
         ]
 
     def test_command_chdir(self):
-        command = make_unix_command("uptime", chdir="/opt/somedir")
+        command = make_unix_command("uptime", _chdir="/opt/somedir")
         assert command.get_raw_value() == "sh -c 'cd /opt/somedir && uptime'"
 
     def test_custom_shell_command(self):
-        command = make_unix_command("uptime", shell_executable="bash")
+        command = make_unix_command("uptime", _shell_executable="bash")
         assert command.get_raw_value() == "bash -c uptime"
 
     def test_mixed_command(self):
         command = make_unix_command(
             "echo hi",
-            chdir="/opt/somedir",
-            env={"key": "value"},
-            sudo=True,
-            sudo_user="root",
-            preserve_sudo_env=True,
-            su_user="pyinfra",
-            shell_executable="bash",
+            _chdir="/opt/somedir",
+            _env={"key": "value"},
+            _sudo=True,
+            _sudo_user="root",
+            _preserve_sudo_env=True,
+            _su_user="pyinfra",
+            _shell_executable="bash",
         )
         assert command.get_raw_value() == (
             "sudo -H -n -E -u root "  # sudo bit
             "su pyinfra -c "  # su bit
             "'bash -c '\"'\"'cd /opt/somedir && export \"key=value\" "  # shell and export bit
             "&& echo hi'\"'\"''"  # command bit
         )
 
     def test_command_exists_su_config_only(self):
         """
         This tests covers a bug that appeared when `make_unix_command` is called
-        with `su_user=False` (default) but `SU_USER` set on the config object,
+        with `_su_user=False` (default) but `SU_USER` set on the config object,
         resulting in an empty command output.
         """
         state = State(make_inventory(), Config(SU_USER=True))
         host = state.inventory.get_host("somehost")
         command = make_unix_command_for_host(state, host, "echo Šablony")
         assert command.get_raw_value() == "sh -c 'echo Šablony'"
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_connectors/test_vagrant.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_connectors/test_vagrant.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from unittest import TestCase
 from unittest.mock import mock_open, patch
 
 from pyinfra.api.exceptions import InventoryError
-from pyinfra.connectors.vagrant import get_vagrant_options, make_names_data
+from pyinfra.connectors.vagrant import VagrantInventoryConnector, get_vagrant_options
 
 FAKE_VAGRANT_OPTIONS = {
     "groups": {
         "ubuntu16": ["mygroup"],
     },
     "data": {
         "centos7": {
@@ -65,15 +65,15 @@
     @patch(
         "pyinfra.connectors.vagrant.open",
         mock_open(read_data=FAKE_VAGRANT_OPTIONS_DATA),
         create=True,
     )
     @patch("pyinfra.connectors.vagrant.path.exists", lambda path: True)
     def test_make_names_data_with_options(self):
-        data = make_names_data()
+        data = list(VagrantInventoryConnector.make_names_data())
 
         assert data == [
             (
                 "@vagrant/ubuntu16",
                 {
                     "ssh_port": "2222",
                     "ssh_user": "vagrant",
@@ -99,15 +99,15 @@
                     "ssh_hostname": "127.0.0.1",
                 },
                 ["@vagrant"],
             ),
         ]
 
     def test_make_names_data_with_limit(self):
-        data = make_names_data(limit=("ubuntu16",))
+        data = list(VagrantInventoryConnector.make_names_data(name=("ubuntu16",)))
 
         assert data == [
             (
                 "@vagrant/ubuntu16",
                 {
                     "ssh_port": "2222",
                     "ssh_user": "vagrant",
@@ -116,8 +116,8 @@
                 },
                 ["@vagrant"],
             ),
         ]
 
     def test_make_names_data_no_matches(self):
         with self.assertRaises(InventoryError):
-            make_names_data(limit="nope")
+            list(VagrantInventoryConnector.make_names_data(name="nope"))
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_facts.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_facts.py`

 * *Files identical despite different names*

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_global_arguments.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_global_arguments.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 try:
     from inspect import getfullargspec
 except ImportError:
     from inspect import signature as getfullargspec
 
 from pyinfra import operations
-from pyinfra.api.arguments import ALL_ARGUMENTS
+from pyinfra.api.arguments import all_argument_meta
 
 
 def _is_pyinfra_operation(module, key, value):
     return (
         isinstance(value, FunctionType)
         and value.__module__ == module.__name__
         and getattr(value, "_pyinfra_op", False)
@@ -37,15 +37,15 @@
         for key, value in sorted(getmembers(module)):
             if _is_pyinfra_operation(module, key, value):
                 yield module, value
 
 
 class TestOperationGlobalArguments(TestCase):
     def test_operations_do_not_use_global_arguments(self):
-        global_arg_keys = ALL_ARGUMENTS.keys()
+        global_arg_keys = all_argument_meta.keys()
 
         for op_module, op_func in iter_operations():
             argspec = getfullargspec(op_func._pyinfra_op)
             for arg in argspec.args:
                 assert (
                     arg not in global_arg_keys
                 ), "`{0}` argument found in {1}.{2} operation function".format(
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_operations.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_operations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import platform
 import warnings
 from importlib import import_module
 from os import listdir, path
 from unittest import TestCase
-from unittest.mock import MagicMock, patch
+from unittest.mock import patch
 
 from pyinfra.api import FileDownloadCommand, FileUploadCommand, FunctionCommand, StringCommand
 from pyinfra.context import ctx_host, ctx_state
 from pyinfra_cli.util import json_encode
 
 from .util import FakeState, JsonTest, create_host, get_command_string, parse_value, patch_files
 
@@ -39,27 +39,29 @@
                 command.kwargs,
             ]
 
         elif isinstance(command, FileUploadCommand):
             if hasattr(command.src, "read"):
                 command.src.seek(0)
                 data = command.src.read()
+                if isinstance(data, bytes):
+                    data = data.decode()
             else:
                 data = str(command.src)
             json_command = ["upload", data, str(command.dest)]
 
         elif isinstance(command, FileDownloadCommand):
             json_command = ["download", str(command.src), str(command.dest)]
 
         else:
             raise Exception("{0} is not a valid command!".format(command))
 
-        if command.executor_kwargs:
-            command.executor_kwargs["command"] = json_command
-            json_command = command.executor_kwargs
+        if command.connector_arguments:
+            command.connector_arguments["command"] = json_command
+            json_command = command.connector_arguments
 
         json_commands.append(json_command)
     return json_commands
 
 
 def assert_commands(commands, wanted_commands):
     try:
@@ -86,15 +88,14 @@
     module_name, op_name = arg.split(".")
     module = import_module("pyinfra.operations.{0}".format(module_name))
     op = getattr(module, op_name)
 
     # Generate a test class
     @patch("pyinfra.operations.files.get_timestamp", lambda: "a-timestamp")
     @patch("pyinfra.operations.util.files.get_timestamp", lambda: "a-timestamp")
-    @patch("pyinfra.operations.python.getfullargspec", lambda x: MagicMock())
     class TestTests(TestCase, metaclass=JsonTest):
         jsontest_files = path.join("tests", "operations", arg)
         jsontest_prefix = "test_{0}_{1}_".format(module_name, op_name)
 
         @classmethod
         def setUpClass(cls):
             # Create a global fake state that attach to context state
@@ -117,15 +118,15 @@
             args = parse_value(test_data.get("args", []))
             kwargs = parse_value(test_data.get("kwargs", {}))
 
             with ctx_state.use(self.state):
                 with ctx_host.use(host):
                     with patch_files(test_data.get("local_files", {})):
                         try:
-                            output_commands = list(op._pyinfra_op(*args, **kwargs))
+                            output_commands = list(op._inner(*args, **kwargs))
                         except Exception as e:
                             if allowed_exception:
                                 allowed_exception_names = allowed_exception.get("names")
                                 if not allowed_exception_names:
                                     allowed_exception_names = [allowed_exception["name"]]
 
                                 if e.__class__.__name__ not in allowed_exception_names:
@@ -133,62 +134,17 @@
                                     raise
 
                                 assert e.args[0] == allowed_exception["message"]
                                 return
 
                             raise
 
-                        op_is_idempotent = getattr(op._pyinfra_op, "is_idempotent", True)
-                        second_output_commands = []
-                        test_second_output_commands = "second_output_commands" in test_data
-
-                        if op_is_idempotent or test_second_output_commands:
-                            second_output_commands = list(op._pyinfra_op(*args, **kwargs))
-
-            if op_is_idempotent:
-                if test_data.get("idempotent", True):
-                    if second_output_commands:
-                        raise Exception(
-                            "Operation not idempotent, second output commands: {0}".format(
-                                second_output_commands,
-                            ),
-                        )
-                else:
-                    if not second_output_commands:
-                        raise Exception(
-                            (
-                                "Operation tests as idempotent but test " "says it is not: {0}"
-                            ).format(op_test_name),
-                        )
-                    if not test_data.get("disable_idempotent_warning_reason"):
-                        warnings.warn(
-                            (
-                                "This operation should be idempotent, but the test has "
-                                "disabled this check without reason: {0}"
-                            ).format(op_test_name),
-                        )
-
-            if op_is_idempotent is False:
-                if "disable_idempotent_warning_reason" in test_data:
-                    warnings.warn(
-                        (
-                            "This operation is not idempotent and so the test does not need "
-                            "`disable_idempotent_warning_reason` set: {0}"
-                        ).format(op_test_name),
-                    )
-
             commands = parse_commands(output_commands)
             assert_commands(commands, test_data["commands"])
 
-            if test_second_output_commands:
-                assert_commands(
-                    parse_commands(second_output_commands),
-                    test_data["second_output_commands"],
-                )
-
             noop_description = test_data.get("noop_description")
             if len(commands) == 0 or noop_description:
                 if noop_description is not None:
                     assert host.noop_description == noop_description
                 else:
                     assert host.noop_description is not None, "no noop description was set"
                     warnings.warn(
```

### Comparing `pyinfra_forked_by_stone-w4tch3r-0.1.1/tests/test_operations_utils.py` & `pyinfra_forked_by_stone-w4tch3r-0.3.0/tests/test_operations_utils.py`

 * *Files identical despite different names*

