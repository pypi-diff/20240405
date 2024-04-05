# Comparing `tmp/stix2-validator-3.1.4.tar.gz` & `tmp/stix2-validator-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stix2-validator-3.1.4.tar", last modified: Tue Jul 25 21:50:12 2023, max compression
+gzip compressed data, was "stix2-validator-3.2.0.tar", last modified: Fri Apr  5 16:02:19 2024, max compression
```

## Comparing `stix2-validator-3.1.4.tar` & `stix2-validator-3.2.0.tar`

### file list

```diff
@@ -1,194 +1,220 @@
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1490 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/LICENSE
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)       49 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/MANIFEST.in
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9556 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/PKG-INFO
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     8377 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/README.rst
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      246 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/setup.cfg
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2406 2023-07-25 21:19:00.000000 stix2-validator-3.1.4/setup.py
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.624168 stix2-validator-3.1.4/stix2_validator.egg-info/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9556 2023-07-25 21:50:12.000000 stix2-validator-3.1.4/stix2_validator.egg-info/PKG-INFO
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9022 2023-07-25 21:50:12.000000 stix2-validator-3.1.4/stix2_validator.egg-info/SOURCES.txt
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        1 2023-07-25 21:50:12.000000 stix2-validator-3.1.4/stix2_validator.egg-info/dependency_links.txt
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)       81 2023-07-25 21:50:12.000000 stix2-validator-3.1.4/stix2_validator.egg-info/entry_points.txt
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      233 2023-07-25 21:50:12.000000 stix2-validator-3.1.4/stix2_validator.egg-info/requires.txt
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)       15 2023-07-25 21:50:12.000000 stix2-validator-3.1.4/stix2_validator.egg-info/top_level.txt
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.624168 stix2-validator-3.1.4/stix2validator/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      443 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/__init__.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1196 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/codes.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    13748 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/errors.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     5452 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/output.py
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.620169 stix2-validator-3.1.4/stix2validator/schemas-2.0/
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.624168 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      523 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/indicator-for-c2-ip-address.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1080 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/indicator-to-campaign-relationship.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4163 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/indicators-for-C2-with-COA.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3310 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/malicious-email-indicator-with-attachment.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.624168 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/threat-reports/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    49449 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/threat-reports/apt1.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    83654 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/threat-reports/poisonivy.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.620169 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.624168 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      695 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/binary.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3829 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/bundle.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4256 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/core.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1486 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/cyber-observable-core.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      781 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/dictionary.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2685 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/external-reference.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1186 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/granular-marking.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3058 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/hashes-type.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      616 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/hex.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      557 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/identifier.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      621 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/kill-chain-phase.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     7324 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/marking-definition.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      510 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/timestamp.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      914 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/url-regex.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.628168 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2220 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/artifact.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1215 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/autonomous-system.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1817 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/directory.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1113 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/domain-name.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1310 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/email-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     6068 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/email-message.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    23160 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/file.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1442 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/ipv4-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1467 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/ipv6-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      895 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/mac-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      785 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/mutex.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    11980 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/network-traffic.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9651 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/process.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2023 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/software.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      786 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/url.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     5371 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/user-account.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2801 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/windows-registry-key.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     8407 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/x509-certificate.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.628168 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1444 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/attack-pattern.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1906 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/campaign.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1184 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/course-of-action.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3071 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/identity.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2512 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/indicator.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3195 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/intrusion-set.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2298 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/malware.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4486 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/observed-data.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2276 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/report.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4798 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/threat-actor.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1986 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/tool.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1112 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/vulnerability.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.628168 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sros/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1963 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sros/relationship.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3227 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sros/sighting.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.620169 stix2-validator-3.1.4/stix2validator/schemas-2.1/
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.628168 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      619 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/indicator-for-c2-ip-address.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1250 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/indicator-to-campaign-relationship.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4640 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/indicators-for-C2-with-COA.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4019 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/infrastructure.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      620 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/interop-objectmarking-test.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3517 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/malicious-email-indicator-with-attachment.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.628168 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/threat-reports/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    52903 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/threat-reports/apt1.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    89906 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/threat-reports/poisonivy.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.628168 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      443 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/attack-pattern.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      369 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/campaign.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1196 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/core.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      430 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/course-of-action.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      369 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/grouping.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      414 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/indicator.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      413 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/infrastructure.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      435 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/intrusion-set.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      387 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/location.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      497 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/malware-analysis.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      594 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/malware.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      361 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/note.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      411 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/observed-data.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      367 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/opinion.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      377 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/relationship.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      389 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/report.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      429 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/sighting.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      506 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/threat-actor.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      383 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/tool.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      411 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/vulnerability.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.620169 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.632168 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      695 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/binary.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     6457 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/bundle.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4453 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/core.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2835 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/cyber-observable-core.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      805 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/dictionary.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2749 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/extension-definition.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      701 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/extension.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2879 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/external-reference.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1318 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/granular-marking.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1928 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/hashes-type.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      616 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/hex.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      558 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/identifier.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      621 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/kill-chain-phase.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1615 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/language-content.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     9274 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/marking-definition.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      861 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/properties.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      510 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/timestamp.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      301 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/url-regex.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.632168 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3473 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/artifact.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1311 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/autonomous-system.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1898 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/directory.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1228 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/domain-name.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1352 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/email-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     6417 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/email-message.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    21461 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/file.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1691 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/ipv4-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2612 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/ipv6-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      982 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/mac-addr.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      869 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/mutex.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    11490 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/network-traffic.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    10028 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/process.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2282 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/software.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      868 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/url.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     6435 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/user-account.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3198 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/windows-registry-key.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     8502 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/x509-certificate.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1653 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/attack-pattern.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1906 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/campaign.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1184 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/course-of-action.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1773 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/grouping.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3212 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/identity.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1044 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/incident.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2960 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/indicator.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2730 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/infrastructure.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3195 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/intrusion-set.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4342 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/location.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     5179 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/malware-analysis.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     7319 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/malware.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1627 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/note.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     4861 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/observed-data.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1901 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/opinion.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2266 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/report.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     5125 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/threat-actor.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2218 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/tool.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1112 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/vulnerability.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sros/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     2839 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sros/relationship.json
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     3575 2023-07-25 21:14:46.000000 stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sros/sighting.json
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/stix2validator/scripts/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/scripts/__init__.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1246 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/scripts/stix2_validator.py
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/stix2validator/test/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/test/__init__.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    23562 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/util.py
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/stix2validator/v20/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v20/__init__.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    38942 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v20/enums.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      838 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v20/errors.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    19956 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v20/musts.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    68155 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v20/shoulds.py
-drwxrwxr-x   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 21:50:12.636168 stix2-validator-3.1.4/stix2validator/v21/
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)        0 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v21/__init__.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    65038 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v21/enums.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)      838 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v21/errors.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)     1469 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v21/interop.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    26496 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v21/musts.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    78565 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/v21/shoulds.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)    32589 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/validator.py
--rw-rw-r--   0 ratliff   (1000) ratliff   (1000)       22 2023-07-25 20:57:48.000000 stix2-validator-3.1.4/stix2validator/version.py
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:19.132401 stix2-validator-3.2.0/
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1490 2020-05-04 21:05:14.000000 stix2-validator-3.2.0/LICENSE
+-rw-rw-r--   0 lu        (1000) lu        (1001)      151 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/MANIFEST.in
+-rw-rw-r--   0 lu        (1000) lu        (1001)    11058 2024-04-05 16:02:19.140404 stix2-validator-3.2.0/PKG-INFO
+-rw-rw-r--   0 lu        (1000) lu        (1001)     8366 2024-04-03 14:33:37.000000 stix2-validator-3.2.0/README.rst
+-rw-rw-r--   0 lu        (1000) lu        (1001)      246 2024-04-05 16:02:19.148407 stix2-validator-3.2.0/setup.cfg
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2437 2024-04-05 14:12:09.000000 stix2-validator-3.2.0/setup.py
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.580212 stix2-validator-3.2.0/stix2_validator.egg-info/
+-rw-r--r--   0 lu        (1000) lu        (1001)    11058 2024-04-05 16:02:18.000000 stix2-validator-3.2.0/stix2_validator.egg-info/PKG-INFO
+-rw-rw-r--   0 lu        (1000) lu        (1001)    10142 2024-04-05 16:02:18.000000 stix2-validator-3.2.0/stix2_validator.egg-info/SOURCES.txt
+-rw-rw-r--   0 lu        (1000) lu        (1001)        1 2024-04-05 16:02:18.000000 stix2-validator-3.2.0/stix2_validator.egg-info/dependency_links.txt
+-rw-rw-r--   0 lu        (1000) lu        (1001)       81 2024-04-05 16:02:18.000000 stix2-validator-3.2.0/stix2_validator.egg-info/entry_points.txt
+-rw-rw-r--   0 lu        (1000) lu        (1001)      212 2024-04-05 16:02:18.000000 stix2-validator-3.2.0/stix2_validator.egg-info/requires.txt
+-rw-rw-r--   0 lu        (1000) lu        (1001)       15 2024-04-05 16:02:18.000000 stix2-validator-3.2.0/stix2_validator.egg-info/top_level.txt
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.596217 stix2-validator-3.2.0/stix2validator/
+-rw-rw-r--   0 lu        (1000) lu        (1001)      443 2020-05-04 21:05:14.000000 stix2-validator-3.2.0/stix2validator/__init__.py
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1196 2020-05-04 21:05:14.000000 stix2-validator-3.2.0/stix2validator/codes.py
+-rw-rw-r--   0 lu        (1000) lu        (1001)    13748 2022-12-08 20:46:21.000000 stix2-validator-3.2.0/stix2validator/errors.py
+-rw-rw-r--   0 lu        (1000) lu        (1001)     5452 2022-12-08 20:46:21.000000 stix2-validator-3.2.0/stix2validator/output.py
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.532196 stix2-validator-3.2.0/stix2validator/schemas-2.0/
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.616224 stix2-validator-3.2.0/stix2validator/schemas-2.0/examples/
+-rw-rw-r--   0 lu        (1000) lu        (1001)      523 2020-06-03 18:49:17.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/examples/indicator-for-c2-ip-address.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1080 2020-06-03 18:49:17.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/examples/indicator-to-campaign-relationship.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     4163 2020-06-03 18:49:17.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/examples/indicators-for-C2-with-COA.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     3310 2020-06-03 18:49:17.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/examples/malicious-email-indicator-with-attachment.json
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.620226 stix2-validator-3.2.0/stix2validator/schemas-2.0/examples/threat-reports/
+-rw-rw-r--   0 lu        (1000) lu        (1001)    49449 2020-06-03 18:49:17.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/examples/threat-reports/apt1.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)    83654 2020-06-03 18:49:17.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/examples/threat-reports/poisonivy.json
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.532196 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.656238 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/
+-rw-rw-r--   0 lu        (1000) lu        (1001)      695 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/binary.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     3829 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/bundle.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     4256 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/core.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1486 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/cyber-observable-core.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      781 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/dictionary.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2685 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/external-reference.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1186 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/granular-marking.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     3058 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/hashes-type.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      616 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/hex.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      557 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/identifier.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      621 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/kill-chain-phase.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     7324 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/marking-definition.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      510 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/timestamp.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      914 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/url-regex.json
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.704254 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2220 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/artifact.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1215 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/autonomous-system.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1817 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/directory.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1113 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/domain-name.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1310 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/email-addr.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     6068 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/email-message.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)    23160 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/file.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1442 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/ipv4-addr.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1467 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/ipv6-addr.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      895 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/mac-addr.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      785 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/mutex.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)    11980 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/network-traffic.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     9651 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/process.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2023 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/software.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      786 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/url.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     5371 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/user-account.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2801 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/windows-registry-key.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     8407 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/x509-certificate.json
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.728263 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1444 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/attack-pattern.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1906 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/campaign.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1184 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/course-of-action.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     3071 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/identity.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2512 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/indicator.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     3195 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/intrusion-set.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2298 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/malware.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     4486 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/observed-data.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2276 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/report.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     4798 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/threat-actor.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1986 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/tool.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1112 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/vulnerability.json
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.728263 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sros/
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1963 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sros/relationship.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     3227 2024-04-04 20:12:52.000000 stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sros/sighting.json
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.540198 stix2-validator-3.2.0/stix2validator/schemas-2.1/
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.748270 stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/
+-rw-rw-r--   0 lu        (1000) lu        (1001)      619 2021-05-23 01:00:23.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/indicator-for-c2-ip-address.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1250 2021-05-23 01:00:23.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/indicator-to-campaign-relationship.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     4640 2021-05-23 01:00:23.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/indicators-for-C2-with-COA.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     4019 2021-05-23 01:00:23.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/infrastructure.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      620 2022-08-08 15:24:06.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/interop-objectmarking-test.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     3517 2022-08-02 14:57:11.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/malicious-email-indicator-with-attachment.json
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.748270 stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/threat-reports/
+-rw-rw-r--   0 lu        (1000) lu        (1001)    52903 2021-05-23 01:00:23.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/threat-reports/apt1.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)    89906 2021-05-23 01:00:23.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/threat-reports/poisonivy.json
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.800288 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/
+-rw-rw-r--   0 lu        (1000) lu        (1001)      443 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/attack-pattern.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      369 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/campaign.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1196 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/core.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      430 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/course-of-action.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      369 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/grouping.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      414 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/indicator.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      413 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/infrastructure.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      435 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/intrusion-set.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      387 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/location.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      497 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/malware-analysis.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      594 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/malware.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      361 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/note.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      411 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/observed-data.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      367 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/opinion.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      377 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/relationship.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      389 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/report.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      429 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/sighting.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      506 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/threat-actor.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      383 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/tool.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      411 2024-03-27 17:48:55.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/vulnerability.json
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.544200 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.836300 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/
+-rw-rw-r--   0 lu        (1000) lu        (1001)      695 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/binary.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     6457 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/bundle.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     4646 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/core.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2835 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/cyber-observable-core.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      805 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/dictionary.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2749 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/extension-definition.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      701 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/extension.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2879 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/external-reference.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1318 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/granular-marking.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1928 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/hashes-type.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      616 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/hex.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      558 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/identifier.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      621 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/kill-chain-phase.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1615 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/language-content.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     9274 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/marking-definition.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      861 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/properties.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      510 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/timestamp.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      301 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/url-regex.json
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.896320 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/
+-rw-rw-r--   0 lu        (1000) lu        (1001)     3473 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/artifact.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1311 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/autonomous-system.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1898 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/directory.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1228 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/domain-name.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1352 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/email-addr.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     6417 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/email-message.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)    21461 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/file.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1691 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/ipv4-addr.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2612 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/ipv6-addr.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      982 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/mac-addr.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      869 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/mutex.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)    11576 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/network-traffic.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)    10028 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/process.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2282 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/software.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)      868 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/url.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     6435 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/user-account.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     3198 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/windows-registry-key.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     8502 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/x509-certificate.json
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.984351 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1653 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/attack-pattern.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1906 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/campaign.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1184 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/course-of-action.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1773 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/grouping.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     3212 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/identity.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1044 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/incident.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2960 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/indicator.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2730 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/infrastructure.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     3195 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/intrusion-set.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     4342 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/location.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     5179 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/malware-analysis.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     7319 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/malware.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1627 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/note.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     4861 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/observed-data.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1901 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/opinion.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2266 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/report.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     5125 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/threat-actor.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2218 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/tool.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1112 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/vulnerability.json
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.984351 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sros/
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2839 2024-04-04 20:13:48.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sros/relationship.json
+-rw-rw-r--   0 lu        (1000) lu        (1001)     3575 2024-03-25 20:03:54.000000 stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sros/sighting.json
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.988352 stix2-validator-3.2.0/stix2validator/scripts/
+-rw-rw-r--   0 lu        (1000) lu        (1001)        0 2020-05-04 21:05:14.000000 stix2-validator-3.2.0/stix2validator/scripts/__init__.py
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1281 2024-04-03 14:33:37.000000 stix2-validator-3.2.0/stix2validator/scripts/stix2_validator.py
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:18.996355 stix2-validator-3.2.0/stix2validator/test/
+-rw-rw-r--   0 lu        (1000) lu        (1001)        0 2020-05-04 21:05:14.000000 stix2-validator-3.2.0/stix2validator/test/__init__.py
+-rw-rw-r--   0 lu        (1000) lu        (1001)    21748 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/util.py
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:19.012360 stix2-validator-3.2.0/stix2validator/v20/
+-rw-rw-r--   0 lu        (1000) lu        (1001)        0 2020-05-04 21:05:14.000000 stix2-validator-3.2.0/stix2validator/v20/__init__.py
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:19.044371 stix2-validator-3.2.0/stix2validator/v20/assets/
+-rw-rw-r--   0 lu        (1000) lu        (1001)    40692 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v20/assets/charsets.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)   190594 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v20/assets/ipfix-information-elements.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)   113072 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v20/assets/mediatype_application.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)     6347 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v20/assets/mediatype_audio.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)      191 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v20/assets/mediatype_font.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)     3757 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v20/assets/mediatype_image.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1210 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v20/assets/mediatype_message.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2126 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v20/assets/mediatype_model.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)      742 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v20/assets/mediatype_multipart.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)     4362 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v20/assets/mediatype_text.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)     4142 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v20/assets/mediatype_video.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)  1143972 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v20/assets/protocols.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)    38004 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v20/enums.py
+-rw-rw-r--   0 lu        (1000) lu        (1001)      838 2020-05-04 21:05:14.000000 stix2-validator-3.2.0/stix2validator/v20/errors.py
+-rw-rw-r--   0 lu        (1000) lu        (1001)    19956 2020-10-07 20:33:16.000000 stix2-validator-3.2.0/stix2validator/v20/musts.py
+-rw-rw-r--   0 lu        (1000) lu        (1001)    68155 2020-10-07 20:33:16.000000 stix2-validator-3.2.0/stix2validator/v20/shoulds.py
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:19.072381 stix2-validator-3.2.0/stix2validator/v21/
+-rw-rw-r--   0 lu        (1000) lu        (1001)        0 2020-05-04 21:05:14.000000 stix2-validator-3.2.0/stix2validator/v21/__init__.py
+drwxrwxr-x   0 lu        (1000) lu        (1001)        0 2024-04-05 16:02:19.116396 stix2-validator-3.2.0/stix2validator/v21/assets/
+-rw-rw-r--   0 lu        (1000) lu        (1001)    40692 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v21/assets/charsets.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)   190594 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v21/assets/ipfix-information-elements.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)   113072 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v21/assets/mediatype_application.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)     6347 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v21/assets/mediatype_audio.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)      191 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v21/assets/mediatype_font.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)     3757 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v21/assets/mediatype_image.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1210 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v21/assets/mediatype_message.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)     2126 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v21/assets/mediatype_model.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)      742 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v21/assets/mediatype_multipart.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)     4362 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v21/assets/mediatype_text.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)     4142 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v21/assets/mediatype_video.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)  1143972 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v21/assets/protocols.csv
+-rw-rw-r--   0 lu        (1000) lu        (1001)    64098 2024-02-21 22:30:27.000000 stix2-validator-3.2.0/stix2validator/v21/enums.py
+-rw-rw-r--   0 lu        (1000) lu        (1001)      838 2020-05-04 21:05:14.000000 stix2-validator-3.2.0/stix2validator/v21/errors.py
+-rw-rw-r--   0 lu        (1000) lu        (1001)     1469 2022-11-08 18:58:55.000000 stix2-validator-3.2.0/stix2validator/v21/interop.py
+-rw-rw-r--   0 lu        (1000) lu        (1001)    26496 2022-06-16 00:54:33.000000 stix2-validator-3.2.0/stix2validator/v21/musts.py
+-rw-rw-r--   0 lu        (1000) lu        (1001)    78565 2022-05-24 05:07:51.000000 stix2-validator-3.2.0/stix2validator/v21/shoulds.py
+-rw-rw-r--   0 lu        (1000) lu        (1001)    34083 2024-04-05 14:12:09.000000 stix2-validator-3.2.0/stix2validator/validator.py
+-rw-rw-r--   0 lu        (1000) lu        (1001)       22 2024-04-03 14:33:37.000000 stix2-validator-3.2.0/stix2validator/version.py
```

### Comparing `stix2-validator-3.1.4/LICENSE` & `stix2-validator-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/PKG-INFO` & `stix2-validator-3.2.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: stix2-validator
-Version: 3.1.4
-Summary: APIs and scripts for validating STIX 2.x documents.
-Home-page: https://github.com/oasis-open/cti-stix-validator
-Author: OASIS Cyber Threat Intelligence Technical Committee
-Author-email: cti-users@lists.oasis-open.org
-Maintainer: Chris Lenk
-Maintainer-email: clenk@mitre.org
-License: UNKNOWN
-Project-URL: Documentation, https://stix2-validator.readthedocs.io/
-Project-URL: Source Code, https://github.com/oasis-open/cti-stix-validator/
-Project-URL: Bug Tracker, https://github.com/oasis-open/cti-stix-validator/issues/
-Keywords: stix stix2 json validation validator stix-validator stix2-validator
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Topic :: Security
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: test
-License-File: LICENSE
-
 |Build_Status|  |Coverage|  |Version|  |Documentation_Status|
 
 ====================
 `cti-stix-validator`
 ====================
 NOTE: This is an `OASIS TC Open Repository <https://www.oasis-
 open.org/resources/open-repositories/>`__. See the `Governance`_
@@ -169,16 +140,17 @@
 .. _currentMaintainers:
 
 **Current Maintainers of this TC Open Repository**
 
 .. Initial Maintainers: Greg Back & Ivan Kirillov & Chris Lenk
 
 * `Emily Ratliff <mailto:emily.ratliff@ibm.com>`__; GitHub ID: `https://github.com/ejratl <https://github.com/ejratl>`_; WWW: `IBM <http://www.ibm.com/>`__
-* `Duncan Sparrell <mailto:duncan@sfractal.com>`__; GitHub ID: `https://github.com/sparrell <https://github.com/sparrell>`_; WWW: `sFractal <http://sfractal.com/>`__
 *  `Jason Keirstead <mailto:Jason.Keirstead@ca.ibm.com>`__; GitHub ID: `https://github.com/JasonKeirstead <https://github.com/JasonKeirstead>`_; WWW: `IBM <http://www.ibm.com/>`__
+* `Rich Piazza <mailto:rpiazza@mitre.org>`_; GitHub ID: `https://github.com/rpiazza <https://github.com/rpiazza>`_; WWW: `MITRE <http://www.mitre.org/>`_
+
 
 .. _aboutOpenRepos:
 
 `About OASIS TC Open Repositories`
 ==================================
 *  `TC Open Repositories: Overview and Resources <https://www.oasis-open.org/resources/open-repositories/>`_
 *  `Frequently Asked Questions <https://www.oasis-open.org/resources/open-repositories/faq>`_
@@ -206,9 +178,7 @@
    :target: https://codecov.io/gh/oasis-open/cti-stix-validator
 .. |Version| image:: https://img.shields.io/pypi/v/stix2-validator.svg?maxAge=3600
    :target: https://pypi.python.org/pypi/stix2-validator/
 .. |Documentation_Status| image:: https://readthedocs.org/projects/stix2-validator/badge/?version=latest
    :target: https://stix2-validator.readthedocs.io/en/latest/
    :alt: Documentation Status
 
-
-
```

### Comparing `stix2-validator-3.1.4/setup.py` & `stix2-validator-3.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,19 @@
             if line.startswith("__version__"):
                 version = line.split()[-1].strip('"')
                 return version
         raise AttributeError("Package does not have a __version__")
 
 
 install_requires = [
-    'appdirs',
     'colorama',
     'cpe',
-    'jsonschema[format-nongpl]>=4.6.0,<4.18.0',
+    'jsonschema[format-nongpl]>=4.20.0',
     'python-dateutil',
     'requests',
-    'requests_cache',
     'simplejson',
     'stix2-patterns>=0.4.1',
 ]
 
 setup(
     name='stix2-validator',
     version=get_version(),
@@ -40,18 +38,19 @@
     maintainer='Chris Lenk',
     maintainer_email='clenk@mitre.org',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Topic :: Security',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12'
     ],
     keywords="stix stix2 json validation validator stix-validator stix2-validator",
     project_urls={
         'Documentation': 'https://stix2-validator.readthedocs.io/',
         'Source Code': 'https://github.com/oasis-open/cti-stix-validator/',
         'Bug Tracker': 'https://github.com/oasis-open/cti-stix-validator/issues/',
     },
@@ -63,14 +62,15 @@
             'stix2_validator = stix2validator.scripts.stix2_validator:main',
         ],
     },
     extras_require={
         'dev': [
             'bumpversion',
             'pre-commit',
+            'requests',
         ],
         'test': [
             'coverage',
             'pytest',
             'pytest-cov',
             'tox',
         ],
```

### Comparing `stix2-validator-3.1.4/stix2_validator.egg-info/PKG-INFO` & `stix2-validator-3.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,214 +1,213 @@
 Metadata-Version: 2.1
 Name: stix2-validator
-Version: 3.1.4
+Version: 3.2.0
 Summary: APIs and scripts for validating STIX 2.x documents.
 Home-page: https://github.com/oasis-open/cti-stix-validator
 Author: OASIS Cyber Threat Intelligence Technical Committee
 Author-email: cti-users@lists.oasis-open.org
 Maintainer: Chris Lenk
 Maintainer-email: clenk@mitre.org
 License: UNKNOWN
 Project-URL: Documentation, https://stix2-validator.readthedocs.io/
 Project-URL: Source Code, https://github.com/oasis-open/cti-stix-validator/
 Project-URL: Bug Tracker, https://github.com/oasis-open/cti-stix-validator/issues/
+Description: |Build_Status|  |Coverage|  |Version|  |Documentation_Status|
+        
+        ====================
+        `cti-stix-validator`
+        ====================
+        NOTE: This is an `OASIS TC Open Repository <https://www.oasis-
+        open.org/resources/open-repositories/>`__. See the `Governance`_
+        section for more information.
+        
+        The STIX Validator checks that STIX JSON content conforms to the
+        requirements specified in the STIX 2.1 specification. In addition to
+        checking conformance with the `JSON schemas <https://github.com/oasis-
+        open/cti-stix2-json-schemas>`_, the validator checks conformance with
+        requirements that cannot be specified in JSON schema, as well as with
+        established "best practices". This validator is non-normative; in
+        cases of conflict with the STIX 2.1 specification, the specification
+        takes precedence.
+        
+        The STIX 2.1 specification contains two types of requirements:
+        mandatory "MUST" requirements, and recommended "SHOULD" best practice
+        requirements. The validator checks documents against the "MUST"
+        requirements using JSON schemas. Some of these mandatory requirements
+        cannot be implemented in JSON Schema, however, so the validator uses
+        Python functions to check them. The "SHOULD" requirements are all
+        checked by Python functions, and options may be used to ignore some or
+        all of these recommended "best practices."
+        
+        The only exception to this is the mandatory requirement that an
+        object's 'type' be one of those defined by a STIX Object in the
+        specification. This rules out custom objects, so this check was made
+        optional.
+        
+        The validator also color-codes its output to make it easier to tell at
+        a glance whether validation passed.
+        
+        `Installation`
+        ==============
+        
+        The easiest way to install the STIX validator is with pip:
+        
+        ::
+        
+          $ pip install stix2-validator
+        
+        `Usage`
+        =======
+        
+        As A Script
+        -----------
+        
+        The validator comes with a bundled script which you can use to
+        validate a JSON file containing STIX content:
+        
+        ::
+        
+          $ stix2_validator <stix_file.json>
+        
+        As A Library
+        ------------
+        
+        You can also use this library to integrate STIX validation into your
+        own tools. You can validate a JSON file:
+        
+        .. code:: python
+        
+          from stix2validator import validate_file, print_results
+        
+          results = validate_file("stix_file.json")
+          print_results(results)
+        
+        You can also validate a JSON string using ``validate_string()``, or a Python
+        dictionary representing a STIX object using ``validate_instance()``. For more
+        information, see the full documentation
+        `here <https://stix2-validator.readthedocs.io/en/latest/usage.html>`_.
+        
+        Governance
+        ==========
+        
+        This GitHub public repository ( `https://github.com/oasis-open/cti-
+        stix-validator <https://github.com/oasis-open/cti-stix-validator>`_ )
+        was `proposed <https://lists.oasis-
+        open.org/archives/cti/201609/msg00001.html>`_ and `approved
+        <https://www.oasis-open.org/committees/ballot.php?id=2971>`_ [`bis
+        <https://issues.oasis-open.org/browse/TCADMIN-2434>`_] by the `OASIS
+        Cyber Threat Intelligence (CTI) TC <https://www.oasis-
+        open.org/committees/cti/>`_ as an `OASIS TC Open Repository
+        <https://www.oasis-open.org/resources/open-repositories/>`__ to support
+        development of open source resources related to Technical Committee
+        work.
+        
+        While this TC Open Repository remains associated with the sponsor TC,
+        its development priorities, leadership, intellectual property terms,
+        participation rules, and other matters of governance are `separate and
+        distinct <https://github.com/oasis-open/cti-stix-
+        validator/blob/master/CONTRIBUTING.md#governance-distinct-from-oasis-
+        tc-process>`_ from the OASIS TC Process and related policies.
+        
+        All contributions made to this TC Open Repository are subject to open
+        source license terms expressed in the `BSD-3-Clause License
+        <https://www.oasis-open.org/sites/www.oasis-open.org/files/BSD-3-
+        Clause.txt>`_. That license was selected as the declared `"Applicable
+        License" <https://www.oasis-open.org/resources/open-
+        repositories/licenses>`_ when the TC Open Repository was created.
+        
+        As documented in `"Public Participation Invited"
+        <https://github.com/oasis-open/cti-stix-
+        validator/blob/master/CONTRIBUTING.md#public-participation-invited>`_,
+        contributions to this OASIS TC Open Repository are invited from all
+        parties, whether affiliated with OASIS or not. Participants must have
+        a GitHub account, but no fees or OASIS membership obligations are
+        required. Participation is expected to be consistent with the `OASIS
+        TC Open Repository Guidelines and Procedures <https://www.oasis-
+        open.org/policies-guidelines/open-repositories>`_, the open source
+        `LICENSE <https://github.com/oasis-open/cti-stix-
+        validator/blob/master/LICENSE>`_ designated for this particular
+        repository, and the requirement for an `Individual Contributor License
+        Agreement <https://www.oasis-open.org/resources/open-
+        repositories/cla/individual-cla>`_ that governs intellectual property.
+        
+        `Maintainers`
+        =============
+        TC Open Repository `Maintainers <https://www.oasis-
+        open.org/resources/open-repositories/maintainers-guide>`__ are
+        responsible for oversight of this project's community development
+        activities, including evaluation of GitHub `pull requests
+        <https://github.com/oasis-open/cti-stix-
+        validator/blob/master/CONTRIBUTING.md#fork-and-pull-collaboration-
+        model>`_ and `preserving <https://www.oasis-open.org/policies-
+        guidelines/open-repositories#repositoryManagement>`_ open source
+        principles of openness and fairness. Maintainers are recognized and
+        trusted experts who serve to implement community goals and consensus
+        design preferences.
+        
+        Initially, the associated TC members have designated one or more
+        persons to serve as Maintainer(s); subsequently, participating
+        community members may select additional or substitute Maintainers, per
+        `consensus agreements <https://www.oasis-open.org/resources/open-
+        repositories/maintainers-guide#additionalMaintainers>`_.
+        
+        .. _currentMaintainers:
+        
+        **Current Maintainers of this TC Open Repository**
+        
+        .. Initial Maintainers: Greg Back & Ivan Kirillov & Chris Lenk
+        
+        * `Emily Ratliff <mailto:emily.ratliff@ibm.com>`__; GitHub ID: `https://github.com/ejratl <https://github.com/ejratl>`_; WWW: `IBM <http://www.ibm.com/>`__
+        *  `Jason Keirstead <mailto:Jason.Keirstead@ca.ibm.com>`__; GitHub ID: `https://github.com/JasonKeirstead <https://github.com/JasonKeirstead>`_; WWW: `IBM <http://www.ibm.com/>`__
+        * `Rich Piazza <mailto:rpiazza@mitre.org>`_; GitHub ID: `https://github.com/rpiazza <https://github.com/rpiazza>`_; WWW: `MITRE <http://www.mitre.org/>`_
+        
+        
+        .. _aboutOpenRepos:
+        
+        `About OASIS TC Open Repositories`
+        ==================================
+        *  `TC Open Repositories: Overview and Resources <https://www.oasis-open.org/resources/open-repositories/>`_
+        *  `Frequently Asked Questions <https://www.oasis-open.org/resources/open-repositories/faq>`_
+        *  `Open Source Licenses <https://www.oasis-open.org/resources/open-repositories/licenses>`_
+        *  `Contributor License Agreements (CLAs) <https://www.oasis-open.org/resources/open-repositories/cla>`_
+        *  `Maintainers' Guidelines and Agreement <https://www.oasis-open.org/resources/open-repositories/maintainers-guide>`__
+        
+        `Feedback`
+        ==========
+        Questions or comments about this TC Open Repository's activities
+        should be composed as GitHub issues or comments. If use of an
+        issue/comment is not possible or appropriate, questions may be
+        directed by email to the Maintainer(s) `listed above
+        <#currentmaintainers>`_. Please send general questions about TC Open
+        Repository participation to OASIS Staff at `repository-admin@oasis-
+        open.org <mailto:repository-admin@oasis-open.org>`_ and any specific
+        CLA-related questions to `repository-cla@oasis-open.org
+        <mailto:repository-cla@oasis-open.org>`_.
+        
+        
+        
+        .. |Build_Status| image:: https://github.com/oasis-open/cti-stix-validator/workflows/cti-stix-validator%20test%20harness/badge.svg
+           :target: https://github.com/oasis-open/cti-stix-validator/actions?query=workflow%3A%22cti-stix-validator+test+harness%22
+        .. |Coverage| image:: https://codecov.io/gh/oasis-open/cti-stix-validator/branch/master/graph/badge.svg
+           :target: https://codecov.io/gh/oasis-open/cti-stix-validator
+        .. |Version| image:: https://img.shields.io/pypi/v/stix2-validator.svg?maxAge=3600
+           :target: https://pypi.python.org/pypi/stix2-validator/
+        .. |Documentation_Status| image:: https://readthedocs.org/projects/stix2-validator/badge/?version=latest
+           :target: https://stix2-validator.readthedocs.io/en/latest/
+           :alt: Documentation Status
+        
+        
 Keywords: stix stix2 json validation validator stix-validator stix2-validator
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
-Provides-Extra: docs
 Provides-Extra: test
-License-File: LICENSE
-
-|Build_Status|  |Coverage|  |Version|  |Documentation_Status|
-
-====================
-`cti-stix-validator`
-====================
-NOTE: This is an `OASIS TC Open Repository <https://www.oasis-
-open.org/resources/open-repositories/>`__. See the `Governance`_
-section for more information.
-
-The STIX Validator checks that STIX JSON content conforms to the
-requirements specified in the STIX 2.1 specification. In addition to
-checking conformance with the `JSON schemas <https://github.com/oasis-
-open/cti-stix2-json-schemas>`_, the validator checks conformance with
-requirements that cannot be specified in JSON schema, as well as with
-established "best practices". This validator is non-normative; in
-cases of conflict with the STIX 2.1 specification, the specification
-takes precedence.
-
-The STIX 2.1 specification contains two types of requirements:
-mandatory "MUST" requirements, and recommended "SHOULD" best practice
-requirements. The validator checks documents against the "MUST"
-requirements using JSON schemas. Some of these mandatory requirements
-cannot be implemented in JSON Schema, however, so the validator uses
-Python functions to check them. The "SHOULD" requirements are all
-checked by Python functions, and options may be used to ignore some or
-all of these recommended "best practices."
-
-The only exception to this is the mandatory requirement that an
-object's 'type' be one of those defined by a STIX Object in the
-specification. This rules out custom objects, so this check was made
-optional.
-
-The validator also color-codes its output to make it easier to tell at
-a glance whether validation passed.
-
-`Installation`
-==============
-
-The easiest way to install the STIX validator is with pip:
-
-::
-
-  $ pip install stix2-validator
-
-`Usage`
-=======
-
-As A Script
------------
-
-The validator comes with a bundled script which you can use to
-validate a JSON file containing STIX content:
-
-::
-
-  $ stix2_validator <stix_file.json>
-
-As A Library
-------------
-
-You can also use this library to integrate STIX validation into your
-own tools. You can validate a JSON file:
-
-.. code:: python
-
-  from stix2validator import validate_file, print_results
-
-  results = validate_file("stix_file.json")
-  print_results(results)
-
-You can also validate a JSON string using ``validate_string()``, or a Python
-dictionary representing a STIX object using ``validate_instance()``. For more
-information, see the full documentation
-`here <https://stix2-validator.readthedocs.io/en/latest/usage.html>`_.
-
-Governance
-==========
-
-This GitHub public repository ( `https://github.com/oasis-open/cti-
-stix-validator <https://github.com/oasis-open/cti-stix-validator>`_ )
-was `proposed <https://lists.oasis-
-open.org/archives/cti/201609/msg00001.html>`_ and `approved
-<https://www.oasis-open.org/committees/ballot.php?id=2971>`_ [`bis
-<https://issues.oasis-open.org/browse/TCADMIN-2434>`_] by the `OASIS
-Cyber Threat Intelligence (CTI) TC <https://www.oasis-
-open.org/committees/cti/>`_ as an `OASIS TC Open Repository
-<https://www.oasis-open.org/resources/open-repositories/>`__ to support
-development of open source resources related to Technical Committee
-work.
-
-While this TC Open Repository remains associated with the sponsor TC,
-its development priorities, leadership, intellectual property terms,
-participation rules, and other matters of governance are `separate and
-distinct <https://github.com/oasis-open/cti-stix-
-validator/blob/master/CONTRIBUTING.md#governance-distinct-from-oasis-
-tc-process>`_ from the OASIS TC Process and related policies.
-
-All contributions made to this TC Open Repository are subject to open
-source license terms expressed in the `BSD-3-Clause License
-<https://www.oasis-open.org/sites/www.oasis-open.org/files/BSD-3-
-Clause.txt>`_. That license was selected as the declared `"Applicable
-License" <https://www.oasis-open.org/resources/open-
-repositories/licenses>`_ when the TC Open Repository was created.
-
-As documented in `"Public Participation Invited"
-<https://github.com/oasis-open/cti-stix-
-validator/blob/master/CONTRIBUTING.md#public-participation-invited>`_,
-contributions to this OASIS TC Open Repository are invited from all
-parties, whether affiliated with OASIS or not. Participants must have
-a GitHub account, but no fees or OASIS membership obligations are
-required. Participation is expected to be consistent with the `OASIS
-TC Open Repository Guidelines and Procedures <https://www.oasis-
-open.org/policies-guidelines/open-repositories>`_, the open source
-`LICENSE <https://github.com/oasis-open/cti-stix-
-validator/blob/master/LICENSE>`_ designated for this particular
-repository, and the requirement for an `Individual Contributor License
-Agreement <https://www.oasis-open.org/resources/open-
-repositories/cla/individual-cla>`_ that governs intellectual property.
-
-`Maintainers`
-=============
-TC Open Repository `Maintainers <https://www.oasis-
-open.org/resources/open-repositories/maintainers-guide>`__ are
-responsible for oversight of this project's community development
-activities, including evaluation of GitHub `pull requests
-<https://github.com/oasis-open/cti-stix-
-validator/blob/master/CONTRIBUTING.md#fork-and-pull-collaboration-
-model>`_ and `preserving <https://www.oasis-open.org/policies-
-guidelines/open-repositories#repositoryManagement>`_ open source
-principles of openness and fairness. Maintainers are recognized and
-trusted experts who serve to implement community goals and consensus
-design preferences.
-
-Initially, the associated TC members have designated one or more
-persons to serve as Maintainer(s); subsequently, participating
-community members may select additional or substitute Maintainers, per
-`consensus agreements <https://www.oasis-open.org/resources/open-
-repositories/maintainers-guide#additionalMaintainers>`_.
-
-.. _currentMaintainers:
-
-**Current Maintainers of this TC Open Repository**
-
-.. Initial Maintainers: Greg Back & Ivan Kirillov & Chris Lenk
-
-* `Emily Ratliff <mailto:emily.ratliff@ibm.com>`__; GitHub ID: `https://github.com/ejratl <https://github.com/ejratl>`_; WWW: `IBM <http://www.ibm.com/>`__
-* `Duncan Sparrell <mailto:duncan@sfractal.com>`__; GitHub ID: `https://github.com/sparrell <https://github.com/sparrell>`_; WWW: `sFractal <http://sfractal.com/>`__
-*  `Jason Keirstead <mailto:Jason.Keirstead@ca.ibm.com>`__; GitHub ID: `https://github.com/JasonKeirstead <https://github.com/JasonKeirstead>`_; WWW: `IBM <http://www.ibm.com/>`__
-
-.. _aboutOpenRepos:
-
-`About OASIS TC Open Repositories`
-==================================
-*  `TC Open Repositories: Overview and Resources <https://www.oasis-open.org/resources/open-repositories/>`_
-*  `Frequently Asked Questions <https://www.oasis-open.org/resources/open-repositories/faq>`_
-*  `Open Source Licenses <https://www.oasis-open.org/resources/open-repositories/licenses>`_
-*  `Contributor License Agreements (CLAs) <https://www.oasis-open.org/resources/open-repositories/cla>`_
-*  `Maintainers' Guidelines and Agreement <https://www.oasis-open.org/resources/open-repositories/maintainers-guide>`__
-
-`Feedback`
-==========
-Questions or comments about this TC Open Repository's activities
-should be composed as GitHub issues or comments. If use of an
-issue/comment is not possible or appropriate, questions may be
-directed by email to the Maintainer(s) `listed above
-<#currentmaintainers>`_. Please send general questions about TC Open
-Repository participation to OASIS Staff at `repository-admin@oasis-
-open.org <mailto:repository-admin@oasis-open.org>`_ and any specific
-CLA-related questions to `repository-cla@oasis-open.org
-<mailto:repository-cla@oasis-open.org>`_.
-
-
-
-.. |Build_Status| image:: https://github.com/oasis-open/cti-stix-validator/workflows/cti-stix-validator%20test%20harness/badge.svg
-   :target: https://github.com/oasis-open/cti-stix-validator/actions?query=workflow%3A%22cti-stix-validator+test+harness%22
-.. |Coverage| image:: https://codecov.io/gh/oasis-open/cti-stix-validator/branch/master/graph/badge.svg
-   :target: https://codecov.io/gh/oasis-open/cti-stix-validator
-.. |Version| image:: https://img.shields.io/pypi/v/stix2-validator.svg?maxAge=3600
-   :target: https://pypi.python.org/pypi/stix2-validator/
-.. |Documentation_Status| image:: https://readthedocs.org/projects/stix2-validator/badge/?version=latest
-   :target: https://stix2-validator.readthedocs.io/en/latest/
-   :alt: Documentation Status
-
-
-
+Provides-Extra: docs
```

### Comparing `stix2-validator-3.1.4/stix2_validator.egg-info/SOURCES.txt` & `stix2-validator-3.2.0/stix2_validator.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -157,13 +157,37 @@
 stix2validator/scripts/stix2_validator.py
 stix2validator/test/__init__.py
 stix2validator/v20/__init__.py
 stix2validator/v20/enums.py
 stix2validator/v20/errors.py
 stix2validator/v20/musts.py
 stix2validator/v20/shoulds.py
+stix2validator/v20/assets/charsets.csv
+stix2validator/v20/assets/ipfix-information-elements.csv
+stix2validator/v20/assets/mediatype_application.csv
+stix2validator/v20/assets/mediatype_audio.csv
+stix2validator/v20/assets/mediatype_font.csv
+stix2validator/v20/assets/mediatype_image.csv
+stix2validator/v20/assets/mediatype_message.csv
+stix2validator/v20/assets/mediatype_model.csv
+stix2validator/v20/assets/mediatype_multipart.csv
+stix2validator/v20/assets/mediatype_text.csv
+stix2validator/v20/assets/mediatype_video.csv
+stix2validator/v20/assets/protocols.csv
 stix2validator/v21/__init__.py
 stix2validator/v21/enums.py
 stix2validator/v21/errors.py
 stix2validator/v21/interop.py
 stix2validator/v21/musts.py
-stix2validator/v21/shoulds.py
+stix2validator/v21/shoulds.py
+stix2validator/v21/assets/charsets.csv
+stix2validator/v21/assets/ipfix-information-elements.csv
+stix2validator/v21/assets/mediatype_application.csv
+stix2validator/v21/assets/mediatype_audio.csv
+stix2validator/v21/assets/mediatype_font.csv
+stix2validator/v21/assets/mediatype_image.csv
+stix2validator/v21/assets/mediatype_message.csv
+stix2validator/v21/assets/mediatype_model.csv
+stix2validator/v21/assets/mediatype_multipart.csv
+stix2validator/v21/assets/mediatype_text.csv
+stix2validator/v21/assets/mediatype_video.csv
+stix2validator/v21/assets/protocols.csv
```

### Comparing `stix2-validator-3.1.4/stix2validator/codes.py` & `stix2-validator-3.2.0/stix2validator/codes.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/errors.py` & `stix2-validator-3.2.0/stix2validator/errors.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/output.py` & `stix2-validator-3.2.0/stix2validator/output.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/indicator-for-c2-ip-address.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/examples/indicator-for-c2-ip-address.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/indicator-to-campaign-relationship.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/examples/indicator-to-campaign-relationship.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/indicators-for-C2-with-COA.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/examples/indicators-for-C2-with-COA.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/malicious-email-indicator-with-attachment.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/examples/malicious-email-indicator-with-attachment.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/threat-reports/apt1.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/examples/threat-reports/apt1.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/examples/threat-reports/poisonivy.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/examples/threat-reports/poisonivy.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/binary.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/binary.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/bundle.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/bundle.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/core.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/core.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/cyber-observable-core.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/cyber-observable-core.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/dictionary.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/dictionary.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/external-reference.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/external-reference.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/granular-marking.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/granular-marking.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/hashes-type.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/hashes-type.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/hex.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/hex.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/identifier.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/identifier.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/kill-chain-phase.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/kill-chain-phase.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/marking-definition.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/marking-definition.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/common/url-regex.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/common/url-regex.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/artifact.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/artifact.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/autonomous-system.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/autonomous-system.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/directory.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/directory.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/domain-name.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/domain-name.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/email-addr.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/email-addr.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/email-message.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/email-message.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/file.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/file.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/ipv4-addr.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/ipv4-addr.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/ipv6-addr.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/ipv6-addr.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/mac-addr.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/mac-addr.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/mutex.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/mutex.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/network-traffic.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/network-traffic.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/process.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/process.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/software.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/software.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/url.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/url.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/user-account.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/user-account.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/windows-registry-key.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/windows-registry-key.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/observables/x509-certificate.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/observables/x509-certificate.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/attack-pattern.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/attack-pattern.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/campaign.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/campaign.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/course-of-action.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/course-of-action.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/identity.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/identity.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/indicator.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/indicator.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/intrusion-set.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/intrusion-set.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/malware.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/malware.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/observed-data.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/observed-data.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/report.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/report.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/threat-actor.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/threat-actor.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/tool.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/tool.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sdos/vulnerability.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sdos/vulnerability.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sros/relationship.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sros/relationship.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.0/schemas/sros/sighting.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.0/schemas/sros/sighting.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/indicator-for-c2-ip-address.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/indicator-for-c2-ip-address.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/indicator-to-campaign-relationship.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/indicator-to-campaign-relationship.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/indicators-for-C2-with-COA.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/indicators-for-C2-with-COA.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/infrastructure.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/infrastructure.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/interop-objectmarking-test.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/interop-objectmarking-test.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/malicious-email-indicator-with-attachment.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/malicious-email-indicator-with-attachment.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/threat-reports/apt1.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/threat-reports/apt1.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/examples/threat-reports/poisonivy.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/examples/threat-reports/poisonivy.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/core.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/core.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/interop/malware.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/interop/malware.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/binary.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/binary.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,8 +1,8 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/common/binary.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "The \u200bbinary data type represents a sequence of bytes. In order to allow pattern matching on custom objects, for all properties that use the binary type, the property name MUST end with '_bin'. The JSON MTI serialization represents this as a base64-\u00adencoded string as specified in RFC4648\u200b. Other serializations SHOULD use a native binary type, if available.",
     "pattern": "^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{4}|[A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)$",
     "title": "binary",
     "type": "string"
 }
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/bundle.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/bundle.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/common/bundle.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "A Bundle is a collection of arbitrary STIX Objects and Marking Definitions grouped together in a single container.",
     "properties": {
         "id": {
             "allOf": [
                 {
                     "$ref": "../common/identifier.json",
                     "description": "An identifier for this bundle. The id field for the Bundle is designed to help tools that may need it for processing, but tools are not required to store or track it. "
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/core.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/core.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999007936507935%*

 * *Differences: {"'properties'": "{'extensions': {'patternProperties': "*

 * *                 "{'^([a-z][a-z0-9]*)+(-[a-z0-9]+)*\\\\-ext$': OrderedDict([('type', 'object'), "*

 * *                 "('minProperties', 1), ('allOf', [OrderedDict([('$ref', "*

 * *                 "'../common/properties.json')])])])}}}"}*

```diff
@@ -55,14 +55,23 @@
             "description": "The ID of the Source object that describes who created this object."
         },
         "extensions": {
             "additionalProperties": false,
             "description": "Specifies any extensions of the object, as a dictionary.",
             "minProperties": 1,
             "patternProperties": {
+                "^([a-z][a-z0-9]*)+(-[a-z0-9]+)*\\-ext$": {
+                    "allOf": [
+                        {
+                            "$ref": "../common/properties.json"
+                        }
+                    ],
+                    "minProperties": 1,
+                    "type": "object"
+                },
                 "^extension-definition--[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[1-5][0-9a-fA-F]{3}-[89abAB][0-9a-fA-F]{3}-[0-9a-fA-F]{12}$": {
                     "allOf": [
                         {
                             "$ref": "../common/extension.json"
                         }
                     ]
                 }
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/cyber-observable-core.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/cyber-observable-core.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/common/cyber-observable-core.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/properties.json"
         }
     ],
     "description": "Common properties and behavior across all Cyber Observable Objects.",
     "not": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/dictionary.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/dictionary.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/common/dictionary.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "additionalProperties": false,
     "description": "A dictionary captures a set of key/value pairs",
     "minProperties": 1,
     "patternProperties": {
         "^[a-zA-Z0-9_-]{0,250}$": {
             "anyOf": [
                 {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/extension-definition.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/extension-definition.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/common/extension-definition.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "description": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/extension.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/extension.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/common/extension.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/properties.json"
         }
     ],
     "definitions": {
         "extension-type-enum": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/external-reference.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/external-reference.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/common/external-reference.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "External references are used to describe pointers to information represented outside of STIX.",
     "oneOf": [
         {
             "properties": {
                 "external_id": {
                     "description": "An identifier for the external reference content.",
                     "pattern": "^CVE-\\d{4}-(0\\d{3}|[1-9]\\d{3,})$",
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/granular-marking.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/granular-marking.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/common/granular-marking.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "The granular-marking type defines how the list of marking-definition objects referenced by the marking_refs property to apply to a set of content identified by the list of selectors in the selectors property.",
     "properties": {
         "lang": {
             "description": "Identifies the language of the text identified by this marking.",
             "type": "string"
         },
         "marking_ref": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/hashes-type.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/hashes-type.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/common/hashes-type.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "additionalProperties": false,
     "allOf": [
         {
             "$ref": "../common/dictionary.json"
         }
     ],
     "description": "The Hashes type represents one or more cryptographic hashes, as a special set of key/value pairs",
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/hex.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/hex.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,8 +1,8 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/common/hex.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "The hex data type encodes an array of octets (8-bit bytes) as hexadecimal. The string MUST consist of an even number of hexadecimal characters, which are the digits '0' through '9' and the letters 'a' through 'f'.  In order to allow pattern matching on custom objects, all properties that use the hex type, the property name MUST end with '_hex'.",
     "pattern": "^([a-fA-F0-9]{2})+$",
     "title": "hex",
     "type": "string"
 }
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/identifier.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/identifier.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,8 +1,8 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/common/identifier.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "Represents identifiers across the CTI specifications. The format consists of the name of the top-level object being identified, followed by two dashes (--), followed by a UUIDv4.",
     "pattern": "^[a-z][a-z0-9-]+[a-z0-9]--[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[1-5][0-9a-fA-F]{3}-[89abAB][0-9a-fA-F]{3}-[0-9a-fA-F]{12}$",
     "title": "identifier",
     "type": "string"
 }
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/kill-chain-phase.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/kill-chain-phase.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/common/kill-chain-phase.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "description": "The kill-chain-phase represents a phase in a kill chain.",
     "properties": {
         "kill_chain_name": {
             "description": "The name of the kill chain.",
             "type": "string"
         },
         "phase_name": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/language-content.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/language-content.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/common/language-content.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "contents": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/common/marking-definition.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/common/marking-definition.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/common/marking-definition.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "definitions": {
         "statement": {
             "description": "The Statement marking type defines the representation of a textual marking statement (e.g., copyright, terms of use, etc.) in a definition",
             "properties": {
                 "statement": {
                     "description": "A statement (e.g., copyright, terms of use) applied to the content marked by this marking definition.",
                     "type": "string"
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/artifact.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/artifact.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/artifact.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "decryption_key": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/autonomous-system.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/autonomous-system.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/autonomous-system.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "id": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/directory.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/directory.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/directory.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "atime": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/domain-name.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/domain-name.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/domain-name.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "id": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/email-addr.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/email-addr.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/email-addr.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "belongs_to_ref": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/email-message.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/email-message.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/email-message.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "additional_header_fields": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/file.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/file.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/file.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "atime": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/ipv4-addr.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/ipv4-addr.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/ipv4-addr.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "belongs_to_refs": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/ipv6-addr.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/ipv6-addr.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/ipv6-addr.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "belongs_to_refs": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/mac-addr.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/mac-addr.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/mac-addr.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "id": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/mutex.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/mutex.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/mutex.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "id": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/network-traffic.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/network-traffic.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.949999745686849%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'",*

 * * "'definitions'": "{'network-traffic-extensions-dictionary': {'patternProperties': "*

 * *                  "{'^http-request-ext$': {'properties': {'request_header': {'patternProperties': "*

 * *                  "{'^.+$': {'type': 'array', 'items': OrderedDict([('type', 'string')])}}}}}}}}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/network-traffic.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "dst_byte_count": {
@@ -158,15 +158,18 @@
                                 {
                                     "$ref": "../common/dictionary.json"
                                 }
                             ],
                             "description": "Specifies all of the HTTP header fields that may be found in the HTTP client request, as a dictionary.",
                             "patternProperties": {
                                 "^.+$": {
-                                    "type": "string"
+                                    "items": {
+                                        "type": "string"
+                                    },
+                                    "type": "array"
                                 }
                             }
                         },
                         "request_method": {
                             "description": "Specifies the HTTP method portion of the HTTP request line, as a lowercase string.",
                             "type": "string"
                         },
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/process.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/process.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/process.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "child_refs": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/software.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/software.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/software.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "cpe": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/url.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/url.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/url.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "id": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/user-account.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/user-account.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/user-account.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "account_created": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/windows-registry-key.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/windows-registry-key.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/windows-registry-key.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "creator_user_ref": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/observables/x509-certificate.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/observables/x509-certificate.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/observables/x509-certificate.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/cyber-observable-core.json"
         },
         {
             "properties": {
                 "hashes": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/attack-pattern.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/attack-pattern.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/attack-pattern.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "aliases": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/campaign.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/campaign.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/campaign.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "aliases": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/course-of-action.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/course-of-action.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/course-of-action.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "description": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/grouping.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/grouping.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/grouping.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "context": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/identity.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/identity.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/identity.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "contact_information": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/incident.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/incident.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/incident.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "description": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/indicator.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/indicator.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/indicator.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "description": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/infrastructure.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/infrastructure.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/infrastructure.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "aliases": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/intrusion-set.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/intrusion-set.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/intrusion-set.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "aliases": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/location.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/location.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/location.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "administrative_area": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/malware-analysis.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/malware-analysis.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/malware-analysis.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "analysis_definition_version": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/malware.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/malware.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/malware.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "aliases": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/note.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/note.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/note.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "abstract": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/observed-data.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/observed-data.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/observed-data.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "first_observed": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/opinion.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/opinion.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/opinion.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "authors": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/report.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/report.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/report.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "description": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/threat-actor.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/threat-actor.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/threat-actor.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "aliases": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/tool.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/tool.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/tool.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "aliases": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sdos/vulnerability.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sdos/vulnerability.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sdos/vulnerability.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "description": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sros/relationship.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sros/relationship.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft/2020-12/schema'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$id": "http://raw.githubusercontent.com/oasis-open/cti-stix2-json-schemas/stix2.1/schemas/sros/relationship.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema#",
+    "$schema": "https://json-schema.org/draft/2020-12/schema",
     "allOf": [
         {
             "$ref": "../common/core.json"
         },
         {
             "properties": {
                 "description": {
```

### Comparing `stix2-validator-3.1.4/stix2validator/schemas-2.1/schemas/sros/sighting.json` & `stix2-validator-3.2.0/stix2validator/schemas-2.1/schemas/sros/sighting.json`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/scripts/stix2_validator.py` & `stix2-validator-3.2.0/stix2validator/scripts/stix2_validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 import logging
 import os
 import sys
 
 from stix2validator import (ValidationError, codes, output, parse_args,
                             print_results, run_validation)
 
-logging.basicConfig(stream=sys.stdout, level=logging.INFO, format='%(message)s')
-logger = logging.getLogger(__name__)
-
 
 def main():
     # Parse command line arguments
     options = parse_args(sys.argv[1:], is_script=True)
 
+    # Initialize the logger
+    logging.basicConfig(stream=sys.stdout, level=logging.INFO, format='%(message)s')
+    logger = logging.getLogger(__name__)
+
     # Only print prompt if script is run on cmdline and no input is piped in
     if options.files == sys.stdin and os.isatty(0):
-        logging.info('Input STIX content, then press Ctrl+D: ')
+        logger.info('Input STIX content, then press Ctrl+D: ')
 
     try:
         # Validate input documents
         results = run_validation(options)
 
         # Print validation results
         print_results(results)
```

### Comparing `stix2-validator-3.1.4/stix2validator/util.py` & `stix2-validator-3.2.0/stix2validator/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import argparse
 from argparse import RawDescriptionHelpFormatter
 from collections.abc import Iterable
-import datetime
-import errno
-import os
 import sys
 import textwrap
 
-from appdirs import AppDirs
-import requests_cache
-
 from .output import set_level, set_silent
 from .v20.enums import CHECK_CODES as CHECK_CODES20
 from .v21.enums import CHECK_CODES as CHECK_CODES21
 from .v21.enums import OBSERVABLE_TYPES as OBSERVABLE_TYPES21
 
 DEFAULT_VER = "2.1"
 
@@ -349,46 +343,36 @@
         enabled: List of "SHOULD" checks that will be performed.
         strict: Specifies that recommended requirements should produce errors
             instead of mere warnings.
         strict_types: Specifies that no custom object types be used, only
             those defined in the STIX specification.
         strict_properties: Specifies that no custom properties be used, only
             those defined in the STIX specification.
-        no_cache: Specifies that caching of values from external sources should
-            be disabled.
-        refresh_cache: Specifies that the cache of values from external sources
-            should be cleared before validation, and then re-downloaded during
-            validation.
-        clear_cache: Specifies that the cache of values from external sources
-            should be cleared after validation.
         enforce_refs:Ensures that all SDOs being referenced by the SRO are
             contained within the same bundle
 
     """
     def __init__(self, cmd_args=None, version=None, verbose=False, silent=False,
                  files=None, recursive=False, schema_dir=None,
                  disabled="", enabled="", strict=False,
-                 strict_types=False, strict_properties=False, no_cache=False,
-                 refresh_cache=False, clear_cache=False, enforce_refs=False, interop=False):
+                 strict_types=False, strict_properties=False, enforce_refs=False,
+                 interop=False):
 
         if cmd_args is not None:
             self.version = cmd_args.version
             self.verbose = cmd_args.verbose
             self.silent = cmd_args.silent
             self.files = cmd_args.files
             self.recursive = cmd_args.recursive
             self.schema_dir = cmd_args.schema_dir
             self.disabled = cmd_args.disabled
             self.enabled = cmd_args.enabled
             self.strict = cmd_args.strict
             self.strict_types = cmd_args.strict_types
             self.strict_properties = cmd_args.strict_properties
-            self.no_cache = cmd_args.no_cache
-            self.refresh_cache = cmd_args.refresh_cache
-            self.clear_cache = cmd_args.clear_cache
             self.enforce_refs = cmd_args.enforce_refs
             self.interop = cmd_args.interop
         else:
             # input options
             self.version = version
             self.files = files
             self.recursive = recursive
@@ -399,20 +383,14 @@
             self.silent = silent
             self.strict = strict
             self.strict_types = strict_types
             self.strict_properties = strict_properties
             self.disabled = disabled
             self.enabled = enabled
             self.enforce_refs = enforce_refs
-
-            # cache options
-            self.no_cache = no_cache
-            self.refresh_cache = refresh_cache
-            self.clear_cache = clear_cache
-
             self.interop = interop
         # Set the output level (e.g., quiet vs. verbose)
         if self.silent and self.verbose:
             raise ValueError('Error: Output can either be silent or verbose, but not both.')
         set_level(self.verbose)
         set_silent(self.silent)
 
@@ -492,39 +470,7 @@
                 if isinstance(func, Iterable):
                     for x in original_function(*args, **kwargs):
                         yield x
 
         new_function.__name__ = original_function.__name__
         return new_function
     return inner_cyber_observable_check
-
-
-def init_requests_cache(refresh_cache=False):
-    """
-    Initializes a cache which the ``requests`` library will consult for
-    responses, before making network requests.
-
-    :param refresh_cache: Whether the cache should be cleared out
-    """
-    # Cache data from external sources; used in some checks
-    dirs = AppDirs("stix2-validator", "OASIS")
-    # Create cache dir if doesn't exist
-    try:
-        os.makedirs(dirs.user_cache_dir)
-    except OSError as e:
-        if e.errno != errno.EEXIST:
-            raise
-    requests_cache.install_cache(
-        cache_name=os.path.join(dirs.user_cache_dir, 'py{}cache'.format(
-            sys.version_info[0])),
-        expire_after=datetime.timedelta(weeks=1))
-
-    if refresh_cache:
-        clear_requests_cache()
-
-
-def clear_requests_cache():
-    """
-    Clears all cached responses.
-    """
-    now = datetime.datetime.utcnow()
-    requests_cache.get_cache().remove_old_entries(now)
```

### Comparing `stix2-validator-3.1.4/stix2validator/v20/enums.py` & `stix2-validator-3.2.0/stix2validator/v20/enums.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """STIX 2.0 open vocabularies and other lists
 """
 
-import re
-
-import requests
+import csv
+import glob
+import os
 
 # Enumerations of the default values of STIX open vocabularies
 ATTACK_MOTIVATION_OV = [
     "accidental",
     "coercion",
     "dominance",
     "ideology",
@@ -1394,135 +1394,100 @@
     '276': 'pdf-doc-info',
     '301': 'network-traffic-ports',
     '302': 'extref-hashes',
 }
 
 
 def media_types():
-    """Return a list of the IANA Media (MIME) Types, or an empty list if the
-    IANA website is unreachable.
+    """Return a list of the IANA Media (MIME) Types.
     Store it as a function attribute so that we only build the list once.
     """
     if not hasattr(media_types, 'typelist'):
+        basepath = os.path.abspath(os.path.dirname(__file__))
         tlist = []
-        categories = [
-            'application',
-            'audio',
-            'font',
-            'image',
-            'message',
-            'model',
-            'multipart',
-            'text',
-            'video'
-        ]
-        for cat in categories:
-            try:
-                data = requests.get('http://www.iana.org/assignments/'
-                                    'media-types/%s.csv' % cat)
-            except requests.exceptions.RequestException:
-                return []
-
+        for fpath in glob.glob(basepath + '/assets/mediatype_*.csv'):
             types = []
-            for line in data.iter_lines():
-                if line:
-                    line = line.decode("utf-8")
-                    if line.count(',') > 0:
-                        reg_template = line.split(',')[1]
-                        if reg_template:
-                            types.append(reg_template)
-                        else:
-                            types.append(cat + '/' + line.split(',')[0])
-
+            cat = os.path.basename(fpath).split('_', 1)[1].rsplit('.', 1)[0]
+            with open(fpath, 'r', encoding='utf-8') as fd:
+                reader = csv.DictReader(fd)
+                for row in reader:
+                    name = row.get('Name')
+                    template = row.get('Template')
+                    if template:
+                        types.append(template)
+                    elif name:
+                        types.append(cat + '/' + name)
             tlist.extend(types)
         media_types.typelist = tlist
     return media_types.typelist
 
 
 def char_sets():
-    """Return a list of the IANA Character Sets, or an empty list if the
-    IANA website is unreachable.
+    """Return a list of the IANA Character Sets.
     Store it as a function attribute so that we only build the list once.
     """
     if not hasattr(char_sets, 'setlist'):
+        basepath = os.path.abspath(os.path.dirname(__file__))
         clist = []
-        try:
-            data = requests.get('http://www.iana.org/assignments/character-'
-                                'sets/character-sets-1.csv')
-        except requests.exceptions.RequestException:
-            return []
-
-        for line in data.iter_lines():
-            if line:
-                line = line.decode("utf-8")
-                if line.count(',') > 0:
-                    vals = line.split(',')
-                    if vals[0]:
-                        clist.append(vals[0])
-                    else:
-                        clist.append(vals[1])
-
+        with open(basepath + '/assets/charsets.csv', 'r', encoding='utf-8') as fd:
+            reader = csv.DictReader(fd)
+            for row in reader:
+                preferred_name = row.get('Preferred MIME Name')
+                name = row.get('Name')
+                if preferred_name:
+                    clist.append(preferred_name)
+                elif name:
+                    clist.append(name)
         char_sets.setlist = clist
     return char_sets.setlist
 
 
 def protocols():
     """Return a list of values from the IANA Service Name and Transport
-    Protocol Port Number Registry, or an empty list if the IANA website is
-    unreachable.
+    Protocol Port Number Registry.
     Store it as a function attribute so that we only build the list once.
     """
     if not hasattr(protocols, 'protlist'):
-        plist = []
-        try:
-            data = requests.get('http://www.iana.org/assignments/service-names'
-                                '-port-numbers/service-names-port-numbers.csv')
-        except requests.exceptions.RequestException:
-            return []
-
-        for line in data.iter_lines():
-            if line:
-                line = line.decode("utf-8")
-                if line.count(',') > 0:
-                    vals = line.split(',')
-                    if vals[0]:
-                        plist.append(vals[0])
-                    if len(vals) > 2 and vals[2] and vals[2] not in plist:
-                        plist.append(vals[2])
-
-        plist.append('ipv4')
-        plist.append('ipv6')
-        plist.append('ssl')
-        plist.append('tls')
-        plist.append('dns')
+        basepath = os.path.abspath(os.path.dirname(__file__))
+        plist = set()
+        with open(basepath + '/assets/protocols.csv', 'r', encoding='utf-8') as fd:
+            reader = csv.DictReader(fd)
+            for row in reader:
+                name = row.get('Service Name')
+                transport_protocol = row.get('Transport Protocol')
+                if name:
+                    plist.add(name)
+                if transport_protocol:
+                    plist.add(transport_protocol)
+
+        plist.add('ipv4')
+        plist.add('ipv6')
+        plist.add('ssl')
+        plist.add('tls')
+        plist.add('dns')
+        plist = sorted(plist)
         protocols.protlist = plist
     return protocols.protlist
 
 
 def ipfix():
     """Return a list of values from the list of IANA IP Flow Information Export
-    (IPFIX) Entities, or an empty list if the IANA website is unreachable.
+    (IPFIX) Entities.
     Store it as a function attribute so that we only build the list once.
     """
     if not hasattr(ipfix, 'ipflist'):
+        basepath = os.path.abspath(os.path.dirname(__file__))
         ilist = []
-        try:
-            data = requests.get('http://www.iana.org/assignments/ipfix/ipfix-'
-                                'information-elements.csv')
-        except requests.exceptions.RequestException:
-            return []
-
-        for line in data.iter_lines():
-            if line:
-                line = line.decode("utf-8")
-                if re.match(r'^\d+(,[a-zA-Z0-9]+){2},', line):
-                    vals = line.split(',')
-                    if vals[1]:
-                        ilist.append(vals[1])
 
+        with open(basepath + '/assets/ipfix-information-elements.csv', 'r', encoding='utf-8') as fd:
+            reader = csv.DictReader(fd)
+            for row in reader:
+                name = row.get('Name')
+                if name:
+                    ilist.append(name)
         ipfix.ipflist = ilist
     return ipfix.ipflist
 
 
 SOCKET_OPTIONS = [
     'SO_ACCEPTCONN',
     'SO_BINDTODEVICE',
```

### Comparing `stix2-validator-3.1.4/stix2validator/v20/errors.py` & `stix2-validator-3.2.0/stix2validator/v20/errors.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/v20/musts.py` & `stix2-validator-3.2.0/stix2validator/v20/musts.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/v20/shoulds.py` & `stix2-validator-3.2.0/stix2validator/v20/shoulds.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/v21/enums.py` & `stix2-validator-3.2.0/stix2validator/v21/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """STIX 2.1 WD04 open vocabularies and other lists
 """
-
-import re
-
-import requests
+import csv
+import glob
+import os
 
 # Enumerations of the default values of STIX open vocabularies
 ATTACK_MOTIVATION_OV = [
     "accidental",
     "coercion",
     "dominance",
     "ideology",
@@ -2189,135 +2188,99 @@
     '305': 'extension-description',
     '306': 'extension-properties',
     '401': 'extensions-use',
 }
 
 
 def media_types():
-    """Return a list of the IANA Media (MIME) Types, or an empty list if the
-    IANA website is unreachable.
+    """Return a list of the IANA Media (MIME) Types.
     Store it as a function attribute so that we only build the list once.
     """
     if not hasattr(media_types, 'typelist'):
+        basepath = os.path.abspath(os.path.dirname(__file__))
         tlist = []
-        categories = [
-            'application',
-            'audio',
-            'font',
-            'image',
-            'message',
-            'model',
-            'multipart',
-            'text',
-            'video'
-        ]
-        for cat in categories:
-            try:
-                data = requests.get('http://www.iana.org/assignments/'
-                                    'media-types/%s.csv' % cat)
-            except requests.exceptions.RequestException:
-                return []
-
+        for fpath in glob.glob(basepath + '/assets/mediatype_*.csv'):
             types = []
-            for line in data.iter_lines():
-                if line:
-                    line = line.decode("utf-8")
-                    if line.count(',') > 0:
-                        reg_template = line.split(',')[1]
-                        if reg_template:
-                            types.append(reg_template)
-                        else:
-                            types.append(cat + '/' + line.split(',')[0])
-
+            cat = os.path.basename(fpath).split('_', 1)[1].rsplit('.', 1)[0]
+            with open(fpath, 'r', encoding='utf-8') as fd:
+                reader = csv.DictReader(fd)
+                for row in reader:
+                    name = row.get('Name')
+                    template = row.get('Template')
+                    if template:
+                        types.append(template)
+                    elif name:
+                        types.append(cat + '/' + name)
             tlist.extend(types)
         media_types.typelist = tlist
     return media_types.typelist
 
 
 def char_sets():
-    """Return a list of the IANA Character Sets, or an empty list if the
-    IANA website is unreachable.
+    """Return a list of the IANA Character Sets.
     Store it as a function attribute so that we only build the list once.
     """
     if not hasattr(char_sets, 'setlist'):
+        basepath = os.path.abspath(os.path.dirname(__file__))
         clist = []
-        try:
-            data = requests.get('http://www.iana.org/assignments/character-'
-                                'sets/character-sets-1.csv')
-        except requests.exceptions.RequestException:
-            return []
-
-        for line in data.iter_lines():
-            if line:
-                line = line.decode("utf-8")
-                if line.count(',') > 0:
-                    vals = line.split(',')
-                    if vals[0]:
-                        clist.append(vals[0])
-                    else:
-                        clist.append(vals[1])
-
+        with open(basepath + '/assets/charsets.csv', 'r', encoding='utf-8') as fd:
+            reader = csv.DictReader(fd)
+            for row in reader:
+                preferred_name = row.get('Preferred MIME Name')
+                name = row.get('Name')
+                if preferred_name:
+                    clist.append(preferred_name)
+                elif name:
+                    clist.append(name)
         char_sets.setlist = clist
     return char_sets.setlist
 
 
 def protocols():
     """Return a list of values from the IANA Service Name and Transport
-    Protocol Port Number Registry, or an empty list if the IANA website is
-    unreachable.
+    Protocol Port Number Registry.
     Store it as a function attribute so that we only build the list once.
     """
     if not hasattr(protocols, 'protlist'):
-        plist = []
-        try:
-            data = requests.get('http://www.iana.org/assignments/service-names'
-                                '-port-numbers/service-names-port-numbers.csv')
-        except requests.exceptions.RequestException:
-            return []
-
-        for line in data.iter_lines():
-            if line:
-                line = line.decode("utf-8")
-                if line.count(',') > 0:
-                    vals = line.split(',')
-                    if vals[0]:
-                        plist.append(vals[0])
-                    if len(vals) > 2 and vals[2] and vals[2] not in plist:
-                        plist.append(vals[2])
-
-        plist.append('ipv4')
-        plist.append('ipv6')
-        plist.append('ssl')
-        plist.append('tls')
-        plist.append('dns')
+        basepath = os.path.abspath(os.path.dirname(__file__))
+        plist = set()
+        with open(basepath + '/assets/protocols.csv', 'r', encoding='utf-8') as fd:
+            reader = csv.DictReader(fd)
+            for row in reader:
+                name = row.get('Service Name')
+                transport_protocol = row.get('Transport Protocol')
+                if name:
+                    plist.add(name)
+                if transport_protocol:
+                    plist.add(transport_protocol)
+
+        plist.add('ipv4')
+        plist.add('ipv6')
+        plist.add('ssl')
+        plist.add('tls')
+        plist.add('dns')
+        plist = sorted(plist)
         protocols.protlist = plist
     return protocols.protlist
 
 
 def ipfix():
     """Return a list of values from the list of IANA IP Flow Information Export
-    (IPFIX) Entities, or an empty list if the IANA website is unreachable.
+    (IPFIX) Entities.
     Store it as a function attribute so that we only build the list once.
     """
     if not hasattr(ipfix, 'ipflist'):
+        basepath = os.path.abspath(os.path.dirname(__file__))
         ilist = []
-        try:
-            data = requests.get('http://www.iana.org/assignments/ipfix/ipfix-'
-                                'information-elements.csv')
-        except requests.exceptions.RequestException:
-            return []
-
-        for line in data.iter_lines():
-            if line:
-                line = line.decode("utf-8")
-                if re.match(r'^\d+(,[a-zA-Z0-9]+){2},', line):
-                    vals = line.split(',')
-                    if vals[1]:
-                        ilist.append(vals[1])
-
+        with open(basepath + '/assets/ipfix-information-elements.csv', 'r', encoding='utf-8') as fd:
+            reader = csv.DictReader(fd)
+            for row in reader:
+                name = row.get('Name')
+                if name:
+                    ilist.append(name)
         ipfix.ipflist = ilist
     return ipfix.ipflist
 
 
 # If you have a Socket Option not present in this list
 # for SO|ICMP|ICMP6|IP|IPV6|MCAST|TCP|IRLMP please open an issue/PR
 # in https://github.com/oasis-open/cti-stix-validator/ to include it.
```

### Comparing `stix2-validator-3.1.4/stix2validator/v21/errors.py` & `stix2-validator-3.2.0/stix2validator/v21/errors.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/v21/interop.py` & `stix2-validator-3.2.0/stix2validator/v21/interop.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/v21/musts.py` & `stix2-validator-3.2.0/stix2validator/v21/musts.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/v21/shoulds.py` & `stix2-validator-3.2.0/stix2validator/v21/shoulds.py`

 * *Files identical despite different names*

### Comparing `stix2-validator-3.1.4/stix2validator/validator.py` & `stix2-validator-3.2.0/stix2validator/validator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 """Custom jsonschema.IValidator class and validator functions.
 """
 
 from collections.abc import Iterable
+import copy
+import functools
 import io
 from itertools import chain
 import os
+import pathlib
 import re
 import sys
+from urllib import parse, request
 
-from jsonschema import Draft202012Validator, RefResolver
+from jsonschema import Draft202012Validator
 from jsonschema import exceptions as schema_exceptions
 from jsonschema.validators import extend
+from referencing import Registry, Resource
+from referencing.jsonschema import DRAFT202012
+import requests
 import simplejson as json
 
 from . import output
 from .errors import (NoJSONFileFoundError, SchemaError, SchemaInvalidError,
                      ValidationError, pretty_error)
-from .util import (DEFAULT_VER, ValidationOptions, clear_requests_cache,
-                   init_requests_cache)
+from .util import DEFAULT_VER, ValidationOptions
 from .v20 import musts as musts20
 from .v20 import shoulds as shoulds20
 from .v21 import interop
 from .v21 import musts as musts21
 from .v21 import shoulds as shoulds21
 
 try:
@@ -386,17 +392,14 @@
     """
 
     validating_list = isinstance(obj_json, list)
 
     if not options:
         options = ValidationOptions()
 
-    if not options.no_cache:
-        init_requests_cache(options.refresh_cache)
-
     results = None
     if validating_list:
         results = []
         for obj in obj_json:
             try:
                 results.append(validate_instance(obj, options))
             except SchemaInvalidError as ex:
@@ -409,17 +412,14 @@
             results = validate_instance(obj_json, options)
         except SchemaInvalidError as ex:
             error_result = ObjectValidationResults(is_valid=False,
                                                    object_id=obj_json.get('id', ''),
                                                    errors=[str(ex)])
             results = error_result
 
-    if not options.no_cache and options.clear_cache:
-        clear_requests_cache()
-
     return results
 
 
 def validate(in_, options=None):
     """
     Validate objects from JSON data in a textual stream.
 
@@ -451,15 +451,15 @@
     file_results = FileValidationResults(filepath=fn)
     output.info("Performing JSON schema validation on %s" % fn)
 
     if not options:
         options = ValidationOptions(files=fn)
 
     try:
-        with open(fn) as instance_file:
+        with open(fn, encoding="utf-8") as instance_file:
             file_results.object_results = validate(instance_file, options)
 
     except Exception as ex:
         if 'Expecting value' in str(ex):
             line_no = str(ex).split()[3]
             file_results.fatal = ValidationErrorResults(
                 'Invalid JSON input on line %s' % line_no
@@ -493,82 +493,123 @@
 
     """
     output.info("Performing JSON schema validation on input string: " + string)
     stream = io.StringIO(string)
     return validate(stream, options)
 
 
-SCHEMA_STORE = {}
+STIXValidator = extend(Draft202012Validator)
+
+
+# Built-in checker only ensures emails contain an '@'; we want a more robust check
+@Draft202012Validator.FORMAT_CHECKER.checks('email')
+def is_email(instance):
+    if not isinstance(instance, str):
+        return True
+    return EMAIL_RE.match(instance)
+
 
+def from_uri_to_path(uri: str) -> str:
+    """Convert a URI to a file path if possible.
 
-def ref_store(validator, ref, instance, schema):
-    """When validating '$ref' properties, add to global store.
+    Note: replace with 'Path.from_uri(schema_path_uri)' when Python 3.13.
+
+    Args:
+        uri: the URI, potentially containing a file path.
+
+    Returns:
+        The file path if the URI contains a file path, the URI otherwise.
     """
-    remote_path = validator.resolver._urljoin_cache(validator.resolver.base_uri, ref)
+    parsed_url = parse.urlparse(uri)
+    if parsed_url.scheme == "file":
+        return request.url2pathname(parsed_url.path)
+    else:
+        return uri
 
-    if remote_path not in validator.resolver.store:
-        # Add local schema to Resolver store if present, so validator will use local
-        # schemas and only download remote refs in local is not present.
-        local_base_uri = validator.resolver._scopes_stack[0]
 
-        # Take out the the 'file:' prefix
-        if os.name == 'nt':
-            local_base_uri = local_base_uri[8:]
-        else:
-            local_base_uri = local_base_uri[5:]
+def patch_schema(schema_data: dict, schema_path: str) -> dict:
+    """Patch schemas with two important fixes.
 
-        try:
-            local_filepath = os.path.abspath(os.path.join(local_base_uri, '../'+ref))
-            local_schema = load_schema(local_filepath)
-            schema_id = local_schema.get('$id', '')
-            if schema_id:
-                validator.resolver.store[schema_id] = local_schema
-        except FileNotFoundError:
-            pass
+    1) _SPECIFICATIONS dictionary inside referencing.jsonschema is a mapping
+        between URLs and validators; 'DRAFT201909' and 'DRAFT202012' are now
+        only recognized as such if the URLs is https://.
 
-    return Draft202012Validator.VALIDATORS['$ref'](validator, ref, instance, schema)
+    2) For relative references to work, the $id of the schema needs to point
+        to a valid URI or path, that can later be used as a key to retrieve
+        a loaded resource.
 
+    Args:
+        schema_data: the schema itself.
+        schema_path: the path of the schema (can be both URI or path).
 
-STIXValidator = extend(Draft202012Validator, {'$ref': ref_store})
+    Returns:
+        The patched schema.
+    """
+    schema_data = copy.copy(schema_data)
+    if "$schema" in schema_data:
+        schema_data["$schema"] = schema_data["$schema"].replace(
+            "http://json-schema.org/draft/", "https://json-schema.org/draft/"
+        )
+    if "$id" in schema_data:
+        schema_path = pathlib.Path(schema_path)
+        if schema_path.is_absolute():
+            schema_data["$id"] = str(schema_path.as_uri())
+        else:
+            schema_data["$id"] = str(schema_path)
+    return schema_data
 
 
-# Built-in checker only ensures emails contain an '@'; we want a more robust check
-@Draft202012Validator.FORMAT_CHECKER.checks('email')
-def is_email(instance):
-    if not isinstance(instance, str):
-        return True
-    return EMAIL_RE.match(instance)
+def retrieve_from_filesystem(schema_path_uri: str, schema_dir: str) -> Resource:
+    """Callback to retrieve a schema given its path.
+
+    Args:
+        schema_path_uri: the schema URI.
+        schema_dir: the optional directory of local schemas.
 
+    Returns:
+        A resource loaded with the content.
+    """
+    if schema_path_uri.startswith("http://") or schema_path_uri.startswith("https://"):
+        response = requests.get(schema_path_uri, allow_redirects=True)
+        schema = response.json()
+        schema = patch_schema(schema, schema_path_uri)
+        return Resource.from_contents(schema)
+    else:
+        schema_path = pathlib.Path(schema_path_uri)
+        if schema_path.is_absolute() or schema_path_uri.startswith("file://"):
+            is_relative = False
+            schema_path = from_uri_to_path(schema_path_uri)
+        else:
+            is_relative = True
+            schema_path = from_uri_to_path(os.path.join(schema_dir, schema_path_uri))
+        with open(schema_path, "r") as f:
+            schema = json.load(f)
+        schema = patch_schema(schema, schema_path)
+        if is_relative:
+            return Resource.opaque(schema)
+        else:
+            return Resource.from_contents(schema)
 
-def load_validator(schema_path, schema):
+
+def load_validator(schema_path, schema, schema_dir):
     """Create a JSON schema validator for the given schema.
 
     Args:
         schema_path: The filename of the JSON schema.
         schema: A Python object representation of the same schema.
 
     Returns:
         An instance of Draft202012Validator.
-
     """
-    global SCHEMA_STORE
-
-    # Get correct prefix based on OS
-    if os.name == 'nt':
-        file_prefix = 'file:///'
-    else:
-        file_prefix = 'file:'
-
-    resolver = RefResolver(file_prefix + schema_path.replace("\\", "/"), schema, store=SCHEMA_STORE)
-    schema_id = schema.get('$id', '')
-    if schema_id:
-        resolver.store[schema_id] = schema
-    # RefResolver creates a new store internally; persist it so we can use the same mappings every time
-    SCHEMA_STORE = resolver.store
-    validator = STIXValidator(schema, resolver=resolver, format_checker=Draft202012Validator.FORMAT_CHECKER)
+    schema = patch_schema(schema, schema_path)
+    retrieve_callback = functools.partial(retrieve_from_filesystem, schema_dir=schema_dir)
+    registry = Registry(
+        retrieve=retrieve_callback
+    ).with_resource(schema_path, DRAFT202012.create_resource(schema))
+    validator = STIXValidator(schema,  registry=registry, format_checker=Draft202012Validator.FORMAT_CHECKER)
     return validator
 
 
 def find_schema(schema_dir, name):
     """Search the `schema_dir` directory for a schema called `name`.json.
     Return the file path of the first match it finds.
     """
@@ -664,15 +705,15 @@
             "objects": {
                 "type": "array",
                 "minItems": 1
             }
         }
 
     # Don't use custom validator; only check schemas, no additional checks
-    validator = load_validator(schema_path, schema)
+    validator = load_validator(schema_path, schema, schema_dir)
     try:
         error_gen = validator.iter_errors(obj)
     except schema_exceptions.RefResolutionError:
         raise SchemaInvalidError('Invalid JSON schema: a JSON '
                                  'reference failed to resolve')
     return error_gen
```

