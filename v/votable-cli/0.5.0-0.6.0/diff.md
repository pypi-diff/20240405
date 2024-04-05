# Comparing `tmp/votable_cli-0.5.0.tar.gz` & `tmp/votable_cli-0.6.0.tar.gz`

## Comparing `votable_cli-0.5.0.tar` & `votable_cli-0.6.0.tar`

### file list

```diff
@@ -1,98 +1,102 @@
--rw-r--r--   0     1001      127      310 2024-03-11 14:15:53.000000 votable_cli-0.5.0/.github/workflows/clitest.yml
--rw-r--r--   0     1001      127     5890 2024-03-11 14:15:53.000000 votable_cli-0.5.0/.github/workflows/deploy.yml
--rw-r--r--   0     1001      127      460 2024-03-11 14:15:53.000000 votable_cli-0.5.0/.github/workflows/libtest.yml
--rw-r--r--   0     1001      127     6049 2024-03-11 14:15:53.000000 votable_cli-0.5.0/.github/workflows/release.yml
--rw-r--r--   0     1001      127      454 2024-03-11 14:15:53.000000 votable_cli-0.5.0/.github/workflows/wasmtest.yml
--rw-r--r--   0     1001      127     2681 2024-03-11 14:15:53.000000 votable_cli-0.5.0/CHANGELOG.md
--rw-r--r--   0     1001      127    10852 2024-03-11 14:15:53.000000 votable_cli-0.5.0/LICENSE-APACHE
--rw-r--r--   0     1001      127     1076 2024-03-11 14:15:53.000000 votable_cli-0.5.0/LICENSE-MIT
--rw-r--r--   0     1001      127    20424 2024-03-11 14:15:53.000000 votable_cli-0.5.0/README.md
--rw-r--r--   0     1001      127       14 2024-03-11 14:15:53.000000 votable_cli-0.5.0/rustfmt.toml
--rw-r--r--   0     1001      127    19341 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/coosys.rs
--rw-r--r--   0     1001      127     5534 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/data/binary.rs
--rw-r--r--   0     1001      127     5583 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/data/binary2.rs
--rw-r--r--   0     1001      127     3863 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/data/fits.rs
--rw-r--r--   0     1001      127    12617 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/data/mod.rs
--rw-r--r--   0     1001      127    10081 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/data/stream.rs
--rw-r--r--   0     1001      127    10220 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/data/tabledata.rs
--rw-r--r--   0     1001      127     2159 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/datatype.rs
--rw-r--r--   0     1001      127     5190 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/definitions.rs
--rw-r--r--   0     1001      127     4019 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/desc.rs
--rw-r--r--   0     1001      127     3218 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/error.rs
--rw-r--r--   0     1001      127    24793 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/field.rs
--rw-r--r--   0     1001      127     4289 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/fieldref.rs
--rw-r--r--   0     1001      127    16603 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/group.rs
--rw-r--r--   0     1001      127      123 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/impls/b64/mod.rs
--rw-r--r--   0     1001      127    21027 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/impls/b64/read.rs
--rw-r--r--   0     1001      127    10026 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/impls/b64/write.rs
--rw-r--r--   0     1001      127    15681 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/impls/mem.rs
--rw-r--r--   0     1001      127    59686 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/impls/mod.rs
--rw-r--r--   0     1001      127     6445 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/impls/visitors.rs
--rw-r--r--   0     1001      127     8316 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/info.rs
--rw-r--r--   0     1001      127    10646 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/iter/elems.rs
--rw-r--r--   0     1001      127    43291 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/iter/mod.rs
--rw-r--r--   0     1001      127     1772 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/iter/strings.rs
--rw-r--r--   0     1001      127    23552 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/lib.rs
--rw-r--r--   0     1001      127     6172 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/link.rs
--rw-r--r--   0     1001      127    18596 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/macros.rs
--rw-r--r--   0     1001      127    13957 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/attribute.rs
--rw-r--r--   0     1001      127     7036 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/globals/collection/instance.rs
--rw-r--r--   0     1001      127     8938 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/globals/collection/mod.rs
--rw-r--r--   0     1001      127     1054 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/globals/collection/reference.rs
--rw-r--r--   0     1001      127    10952 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/globals/instance/collection/collection.rs
--rw-r--r--   0     1001      127    10211 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/globals/instance/collection/mod.rs
--rw-r--r--   0     1001      127     6281 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/globals/instance/instance.rs
--rw-r--r--   0     1001      127     7447 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/globals/instance/mod.rs
--rw-r--r--   0     1001      127     3259 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/globals/instance/primary_key.rs
--rw-r--r--   0     1001      127     1451 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/globals/instance/reference.rs
--rw-r--r--   0     1001      127     4976 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/globals/mod.rs
--rw-r--r--   0     1001      127     7637 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/join/mod.rs
--rw-r--r--   0     1001      127     2236 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/join/where.rs
--rw-r--r--   0     1001      127    20960 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/macros.rs
--rw-r--r--   0     1001      127     6563 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/mod.rs
--rw-r--r--   0     1001      127     2066 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/model.rs
--rw-r--r--   0     1001      127     3265 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/report.rs
--rw-r--r--   0     1001      127    10913 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/templates/instance/collection/collection.rs
--rw-r--r--   0     1001      127    10221 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/templates/instance/collection/mod.rs
--rw-r--r--   0     1001      127     6584 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/templates/instance/collection/reference.rs
--rw-r--r--   0     1001      127     6258 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/templates/instance/instance.rs
--rw-r--r--   0     1001      127     7243 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/templates/instance/mod.rs
--rw-r--r--   0     1001      127     4562 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/templates/instance/primary_key.rs
--rw-r--r--   0     1001      127     1632 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/templates/instance/reference/foreign_key.rs
--rw-r--r--   0     1001      127     7424 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/templates/instance/reference/mod.rs
--rw-r--r--   0     1001      127     5930 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/templates/mod.rs
--rw-r--r--   0     1001      127     1100 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/templates/where.rs
--rw-r--r--   0     1001      127     3395 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/visitors/donothing.rs
--rw-r--r--   0     1001      127       19 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/visitors/mod.rs
--rw-r--r--   0     1001      127    11708 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/mivot/vodml.rs
--rw-r--r--   0     1001      127    10667 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/param.rs
--rw-r--r--   0     1001      127     4289 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/paramref.rs
--rw-r--r--   0     1001      127    34001 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/resource.rs
--rw-r--r--   0     1001      127    16340 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/table.rs
--rw-r--r--   0     1001      127    12725 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/timesys.rs
--rw-r--r--   0     1001      127      876 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/utils.rs
--rw-r--r--   0     1001      127    16689 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/values.rs
--rw-r--r--   0     1001      127    44194 2024-03-11 14:15:53.000000 votable_cli-0.5.0/src/votable.rs
--rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 votable_cli-0.5.0/crates/cli/Cargo.toml
--rw-r--r--   0     1001      127     1547 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/CHANGELOG.md
--rw-r--r--   0     1001      127      123 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/COPYING
--rw-r--r--   0     1001      127    10852 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/LICENSE-APACHE
--rw-r--r--   0     1001      127     1076 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/LICENSE-MIT
--rw-r--r--   0     1001      127     8152 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/README.md
--rw-r--r--   0     1001      127      962 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/doc/vot.1.txt.tpl
--rw-r--r--   0     1001      127      432 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/src/convert.rs
--rw-r--r--   0     1001      127     7282 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/src/get.rs
--rw-r--r--   0     1001      127     3680 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/src/input.rs
--rw-r--r--   0     1001      127      117 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/src/lib.rs
--rw-r--r--   0     1001      127      671 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/src/main.rs
--rw-r--r--   0     1001      127     2641 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/src/output.rs
--rw-r--r--   0     1001      127    27461 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/src/streaming.rs
--rw-r--r--   0     1001      127     5465 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/src/visitors/colnames.rs
--rw-r--r--   0     1001      127     9247 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/src/visitors/fieldarray.rs
--rw-r--r--   0     1001      127     2772 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/src/visitors/mod.rs
--rw-r--r--   0     1001      127     6136 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/src/visitors/viz_org_names.rs
--rw-r--r--   0     1001      127    21974 2024-03-11 14:15:53.000000 votable_cli-0.5.0/crates/cli/src/visitors/votstruct.rs
--rw-r--r--   0        0        0    16170 2024-03-11 14:16:06.000000 votable_cli-0.5.0/Cargo.lock
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 votable_cli-0.5.0/Cargo.toml
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 votable_cli-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     8939 1970-01-01 00:00:00.000000 votable_cli-0.5.0/PKG-INFO
+-rw-r--r--   0     1001      127      310 2024-04-05 15:04:23.000000 votable_cli-0.6.0/.github/workflows/clitest.yml
+-rw-r--r--   0     1001      127     5890 2024-04-05 15:04:23.000000 votable_cli-0.6.0/.github/workflows/deploy.yml
+-rw-r--r--   0     1001      127      460 2024-04-05 15:04:23.000000 votable_cli-0.6.0/.github/workflows/libtest.yml
+-rw-r--r--   0     1001      127     6049 2024-04-05 15:04:23.000000 votable_cli-0.6.0/.github/workflows/release.yml
+-rw-r--r--   0     1001      127      454 2024-04-05 15:04:23.000000 votable_cli-0.6.0/.github/workflows/wasmtest.yml
+-rw-r--r--   0     1001      127     3427 2024-04-05 15:04:23.000000 votable_cli-0.6.0/CHANGELOG.md
+-rw-r--r--   0     1001      127    10852 2024-04-05 15:04:23.000000 votable_cli-0.6.0/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1076 2024-04-05 15:04:23.000000 votable_cli-0.6.0/LICENSE-MIT
+-rw-r--r--   0     1001      127    20424 2024-04-05 15:04:23.000000 votable_cli-0.6.0/README.md
+-rw-r--r--   0     1001      127       14 2024-04-05 15:04:23.000000 votable_cli-0.6.0/rustfmt.toml
+-rw-r--r--   0     1001      127    21938 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/coosys.rs
+-rw-r--r--   0     1001      127     5035 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/data/binary.rs
+-rw-r--r--   0     1001      127     5043 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/data/binary2.rs
+-rw-r--r--   0     1001      127     3922 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/data/fits.rs
+-rw-r--r--   0     1001      127    12349 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/data/mod.rs
+-rw-r--r--   0     1001      127     9557 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/data/stream.rs
+-rw-r--r--   0     1001      127    10363 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/data/tabledata.rs
+-rw-r--r--   0     1001      127     2159 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/datatype.rs
+-rw-r--r--   0     1001      127     4529 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/definitions.rs
+-rw-r--r--   0     1001      127     4019 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/desc.rs
+-rw-r--r--   0     1001      127     3243 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/error.rs
+-rw-r--r--   0     1001      127    24085 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/field.rs
+-rw-r--r--   0     1001      127     3377 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/fieldref.rs
+-rw-r--r--   0     1001      127    13983 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/group.rs
+-rw-r--r--   0     1001      127      123 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/impls/b64/mod.rs
+-rw-r--r--   0     1001      127    21027 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/impls/b64/read.rs
+-rw-r--r--   0     1001      127    10026 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/impls/b64/write.rs
+-rw-r--r--   0     1001      127    15678 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/impls/mem.rs
+-rw-r--r--   0     1001      127    59686 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/impls/mod.rs
+-rw-r--r--   0     1001      127     6445 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/impls/visitors.rs
+-rw-r--r--   0     1001      127     7116 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/info.rs
+-rw-r--r--   0     1001      127    10643 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/iter/elems.rs
+-rw-r--r--   0     1001      127    43288 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/iter/mod.rs
+-rw-r--r--   0     1001      127     1772 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/iter/strings.rs
+-rw-r--r--   0     1001      127    34182 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/lib.rs
+-rw-r--r--   0     1001      127     4955 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/link.rs
+-rw-r--r--   0     1001      127    32733 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/macros.rs
+-rw-r--r--   0     1001      127    14070 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/attribute.rs
+-rw-r--r--   0     1001      127     6485 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/collection/instance.rs
+-rw-r--r--   0     1001      127     9264 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/collection/mod.rs
+-rw-r--r--   0     1001      127     2147 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/collection/reference.rs
+-rw-r--r--   0     1001      127    11272 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/instance/collection/collection.rs
+-rw-r--r--   0     1001      127    10606 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/instance/collection/mod.rs
+-rw-r--r--   0     1001      127     5683 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/instance/instance.rs
+-rw-r--r--   0     1001      127     6945 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/instance/mod.rs
+-rw-r--r--   0     1001      127     3447 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/instance/primary_key.rs
+-rw-r--r--   0     1001      127     2790 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/instance/reference.rs
+-rw-r--r--   0     1001      127     5985 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/mod.rs
+-rw-r--r--   0     1001      127     8634 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/join/mod.rs
+-rw-r--r--   0     1001      127     3587 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/join/where.rs
+-rw-r--r--   0     1001      127     8218 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/mod.rs
+-rw-r--r--   0     1001      127     3319 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/model.rs
+-rw-r--r--   0     1001      127     3066 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/report.rs
+-rw-r--r--   0     1001      127    11235 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/collection/collection.rs
+-rw-r--r--   0     1001      127    10618 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/collection/mod.rs
+-rw-r--r--   0     1001      127     7200 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/collection/reference.rs
+-rw-r--r--   0     1001      127     5659 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/instance.rs
+-rw-r--r--   0     1001      127     6848 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/mod.rs
+-rw-r--r--   0     1001      127     4983 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/primary_key.rs
+-rw-r--r--   0     1001      127     2491 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/reference/foreign_key.rs
+-rw-r--r--   0     1001      127     8031 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/reference/mod.rs
+-rw-r--r--   0     1001      127     6510 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/mod.rs
+-rw-r--r--   0     1001      127     2499 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/where.rs
+-rw-r--r--   0     1001      127     5529 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/visitors/donothing.rs
+-rw-r--r--   0     1001      127       19 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/visitors/mod.rs
+-rw-r--r--   0     1001      127    10659 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/vodml.rs
+-rw-r--r--   0     1001      127     8247 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/param.rs
+-rw-r--r--   0     1001      127     3333 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/paramref.rs
+-rw-r--r--   0     1001      127    35855 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/resource.rs
+-rw-r--r--   0     1001      127    15234 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/table.rs
+-rw-r--r--   0     1001      127    11556 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/timesys.rs
+-rw-r--r--   0     1001      127     1215 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/utils.rs
+-rw-r--r--   0     1001      127    13247 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/values.rs
+-rw-r--r--   0     1001      127    43953 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/votable.rs
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 votable_cli-0.6.0/crates/cli/Cargo.toml
+-rw-r--r--   0     1001      127     1625 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/CHANGELOG.md
+-rw-r--r--   0     1001      127      123 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/COPYING
+-rw-r--r--   0     1001      127    10852 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1076 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/LICENSE-MIT
+-rw-r--r--   0     1001      127    16159 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/README.md
+-rw-r--r--   0     1001      127     1981 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/doc/vot.1.txt.tpl
+-rwxr-xr-x   0     1001      127     1572 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/resource/test_edit.bash
+-rw-r--r--   0     1001      127     8406 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/resource/test_edit.td.xml
+-rw-r--r--   0     1001      127      432 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/convert.rs
+-rw-r--r--   0     1001      127    26312 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/edit.rs
+-rw-r--r--   0     1001      127     7370 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/get.rs
+-rw-r--r--   0     1001      127     3786 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/input.rs
+-rw-r--r--   0     1001      127      134 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/lib.rs
+-rw-r--r--   0     1001      127      943 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/main.rs
+-rw-r--r--   0     1001      127     2902 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/output.rs
+-rw-r--r--   0     1001      127    27220 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/streaming.rs
+-rw-r--r--   0     1001      127     5465 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/visitors/colnames.rs
+-rw-r--r--   0     1001      127     9247 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/visitors/fieldarray.rs
+-rw-r--r--   0     1001      127     4803 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/visitors/mod.rs
+-rw-r--r--   0     1001      127    37629 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/visitors/update.rs
+-rw-r--r--   0     1001      127     6160 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/visitors/viz_org_names.rs
+-rw-r--r--   0     1001      127    22004 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/visitors/votstruct.rs
+-rw-r--r--   0     1001      127    33344 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/wrappedelems.rs
+-rw-r--r--   0        0        0    16181 2024-04-05 15:04:36.000000 votable_cli-0.6.0/Cargo.lock
+-rw-r--r--   0        0        0     1999 1970-01-01 00:00:00.000000 votable_cli-0.6.0/Cargo.toml
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 votable_cli-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    16946 1970-01-01 00:00:00.000000 votable_cli-0.6.0/PKG-INFO
```

### Comparing `votable_cli-0.5.0/.github/workflows/deploy.yml` & `votable_cli-0.6.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/.github/workflows/release.yml` & `votable_cli-0.6.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/CHANGELOG.md` & `votable_cli-0.6.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 # `votable` Change Log
 
+## 0.6.0
+
+Released 2024-04-05
+
+### Changed
+
+* ⚠️  BREAKING: the tag is now in the `VOTableTrait` instead of the `QuickXmlReadWrite` trait 
+* ⚠️  BREAKING: extra attribute names (allowed in some Tags in the lib, but not in the standard) 
+  must contains ':'. If not, a prefix 'extra:' is automatically addded by the API (not when deserializing)
+* ⚠️  BREAKING: update the MIVOT visitor to consistent with the VOTable visitor
+* Add `for_each_attribute` in MIVOT tags
+* Add setters
+* Add documentation
+* Internal changes: 
+    + add trait `VOTableElement` for more genericity and to lighten the role of the `QuickXMLReadWrite` trait 
+    + add markers trait to distinguish between several `VOTableElement` patterns
+    + remove macros
+
+
 ## 0.5.0
 
 Released 2024-03-11
 
 ### Added
 
 * Add genericity and remove (some) duplicated code
```

### Comparing `votable_cli-0.5.0/LICENSE-APACHE` & `votable_cli-0.6.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/LICENSE-MIT` & `votable_cli-0.6.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/README.md` & `votable_cli-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/src/coosys.rs` & `votable_cli-0.6.0/src/coosys.rs`

 * *Files 15% similar despite different names*

```diff
@@ -3,29 +3,25 @@
 use std::{
   fmt::{self, Display, Formatter},
   io::{BufRead, Write},
   num::ParseFloatError,
   str::{self, FromStr},
 };
 
-use log::warn;
+use log::trace;
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
-  ElementWriter, Reader, Writer,
-};
-// use serde;
+use quick_xml::{events::Event, Reader, Writer};
 
 use crate::{
   error::VOTableError,
   fieldref::FieldRef,
   paramref::ParamRef,
   timesys::RefPosition,
-  utils::{discard_comment, discard_event},
-  QuickXmlReadWrite, TableDataContent, VOTableVisitor,
+  utils::{discard_comment, discard_event, unexpected_attr_warn},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, TableDataContent, VOTableElement, VOTableVisitor,
 };
 
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "elem_type")]
 pub enum CooSysElem {
   FieldRef(FieldRef),
   ParamRef(ParamRef),
@@ -46,14 +42,15 @@
     match self {
       CooSysElem::FieldRef(e) => e.visit(visitor),
       CooSysElem::ParamRef(e) => e.visit(visitor),
     }
   }
 }
 
+/// Struct corresponding to the `COOSYS` XML tag.
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct CooSys {
   #[serde(rename = "ID")]
   pub id: String,
   #[serde(flatten)]
   pub coosys: System,
   /// We so far put `refposition` as Optional to stay compatible with VOTable 1.4
@@ -71,204 +68,173 @@
       id: id.into(),
       coosys,
       refposition: None,
       elems: Default::default(),
     }
   }
 
-  /// Calls a closure on each (key, value) attribute pairs.
-  pub fn for_each_attribute<F>(&self, mut f: F)
-  where
-    F: FnMut(&str, &str),
-  {
-    f("ID", self.id.as_str());
-    self.coosys.for_each_attribute(&mut f);
-    if let Some(refposition) = &self.refposition {
-      f("refposition", refposition.to_string().as_str());
-    }
-  }
+  // attributes
+  impl_builder_mandatory_string_attr!(id);
+  impl_builder_mandatory_attr!(coosys, System);
+  impl_builder_opt_attr!(refposition, RefPosition);
+  /// Use for modification.
+  /// No `set_equinox` for construction since we have `set_coosys`.
+  pub fn set_equinox_by_ref<S: AsRef<str>>(&mut self, epoch: S) -> Result<(), VOTableError> {
+    self.coosys.set_equinox_from_str_by_ref(epoch.as_ref())
+  }
+  /// Use for modification.
+  /// No `set_epoch` for construction since we have `set_coosys`.
+  pub fn set_epoch_by_ref<S: AsRef<str>>(&mut self, epoch: S) -> Result<(), VOTableError> {
+    self.coosys.set_epoch_from_str_by_ref(epoch.as_ref())
+  }
+  // sub-elements
+  impl_builder_push_elem!(FieldRef, CooSysElem);
+  impl_builder_push_elem!(ParamRef, CooSysElem);
 
   pub fn visit<C, V>(&mut self, visitor: &mut V) -> Result<(), V::E>
   where
     C: TableDataContent,
     V: VOTableVisitor<C>,
   {
     visitor.visit_coosys_start(self)?;
     for elem in &mut self.elems {
       elem.visit(visitor)?;
     }
     visitor.visit_coosys_ended(self)
   }
-
-  impl_builder_opt_attr!(refposition, RefPosition);
 }
 
-impl QuickXmlReadWrite for CooSys {
+impl VOTableElement for CooSys {
   const TAG: &'static str = "COOSYS";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
     let mut id: Option<String> = None;
     let mut system: Option<String> = None;
     let mut equinox: Option<String> = None;
     let mut epoch: Option<String> = None;
     let mut refposition: Option<RefPosition> = None;
     // Look for attributes
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let value =
-        String::from_utf8(attr.value.as_ref().to_vec()).map_err(VOTableError::FromUtf8)?;
-      match attr.key {
-        b"ID" => id = Some(value),
-        b"system" => system = Some(value),
-        b"equinox" => equinox = Some(value),
-        b"epoch" => epoch = Some(value),
-        b"refposition" => refposition = Some(value.parse().map_err(VOTableError::Variant)?),
-        _ => {
-          warn!(
-            "Attribute {:?} in {} is ignored",
-            std::str::from_utf8(attr.key),
-            Self::TAG
-          );
-        }
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "ID" => id = Some(val.into()),
+        "system" => system = Some(val.into()),
+        "equinox" => equinox = Some(val.into()),
+        "epoch" => epoch = Some(val.into()),
+        "refposition" => refposition = Some(val.as_ref().parse().map_err(VOTableError::Variant)?),
+        _ => unexpected_attr_warn(key, Self::TAG),
       }
     }
     // Set from found attributes
     if let (Some(id), Some(system)) = (id, system) {
-      let mut system = match system.as_str() {
-        "eq_FK4" => {
-          if let Some(equinox) = equinox {
-            System::new_eq_fk4(
-              equinox
-                .parse::<BesselianYear>()
-                .map_err(VOTableError::ParseYear)?
-                .0,
-            )
-          } else {
-            System::new_default_eq_fk4()
-          }
-        }
-        "eq_FK5" => {
-          if let Some(equinox) = equinox {
-            System::new_eq_fk5(
-              equinox
-                .parse::<JulianYear>()
-                .map_err(VOTableError::ParseYear)?
-                .0,
-            )
-          } else {
-            System::new_default_eq_fk5()
-          }
-        }
-        "ICRS" => System::new_icrs(),
-        "ecl_FK4" => {
-          if let Some(equinox) = equinox {
-            System::new_ecl_fk4(
-              equinox
-                .parse::<BesselianYear>()
-                .map_err(VOTableError::ParseYear)?
-                .0,
-            )
-          } else {
-            System::new_default_ecl_fk4()
-          }
-        }
-        "ecl_FK5" => {
-          if let Some(equinox) = equinox {
-            System::new_ecl_fk5(
-              equinox
-                .parse::<JulianYear>()
-                .map_err(VOTableError::ParseYear)?
-                .0,
-            )
-          } else {
-            System::new_default_ecl_fk5()
-          }
-        }
-        "galactic" => System::new_galactic(),
-        "supergalactic" => System::new_supergalactic(),
-        _ => {
-          return Err(VOTableError::Custom(format!(
-            "System '{}' not recognized in tag '{}'",
-            system,
-            Self::TAG
-          )));
-        }
-      };
+      // Create and set system
+      let mut system = equinox
+        .map(|equinox| System::from_system_and_equinox(&system, equinox))
+        .unwrap_or(System::from_system(system))?;
       if let Some(epoch) = epoch {
-        system = system
-          .set_epoch_from_str(epoch.as_str())
-          .map_err(VOTableError::ParseYear)?;
+        system.set_epoch_from_str_by_ref(epoch)?;
       }
-      // Create CooSys
+      // Create and set CooSys
       let mut coosys = CooSys::new(id, system);
-      // Add refposition if any
       if let Some(refposition) = refposition {
-        coosys = coosys.set_refposition(refposition);
+        coosys.set_refposition_by_ref(refposition);
       }
       Ok(coosys)
     } else {
       Err(VOTableError::Custom(format!(
         "Attributes 'ID' and 'system' are mandatory in tag '{}'",
         Self::TAG
       )))
     }
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, context)
-      .map(|()| reader)
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    let mut system: Option<String> = None;
+    let mut equinox: Option<String> = None;
+    let mut epoch: Option<String> = None;
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "ID" => self.set_id_by_ref(val),
+        "refposition" => {
+          self.set_refposition_by_ref(val.as_ref().parse().map_err(VOTableError::Variant)?)
+        }
+        "system" => system = Some(val.into()),
+        "equinox" => equinox = Some(val.into()),
+        "epoch" => epoch = Some(val.into()),
+        _ => unexpected_attr_warn(key, Self::TAG),
+      }
+    }
+    match (system, equinox) {
+      (Some(system), Some(equinox)) => {
+        self.coosys = System::from_system_and_equinox(system, equinox)?
+      }
+      (Some(system), None) => self.coosys = System::from_system(system)?,
+      (None, Some(equinox)) => self.coosys.set_equinox_from_str_by_ref(equinox)?,
+      (None, None) => {}
+    }
+    if let Some(epoch) = epoch {
+      self.coosys.set_epoch_from_str_by_ref(epoch.as_str())?;
+    }
+    Ok(())
+  }
+
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    f("ID", self.id.as_str());
+    self.coosys.for_each_attribute(&mut f);
+    if let Some(refposition) = &self.refposition {
+      f("refposition", refposition.to_string().as_str());
+    }
+  }
+}
+
+impl HasSubElements for CooSys {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    self.elems.is_empty()
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          FieldRef::TAG_BYTES => self
-            .elems
-            .push(CooSysElem::FieldRef(from_event_start_by_ref!(
-              FieldRef,
-              reader,
-              reader_buff,
-              e
-            ))),
-          ParamRef::TAG_BYTES => self
-            .elems
-            .push(CooSysElem::ParamRef(from_event_start_by_ref!(
-              ParamRef,
-              reader,
-              reader_buff,
-              e
-            ))),
+          FieldRef::TAG_BYTES => push_from_event_start!(self, FieldRef, reader, reader_buff, e),
+          ParamRef::TAG_BYTES => push_from_event_start!(self, ParamRef, reader, reader_buff, e),
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
-          FieldRef::TAG_BYTES => self
-            .elems
-            .push(CooSysElem::FieldRef(FieldRef::from_event_empty(e)?)),
-          ParamRef::TAG_BYTES => self
-            .elems
-            .push(CooSysElem::ParamRef(ParamRef::from_event_empty(e)?)),
+          FieldRef::TAG_BYTES => push_from_event_empty!(self, FieldRef, e),
+          ParamRef::TAG_BYTES => push_from_event_empty!(self, ParamRef, e),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
@@ -276,42 +242,21 @@
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    if self.elems.is_empty() {
-      let mut elem_writer = writer.create_element(Self::TAG_BYTES);
-      elem_writer = elem_writer.with_attribute(("ID", self.id.as_str()));
-      elem_writer = self.coosys.with_attributes(elem_writer);
-      write_opt_tostring_attr!(self, elem_writer, refposition);
-      elem_writer.write_empty().map_err(VOTableError::Write)?;
-      Ok(())
-    } else {
-      let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-      // Write tag + attributes
-      tag.push_attribute(("ID", self.id.as_str()));
-      self.coosys.push_attributes(&mut tag);
-      push2write_opt_tostring_attr!(self, tag, refposition);
-      writer
-        .write_event(Event::Start(tag.to_borrowed()))
-        .map_err(VOTableError::Write)?;
-      // Write sub-elems
-      write_elem_vec_no_context!(self, elems, writer);
-      // Close tag
-      writer
-        .write_event(Event::End(tag.to_end()))
-        .map_err(VOTableError::Write)
-    }
+    write_elem_vec_no_context!(self, elems, writer);
+    Ok(())
   }
 }
 
 /// Besselian (= tropical) year, e.g. B1950
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct BesselianYear(pub f64);
 impl FromStr for BesselianYear {
@@ -319,14 +264,15 @@
 
   fn from_str(s: &str) -> Result<Self, Self::Err> {
     let decimal_year_str = if let Some(stripped) = s.strip_prefix('B') {
       stripped
     } else {
       s
     };
+    trace!("Parse Besselian year: '{}'", decimal_year_str);
     decimal_year_str.parse::<f64>().map(BesselianYear)
   }
 }
 impl Display for BesselianYear {
   fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
     f.write_fmt(format_args!("B{}", self.0))
   }
@@ -340,14 +286,15 @@
 
   fn from_str(s: &str) -> Result<Self, Self::Err> {
     let decimal_year_str = if let Some(stripped) = s.strip_prefix('J') {
       stripped
     } else {
       s
     };
+    trace!("Parse Julian year: '{}'", decimal_year_str);
     decimal_year_str.parse::<f64>().map(JulianYear)
   }
 }
 impl Display for JulianYear {
   fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
     f.write_fmt(format_args!("J{}", self.0))
   }
@@ -465,68 +412,163 @@
     System::Galactic { epoch: None }
   }
 
   pub fn new_supergalactic() -> System {
     System::SuperGalactic { epoch: None }
   }
 
+  pub fn from_system<S>(system: S) -> Result<Self, VOTableError>
+  where
+    S: AsRef<str>,
+  {
+    let system = system.as_ref();
+    match system {
+      "eq_FK4" => Ok(System::new_default_eq_fk4()),
+      "eq_FK5" => Ok(System::new_default_eq_fk5()),
+      "ICRS" => Ok(System::new_icrs()),
+      "ecl_FK4" => Ok(System::new_default_ecl_fk4()),
+      "ecl_FK5" => Ok(System::new_default_ecl_fk5()),
+      "galactic" => Ok(System::new_galactic()),
+      "supergalactic" => Ok(System::new_supergalactic()),
+      _ => {
+        Err(VOTableError::Custom(format!(
+          "System not recognized in tag '{}'. Expected: one of [eq_FK4, eq_FK5, ICRS, ecl_FK4, ecl_FK5, galactic, supergalactic]. Actual: '{}'.",
+          CooSys::TAG, system,
+        )))
+      }
+    }
+  }
+
+  pub fn from_system_and_equinox<S, E>(system: S, equinox: E) -> Result<Self, VOTableError>
+  where
+    S: AsRef<str>,
+    E: AsRef<str>,
+  {
+    let system = system.as_ref();
+    let equinox = equinox.as_ref();
+    match system {
+      "eq_FK4" => equinox
+        .parse::<BesselianYear>()
+        .map_err(|e| VOTableError::ParseYear(equinox.to_string(), e))
+        .map(|equinox| System::new_eq_fk4(equinox.0)),
+      "eq_FK5" => equinox
+        .parse::<JulianYear>()
+        .map_err(|e| VOTableError::ParseYear(equinox.to_string(), e))
+        .map(|equinox| System::new_eq_fk5(equinox.0)),
+      "ICRS" => Ok(System::new_icrs()),
+      "ecl_FK4" => equinox
+        .parse::<BesselianYear>()
+        .map_err(|e| VOTableError::ParseYear(equinox.to_string(), e))
+        .map(|equinox| System::new_ecl_fk4(equinox.0)),
+      "ecl_FK5" => equinox
+        .parse::<JulianYear>()
+        .map_err(|e| VOTableError::ParseYear(equinox.to_string(), e))
+        .map(|equinox| System::new_ecl_fk5(equinox.0)),
+      "galactic" => Ok(System::new_galactic()),
+      "supergalactic" => Ok(System::new_supergalactic()),
+      _ => Err(VOTableError::Custom(format!(
+        "System not recognized in tag '{}'. Expected: one of [eq_FK4, eq_FK5, ICRS, ecl_FK4, ecl_FK5, galactic, supergalactic]. Actual: '{}'.",
+        CooSys::TAG, system,
+      ))),
+    }
+  }
+
+  /// For FK4 systems, the epoch must be provided in Besselian years
+  /// For FK5 systems, the epoch must be provided in Julian years
+  pub fn set_equinox(mut self, equinox_in_years: f64) -> Self {
+    self.set_equinox_by_ref(equinox_in_years);
+    self
+  }
+
+  /// For FK4 systems, the epoch must be provided in Besselian years
+  /// For FK5 systems, the epoch must be provided in Julian years
+  pub fn set_equinox_by_ref(&mut self, equinox_in_years: f64) {
+    match self {
+      System::EquatorialFK4 { equinox, .. } => equinox.0 = equinox_in_years,
+      System::EcliptiqueFK4 { equinox, .. } => equinox.0 = equinox_in_years,
+      System::EquatorialFK5 { equinox, .. } => equinox.0 = equinox_in_years,
+      System::EcliptiqueFK5 { equinox, .. } => equinox.0 = equinox_in_years,
+      _ => {}
+    }
+  }
+
+  pub fn set_equinox_from_str<S: AsRef<str>>(mut self, equinox: S) -> Result<Self, VOTableError> {
+    self.set_equinox_from_str_by_ref(equinox).map(|()| self)
+  }
+
+  pub fn set_equinox_from_str_by_ref<S: AsRef<str>>(
+    &mut self,
+    equinox: S,
+  ) -> Result<(), VOTableError> {
+    let equinox_str = equinox.as_ref();
+    match self {
+      System::EquatorialFK4 { equinox, .. } => equinox_str
+        .parse::<BesselianYear>()
+        .map_err(|e| VOTableError::ParseYear(equinox_str.to_string(), e))
+        .map(|new_equinox| *equinox = new_equinox),
+      System::EcliptiqueFK4 { equinox, .. } => equinox_str
+        .parse::<BesselianYear>()
+        .map_err(|e| VOTableError::ParseYear(equinox_str.to_string(), e))
+        .map(|new_equinox| *equinox = new_equinox),
+      System::EquatorialFK5 { equinox, .. } => equinox_str
+        .parse::<JulianYear>()
+        .map_err(|e| VOTableError::ParseYear(equinox_str.to_string(), e))
+        .map(|new_equinox| *equinox = new_equinox),
+      System::EcliptiqueFK5 { equinox, .. } => equinox_str
+        .parse::<JulianYear>()
+        .map_err(|e| VOTableError::ParseYear(equinox_str.to_string(), e))
+        .map(|new_equinox| *equinox = new_equinox),
+      _ => Ok(()),
+    }
+  }
+
   /// For FK4 systems, the epoch must be provided in Besselian years
   /// For FK5 systems, the epoch must be provided in Julian years
   pub fn set_epoch(mut self, epoch_in_years: f64) -> Self {
-    match &mut self {
-      System::EquatorialFK4 { equinox: _, epoch } => {
-        let _prev = epoch.insert(BesselianYear(epoch_in_years));
-      }
-      System::EcliptiqueFK4 { equinox: _, epoch } => {
-        let _prev = epoch.insert(BesselianYear(epoch_in_years));
-      }
-      System::EquatorialFK5 { equinox: _, epoch } => {
-        let _prev = epoch.insert(JulianYear(epoch_in_years));
-      }
-      System::EcliptiqueFK5 { equinox: _, epoch } => {
-        let _prev = epoch.insert(JulianYear(epoch_in_years));
-      }
-      System::ICRS { epoch } => {
-        let _prev = epoch.insert(JulianYear(epoch_in_years));
-      }
-      System::Galactic { epoch } => {
-        let _prev = epoch.insert(JulianYear(epoch_in_years));
-      }
-      System::SuperGalactic { epoch } => {
-        let _prev = epoch.insert(JulianYear(epoch_in_years));
-      }
-    };
+    self.set_epoch_by_ref(epoch_in_years);
     self
   }
 
-  pub fn set_epoch_from_str(mut self, epoch_in_years: &str) -> Result<Self, ParseFloatError> {
-    match &mut self {
-      System::EquatorialFK4 { equinox: _, epoch } => {
-        let _prev = epoch.insert(epoch_in_years.parse()?);
-      }
-      System::EcliptiqueFK4 { equinox: _, epoch } => {
-        let _prev = epoch.insert(epoch_in_years.parse()?);
-      }
+  pub fn set_epoch_by_ref(&mut self, epoch_in_years: f64) {
+    let _ = match self {
+      System::EquatorialFK4 { equinox: _, epoch } => epoch.insert(BesselianYear(epoch_in_years)).0,
+      System::EcliptiqueFK4 { equinox: _, epoch } => epoch.insert(BesselianYear(epoch_in_years)).0,
+      System::EquatorialFK5 { equinox: _, epoch } => epoch.insert(JulianYear(epoch_in_years)).0,
+      System::EcliptiqueFK5 { equinox: _, epoch } => epoch.insert(JulianYear(epoch_in_years)).0,
+      System::ICRS { epoch } => epoch.insert(JulianYear(epoch_in_years)).0,
+      System::Galactic { epoch } => epoch.insert(JulianYear(epoch_in_years)).0,
+      System::SuperGalactic { epoch } => epoch.insert(JulianYear(epoch_in_years)).0,
+    };
+  }
+
+  pub fn set_epoch_from_str<S: AsRef<str>>(mut self, epoch: S) -> Result<Self, VOTableError> {
+    self.set_epoch_from_str_by_ref(epoch).map(|()| self)
+  }
+
+  pub fn set_epoch_from_str_by_ref<S: AsRef<str>>(&mut self, epoch: S) -> Result<(), VOTableError> {
+    let epoch_str = epoch.as_ref();
+    match self {
+      System::EquatorialFK4 { equinox: _, epoch } => epoch_str
+        .parse::<BesselianYear>()
+        .map(|y| epoch.insert(y).0),
+      System::EcliptiqueFK4 { equinox: _, epoch } => epoch_str
+        .parse::<BesselianYear>()
+        .map(|y| epoch.insert(y).0),
       System::EquatorialFK5 { equinox: _, epoch } => {
-        let _prev = epoch.insert(epoch_in_years.parse()?);
+        epoch_str.parse::<JulianYear>().map(|y| epoch.insert(y).0)
       }
       System::EcliptiqueFK5 { equinox: _, epoch } => {
-        let _prev = epoch.insert(epoch_in_years.parse()?);
-      }
-      System::ICRS { epoch } => {
-        let _prev = epoch.insert(epoch_in_years.parse()?);
-      }
-      System::Galactic { epoch } => {
-        let _prev = epoch.insert(epoch_in_years.parse()?);
-      }
-      System::SuperGalactic { epoch } => {
-        let _prev = epoch.insert(epoch_in_years.parse()?);
+        epoch_str.parse::<JulianYear>().map(|y| epoch.insert(y).0)
       }
+      System::ICRS { epoch } => epoch_str.parse::<JulianYear>().map(|y| epoch.insert(y).0),
+      System::Galactic { epoch } => epoch_str.parse::<JulianYear>().map(|y| epoch.insert(y).0),
+      System::SuperGalactic { epoch } => epoch_str.parse::<JulianYear>().map(|y| epoch.insert(y).0),
     }
-    Ok(self)
+    .map_err(|e| VOTableError::ParseYear(epoch_str.to_string(), e))
+    .map(|_| ())
   }
 
   pub fn for_each_attribute<F>(&self, f: &mut F)
   where
     F: FnMut(&str, &str),
   {
     match self {
@@ -574,58 +616,38 @@
         f("system", "supergalactic");
         if let Some(epoch) = epoch {
           f("epoch", epoch.to_string().as_str());
         }
       }
     }
   }
-
-  pub fn with_attributes<'a, W: Write>(
-    &self,
-    mut writer: ElementWriter<'a, W>,
-  ) -> ElementWriter<'a, W> {
-    // I have not (yet) found a way to avoid copies :o/
-    // * I tried 'attrs: Vec<(&str, &str)>' plus  'writer.with_attributes'
-    let mut attrs: Vec<(String, String)> = Vec::with_capacity(3);
-    let mut f = |key: &str, val: &str| attrs.push((key.to_owned(), val.to_owned()));
-    self.for_each_attribute(&mut f);
-    for (k, v) in attrs {
-      writer = writer.with_attribute((k.as_str(), v.as_str()))
-    }
-    writer
-  }
-
-  pub fn push_attributes(&self, tag: &mut BytesStart) {
-    let mut f = |key: &str, val: &str| tag.push_attribute((key, val));
-    self.for_each_attribute(&mut f);
-  }
 }
 
 #[cfg(test)]
 mod tests {
   use std::io::Cursor;
 
   use quick_xml::{events::Event, Reader, Writer};
 
   use crate::{
     coosys::{CooSys, System},
-    QuickXmlReadWrite,
+    QuickXmlReadWrite, VOTableElement,
   };
 
   #[test]
   fn test_coosys_readwrite() {
     let xml = r#"<COOSYS ID="J2000" system="eq_FK5" equinox="J2000"/>"#;
     // Test read
     let mut reader = Reader::from_reader(Cursor::new(xml.as_bytes()));
     let mut buff: Vec<u8> = Vec::with_capacity(xml.len());
     let mut coosys = loop {
       let mut event = reader.read_event(&mut buff).unwrap();
       match &mut event {
         Event::Empty(ref mut e) if e.local_name() == CooSys::TAG_BYTES => {
-          let coosys = CooSys::from_attributes(e.attributes()).unwrap();
+          let coosys = CooSys::from_event_empty(e).unwrap();
           assert_eq!(coosys.id, "J2000");
           match &coosys.coosys {
             System::EquatorialFK5 { equinox, epoch } => {
               assert_eq!(equinox.0, 2000.0);
               assert!(epoch.is_none());
             }
             _ => unreachable!(),
```

### Comparing `votable_cli-0.5.0/src/data/binary.rs` & `votable_cli-0.6.0/src/data/binary.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 //! Module dedicated to the `BINARY` tag.
 
 use std::{
   io::{BufRead, Write},
   str,
 };
 
-use log::warn;
 use quick_xml::{
-  events::{attributes::Attributes, BytesEnd, BytesStart, Event},
+  events::{BytesEnd, BytesStart, Event},
   Reader, Writer,
 };
 
 use super::{
   super::{
     error::VOTableError,
     table::TableElem,
-    utils::{discard_comment, discard_event, is_empty},
-    QuickXmlReadWrite, TableDataContent,
+    utils::{discard_comment, discard_event, is_empty, unexpected_attr_warn},
+    QuickXmlReadWrite, SpecialElem, TableDataContent, VOTableElement,
   },
   stream::Stream,
 };
 
 #[derive(Default, Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct Binary<C: TableDataContent> {
   pub stream: Stream<C>,
@@ -31,91 +30,99 @@
     Self::default()
   }
 
   pub fn from_stream(stream: Stream<C>) -> Self {
     Self { stream }
   }
 
+  pub fn set_stream(mut self, stream: Stream<C>) -> Self {
+    self.set_stream_by_ref(stream);
+    self
+  }
+  pub fn set_stream_by_ref(&mut self, stream: Stream<C>) {
+    self.stream = stream;
+  }
+
   pub(crate) fn write_to_data_beginning<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
   ) -> Result<(), VOTableError> {
     writer
       .write_event(Event::Start(BytesStart::borrowed_name(Self::TAG_BYTES)))
       .map_err(VOTableError::Write)
       .and_then(|()| {
-        //if self.stream.content.is_some() {
         self
           .stream
           .write_start(writer)
           .and_then(|()| writer.write(b"\n").map_err(VOTableError::Write))
-        /*} else {
-          self.stream.write(writer, &())
-        }*/
       })
   }
 
   pub(crate) fn write_from_data_end<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
   ) -> Result<(), VOTableError> {
     //if self.stream.content.is_some() {
-    self
-      .stream
-      .write_end(writer)
-      /*} else {
-        self.stream.write(writer, &())
-      }*/
-      .and_then(|()| {
-        writer
-          .write_event(Event::End(BytesEnd::borrowed(Self::TAG_BYTES)))
-          .map_err(VOTableError::Write)
-      })
+    self.stream.write_end(writer).and_then(|()| {
+      writer
+        .write_event(Event::End(BytesEnd::borrowed(Self::TAG_BYTES)))
+        .map_err(VOTableError::Write)
+    })
   }
 }
 
-impl<C: TableDataContent> QuickXmlReadWrite for Binary<C> {
+impl<C: TableDataContent> VOTableElement for Binary<C> {
   const TAG: &'static str = "BINARY";
-  type Context = Vec<TableElem>;
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let data = Self::new();
-    if attrs.count() > 0 {
-      warn!(
-        "No attribute expected in {}: attribute(s) ignored.",
-        Self::TAG
-      );
+  type MarkerType = SpecialElem;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new().set_attrs(attrs)
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (k, _) in attrs {
+      unexpected_attr_warn(k.as_ref(), Self::TAG);
     }
-    Ok(data)
+    Ok(())
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, context)
-      .map(|()| reader)
+  fn for_each_attribute<F>(&self, _f: F)
+  where
+    F: FnMut(&str, &str),
+  {
   }
+}
+
+impl<C: TableDataContent> QuickXmlReadWrite<SpecialElem> for Binary<C> {
+  type Context = Vec<TableElem>;
 
-  fn read_sub_elements_by_ref<R: BufRead>(
+  fn read_content_by_ref<R: BufRead>(
     &mut self,
     reader: &mut Reader<R>,
     reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
+    context: &Vec<TableElem>,
   ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.name() {
           Stream::<C>::TAG_BYTES => {
             // We could detect if current stream.content.is_some() to prevent from multi-stream...
-            let mut stream = Stream::<C>::from_attributes(e.attributes())?;
+            let mut stream = Stream::<C>::from_event_start(e)?;
             let mut content = C::new();
             content.read_binary_content(reader, reader_buff, context)?;
             stream.content = Some(content);
             self.stream = stream;
             // the next call is a failure (because we consume </STREAM> in read_binary_content)
             let tmp_reader = reader.check_end_names(false);
             loop {
@@ -155,30 +162,14 @@
   }
 
   fn write<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    /*writer
-      .write_event(Event::Start(BytesStart::borrowed_name(Self::TAG_BYTES)))
-      .map_err(VOTableError::Write)?;
-    if self.stream.content.is_some() {
-      self.stream.write_start(writer)?;
-      writer.write(b"\n").map_err(VOTableError::Write)?;
-      let content = self.stream.content.as_mut().unwrap();
-      content.write_in_binary(writer, context)?;
-      // self.content.write_in_datatable(&mut writer)?;
-      self.stream.write_end(writer)?;
-    } else {
-      self.stream.write(writer, &())?;
-    }
-    writer
-      .write_event(Event::End(BytesEnd::borrowed(Self::TAG_BYTES)))
-      .map_err(VOTableError::Write)*/
     self
       .write_to_data_beginning(writer)
       .and_then(|()| {
         self
           .stream
           .content
           .as_mut()
```

### Comparing `votable_cli-0.5.0/src/data/fits.rs` & `votable_cli-0.6.0/src/data/binary2.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,137 +1,181 @@
-//! Module dedicated to the `FITS` tag.
+//! Module dedicated to the `BINARY2` tag.
 
 use std::{
   io::{BufRead, Write},
   str,
 };
 
-use paste::paste;
 use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
+  events::{BytesEnd, BytesStart, Event},
   Reader, Writer,
 };
 
-use crate::impls::mem::VoidTableDataContent;
-
 use super::{
   super::{
     error::VOTableError,
-    utils::{discard_comment, discard_event},
-    QuickXmlReadWrite, TableDataContent, VOTableVisitor,
+    table::TableElem,
+    utils::{discard_comment, discard_event, is_empty, unexpected_attr_warn},
+    QuickXmlReadWrite, SpecialElem, TableDataContent, VOTableElement,
   },
   stream::Stream,
 };
 
 #[derive(Default, Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
-pub struct Fits {
-  // attribute
-  #[serde(skip_serializing_if = "Option::is_none")]
-  pub extnum: Option<u32>,
-  // I assume (so far) that for FITS there is no STREAM content (but a link pointing to the FITS file)
-  pub stream: Stream<VoidTableDataContent>,
+pub struct Binary2<C: TableDataContent> {
+  pub stream: Stream<C>,
 }
 
-impl Fits {
+impl<C: TableDataContent> Binary2<C> {
   pub fn new() -> Self {
     Self::default()
   }
 
-  impl_builder_opt_attr!(extnum, u32);
+  pub fn from_stream(stream: Stream<C>) -> Self {
+    Self { stream }
+  }
+
+  pub fn set_stream(mut self, stream: Stream<C>) -> Self {
+    self.set_stream_by_ref(stream);
+    self
+  }
+  pub fn set_stream_by_ref(&mut self, stream: Stream<C>) {
+    self.stream = stream;
+  }
+
+  pub(crate) fn write_to_data_beginning<W: Write>(
+    &mut self,
+    writer: &mut Writer<W>,
+  ) -> Result<(), VOTableError> {
+    writer
+      .write_event(Event::Start(BytesStart::borrowed_name(Self::TAG_BYTES)))
+      .map_err(VOTableError::Write)
+      .and_then(|()| {
+        self
+          .stream
+          .write_start(writer)
+          .and_then(|()| writer.write(b"\n").map_err(VOTableError::Write))
+      })
+  }
+
+  pub(crate) fn write_from_data_end<W: Write>(
+    &mut self,
+    writer: &mut Writer<W>,
+  ) -> Result<(), VOTableError> {
+    //if self.stream.content.is_some() {
+    self.stream.write_end(writer).and_then(|()| {
+      writer
+        .write_event(Event::End(BytesEnd::borrowed(Self::TAG_BYTES)))
+        .map_err(VOTableError::Write)
+    })
+  }
+}
+
+impl<C: TableDataContent> VOTableElement for Binary2<C> {
+  const TAG: &'static str = "BINARY2";
 
-  pub fn visit<C, V>(&mut self, visitor: &mut V) -> Result<(), V::E>
+  type MarkerType = SpecialElem;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
   where
-    C: TableDataContent,
-    V: VOTableVisitor<C>,
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
   {
-    visitor.visit_fits_start(self)?;
-    visitor.visit_fits_stream(&mut self.stream)?;
-    visitor.visit_fits_ended(self)
+    Self::new().set_attrs(attrs)
   }
-}
 
-impl QuickXmlReadWrite for Fits {
-  const TAG: &'static str = "FITS";
-  type Context = ();
-
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut fits = Self::default();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let value = str::from_utf8(attr.value.as_ref()).map_err(VOTableError::Utf8)?;
-      fits = match attr.key {
-        b"extnum" => fits.set_extnum(value.parse().map_err(VOTableError::ParseInt)?),
-        _ => {
-          return Err(VOTableError::UnexpectedAttr(attr.key.to_vec(), Self::TAG));
-        }
-      }
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (k, _) in attrs {
+      unexpected_attr_warn(k.as_ref(), Self::TAG);
     }
-    Ok(fits)
+    Ok(())
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, context)
-      .map(|()| reader)
+  fn for_each_attribute<F>(&self, _f: F)
+  where
+    F: FnMut(&str, &str),
+  {
   }
+}
+
+impl<C: TableDataContent> QuickXmlReadWrite<SpecialElem> for Binary2<C> {
+  type Context = Vec<TableElem>;
 
-  fn read_sub_elements_by_ref<R: BufRead>(
+  fn read_content_by_ref<R: BufRead>(
     &mut self,
-    mut reader: &mut Reader<R>,
-    mut reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
+    reader: &mut Reader<R>,
+    reader_buff: &mut Vec<u8>,
+    context: &Vec<TableElem>,
   ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.name() {
-          Stream::<VoidTableDataContent>::TAG_BYTES => {
-            self.stream = from_event_start_by_ref!(Stream, reader, reader_buff, e)
+          Stream::<C>::TAG_BYTES => {
+            // We could detect if current stream.content.is_some() to prevent from multi-stream...
+            let mut stream = Stream::<C>::from_event_start(e)?;
+            let mut content = C::new();
+            content.read_binary2_content(reader, reader_buff, context)?;
+            stream.content = Some(content);
+            self.stream = stream;
+            // the next call is a failure (because we consume </STREAM> in read_binary_content)
+            let tmp_reader = reader.check_end_names(false);
+            loop {
+              let mut event = tmp_reader
+                .read_event(reader_buff)
+                .map_err(VOTableError::Read)?;
+              match &mut event {
+                Event::Text(e) if is_empty(e) => {}
+                Event::End(e) if e.name() == Self::TAG_BYTES => return Ok(()),
+                Event::Comment(e) => discard_comment(e, tmp_reader, Self::TAG),
+                _ => discard_event(event, Self::TAG),
+              }
+            }
           }
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.name() {
-          Stream::<VoidTableDataContent>::TAG_BYTES => self.stream = Stream::from_event_empty(e)?,
+          Stream::<C>::TAG_BYTES => self.stream = Stream::<C>::from_event_empty(e)?,
           _ => {
-            return Err(VOTableError::UnexpectedEmptyTag(
+            return Err(VOTableError::UnexpectedStartTag(
               e.name().to_vec(),
               Self::TAG,
             ))
           }
         },
-        Event::End(e) if e.name() == Self::TAG_BYTES => return Ok(()),
+        Event::Text(e) if is_empty(e) => {}
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
   fn write<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
-    _context: &Self::Context,
+    context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    push2write_opt_tostring_attr!(self, tag, extnum);
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elements
-    self.stream.write(writer, &())?;
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    self
+      .write_to_data_beginning(writer)
+      .and_then(|()| {
+        self
+          .stream
+          .content
+          .as_mut()
+          .unwrap()
+          .write_in_binary2(writer, context)
+      })
+      .and_then(|()| self.write_from_data_end(writer))
   }
 }
```

### Comparing `votable_cli-0.5.0/src/data/mod.rs` & `votable_cli-0.6.0/src/data/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 //! Module dedicated to the `DATA` tag.
 use std::{
   io::{BufRead, Write},
   str,
 };
 
-use log::warn;
 use paste::paste;
 use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
+  events::{BytesStart, Event},
   Reader, Writer,
 };
 
 use super::{
   data::stream::{EncodingType, Stream},
   error::VOTableError,
   impls::mem::VoidTableDataContent,
   info::Info,
   table::TableElem,
-  utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite, TableDataContent, VOTableVisitor,
+  utils::{discard_comment, discard_event, is_empty, unexpected_attr_warn},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, TableDataContent, VOTableElement, VOTableVisitor,
 };
 
 // Sub modules
 pub mod binary;
 pub mod binary2;
 pub mod fits;
 pub mod stream;
@@ -64,24 +63,18 @@
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     reader: &mut Reader<R>,
     reader_buff: &mut Vec<u8>,
     context: &Vec<TableElem>,
   ) -> Result<(), VOTableError> {
     match self {
-      DataElem::TableData(ref mut e) => {
-        e.read_sub_elements_and_clean_by_ref(reader, reader_buff, context)
-      }
-      DataElem::Binary(ref mut e) => {
-        e.read_sub_elements_and_clean_by_ref(reader, reader_buff, context)
-      }
-      DataElem::Binary2(ref mut e) => {
-        e.read_sub_elements_and_clean_by_ref(reader, reader_buff, context)
-      }
-      DataElem::Fits(ref mut e) => e.read_sub_elements_and_clean_by_ref(reader, reader_buff, &()),
+      DataElem::TableData(ref mut e) => e.read_content_by_ref(reader, reader_buff, context),
+      DataElem::Binary(ref mut e) => e.read_content_by_ref(reader, reader_buff, context),
+      DataElem::Binary2(ref mut e) => e.read_content_by_ref(reader, reader_buff, context),
+      DataElem::Fits(ref mut e) => e.read_content_by_ref(reader, reader_buff, &()),
     }
   }
 
   fn write<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Vec<TableElem>,
@@ -213,17 +206,15 @@
           .set_content(t.content),
       )),
       DataElem::Binary(b) => DataElem::Binary2(Binary2::from_stream(b.stream)),
       _ => self.data,
     };
     Ok(self)
   }
-}
 
-impl<C: TableDataContent> Data<C> {
   pub(crate) fn read_till_table_bin_or_bin2_or_fits_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
   ) -> Result<Option<TableOrBinOrBin2>, VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
@@ -238,28 +229,24 @@
             return Ok(Some(TableOrBinOrBin2::Fits(from_event_start_by_ref!(
               Fits,
               reader,
               reader_buff,
               e
             ))))
           }
-          Info::TAG_BYTES => {
-            self
-              .infos
-              .push(from_event_start_by_ref!(Info, reader, reader_buff, e))
-          }
+          Info::TAG_BYTES => push_from_event_start!(self, Info, reader, reader_buff, e),
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
-          Info::TAG_BYTES => self.infos.push(Info::from_event_empty(e)?),
+          Info::TAG_BYTES => push_from_event_empty!(self, Info, e),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
@@ -301,51 +288,66 @@
     // Close tag
     writer
       .write_event(Event::End(tag.to_end()))
       .map_err(VOTableError::Write)
   }
 }
 
-impl<C: TableDataContent> QuickXmlReadWrite for Data<C> {
+impl<C: TableDataContent> VOTableElement for Data<C> {
   const TAG: &'static str = "DATA";
-  type Context = Vec<TableElem>;
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let data = Self::new_empty();
-    if attrs.count() > 0 {
-      warn!(
-        "No attribute expected in {}: attribute(s) ignored.",
-        Self::TAG
-      );
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new_empty().set_attrs(attrs)
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (k, _) in attrs {
+      unexpected_attr_warn(k.as_ref(), Self::TAG);
     }
-    Ok(data)
+    Ok(())
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, context)
-      .map(|_| reader)
+  fn for_each_attribute<F>(&self, _f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+  }
+}
+
+impl<C: TableDataContent> HasSubElements for Data<C> {
+  type Context = Vec<TableElem>;
+
+  fn has_no_sub_elements(&self) -> bool {
+    false
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
           TableData::<C>::TAG_BYTES => {
+            // Nothing here because the default is a TableData
             self
               .data
               .read_sub_elements_by_ref(reader, reader_buff, context)?
           }
           Binary::<C>::TAG_BYTES => {
             self.data = DataElem::Binary(Binary::new());
             self
@@ -357,28 +359,24 @@
             self
               .data
               .read_sub_elements_by_ref(reader, reader_buff, context)?
           }
           Fits::TAG_BYTES => {
             self.data = DataElem::Fits(from_event_start_by_ref!(Fits, reader, reader_buff, e))
           }
-          Info::TAG_BYTES => {
-            self
-              .infos
-              .push(from_event_start_by_ref!(Info, reader, reader_buff, e))
-          }
+          Info::TAG_BYTES => push_from_event_start!(self, Info, reader, reader_buff, e),
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
-          Info::TAG_BYTES => self.infos.push(Info::from_event_empty(e)?),
+          Info::TAG_BYTES => push_from_event_empty!(self, Info, e),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
@@ -386,25 +384,17 @@
         Event::End(e) if e.local_name() == Self::TAG_BYTES => return Ok(()),
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-element
     self.data.write(writer, context)?;
     write_elem_vec_empty_context!(self, infos, writer);
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    Ok(())
   }
 }
```

### Comparing `votable_cli-0.5.0/src/data/stream.rs` & `votable_cli-0.6.0/src/data/stream.rs`

 * *Files 11% similar despite different names*

```diff
@@ -4,23 +4,23 @@
   fmt,
   io::{BufRead, Write},
   str::{self, FromStr},
 };
 
 use paste::paste;
 use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
+  events::{BytesStart, Event},
   Reader, Writer,
 };
 
 use crate::{
   error::VOTableError,
   impls::mem::VoidTableDataContent,
-  utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite, TableDataContent,
+  utils::{discard_comment, discard_event, is_empty, unexpected_attr_warn},
+  QuickXmlReadWrite, SpecialElem, TableDataContent, VOTableElement,
 };
 
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 pub enum Type {
   Locator,
   Other,
 }
@@ -131,19 +131,15 @@
   pub encoding: Option<EncodingType>,
   // None by default, base64 if no href
   #[serde(skip_serializing_if = "Option::is_none")]
   pub expires: Option<String>,
   // date!
   #[serde(skip_serializing_if = "Option::is_none")]
   pub rights: Option<String>,
-  // extra attributes
-  // #[serde(flatten, skip_serializing_if = "HashMap::is_empty")]
-  // pub extra: HashMap<String, Value>,
   // content, if not parsed by binary of binary2
-  //#[serde(skip_serializing_if = "Option::is_none")]
   #[serde(flatten)]
   pub content: Option<C>,
 }
 
 impl Stream<VoidTableDataContent> {
   pub(crate) fn open_stream<R: BufRead>(
     reader: &mut Reader<R>,
@@ -151,28 +147,26 @@
   ) -> Result<Stream<VoidTableDataContent>, VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.name() {
           Stream::<VoidTableDataContent>::TAG_BYTES => {
             // We could detect if current stream.content.is_some() to prevent from multi-stream...
-            let stream = Stream::<VoidTableDataContent>::from_attributes(e.attributes())?;
-            return Ok(stream);
+            return Stream::<VoidTableDataContent>::from_event_start(e);
           }
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.name() {
           Stream::<VoidTableDataContent>::TAG_BYTES => {
-            let stream = Stream::<VoidTableDataContent>::from_event_empty(e)?;
-            return Ok(stream);
+            return Stream::<VoidTableDataContent>::from_event_empty(e);
           }
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.name().to_vec(),
               Self::TAG,
             ))
           }
@@ -194,59 +188,27 @@
   // attributes
   impl_builder_opt_attr!(type_, type, Type);
   impl_builder_opt_string_attr!(href);
   impl_builder_opt_attr!(actuate, Actuate);
   impl_builder_opt_attr!(encoding, EncodingType);
   impl_builder_opt_string_attr!(expires);
   impl_builder_opt_string_attr!(rights);
-  // extra attributes
-  // impl_builder_insert_extra!();
 
   pub fn set_content(mut self, content: C) -> Self {
-    self.content = Some(content);
+    self.set_content_by_ref(content);
     self
   }
-
-  /// Calls a closure on each (key, value) attribute pairs.
-  pub fn for_each_attribute<F>(&self, mut f: F)
-  where
-    F: FnMut(&str, &str),
-  {
-    if let Some(type_) = &self.type_ {
-      f("type", type_.to_string().as_str());
-    }
-    if let Some(href) = &self.href {
-      f("href", href.as_str());
-    }
-    if let Some(actuate) = &self.actuate {
-      f("actuate", actuate.to_string().as_str());
-    }
-    if let Some(encoding) = &self.encoding {
-      f("encoding", encoding.to_string().as_str());
-    }
-    if let Some(expires) = &self.expires {
-      f("expires", expires.as_str());
-    }
-    if let Some(rights) = &self.rights {
-      f("rights", rights.as_str());
-    }
-    /*for (k, v) in &self.extra {
-      f(k.as_str(), v.to_string().as_str());
-    }*/
+  pub fn set_content_by_ref(&mut self, content: C) {
+    self.content = Some(content);
   }
 
   pub fn write_start<W: Write>(&mut self, writer: &mut Writer<W>) -> Result<(), VOTableError> {
     let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
     // Write tag + attributes
-    push2write_opt_tostring_attr!(self, tag, type_, type);
-    push2write_opt_string_attr!(self, tag, href);
-    push2write_opt_tostring_attr!(self, tag, actuate);
-    push2write_opt_tostring_attr!(self, tag, encoding);
-    push2write_opt_string_attr!(self, tag, expires);
-    push2write_opt_string_attr!(self, tag, rights);
+    self.for_each_attribute(|k, v| tag.push_attribute((k, v)));
     // push2write_extra!(self, tag);
     writer
       .write_event(Event::Start(tag.to_borrowed()))
       .map_err(VOTableError::Write)
   }
 
   pub fn write_end<W: Write>(&mut self, writer: &mut Writer<W>) -> Result<(), VOTableError> {
@@ -254,63 +216,103 @@
     let tag = BytesStart::borrowed_name(Self::TAG_BYTES);
     writer
       .write_event(Event::End(tag.to_end()))
       .map_err(VOTableError::Write)
   }
 }
 
-impl<C: TableDataContent> QuickXmlReadWrite for Stream<C> {
+impl<C: TableDataContent> VOTableElement for Stream<C> {
   const TAG: &'static str = "STREAM";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut stream = Self::default();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let value = str::from_utf8(attr.value.as_ref()).map_err(VOTableError::Utf8)?;
-      stream = match attr.key {
-        b"type" => stream.set_type(value.parse::<Type>().map_err(VOTableError::Variant)?),
-        b"href" => stream.set_href(value),
-        b"actuate" => stream.set_actuate(value.parse::<Actuate>().map_err(VOTableError::Variant)?),
-        b"encoding" => stream.set_encoding(
-          value
+  type MarkerType = SpecialElem;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new().set_attrs(attrs)
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "type" => self.set_type_by_ref(
+          val
+            .as_ref()
+            .parse::<Type>()
+            .map_err(VOTableError::Variant)?,
+        ),
+        "href" => self.set_href_by_ref(val),
+        "actuate" => self.set_actuate_by_ref(
+          val
+            .as_ref()
+            .parse::<Actuate>()
+            .map_err(VOTableError::Variant)?,
+        ),
+        "encoding" => self.set_encoding_by_ref(
+          val
+            .as_ref()
             .parse::<EncodingType>()
             .map_err(VOTableError::Variant)?,
         ),
-        b"expires" => stream.set_expires(value),
-        b"rights" => stream.set_rights(value),
-        _ => stream, /*stream.insert_extra(
-                       str::from_utf8(attr.key).map_err(VOTableError::Utf8)?,
-                       Value::String(value.into()),
-                     )*/
+        "expires" => self.set_expires_by_ref(val),
+        "rights" => self.set_rights_by_ref(val),
+        _ => unexpected_attr_warn(key, Self::TAG),
       }
     }
-    Ok(stream)
+    Ok(())
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut _reader: Reader<R>,
-    mut _reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    // read_content!(Self, self, reader, reader_buff)
-    Err(VOTableError::Custom(String::from(
-      "Reading STREAM with a content must be taken in charge by the parent \
-    element (since the encoding depends on the parent: BINARY of BINARY2",
-    )))
+  /// Calls a closure on each (key, value) attribute pairs.
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    if let Some(type_) = &self.type_ {
+      f("type", type_.to_string().as_str());
+    }
+    if let Some(href) = &self.href {
+      f("href", href.as_str());
+    }
+    if let Some(actuate) = &self.actuate {
+      f("actuate", actuate.to_string().as_str());
+    }
+    if let Some(encoding) = &self.encoding {
+      f("encoding", encoding.to_string().as_str());
+    }
+    if let Some(expires) = &self.expires {
+      f("expires", expires.as_str());
+    }
+    if let Some(rights) = &self.rights {
+      f("rights", rights.as_str());
+    }
   }
+}
+
+impl<C: TableDataContent> QuickXmlReadWrite<SpecialElem> for Stream<C> {
+  type Context = ();
 
-  fn read_sub_elements_by_ref<R: BufRead>(
+  fn read_content_by_ref<R: BufRead>(
     &mut self,
-    mut _reader: &mut Reader<R>,
-    mut _reader_buff: &mut Vec<u8>,
+    _reader: &mut Reader<R>,
+    _reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    todo!()
+    Err(VOTableError::Custom(String::from(
+      "Reading STREAM with a content must be taken in charge by the parent \
+    element (since the encoding depends on the parent: BINARY of BINARY2)",
+    )))
   }
 
   fn write<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
```

### Comparing `votable_cli-0.5.0/src/data/tabledata.rs` & `votable_cli-0.6.0/src/data/tabledata.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 //! Module dedicated to the `TABLEDATA` tag.
 
 use std::{
   io::{BufRead, Write},
   str,
 };
 
-use log::warn;
 use quick_xml::{
-  events::{attributes::Attributes, BytesEnd, BytesStart, Event},
+  events::{BytesEnd, BytesStart, Event},
   Reader, Writer,
 };
 
-use crate::{error::VOTableError, table::TableElem, utils::*, QuickXmlReadWrite, TableDataContent};
+use crate::{
+  error::VOTableError, table::TableElem, utils::*, QuickXmlReadWrite, SpecialElem,
+  TableDataContent, VOTableElement,
+};
 
 #[derive(Default, Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct TableData<C: TableDataContent> {
   #[serde(flatten)]
   pub content: C,
 }
 
@@ -249,41 +251,51 @@
   ) -> Result<(), VOTableError> {
     writer
       .write_event(Event::End(BytesEnd::borrowed(Self::TAG_BYTES)))
       .map_err(VOTableError::Write)
   }
 }
 
-impl<C: TableDataContent> QuickXmlReadWrite for TableData<C> {
+impl<C: TableDataContent> VOTableElement for TableData<C> {
   const TAG: &'static str = "TABLEDATA";
-  type Context = Vec<TableElem>;
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let table_data = Self::default();
-    if attrs.count() > 0 {
-      warn!(
-        "No attribute expected in {}: attribute(s) ignored.",
-        Self::TAG
-      );
+  type MarkerType = SpecialElem;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::default().set_attrs(attrs)
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (k, _) in attrs {
+      unexpected_attr_warn(k.as_ref(), Self::TAG);
     }
-    Ok(table_data)
+    Ok(())
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, context)
-      .map(|()| reader)
+  fn for_each_attribute<F>(&self, _f: F)
+  where
+    F: FnMut(&str, &str),
+  {
   }
+}
+
+impl<C: TableDataContent> QuickXmlReadWrite<SpecialElem> for TableData<C> {
+  type Context = Vec<TableElem>;
 
-  fn read_sub_elements_by_ref<R: BufRead>(
+  fn read_content_by_ref<R: BufRead>(
     &mut self,
     reader: &mut Reader<R>,
     reader_buff: &mut Vec<u8>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
     self
       .content
```

### Comparing `votable_cli-0.5.0/src/datatype.rs` & `votable_cli-0.6.0/src/datatype.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/src/desc.rs` & `votable_cli-0.6.0/src/desc.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,103 @@
 //! Struct dedicated to the `DESCRIPTION` tag.
 
-use std::{
-  fmt::{self, Display, Formatter},
-  io::{BufRead, Write},
-};
-
-use log::warn;
-use quick_xml::{
-  events::{attributes::Attributes, BytesText, Event},
-  Reader, Writer,
-};
+use std::fmt::{self, Display, Formatter};
 
 use super::{
-  error::VOTableError,
-  utils::{discard_comment, discard_event},
-  QuickXmlReadWrite,
+  error::VOTableError, utils::unexpected_attr_warn, HasContent, HasContentElem, VOTableElement,
 };
 
+/// Struct corresponding to the `DESCRIPTION` XML tag.
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
-pub struct Description(pub String);
+pub struct Description(String);
+
+impl Description {
+  pub fn new<I: Into<String>>(content: I) -> Self {
+    Self::from(content.into())
+  }
+}
+
+impl HasContent for Description {
+  fn get_content(&self) -> Option<&str> {
+    Some(self.0.as_str())
+  }
+  fn set_content<S: Into<String>>(mut self, content: S) -> Self {
+    self.set_content_by_ref(content);
+    self
+  }
+  fn set_content_by_ref<S: Into<String>>(&mut self, content: S) {
+    self.0 = content.into()
+  }
+}
+
+impl Description {
+  pub fn get_content_unwrapped(&self) -> &str {
+    self.0.as_str()
+  }
+}
 
 impl From<&str> for Description {
-  fn from(s: &str) -> Self {
-    s.to_string().into()
+  fn from(content: &str) -> Self {
+    content.to_string().into()
   }
 }
 
 impl From<String> for Description {
-  fn from(s: String) -> Self {
-    Description(s)
+  fn from(content: String) -> Self {
+    Self(content)
   }
 }
 
 impl Display for Description {
   fn fmt(&self, f: &mut Formatter<'_>) -> fmt::Result {
-    f.write_str(self.0.as_str())
+    f.write_str(self.get_content().unwrap_or(""))
   }
 }
 
-impl QuickXmlReadWrite for Description {
+impl VOTableElement for Description {
   const TAG: &'static str = "DESCRIPTION";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    if attrs.count() > 0 {
-      warn!("Unexpected attributes in DESCRIPTION (not serialized!)");
+  type MarkerType = HasContentElem;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new("").set_attrs(attrs)
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (k, _) in attrs {
+      unexpected_attr_warn(k.as_ref(), Self::TAG);
     }
-    Ok(Description(Default::default()))
+    Ok(())
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    // I dot not like the fact that we first create an empty String that we replace here... :o/
-    read_content!(Self, self, reader, reader_buff, 0)
-  }
-
-  fn read_sub_elements_by_ref<R: BufRead>(
-    &mut self,
-    reader: &mut Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    read_content_by_ref!(Self, self, reader, reader_buff, 0)
-  }
-
-  fn write<W: Write>(
-    &mut self,
-    writer: &mut Writer<W>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    let elem_writer = writer.create_element(Self::TAG_BYTES);
-    elem_writer
-      .write_text_content(BytesText::from_plain_str(self.0.as_str()))
-      .map_err(VOTableError::Write)?;
-    Ok(())
+  fn for_each_attribute<F>(&self, _f: F)
+  where
+    F: FnMut(&str, &str),
+  {
   }
 }
 
 #[cfg(test)]
 mod tests {
   use std::io::Cursor;
 
-  use crate::{desc::Description, QuickXmlReadWrite};
   use quick_xml::{events::Event, Reader, Writer};
 
+  use crate::{desc::Description, HasContent, QuickXmlReadWrite, VOTableElement};
+
   #[test]
   fn test_description_readwrite() {
     let xml = r#"<DESCRIPTION>
    VizieR Astronomical Server vizier.u-strasbg.fr
     Date: 2022-04-19T13:38:24 [V1.99+ (14-Oct-2013)]
    Explanations and Statistics of UCDs:			See LINK below
    In case of problem, please report to:	cds-question@unistra.fr
@@ -100,27 +106,28 @@
     // Test read
     let mut reader = Reader::from_reader(Cursor::new(xml.as_bytes()));
     let mut buff: Vec<u8> = Vec::with_capacity(xml.len());
     let mut description = loop {
       let mut event = reader.read_event(&mut buff).unwrap();
       match &mut event {
         Event::Start(ref mut e) if e.local_name() == Description::TAG_BYTES => {
-          let mut desc = Description::from_attributes(e.attributes()).unwrap();
-          desc
-            .read_sub_elements_and_clean(reader, &mut buff, &())
+          let desc = Description::from_event_start(&e)
+            .and_then(|desc| desc.read_content(&mut reader, &mut buff, &()))
             .unwrap();
           assert_eq!(
-            desc.0,
-            r#"
+            desc.get_content(),
+            Some(
+              r#"
    VizieR Astronomical Server vizier.u-strasbg.fr
     Date: 2022-04-19T13:38:24 [V1.99+ (14-Oct-2013)]
    Explanations and Statistics of UCDs:			See LINK below
    In case of problem, please report to:	cds-question@unistra.fr
    In this version, NULL integer columns are written as an empty string
    <TD></TD>, explicitely possible from VOTable-1.3"#
+            )
           );
           break desc;
         }
         Event::Text(ref mut e) if e.escaped().is_empty() => (), // First even read
         _ => unreachable!(),
       }
     };
```

### Comparing `votable_cli-0.5.0/src/error.rs` & `votable_cli-0.6.0/src/error.rs`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     }
     ParseInt(err: ParseIntError) {
       display("Error parsing an integer: {}", err)
     }
     ParseFloat(err: ParseFloatError) {
       display("Error parsing a float: {}", err)
     }
-    ParseYear(err: ParseFloatError) {
-      display("Error parsing a Besselian or Julian year: {}", err)
+    ParseYear(year: String, err: ParseFloatError) {
+      display("Error parsing a Besselian or Julian year '{}': {}", year, err)
     }
     ParseDatatype(err: String) {
       display("Error parsing Datatype: {}", err)
     }
     Read(err: quick_xml::Error) {
       display("Error while reading: {}", err)
     }
```

### Comparing `votable_cli-0.5.0/src/field.rs` & `votable_cli-0.6.0/src/field.rs`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,26 @@
   io::{BufRead, Write},
   num::ParseIntError,
   str::{self, FromStr},
 };
 
 use log::warn;
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
-  Reader, Writer,
-};
+use quick_xml::{events::Event, Reader, Writer};
 use serde::{de, Deserialize, Deserializer, Serialize, Serializer};
 use serde_json::Value;
 
 use super::{
   datatype::Datatype,
   desc::Description,
   error::VOTableError,
   link::Link,
   utils::{discard_comment, discard_event, is_empty},
   values::Values,
-  QuickXmlReadWrite, TableDataContent, VOTableVisitor,
+  HasSubElements, HasSubElems, QuickXmlReadWrite, TableDataContent, VOTableElement, VOTableVisitor,
 };
 
 #[derive(Clone, Debug, PartialEq, Eq)]
 pub enum ArraySize {
   // 8
   Fixed1D { size: u32 },
   // 8x5x...
@@ -246,14 +243,16 @@
     D: Deserializer<'de>,
   {
     let s = String::deserialize(deserializer)?;
     FromStr::from_str(&s).map_err(de::Error::custom)
   }
 }
 
+/// Struct corresponding to the `FIELD` XML tag.
+///
 /// From the VOTable [official document](https://www.ivoa.net/documents/VOTable/20191021/REC-VOTable-1.4-20191021.html#sec:values),
 /// the 'null' attribute in VALUES is reserved to integer types:
 /// "This mechanism is only intended for use with integer types; it should not be used for floating point types, which can use NaN instead."
 /// "This mechanism for representing null values is required for integer columns in the BINARY serialization [but not in BINARY2]"
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct Field {
   // attributes
@@ -308,73 +307,36 @@
       extra: Default::default(),
       description: None,
       values: None,
       links: vec![],
     }
   }
 
-  /// Look for a NULL value and returns it
-  pub fn null_value(&self) -> Option<&String> {
-    self.values.as_ref().and_then(|values| values.null.as_ref())
-  }
-
   // attributes
   impl_builder_opt_string_attr!(id);
+  impl_builder_mandatory_string_attr!(name);
+  impl_builder_mandatory_attr!(datatype, Datatype);
   impl_builder_opt_string_attr!(unit);
   impl_builder_opt_attr!(precision, Precision);
   impl_builder_opt_attr!(width, u16);
   impl_builder_opt_string_attr!(xtype);
   impl_builder_opt_string_attr!(ref_, ref);
   impl_builder_opt_string_attr!(ucd);
   impl_builder_opt_string_attr!(utype);
   impl_builder_opt_attr!(arraysize, ArraySize);
   // extra attributes
   impl_builder_insert_extra!();
   // sub-elements
-  impl_builder_opt_attr!(description, Description);
-  impl_builder_opt_attr!(values, Values);
+  impl_builder_opt_subelem!(description, Description);
+  impl_builder_opt_subelem!(values, Values);
   impl_builder_push!(Link);
 
-  /// Calls a closure on each (key, value) attribute pairs.
-  pub fn for_each_attribute<F>(&self, mut f: F)
-  where
-    F: FnMut(&str, &str),
-  {
-    if let Some(id) = &self.id {
-      f("ID", id.as_str());
-    }
-    f("name", self.name.as_str());
-    f("datatype", self.datatype.to_string().as_str());
-    if let Some(arraysize) = &self.arraysize {
-      f("arraysize", arraysize.to_string().as_str());
-    }
-    if let Some(width) = &self.width {
-      f("width", width.to_string().as_str());
-    }
-    if let Some(precision) = &self.precision {
-      f("precision", precision.to_string().as_str());
-    }
-    if let Some(unit) = &self.unit {
-      f("unit", unit.as_str());
-    }
-    if let Some(ucd) = &self.ucd {
-      f("ucd", ucd.as_str());
-    }
-    if let Some(utype) = &self.utype {
-      f("utype", utype.as_str());
-    }
-    if let Some(xtype) = &self.xtype {
-      f("xtype", xtype.as_str());
-    }
-    if let Some(ref_) = &self.ref_ {
-      f("ref", ref_.as_str());
-    }
-    for (k, v) in &self.extra {
-      f(k.as_str(), v.to_string().as_str());
-    }
+  /// Look for a NULL value and returns it
+  pub fn null_value(&self) -> Option<&String> {
+    self.values.as_ref().and_then(|values| values.null.as_ref())
   }
 
   pub fn visit<C, V>(&mut self, visitor: &mut V) -> Result<(), V::E>
   where
     C: TableDataContent,
     V: VOTableVisitor<C>,
   {
@@ -531,112 +493,159 @@
         }
       }
       Ok(())
     }
   }
 }
 
-impl QuickXmlReadWrite for Field {
+impl VOTableElement for Field {
   const TAG: &'static str = "FIELD";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    const NULL: &str = "@TBD";
-    const NULL_DT: Datatype = Datatype::Logical;
-    let mut field = Self::new(NULL, NULL_DT);
-    let mut has_datatype = false;
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      field = match attr.key {
-        b"ID" => field.set_id(value),
-        b"name" => {
-          field.name = value.to_string();
-          field
-        }
-        b"datatype" => {
-          field.datatype = value
-            .parse::<Datatype>()
-            .map_err(VOTableError::ParseDatatype)?;
-          has_datatype = true;
-          field
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    const DEFAULT_VALUE: &str = "@TBD";
+    const DEFAULT_DT: Datatype = Datatype::Logical;
+    let mut name_found = false;
+    let mut dt_found = false;
+    Self::new(DEFAULT_VALUE, DEFAULT_DT)
+      .set_attrs(attrs.map(|(k, v)| {
+        match k.as_ref() {
+          "name" => name_found = true,
+          "datatype" => dt_found = true,
+          _ => {}
+        };
+        (k, v)
+      }))
+      .and_then(|field| {
+        if name_found && dt_found {
+          Ok(field)
+        } else {
+          Err(VOTableError::Custom(format!(
+            "Attributes 'name' and 'datatype' are mandatory in tag '{}'",
+            Self::TAG
+          )))
         }
-        b"unit" => field.set_unit(value),
-        b"precision" if !value.is_empty() => {
-          field.set_precision(value.parse::<Precision>().map_err(VOTableError::ParseInt)?)
+      })
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "ID" => self.set_id_by_ref(val),
+        "name" => self.set_name_by_ref(val),
+        "datatype" => {
+          self.set_datatype_by_ref(val.as_ref().parse().map_err(VOTableError::ParseDatatype)?)
         }
-        b"width" if !value.is_empty() => {
-          field.set_width(value.parse().map_err(VOTableError::ParseInt)?)
+        "unit" => self.set_unit_by_ref(val),
+        "precision" => {
+          if val.as_ref().is_empty() {
+            warn!(
+              "Emtpy 'precision' attribute in tag {}: attribute ignored",
+              Self::TAG
+            )
+          } else {
+            self.set_precision_by_ref(val.as_ref().parse().map_err(VOTableError::ParseInt)?)
+          }
         }
-        b"xtype" => field.set_xtype(value),
-        b"ref" => field.set_ref(value),
-        b"ucd" => field.set_ucd(value),
-        b"utype" => field.set_utype(value),
-        b"arraysize" if !value.is_empty() => {
-          field.set_arraysize(value.parse::<ArraySize>().map_err(VOTableError::ParseInt)?)
+        "width" => self.set_width_by_ref(val.as_ref().parse().map_err(VOTableError::ParseInt)?),
+        "xtype" => self.set_xtype_by_ref(val),
+        "ref" => self.set_ref_by_ref(val),
+        "ucd" => self.set_ucd_by_ref(val),
+        "utype" => self.set_utype_by_ref(val),
+        "arraysize" => {
+          self.set_arraysize_by_ref(val.as_ref().parse().map_err(VOTableError::ParseInt)?)
         }
-        _ => field.insert_extra(
-          str::from_utf8(attr.key).map_err(VOTableError::Utf8)?,
-          Value::String(value.into()),
-        ),
+        _ => self.insert_extra_str_by_ref(key, val),
       }
     }
-    if field.name.as_str() == NULL || !has_datatype {
-      Err(VOTableError::Custom(format!(
-        "Attributes 'name' and 'datatype' are mandatory in tag '{}'",
-        Self::TAG
-      )))
-    } else {
-      Ok(field)
+    Ok(())
+  }
+
+  /// Calls a closure on each (key, value) attribute pairs.
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    if let Some(id) = &self.id {
+      f("ID", id.as_str());
+    }
+    f("name", self.name.as_str());
+    f("datatype", self.datatype.to_string().as_str());
+    if let Some(arraysize) = &self.arraysize {
+      f("arraysize", arraysize.to_string().as_str());
+    }
+    if let Some(width) = &self.width {
+      f("width", width.to_string().as_str());
+    }
+    if let Some(precision) = &self.precision {
+      f("precision", precision.to_string().as_str());
+    }
+    if let Some(unit) = &self.unit {
+      f("unit", unit.as_str());
     }
+    if let Some(ucd) = &self.ucd {
+      f("ucd", ucd.as_str());
+    }
+    if let Some(utype) = &self.utype {
+      f("utype", utype.as_str());
+    }
+    if let Some(xtype) = &self.xtype {
+      f("xtype", xtype.as_str());
+    }
+    if let Some(ref_) = &self.ref_ {
+      f("ref", ref_.as_str());
+    }
+    for_each_extra_attribute!(self, f);
   }
+}
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+impl HasSubElements for Field {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    self.description.is_none() && self.values.is_none() && self.links.is_empty()
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
           Description::TAG_BYTES => {
-            from_event_start_desc_by_ref!(self, Description, reader, reader_buff, e)
-          }
-          Values::TAG_BYTES => {
-            self.values = Some(from_event_start_by_ref!(Values, reader, reader_buff, e))
-          }
-          Link::TAG_BYTES => {
-            self
-              .links
-              .push(from_event_start_by_ref!(Link, reader, reader_buff, e))
+            set_from_event_start!(self, Description, reader, reader_buff, e)
           }
+          Values::TAG_BYTES => set_from_event_start!(self, Values, reader, reader_buff, e),
+          Link::TAG_BYTES => push_from_event_start!(self, Link, reader, reader_buff, e),
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
-          Values::TAG_BYTES => self.values = Some(Values::from_event_empty(e)?),
-          Link::TAG_BYTES => self.links.push(Link::from_event_empty(e)?),
+          Values::TAG_BYTES => set_from_event_empty!(self, Values, e),
+          Link::TAG_BYTES => push_from_event_empty!(self, Link, e),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
@@ -645,56 +654,37 @@
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    push2write_opt_string_attr!(self, tag, ID);
-    tag.push_attribute(("name", self.name.as_str()));
-    tag.push_attribute(("datatype", self.datatype.to_string().as_str()));
-    push2write_opt_string_attr!(self, tag, unit);
-    push2write_opt_tostring_attr!(self, tag, precision);
-    push2write_opt_tostring_attr!(self, tag, width);
-    push2write_opt_string_attr!(self, tag, xtype);
-    push2write_opt_string_attr!(self, tag, ref_, ref);
-    push2write_opt_string_attr!(self, tag, ucd);
-    push2write_opt_string_attr!(self, tag, utype);
-    push2write_opt_tostring_attr!(self, tag, arraysize);
-    push2write_extra!(self, tag);
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elements
     write_elem!(self, description, writer, context);
     write_elem!(self, values, writer, context);
     write_elem_vec!(self, links, writer, context);
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    Ok(())
   }
 }
 
 #[cfg(test)]
 mod tests {
+
+  use std::str::FromStr;
+
   use crate::{
     datatype::Datatype,
     field::ArraySize,
     field::Field,
     tests::{test_read, test_writer},
   };
-  use std::str::FromStr;
 
   #[test]
   fn test_arraysize_from_str() {
     assert_eq!(
       ArraySize::from_str("12"),
       Ok(ArraySize::Fixed1D { size: 12 })
     );
@@ -742,15 +732,15 @@
     for elem in elems {
       assert_eq!(ArraySize::from_str(elem).unwrap().to_string(), elem);
     }
   }
 
   #[test]
   fn test_field_read_write() {
-    let xml = r#"<FIELD ID="id" name="nomo" datatype="float" unit="unit" precision="1" width="5" xtype="xt" ucd="UCD" utype="ut" arraysize="5"></FIELD>"#; // Test read
+    let xml = r#"<FIELD ID="id" name="nomo" datatype="float" arraysize="5" width="5" precision="1" unit="unit" ucd="UCD" utype="ut" xtype="xt"/>"#; // Test read
     let field = test_read::<Field>(xml);
     // Test read
     assert_eq!(field.id, Some("id".to_string()));
     assert_eq!(field.name, "nomo".to_string());
     assert_eq!(field.datatype, Datatype::Float);
     assert_eq!(field.unit, Some("unit".to_string()));
     let prec = format!("{}", field.precision.as_ref().unwrap());
@@ -761,38 +751,38 @@
     assert_eq!(field.ucd, Some("UCD".to_string()));
     // Test write
     test_writer(field, xml)
   }
 
   #[test]
   fn test_field_read_write_w_desc() {
-    let xml = r#"<FIELD name="band" datatype="char" ucd="instr.bandpass" utype="ssa:DataID.Bandpass" arraysize="*"><DESCRIPTION>Description</DESCRIPTION></FIELD>"#;
+    let xml = r#"<FIELD name="band" datatype="char" arraysize="*" ucd="instr.bandpass" utype="ssa:DataID.Bandpass"><DESCRIPTION>Description</DESCRIPTION></FIELD>"#;
     let field = test_read::<Field>(xml);
     assert_eq!(
-      field.description.as_ref().unwrap().0,
-      "Description".to_string()
+      field.description.as_ref().unwrap().get_content_unwrapped(),
+      "Description"
     );
     // Test write
     test_writer(field, xml)
   }
 
   #[test]
   fn test_field_read_write_w_link() {
-    let xml = r#"<FIELD name="band" datatype="char" ucd="instr.bandpass" utype="ssa:DataID.Bandpass" arraysize="*"><LINK href="http://127.0.0.1/"/></FIELD>"#;
+    let xml = r#"<FIELD name="band" datatype="char" arraysize="*" ucd="instr.bandpass" utype="ssa:DataID.Bandpass"><LINK href="http://127.0.0.1/"/></FIELD>"#;
     let field = test_read::<Field>(xml);
     assert_eq!(
       field.links.get(0).as_ref().unwrap().href,
       Some("http://127.0.0.1/".to_string())
     );
     // Test write
     test_writer(field, xml)
   }
 
   #[test]
   fn test_field_read_write_w_val() {
-    let xml = r#"<FIELD name="gmag" datatype="float" unit="mag" precision="3" width="6" ucd="phot.mag;em.opt.B"><VALUES null="NaN"/></FIELD>"#;
+    let xml = r#"<FIELD name="gmag" datatype="float" width="6" precision="3" unit="mag" ucd="phot.mag;em.opt.B"><VALUES null="NaN"/></FIELD>"#;
     let field = test_read::<Field>(xml);
     assert_eq!(field.values.as_ref().unwrap().null, Some("NaN".to_string()));
     // Test write
     test_writer(field, xml)
   }
 }
```

### Comparing `votable_cli-0.5.0/src/fieldref.rs` & `votable_cli-0.6.0/src/fieldref.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 //! Struct dedicated to the `FIELDref` tag.
 
-use std::{
-  collections::HashMap,
-  io::{BufRead, Write},
-  str,
-};
+use std::{collections::HashMap, str};
 
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesText, Event},
-  Reader, Writer,
-};
 use serde_json::Value;
 
 use super::{
-  error::VOTableError,
-  utils::{discard_comment, discard_event},
-  QuickXmlReadWrite, TableDataContent, VOTableVisitor,
+  error::VOTableError, HasContent, HasContentElem, TableDataContent, VOTableElement, VOTableVisitor,
 };
 
+/// Struct corresponding to the `FIELDRef` XML tag.
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct FieldRef {
   #[serde(rename = "ref")]
   pub ref_: String,
   #[serde(skip_serializing_if = "Option::is_none")]
   pub ucd: Option<String>,
   #[serde(skip_serializing_if = "Option::is_none")]
@@ -42,110 +33,88 @@
       ucd: None,
       utype: None,
       extra: Default::default(),
       content: None,
     }
   }
 
+  // attributes
+  impl_builder_mandatory_string_attr!(ref_, ref);
   impl_builder_opt_string_attr!(ucd);
   impl_builder_opt_string_attr!(utype);
-
+  // extra attributes
   impl_builder_insert_extra!();
 
-  impl_builder_opt_string_attr!(content);
-
-  /// Calls a closure on each (key, value) attribute pairs.
-  pub fn for_each_attribute<F>(&self, mut f: F)
-  where
-    F: FnMut(&str, &str),
-  {
-    f("ref", self.ref_.as_str());
-    if let Some(ucd) = &self.ucd {
-      f("ucd", ucd.as_str());
-    }
-    if let Some(utype) = &self.utype {
-      f("utype", utype.as_str());
-    }
-    for (k, v) in &self.extra {
-      f(k.as_str(), v.to_string().as_str());
-    }
-  }
-
   pub fn visit<C, V>(&mut self, visitor: &mut V) -> Result<(), V::E>
   where
     C: TableDataContent,
     V: VOTableVisitor<C>,
   {
     visitor.visit_fieldref(self)
   }
 }
 
-impl QuickXmlReadWrite for FieldRef {
+impl_has_content!(FieldRef);
+
+impl VOTableElement for FieldRef {
   const TAG: &'static str = "FIELDref";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    const NULL: &str = "@TBD";
-    let mut paramref = Self::new(NULL);
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let value = str::from_utf8(attr.value.as_ref()).map_err(VOTableError::Utf8)?;
-      paramref = match attr.key {
-        b"ref" => {
-          paramref.ref_ = value.to_string();
-          paramref
-        }
-        b"ucd" => paramref.set_ucd(value),
-        b"utype" => paramref.set_utype(value),
-        _ => paramref.insert_extra(
-          str::from_utf8(attr.key).map_err(VOTableError::Utf8)?,
-          Value::String(value.into()),
-        ),
-      }
-    }
-    if paramref.ref_.as_str() == NULL {
-      Err(VOTableError::Custom(format!(
-        "Attributes 'ref' is mandatory in tag '{}'",
-        Self::TAG
-      )))
-    } else {
-      Ok(paramref)
-    }
-  }
+  type MarkerType = HasContentElem;
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    read_content!(Self, self, reader, reader_buff)
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    const DEFAULT_VALUE: &str = "@TBD";
+    Self::new(DEFAULT_VALUE)
+      .set_attrs(attrs)
+      .and_then(|fieldref| {
+        if fieldref.ref_.as_str() == DEFAULT_VALUE {
+          Err(VOTableError::Custom(format!(
+            "Mandatory attribute 'ref' not found in tag '{}'",
+            Self::TAG
+          )))
+        } else {
+          Ok(fieldref)
+        }
+      })
   }
 
-  fn read_sub_elements_by_ref<R: BufRead>(
-    &mut self,
-    reader: &mut Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    read_content_by_ref!(Self, self, reader, reader_buff)
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "ref" => self.set_ref_by_ref(val),
+        "ucd" => self.set_ucd_by_ref(val),
+        "utype" => self.set_utype_by_ref(val),
+        _ => self.insert_extra_str_by_ref(key, val),
+      }
+    }
+    Ok(())
   }
 
-  fn write<W: Write>(
-    &mut self,
-    writer: &mut Writer<W>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    let mut elem_writer = writer.create_element(Self::TAG_BYTES);
-    elem_writer = elem_writer.with_attribute(("ref", self.ref_.as_str()));
-    write_opt_string_attr!(self, elem_writer, ucd);
-    write_opt_string_attr!(self, elem_writer, utype);
-    write_extra!(self, elem_writer);
-    write_content!(self, elem_writer);
-    Ok(())
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    f("ref", self.ref_.as_str());
+    if let Some(ucd) = &self.ucd {
+      f("ucd", ucd.as_str());
+    }
+    if let Some(utype) = &self.utype {
+      f("utype", utype.as_str());
+    }
+    for_each_extra_attribute!(self, f);
   }
 }
 
 #[cfg(test)]
 mod tests {
   use crate::{
     fieldref::FieldRef,
```

### Comparing `votable_cli-0.5.0/src/group.rs` & `votable_cli-0.6.0/src/group.rs`

 * *Files 17% similar despite different names*

```diff
@@ -3,27 +3,24 @@
 use std::{
   io::{BufRead, Write},
   str,
 };
 
 use log::warn;
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
-  Reader, Writer,
-};
+use quick_xml::{events::Event, Reader, Writer};
 
 use super::{
   desc::Description,
   error::VOTableError,
   fieldref::FieldRef,
   param::Param,
   paramref::ParamRef,
-  utils::{discard_comment, discard_event},
-  QuickXmlReadWrite, TableDataContent, VOTableVisitor,
+  utils::{discard_comment, discard_event, unexpected_attr_warn},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, TableDataContent, VOTableElement, VOTableVisitor,
 };
 
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "elem_type")]
 pub enum GroupElem {
   ParamRef(ParamRef),
   Param(Param),
@@ -47,14 +44,15 @@
       GroupElem::ParamRef(e) => visitor.visit_paramref(e),
       GroupElem::Param(e) => e.visit(visitor),
       GroupElem::Group(e) => e.visit(visitor),
     }
   }
 }
 
+/// Struct corresponding to the `GROUP` XML tag when it is in a `VOTABLE` or a `RESOURCE`.
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct Group {
   // attributes
   #[serde(rename = "ID", skip_serializing_if = "Option::is_none")]
   pub id: Option<String>,
   #[serde(skip_serializing_if = "Option::is_none")]
   pub name: Option<String>,
@@ -86,26 +84,77 @@
       ucd: None,
       utype: None,
       description: None,
       elems: vec![],
     }
   }
 
+  // attributes
   impl_builder_opt_string_attr!(id);
   impl_builder_opt_string_attr!(name);
   impl_builder_opt_string_attr!(ref_, ref);
   impl_builder_opt_string_attr!(ucd);
   impl_builder_opt_string_attr!(utype);
-  impl_builder_opt_attr!(description, Description);
+  // sub-elements
+  impl_builder_opt_subelem!(description, Description);
   impl_builder_push_elem!(ParamRef, GroupElem);
   impl_builder_push_elem!(Param, GroupElem);
   impl_builder_push_elem!(Group, GroupElem);
 
-  /// Calls a closure on each (key, value) attribute pairs.
-  pub fn for_each_attribute<F>(&self, mut f: F)
+  pub fn visit<C, V>(&mut self, visitor: &mut V) -> Result<(), V::E>
+  where
+    C: TableDataContent,
+    V: VOTableVisitor<C>,
+  {
+    visitor.visit_group_start(self)?;
+    if let Some(descrition) = &mut self.description {
+      visitor.visit_description(descrition)?;
+    }
+    for elem in &mut self.elems {
+      elem.visit(visitor)?;
+    }
+    visitor.visit_group_ended(self)
+  }
+}
+
+impl VOTableElement for Group {
+  const TAG: &'static str = "GROUP";
+
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new().set_attrs(attrs)
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "ID" => self.set_id_by_ref(val),
+        "name" => self.set_name_by_ref(val),
+        "ref" => self.set_ref_by_ref(val),
+        "ucd" => self.set_ucd_by_ref(val),
+        "utype" => self.set_utype_by_ref(val),
+        _ => unexpected_attr_warn(key, Self::TAG),
+      }
+    }
+    Ok(())
+  }
+
+  fn for_each_attribute<F>(&self, mut f: F)
   where
     F: FnMut(&str, &str),
   {
     if let Some(id) = &self.id {
       f("ID", id.as_str());
     }
     if let Some(name) = &self.name {
@@ -117,97 +166,47 @@
     if let Some(ucd) = &self.ucd {
       f("ucd", ucd.as_str());
     }
     if let Some(utype) = &self.utype {
       f("utype", utype.as_str());
     }
   }
-
-  pub fn visit<C, V>(&mut self, visitor: &mut V) -> Result<(), V::E>
-  where
-    C: TableDataContent,
-    V: VOTableVisitor<C>,
-  {
-    visitor.visit_group_start(self)?;
-    if let Some(descrition) = &mut self.description {
-      visitor.visit_description(descrition)?;
-    }
-    for elem in &mut self.elems {
-      elem.visit(visitor)?;
-    }
-    visitor.visit_group_ended(self)
-  }
 }
 
-impl QuickXmlReadWrite for Group {
-  const TAG: &'static str = "GROUP";
+impl HasSubElements for Group {
   type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut group = Self::new();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let value = str::from_utf8(attr.value.as_ref()).map_err(VOTableError::Utf8)?;
-      group = match attr.key {
-        b"ID" => group.set_id(value),
-        b"name" => group.set_name(value),
-        b"ref" => group.set_ref(value),
-        b"ucd" => group.set_ucd(value),
-        b"utype" => group.set_utype(value),
-        _ => {
-          return Err(VOTableError::UnexpectedAttr(attr.key.to_vec(), Self::TAG));
-        }
-      }
-    }
-    Ok(group)
-  }
-
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, context)
-      .map(|()| reader)
+  fn has_no_sub_elements(&self) -> bool {
+    self.description.is_none() && self.elems.is_empty()
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          Description::TAG_BYTES => {
-            from_event_start_desc_by_ref!(self, Description, reader, reader_buff, e);
-          }
-          ParamRef::TAG_BYTES => {
-            self.push_paramref_by_ref(from_event_start_by_ref!(ParamRef, reader, reader_buff, e))
-          }
-          Param::TAG_BYTES => {
-            self.push_param_by_ref(from_event_start_by_ref!(Param, reader, reader_buff, e))
-          }
-          Group::TAG_BYTES => {
-            self.push_group_by_ref(from_event_start_by_ref!(Group, reader, reader_buff, e))
-          }
+          Description::TAG_BYTES => set_desc_from_event_start!(self, reader, reader_buff, e),
+          ParamRef::TAG_BYTES => push_from_event_start!(self, ParamRef, reader, reader_buff, e),
+          Param::TAG_BYTES => push_from_event_start!(self, Param, reader, reader_buff, e),
+          Group::TAG_BYTES => push_from_event_start!(self, Group, reader, reader_buff, e),
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
-          ParamRef::TAG_BYTES => self.push_paramref_by_ref(ParamRef::from_event_empty(e)?),
-          Param::TAG_BYTES => self.push_param_by_ref(Param::from_event_empty(e)?),
+          ParamRef::TAG_BYTES => push_from_event_empty!(self, ParamRef, e),
+          Param::TAG_BYTES => push_from_event_empty!(self, Param, e),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
@@ -215,47 +214,22 @@
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    if self.description.is_none() && self.elems.is_empty() {
-      let mut elem_writer = writer.create_element(Self::TAG_BYTES);
-      write_opt_string_attr!(self, elem_writer, ID);
-      write_opt_string_attr!(self, elem_writer, name);
-      write_opt_string_attr!(self, elem_writer, ref_, "ref");
-      write_opt_string_attr!(self, elem_writer, ucd);
-      write_opt_string_attr!(self, elem_writer, utype);
-      elem_writer.write_empty().map_err(VOTableError::Write)?;
-      Ok(())
-    } else {
-      let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-      // Write tag + attributes
-      push2write_opt_string_attr!(self, tag, ID);
-      push2write_opt_string_attr!(self, tag, name);
-      push2write_opt_string_attr!(self, tag, ref_, ref);
-      push2write_opt_string_attr!(self, tag, ucd);
-      push2write_opt_string_attr!(self, tag, utype);
-      writer
-        .write_event(Event::Start(tag.to_borrowed()))
-        .map_err(VOTableError::Write)?;
-      // Write sub-elems
-      write_elem!(self, description, writer, context);
-      write_elem_vec_no_context!(self, elems, writer);
-      // Close tag
-      writer
-        .write_event(Event::End(tag.to_end()))
-        .map_err(VOTableError::Write)
-    }
+    write_elem!(self, description, writer, context);
+    write_elem_vec_no_context!(self, elems, writer);
+    Ok(())
   }
 }
 
 /// The only difference with the Group than can be in a VOTable or in a Resource
 /// is that the TableGroup can contain FieldRef!
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "elem_type")]
@@ -285,14 +259,15 @@
       TableGroupElem::ParamRef(e) => visitor.visit_paramref(e),
       TableGroupElem::Param(e) => e.visit(visitor),
       TableGroupElem::TableGroup(e) => e.visit(visitor),
     }
   }
 }
 
+/// Struct corresponding to the `GROUP` XML tag when it is in a `TABLE`.
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 #[serde(rename = "Group")]
 pub struct TableGroup {
   // attributes
   #[serde(skip_serializing_if = "Option::is_none")]
   pub id: Option<String>,
   #[serde(skip_serializing_if = "Option::is_none")]
@@ -325,27 +300,78 @@
       ucd: None,
       utype: None,
       description: None,
       elems: vec![],
     }
   }
 
+  // attributes
   impl_builder_opt_string_attr!(id);
   impl_builder_opt_string_attr!(name);
   impl_builder_opt_string_attr!(ref_, ref);
   impl_builder_opt_string_attr!(ucd);
   impl_builder_opt_string_attr!(utype);
-  impl_builder_opt_attr!(description, Description);
+  // sub-elements
+  impl_builder_opt_subelem!(description, Description);
   impl_builder_push_elem!(FieldRef, TableGroupElem);
   impl_builder_push_elem!(ParamRef, TableGroupElem);
   impl_builder_push_elem!(Param, TableGroupElem);
   impl_builder_push_elem!(TableGroup, TableGroupElem);
 
-  /// Calls a closure on each (key, value) attribute pairs.
-  pub fn for_each_attribute<F>(&self, mut f: F)
+  pub fn visit<C, V>(&mut self, visitor: &mut V) -> Result<(), V::E>
+  where
+    C: TableDataContent,
+    V: VOTableVisitor<C>,
+  {
+    visitor.visit_table_group_start(self)?;
+    if let Some(desc) = &mut self.description {
+      visitor.visit_description(desc)?;
+    }
+    for e in &mut self.elems {
+      e.visit(visitor)?;
+    }
+    visitor.visit_table_group_ended(self)
+  }
+}
+
+impl VOTableElement for TableGroup {
+  const TAG: &'static str = "GROUP";
+
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new().set_attrs(attrs)
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "ID" => self.set_id_by_ref(val),
+        "name" => self.set_name_by_ref(val),
+        "ref" => self.set_ref_by_ref(val),
+        "ucd" => self.set_ucd_by_ref(val),
+        "utype" => self.set_utype_by_ref(val),
+        _ => unexpected_attr_warn(key, Self::TAG),
+      }
+    }
+    Ok(())
+  }
+
+  fn for_each_attribute<F>(&self, mut f: F)
   where
     F: FnMut(&str, &str),
   {
     if let Some(id) = &self.id {
       f("ID", id.as_str());
     }
     if let Some(name) = &self.name {
@@ -357,110 +383,49 @@
     if let Some(ucd) = &self.ucd {
       f("ucd", ucd.as_str());
     }
     if let Some(utype) = &self.utype {
       f("utype", utype.as_str());
     }
   }
-
-  pub fn visit<C, V>(&mut self, visitor: &mut V) -> Result<(), V::E>
-  where
-    C: TableDataContent,
-    V: VOTableVisitor<C>,
-  {
-    visitor.visit_table_group_start(self)?;
-    if let Some(desc) = &mut self.description {
-      visitor.visit_description(desc)?;
-    }
-    for e in &mut self.elems {
-      e.visit(visitor)?;
-    }
-    visitor.visit_table_group_ended(self)
-  }
 }
 
-impl QuickXmlReadWrite for TableGroup {
-  const TAG: &'static str = "GROUP";
+impl HasSubElements for TableGroup {
   type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut group = Self::new();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let value = str::from_utf8(attr.value.as_ref()).map_err(VOTableError::Utf8)?;
-      group = match attr.key {
-        b"ID" => group.set_id(value),
-        b"name" => group.set_name(value),
-        b"ref" => group.set_ref(value),
-        b"ucd" => group.set_ucd(value),
-        b"utype" => group.set_utype(value),
-        _ => {
-          return Err(VOTableError::UnexpectedAttr(attr.key.to_vec(), Self::TAG));
-        }
-      }
-    }
-    Ok(group)
-  }
-
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, context)
-      .map(|()| reader)
+  fn has_no_sub_elements(&self) -> bool {
+    self.description.is_none() && self.elems.is_empty()
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          Description::TAG_BYTES => {
-            from_event_start_desc_by_ref!(self, Description, reader, reader_buff, e);
-          }
-          FieldRef::TAG_BYTES => {
-            self.push_fieldref_by_ref(from_event_start_by_ref!(FieldRef, reader, reader_buff, e))
-          }
-          ParamRef::TAG_BYTES => {
-            self.push_paramref_by_ref(from_event_start_by_ref!(ParamRef, reader, reader_buff, e))
-          }
-          Param::TAG_BYTES => {
-            self.push_param_by_ref(from_event_start_by_ref!(Param, reader, reader_buff, e))
-          }
-          TableGroup::TAG_BYTES => self.push_tablegroup_by_ref(from_event_start_by_ref!(
-            TableGroup,
-            reader,
-            reader_buff,
-            e
-          )),
+          Description::TAG_BYTES => set_desc_from_event_start!(self, reader, reader_buff, e),
+          FieldRef::TAG_BYTES => push_from_event_start!(self, FieldRef, reader, reader_buff, e),
+          ParamRef::TAG_BYTES => push_from_event_start!(self, ParamRef, reader, reader_buff, e),
+          Param::TAG_BYTES => push_from_event_start!(self, Param, reader, reader_buff, e),
+          TableGroup::TAG_BYTES => push_from_event_start!(self, TableGroup, reader, reader_buff, e),
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
-          FieldRef::TAG_BYTES => self
-            .elems
-            .push(TableGroupElem::FieldRef(FieldRef::from_event_empty(e)?)),
-          ParamRef::TAG_BYTES => self
-            .elems
-            .push(TableGroupElem::ParamRef(ParamRef::from_event_empty(e)?)),
-          Param::TAG_BYTES => self
-            .elems
-            .push(TableGroupElem::Param(Param::from_event_empty(e)?)),
+          FieldRef::TAG_BYTES => push_from_event_empty!(self, FieldRef, e),
+          ParamRef::TAG_BYTES => push_from_event_empty!(self, ParamRef, e),
+          Param::TAG_BYTES => push_from_event_empty!(self, Param, e),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
@@ -468,63 +433,40 @@
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    if self.description.is_none() && self.elems.is_empty() {
-      let mut elem_writer = writer.create_element(Self::TAG_BYTES);
-      write_opt_string_attr!(self, elem_writer, ID);
-      write_opt_string_attr!(self, elem_writer, name);
-      write_opt_string_attr!(self, elem_writer, ref_, "ref");
-      write_opt_string_attr!(self, elem_writer, ucd);
-      write_opt_string_attr!(self, elem_writer, utype);
-      elem_writer.write_empty().map_err(VOTableError::Write)?;
-      Ok(())
-    } else {
-      let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-      // Write tag + attributes
-      push2write_opt_string_attr!(self, tag, ID);
-      push2write_opt_string_attr!(self, tag, name);
-      push2write_opt_string_attr!(self, tag, ref_, ref);
-      push2write_opt_string_attr!(self, tag, ucd);
-      push2write_opt_string_attr!(self, tag, utype);
-      writer
-        .write_event(Event::Start(tag.to_borrowed()))
-        .map_err(VOTableError::Write)?;
-      // Write sub-elems
-      write_elem!(self, description, writer, context);
-      write_elem_vec_no_context!(self, elems, writer);
-      // Close tag
-      writer
-        .write_event(Event::End(tag.to_end()))
-        .map_err(VOTableError::Write)
-    }
+    write_elem!(self, description, writer, context);
+    write_elem_vec_no_context!(self, elems, writer);
+    Ok(())
   }
 }
 
 #[cfg(test)]
 mod tests {
-  use crate::group::Group;
-  use crate::tests::{test_read, test_writer};
+  use crate::{
+    group::Group,
+    tests::{test_read, test_writer},
+  };
 
   #[test]
   fn test_group_read_write() {
-    let xml = r#"<GROUP ID="flux" name="Flux" ucd="phot.flux;em.radio.200-400MHz"><DESCRIPTION>Flux measured at 352MHz</DESCRIPTION><PARAM name="Freq" datatype="float" value="352" ucd="em.freq" utype="MHz"></PARAM><PARAMref ref="col4"/><PARAMref ref="col5"/></GROUP>"#;
+    let xml = r#"<GROUP ID="flux" name="Flux" ucd="phot.flux;em.radio.200-400MHz"><DESCRIPTION>Flux measured at 352MHz</DESCRIPTION><PARAM name="Freq" datatype="float" value="352" ucd="em.freq" utype="MHz"/><PARAMref ref="col4"/><PARAMref ref="col5"/></GROUP>"#;
     let group = test_read::<Group>(xml);
     assert_eq!(group.id, Some("flux".to_string()));
     assert_eq!(group.name, Some("Flux".to_string()));
     assert_eq!(group.ucd, Some("phot.flux;em.radio.200-400MHz".to_string()));
     assert_eq!(
-      group.description.as_ref().unwrap().0,
+      group.description.as_ref().unwrap().get_content_unwrapped(),
       "Flux measured at 352MHz"
     );
     assert_eq!(group.elems.len(), 3);
     test_writer(group, xml);
   }
 }
```

### Comparing `votable_cli-0.5.0/src/impls/b64/read.rs` & `votable_cli-0.6.0/src/impls/b64/read.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/src/impls/b64/write.rs` & `votable_cli-0.6.0/src/impls/b64/write.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/src/impls/mem.rs` & `votable_cli-0.6.0/src/impls/mem.rs`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
       write::{B64Formatter, BinarySerializer},
     },
     visitors::FixedLengthArrayVisitor,
     Schema, VOTableValue,
   },
   table::TableElem,
   utils::{discard_comment, is_empty, unexpected_event},
-  QuickXmlReadWrite, TableDataContent,
+  TableDataContent, VOTableElement,
 };
 
 /// Do not parse/contains any data.
 /// Only made for VOTable parsers taking charge of parsing (and dealing with) the data part
 /// of the VOTable.
 #[derive(Default, Debug, Clone, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(transparent)]
```

### Comparing `votable_cli-0.5.0/src/impls/mod.rs` & `votable_cli-0.6.0/src/impls/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/src/impls/visitors.rs` & `votable_cli-0.6.0/src/impls/visitors.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/src/iter/elems.rs` & `votable_cli-0.6.0/src/iter/elems.rs`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     mem::VoidTableDataContent,
     visitors::FixedLengthArrayVisitor,
     Schema, VOTableValue,
   },
   iter::TableIter,
   table::Table,
   utils::{discard_comment, is_empty, unexpected_event},
-  Binary, Binary2, QuickXmlReadWrite, Stream, TableData,
+  Binary, Binary2, Stream, TableData, VOTableElement,
 };
 
 /// Possible iterators and a table row value.
 pub enum RowValueIterator<'a, R: BufRead> {
   TableData(DataTableRowValueIterator<'a, R>),
   BinaryTable(BinaryRowValueIterator<'a, R>),
   Binary2Table(Binary2RowValueIterator<'a, R>),
```

### Comparing `votable_cli-0.5.0/src/iter/mod.rs` & `votable_cli-0.6.0/src/iter/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   iter::elems::{
     Binary2RowValueIterator, BinaryRowValueIterator, DataTableRowValueIterator, RowValueIterator,
   },
   resource::{Resource, ResourceOrTable, ResourceSubElem},
   table::{Table, TableElem},
   utils::{discard_comment, discard_event, is_empty},
   votable::{VOTable, VOTableWrapper},
-  QuickXmlReadWrite,
+  VOTableElement,
 };
 
 pub mod elems;
 pub mod strings;
 
 static TR_END_FINDER: Lazy<Finder<'static>> = Lazy::new(|| Finder::new("</TR>"));
 static STREAM_END_FINDER: Lazy<Finder<'static>> = Lazy::new(|| Finder::new("</STREAM>"));
```

### Comparing `votable_cli-0.5.0/src/iter/strings.rs` & `votable_cli-0.6.0/src/iter/strings.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/src/lib.rs` & `votable_cli-0.6.0/src/lib.rs`

 * *Files 20% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 /// `metadata` my be complex, we would like to build it from a simpler (e.x. TOML) files.
 ///
 /// We used first the `VOTable` format to defined a `metadata` set, add other elements,
 /// plus a mechanism to allow for custom metadata.
 use std::{
   error::Error,
   io::{BufRead, Write},
+  str::from_utf8,
 };
 
 use quick_xml::{
-  events::{attributes::Attributes, BytesStart},
+  events::{attributes::Attributes, BytesStart, BytesText, Event},
   Reader, Writer,
 };
 
 #[macro_use]
 mod macros;
 mod utils;
 
@@ -50,14 +51,15 @@
 pub mod votable;
 
 #[cfg(feature = "mivot")]
 pub mod mivot;
 
 #[cfg(feature = "mivot")]
 pub use self::mivot::VodmlVisitor;
+use self::utils::{discard_comment, discard_event};
 pub use self::{
   coosys::CooSys,
   data::{
     binary::Binary, binary2::Binary2, fits::Fits, stream::Stream, tabledata::TableData, Data,
   },
   definitions::Definitions,
   desc::Description,
@@ -74,14 +76,307 @@
   table::Table,
   table::TableElem,
   timesys::TimeSys,
   values::{Max, Min, Opt, Values},
   votable::VOTable,
 };
 
+pub trait VOTableElement: Sized {
+  /// XML Tag og the VOTable element.
+  const TAG: &'static str;
+  const TAG_BYTES: &'static [u8] = Self::TAG.as_bytes();
+
+  type MarkerType: VOTableElementType;
+
+  /// Returns the XML tag of this VOTable Element.
+  fn tag(&self) -> &'static str {
+    Self::TAG
+  }
+
+  fn tag_bytes(&self) -> &'static [u8] {
+    Self::TAG_BYTES
+  }
+
+  /// Create a new object from a set of attributes.
+  ///
+  /// Usually, `from_attributes` simply call the object default constructor
+  /// and delegate the setting of attributes to `set_attributes`.
+  /// It may be more complicated when the object contains mandatory attributes.
+  /// # Warning
+  /// The returned object should not be considered in its final state.
+  /// Indeed, it may not be valid yet (e.g. if it **must** contains mandatory sub-elements,
+  /// those sub-elements have to be set afterwards).
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>;
+
+  /// Set (or re-set) the objet attributes.
+  fn set_attrs<K, V, I>(mut self, attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    self.set_attrs_by_ref(attrs).map(|_| self)
+  }
+
+  /// Set (or re-set) the objet attributes.
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>;
+
+  /// Calls the given function `f` on each `key=value` attribute pairs.
+  fn for_each_attribute<F>(&self, f: F)
+  where
+    F: FnMut(&str, &str);
+
+  fn get_attrs(&self) -> Vec<(String, String)> {
+    let mut attrs = Vec::new();
+    self.for_each_attribute(|k, v| attrs.push((k.to_string(), v.to_string())));
+    attrs
+  }
+}
+
+/// This trait is a marker trait used to provide specific `QuickXmlReadWrite` implementations
+/// for VOTable element families.
+/// We resort to it because negative traits is not yet fully implemented in Rust, e.g. we cannot write
+/// ```ignore
+/// impl<T: HasContent> !IsEmpty for T {}
+/// impl<T: IsEmpty> !HasContent for T {}
+/// ```
+/// For more details, see e.g. [this blog post](https://geo-ant.github.io/blog/2021/mutually-exclusive-traits-rust/)
+pub trait VOTableElementType {}
+/// Marker struct telling that the VOTable element has neither a content nor sub-elements
+pub struct EmptyElem;
+impl VOTableElementType for EmptyElem {}
+/// Marker struct telling that the VOTable element has a content, but no sub-elements
+pub struct HasContentElem;
+impl VOTableElementType for HasContentElem {}
+/// Marker struct telling that the VOTable element has sub-elements (but no content)
+pub struct HasSubElems;
+impl VOTableElementType for HasSubElems {}
+/// Marker struct telling that the VOTable element has specific reader/writers.
+pub struct SpecialElem;
+impl VOTableElementType for SpecialElem {}
+
+/// Marker trait telling that the tag is always empty: i.e. has no content and no sub-elements.
+pub trait IsEmpty: VOTableElement<MarkerType = EmptyElem> {}
+/// Implements 'IsEmpty' for all `VOTableElements` having the `EmptyElem` marker.
+impl<T> IsEmpty for T where T: VOTableElement<MarkerType = EmptyElem> {}
+
+impl<T: IsEmpty> QuickXmlReadWrite<EmptyElem> for T {
+  type Context = ();
+
+  fn read_content_by_ref<R: BufRead>(
+    &mut self,
+    _reader: &mut Reader<R>,
+    _reader_buff: &mut Vec<u8>,
+    _context: &Self::Context,
+  ) -> Result<(), VOTableError> {
+    Ok(())
+  }
+
+  fn write<W: Write>(
+    &mut self,
+    writer: &mut Writer<W>,
+    _context: &Self::Context,
+  ) -> Result<(), VOTableError> {
+    let mut elem_writer = writer.create_element(Self::TAG_BYTES);
+    elem_writer = elem_writer.with_attributes(
+      self
+        .get_attrs()
+        .iter()
+        .map(|(k, v)| (k.as_str(), v.as_str())),
+    );
+    elem_writer
+      .write_empty()
+      .map_err(VOTableError::Write)
+      .map(|_| ())
+  }
+}
+
+/// Tels that the element may contains text between its opening and closing tags.
+/// In the VOTable standard, tags possibly having a content do not have sub-elements
+pub trait HasContent: VOTableElement<MarkerType = HasContentElem> {
+  /// Returns the string content of the tag.
+  fn get_content(&self) -> Option<&str>;
+  /// Set the optional content of this tag, taking the ownership and returning itself.
+  fn set_content<S: Into<String>>(self, content: S) -> Self;
+  /// Set the optional content of this tag, by mutable ref.
+  fn set_content_by_ref<S: Into<String>>(&mut self, content: S);
+}
+impl<T: HasContent> QuickXmlReadWrite<HasContentElem> for T {
+  type Context = ();
+
+  fn read_content_by_ref<R: BufRead>(
+    &mut self,
+    reader: &mut Reader<R>,
+    reader_buff: &mut Vec<u8>,
+    _context: &Self::Context,
+  ) -> Result<(), VOTableError> {
+    let mut content = String::new();
+    loop {
+      let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
+      match &mut event {
+        Event::Text(e) => content.push_str(
+          e.unescape_and_decode(reader)
+            .map_err(VOTableError::Read)?
+            .as_str(),
+        ),
+        Event::CData(e) => {
+          content.push_str(from_utf8(e.clone().into_inner().as_ref()).map_err(VOTableError::Utf8)?)
+        }
+        Event::End(e) if e.local_name() == Self::TAG_BYTES => {
+          self.set_content_by_ref(content);
+          reader_buff.clear();
+          return Ok(());
+        }
+        Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
+        Event::Comment(e) => discard_comment(e, reader, Self::TAG),
+        _ => discard_event(event, Self::TAG),
+      }
+    }
+  }
+
+  fn write<W: Write>(
+    &mut self,
+    writer: &mut Writer<W>,
+    _context: &Self::Context,
+  ) -> Result<(), VOTableError> {
+    let mut elem_writer = writer.create_element(Self::TAG_BYTES);
+    elem_writer = elem_writer.with_attributes(
+      self
+        .get_attrs()
+        .iter()
+        .map(|(k, v)| (k.as_str(), v.as_str())),
+    );
+    if let Some(content) = self.get_content() {
+      elem_writer.write_text_content(BytesText::from_plain_str(content))
+    } else {
+      elem_writer.write_empty()
+    }
+    .map_err(VOTableError::Write)
+    .map(|_| ())
+  }
+}
+
+/// Marker trait telling that the tag mau contents sub-elements (but no content).
+pub trait HasSubElements: VOTableElement<MarkerType = HasSubElems> {
+  type Context;
+
+  /// Returns `false` if this object contains sub-elements.
+  fn has_no_sub_elements(&self) -> bool;
+
+  /// Same as `read_sub_elements`, cleaning the `reader_buf` before returning.
+  fn read_sub_elements_and_clean<R: BufRead>(
+    &mut self,
+    reader: Reader<R>,
+    reader_buff: &mut Vec<u8>,
+    context: &Self::Context,
+  ) -> Result<Reader<R>, VOTableError> {
+    let res = self.read_sub_elements(reader, reader_buff, context);
+    reader_buff.clear();
+    res
+  }
+
+  /// We assume that the previous event was `Start`, and that the method returns
+  /// when finding the `End` event matching the last `Start` event before entering the method.
+  fn read_sub_elements<R: BufRead>(
+    &mut self,
+    mut reader: Reader<R>,
+    reader_buff: &mut Vec<u8>,
+    context: &Self::Context,
+  ) -> Result<Reader<R>, VOTableError> {
+    self
+      .read_sub_elements_by_ref(&mut reader, reader_buff, context)
+      .map(|()| reader)
+  }
+
+  /// Same as `read_sub_elements`, cleaning the `reader_buf` before returning.
+  fn read_sub_elements_and_clean_by_ref<R: BufRead>(
+    &mut self,
+    reader: &mut Reader<R>,
+    reader_buff: &mut Vec<u8>,
+    context: &Self::Context,
+  ) -> Result<(), VOTableError> {
+    let res = self.read_sub_elements_by_ref(reader, reader_buff, context);
+    reader_buff.clear();
+    res
+  }
+
+  /// We assume that the previous event was `Start`, and that the method returns
+  /// when finding the `End` event matching the last `Start` event before entering the method.
+  fn read_sub_elements_by_ref<R: BufRead>(
+    &mut self,
+    reader: &mut Reader<R>,
+    reader_buff: &mut Vec<u8>,
+    context: &Self::Context,
+  ) -> Result<(), VOTableError>;
+
+  /// Write sub_elements
+  fn write_sub_elements_by_ref<W: Write>(
+    &mut self,
+    writer: &mut Writer<W>,
+    context: &Self::Context,
+  ) -> Result<(), VOTableError>;
+}
+
+impl<T: HasSubElements> QuickXmlReadWrite<HasSubElems> for T {
+  type Context = <Self as HasSubElements>::Context;
+
+  fn read_content_by_ref<R: BufRead>(
+    &mut self,
+    reader: &mut Reader<R>,
+    reader_buff: &mut Vec<u8>,
+    context: &Self::Context,
+  ) -> Result<(), VOTableError> {
+    self.read_sub_elements_by_ref(reader, reader_buff, context)
+  }
+
+  /// `&mut self` in case internals are modified while writing (e.g. if we iterate on rows
+  /// and discard them as we iterate).
+  /// We could add a context, e.g. to modify the parent (adding infos for example).
+  fn write<W: Write>(
+    &mut self,
+    writer: &mut Writer<W>,
+    context: &Self::Context,
+  ) -> Result<(), VOTableError> {
+    if self.has_no_sub_elements() {
+      let mut elem_writer = writer.create_element(Self::TAG_BYTES);
+      elem_writer = elem_writer.with_attributes(
+        self
+          .get_attrs()
+          .iter()
+          .map(|(k, v)| (k.as_str(), v.as_str())),
+      );
+      elem_writer
+        .write_empty()
+        .map_err(VOTableError::Write)
+        .map(|_| ())
+    } else {
+      let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
+      // Write tag + attributes
+      self.for_each_attribute(|k, v| tag.push_attribute((k, v)));
+      writer
+        .write_event(Event::Start(tag.to_borrowed()))
+        .map_err(VOTableError::Write)?;
+      // Write_sub-elems
+      self.write_sub_elements_by_ref(writer, context)?;
+      // Close tag
+      writer
+        .write_event(Event::End(tag.to_end()))
+        .map_err(VOTableError::Write)
+    }
+  }
+}
+
 pub trait TableDataContent: Default + PartialEq + serde::Serialize {
   fn new() -> Self {
     Self::default()
   }
 
   /// When deserializing from JSON, TOML or YAML, we should implement a 'DeserializeSeed'
   /// based on the table Schema. But:
@@ -142,70 +437,93 @@
   fn write_in_binary2<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &[TableElem],
   ) -> Result<(), VOTableError>;
 }
 
-trait QuickXmlReadWrite: Sized {
-  const TAG: &'static str;
-  const TAG_BYTES: &'static [u8] = Self::TAG.as_bytes();
+/// The `VOTableElementType` generic parameter is here only to be able to provide
+/// various default implementations, emulating mutually exclusive traits
+/// extended by `QuickXmlReadWrite`.
+pub trait QuickXmlReadWrite<VOTableElementType>: VOTableElement {
   type Context;
 
-  fn tag(&self) -> &str {
-    Self::TAG
-  }
-
-  fn tag_bytes(&self) -> &[u8] {
-    Self::TAG_BYTES
+  fn from_event_empty(e: &BytesStart) -> Result<Self, VOTableError> {
+    Self::from_event_start(e)
   }
 
-  fn from_event_empty(e: &BytesStart) -> Result<Self, VOTableError> {
+  fn from_event_start(e: &BytesStart) -> Result<Self, VOTableError> {
     Self::from_attributes(e.attributes())
   }
 
   /// We assume that the previous event was either `Start` or `Empty`.
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError>;
-
-  /// Same as `read_sub_elements`, cleaning the `reader_buf` before returning.
-  fn read_sub_elements_and_clean<R: BufRead>(
-    &mut self,
-    reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    let res = self.read_sub_elements(reader, reader_buff, context);
-    reader_buff.clear();
-    res
+  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
+    Self::quick_xml_attrs_to_vec(attrs).and_then(|attrs| Self::from_attrs(attrs.into_iter()))
   }
 
-  /// We assume that the previous event was `Start`, and that the method returns
-  /// when finding the `End` event matching the last `Start` event before entering the method.
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    reader: Reader<R>,
+  /*
+  // Does not work because BytesStart has a lifetime depending on reader_buff...
+  fn from_event_start<R: BufRead>(
+    e: &BytesStart,
+    mut reader: &mut Reader<R>,
     reader_buff: &mut Vec<u8>,
     context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError>;
+  ) -> Result<Self, VOTableError> {
+    Self::from_attributes(e.attributes()).and_then(|mut elem| {
+      elem
+        .read_sub_elements_and_clean_by_ref(&mut reader, reader_buff, context)
+        .map(|()| elem)
+    })
+  }*/
+
+  fn quick_xml_attrs_to_vec(attrs: Attributes) -> Result<Vec<(String, String)>, VOTableError> {
+    attrs
+      //.filter_map(|r| {
+      .map(|r| {
+        r.map_err(VOTableError::Attr).and_then(|attr| {
+          from_utf8(attr.key)
+            .map_err(VOTableError::Utf8)
+            .and_then(|key| {
+              attr
+                .unescaped_value()
+                .map_err(VOTableError::Read)
+                .and_then(|val| {
+                  from_utf8(val.as_ref())
+                    .map(|val| val.to_string())
+                    .map_err(VOTableError::Utf8)
+                })
+                .map(
+                  |val| (key.to_string(), val),
+                  /*{
+                    if val.is_empty() {
+                      None
+                    } else {
+                      Some((key.to_string(), val))
+                    }
+                  }*/
+                )
+            })
+        })
+        //.transpose()
+      })
+      .collect::<Result<Vec<(String, String)>, _>>()
+  }
 
-  /// Same as `read_sub_elements`, cleaning the `reader_buf` before returning.
-  fn read_sub_elements_and_clean_by_ref<R: BufRead>(
-    &mut self,
+  fn read_content<R: BufRead>(
+    mut self,
     reader: &mut Reader<R>,
     reader_buff: &mut Vec<u8>,
     context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    let res = self.read_sub_elements_by_ref(reader, reader_buff, context);
-    reader_buff.clear();
-    res
+  ) -> Result<Self, VOTableError> {
+    self
+      .read_content_by_ref(reader, reader_buff, context)
+      .map(|()| self)
   }
 
-  /// We assume that the previous event was `Start`, and that the method returns
-  /// when finding the `End` event matching the last `Start` event before entering the method.
-  fn read_sub_elements_by_ref<R: BufRead>(
+  fn read_content_by_ref<R: BufRead>(
     &mut self,
     reader: &mut Reader<R>,
     reader_buff: &mut Vec<u8>,
     context: &Self::Context,
   ) -> Result<(), VOTableError>;
 
   /// `&mut self` in case internals are modified while writing (e.g. if we iterate on rows
@@ -215,15 +533,15 @@
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError>;
 }
 
 // We visit all sub elements, bu we retrieve attributes from objects
-// We kinf of added a part of the context by prefixing some visit methods with the name of the
+// We kind of added a part of the context by prefixing some visit methods with the name of the
 // TAG it is called from.
 pub trait VOTableVisitor<C: TableDataContent> {
   type E: Error;
 
   #[cfg(feature = "mivot")]
   type M: VodmlVisitor<E = Self::E>;
 
@@ -285,37 +603,34 @@
   fn visit_values_min(&mut self, min: &mut Min) -> Result<(), Self::E>; // No start/end
   fn visit_values_max(&mut self, max: &mut Max) -> Result<(), Self::E>; // No start/end
   fn visit_values_opt_start(&mut self, opt: &mut Opt) -> Result<(), Self::E>;
   fn visit_values_opt_ended(&mut self, opt: &mut Opt) -> Result<(), Self::E>;
   fn visit_values_ended(&mut self, values: &mut Values) -> Result<(), Self::E>;
 }
 
-// For Javascript, see https://rustwasm.github.io/wasm-bindgen/reference/arbitrary-data-with-serde.html
-
 #[cfg(test)]
 mod tests {
-  use std::{i64, str::from_utf8};
+  use std::{i64, io::Cursor, str::from_utf8};
 
   use quick_xml::{events::Event, Reader, Writer};
   use serde_json::{Number, Value};
 
   use super::{
     coosys::{CooSys, System},
     data::Data,
     datatype::Datatype,
-    field::{Field, Precision},
-    impls::mem::InMemTableDataRows,
-    impls::VOTableValue,
+    field::{ArraySize, Field, Precision},
+    impls::{mem::InMemTableDataRows, VOTableValue},
     info::Info,
     link::Link,
-    resource::Resource,
+    resource::{Resource, ResourceSubElem},
     table::Table,
     values::Values,
     votable::{VOTable, Version},
-    QuickXmlReadWrite,
+    HasContent, QuickXmlReadWrite, VOTableElement,
   };
 
   #[test]
   fn test_create_in_mem_1() {
     let rows = vec![
       vec![
         VOTableValue::Null, //VOTableValue::Double(f64::NAN),
@@ -474,16 +789,16 @@
         println!("{}", from_utf8(content.as_slice()).unwrap());
 
         let mut votable2 = VOTable::<InMemTableDataRows>::from_reader(content.as_slice()).unwrap();
         let mut content2 = Vec::new();
         let mut write2 = Writer::new_with_indent(&mut content2, b' ', 4);
         votable2.write(&mut write2, &()).unwrap();
 
-        //eprintln!("CONTENT1:\n{}", from_utf8(content.as_slice()).unwrap());
-        //eprintln!("CONTENT2:\n{}", from_utf8(content2.as_slice()).unwrap());
+        eprintln!("CONTENT1:\n{}", from_utf8(content.as_slice()).unwrap());
+        eprintln!("CONTENT2:\n{}", from_utf8(content2.as_slice()).unwrap());
 
         assert_eq!(content, content2);
       }
       Err(error) => {
         println!("Error: {:?}", &error);
         assert!(false);
       }
@@ -616,50 +931,54 @@
     match quick_xml::se::to_string(&votable) {
       Ok(content) => println!("{}", &content),
       Err(error) => println!("{:?}", &error),
     }*/
     // AVRO ?
   }
 
-  use crate::field::ArraySize;
-  use crate::resource::ResourceSubElem;
-  use std::io::Cursor;
-
-  pub(crate) fn test_read<X: QuickXmlReadWrite<Context = ()>>(xml: &str) -> X {
+  pub(crate) fn test_read<X>(xml: &str) -> X
+  where
+    X: VOTableElement + QuickXmlReadWrite<<X as VOTableElement>::MarkerType, Context = ()>,
+  {
     let mut reader = Reader::from_reader(Cursor::new(xml.as_bytes()));
     let mut buff: Vec<u8> = Vec::with_capacity(xml.len());
     loop {
       let mut event = reader.read_event(&mut buff).unwrap();
       match &mut event {
         Event::Start(ref mut e) if e.local_name() == X::TAG_BYTES => {
-          let mut info = X::from_attributes(e.attributes()).unwrap();
-          let res = info.read_sub_elements_and_clean(reader, &mut buff, &());
-          if let Err(e) = res {
-            eprintln!("Error: {}", e.to_string());
-            assert!(false);
+          match X::from_event_start(e)
+            .and_then(|info| info.read_content(&mut reader, &mut buff, &()))
+          {
+            Err(e) => {
+              eprintln!("Error: {}", e.to_string());
+              assert!(false);
+            }
+            Ok(info) => return info,
           }
-          return info;
         }
         Event::Empty(ref mut e) if e.local_name() == X::TAG_BYTES => {
-          let info = X::from_attributes(e.attributes()).unwrap();
+          let info = X::from_event_start(e).unwrap();
           return info;
         }
         Event::Text(ref mut e) if e.escaped().is_empty() => (), // First even read
         Event::Comment(_) => (),
         Event::DocType(_) => (),
         Event::Decl(_) => (),
         _ => {
           println!("{:?}", event);
           assert!(false);
         }
       }
     }
   }
 
-  pub(crate) fn test_writer<X: QuickXmlReadWrite<Context = ()>>(mut writable: X, xml: &str) {
+  pub(crate) fn test_writer<X>(mut writable: X, xml: &str)
+  where
+    X: VOTableElement + QuickXmlReadWrite<<X as VOTableElement>::MarkerType, Context = ()>,
+  {
     // Test write
     let mut writer = Writer::new(Cursor::new(Vec::new()));
     writable.write(&mut writer, &()).unwrap();
     let output = writer.into_inner().into_inner();
     let output_str = unsafe { std::str::from_utf8_unchecked(output.as_slice()) };
     assert_eq!(output_str, xml);
   }
```

### Comparing `votable_cli-0.5.0/src/link.rs` & `votable_cli-0.6.0/src/link.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 //! Struct dedicated to the `LINK` tag.
 
 use std::{
   collections::HashMap,
   fmt::{self, Debug},
-  io::{BufRead, Write},
   str::{self, FromStr},
 };
 
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesText, Event},
-  Reader, Writer,
-};
 use serde_json::Value;
 
-use super::{
-  error::VOTableError,
-  utils::{discard_comment, discard_event},
-  QuickXmlReadWrite,
-};
+use super::{error::VOTableError, HasContent, HasContentElem, VOTableElement};
 
+/// Enum for the possible values of the `content-role` attriute.
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 pub enum ContentRole {
   Query,
   Hints,
   Doc,
   Location,
 }
@@ -55,14 +47,15 @@
 
 impl fmt::Display for ContentRole {
   fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
     Debug::fmt(self, f)
   }
 }
 
+/// Struct corresponding to the `LINK` XML tag.
 #[derive(Default, Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct Link {
   #[serde(rename = "ID", skip_serializing_if = "Option::is_none")]
   pub id: Option<String>,
   #[serde(rename = "content-role", skip_serializing_if = "Option::is_none")]
   pub content_role: Option<ContentRole>,
   #[serde(rename = "content-type", skip_serializing_if = "Option::is_none")]
@@ -82,115 +75,86 @@
 }
 
 impl Link {
   pub fn new() -> Self {
     Self::default()
   }
 
+  // attributes
   impl_builder_opt_string_attr!(id);
   impl_builder_opt_attr!(content_role, ContentRole);
   impl_builder_opt_string_attr!(content_type);
   impl_builder_opt_string_attr!(title);
   impl_builder_opt_string_attr!(value);
   impl_builder_opt_string_attr!(href);
-
+  // extra attributes
   impl_builder_insert_extra!();
+}
+impl_has_content!(Link);
+
+impl VOTableElement for Link {
+  const TAG: &'static str = "LINK";
+
+  type MarkerType = HasContentElem;
 
-  impl_builder_opt_string_attr!(content);
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new().set_attrs(attrs)
+  }
 
-  /// Calls a closure on each (key, value) attribute pairs.
-  pub fn for_each_attribute<F>(&self, mut f: F)
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "ID" => self.set_id_by_ref(val),
+        "content-role" => {
+          self.set_content_role_by_ref(val.as_ref().parse().map_err(VOTableError::Custom)?)
+        }
+        "content-type" => self.set_content_type_by_ref(val),
+        "title" => self.set_title_by_ref(val),
+        "value" => self.set_value_by_ref(val),
+        "href" => self.set_href_by_ref(val),
+        _ => self.insert_extra_str_by_ref(key, val),
+      }
+    }
+    Ok(())
+  }
+
+  fn for_each_attribute<F>(&self, mut f: F)
   where
     F: FnMut(&str, &str),
   {
     if let Some(id) = &self.id {
       f("ID", id.as_str());
     }
     if let Some(content_role) = &self.content_role {
-      f("content-role", content_role.to_string().as_str());
+      f("content-role", content_role.into());
     }
     if let Some(content_type) = &self.content_type {
       f("content-type", content_type.as_str());
     }
     if let Some(title) = &self.title {
       f("title", title.as_str());
     }
     if let Some(value) = &self.value {
       f("value", value.as_str());
     }
     if let Some(href) = &self.href {
       f("href", href.as_str());
     }
-    for (k, v) in &self.extra {
-      f(k.as_str(), v.to_string().as_str());
-    }
-  }
-}
-
-impl QuickXmlReadWrite for Link {
-  const TAG: &'static str = "LINK";
-  type Context = ();
-
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut link = Self::new();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      link = match attr.key {
-        b"ID" => link.set_id(value),
-        b"content-role" => {
-          link.set_content_role(ContentRole::from_str(value).map_err(VOTableError::Custom)?)
-        }
-        b"content-type" => link.set_content_type(value),
-        b"title" => link.set_title(value),
-        b"value" => link.set_value(value),
-        b"href" => link.set_href(value),
-        _ => link.insert_extra(
-          str::from_utf8(attr.key).map_err(VOTableError::Utf8)?,
-          Value::String(value.into()),
-        ),
-      }
-    }
-    Ok(link)
-  }
-
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    read_content!(Self, self, reader, reader_buff)
-  }
-
-  fn read_sub_elements_by_ref<R: BufRead>(
-    &mut self,
-    reader: &mut Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    read_content_by_ref!(Self, self, reader, reader_buff)
-  }
-
-  fn write<W: Write>(
-    &mut self,
-    writer: &mut Writer<W>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    let mut elem_writer = writer.create_element(Self::TAG_BYTES);
-    write_opt_string_attr!(self, elem_writer, ID);
-    write_opt_into_attr!(self, elem_writer, content_role, "content-role");
-    write_opt_string_attr!(self, elem_writer, content_type, "content-type");
-    write_opt_string_attr!(self, elem_writer, title);
-    write_opt_string_attr!(self, elem_writer, value);
-    write_opt_string_attr!(self, elem_writer, href);
-    write_extra!(self, elem_writer);
-    write_content!(self, elem_writer);
-    Ok(())
+    for_each_extra_attribute!(self, f);
   }
 }
 
 #[cfg(test)]
 mod tests {
   use crate::{
     link::Link,
```

### Comparing `votable_cli-0.5.0/src/mivot/attribute.rs` & `votable_cli-0.6.0/src/mivot/attribute.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 //! Contains common code for `ATTRIBUTE` child of `COLLECTION` and `INSTANCE`
 //! in both `GLOBALS` and `TEMPLATES`.
 
-use std::{io::Write, str};
+use std::str;
 
 use paste::paste;
 
-use quick_xml::{events::attributes::Attributes, ElementWriter, Reader, Writer};
-
-use crate::{error::VOTableError, mivot::VodmlVisitor, QuickXmlReadWrite};
+use crate::{
+  error::VOTableError, mivot::VodmlVisitor, utils::unexpected_attr_err, EmptyElem, VOTableElement,
+};
 
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(untagged)]
 pub enum RefOrValueOrBoth {
   Ref {
     #[serde(rename = "ref")]
     ref_: String,
@@ -55,22 +55,26 @@
       1 => Ok(Self::from_value(value)),
       2 => Ok(Self::from_ref(ref_)),
       3 => Ok(Self::from_ref_with_default(ref_, value)),
       _ => unreachable!(),
     }
   }
 
-  pub fn push_in_tag<'a, W: Write>(&'a self, tag: ElementWriter<'a, W>) -> ElementWriter<W> {
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
     match self {
-      Self::Ref { ref_ } => tag.with_attribute(("ref", ref_.as_str())),
-      Self::Value { value } => tag.with_attribute(("value", value.as_str())),
-      Self::RefAndValue { ref_, value } => tag
-        .with_attribute(("ref", ref_.as_str()))
-        .with_attribute(("value", value.as_str())),
-    }
+      Self::Ref { ref_ } => f("ref", ref_.as_str()),
+      Self::Value { value } => f("value", value.as_str()),
+      Self::RefAndValue { ref_, value } => {
+        f("ref", ref_.as_str());
+        f("value", value.as_str())
+      }
+    };
   }
 }
 
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 pub struct AttributeChildOfInstance {
   /// Attribute name.
   pub dmrole: String,
@@ -129,98 +133,104 @@
       dmtype: dmtype.into(),
       ref_or_val_or_both: RefOrValueOrBoth::from_ref_with_default(ref_, default_value),
       arrayindex: None,
       unit: None,
     }
   }
 
+  impl_builder_mandatory_string_attr!(dmrole);
+  impl_builder_mandatory_string_attr!(dmtype);
+  impl_builder_mandatory_attr!(ref_or_val_or_both, RefOrValueOrBoth);
   impl_builder_opt_attr!(arrayindex, u32);
   impl_builder_opt_string_attr!(unit);
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
     visitor.visit_attribute_childof_instance(self)
   }
 }
-impl QuickXmlReadWrite for AttributeChildOfInstance {
+
+impl VOTableElement for AttributeChildOfInstance {
   const TAG: &'static str = "ATTRIBUTE";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut dmrole = String::from("");
-    let mut dmtype = String::from("");
-    let mut ref_ = String::from("");
-    let mut value = String::from("");
-    let mut arrayindex: Option<u32> = None;
-    let mut unit = String::from("");
+  type MarkerType = EmptyElem;
 
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let val = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      if !val.is_empty() {
-        match attr.key {
-          b"dmrole" => dmrole = val.to_string(),
-          b"dmtype" => dmtype = val.to_string(),
-          b"ref" => ref_ = val.to_string(),
-          b"value" => value = val.to_string(),
-          b"arrayindex" => {
-            arrayindex = Some(val.parse::<u32>().map_err(|e| {
-              VOTableError::Custom(format!(
-                "Unable to parse 'arrayindex' attribute '{}': {}",
-                val, e
-              ))
-            })?)
-          }
-          b"unit" => unit = val.to_string(),
-          _ => {
-            return Err(VOTableError::UnexpectedAttr(attr.key.to_vec(), Self::TAG));
-          }
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    const DEFAULT_VALUE: &str = "@TBD";
+    Self::from_ref(DEFAULT_VALUE, DEFAULT_VALUE, DEFAULT_VALUE).set_attrs(attrs).and_then(|attr| {
+      if attr.dmrole.as_str() == DEFAULT_VALUE {
+        Err(VOTableError::Custom(format!(
+          "Mandatory attribute 'dmrole' not found in tag '{}' child of INSTANCE child of GLOBALS",
+          Self::TAG
+        )))
+      } else if attr.dmtype.as_str() == DEFAULT_VALUE {
+        Err(VOTableError::Custom(format!(
+          "Mandatory attribute 'dmtype' not found in tag '{}' child of INSTANCE child of GLOBALS",
+          &Self::TAG
+        )))
+      } else if let RefOrValueOrBoth::Ref { ref_: e } = &attr.ref_or_val_or_both {
+        if e.as_str() == DEFAULT_VALUE {
+          Err(VOTableError::Custom(format!(
+            "Mandatory attributes 'ref' or 'value' not found in tag '{}' child of INSTANCE child of GLOBALS",
+            &Self::TAG
+          )))
+        } else {
+          Ok(attr)
         }
-      };
-    }
-
-    if dmrole.is_empty() {
-      Err(VOTableError::Custom(format!(
-        "Attribute 'dmrole' mandatory in tag {} child of INSTANCE child of GLOBALS",
-        &Self::TAG
-      )))
-    } else if dmtype.is_empty() {
-      Err(VOTableError::Custom(format!(
-        "Attribute 'dmtype'  mandatory in tag {} child of INSTANCE child of GLOBALS",
-        &Self::TAG
-      )))
-    } else {
-      let ref_or_val = RefOrValueOrBoth::from_possibly_empty_ref_or_val(ref_, value)?;
-      let mut tag = Self::new(dmrole, dmtype, ref_or_val);
-      if let Some(arrayindex) = arrayindex {
-        tag = tag.set_arrayindex(arrayindex);
+      } else {
+        Ok(attr)
       }
-      if !unit.is_empty() {
-        tag = tag.set_unit(unit);
+    })
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    let mut ref_ = String::from("");
+    let mut value = String::from("");
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "dmrole" => self.set_dmrole_by_ref(val),
+        "dmtype" => self.set_dmtype_by_ref(val),
+        "ref" => ref_ = val.into(),
+        "value" => value = val.into(),
+        "arrayindex" => {
+          self.set_arrayindex_by_ref(val.as_ref().parse().map_err(VOTableError::ParseInt)?)
+        }
+        "unit" => self.set_unit_by_ref(val),
+        _ => return Err(unexpected_attr_err(key, Self::TAG)),
       }
-      Ok(tag)
     }
+    self.set_ref_or_val_or_both_by_ref(RefOrValueOrBoth::from_possibly_empty_ref_or_val(
+      ref_, value,
+    )?);
+    Ok(())
   }
 
-  empty_read_sub!();
-
-  fn write<W: Write>(
-    &mut self,
-    writer: &mut Writer<W>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    let mut tag = writer
-      .create_element(Self::TAG_BYTES)
-      .with_attribute(("dmrole", self.dmrole.as_str()))
-      .with_attribute(("dmtype", self.dmtype.as_str()));
-    tag = self.ref_or_val_or_both.push_in_tag(tag);
-    write_opt_tostring_attr!(self, tag, arrayindex, "arrayindex");
-    write_opt_string_attr!(self, tag, unit);
-    tag.write_empty().map_err(VOTableError::Write)?;
-    Ok(())
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    f("dmrole", self.dmrole.as_str());
+    f("dmtype", self.dmtype.as_str());
+    self.ref_or_val_or_both.for_each_attribute(&mut f);
+    if let Some(arrayindex) = &self.arrayindex {
+      f("arrayindex", arrayindex.to_string().as_str());
+    }
+    if let Some(unit) = &self.unit {
+      f("unit", unit.as_str());
+    }
   }
 }
 
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 pub struct AttributeChildOfCollection {
   /// Attribute type.
   pub dmtype: String,
@@ -268,90 +278,96 @@
       dmtype: dmtype.into(),
       ref_or_val_or_both: RefOrValueOrBoth::from_ref_with_default(ref_, default_value),
       arrayindex: None,
       unit: None,
     }
   }
 
+  impl_builder_mandatory_string_attr!(dmtype);
+  impl_builder_mandatory_attr!(ref_or_val_or_both, RefOrValueOrBoth);
   impl_builder_opt_attr!(arrayindex, u32);
   impl_builder_opt_string_attr!(unit);
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
     visitor.visit_attribute_childof_collection(self)
   }
 }
-impl QuickXmlReadWrite for AttributeChildOfCollection {
+
+impl VOTableElement for AttributeChildOfCollection {
   const TAG: &'static str = "ATTRIBUTE";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut dmtype = String::from("");
-    let mut ref_ = String::from("");
-    let mut value = String::from("");
-    let mut arrayindex: Option<u32> = None;
-    let mut unit = String::from("");
+  type MarkerType = EmptyElem;
 
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let val = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      if !val.is_empty() {
-        match attr.key {
-          b"dmtype" => dmtype = val.to_string(),
-          b"ref" => ref_ = val.to_string(),
-          b"value" => value = val.to_string(),
-          b"arrayindex" => {
-            arrayindex = Some(val.parse::<u32>().map_err(|e| {
-              VOTableError::Custom(format!(
-                "Unable to parse 'arrayindex' attribute '{}': {}",
-                val, e
-              ))
-            })?)
-          }
-          b"unit" => unit = val.to_string(),
-          _ => {
-            return Err(VOTableError::UnexpectedAttr(attr.key.to_vec(), Self::TAG));
-          }
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    const DEFAULT_VALUE: &str = "@TBD";
+    Self::from_ref(DEFAULT_VALUE, DEFAULT_VALUE).set_attrs(attrs).and_then(|attr| {
+      if attr.dmtype.as_str() == DEFAULT_VALUE {
+        Err(VOTableError::Custom(format!(
+          "Mandatory attribute 'dmtype' not found in tag '{}' child of COLLECTION child of GLOBALS",
+          &Self::TAG
+        )))
+      } else if let RefOrValueOrBoth::Ref { ref_: e } = &attr.ref_or_val_or_both {
+        if e.as_str() == DEFAULT_VALUE {
+          Err(VOTableError::Custom(format!(
+            "Mandatory attributes 'ref' or 'value' not found in tag '{}' child of COLLECTION child of GLOBALS",
+            &Self::TAG
+          )))
+        } else {
+          Ok(attr)
         }
-      };
-    }
-
-    if dmtype.is_empty() {
-      Err(VOTableError::Custom(format!(
-        "Attribute 'dmtype'  mandatory in tag {} child of COLLECTION child of GLOBALS",
-        &Self::TAG
-      )))
-    } else {
-      let ref_or_val = RefOrValueOrBoth::from_possibly_empty_ref_or_val(ref_, value)?;
-      let mut tag = Self::new(dmtype, ref_or_val);
-      if let Some(arrayindex) = arrayindex {
-        tag = tag.set_arrayindex(arrayindex);
+      } else {
+        Ok(attr)
       }
-      if !unit.is_empty() {
-        tag = tag.set_unit(unit);
+    })
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    let mut ref_ = String::from("");
+    let mut value = String::from("");
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "dmtype" => self.set_dmtype_by_ref(val),
+        "ref" => ref_ = val.into(),
+        "value" => value = val.into(),
+        "arrayindex" => {
+          self.set_arrayindex_by_ref(val.as_ref().parse().map_err(VOTableError::ParseInt)?)
+        }
+        "unit" => self.set_unit_by_ref(val),
+        _ => return Err(unexpected_attr_err(key, Self::TAG)),
       }
-      Ok(tag)
     }
+    self.set_ref_or_val_or_both_by_ref(RefOrValueOrBoth::from_possibly_empty_ref_or_val(
+      ref_, value,
+    )?);
+    Ok(())
   }
 
-  empty_read_sub!();
-
-  fn write<W: Write>(
-    &mut self,
-    writer: &mut Writer<W>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    let mut tag = writer
-      .create_element(Self::TAG_BYTES)
-      .with_attribute(("dmtype", self.dmtype.as_str()));
-    tag = self.ref_or_val_or_both.push_in_tag(tag);
-    write_opt_tostring_attr!(self, tag, arrayindex);
-    write_opt_tostring_attr!(self, tag, unit);
-    tag.write_empty().map_err(VOTableError::Write)?;
-    Ok(())
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    f("dmtype", self.dmtype.as_str());
+    self.ref_or_val_or_both.for_each_attribute(&mut f);
+    if let Some(arrayindex) = &self.arrayindex {
+      f("arrayindex", arrayindex.to_string().as_str());
+    }
+    if let Some(unit) = &self.unit {
+      f("unit", unit.as_str());
+    }
   }
 }
 
 #[cfg(test)]
 mod tests {
   use crate::{
     mivot::test::{get_xml, test_error},
```

### Comparing `votable_cli-0.5.0/src/mivot/globals/collection/instance.rs` & `votable_cli-0.6.0/src/mivot/globals/collection/instance.rs`

 * *Files 12% similar despite different names*

```diff
@@ -5,24 +5,21 @@
 
 use std::{
   io::{BufRead, Write},
   str,
 };
 
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
-  Reader, Writer,
-};
+use quick_xml::{events::Event, Reader, Writer};
 
 use crate::{
   error::VOTableError,
   mivot::{attribute::AttributeChildOfInstance as Attribute, VodmlVisitor},
-  utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite,
+  utils::{discard_comment, discard_event, is_empty, unexpected_attr_err},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, VOTableElement,
 };
 
 use super::super::instance::{
   collection::Collection, instance::Instance as InstanceChildOfInstance,
   primary_key::PrimaryKeyStatic as PrimaryKey, reference::Reference, InstanceElem,
 };
 
@@ -54,177 +51,162 @@
       dmtype: dmtype.into(),
       primarykeys: Default::default(),
       elems: Default::default(),
     }
   }
 
   impl_builder_opt_string_attr!(dmid);
+  impl_builder_mandatory_string_attr!(dmtype);
 
   impl_builder_push!(PrimaryKey);
 
   impl_builder_push_elem!(Attribute, InstanceElem);
   impl_builder_push_elem!(Instance, InstanceElem, InstanceChildOfInstance);
   impl_builder_push_elem!(Reference, InstanceElem);
   impl_builder_push_elem!(Collection, InstanceElem);
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    visitor.visit_instance_childof_collection_in_globals(self)?;
+    visitor.visit_instance_childof_collection_in_globals_start(self)?;
     for pk in self.primarykeys.iter_mut() {
       pk.visit(visitor)?;
     }
     for elem in self.elems.iter_mut() {
       elem.visit(visitor)?;
     }
-    Ok(())
+    visitor.visit_instance_childof_collection_in_globals_ended(self)
   }
 }
 
-impl QuickXmlReadWrite for Instance {
+impl VOTableElement for Instance {
   const TAG: &'static str = "INSTANCE";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut dmid = String::new();
-    let mut dmtype = String::new();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      if !value.is_empty() {
-        match attr.key {
-          b"dmid" => dmid.push_str(value),
-          b"dmtype" => dmtype.push_str(value),
-          _ => {
-            return Err(VOTableError::UnexpectedAttr(
-              attr.key.to_vec(),
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new_tmp("").set_attrs(attrs).and_then(|instance| {
+      if instance.dmtype.is_empty() {
+        Err(VOTableError::Custom(format!(
+          "Attribute 'dmtype' is mandatory and must be non-empty in tag '{}' child of GLOBALS",
+          Self::TAG
+        )))
+      } else {
+        Ok(instance)
+      }
+    })
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "dmid" => self.set_dmid_by_ref(val),
+        "dmtype" => self.set_dmtype_by_ref(val),
+        _ => {
+          if !val.as_ref().is_empty() {
+            return Err(unexpected_attr_err(
+              key,
               "INSTANCE child of COLLECTION child of GLOBALS",
-            ))
+            ));
           }
         }
       }
     }
-    if dmtype.is_empty() {
-      Err(VOTableError::Custom(format!(
-        "Attribute 'dmtype' is mandatory and must be non-empty in tag '{}' child of GLOBALS",
-        Self::TAG
-      )))
-    } else {
-      // TODO: replace this by a code similar to COLLECTION not to use a constructor with empty PRIMARY_KEY
-      let mut elem = Self::new_tmp(dmtype);
-      if !dmid.is_empty() {
-        elem = elem.set_dmid(dmid);
-      }
-      Ok(elem)
+    Ok(())
+  }
+
+  /// Calls a closure on each (key, value) attribute pairs.
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    if let Some(dmid) = &self.dmid {
+      f("dmid", dmid.as_str());
     }
+    f("dmtype", self.dmtype.as_str());
   }
+}
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+impl HasSubElements for Instance {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    // Note: Should always be true to be a valid Instance element
+    self.primarykeys.is_empty() && self.elems.is_empty()
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          InstanceChildOfInstance::TAG_BYTES => {
-            self
-              .elems
-              .push(InstanceElem::Instance(from_event_start_by_ref!(
-                InstanceChildOfInstance,
-                reader,
-                reader_buff,
-                e
-              )))
-          }
+          InstanceChildOfInstance::TAG_BYTES => self.push_instance_by_ref(
+            from_event_start_by_ref!(InstanceChildOfInstance, reader, reader_buff, e),
+          ),
           Reference::TAG_BYTES => {
-            self
-              .elems
-              .push(InstanceElem::Reference(from_event_start_by_ref!(
-                Reference,
-                reader,
-                reader_buff,
-                e
-              )))
-          }
-          Collection::TAG_BYTES => {
-            self
-              .elems
-              .push(InstanceElem::Collection(from_event_start_by_ref!(
-                Collection,
-                reader,
-                reader_buff,
-                e
-              )))
+            self.push_reference_by_ref(from_event_start_by_ref!(Reference, reader, reader_buff, e))
           }
+          Collection::TAG_BYTES => self.push_collection_by_ref(from_event_start_by_ref!(
+            Collection,
+            reader,
+            reader_buff,
+            e
+          )),
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
-          PrimaryKey::TAG_BYTES => self.primarykeys.push(PrimaryKey::from_event_empty(e)?),
-          Attribute::TAG_BYTES => self
-            .elems
-            .push(InstanceElem::Attribute(Attribute::from_event_empty(e)?)),
-          Reference::TAG_BYTES => self
-            .elems
-            .push(InstanceElem::Reference(Reference::from_event_empty(e)?)),
+          PrimaryKey::TAG_BYTES => self.push_primarykey_by_ref(PrimaryKey::from_event_empty(e)?),
+          Attribute::TAG_BYTES => self.push_attribute_by_ref(Attribute::from_event_empty(e)?),
+          Reference::TAG_BYTES => self.push_reference_by_ref(Reference::from_event_empty(e)?),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Text(e) if is_empty(e) => {}
         Event::End(e) if e.local_name() == Self::TAG_BYTES => {
           return if self.primarykeys.is_empty() {
             Err(VOTableError::Custom(String::from(
-              "`INSTANCE` child of `COLLECTION` must contains at leas ont `PRIMARY_KEY`",
+              "`INSTANCE` child of `COLLECTION` must contains at least ont `PRIMARY_KEY`",
             )))
           } else {
             Ok(())
           }
         }
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    push2write_opt_string_attr!(self, tag, dmid);
-    tag.push_attribute(("dmtype", self.dmtype.as_str()));
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elements
     write_elem_vec!(self, primarykeys, writer, context);
     write_elem_vec_no_context!(self, elems, writer);
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    Ok(())
   }
 }
```

### Comparing `votable_cli-0.5.0/src/mivot/globals/collection/mod.rs` & `votable_cli-0.6.0/src/mivot/globals/collection/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 //! Hence, it has **no** `dmrole`.
 
 use std::{
   io::{BufRead, Write},
   str,
 };
 
+use paste::paste;
 use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
+  events::{attributes::Attributes, Event},
   Reader, Writer,
 };
 
 use crate::{
   error::VOTableError,
   mivot::{join::Join, VodmlVisitor},
-  utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite,
+  utils::{discard_comment, discard_event, is_empty, unexpected_attr_err},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, VOTableElement,
 };
 
 pub mod reference;
 use reference::Reference;
 
 pub mod instance;
 use instance::Instance;
@@ -208,14 +209,16 @@
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
+  impl_builder_mandatory_string_attr!(dmid);
+
   pub(crate) fn get_dmid_from_atttributes(attrs: Attributes) -> Result<String, VOTableError> {
     let mut dmid = String::new();
     for attr_res in attrs {
       let attr = attr_res.map_err(VOTableError::Attr)?;
       let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
       let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
       if !value.is_empty() {
@@ -225,65 +228,82 @@
         }
       };
     }
     Ok(dmid)
   }
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    visitor.visit_collection_childof_globals(self)?;
-    self.elems.visit(visitor)
+    visitor
+      .visit_collection_childof_globals_start(self)
+      .and_then(|()| self.elems.visit(visitor))
+      .and_then(|()| visitor.visit_collection_childof_globals_ended(self))
   }
 }
 
-impl QuickXmlReadWrite for Collection {
+impl VOTableElement for Collection {
   const TAG: &'static str = "COLLECTION";
-  type Context = ();
 
-  fn from_attributes(_attrs: Attributes) -> Result<Self, VOTableError> {
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(_attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
     Err(VOTableError::Custom(format!(
       "Tag {} cannot be built directly from attributes",
       Self::TAG
     )))
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "dmid" => self.set_dmid_by_ref(val),
+        _ => return Err(unexpected_attr_err(key, Self::TAG)),
+      }
+    }
+    Ok(())
+  }
+
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    f("dmid", self.dmid.as_str());
+  }
+}
+
+impl HasSubElements for Collection {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    false
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
-    mut _reader: &mut Reader<R>,
-    mut _reader_buff: &mut Vec<u8>,
+    _reader: &mut Reader<R>,
+    _reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     Err(VOTableError::Custom(format!(
       "Tag {} cannot be built before reading sub-elements",
       Self::TAG
     )))
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    tag.push_attribute(("name", self.dmid.as_str()));
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elements
-    self.elems.write(writer)?;
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    self.elems.write(writer)
   }
 }
```

### Comparing `votable_cli-0.5.0/src/mivot/globals/instance/collection/collection.rs` & `votable_cli-0.6.0/src/mivot/templates/instance/collection/collection.rs`

 * *Files 4% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 use std::{
   io::{BufRead, Write},
   str,
 };
 
 use paste::paste;
 use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
+  events::{attributes::Attributes, Event},
   Reader, Writer,
 };
 
 use crate::{
   error::VOTableError,
   mivot::{
-    attribute::AttributeChildOfCollection as Attribute,
-    globals::{collection::reference::Reference, instance::Instance}, // No dmrole
-    join::Join,
+    attribute::AttributeChildOfCollection as Attribute, join::Join, templates::instance::Instance,
     VodmlVisitor,
   },
-  utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite,
+  utils::{discard_comment, discard_event, is_empty, unexpected_attr_err},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, VOTableElement,
 };
 
+use super::reference::Reference;
+
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "elem_type")]
 pub enum InstanceOrRef {
   Instance(Instance),
   /// Reference here is **child of** `COLLECTION` in `GLOBALS`
   Reference(Reference),
 }
@@ -46,15 +46,14 @@
       InstanceOrRef::Reference(elem) => elem.visit(visitor),
     }
   }
 }
 
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "elem_type", content = "content")]
-// #[serde(untagged)]
 pub enum CollectionElems {
   Attribute(Vec<Attribute>),
   Collection(Vec<Collection>),
   InstanceOrRef(Vec<InstanceOrRef>),
   Join(Join),
 }
 
@@ -249,28 +248,28 @@
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Text(e) if is_empty(e) => {}
         Event::End(e) if e.local_name() == Self::TAG_BYTES => {
-          return match (((!attr_vec.is_empty()) as u8) << 3)
+          return match (((!attr_vec.is_empty()) as u8) << 4)
             + (((!col_vec.is_empty()) as u8) << 2)
             + (((!inst_or_ref_vec.is_empty()) as u8) << 1)
             + ((!join_vec.is_empty()) as u8)
           {
             8 => Self::from_attribute(attr_vec),
             4 => Self::from_collections(col_vec),
             2 => Self::from_instance_or_reference_elems(inst_or_ref_vec),
             1 if join_vec.len() == 1 => Self::from_join(join_vec.drain(..).next().unwrap()),
             1 => Err(VOTableError::Custom(
               "A collection cannot have more than one join".to_owned(),
             )),
             0 => Err(VOTableError::Custom(
-              "In COLLECTION child of COLLECTION in GLOBALS: must have at least one item"
+              "In COLLECTION child of COLLECTION in TEMPLATES: must have at least one item"
                 .to_owned(),
             )),
             _ => Err(VOTableError::Custom(
               "A collection cannot have items of different types".to_owned(),
             )),
           } // Set dmid if any
           .map(|c| {
@@ -285,65 +284,84 @@
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    visitor.visit_collection_childof_collection_in_globals(self)?;
-    self.elems.visit(visitor)
+    visitor
+      .visit_collection_childof_collection_in_templates_start(self)
+      .and_then(|()| self.elems.visit(visitor))
+      .and_then(|()| visitor.visit_collection_childof_collection_in_templates_ended(self))
   }
 }
 
-impl QuickXmlReadWrite for Collection {
+impl VOTableElement for Collection {
   const TAG: &'static str = "COLLECTION";
-  type Context = ();
 
-  fn from_attributes(_attrs: Attributes) -> Result<Self, VOTableError> {
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(_attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
     Err(VOTableError::Custom(format!(
       "Tag {} cannot be built directly from attributes",
       Self::TAG
     )))
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "dmid" => self.set_dmid_by_ref(val),
+        _ => return Err(unexpected_attr_err(key, Self::TAG)),
+      }
+    }
+    Ok(())
+  }
+
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    if let Some(dmid) = &self.dmid {
+      f("dmid", dmid.as_str());
+    }
+  }
+}
+
+impl HasSubElements for Collection {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    false
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
-    mut _reader: &mut Reader<R>,
-    mut _reader_buff: &mut Vec<u8>,
+    _reader: &mut Reader<R>,
+    _reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     Err(VOTableError::Custom(format!(
       "Tag {} cannot be built before reading sub-elements",
       Self::TAG
     )))
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    push2write_opt_string_attr!(self, tag, dmid);
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elements
-    self.elems.write(writer)?;
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    self.elems.write(writer)
   }
 }
```

### Comparing `votable_cli-0.5.0/src/mivot/globals/instance/collection/mod.rs` & `votable_cli-0.6.0/src/mivot/globals/instance/collection/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 use std::{
   io::{BufRead, Write},
   str,
 };
 
 use paste::paste;
 use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
+  events::{attributes::Attributes, Event},
   Reader, Writer,
 };
 
 use crate::{
   error::VOTableError,
   mivot::{
     attribute::AttributeChildOfCollection as Attribute,
     globals::{collection::reference::Reference, instance::Instance},
     join::Join,
     VodmlVisitor,
   },
-  utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite,
+  utils::{discard_comment, discard_event, is_empty, unexpected_attr_err},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, VOTableElement,
 };
 
 pub mod collection;
 use collection::{Collection as CollectionChildOfCollection, CollectionElems, InstanceOrRef};
 
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 pub struct Collection {
@@ -136,14 +136,15 @@
         dmrole,
         dmid: None,
         elems: CollectionElems::Join(join),
       })
     }
   }
 
+  impl_builder_mandatory_string_attr!(dmrole);
   impl_builder_opt_string_attr!(dmid);
 
   pub(crate) fn get_dmrole_opt_dmid_from_atttributes(
     attrs: Attributes,
   ) -> Result<(String, Option<String>), VOTableError> {
     let mut dmrole = String::new();
     let mut dmid: Option<String> = None;
@@ -257,66 +258,86 @@
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    visitor.visit_collection_childof_instance_in_globals(self)?;
-    self.elems.visit(visitor)
+    visitor
+      .visit_collection_childof_instance_in_globals_start(self)
+      .and_then(|()| self.elems.visit(visitor))
+      .and_then(|()| visitor.visit_collection_childof_instance_in_globals_ended(self))
   }
 }
 
-impl QuickXmlReadWrite for Collection {
+impl VOTableElement for Collection {
   const TAG: &'static str = "COLLECTION";
-  type Context = ();
 
-  fn from_attributes(_attrs: Attributes) -> Result<Self, VOTableError> {
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(_attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
     Err(VOTableError::Custom(format!(
       "Tag {} cannot be built directly from attributes",
       Self::TAG
     )))
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "dmrole" => self.set_dmrole_by_ref(val),
+        "dmid" => self.set_dmid_by_ref(val),
+        _ => return Err(unexpected_attr_err(key, Self::TAG)),
+      }
+    }
+    Ok(())
+  }
+
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    f("dmrole", self.dmrole.as_str());
+    if let Some(dmid) = &self.dmid {
+      f("dmid", dmid.as_str());
+    }
+  }
+}
+
+impl HasSubElements for Collection {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    false
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
-    mut _reader: &mut Reader<R>,
-    mut _reader_buff: &mut Vec<u8>,
+    _reader: &mut Reader<R>,
+    _reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     Err(VOTableError::Custom(format!(
       "Tag {} cannot be built before reading sub-elements",
       Self::TAG
     )))
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    tag.push_attribute(("dmrole", self.dmrole.as_str()));
-    push2write_opt_string_attr!(self, tag, dmid);
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elements
-    self.elems.write(writer)?;
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    self.elems.write(writer)
   }
 }
```

### Comparing `votable_cli-0.5.0/src/mivot/globals/instance/instance.rs` & `votable_cli-0.6.0/src/mivot/globals/mod.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,205 +1,203 @@
-//! Here `INSTANCE` is a **child of** `INSTANCE`.
-//! Hence, it **must have** `dmrole`.
+//! Module dedicated to the `GLOBALS` tag.
+//!
+//! The `GLOBALS` block contains model element(s)  having no reference to any table.
+//! Thus, an element in a `GLOBALS` block cannot contains a `ref` attribute pointing to a table
+//! (`FIELD` or `PARAM`), **but** it may contain a `ref` attribute pointing to a `PARAM` which is
+//! not in a VOTable table.
+//! For `PRIMARY_KEY`,
 
 use std::{
   io::{BufRead, Write},
   str,
 };
 
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
-  Reader, Writer,
-};
+use quick_xml::{events::Event, Reader, Writer};
 
 use crate::{
   error::VOTableError,
-  mivot::{attribute::AttributeChildOfInstance as Attribute, VodmlVisitor},
-  utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite,
+  mivot::VodmlVisitor,
+  utils::{discard_comment, discard_event, is_empty, unexpected_attr_err},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, VOTableElement,
 };
 
-use super::{
-  collection::Collection, primary_key::PrimaryKeyStatic as PrimaryKey, reference::Reference,
-  InstanceElem,
-};
+pub mod collection;
+use collection::Collection;
+
+pub mod instance;
+use instance::Instance;
 
-/// The same as `INSTANCE` **child of** `GLOBALS`, but with having a `dmrole`.
+/// The two sub-elements `GLOBALS` may contains (in any order).
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
-pub struct Instance {
-  #[serde(skip_serializing_if = "Option::is_none")]
-  pub dmid: Option<String>,
-  pub dmrole: String,
-  pub dmtype: String,
-  #[serde(skip_serializing_if = "Vec::is_empty")]
-  pub primarykeys: Vec<PrimaryKey>,
-  #[serde(skip_serializing_if = "Vec::is_empty")]
-  pub elems: Vec<InstanceElem>,
+#[serde(tag = "elem_type")]
+pub enum GlobalsElem {
+  Instance(Instance),
+  Collection(Collection),
 }
+impl GlobalsElem {
+  fn write<W: Write>(&mut self, writer: &mut Writer<W>) -> Result<(), VOTableError> {
+    match self {
+      GlobalsElem::Instance(elem) => elem.write(writer, &()),
+      GlobalsElem::Collection(elem) => elem.write(writer, &()),
+    }
+  }
 
-impl Instance {
-  impl_new!([dmrole, dmtype], [dmid], [primarykeys, elems]);
+  pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
+    match self {
+      GlobalsElem::Instance(elem) => elem.visit(visitor),
+      GlobalsElem::Collection(elem) => elem.visit(visitor),
+    }
+  }
+}
 
-  impl_builder_opt_string_attr!(dmid);
+/// Structure storing the content of the `GLOABLS` tag.
+#[derive(Clone, Debug, PartialEq, Eq, Default, serde::Serialize, serde::Deserialize)]
+pub struct Globals {
+  #[serde(skip_serializing_if = "Vec::is_empty")]
+  pub elems: Vec<GlobalsElem>,
+}
 
-  impl_builder_push!(PrimaryKey);
+impl Globals {
+  pub fn new() -> Self {
+    Self {
+      elems: Default::default(),
+    }
+  }
 
-  impl_builder_push_elem!(Attribute, InstanceElem);
-  impl_builder_push_elem!(Instance, InstanceElem);
-  impl_builder_push_elem!(Reference, InstanceElem);
-  impl_builder_push_elem!(Collection, InstanceElem);
+  impl_builder_push_elem!(Instance, GlobalsElem);
+  impl_builder_push_elem!(Collection, GlobalsElem);
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    visitor.visit_instance_childof_instance_in_globals(self)?;
-    for pk in self.primarykeys.iter_mut() {
-      pk.visit(visitor)?;
-    }
+    visitor.visit_globals_start(self)?;
     for elem in self.elems.iter_mut() {
       elem.visit(visitor)?;
     }
-    Ok(())
+    visitor.visit_globals_ended(self)
   }
 }
 
-impl QuickXmlReadWrite for Instance {
-  const TAG: &'static str = "INSTANCE";
-  type Context = ();
+impl VOTableElement for Globals {
+  const TAG: &'static str = "GLOBALS";
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut dmid = String::new();
-    let mut dmrole = String::new();
-    let mut dmtype = String::new();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      if !value.is_empty() {
-        match attr.key {
-          b"dmid" => dmid.push_str(value),
-          b"dmrole" => dmrole.push_str(value),
-          b"dmtype" => dmtype.push_str(value),
-          _ => {
-            return Err(VOTableError::UnexpectedAttr(
-              attr.key.to_vec(),
-              "INSTANCE child of INSTANCE child of GLOBALS",
-            ))
-          }
-        }
-      }
-    }
-    if dmtype.is_empty() || dmrole.is_empty() {
-      Err(VOTableError::Custom(format!(
-        "Attributes 'dmtype' and 'dmrole' are mandatory and must be non-empty in tag '{}' child of `INSTANCE`",
-        Self::TAG
-      )))
-    } else {
-      let mut elem = Self::new(dmrole, dmtype);
-      if !dmid.is_empty() {
-        elem = elem.set_dmid(dmid);
-      }
-      Ok(elem)
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new().set_attrs(attrs)
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, mut attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    if let Some((k, _)) = attrs.next() {
+      return Err(unexpected_attr_err(k.as_ref(), Self::TAG));
     }
+    Ok(())
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+  fn for_each_attribute<F>(&self, _f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+  }
+}
+
+impl HasSubElements for Globals {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    self.elems.is_empty()
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          Instance::TAG_BYTES => self
-            .elems
-            .push(InstanceElem::Instance(from_event_start_by_ref!(
-              Instance,
-              reader,
-              reader_buff,
-              e
-            ))),
-          Reference::TAG_BYTES => {
-            self
-              .elems
-              .push(InstanceElem::Reference(from_event_start_by_ref!(
-                Reference,
-                reader,
-                reader_buff,
-                e
-              )))
-          }
+          Instance::TAG_BYTES => push_from_event_start!(self, Instance, reader, reader_buff, e),
           Collection::TAG_BYTES => {
-            self
-              .elems
-              .push(InstanceElem::Collection(from_event_start_by_ref!(
-                Collection,
-                reader,
-                reader_buff,
-                e
-              )))
+            let dmid = Collection::get_dmid_from_atttributes(e.attributes())?;
+            let collection =
+              Collection::from_dmid_and_reading_sub_elems(dmid, &(), reader, reader_buff)?;
+            self.push_collection_by_ref(collection);
           }
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
-          PrimaryKey::TAG_BYTES => self.primarykeys.push(PrimaryKey::from_event_empty(e)?),
-          Attribute::TAG_BYTES => self
-            .elems
-            .push(InstanceElem::Attribute(Attribute::from_event_empty(e)?)),
-          Reference::TAG_BYTES => self
-            .elems
-            .push(InstanceElem::Reference(Reference::from_event_empty(e)?)),
+          Instance::TAG_BYTES => push_from_event_empty!(self, Instance, e),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
-            ))
+            ));
           }
         },
         Event::Text(e) if is_empty(e) => {}
         Event::End(e) if e.local_name() == Self::TAG_BYTES => return Ok(()),
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
-    context: &Self::Context,
+    _context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    push2write_opt_string_attr!(self, tag, dmid);
-    tag.push_attribute(("dmrole", self.dmrole.as_str()));
-    tag.push_attribute(("dmtype", self.dmtype.as_str()));
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elements
-    write_elem_vec!(self, primarykeys, writer, context);
     write_elem_vec_no_context!(self, elems, writer);
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    Ok(())
+  }
+}
+
+#[cfg(test)]
+mod tests {
+  use crate::{
+    mivot::globals::Globals,
+    mivot::test::{get_xml, test_error},
+    tests::test_read,
+  };
+
+  #[test]
+  fn test_globals_read() {
+    // OK MODELS
+    // Should npot be valid according to 4.14 and Table 28: Dynamic Primary key only in TEMPLATES
+    //   let xml = get_xml("./resources/mivot/3/test_3_ok_3.1.xml");
+    //   println!("testing 3.1");
+    //   test_read::<Globals>(&xml);
+    //  let xml = get_xml("./resources/mivot/3/test_3_ok_3.2.xml");
+    //  println!("testing 3.2");
+    //  test_read::<Globals>(&xml);
+    let xml = get_xml("./resources/mivot/3/test_3_ok_3.3.xml");
+    println!("testing 3.3");
+    test_read::<Globals>(&xml);
+    //  let xml = get_xml("./resources/mivot/3/test_3_ok_3.4.xml");
+    //  println!("testing 3.4");
+    //  test_read::<Globals>(&xml);
+    let xml = get_xml("./resources/mivot/3/test_3_ok_3.5.xml");
+    println!("testing 3.5");
+    test_read::<Globals>(&xml);
+    // KO MODELS
+    let xml = get_xml("./resources/mivot/3/test_3_ko_3.6.xml");
+    println!("testing 3.6"); // Unexpected subnode.
+    test_error::<Globals>(&xml, false);
   }
 }
```

### Comparing `votable_cli-0.5.0/src/mivot/globals/instance/mod.rs` & `votable_cli-0.6.0/src/mivot/globals/instance/mod.rs`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,21 @@
 
 use std::{
   io::{BufRead, Write},
   str,
 };
 
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
-  Reader, Writer,
-};
+use quick_xml::{events::Event, Reader, Writer};
 
 use crate::{
   error::VOTableError,
   mivot::{attribute::AttributeChildOfInstance as Attribute, VodmlVisitor},
-  utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite,
+  utils::{discard_comment, discard_event, is_empty, unexpected_attr_err},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, VOTableElement,
 };
 
 pub mod collection;
 use collection::Collection;
 pub mod instance;
 use instance::Instance as InstanceChildOfInstance;
 pub mod primary_key;
@@ -66,143 +63,145 @@
   #[serde(skip_serializing_if = "Vec::is_empty")]
   pub primarykeys: Vec<PrimaryKey>,
   #[serde(skip_serializing_if = "Vec::is_empty")]
   pub elems: Vec<InstanceElem>,
 }
 
 impl Instance {
-  impl_new!([dmtype], [dmid], [primarykeys, elems]);
+  pub fn new<S: Into<String>>(dmtype: S) -> Self {
+    Self {
+      dmid: None,
+      dmtype: dmtype.into(),
+      primarykeys: Default::default(),
+      elems: Default::default(),
+    }
+  }
 
   impl_builder_opt_string_attr!(dmid);
+  impl_builder_mandatory_string_attr!(dmtype);
 
   impl_builder_push!(PrimaryKey);
 
   impl_builder_push_elem!(Attribute, InstanceElem);
   impl_builder_push_elem!(Instance, InstanceElem, InstanceChildOfInstance);
   impl_builder_push_elem!(Reference, InstanceElem);
   impl_builder_push_elem!(Collection, InstanceElem);
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    visitor.visit_instance_childof_globals(self)?;
+    visitor.visit_instance_childof_globals_start(self)?;
     for pk in self.primarykeys.iter_mut() {
       pk.visit(visitor)?;
     }
     for elem in self.elems.iter_mut() {
       elem.visit(visitor)?;
     }
-    Ok(())
+    visitor.visit_instance_childof_globals_ended(self)
   }
 }
 
-impl QuickXmlReadWrite for Instance {
+impl VOTableElement for Instance {
   const TAG: &'static str = "INSTANCE";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut dmid = String::new();
-    let mut dmtype = String::new();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      if !value.is_empty() {
-        match attr.key {
-          b"dmid" => dmid.push_str(value),
-          b"dmtype" => dmtype.push_str(value),
-          _ => {
-            return Err(VOTableError::UnexpectedAttr(
-              attr.key.to_vec(),
-              "INSTANCE child of GLOBALS",
-            ))
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new("").set_attrs(attrs).and_then(|instance| {
+      if instance.dmtype.is_empty() {
+        Err(VOTableError::Custom(format!(
+          "Attribute 'dmtype' is mandatory and must be non-empty in tag '{}' child of GLOBALS",
+          Self::TAG
+        )))
+      } else {
+        Ok(instance)
+      }
+    })
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "dmid" => self.set_dmid_by_ref(val),
+        "dmtype" => self.set_dmtype_by_ref(val),
+        _ => {
+          if !val.as_ref().is_empty() {
+            return Err(unexpected_attr_err(key, "INSTANCE child of GLOBALS"));
           }
         }
       }
     }
-    if dmtype.is_empty() {
-      Err(VOTableError::Custom(format!(
-        "Attribute 'dmtype' is mandatory and must be non-empty in tag '{}' child of GLOBALS",
-        Self::TAG
-      )))
-    } else {
-      let mut elem = Self::new(dmtype);
-      if !dmid.is_empty() {
-        elem = elem.set_dmid(dmid);
-      }
-      Ok(elem)
+    Ok(())
+  }
+
+  /// Calls a closure on each (key, value) attribute pairs.
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    if let Some(dmid) = &self.dmid {
+      f("dmid", dmid.as_str());
     }
+    f("dmtype", self.dmtype.as_str());
   }
+}
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+impl HasSubElements for Instance {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    false
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          InstanceChildOfInstance::TAG_BYTES => {
-            self
-              .elems
-              .push(InstanceElem::Instance(from_event_start_by_ref!(
-                InstanceChildOfInstance,
-                reader,
-                reader_buff,
-                e
-              )))
-          }
-          Reference::TAG_BYTES => {
-            self
-              .elems
-              .push(InstanceElem::Reference(from_event_start_by_ref!(
-                Reference,
-                reader,
-                reader_buff,
-                e
-              )))
-          }
+          InstanceChildOfInstance::TAG_BYTES => self.push_instance_by_ref(
+            from_event_start_by_ref!(InstanceChildOfInstance, reader, reader_buff, e),
+          ),
+          Reference::TAG_BYTES => push_from_event_start!(self, Reference, reader, reader_buff, e),
           Collection::TAG_BYTES => {
             let (dmrole, dmid_opt) =
               Collection::get_dmrole_opt_dmid_from_atttributes(e.attributes())?;
             let collection = Collection::from_dmrole_and_reading_sub_elems(
               dmrole,
               dmid_opt,
               &(),
               reader,
               reader_buff,
             )?;
-            self.elems.push(InstanceElem::Collection(collection))
+            self.push_collection_by_ref(collection)
           }
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
-          PrimaryKey::TAG_BYTES => self.primarykeys.push(PrimaryKey::from_event_empty(e)?),
-          Attribute::TAG_BYTES => self
-            .elems
-            .push(InstanceElem::Attribute(Attribute::from_event_empty(e)?)),
-          Reference::TAG_BYTES => self
-            .elems
-            .push(InstanceElem::Reference(Reference::from_event_empty(e)?)),
+          PrimaryKey::TAG_BYTES => push_from_event_empty!(self, PrimaryKey, e),
+          Attribute::TAG_BYTES => push_from_event_empty!(self, Attribute, e),
+          Reference::TAG_BYTES => push_from_event_empty!(self, Reference, e),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
@@ -211,28 +210,17 @@
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    push2write_opt_string_attr!(self, tag, dmid);
-    tag.push_attribute(("dmtype", self.dmtype.as_str()));
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elements
     write_elem_vec!(self, primarykeys, writer, context);
     write_elem_vec_no_context!(self, elems, writer);
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    Ok(())
   }
 }
```

### Comparing `votable_cli-0.5.0/src/mivot/globals/instance/primary_key.rs` & `votable_cli-0.6.0/src/mivot/globals/instance/primary_key.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,86 @@
 use std::str;
 
 use paste::paste;
-use quick_xml::{events::attributes::Attributes, Reader, Writer};
 
-use crate::{error::VOTableError, mivot::VodmlVisitor, QuickXmlReadWrite};
+use crate::{
+  error::VOTableError, mivot::VodmlVisitor, utils::unexpected_attr_err, EmptyElem, VOTableElement,
+};
 
 /// `Static` primary key can be both in `GLOBALS` or in `TEMPLATES`, but `GLOBALS` contains only
 /// static `PRIMARY_KEY`s
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 pub struct PrimaryKeyStatic {
   pub dmtype: String,
   pub value: String,
 }
+
 impl PrimaryKeyStatic {
-  impl_new!([dmtype, value], []);
-  impl_empty_new!([dmtype, value], []);
+  pub fn new<S: Into<String>>(dmtype: S, value: S) -> Self {
+    Self {
+      dmtype: dmtype.into(),
+      value: value.into(),
+    }
+  }
+
+  impl_builder_mandatory_string_attr!(dmtype);
+  impl_builder_mandatory_string_attr!(value);
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
     visitor.visit_primarykey_static(self)
   }
 }
 
-impl QuickXmlReadWrite for PrimaryKeyStatic {
+impl VOTableElement for PrimaryKeyStatic {
   const TAG: &'static str = "PRIMARY_KEY";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    const NULL: &str = "@TBD";
-    let mut tag = Self::new_empty();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      if !value.is_empty() {
-        tag = match attr.key {
-          b"dmtype" => {
-            tag.dmtype = value.to_string();
-            tag
-          }
-          b"value" => {
-            tag.value = value.to_string();
-            tag
-          }
-          _ => {
-            return Err(VOTableError::UnexpectedAttr(attr.key.to_vec(), Self::TAG));
-          }
-        }
-      };
-    }
-    if tag.dmtype.as_str() == NULL || tag.value.as_str() == NULL {
-      Err(VOTableError::Custom(format!(
-        "Attributes dmtype value are mandatory in tag {}",
-        Self::TAG
-      )))
-    } else {
-      Ok(tag)
+  type MarkerType = EmptyElem;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new("", "").set_attrs(attrs).and_then(|pk| {
+      if pk.dmtype.is_empty() || pk.value.is_empty() {
+        Err(VOTableError::Custom(format!(
+          "Mandatory attributes 'dmtype' or 'value' not found in tag '{}'",
+          Self::TAG
+        )))
+      } else {
+        Ok(pk)
+      }
+    })
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "dmtype" => self.set_dmtype_by_ref(val),
+        "value" => self.set_value_by_ref(val),
+        _ => return Err(unexpected_attr_err(key, Self::TAG)),
+      }
     }
+    Ok(())
+  }
+
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    f("dmtype", self.dmtype.as_str());
+    f("value", self.value.as_str());
   }
-  empty_read_sub!();
-  impl_write_e!([dmtype, value], []);
 }
 
 #[cfg(test)]
 mod tests {
   use crate::{
     mivot::test::{get_xml, test_error},
     tests::test_read,
```

### Comparing `votable_cli-0.5.0/src/mivot/join/mod.rs` & `votable_cli-0.6.0/src/mivot/join/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -3,36 +3,85 @@
 //! `JOIN` is the same for either `GLOBALS` `COLLECTION`s or `TEMPLATE` `COLLECTION`s.
 
 use std::{
   io::{BufRead, Write},
   str,
 };
 
-use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
-  Reader, Writer,
-};
+use quick_xml::{events::Event, Reader, Writer};
 
 use crate::{
   error::VOTableError,
   mivot::VodmlVisitor,
-  utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite,
+  utils::{discard_comment, discard_event, is_empty, unexpected_attr_err},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, VOTableElement,
 };
 
 pub mod r#where;
 use r#where::Where;
 
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "attr_type")]
 pub enum JoinAttributes {
   DmRef { dmref: String },
   SrcRef { sourceref: String },
   BothRef { dmref: String, sourceref: String },
 }
+impl JoinAttributes {
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    let mut new_dmref = String::new();
+    let mut new_sourceref = String::new();
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "dmref" => new_dmref = val.into(),
+        "sourceref" => new_sourceref = val.into(),
+        _ => return Err(unexpected_attr_err(key, Join::TAG)),
+      }
+    }
+    match self {
+      JoinAttributes::DmRef { dmref } => {
+        *dmref = new_dmref;
+        if new_sourceref.is_empty() {
+          return Err(VOTableError::Custom("Unable to set 'sourceref'".into()));
+        }
+      }
+      JoinAttributes::SrcRef { sourceref } => {
+        *sourceref = new_sourceref;
+        if new_dmref.is_empty() {
+          return Err(VOTableError::Custom("Unable to set 'dmref'".into()));
+        }
+      }
+      JoinAttributes::BothRef { dmref, sourceref } => {
+        *dmref = new_dmref;
+        *sourceref = new_sourceref;
+      }
+    }
+    Ok(())
+  }
+
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    match &self {
+      JoinAttributes::DmRef { dmref } => f("dmtype", dmref.as_str()),
+      JoinAttributes::SrcRef { sourceref } => f("sourceref", sourceref.as_str()),
+      JoinAttributes::BothRef { dmref, sourceref } => {
+        f("dmtype", dmref.as_str());
+        f("sourceref", sourceref.as_str());
+      }
+    }
+  }
+}
 
 /// In`TEMPLATES`, `JOIN` populates a `COLLECTION` with `INSTANCE` elements resulting from the
 /// iteration overs a `TEMPLATES`.
 /// * If at least one `where`, `sourceref` is mandatory because it is a join with another template
 ///   referenced by the sourceref.
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 pub struct Join {
@@ -76,87 +125,103 @@
   }
 
   pub fn push_where_by_ref(&mut self, r#where: Where) {
     self.wheres.push(r#where);
   }
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    visitor.visit_join(self)?;
+    visitor.visit_join_start(self)?;
     for w in self.wheres.iter_mut() {
       w.visit(visitor)?;
     }
-    Ok(())
+    visitor.visit_join_ended(self)
   }
 }
 
-impl QuickXmlReadWrite for Join {
+impl VOTableElement for Join {
   const TAG: &'static str = "JOIN";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
     let mut dmref = String::new();
     let mut sourceref = String::new();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      if !value.is_empty() {
-        match attr.key {
-          b"dmref" => dmref.push_str(value),
-          b"sourceref" => sourceref.push_str(value),
-          _ => return Err(VOTableError::UnexpectedAttr(attr.key.to_vec(), Self::TAG)),
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      let val = val.as_ref();
+      if !val.is_empty() {
+        match key {
+          "dmref" => dmref.push_str(val),
+          "sourceref" => sourceref.push_str(val),
+          _ => return Err(unexpected_attr_err(key, Self::TAG)),
         }
       }
     }
     match (dmref.is_empty(), sourceref.is_empty()) {
       (false, false) => Ok(Self::from_both_ref(dmref, sourceref)),
       (false, true) => Ok(Self::from_dmref(dmref)),
       (true, false) => Ok(Self::from_sourceref(sourceref)),
       (true, true) => Err(VOTableError::Custom(format!(
         "One of the attribute 'dmref' or 'sourceref' mandatory in {}.",
         Self::TAG
       ))),
     }
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    self.attr.set_attrs_by_ref(attrs)
+  }
+
+  fn for_each_attribute<F>(&self, f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    self.attr.for_each_attribute(f)
+  }
+}
+
+impl HasSubElements for Join {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    self.wheres.is_empty()
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
           Where::TAG_BYTES => {
-            self
-              .wheres
-              .push(from_event_start_by_ref!(Where, reader, reader_buff, e))
+            self.push_where_by_ref(from_event_start_by_ref!(Where, reader, reader_buff, e))
           }
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
-          Where::TAG_BYTES => self.wheres.push(Where::from_event_empty(e)?),
+          Where::TAG_BYTES => self.push_where_by_ref(Where::from_event_empty(e)?),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
@@ -167,38 +232,21 @@
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    match &self.attr {
-      JoinAttributes::DmRef { dmref } => tag.push_attribute(("dmtype", dmref.as_str())),
-      JoinAttributes::SrcRef { sourceref } => tag.push_attribute(("sourceref", sourceref.as_str())),
-      JoinAttributes::BothRef { dmref, sourceref } => {
-        tag.push_attribute(("dmtype", dmref.as_str()));
-        tag.push_attribute(("sourceref", sourceref.as_str()));
-      }
-    }
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elements
     write_elem_vec!(self, wheres, writer, context);
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    Ok(())
   }
 }
 
 #[cfg(test)]
 mod tests {
   use crate::{mivot::test::get_xml, tests::test_read};
```

### Comparing `votable_cli-0.5.0/src/mivot/join/where.rs` & `votable_cli-0.6.0/src/mivot/join/where.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,90 @@
 //! Defines the `WHERE` **child of** `JOIN`.
 
 use std::str;
 
-use bstringify::bstringify;
-
 use paste::paste;
 
-use quick_xml::{events::attributes::Attributes, Reader, Writer};
-
 use crate::{
-  error::VOTableError,
-  mivot::{value_checker, VodmlVisitor},
-  QuickXmlReadWrite,
+  error::VOTableError, mivot::VodmlVisitor, utils::unexpected_attr_err, EmptyElem, VOTableElement,
 };
 
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 /// The `WHERE` when it is a **child of** `JOIN`.
 pub struct Where {
+  #[serde(rename = "foreignkey")]
   pub foreign_key: String,
+  #[serde(rename = "primarykey")]
   pub primary_key: String,
 }
 
 impl Where {
-  impl_new!([primary_key, foreign_key], []);
-  impl_empty_new!([primary_key, foreign_key], []);
+  pub fn new<S: Into<String>>(foreign_key: S, primary_key: S) -> Self {
+    Self {
+      foreign_key: foreign_key.into(),
+      primary_key: primary_key.into(),
+    }
+  }
+
+  impl_builder_mandatory_string_attr!(foreign_key, foreignkey);
+  impl_builder_mandatory_string_attr!(primary_key, primarykey);
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
     visitor.visit_where_childof_join(self)
   }
 }
 
-impl_quickrw_e!(
-  [primary_key, "primarykey", foreign_key, "foreignkey"],
-  [],
-  "WHERE",
-  Where,
-  ()
-);
+impl VOTableElement for Where {
+  const TAG: &'static str = "WHERE";
+
+  type MarkerType = EmptyElem;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new("", "").set_attrs(attrs).and_then(|w| {
+      if w.foreign_key.is_empty() || w.primary_key.is_empty() {
+        Err(VOTableError::Custom(format!(
+          "Mandatory attribute 'foreignkey' and/or 'primarykey' not found in tag '{}'",
+          Self::TAG
+        )))
+      } else {
+        Ok(w)
+      }
+    })
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "foreignkey" => self.set_foreignkey_by_ref(val),
+        "primarykey" => self.set_primarykey_by_ref(val),
+        _ => return Err(unexpected_attr_err(key, Self::TAG)),
+      }
+    }
+    Ok(())
+  }
+
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    f("foreignkey", self.foreign_key.as_str());
+    f("primarykey", self.primary_key.as_str());
+  }
+}
 
 #[cfg(test)]
 mod tests {
   use crate::{
     mivot::test::{get_xml, test_error},
     tests::test_read,
   };
```

### Comparing `votable_cli-0.5.0/src/mivot/report.rs` & `votable_cli-0.6.0/src/mivot/report.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 //! Module dedicated to the `REPORT` tag.
 
 use std::str::{self, FromStr};
 
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesText, Event},
-  Reader, Writer,
-};
 
 use crate::{
-  error::VOTableError,
-  mivot::VodmlVisitor,
-  utils::{discard_comment, discard_event},
-  QuickXmlReadWrite,
+  error::VOTableError, mivot::VodmlVisitor, utils::unexpected_attr_err, HasContent, HasContentElem,
+  VOTableElement,
 };
 
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 pub enum Status {
   OK,
   FAILED,
 }
@@ -59,65 +53,70 @@
   pub fn new(status: Status) -> Self {
     Report {
       status,
       content: None,
     }
   }
 
+  impl_builder_mandatory_attr!(status, Status);
   impl_builder_opt_string_attr!(content);
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
     visitor.visit_report(self)
   }
 }
+impl_has_content!(Report);
 
-impl QuickXmlReadWrite for Report {
+impl VOTableElement for Report {
   const TAG: &'static str = "REPORT";
-  type Context = ();
 
-  fn from_attributes(mut attrs: Attributes) -> Result<Self, VOTableError> {
-    if let Some(attr_res) = attrs.next() {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let value = std::str::from_utf8(attr.value.as_ref()).map_err(VOTableError::Utf8)?;
-      return match attr.key {
-        b"status" => Status::from_str(value)
-          .map(Report::new)
-          .map_err(VOTableError::Custom),
-        _ => Err(VOTableError::UnexpectedAttr(attr.key.to_vec(), Self::TAG)),
-      };
-    }
-    Err(VOTableError::Custom(format!(
-      "Attribute 'status' is mandatory in tag '{}'",
-      Self::TAG
-    )))
-  }
-
-  fn read_sub_elements<R: std::io::BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    // I dot not like the fact that we first create an empty String that we replace here... :o/
-    read_content!(Self, self, reader, reader_buff)
-  }
-
-  fn read_sub_elements_by_ref<R: std::io::BufRead>(
-    &mut self,
-    reader: &mut Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    read_content_by_ref!(Self, self, reader, reader_buff)
-  }
-
-  fn write<W: std::io::Write>(
-    &mut self,
-    writer: &mut Writer<W>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    let mut elem_writer = writer.create_element(Self::TAG_BYTES);
-    elem_writer = elem_writer.with_attribute(("status", self.status.to_string().as_str()));
-    write_content!(self, elem_writer);
+  type MarkerType = HasContentElem;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    let mut status: Option<Status> = None;
+    // Look for attributes (especially mandatory attributes)
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "status" => status = Some(val.as_ref().parse().map_err(VOTableError::Custom)?),
+        _ => return Err(unexpected_attr_err(key, Self::TAG)),
+      }
+    }
+    // Set from found attributes
+    if let Some(status) = status {
+      Ok(Self::new(status))
+    } else {
+      Err(VOTableError::Custom(format!(
+        "Attributes 'status' is mandatory in tag '{}'",
+        Self::TAG
+      )))
+    }
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "status" => self.set_status_by_ref(val.as_ref().parse().map_err(VOTableError::Custom)?),
+        _ => return Err(unexpected_attr_err(key, Self::TAG)),
+      }
+    }
     Ok(())
   }
+
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    f("status", self.status.to_string().as_str());
+  }
 }
```

### Comparing `votable_cli-0.5.0/src/mivot/templates/instance/collection/collection.rs` & `votable_cli-0.6.0/src/mivot/globals/instance/collection/collection.rs`

 * *Files 9% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 use std::{
   io::{BufRead, Write},
   str,
 };
 
 use paste::paste;
 use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
+  events::{attributes::Attributes, Event},
   Reader, Writer,
 };
 
 use crate::{
   error::VOTableError,
   mivot::{
-    attribute::AttributeChildOfCollection as Attribute, join::Join, templates::instance::Instance,
+    attribute::AttributeChildOfCollection as Attribute,
+    globals::{collection::reference::Reference, instance::Instance}, // No dmrole
+    join::Join,
     VodmlVisitor,
   },
-  utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite,
+  utils::{discard_comment, discard_event, is_empty, unexpected_attr_err},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, VOTableElement,
 };
 
-use super::reference::Reference;
-
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "elem_type")]
 pub enum InstanceOrRef {
   Instance(Instance),
   /// Reference here is **child of** `COLLECTION` in `GLOBALS`
   Reference(Reference),
 }
@@ -46,14 +46,15 @@
       InstanceOrRef::Reference(elem) => elem.visit(visitor),
     }
   }
 }
 
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "elem_type", content = "content")]
+// #[serde(untagged)]
 pub enum CollectionElems {
   Attribute(Vec<Attribute>),
   Collection(Vec<Collection>),
   InstanceOrRef(Vec<InstanceOrRef>),
   Join(Join),
 }
 
@@ -248,28 +249,28 @@
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Text(e) if is_empty(e) => {}
         Event::End(e) if e.local_name() == Self::TAG_BYTES => {
-          return match (((!attr_vec.is_empty()) as u8) << 4)
+          return match (((!attr_vec.is_empty()) as u8) << 3)
             + (((!col_vec.is_empty()) as u8) << 2)
             + (((!inst_or_ref_vec.is_empty()) as u8) << 1)
             + ((!join_vec.is_empty()) as u8)
           {
             8 => Self::from_attribute(attr_vec),
             4 => Self::from_collections(col_vec),
             2 => Self::from_instance_or_reference_elems(inst_or_ref_vec),
             1 if join_vec.len() == 1 => Self::from_join(join_vec.drain(..).next().unwrap()),
             1 => Err(VOTableError::Custom(
               "A collection cannot have more than one join".to_owned(),
             )),
             0 => Err(VOTableError::Custom(
-              "In COLLECTION child of COLLECTION in TEMPLATES: must have at least one item"
+              "In COLLECTION child of COLLECTION in GLOBALS: must have at least one item"
                 .to_owned(),
             )),
             _ => Err(VOTableError::Custom(
               "A collection cannot have items of different types".to_owned(),
             )),
           } // Set dmid if any
           .map(|c| {
@@ -284,65 +285,84 @@
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    visitor.visit_collection_childof_collection_in_templates(self)?;
-    self.elems.visit(visitor)
+    visitor
+      .visit_collection_childof_collection_in_globals_start(self)
+      .and_then(|()| self.elems.visit(visitor))
+      .and_then(|()| visitor.visit_collection_childof_collection_in_globals_ended(self))
   }
 }
 
-impl QuickXmlReadWrite for Collection {
+impl VOTableElement for Collection {
   const TAG: &'static str = "COLLECTION";
-  type Context = ();
 
-  fn from_attributes(_attrs: Attributes) -> Result<Self, VOTableError> {
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(_attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
     Err(VOTableError::Custom(format!(
       "Tag {} cannot be built directly from attributes",
       Self::TAG
     )))
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "dmid" => self.set_dmid_by_ref(val),
+        _ => return Err(unexpected_attr_err(key, Self::TAG)),
+      }
+    }
+    Ok(())
+  }
+
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    if let Some(dmid) = &self.dmid {
+      f("dmid", dmid.as_str());
+    }
+  }
+}
+
+impl HasSubElements for Collection {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    false
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
-    mut _reader: &mut Reader<R>,
-    mut _reader_buff: &mut Vec<u8>,
+    _reader: &mut Reader<R>,
+    _reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     Err(VOTableError::Custom(format!(
       "Tag {} cannot be built before reading sub-elements",
       Self::TAG
     )))
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    push2write_opt_string_attr!(self, tag, dmid);
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elements
-    self.elems.write(writer)?;
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    self.elems.write(writer)
   }
 }
```

### Comparing `votable_cli-0.5.0/src/mivot/templates/instance/collection/mod.rs` & `votable_cli-0.6.0/src/mivot/templates/instance/collection/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 use std::{
   io::{BufRead, Write},
   str,
 };
 
 use paste::paste;
 use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
+  events::{attributes::Attributes, Event},
   Reader, Writer,
 };
 
 use crate::{
   error::VOTableError,
   mivot::{
     attribute::AttributeChildOfCollection as Attribute, join::Join, templates::instance::Instance,
     VodmlVisitor,
   },
-  utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite,
+  utils::{discard_comment, discard_event, is_empty, unexpected_attr_err},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, VOTableElement,
 };
 
 pub mod collection;
 use collection::{Collection as CollectionChildOfCollection, CollectionElems, InstanceOrRef};
 pub mod reference;
 use reference::Reference;
 
@@ -137,14 +137,15 @@
         dmrole,
         dmid: None,
         elems: CollectionElems::Join(join),
       })
     }
   }
 
+  impl_builder_mandatory_string_attr!(dmrole);
   impl_builder_opt_string_attr!(dmid);
 
   pub(crate) fn get_dmrole_opt_dmid_from_atttributes(
     attrs: Attributes,
   ) -> Result<(String, Option<String>), VOTableError> {
     let mut dmrole = String::new();
     let mut dmid: Option<String> = None;
@@ -258,66 +259,86 @@
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    visitor.visit_collection_childof_instance_in_templates(self)?;
-    self.elems.visit(visitor)
+    visitor
+      .visit_collection_childof_instance_in_templates_start(self)
+      .and_then(|()| self.elems.visit(visitor))
+      .and_then(|()| visitor.visit_collection_childof_instance_in_templates_ended(self))
   }
 }
 
-impl QuickXmlReadWrite for Collection {
+impl VOTableElement for Collection {
   const TAG: &'static str = "COLLECTION";
-  type Context = ();
 
-  fn from_attributes(_attrs: Attributes) -> Result<Self, VOTableError> {
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(_attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
     Err(VOTableError::Custom(format!(
       "Tag {} cannot be built directly from attributes",
       Self::TAG
     )))
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "dmrole" => self.set_dmrole_by_ref(val),
+        "dmid" => self.set_dmid_by_ref(val),
+        _ => return Err(unexpected_attr_err(key, Self::TAG)),
+      }
+    }
+    Ok(())
+  }
+
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    f("dmrole", self.dmrole.as_str());
+    if let Some(dmid) = &self.dmid {
+      f("dmid", dmid.as_str());
+    }
+  }
+}
+
+impl HasSubElements for Collection {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    false
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
-    mut _reader: &mut Reader<R>,
-    mut _reader_buff: &mut Vec<u8>,
+    _reader: &mut Reader<R>,
+    _reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     Err(VOTableError::Custom(format!(
       "Tag {} cannot be built before reading sub-elements",
       Self::TAG
     )))
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    tag.push_attribute(("dmrole", self.dmrole.as_str()));
-    push2write_opt_string_attr!(self, tag, dmid);
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elements
-    self.elems.write(writer)?;
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    self.elems.write(writer)
   }
 }
```

### Comparing `votable_cli-0.5.0/src/mivot/templates/instance/collection/reference.rs` & `votable_cli-0.6.0/src/mivot/templates/instance/collection/reference.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 use std::{
   io::{BufRead, Write},
   str,
 };
 
-use bstringify::bstringify;
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
-  Reader, Writer,
-};
+use quick_xml::{events::Event, Reader, Writer};
 
 use crate::{
   error::VOTableError,
   mivot::{
     globals::collection::reference::Reference as ReferenceStatic,
-    templates::instance::reference::foreign_key::ForeignKey, value_checker, VodmlVisitor,
+    templates::instance::reference::foreign_key::ForeignKey, VodmlVisitor,
   },
-  utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite,
+  utils::{discard_comment, discard_event, is_empty, unexpected_attr_err},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, SpecialElem, VOTableElement,
 };
 
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "elem_type")]
 pub enum Reference {
   Static(ReferenceStatic),
   Dynamic(ReferenceDyn),
@@ -32,67 +28,87 @@
     match self {
       Reference::Static(r) => r.visit(visitor),
       Reference::Dynamic(r) => r.visit(visitor),
     }
   }
 }
 
-impl QuickXmlReadWrite for Reference {
+impl VOTableElement for Reference {
   const TAG: &'static str = "REFERENCE";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
+  type MarkerType = SpecialElem;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
     let mut dmref = String::new();
     let mut sourceref = String::new();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      if !value.is_empty() {
-        match attr.key {
-          b"dmref" => dmref.push_str(value),
-          b"sourceref" => sourceref.push_str(value),
-          _ => return Err(VOTableError::UnexpectedAttr(attr.key.to_vec(), Self::TAG)),
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      let val = val.as_ref();
+      if !val.is_empty() {
+        match key {
+          "dmref" => dmref.push_str(val),
+          "sourceref" => sourceref.push_str(val),
+          _ => return Err(unexpected_attr_err(key, Self::TAG)),
         }
       }
     }
     match (dmref.as_str(), sourceref.as_str()) {
       (dmref, "") => Ok(Reference::Static(ReferenceStatic::new(dmref))),
       ("", sourceref) => Ok(Reference::Dynamic(ReferenceDyn::new(sourceref))),
       _ =>
         Err(VOTableError::Custom(format!(
-          "Either attribute 'dmref' or 'sourceref', not both, are accepted in tag '{}' child of COLLECTIOn",
+          "Either attribute 'dmref' or 'sourceref', not both, are accepted in tag '{}' child of COLLECTION",
           Self::TAG
         ))),
     }
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    match self {
+      Reference::Static(e) => e.set_attrs_by_ref(attrs),
+      Reference::Dynamic(e) => e.set_attrs_by_ref(attrs),
+    }
   }
 
-  fn read_sub_elements_by_ref<R: BufRead>(
+  fn for_each_attribute<F>(&self, f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    match self {
+      Reference::Static(e) => e.for_each_attribute(f),
+      Reference::Dynamic(e) => e.for_each_attribute(f),
+    }
+  }
+}
+
+impl QuickXmlReadWrite<SpecialElem> for Reference {
+  type Context = ();
+
+  fn read_content_by_ref<R: BufRead>(
     &mut self,
     reader: &mut Reader<R>,
     reader_buff: &mut Vec<u8>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
     match self {
       Reference::Static(static_ref_mut) => {
-        static_ref_mut.read_sub_elements_by_ref(reader, reader_buff, context)
+        static_ref_mut.read_content_by_ref(reader, reader_buff, context)
       }
       Reference::Dynamic(dyn_ref_mut) => {
-        dyn_ref_mut.read_sub_elements_by_ref(reader, reader_buff, context)
+        dyn_ref_mut.read_content_by_ref(reader, reader_buff, context)
       }
     }
   }
 
   fn write<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
@@ -100,52 +116,96 @@
   ) -> Result<(), VOTableError> {
     match self {
       Reference::Static(static_ref) => static_ref.write(writer, context),
       Reference::Dynamic(dyn_ref) => dyn_ref.write(writer, context),
     }
   }
 }
+
 /// Dynamic `REFERENCE` **child of** `COLLECTION` in `TEMPLATES`.
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 pub struct ReferenceDyn {
   /// Reference to the `dmid` of the `COLLECTION` or `TEMPLATES` to be searches.
   pub sourceref: String,
   #[serde(skip_serializing_if = "Vec::is_empty")]
   pub foreignkeys: Vec<ForeignKey>, // TODO: ensure contains a least one FK!
 }
 impl ReferenceDyn {
-  impl_new!([sourceref], [], [foreignkeys]);
-  impl_empty_new!([sourceref], [], [foreignkeys]);
+  pub fn new<S: Into<String>>(sourceref: S) -> Self {
+    Self {
+      sourceref: sourceref.into(),
+      foreignkeys: Default::default(),
+    }
+  }
+
+  impl_builder_mandatory_string_attr!(sourceref);
 
   impl_builder_push!(ForeignKey);
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    visitor.visit_reference_dynamic_childof_collection_in_templates(self)?;
+    visitor.visit_reference_dynamic_childof_collection_in_templates_start(self)?;
     for fk in self.foreignkeys.iter_mut() {
       fk.visit(visitor)?;
     }
-    Ok(())
+    visitor.visit_reference_dynamic_childof_collection_in_templates_ended(self)
   }
 }
 
-impl QuickXmlReadWrite for ReferenceDyn {
+impl VOTableElement for ReferenceDyn {
   const TAG: &'static str = "REFERENCE";
-  type Context = ();
 
-  impl_builder_from_attr!([sourceref], []);
+  type MarkerType = HasSubElems;
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new("").set_attrs(attrs).and_then(|reference| {
+      if reference.sourceref.is_empty() {
+        Err(VOTableError::Custom(format!(
+          "Attribute 'sourceref' is' mandatory and must be non-empty in tag '{}'",
+          Self::TAG
+        )))
+      } else {
+        Ok(reference)
+      }
+    })
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "sourceref" => self.set_sourceref_by_ref(val),
+        _ => return Err(unexpected_attr_err(key, Self::TAG)),
+      }
+    }
+    Ok(())
+  }
+
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    f("sourceref", self.sourceref.as_str());
+  }
+}
+
+impl HasSubElements for ReferenceDyn {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    self.foreignkeys.is_empty()
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     reader: &mut Reader<R>,
     reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
@@ -181,33 +241,16 @@
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    if self.foreignkeys.is_empty() {
-      let mut elem_writer = writer.create_element(Self::TAG_BYTES);
-      elem_writer = elem_writer.with_attribute(("sourceref", self.sourceref.as_str()));
-      elem_writer.write_empty().map_err(VOTableError::Write)?;
-      Ok(())
-    } else {
-      let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-      // Write tag + attributes
-      tag.push_attribute(("sourceref", self.sourceref.as_str()));
-      writer
-        .write_event(Event::Start(tag.to_borrowed()))
-        .map_err(VOTableError::Write)?;
-      // Write sub-elems
-      write_elem_vec!(self, foreignkeys, writer, context);
-      // Close tag
-      writer
-        .write_event(Event::End(tag.to_end()))
-        .map_err(VOTableError::Write)
-    }
+    write_elem_vec!(self, foreignkeys, writer, context);
+    Ok(())
   }
 }
```

### Comparing `votable_cli-0.5.0/src/mivot/templates/instance/instance.rs` & `votable_cli-0.6.0/src/mivot/templates/instance/mod.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,202 +1,226 @@
-//! Here `INSTANCE` is a **child of** `INSTANCE`.
-//! Hence, it **must have** `dmrole`.
+//! Here `INSTANCE` is a **child of** `TEMPLATES`.
+//! Hence, it has **no** `dmrole`.
 
 use std::{
   io::{BufRead, Write},
   str,
 };
 
+use log::debug;
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
-  Reader, Writer,
-};
+use quick_xml::{events::Event, Reader, Writer};
 
 use crate::{
   error::VOTableError,
   mivot::{attribute::AttributeChildOfInstance as Attribute, VodmlVisitor},
-  utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite,
+  utils::{is_empty, unexpected_attr_err},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, VOTableElement,
 };
 
-use super::{collection::Collection, primary_key::PrimaryKey, reference::Reference, InstanceElem};
+pub mod collection;
+use collection::Collection;
+pub mod instance;
+use instance::Instance as InstanceChildOfInstance;
+pub mod primary_key;
+use primary_key::PrimaryKeyDyn as PrimaryKey;
+pub mod reference;
+use reference::Reference;
+
+#[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
+#[serde(tag = "elem_type")]
+pub enum InstanceElem {
+  Attribute(Attribute),
+  Instance(InstanceChildOfInstance),
+  Reference(Reference),
+  Collection(Collection),
+}
+impl InstanceElem {
+  fn write<W: Write>(&mut self, writer: &mut Writer<W>) -> Result<(), VOTableError> {
+    match self {
+      InstanceElem::Attribute(elem) => elem.write(writer, &()),
+      InstanceElem::Instance(elem) => elem.write(writer, &()),
+      InstanceElem::Reference(elem) => elem.write(writer, &()),
+      InstanceElem::Collection(elem) => elem.write(writer, &()),
+    }
+  }
+
+  pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
+    match self {
+      InstanceElem::Attribute(elem) => elem.visit(visitor),
+      InstanceElem::Instance(elem) => elem.visit(visitor),
+      InstanceElem::Reference(elem) => elem.visit(visitor),
+      InstanceElem::Collection(elem) => elem.visit(visitor),
+    }
+  }
+}
 
-/// The same as `INSTANCE` **child of** `GLOBALS`, but with having a `dmrole`.
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 pub struct Instance {
   #[serde(skip_serializing_if = "Option::is_none")]
   pub dmid: Option<String>,
-  pub dmrole: String,
   pub dmtype: String,
   #[serde(skip_serializing_if = "Vec::is_empty")]
   pub primarykeys: Vec<PrimaryKey>,
   #[serde(skip_serializing_if = "Vec::is_empty")]
   pub elems: Vec<InstanceElem>,
 }
 
 impl Instance {
-  impl_new!([dmrole, dmtype], [dmid], [primarykeys, elems]);
+  pub fn new<S: Into<String>>(dmtype: S) -> Self {
+    Self {
+      dmid: None,
+      dmtype: dmtype.into(),
+      primarykeys: Default::default(),
+      elems: Default::default(),
+    }
+  }
 
   impl_builder_opt_string_attr!(dmid);
+  impl_builder_mandatory_string_attr!(dmtype);
 
   impl_builder_push!(PrimaryKey);
 
   impl_builder_push_elem!(Attribute, InstanceElem);
-  impl_builder_push_elem!(Instance, InstanceElem);
+  impl_builder_push_elem!(Instance, InstanceElem, InstanceChildOfInstance);
   impl_builder_push_elem!(Reference, InstanceElem);
   impl_builder_push_elem!(Collection, InstanceElem);
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    visitor.visit_instance_childof_instance_in_templates(self)?;
+    visitor.visit_instance_childof_templates_start(self)?;
     for pk in self.primarykeys.iter_mut() {
       pk.visit(visitor)?;
     }
     for elem in self.elems.iter_mut() {
       elem.visit(visitor)?;
     }
-    Ok(())
+    visitor.visit_instance_childof_templates_ended(self)
   }
 }
 
-impl QuickXmlReadWrite for Instance {
+impl VOTableElement for Instance {
   const TAG: &'static str = "INSTANCE";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut dmid = String::new();
-    let mut dmrole = String::new();
-    let mut dmtype = String::new();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      if !value.is_empty() {
-        match attr.key {
-          b"dmid" => dmid.push_str(value),
-          b"dmrole" => dmrole.push_str(value),
-          b"dmtype" => dmtype.push_str(value),
-          _ => {
-            return Err(VOTableError::UnexpectedAttr(
-              attr.key.to_vec(),
-              "INSTANCE child of INSTANCE child of TEMPLATES",
-            ))
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new("").set_attrs(attrs).and_then(|instance| {
+      if instance.dmtype.is_empty() {
+        Err(VOTableError::Custom(format!(
+          "Attribute 'dmtype' is mandatory and must be non-empty in tag '{}' child of TEMPLATES",
+          Self::TAG
+        )))
+      } else {
+        Ok(instance)
+      }
+    })
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "dmid" => self.set_dmid_by_ref(val),
+        "dmtype" => self.set_dmtype_by_ref(val),
+        _ => {
+          if !val.as_ref().is_empty() {
+            return Err(unexpected_attr_err(key, "INSTANCE child of TEMPLATES"));
           }
         }
       }
     }
-    if dmtype.is_empty() || dmrole.is_empty() {
-      Err(VOTableError::Custom(format!(
-        "Attributes 'dmtype' and 'dmrole' are mandatory and must be non-empty in tag '{}' child of `INSTANCE`",
-        Self::TAG
-      )))
-    } else {
-      let mut elem = Self::new(dmrole, dmtype);
-      if !dmid.is_empty() {
-        elem = elem.set_dmid(dmid);
-      }
-      Ok(elem)
+    Ok(())
+  }
+
+  /// Calls a closure on each (key, value) attribute pairs.
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    if let Some(dmid) = &self.dmid {
+      f("dmid", dmid.as_str());
     }
+    f("dmtype", self.dmtype.as_str());
   }
+}
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+impl HasSubElements for Instance {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    false
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
+    context: &Self::Context,
   ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          Instance::TAG_BYTES => self
-            .elems
-            .push(InstanceElem::Instance(from_event_start_by_ref!(
-              Instance,
-              reader,
-              reader_buff,
-              e
-            ))),
+          InstanceChildOfInstance::TAG_BYTES => self.push_instance_by_ref(
+            from_event_start_by_ref!(InstanceChildOfInstance, reader, reader_buff, e),
+          ),
           Reference::TAG_BYTES => {
-            self
-              .elems
-              .push(InstanceElem::Reference(from_event_start_by_ref!(
-                Reference,
-                reader,
-                reader_buff,
-                e
-              )))
+            self.push_reference_by_ref(from_event_start_by_ref!(Reference, reader, reader_buff, e))
           }
           Collection::TAG_BYTES => {
-            self
-              .elems
-              .push(InstanceElem::Collection(from_event_start_by_ref!(
-                Collection,
-                reader,
-                reader_buff,
-                e
-              )))
+            let (dmrole, dmid_opt) =
+              Collection::get_dmrole_opt_dmid_from_atttributes(e.attributes())?;
+            let collection = Collection::from_dmrole_and_reading_sub_elems(
+              dmrole,
+              dmid_opt,
+              context,
+              reader,
+              reader_buff,
+            )?;
+            self.push_collection_by_ref(collection)
           }
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
-          PrimaryKey::TAG_BYTES => self.primarykeys.push(PrimaryKey::from_event_empty(e)?),
-          Attribute::TAG_BYTES => self
-            .elems
-            .push(InstanceElem::Attribute(Attribute::from_event_empty(e)?)),
-          Reference::TAG_BYTES => self
-            .elems
-            .push(InstanceElem::Reference(Reference::from_event_empty(e)?)),
+          PrimaryKey::TAG_BYTES => self.push_primarykey_by_ref(PrimaryKey::from_event_empty(e)?),
+          Attribute::TAG_BYTES => self.push_attribute_by_ref(Attribute::from_event_empty(e)?),
+          Reference::TAG_BYTES => self.push_reference_by_ref(Reference::from_event_empty(e)?),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Text(e) if is_empty(e) => {}
         Event::End(e) if e.local_name() == Self::TAG_BYTES => return Ok(()),
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
-        Event::Comment(e) => discard_comment(e, reader, Self::TAG),
-        _ => discard_event(event, Self::TAG),
+        _ => debug!("Discarded event in {}: {:?}", Self::TAG, event),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    push2write_opt_string_attr!(self, tag, dmid);
-    tag.push_attribute(("dmrole", self.dmrole.as_str()));
-    tag.push_attribute(("dmtype", self.dmtype.as_str()));
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elements
     write_elem_vec!(self, primarykeys, writer, context);
     write_elem_vec_no_context!(self, elems, writer);
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    Ok(())
   }
 }
```

### Comparing `votable_cli-0.5.0/src/mivot/templates/instance/mod.rs` & `votable_cli-0.6.0/src/mivot/templates/instance/reference/mod.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,236 +1,268 @@
-//! Here `INSTANCE` is a **child of** `TEMPLATES`.
-//! Hence, it has **no** `dmrole`.
-
 use std::{
   io::{BufRead, Write},
   str,
 };
 
-use log::debug;
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
-  Reader, Writer,
-};
+use quick_xml::{events::Event, Reader, Writer};
 
 use crate::{
   error::VOTableError,
-  mivot::{attribute::AttributeChildOfInstance as Attribute, VodmlVisitor},
-  utils::is_empty,
-  QuickXmlReadWrite,
+  mivot::{globals::instance::reference::Reference as ReferenceStatic, VodmlVisitor},
+  utils::{discard_comment, discard_event, is_empty, unexpected_attr_err},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, SpecialElem, VOTableElement,
 };
 
-pub mod collection;
-use collection::Collection;
-pub mod instance;
-use instance::Instance as InstanceChildOfInstance;
-pub mod primary_key;
-use primary_key::PrimaryKeyDyn as PrimaryKey;
-pub mod reference;
-use reference::Reference;
+pub mod foreign_key;
+use foreign_key::ForeignKey;
 
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "elem_type")]
-pub enum InstanceElem {
-  Attribute(Attribute),
-  Instance(InstanceChildOfInstance),
-  Reference(Reference),
-  Collection(Collection),
+pub enum Reference {
+  Static(ReferenceStatic),
+  Dynamic(ReferenceDyn),
 }
-impl InstanceElem {
-  fn write<W: Write>(&mut self, writer: &mut Writer<W>) -> Result<(), VOTableError> {
+
+impl Reference {
+  pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
     match self {
-      InstanceElem::Attribute(elem) => elem.write(writer, &()),
-      InstanceElem::Instance(elem) => elem.write(writer, &()),
-      InstanceElem::Reference(elem) => elem.write(writer, &()),
-      InstanceElem::Collection(elem) => elem.write(writer, &()),
+      Reference::Static(r) => r.visit(visitor),
+      Reference::Dynamic(r) => r.visit(visitor),
     }
   }
+}
 
-  pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
+impl VOTableElement for Reference {
+  const TAG: &'static str = "REFERENCE";
+
+  type MarkerType = SpecialElem;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    let mut dmrole = String::new();
+    let mut dmref = String::new();
+    let mut sourceref = String::new();
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      let val = val.as_ref();
+      if !val.is_empty() {
+        match key {
+          "dmrole" => dmrole.push_str(val),
+          "dmref" => dmref.push_str(val),
+          "sourceref" => sourceref.push_str(val),
+          _ => return Err(unexpected_attr_err(key, Self::TAG)),
+        }
+      }
+    }
+    match (dmrole.as_str(), dmref.as_str(), sourceref.as_str()) {
+      ("", _, _) => Err(VOTableError::Custom(format!(
+        "Attribute 'dmrole' is mandatory and must be non-empty in tag '{}' child of INSTANCE",
+        Self::TAG
+      ))),
+      (_, "", "") => Err(VOTableError::Custom(format!(
+        "Either attribute 'dmref' or 'sourceref' is mandatory and must be non-empty in tag '{}' child of INSTANCE",
+        Self::TAG
+      ))),
+      (dmrole, dmref, "") => Ok(Reference::Static(ReferenceStatic::new(dmrole, dmref))),
+      (dmrole, "", sourceref) => Ok(Reference::Dynamic(ReferenceDyn::new(dmrole, sourceref))),
+      _ =>
+        Err(VOTableError::Custom(format!(
+          "Either attribute 'dmref' or 'sourceref', not both, are accepted in tag '{}' child of INSTANCE",
+          Self::TAG
+        ))),
+    }
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
     match self {
-      InstanceElem::Attribute(elem) => elem.visit(visitor),
-      InstanceElem::Instance(elem) => elem.visit(visitor),
-      InstanceElem::Reference(elem) => elem.visit(visitor),
-      InstanceElem::Collection(elem) => elem.visit(visitor),
+      Reference::Static(e) => e.set_attrs_by_ref(attrs),
+      Reference::Dynamic(e) => e.set_attrs_by_ref(attrs),
     }
   }
-}
 
-#[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
-pub struct Instance {
-  #[serde(skip_serializing_if = "Option::is_none")]
-  pub dmid: Option<String>,
-  pub dmtype: String,
-  #[serde(skip_serializing_if = "Vec::is_empty")]
-  pub primarykeys: Vec<PrimaryKey>,
-  #[serde(skip_serializing_if = "Vec::is_empty")]
-  pub elems: Vec<InstanceElem>,
+  fn for_each_attribute<F>(&self, f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    match self {
+      Reference::Static(e) => e.for_each_attribute(f),
+      Reference::Dynamic(e) => e.for_each_attribute(f),
+    }
+  }
 }
 
-impl Instance {
-  impl_new!([dmtype], [dmid], [primarykeys, elems]);
+impl QuickXmlReadWrite<SpecialElem> for Reference {
+  type Context = ();
 
-  impl_builder_opt_string_attr!(dmid);
+  fn read_content_by_ref<R: BufRead>(
+    &mut self,
+    reader: &mut Reader<R>,
+    reader_buff: &mut Vec<u8>,
+    context: &Self::Context,
+  ) -> Result<(), VOTableError> {
+    match self {
+      Reference::Static(e) => e.read_content_by_ref(reader, reader_buff, context),
+      Reference::Dynamic(e) => e.read_content_by_ref(reader, reader_buff, context),
+    }
+  }
 
-  impl_builder_push!(PrimaryKey);
+  fn write<W: Write>(
+    &mut self,
+    writer: &mut Writer<W>,
+    context: &Self::Context,
+  ) -> Result<(), VOTableError> {
+    match self {
+      Reference::Static(e) => e.write(writer, context),
+      Reference::Dynamic(e) => e.write(writer, context),
+    }
+  }
+}
 
-  impl_builder_push_elem!(Attribute, InstanceElem);
-  impl_builder_push_elem!(Instance, InstanceElem, InstanceChildOfInstance);
-  impl_builder_push_elem!(Reference, InstanceElem);
-  impl_builder_push_elem!(Collection, InstanceElem);
+/// Static `REFERENCE` **child of** `INSTANCE` in `TEMPLATES`.
+#[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
+pub struct ReferenceDyn {
+  /// Name of the referenced `INSTANCE` or `COLLECTION` in the data model.
+  pub dmrole: String,
+  /// Reference to the `dmid` of the `COLLECTION` or `TEMPLATES` to be searches.
+  pub sourceref: String,
+  #[serde(skip_serializing_if = "Vec::is_empty")]
+  pub foreignkeys: Vec<ForeignKey>, // TODO: ensure contains a least one FK!
+}
+impl ReferenceDyn {
+  pub fn new<S: Into<String>>(dmrole: S, sourceref: S) -> Self {
+    Self {
+      dmrole: dmrole.into(),
+      sourceref: sourceref.into(),
+      foreignkeys: Default::default(),
+    }
+  }
+
+  impl_builder_mandatory_string_attr!(dmrole);
+  impl_builder_mandatory_string_attr!(sourceref);
+  impl_builder_push!(ForeignKey);
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    visitor.visit_instance_childof_templates(self)?;
-    for pk in self.primarykeys.iter_mut() {
-      pk.visit(visitor)?;
-    }
-    for elem in self.elems.iter_mut() {
-      elem.visit(visitor)?;
+    visitor.visit_reference_dynamic_childof_instance_in_templates_start(self)?;
+    for fk in self.foreignkeys.iter_mut() {
+      fk.visit(visitor)?;
     }
-    Ok(())
+    visitor.visit_reference_dynamic_childof_instance_in_templates_ended(self)
   }
 }
+impl VOTableElement for ReferenceDyn {
+  const TAG: &'static str = "REFERENCE";
 
-impl QuickXmlReadWrite for Instance {
-  const TAG: &'static str = "INSTANCE";
-  type Context = ();
+  type MarkerType = HasSubElems;
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut dmid = String::new();
-    let mut dmtype = String::new();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      if !value.is_empty() {
-        match attr.key {
-          b"dmid" => dmid.push_str(value),
-          b"dmtype" => dmtype.push_str(value),
-          _ => {
-            return Err(VOTableError::UnexpectedAttr(
-              attr.key.to_vec(),
-              "INSTANCE child of TEMPLATES",
-            ))
-          }
-        }
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new("", "").set_attrs(attrs).and_then(|reference| {
+      if reference.dmrole.is_empty() || reference.sourceref.is_empty() {
+        Err(VOTableError::Custom(format!(
+          "Attribute 'dmrole' and 'sourceref' are mandatory and must be non-empty in tag '{}'",
+          Self::TAG
+        )))
+      } else {
+        Ok(reference)
       }
-    }
-    if dmtype.is_empty() {
-      Err(VOTableError::Custom(format!(
-        "Attribute 'dmtype' is mandatory and must be non-empty in tag '{}' child of GLOBALS",
-        Self::TAG
-      )))
-    } else {
-      let mut elem = Self::new(dmtype);
-      if !dmid.is_empty() {
-        elem = elem.set_dmid(dmid);
+    })
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "dmrole" => self.set_dmrole_by_ref(val),
+        "sourceref" => self.set_sourceref_by_ref(val),
+        _ => return Err(unexpected_attr_err(key, Self::TAG)),
       }
-      Ok(elem)
     }
+    Ok(())
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    f("dmrole", self.dmrole.as_str());
+    f("sourceref", self.sourceref.as_str());
+  }
+}
+impl HasSubElements for ReferenceDyn {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    self.foreignkeys.is_empty()
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
-    mut reader: &mut Reader<R>,
-    mut reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
+    reader: &mut Reader<R>,
+    reader_buff: &mut Vec<u8>,
+    _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
-        Event::Start(ref e) => match e.local_name() {
-          InstanceChildOfInstance::TAG_BYTES => {
-            self
-              .elems
-              .push(InstanceElem::Instance(from_event_start_by_ref!(
-                InstanceChildOfInstance,
-                reader,
-                reader_buff,
-                e
-              )))
-          }
-          Reference::TAG_BYTES => {
-            self
-              .elems
-              .push(InstanceElem::Reference(from_event_start_by_ref!(
-                Reference,
-                reader,
-                reader_buff,
-                e
-              )))
-          }
-          Collection::TAG_BYTES => {
-            let (dmrole, dmid_opt) =
-              Collection::get_dmrole_opt_dmid_from_atttributes(e.attributes())?;
-            let collection = Collection::from_dmrole_and_reading_sub_elems(
-              dmrole,
-              dmid_opt,
-              context,
-              reader,
-              reader_buff,
-            )?;
-            self.elems.push(InstanceElem::Collection(collection))
-          }
-          _ => {
-            return Err(VOTableError::UnexpectedStartTag(
-              e.local_name().to_vec(),
-              Self::TAG,
-            ))
-          }
-        },
+        Event::Start(ref e) => {
+          return Err(VOTableError::UnexpectedStartTag(
+            e.local_name().to_vec(),
+            Self::TAG,
+          ))
+        }
         Event::Empty(ref e) => match e.local_name() {
-          PrimaryKey::TAG_BYTES => self.primarykeys.push(PrimaryKey::from_event_empty(e)?),
-          Attribute::TAG_BYTES => self
-            .elems
-            .push(InstanceElem::Attribute(Attribute::from_event_empty(e)?)),
-          Reference::TAG_BYTES => self
-            .elems
-            .push(InstanceElem::Reference(Reference::from_event_empty(e)?)),
+          ForeignKey::TAG_BYTES => self.push_foreignkey_by_ref(ForeignKey::from_event_empty(e)?),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Text(e) if is_empty(e) => {}
-        Event::End(e) if e.local_name() == Self::TAG_BYTES => return Ok(()),
+        Event::End(e) if e.local_name() == Self::TAG_BYTES => {
+          return if self.foreignkeys.is_empty() {
+            Err(VOTableError::Custom(
+              "A Dynamic Reference must have at least one ForeignKey".to_owned(),
+            ))
+          } else {
+            Ok(())
+          }
+        }
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
-        _ => debug!("Discarded event in {}: {:?}", Self::TAG, event),
+        Event::Comment(e) => discard_comment(e, reader, Self::TAG),
+        _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    push2write_opt_string_attr!(self, tag, dmid);
-    tag.push_attribute(("dmtype", self.dmtype.as_str()));
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elements
-    write_elem_vec!(self, primarykeys, writer, context);
-    write_elem_vec_no_context!(self, elems, writer);
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    /*if self.foreignkeys.is_empty(): Err(VOTableError::Custom(
+      "A Dynamic Reference must have at least one ForeignKey".to_owned(),
+    ))*/
+    write_elem_vec!(self, foreignkeys, writer, context);
+    Ok(())
   }
 }
```

### Comparing `votable_cli-0.5.0/src/mivot/templates/instance/reference/mod.rs` & `votable_cli-0.6.0/src/mivot/templates/mod.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,230 +1,216 @@
-use std::{
-  io::{BufRead, Write},
-  str,
-};
+//! Module dedicated to the `TEPLATES` tag.
+//!
+//! The `TEMPLATES` block maps data model instances on the rows of a table in the VOTable.
+
+use std::{io::Write, str};
 
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
-  Reader, Writer,
-};
+use quick_xml::{events::Event, Reader, Writer};
 
 use crate::{
   error::VOTableError,
-  mivot::{globals::instance::reference::Reference as ReferenceStatic, VodmlVisitor},
-  utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite,
+  mivot::VodmlVisitor,
+  utils::{discard_comment, discard_event, is_empty, unexpected_attr_err},
+  HasSubElements, HasSubElems, QuickXmlReadWrite, VOTableElement,
 };
 
-pub mod foreign_key;
-use foreign_key::ForeignKey;
+pub mod instance;
+use instance::Instance;
+pub mod r#where;
+use r#where::Where;
 
+/// Structure storing the content of the `TEMPLATES` tag.
 #[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
-#[serde(tag = "elem_type")]
-pub enum Reference {
-  Static(ReferenceStatic),
-  Dynamic(ReferenceDyn),
+pub struct Templates {
+  #[serde(skip_serializing_if = "Option::is_none")]
+  pub tableref: Option<String>,
+  #[serde(skip_serializing_if = "Vec::is_empty")]
+  pub wheres: Vec<Where>,
+  #[serde(skip_serializing_if = "Vec::is_empty")]
+  pub instances: Vec<Instance>,
 }
-
-impl Reference {
-  pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    match self {
-      Reference::Static(r) => r.visit(visitor),
-      Reference::Dynamic(r) => r.visit(visitor),
+impl Templates {
+  fn new() -> Self {
+    Self {
+      tableref: None,
+      wheres: vec![],
+      instances: vec![],
     }
   }
-}
 
-impl QuickXmlReadWrite for Reference {
-  const TAG: &'static str = "REFERENCE";
-  type Context = ();
-
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut dmrole = String::new();
-    let mut dmref = String::new();
-    let mut sourceref = String::new();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      if !value.is_empty() {
-        match attr.key {
-          b"dmrole" => dmrole.push_str(value),
-          b"dmref" => dmref.push_str(value),
-          b"sourceref" => sourceref.push_str(value),
-          _ => return Err(VOTableError::UnexpectedAttr(attr.key.to_vec(), Self::TAG)),
-        }
-      }
-    }
-    match (dmrole.as_str(), dmref.as_str(), sourceref.as_str()) {
-      ("", _, _) => Err(VOTableError::Custom(format!(
-        "Attribute 'dmrole' is mandatory and must be non-empty in tag '{}' child of INSTANCE",
-        Self::TAG
-      ))),
-      (_, "", "") => Err(VOTableError::Custom(format!(
-        "Either attribute 'dmref' or 'sourceref' is mandatory and must be non-empty in tag '{}' child of INSTANCE",
-        Self::TAG
-      ))),
-      (dmrole, dmref, "") => Ok(Reference::Static(ReferenceStatic::new(dmrole, dmref))),
-      (dmrole, "", sourceref) => Ok(Reference::Dynamic(ReferenceDyn::new(dmrole, sourceref))),
-      _ =>
-        Err(VOTableError::Custom(format!(
-          "Either attribute 'dmref' or 'sourceref', not both, are accepted in tag '{}' child of INSTANCE",
-          Self::TAG
-        ))),
-    }
-  }
+  impl_builder_opt_string_attr!(tableref);
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
+  pub fn push_where(mut self, where_: Where) -> Self {
+    self.push_where_by_ref(where_);
     self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
   }
-
-  fn read_sub_elements_by_ref<R: BufRead>(
-    &mut self,
-    reader: &mut Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    match self {
-      Reference::Static(static_ref_mut) => {
-        static_ref_mut.read_sub_elements_by_ref(reader, reader_buff, context)
-      }
-      Reference::Dynamic(dyn_ref_mut) => {
-        dyn_ref_mut.read_sub_elements_by_ref(reader, reader_buff, context)
-      }
-    }
+  pub fn push_where_by_ref(&mut self, where_: Where) {
+    self.wheres.push(where_);
   }
+  impl_builder_push!(Instance);
 
-  fn write<W: Write>(
-    &mut self,
-    writer: &mut Writer<W>,
-    context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    match self {
-      Reference::Static(static_ref) => static_ref.write(writer, context),
-      Reference::Dynamic(dyn_ref) => dyn_ref.write(writer, context),
-    }
+  pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
+    visitor.visit_templates_start(self)?;
+    for w in self.wheres.iter_mut() {
+      w.visit(visitor)?;
+    }
+    for elem in self.instances.iter_mut() {
+      elem.visit(visitor)?;
+    }
+    visitor.visit_templates_ended(self)
   }
 }
 
-/// Static `REFERENCE` **child of** `INSTANCE` in `TEMPLATES`.
-#[derive(Clone, Debug, PartialEq, Eq, serde::Serialize, serde::Deserialize)]
-pub struct ReferenceDyn {
-  /// Name of the referenced `INSTANCE` or `COLLECTION` in the data model.
-  pub dmrole: String,
-  /// Reference to the `dmid` of the `COLLECTION` or `TEMPLATES` to be searches.
-  pub sourceref: String,
-  #[serde(skip_serializing_if = "Vec::is_empty")]
-  pub foreignkeys: Vec<ForeignKey>, // TODO: ensure contains a least one FK!
-}
-impl ReferenceDyn {
-  impl_new!([dmrole, sourceref], [], [foreignkeys]);
-  impl_builder_push!(ForeignKey);
-
-  pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    visitor.visit_reference_dynamic_childof_instance_in_templates(self)?;
-    for fk in self.foreignkeys.iter_mut() {
-      fk.visit(visitor)?;
+impl VOTableElement for Templates {
+  const TAG: &'static str = "TEMPLATES";
+
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new().set_attrs(attrs)
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "tableref" => {
+          if val.as_ref().is_empty() {
+            return Err(VOTableError::Custom(String::from(
+              "Attribute 'tableref' must not be empty.",
+            )));
+          } else {
+            self.set_tableref_by_ref(val)
+          }
+        }
+        _ => return Err(unexpected_attr_err(key, Self::TAG)),
+      }
     }
     Ok(())
   }
+
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    if let Some(tableref) = &self.tableref {
+      f("tableref", tableref.as_ref());
+    }
+  }
 }
 
-impl QuickXmlReadWrite for ReferenceDyn {
-  const TAG: &'static str = "REFERENCE";
+impl HasSubElements for Templates {
   type Context = ();
 
-  fn from_attributes(_attrs: Attributes) -> Result<Self, VOTableError> {
-    unreachable!("Should not be called directly!")
-  }
-
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, _context)
-      .map(|()| reader)
+  fn has_no_sub_elements(&self) -> bool {
+    // Note: Should always be true to be a valid VODML element
+    self.wheres.is_empty() && self.instances.is_empty()
   }
 
-  fn read_sub_elements_by_ref<R: BufRead>(
+  fn read_sub_elements_by_ref<R: std::io::BufRead>(
     &mut self,
-    reader: &mut Reader<R>,
-    reader_buff: &mut Vec<u8>,
+    mut reader: &mut Reader<R>,
+    mut reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
+  ) -> Result<(), crate::error::VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
-        Event::Start(ref e) => {
-          return Err(VOTableError::UnexpectedStartTag(
-            e.local_name().to_vec(),
-            Self::TAG,
-          ))
-        }
+        Event::Start(ref e) => match e.local_name() {
+          Instance::TAG_BYTES => push_from_event_start!(self, Instance, reader, reader_buff, e),
+          _ => {
+            return Err(VOTableError::UnexpectedStartTag(
+              e.local_name().to_vec(),
+              Templates::TAG,
+            ))
+          }
+        },
         Event::Empty(ref e) => match e.local_name() {
-          ForeignKey::TAG_BYTES => self.push_foreignkey_by_ref(ForeignKey::from_event_empty(e)?),
+          Where::TAG_BYTES => push_from_event_empty!(self, Where, e),
+          Instance::TAG_BYTES => push_from_event_empty!(self, Instance, e),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
-              Self::TAG,
+              Templates::TAG,
             ))
           }
         },
         Event::Text(e) if is_empty(e) => {}
-        Event::End(e) if e.local_name() == Self::TAG_BYTES => {
-          return if self.foreignkeys.is_empty() {
-            Err(VOTableError::Custom(
-              "A Dynamic Reference must have at least one ForeignKey".to_owned(),
-            ))
+        Event::End(e) if e.local_name() == Templates::TAG_BYTES => {
+          if self.instances.is_empty() {
+            return Err(VOTableError::Custom(
+              "At least one instance should be present in a templates tag.".to_owned(),
+            ));
           } else {
-            Ok(())
+            return Ok(());
           }
         }
-        Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
-        Event::Comment(e) => discard_comment(e, reader, Self::TAG),
-        _ => discard_event(event, Self::TAG),
+        Event::Eof => return Err(VOTableError::PrematureEOF(Templates::TAG)),
+        Event::Comment(e) => discard_comment(e, reader, Templates::TAG),
+        _ => discard_event(event, Templates::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    if self.foreignkeys.is_empty() {
-      /*let mut elem_writer = writer.create_element(Self::TAG_BYTES);
-      elem_writer = elem_writer.with_attribute(("dmrole", self.dmrole.as_str()));
-      elem_writer = elem_writer.with_attribute(("sourceref", self.sourceref.as_str()));
-      elem_writer.write_empty().map_err(VOTableError::Write)?;
-      Ok(())*/
-      Err(VOTableError::Custom(
-        "A Dynamic Reference must have at least one ForeignKey".to_owned(),
-      ))
-    } else {
-      let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-      // Write tag + attributes
-      tag.push_attribute(("dmrole", self.dmrole.as_str()));
-      tag.push_attribute(("sourceref", self.sourceref.as_str()));
-      writer
-        .write_event(Event::Start(tag.to_borrowed()))
-        .map_err(VOTableError::Write)?;
-      // Write sub-elems
-      write_elem_vec!(self, foreignkeys, writer, context);
-      // Close tag
-      writer
-        .write_event(Event::End(tag.to_end()))
-        .map_err(VOTableError::Write)
-    }
+    write_elem_vec!(self, wheres, writer, context);
+    write_elem_vec!(self, instances, writer, context);
+    Ok(())
+  }
+}
+
+#[cfg(test)]
+mod tests {
+  use crate::{
+    mivot::templates::Templates,
+    mivot::test::{get_xml, test_error},
+    tests::test_read,
+  };
+
+  #[test]
+  fn test_templates_read() {
+    // OK MODELS
+    let xml = get_xml("./resources/mivot/4/test_4_ok_4.1.xml");
+    println!("testing 4.1");
+    test_read::<Templates>(&xml);
+    let xml = get_xml("./resources/mivot/4/test_4_ok_4.2.xml");
+    println!("testing 4.2");
+    test_read::<Templates>(&xml);
+    let xml = get_xml("./resources/mivot/4/test_4_ok_4.5.xml");
+    println!("testing 4.5");
+    test_read::<Templates>(&xml);
+    let xml = get_xml("./resources/mivot/4/test_4_ok_4.6.xml");
+    println!("testing 4.6");
+    test_read::<Templates>(&xml);
+    let xml = get_xml("./resources/mivot/4/test_4_ok_4.8.xml");
+    println!("testing 4.8");
+    test_read::<Templates>(&xml);
+    // KO MODELS
+    let xml = get_xml("./resources/mivot/4/test_4_ko_4.3.xml");
+    println!("testing 4.3"); // WHERE only; INSTANCE required
+    test_error::<Templates>(&xml, false);
+    let xml = get_xml("./resources/mivot/4/test_4_ko_4.4.xml");
+    println!("testing 4.4"); // Where should be before instance (parser can overlook this and write it correctly later)
+    test_read::<Templates>(&xml); // Should read correctly
+    let xml = get_xml("./resources/mivot/4/test_4_ko_4.7.xml");
+    println!("testing 4.7"); // includes invalid subnode
+    test_error::<Templates>(&xml, false);
+    let xml = get_xml("./resources/mivot/4/test_4_ko_4.9.xml");
+    println!("testing 4.9"); // tableref must not be empty
+    test_error::<Templates>(&xml, true);
   }
 }
```

### Comparing `votable_cli-0.5.0/src/mivot/visitors/donothing.rs` & `votable_cli-0.6.0/src/mivot/visitors/donothing.rs`

 * *Files 23% similar despite different names*

```diff
@@ -11,107 +11,184 @@
 
 impl<E: Error> Default for DoNothing<E> {
   fn default() -> Self {
     Self::new()
   }
 }
 
-
 impl<E: Error> VodmlVisitor for DoNothing<E> {
   type E = E;
 
-  fn visit_vodml(&mut self, _: &mut Vodml) -> Result<(), Self::E> {
+  fn visit_vodml_start(&mut self, _: &mut Vodml) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_vodml_ended(&mut self, _: &mut Vodml) -> Result<(), Self::E> {
     Ok(())
   }
 
   fn visit_report(&mut self, _: &mut Report) -> Result<(), Self::E> {
     Ok(())
   }
 
   fn visit_model(&mut self, _: &mut Model) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_globals(&mut self, _: &mut Globals) -> Result<(), Self::E> {
+  fn visit_globals_start(&mut self, _: &mut Globals) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_globals_ended(&mut self, _: &mut Globals) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_templates(&mut self, _: &mut Templates) -> Result<(), Self::E> {
+  fn visit_templates_start(&mut self, _: &mut Templates) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_templates_ended(&mut self, _: &mut Templates) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_instance_childof_globals(&mut self, _: &mut InstanceGI) -> Result<(), Self::E> {
+  fn visit_instance_childof_globals_start(&mut self, _: &mut InstanceGI) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_instance_childof_globals_ended(&mut self, _: &mut InstanceGI) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_instance_childof_instance_in_globals(
+  fn visit_instance_childof_instance_in_globals_start(
+    &mut self,
+    _: &mut InstanceGII,
+  ) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_instance_childof_instance_in_globals_ended(
     &mut self,
     _: &mut InstanceGII,
   ) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_instance_childof_collection_in_globals(
+  fn visit_instance_childof_collection_in_globals_start(
+    &mut self,
+    _: &mut InstanceGCI,
+  ) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_instance_childof_collection_in_globals_ended(
     &mut self,
     _: &mut InstanceGCI,
   ) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_collection_childof_instance_in_globals(
+  fn visit_collection_childof_instance_in_globals_start(
+    &mut self,
+    _: &mut CollectionGIC,
+  ) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_collection_childof_instance_in_globals_ended(
     &mut self,
     _: &mut CollectionGIC,
   ) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_collection_childof_globals(&mut self, _: &mut CollectionGC) -> Result<(), Self::E> {
+  fn visit_collection_childof_globals_start(
+    &mut self,
+    _: &mut CollectionGC,
+  ) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_collection_childof_globals_ended(
+    &mut self,
+    _: &mut CollectionGC,
+  ) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_collection_childof_collection_in_globals(
+  fn visit_collection_childof_collection_in_globals_start(
+    &mut self,
+    _: &mut CollectionGICC,
+  ) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_collection_childof_collection_in_globals_ended(
     &mut self,
     _: &mut CollectionGICC,
   ) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_instance_childof_templates(&mut self, _: &mut InstanceTI) -> Result<(), Self::E> {
+  fn visit_instance_childof_templates_start(&mut self, _: &mut InstanceTI) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_instance_childof_templates_ended(&mut self, _: &mut InstanceTI) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_instance_childof_instance_in_templates(
+  fn visit_instance_childof_instance_in_templates_start(
+    &mut self,
+    _: &mut InstanceTII,
+  ) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_instance_childof_instance_in_templates_ended(
     &mut self,
     _: &mut InstanceTII,
   ) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_collection_childof_instance_in_templates(
+  fn visit_collection_childof_instance_in_templates_start(
+    &mut self,
+    _: &mut CollectionTIC,
+  ) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_collection_childof_instance_in_templates_ended(
     &mut self,
     _: &mut CollectionTIC,
   ) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_collection_childof_collection_in_templates(
+  fn visit_collection_childof_collection_in_templates_start(
+    &mut self,
+    _: &mut CollectionTICC,
+  ) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_collection_childof_collection_in_templates_ended(
     &mut self,
     _: &mut CollectionTICC,
   ) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_reference_dynamic_childof_instance_in_templates(
+  fn visit_reference_dynamic_childof_instance_in_templates_start(
+    &mut self,
+    _: &mut RefDynTIR,
+  ) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_reference_dynamic_childof_instance_in_templates_ended(
     &mut self,
     _: &mut RefDynTIR,
   ) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_reference_dynamic_childof_collection_in_templates(
+  fn visit_reference_dynamic_childof_collection_in_templates_start(
+    &mut self,
+    _: &mut RefDynTICR,
+  ) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_reference_dynamic_childof_collection_in_templates_ended(
     &mut self,
     _: &mut RefDynTICR,
   ) -> Result<(), Self::E> {
     Ok(())
   }
 
   fn visit_attribute_childof_instance(&mut self, _: &mut AttributeI) -> Result<(), Self::E> {
@@ -138,15 +215,18 @@
     Ok(())
   }
 
   fn visit_foreign_key(&mut self, _: &mut ForeignKey) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_join(&mut self, _: &mut Join) -> Result<(), Self::E> {
+  fn visit_join_start(&mut self, _: &mut Join) -> Result<(), Self::E> {
+    Ok(())
+  }
+  fn visit_join_ended(&mut self, _: &mut Join) -> Result<(), Self::E> {
     Ok(())
   }
 
   fn visit_where_childof_join(&mut self, _: &mut WhereJ) -> Result<(), Self::E> {
     Ok(())
   }
```

### Comparing `votable_cli-0.5.0/src/mivot/vodml.rs` & `votable_cli-0.6.0/src/mivot/vodml.rs`

 * *Files 20% similar despite different names*

```diff
@@ -49,25 +49,23 @@
 //! and [guidline](https://github.com/ivoa/modelinstanceinvot-code/wiki/guideline)
 //!
 //! and the [Meas data model](https://ivoa.net/documents/Meas/20211019/index.html)
 //!
 
 use std::{collections::HashMap, io::Write, str};
 
+use log::warn;
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
-  Reader, Writer,
-};
+use quick_xml::{events::Event, Reader, Writer};
 use serde_json::Value;
 
 use crate::{
   error::VOTableError,
   utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite,
+  HasSubElements, HasSubElems, QuickXmlReadWrite, VOTableElement,
 };
 
 use super::{globals::Globals, model::Model, report::Report, templates::Templates, VodmlVisitor};
 
 /// Structure storing the content of the `VODML` tag.
 #[derive(Clone, Debug, Default, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct Vodml {
@@ -100,133 +98,115 @@
   }
 
   // Attributes
   impl_builder_opt_string_attr!(xmlns);
   // Extra attributes
   impl_builder_insert_extra!();
   // Sub-elements
-  impl_builder_opt_attr!(report, Report);
+  impl_builder_opt_subelem!(report, Report);
   impl_builder_push!(Model);
-  impl_builder_opt_attr!(globals, Globals);
+  impl_builder_opt_subelem!(globals, Globals);
   impl_builder_push_no_s!(Templates);
 
   pub fn visit<V: VodmlVisitor>(&mut self, visitor: &mut V) -> Result<(), V::E> {
-    visitor.visit_vodml(self)?;
+    visitor.visit_vodml_start(self)?;
     if let Some(report) = self.report.as_mut() {
       report.visit(visitor)?;
     }
     for model in self.models.iter_mut() {
       model.visit(visitor)?;
     }
     if let Some(globals) = self.globals.as_mut() {
       globals.visit(visitor)?;
     }
     for template in self.templates.iter_mut() {
       template.visit(visitor)?;
     }
-    Ok(())
+    visitor.visit_vodml_ended(self)
   }
 }
-impl QuickXmlReadWrite for Vodml {
+
+impl VOTableElement for Vodml {
   const TAG: &'static str = "VODML";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, crate::error::VOTableError> {
-    let mut vodml = Self::default();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      vodml = match attr.key {
-        b"xmlns" => vodml.set_xmlns(value),
-        _ => vodml.insert_extra(
-          str::from_utf8(attr.key).map_err(VOTableError::Utf8)?,
-          Value::String(value.into()),
-        ),
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new().set_attrs(attrs)
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "xmlns" => self.set_xmlns_by_ref(val),
+        _ => self.insert_extra_str_by_ref(key, val),
       }
     }
-    Ok(vodml)
+    Ok(())
   }
 
-  fn read_sub_elements<R: std::io::BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
-  ) -> Result<Reader<R>, crate::error::VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, context)
-      .map(|()| reader)
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    if let Some(xmlns) = &self.xmlns {
+      f("xmlns", xmlns.to_string().as_str());
+    }
+    for_each_extra_attribute!(self, f);
+  }
+}
+
+impl HasSubElements for Vodml {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    // Note: Should always be true to be a valid VODML element
+    self.report.is_none()
+      && self.models.is_empty()
+      && self.globals.is_none()
+      && self.extra.is_empty()
   }
 
   fn read_sub_elements_by_ref<R: std::io::BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
-  ) -> Result<(), crate::error::VOTableError> {
+  ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          Report::TAG_BYTES => {
-            if self
-              .report
-              .replace(from_event_start_by_ref!(Report, reader, reader_buff, e))
-              .is_some()
-            {
-              return Err(VOTableError::Custom(
-                "Maximum one <REPORT> tag should be present".to_owned(),
-              ));
-            }
-          }
-          Globals::TAG_BYTES => {
-            if self
-              .globals
-              .replace(from_event_start_by_ref!(Globals, reader, reader_buff, e))
-              .is_some()
-            {
-              return Err(VOTableError::Custom(
-                "Maximum one <GLOBALS> tag should be present".to_owned(),
-              ));
-            }
-          }
-          Templates::TAG_BYTES => {
-            self
-              .templates
-              .push(from_event_start_by_ref!(Templates, reader, reader_buff, e))
-          }
+          Report::TAG_BYTES => set_from_event_start!(self, Report, reader, reader_buff, e),
+          Model::TAG_BYTES => push_from_event_start!(self, Model, reader, reader_buff, e),
+          Globals::TAG_BYTES => set_from_event_start!(self, Globals, reader, reader_buff, e),
+          Templates::TAG_BYTES => push_from_event_start!(self, Templates, reader, reader_buff, e),
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
-          Report::TAG_BYTES => {
-            if self.report.replace(Report::from_event_empty(e)?).is_some() {
-              return Err(VOTableError::Custom(
-                "Maximum one <REPORT> tag should be present".to_owned(),
-              ));
-            }
-          }
-          Model::TAG_BYTES => self.models.push(Model::from_event_empty(e)?),
-          Globals::TAG_BYTES => {
-            if self
-              .globals
-              .replace(Globals::from_event_empty(e)?)
-              .is_some()
-            {
-              return Err(VOTableError::Custom(
-                "Maximum one <GLOBALS> tag should be present".to_owned(),
-              ));
-            }
-          }
-          Templates::TAG_BYTES => self.templates.push(Templates::from_event_empty(e)?),
+          Report::TAG_BYTES => set_from_event_empty!(self, Report, e),
+          Model::TAG_BYTES => push_from_event_empty!(self, Model, e),
+          Globals::TAG_BYTES => set_from_event_empty!(self, Globals, e),
+          Templates::TAG_BYTES => push_from_event_empty!(self, Templates, e),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
@@ -243,32 +223,24 @@
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
-  ) -> Result<(), crate::error::VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    push2write_opt_string_attr!(self, tag, xmlns);
-    push2write_extra!(self, tag);
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
+  ) -> Result<(), VOTableError> {
     write_elem!(self, report, writer, context);
     write_elem_vec!(self, models, writer, context);
     write_elem!(self, globals, writer, context);
     write_elem_vec!(self, templates, writer, context);
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    Ok(())
   }
 }
 
 #[cfg(test)]
 mod tests {
   use crate::{
     mivot::test::test_error,
@@ -306,13 +278,13 @@
     println!("testing 1.6"); // MODEL subnode must be first (parser can overlook this and write it correctly later)
     test_read::<Vodml>(&xml); // Should read correctly
     let xml = get_xml("./resources/mivot/1/test_1_ko_1.7.xml");
     println!("testing 1.7"); // GLOBALS must be after MODEL and before TEMPLATES (parser can overlook this and write it correctly later)
     test_read::<Vodml>(&xml); // Should read correctly
     let xml = get_xml("./resources/mivot/1/test_1_ko_1.10.xml");
     println!("testing 1.10"); // Only 1 GLOBALS subnode allowed.
-    test_error::<Vodml>(&xml, false);
+    test_read::<Vodml>(&xml); // It is OK, since we produce a WARNING
     let xml = get_xml("./resources/mivot/1/test_1_ko_1.11.xml");
     println!("testing 1.11"); // Includes invalid subnode.
     test_error::<Vodml>(&xml, false);
   }
 }
```

### Comparing `votable_cli-0.5.0/src/param.rs` & `votable_cli-0.6.0/src/param.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 //! Struct dedicated to the `PARAM` tag.
 
 use std::{
   io::{BufRead, Write},
   str,
 };
 
-use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
-  Reader, Writer,
-};
-
+use log::warn;
+use paste::paste;
+use quick_xml::{events::Event, Reader, Writer};
 use serde_json::Value;
 
 use super::{
   datatype::Datatype,
   desc::Description,
   error::VOTableError,
   field::{ArraySize, Field, Precision},
   link::Link,
   utils::{discard_comment, discard_event},
   values::Values,
-  QuickXmlReadWrite, TableDataContent, VOTableVisitor,
+  HasSubElements, HasSubElems, QuickXmlReadWrite, TableDataContent, VOTableElement, VOTableVisitor,
 };
 
+/// Struct corresponding to the `PARAM` XML tag.
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct Param {
   #[serde(flatten)]
   pub field: Field,
   pub value: String,
 }
 
@@ -34,71 +33,132 @@
   pub fn new<N: Into<String>, V: Into<String>>(name: N, datatype: Datatype, value: V) -> Self {
     Param {
       field: Field::new(name, datatype),
       value: value.into(),
     }
   }
 
-  // copy/paste + modified from `cargo expand field`
-  // TODO: add _by_ref setters!!
+  // attributes
+  impl_builder_opt_string_attr_delegated!(id, field);
+  impl_builder_mandatory_string_attr_delegated!(name, field);
+  impl_builder_mandatory_attr_delegated!(datatype, Datatype, field);
+  impl_builder_opt_string_attr_delegated!(unit, field);
+  impl_builder_opt_attr_delegated!(precision, Precision, field);
+  impl_builder_opt_attr_delegated!(width, u16, field);
+  impl_builder_opt_string_attr_delegated!(xtype, field);
+  impl_builder_opt_string_attr_delegated!(ref_, ref, field);
+  impl_builder_opt_string_attr_delegated!(ucd, field);
+  impl_builder_opt_string_attr_delegated!(utype, field);
+  impl_builder_opt_attr_delegated!(arraysize, ArraySize, field);
+  impl_builder_mandatory_string_attr!(value);
+  // extra attributes
+  impl_builder_insert_extra_delegated!(field);
+  // sub-elements
+  impl_builder_opt_subelem_delegated!(description, Description, field);
+  impl_builder_opt_subelem_delegated!(values, Values, field);
+  impl_builder_push_delegated!(Link, field);
 
-  pub fn set_id<I: Into<String>>(mut self, id: I) -> Self {
-    self.field.id = Some(id.into());
-    self
-  }
-  pub fn set_unit<I: Into<String>>(mut self, unit: I) -> Self {
-    self.field.unit = Some(unit.into());
-    self
-  }
-  pub fn set_precision(mut self, precision: Precision) -> Self {
-    self.field.precision = Some(precision);
-    self
-  }
-  pub fn set_width(mut self, width: u16) -> Self {
-    self.field.width = Some(width);
-    self
-  }
-  pub fn set_xtype<I: Into<String>>(mut self, xtype: I) -> Self {
-    self.field.xtype = Some(xtype.into());
-    self
-  }
-  pub fn set_ref<I: Into<String>>(mut self, ref_: I) -> Self {
-    self.field.ref_ = Some(ref_.into());
-    self
-  }
-  pub fn set_ucd<I: Into<String>>(mut self, ucd: I) -> Self {
-    self.field.ucd = Some(ucd.into());
-    self
-  }
-  pub fn set_utype<I: Into<String>>(mut self, utype: I) -> Self {
-    self.field.utype = Some(utype.into());
-    self
-  }
-  pub fn set_arraysize(mut self, arraysize: ArraySize) -> Self {
-    self.field.arraysize = Some(arraysize);
-    self
-  }
-  pub fn insert_extra<S: Into<String>>(mut self, key: S, value: Value) -> Self {
-    self.field.extra.insert(key.into(), value);
-    self
-  }
-  pub fn set_description(mut self, description: Description) -> Self {
-    self.field.description = Some(description);
-    self
+  pub fn visit<C, V>(&mut self, visitor: &mut V) -> Result<(), V::E>
+  where
+    C: TableDataContent,
+    V: VOTableVisitor<C>,
+  {
+    visitor.visit_param_start(self)?;
+    if let Some(description) = &mut self.field.description {
+      visitor.visit_description(description)?;
+    }
+    if let Some(values) = &mut self.field.values {
+      values.visit(visitor)?;
+    }
+    for l in &mut self.field.links {
+      visitor.visit_link(l)?;
+    }
+    visitor.visit_param_ended(self)
   }
-  pub fn set_values(mut self, values: Values) -> Self {
-    self.field.values = Some(values);
-    self
+}
+
+impl VOTableElement for Param {
+  const TAG: &'static str = "PARAM";
+
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    const DEFAULT_VALUE: &str = "@TBD";
+    const DEFAULT_DT: Datatype = Datatype::Logical;
+    let mut name_found = false;
+    let mut dt_found = false;
+    let mut val_found = false;
+    Self::new(DEFAULT_VALUE, DEFAULT_DT, DEFAULT_VALUE)
+      .set_attrs(attrs.map(|(k, v)| {
+        match k.as_ref() {
+          "name" => name_found = true,
+          "datatype" => dt_found = true,
+          "value" => val_found = true,
+          _ => {}
+        };
+        (k, v)
+      }))
+      .and_then(|param| {
+        if name_found && dt_found && val_found {
+          Ok(param)
+        } else {
+          Err(VOTableError::Custom(format!(
+            "Attributes 'name', 'datatype' and 'value' are mandatory in tag '{}'",
+            Self::TAG
+          )))
+        }
+      })
   }
-  pub fn push_link(mut self, link: Link) -> Self {
-    self.field.links.push(link);
-    self
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "ID" => self.set_id_by_ref(val),
+        "name" => self.set_name_by_ref(val),
+        "datatype" => {
+          self.set_datatype_by_ref(val.as_ref().parse().map_err(VOTableError::ParseDatatype)?)
+        }
+        "unit" => self.set_unit_by_ref(val),
+        "precision" => {
+          if val.as_ref().is_empty() {
+            warn!(
+              "Emtpy 'precision' attribute in tag {}: attribute ignored",
+              Self::TAG
+            )
+          } else {
+            self.set_precision_by_ref(val.as_ref().parse().map_err(VOTableError::ParseInt)?)
+          }
+        }
+        "width" => self.set_width_by_ref(val.as_ref().parse().map_err(VOTableError::ParseInt)?),
+        "xtype" => self.set_xtype_by_ref(val),
+        "ref" => self.set_ref_by_ref(val),
+        "ucd" => self.set_ucd_by_ref(val),
+        "utype" => self.set_utype_by_ref(val),
+        "arraysize" => {
+          self.set_arraysize_by_ref(val.as_ref().parse().map_err(VOTableError::ParseInt)?)
+        }
+        "value" => self.set_value_by_ref(val),
+        _ => self.insert_extra_str_by_ref(key, val),
+      }
+    }
+    Ok(())
   }
 
-  pub fn for_each_attribute<F>(&self, mut f: F)
+  fn for_each_attribute<F>(&self, mut f: F)
   where
     F: FnMut(&str, &str),
   {
     if let Some(id) = &self.field.id {
       f("ID", id.as_str());
     }
     f("name", self.field.name.as_str());
@@ -124,147 +184,50 @@
     }
     if let Some(xtype) = &self.field.xtype {
       f("xtype", xtype.as_str());
     }
     if let Some(ref_) = &self.field.ref_ {
       f("ref", ref_.as_str());
     }
-    for (k, v) in &self.field.extra {
-      f(k.as_str(), v.to_string().as_str());
-    }
-  }
-
-  pub fn visit<C, V>(&mut self, visitor: &mut V) -> Result<(), V::E>
-  where
-    C: TableDataContent,
-    V: VOTableVisitor<C>,
-  {
-    visitor.visit_param_start(self)?;
-    if let Some(description) = &mut self.field.description {
-      visitor.visit_description(description)?;
-    }
-    if let Some(values) = &mut self.field.values {
-      values.visit(visitor)?;
-    }
-    for l in &mut self.field.links {
-      visitor.visit_link(l)?;
-    }
-    visitor.visit_param_ended(self)
+    for_each_extra_attribute_delegated!(self, field, f);
   }
 }
 
-impl QuickXmlReadWrite for Param {
-  const TAG: &'static str = "PARAM";
+impl HasSubElements for Param {
   type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    const NULL: &str = "@TBD";
-    const NULL_DT: Datatype = Datatype::Logical;
-    let mut param = Self::new(NULL, NULL_DT, NULL);
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      param = match attr.key {
-        b"ID" => param.set_id(value),
-        b"name" => {
-          param.field.name = value.to_string();
-          param
-        }
-        b"datatype" => {
-          param.field.datatype = value
-            .parse::<Datatype>()
-            .map_err(VOTableError::ParseDatatype)?;
-          param
-        }
-        b"unit" => param.set_utype(value),
-        b"precision" if !value.is_empty() => {
-          param.set_precision(value.parse::<Precision>().map_err(VOTableError::ParseInt)?)
-        }
-        b"width" if !value.is_empty() => {
-          param.set_width(value.parse().map_err(VOTableError::ParseInt)?)
-        }
-        b"xtype" => param.set_xtype(value),
-        b"ref" => param.set_ref(value),
-        b"ucd" => param.set_ucd(value),
-        b"utype" => param.set_utype(value),
-        b"arraysize" if !value.is_empty() => {
-          param.set_arraysize(value.parse::<ArraySize>().map_err(VOTableError::ParseInt)?)
-        }
-        b"value" => {
-          param.value = value.to_string();
-          param
-        }
-        _ => param.insert_extra(
-          str::from_utf8(attr.key).map_err(VOTableError::Utf8)?,
-          Value::String(value.into()),
-        ),
-      }
-    }
-    if param.field.name.as_str() == NULL
-      || param.field.datatype == NULL_DT
-      || param.value.as_str() == NULL
-    {
-      Err(VOTableError::Custom(format!(
-        "Attributes 'name', 'datatype' and 'value' are mandatory in tag '{}'",
-        Self::TAG
-      )))
-    } else {
-      Ok(param)
-    }
-  }
-
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, context)
-      .map(|()| reader)
+  fn has_no_sub_elements(&self) -> bool {
+    self.field.has_no_sub_elements()
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
           Description::TAG_BYTES => {
-            self.field.description = Some(from_event_start_by_ref!(
-              Description,
-              reader,
-              reader_buff,
-              e
-            ))
-          }
-          Values::TAG_BYTES => {
-            self.field.values = Some(from_event_start_by_ref!(Values, reader, reader_buff, e))
-          }
-          Link::TAG_BYTES => {
-            self
-              .field
-              .links
-              .push(from_event_start_by_ref!(Link, reader, reader_buff, e))
+            set_from_event_start!(self, Description, reader, reader_buff, e)
           }
+          Values::TAG_BYTES => set_from_event_start!(self, Values, reader, reader_buff, e),
+          Link::TAG_BYTES => push_from_event_start!(self, Link, reader, reader_buff, e),
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
-          Values::TAG_BYTES => self.field.values = Some(Values::from_event_empty(e)?),
-          Link::TAG_BYTES => self.field.links.push(Link::from_event_empty(e)?),
+          Values::TAG_BYTES => set_from_event_empty!(self, Values, e),
+          Link::TAG_BYTES => push_from_event_empty!(self, Link, e),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
@@ -272,84 +235,33 @@
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
-    _context: &Self::Context,
+    context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    // copy/paste + modified from `cargo expand field`
-
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    if let Some(id) = &self.field.id {
-      tag.push_attribute(("ID", id.as_str()));
-    };
-    tag.push_attribute(("name", self.field.name.as_str()));
-    tag.push_attribute(("datatype", self.field.datatype.to_string().as_str()));
-    tag.push_attribute(("value", self.value.as_str()));
-    if let Some(unit) = &self.field.unit {
-      tag.push_attribute(("unit", unit.as_str()));
-    };
-    if let Some(precision) = &self.field.precision {
-      tag.push_attribute(("precision", precision.to_string().as_str()));
-    };
-    if let Some(width) = &self.field.width {
-      tag.push_attribute(("width", width.to_string().as_str()));
-    };
-    if let Some(xtype) = &self.field.xtype {
-      tag.push_attribute(("xtype", xtype.as_str()));
-    };
-    if let Some(ref_) = &self.field.ref_ {
-      tag.push_attribute(("ref", ref_.as_str()));
-    };
-    if let Some(ucd) = &self.field.ucd {
-      tag.push_attribute(("ucd", ucd.as_str()));
-    };
-    if let Some(utype) = &self.field.utype {
-      tag.push_attribute(("utype", utype.as_str()));
-    };
-    if let Some(arraysize) = &self.field.arraysize {
-      tag.push_attribute(("arraysize", arraysize.to_string().as_str()));
-    };
-    for (key, val) in &self.field.extra {
-      tag.push_attribute((key.as_str(), val.to_string().as_str()));
-    }
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    if let Some(elem) = &mut self.field.description {
-      elem.write(writer, &())?;
-    };
-    if let Some(elem) = &mut self.field.values {
-      elem.write(writer, &())?;
-    };
-    for elem in &mut self.field.links {
-      elem.write(writer, &())?;
-    }
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    self.field.write_sub_elements_by_ref(writer, context)
   }
 }
 
 #[cfg(test)]
 mod tests {
   use crate::{
     param::Param,
     tests::{test_read, test_writer},
   };
 
   #[test]
   fn test_params_read_write() {
-    let xml =
-      r#"<PARAM name="Freq" datatype="float" value="352" ucd="em.freq" utype="MHz"></PARAM>"#; // Test read
+    let xml = r#"<PARAM name="Freq" datatype="float" value="352" ucd="em.freq" utype="MHz"/>"#; // Test read
     let param = test_read::<Param>(xml);
     //Other parameters like name datatype etc... depend on Field reading, see Field read_write_test
     assert_eq!(param.value.as_str(), "352");
     // Test write
     test_writer(param, xml)
   }
 }
```

### Comparing `votable_cli-0.5.0/src/paramref.rs` & `votable_cli-0.6.0/src/paramref.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 //! Struct dedicated to the `PARAMref` tag.
 
-use std::{
-  collections::HashMap,
-  io::{BufRead, Write},
-  str,
-};
+use std::{collections::HashMap, str};
 
 use paste::paste;
-use quick_xml::{
-  events::{attributes::Attributes, BytesText, Event},
-  Reader, Writer,
-};
 use serde_json::Value;
 
 use super::{
-  error::VOTableError,
-  utils::{discard_comment, discard_event},
-  QuickXmlReadWrite, TableDataContent, VOTableVisitor,
+  error::VOTableError, HasContent, HasContentElem, TableDataContent, VOTableElement, VOTableVisitor,
 };
 
+/// Struct corresponding to the `PARAMRef` XML tag.
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct ParamRef {
   #[serde(rename = "ref")]
   pub ref_: String,
   #[serde(skip_serializing_if = "Option::is_none")]
   pub ucd: Option<String>,
   #[serde(skip_serializing_if = "Option::is_none")]
@@ -42,110 +33,86 @@
       ucd: None,
       utype: None,
       extra: Default::default(),
       content: None,
     }
   }
 
+  // attributes
+  impl_builder_mandatory_string_attr!(ref_, ref);
   impl_builder_opt_string_attr!(ucd);
   impl_builder_opt_string_attr!(utype);
-
+  // extra attributes
   impl_builder_insert_extra!();
 
-  impl_builder_opt_string_attr!(content);
-
-  /// Calls a closure on each (key, value) attribute pairs.
-  pub fn for_each_attribute<F>(&self, mut f: F)
-  where
-    F: FnMut(&str, &str),
-  {
-    f("ref", self.ref_.as_str());
-    if let Some(ucd) = &self.ucd {
-      f("ucd", ucd.as_str());
-    }
-    if let Some(utype) = &self.utype {
-      f("utype", utype.as_str());
-    }
-    for (k, v) in &self.extra {
-      f(k.as_str(), v.to_string().as_str());
-    }
-  }
-
   pub fn visit<C, V>(&mut self, visitor: &mut V) -> Result<(), V::E>
   where
     C: TableDataContent,
     V: VOTableVisitor<C>,
   {
     visitor.visit_paramref(self)
   }
 }
 
-impl QuickXmlReadWrite for ParamRef {
+impl_has_content!(ParamRef);
+
+impl VOTableElement for ParamRef {
   const TAG: &'static str = "PARAMref";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    const NULL: &str = "@TBD";
-    let mut paramref = Self::new(NULL);
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let value = str::from_utf8(attr.value.as_ref()).map_err(VOTableError::Utf8)?;
-      paramref = match attr.key {
-        b"ref" => {
-          paramref.ref_ = value.to_string();
-          paramref
-        }
-        b"ucd" => paramref.set_ucd(value),
-        b"utype" => paramref.set_utype(value),
-        _ => paramref.insert_extra(
-          str::from_utf8(attr.key).map_err(VOTableError::Utf8)?,
-          Value::String(value.into()),
-        ),
-      }
-    }
-    if paramref.ref_.as_str() == NULL {
-      Err(VOTableError::Custom(format!(
-        "Attributes 'ref' is mandatory in tag '{}'",
-        Self::TAG
-      )))
-    } else {
-      Ok(paramref)
-    }
-  }
+  type MarkerType = HasContentElem;
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    read_content!(Self, self, reader, reader_buff)
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    const DEFAULT_VALUE: &str = "@TBD";
+    Self::new(DEFAULT_VALUE).set_attrs(attrs).and_then(|pref| {
+      if pref.ref_.as_str() == DEFAULT_VALUE {
+        Err(VOTableError::Custom(format!(
+          "Mandatory attribute 'ref' not found in tag '{}'",
+          Self::TAG
+        )))
+      } else {
+        Ok(pref)
+      }
+    })
   }
 
-  fn read_sub_elements_by_ref<R: BufRead>(
-    &mut self,
-    reader: &mut Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    read_content_by_ref!(Self, self, reader, reader_buff)
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "ref" => self.set_ref_by_ref(val),
+        "ucd" => self.set_ucd_by_ref(val),
+        "utype" => self.set_utype_by_ref(val),
+        _ => self.insert_extra_str_by_ref(key, val),
+      }
+    }
+    Ok(())
   }
 
-  fn write<W: Write>(
-    &mut self,
-    writer: &mut Writer<W>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    let mut elem_writer = writer.create_element(Self::TAG_BYTES);
-    elem_writer = elem_writer.with_attribute(("ref", self.ref_.as_str()));
-    write_opt_string_attr!(self, elem_writer, ucd);
-    write_opt_string_attr!(self, elem_writer, utype);
-    write_extra!(self, elem_writer);
-    write_content!(self, elem_writer);
-    Ok(())
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    f("ref", self.ref_.as_str());
+    if let Some(ucd) = &self.ucd {
+      f("ucd", ucd.as_str());
+    }
+    if let Some(utype) = &self.utype {
+      f("utype", utype.as_str());
+    }
+    for_each_extra_attribute!(self, f);
   }
 }
 
 #[cfg(test)]
 mod tests {
   use crate::{
     paramref::ParamRef,
```

### Comparing `votable_cli-0.5.0/src/resource.rs` & `votable_cli-0.6.0/src/resource.rs`

 * *Files 13% similar despite different names*

```diff
@@ -5,35 +5,35 @@
   io::{BufRead, Write},
   mem, str,
 };
 
 use log::warn;
 use paste::paste;
 use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
+  events::{BytesStart, Event},
   Reader, Writer,
 };
 use serde_json::Value;
 
 #[cfg(feature = "mivot")]
-use super::mivot::{vodml::Vodml, VodmlVisitor};
+use super::mivot::vodml::Vodml;
 use super::{
   coosys::CooSys,
   data::{binary::Binary, binary2::Binary2, Data},
   desc::Description,
   error::VOTableError,
   group::Group,
   impls::mem::VoidTableDataContent,
   info::Info,
   link::Link,
   param::Param,
   table::Table,
   timesys::TimeSys,
   utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite, TableDataContent, VOTableVisitor,
+  HasSubElements, HasSubElems, QuickXmlReadWrite, TableDataContent, VOTableElement, VOTableVisitor,
 };
 
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "elem_type")]
 pub enum ResourceElem {
   CooSys(CooSys),
   TimeSys(TimeSys),
@@ -67,14 +67,24 @@
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "elem_type")]
 pub enum ResourceOrTable<C: TableDataContent> {
   Resource(Resource<C>),
   Table(Table<C>),
 }
 impl<C: TableDataContent> ResourceOrTable<C> {
+  /// # WARNING
+  /// Call only for a resource, not for a table with actual data.
+  fn from_void_table_data_content(value: ResourceOrTable<VoidTableDataContent>) -> Self {
+    match value {
+      ResourceOrTable::<VoidTableDataContent>::Resource(e) => {
+        Self::Resource(Resource::from_void_table_data_content(e))
+      }
+      ResourceOrTable::<VoidTableDataContent>::Table(_) => todo!(), // No supposed to call this!!
+    }
+  }
   fn write<W: Write>(&mut self, writer: &mut Writer<W>) -> Result<(), VOTableError> {
     match self {
       ResourceOrTable::Resource(elem) => elem.write(writer, &()),
       ResourceOrTable::Table(elem) => elem.write(writer, &()),
     }
   }
   pub fn visit<V>(&mut self, visitor: &mut V) -> Result<(), V::E>
@@ -109,14 +119,27 @@
     Self {
       links: Default::default(),
       resource_or_table: ResourceOrTable::Table(table),
       infos: Default::default(),
     }
   }
 
+  pub fn from_void_table_data_content(value: ResourceSubElem<VoidTableDataContent>) -> Self {
+    let ResourceSubElem {
+      links,
+      resource_or_table,
+      infos,
+    } = value;
+    Self {
+      links,
+      resource_or_table: ResourceOrTable::from_void_table_data_content(resource_or_table),
+      infos,
+    }
+  }
+
   impl_builder_push!(Link);
   impl_builder_push!(Info);
 
   pub fn set_links(mut self, links: Vec<Link>) -> Self {
     self.links = links;
     self
   }
@@ -195,14 +218,15 @@
     write_elem_vec_empty_context!(self, links, writer);
     self.resource_or_table.write(writer)?;
     write_elem_vec_empty_context!(self, infos, writer);
     Ok(())
   }
 }
 
+/// Struct corresponding to the `RESOURCE` XML tag.
 #[derive(Default, Clone, PartialEq, Debug, serde::Serialize, serde::Deserialize)]
 pub struct Resource<C: TableDataContent> {
   // Attributes
   #[serde(rename = "ID", default, skip_serializing_if = "Option::is_none")]
   pub id: Option<String>,
   #[serde(skip_serializing_if = "Option::is_none")]
   pub name: Option<String>,
@@ -246,70 +270,127 @@
 }
 
 impl<C: TableDataContent> Resource<C> {
   pub fn new() -> Self {
     Default::default()
   }
 
+  pub fn from_void_table_data_content(value: Resource<VoidTableDataContent>) -> Self {
+    let Resource {
+      id,
+      name,
+      type_,
+      utype,
+      extra,
+      description,
+      infos,
+      elems,
+      mut sub_elems,
+      vodml,
+    } = value;
+    Self {
+      id,
+      name,
+      type_,
+      utype,
+      extra,
+      description,
+      infos,
+      elems,
+      sub_elems: sub_elems
+        .drain(..)
+        .map(ResourceSubElem::from_void_table_data_content)
+        .collect(),
+      vodml,
+    }
+  }
+
   // Optional attributes
   impl_builder_opt_string_attr!(id);
   impl_builder_opt_string_attr!(name);
   impl_builder_opt_string_attr!(type_, type);
   impl_builder_opt_string_attr!(utype);
   // - extra attributes
   impl_builder_insert_extra!();
   // Sequence elements
-  impl_builder_opt_attr!(description, Description);
+  impl_builder_opt_subelem!(description, Description);
   impl_builder_push!(Info);
   // - choice elements
   impl_builder_push_elem!(CooSys, ResourceElem);
   impl_builder_push_elem!(TimeSys, ResourceElem);
   impl_builder_push_elem!(Group, ResourceElem);
   impl_builder_push_elem!(Param, ResourceElem);
+
   pub fn push_elem(mut self, elem: ResourceElem) -> Self {
     self.push_elem_by_ref(elem);
     self
   }
   pub fn push_elem_by_ref(&mut self, elem: ResourceElem) {
     self.elems.push(elem);
   }
+
   // - sub-sequence elements
   pub fn push_sub_elem(mut self, sub_elem: ResourceSubElem<C>) -> Self {
     self.sub_elems.push(sub_elem);
     self
   }
   pub fn push_sub_elem_by_ref(&mut self, sub_elem: ResourceSubElem<C>) {
     self.sub_elems.push(sub_elem);
   }
-  // - extra optional element
-  #[cfg(feature = "mivot")]
-  impl_builder_opt_attr!(vodml, Vodml);
 
-  /// Calls a closure on each (key, value) attribute pairs.
-  pub fn for_each_attribute<F>(&self, mut f: F)
-  where
-    F: FnMut(&str, &str),
-  {
-    if let Some(id) = &self.id {
-      f("ID", id.as_str());
-    }
-    if let Some(name) = &self.name {
-      f("name", name.as_str());
-    }
-    if let Some(type_) = &self.type_ {
-      f("type", type_.as_str());
-    }
-    if let Some(utype) = &self.utype {
-      f("utype", utype.as_str());
-    }
-    for (k, v) in &self.extra {
-      f(k.as_str(), v.to_string().as_str());
-    }
+  /// Create and push a simple sub-elem only containing a table.
+  pub fn push_table(mut self, table: Table<C>) -> Self {
+    self.push_table_by_ref(table);
+    self
+  }
+  /// Create and push a simple sub-elem only containing a table.
+  pub fn push_table_by_ref(&mut self, table: Table<C>) {
+    self.sub_elems.push(ResourceSubElem::from_table(table));
+  }
+  /// Create and push a simple sub-elem only containing a resource.
+  pub fn push_resource(mut self, resource: Resource<C>) -> Self {
+    self.push_resource_by_ref(resource);
+    self
+  }
+  /// Create and push a simple sub-elem only containing a resource.
+  pub fn push_resource_by_ref(&mut self, resource: Resource<C>) {
+    self
+      .sub_elems
+      .push(ResourceSubElem::from_resource(resource));
+  }
+  /// Create and prepend a simple sub-elem only containing a resource.
+  pub fn prepend_resource(mut self, resource: Resource<C>) -> Self {
+    self.prepend_resource_by_ref(resource);
+    self
+  }
+  /// Create and prepend a simple sub-elem only containing a resource.
+  pub fn prepend_resource_by_ref(&mut self, resource: Resource<C>) {
+    self
+      .sub_elems
+      .insert(0, ResourceSubElem::from_resource(resource));
+  }
+  /// Push the given link into the last sub-element.
+  pub fn push_link(mut self, link: Link) -> Result<Self, VOTableError> {
+    self.push_link_by_ref(link).map(|()| self)
+  }
+  /// Push the given link into the last sub-element
+  pub fn push_link_by_ref(&mut self, link: Link) -> Result<(), VOTableError> {
+    self
+      .sub_elems
+      .last_mut()
+      .map(|sub_elem| sub_elem.push_link_by_ref(link))
+      .ok_or(VOTableError::Custom(String::from(
+        "No sub-resource in which a link can be added",
+      )))
   }
 
+  // - extra optional element
+  #[cfg(feature = "mivot")]
+  impl_builder_opt_subelem!(vodml, Vodml);
+
   pub fn visit<V>(&mut self, visitor: &mut V) -> Result<(), V::E>
   where
     V: VOTableVisitor<C>,
   {
     visitor.visit_resource_start(self)?;
     if let Some(desc) = &mut self.description {
       visitor.visit_description(desc)?;
@@ -321,15 +402,16 @@
       e.visit(visitor)?;
     }
     for e in self.sub_elems.iter_mut() {
       e.visit(visitor)?;
     }
     #[cfg(feature = "mivot")]
     if let Some(vodml) = &mut self.vodml {
-      visitor.get_mivot_visitor().visit_vodml(vodml)?;
+      let mut vodml_visitor = visitor.get_mivot_visitor();
+      vodml.visit(&mut vodml_visitor)?;
     }
     visitor.visit_resource_ended(self)
   }
 
   pub(crate) fn ensures_consistency(&mut self) -> Result<(), String> {
     for elem in self.sub_elems.iter_mut() {
       if let ResourceOrTable::Table(table) = &mut elem.resource_or_table {
@@ -500,44 +582,33 @@
   ) -> Result<Option<ResourceSubElem<C>>, VOTableError> {
     let mut links: Vec<Link> = Default::default();
     reader = reader.check_end_names(false);
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          Description::TAG_BYTES => {
-            from_event_start_desc_by_ref!(self, Description, reader, reader_buff, e)
-          }
+          Description::TAG_BYTES => set_desc_from_event_start!(self, reader, reader_buff, e),
           Info::TAG_BYTES => {
             let info = from_event_start_by_ref!(Info, reader, reader_buff, e);
             if let Some(sub_elem) = self.sub_elems.last_mut() {
               sub_elem.push_info_by_ref(info)
             } else {
               self.push_info_by_ref(info)
             }
           }
-          CooSys::TAG_BYTES => {
-            self.push_coosys_by_ref(from_event_start_by_ref!(CooSys, reader, reader_buff, e))
-          }
-          Group::TAG_BYTES => {
-            self.push_group_by_ref(from_event_start_by_ref!(Group, reader, reader_buff, e))
-          }
-          Param::TAG_BYTES => {
-            self.push_param_by_ref(from_event_start_by_ref!(Param, reader, reader_buff, e))
-          }
+          CooSys::TAG_BYTES => push_from_event_start!(self, CooSys, reader, reader_buff, e),
+          Group::TAG_BYTES => push_from_event_start!(self, Group, reader, reader_buff, e),
+          Param::TAG_BYTES => push_from_event_start!(self, Param, reader, reader_buff, e),
           Link::TAG_BYTES => links.push(from_event_start_by_ref!(Link, reader, reader_buff, e)),
           #[cfg(feature = "mivot")]
-          Vodml::TAG_BYTES => {
-            from_event_start_vodml_by_ref!(self, Vodml, reader, reader_buff, e)
-          }
+          Vodml::TAG_BYTES => set_from_event_start!(self, Vodml, reader, reader_buff, e),
           Table::<C>::TAG_BYTES => {
-            let table = Table::<C>::from_attributes(e.attributes())?;
-            return Ok(Some(
-              ResourceSubElem::from_table(table).set_links(mem::take(&mut links)),
-            ));
+            return Table::<C>::from_event_start(e).map(|table| {
+              Some(ResourceSubElem::from_table(table).set_links(mem::take(&mut links)))
+            });
           }
           Resource::<C>::TAG_BYTES => {
             let resource = from_event_start_by_ref!(Resource, reader, reader_buff, e);
             self.push_sub_elem_by_ref(
               ResourceSubElem::from_resource(resource).set_links(mem::take(&mut links)),
             );
           }
@@ -553,18 +624,18 @@
             let info = Info::from_event_empty(e)?;
             if let Some(sub_elem) = self.sub_elems.last_mut() {
               sub_elem.push_info_by_ref(info)
             } else {
               self.infos.push(info)
             }
           }
-          TimeSys::TAG_BYTES => self.push_timesys_by_ref(TimeSys::from_event_empty(e)?),
-          CooSys::TAG_BYTES => self.push_coosys_by_ref(CooSys::from_event_empty(e)?),
-          Group::TAG_BYTES => self.push_group_by_ref(Group::from_event_empty(e)?),
-          Param::TAG_BYTES => self.push_param_by_ref(Param::from_event_empty(e)?),
+          TimeSys::TAG_BYTES => push_from_event_empty!(self, TimeSys, e),
+          CooSys::TAG_BYTES => push_from_event_empty!(self, CooSys, e),
+          Group::TAG_BYTES => push_from_event_empty!(self, Group, e),
+          Param::TAG_BYTES => push_from_event_empty!(self, Param, e),
           Link::TAG_BYTES => links.push(Link::from_event_empty(e)?),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
@@ -593,50 +664,38 @@
   ) -> Result<Option<ResourceSubElem<C>>, VOTableError> {
     let mut links: Vec<Link> = Default::default();
     reader = reader.check_end_names(false);
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          Description::TAG_BYTES => {
-            from_event_start_desc_by_ref!(self, Description, reader, reader_buff, e)
-          }
+          Description::TAG_BYTES => set_desc_from_event_start!(self, reader, reader_buff, e),
           Info::TAG_BYTES => {
             let info = from_event_start_by_ref!(Info, reader, reader_buff, e);
             if let Some(sub_elem) = self.sub_elems.last_mut() {
               sub_elem.push_info_by_ref(info)
             } else {
               self.push_info_by_ref(info)
             }
           }
-          CooSys::TAG_BYTES => {
-            self.push_coosys_by_ref(from_event_start_by_ref!(CooSys, reader, reader_buff, e))
-          }
-          Group::TAG_BYTES => {
-            self.push_group_by_ref(from_event_start_by_ref!(Group, reader, reader_buff, e))
-          }
-          Param::TAG_BYTES => {
-            self.push_param_by_ref(from_event_start_by_ref!(Param, reader, reader_buff, e))
-          }
+          CooSys::TAG_BYTES => push_from_event_start!(self, CooSys, reader, reader_buff, e),
+          Group::TAG_BYTES => push_from_event_start!(self, Group, reader, reader_buff, e),
+          Param::TAG_BYTES => push_from_event_start!(self, Param, reader, reader_buff, e),
           Link::TAG_BYTES => links.push(from_event_start_by_ref!(Link, reader, reader_buff, e)),
           #[cfg(feature = "mivot")]
-          Vodml::TAG_BYTES => {
-            from_event_start_vodml_by_ref!(self, Vodml, reader, reader_buff, e)
-          }
+          Vodml::TAG_BYTES => set_from_event_start!(self, Vodml, reader, reader_buff, e),
           Table::<C>::TAG_BYTES => {
-            let table = Table::<C>::from_attributes(e.attributes())?;
-            return Ok(Some(
-              ResourceSubElem::from_table(table).set_links(mem::take(&mut links)),
-            ));
+            return Table::<C>::from_event_start(e).map(|table| {
+              Some(ResourceSubElem::from_table(table).set_links(mem::take(&mut links)))
+            });
           }
           Resource::<C>::TAG_BYTES => {
-            let resource = Resource::<C>::from_attributes(e.attributes())?;
-            return Ok(Some(
-              ResourceSubElem::from_resource(resource).set_links(mem::take(&mut links)),
-            ));
+            return Resource::<C>::from_event_start(e).map(|resource| {
+              Some(ResourceSubElem::from_resource(resource).set_links(mem::take(&mut links)))
+            });
           }
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
@@ -646,18 +705,18 @@
             let info = Info::from_event_empty(e)?;
             if let Some(sub_elem) = self.sub_elems.last_mut() {
               sub_elem.push_info_by_ref(info)
             } else {
               self.infos.push(info)
             }
           }
-          TimeSys::TAG_BYTES => self.push_timesys_by_ref(TimeSys::from_event_empty(e)?),
-          CooSys::TAG_BYTES => self.push_coosys_by_ref(CooSys::from_event_empty(e)?),
-          Group::TAG_BYTES => self.push_group_by_ref(Group::from_event_empty(e)?),
-          Param::TAG_BYTES => self.push_param_by_ref(Param::from_event_empty(e)?),
+          TimeSys::TAG_BYTES => push_from_event_empty!(self, TimeSys, e),
+          CooSys::TAG_BYTES => push_from_event_empty!(self, CooSys, e),
+          Group::TAG_BYTES => push_from_event_empty!(self, Group, e),
+          Param::TAG_BYTES => push_from_event_empty!(self, Param, e),
           Link::TAG_BYTES => links.push(Link::from_event_empty(e)?),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
@@ -687,19 +746,15 @@
     &mut self,
     writer: &mut Writer<W>,
     context: &(),
     stop_before_data: bool,
   ) -> Result<bool, VOTableError> {
     let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
     // Write tag + attributes
-    push2write_opt_string_attr!(self, tag, ID);
-    push2write_opt_string_attr!(self, tag, name);
-    push2write_opt_string_attr!(self, tag, type_, type);
-    push2write_opt_string_attr!(self, tag, utype);
-    push2write_extra!(self, tag);
+    self.for_each_attribute(|k, v| tag.push_attribute((k, v)));
     writer
       .write_event(Event::Start(tag.to_borrowed()))
       .map_err(VOTableError::Write)?;
     // Write sub-elements
     write_elem!(self, description, writer, context);
     write_elem_vec!(self, infos, writer, context);
     write_elem_vec_no_context!(self, elems, writer);
@@ -767,91 +822,125 @@
     } else {
       // Tag has already been closed by the call to write_to_data_beginning
       Ok(false)
     }
   }
 }
 
-impl<C: TableDataContent> QuickXmlReadWrite for Resource<C> {
+impl<C: TableDataContent> VOTableElement for Resource<C> {
   const TAG: &'static str = "RESOURCE";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut resource = Self::new();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let value = str::from_utf8(attr.value.as_ref()).map_err(VOTableError::Utf8)?;
-      resource = match attr.key {
-        b"ID" => resource.set_id(value),
-        b"name" => resource.set_name(value),
-        b"type" => resource.set_type(value),
-        b"utype" => resource.set_utype(value),
-        _ => resource.insert_extra(
-          str::from_utf8(attr.key).map_err(VOTableError::Utf8)?,
-          Value::String(value.into()),
-        ),
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::default().set_attrs(attrs)
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key_str = key.as_ref();
+      match key_str {
+        "ID" => self.set_id_by_ref(val),
+        "name" => self.set_name_by_ref(val),
+        "type" => self.set_type_by_ref(val),
+        "utype" => self.set_utype_by_ref(val),
+        _ => self.insert_extra_str_by_ref(key, val),
       }
     }
-    Ok(resource)
+    Ok(())
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, context)
-      .map(|()| reader)
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    if let Some(id) = &self.id {
+      f("ID", id.as_str());
+    }
+    if let Some(name) = &self.name {
+      f("name", name.as_str());
+    }
+    if let Some(type_) = &self.type_ {
+      f("type", type_.as_str());
+    }
+    if let Some(utype) = &self.utype {
+      f("utype", utype.as_str());
+    }
+    for_each_extra_attribute!(self, f);
+  }
+}
+
+impl<C: TableDataContent> HasSubElements for Resource<C> {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    #[cfg(not(feature = "mivot"))]
+    {
+      self.description.is_none()
+        && self.infos.is_empty()
+        && self.elems.is_empty()
+        && self.sub_elems.is_empty()
+    }
+    #[cfg(feature = "mivot")]
+    {
+      self.description.is_none()
+        && self.infos.is_empty()
+        && self.elems.is_empty()
+        && self.sub_elems.is_empty()
+        && self.vodml.is_none()
+    }
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
   ) -> Result<(), VOTableError> {
     let mut links: Vec<Link> = Default::default();
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          Description::TAG_BYTES => {
-            from_event_start_desc_by_ref!(self, Description, reader, reader_buff, e)
-          }
+          Description::TAG_BYTES => set_desc_from_event_start!(self, reader, reader_buff, e),
           Info::TAG_BYTES => {
             let info = from_event_start_by_ref!(Info, reader, reader_buff, e);
             if let Some(sub_elem) = self.sub_elems.last_mut() {
               sub_elem.push_info_by_ref(info)
             } else {
               self.push_info_by_ref(info)
             }
           }
-          Group::TAG_BYTES => {
-            self.push_group_by_ref(from_event_start_by_ref!(Group, reader, reader_buff, e))
-          }
-          Param::TAG_BYTES => {
-            self.push_param_by_ref(from_event_start_by_ref!(Param, reader, reader_buff, e))
-          }
+          Group::TAG_BYTES => push_from_event_start!(self, Group, reader, reader_buff, e),
+          Param::TAG_BYTES => push_from_event_start!(self, Param, reader, reader_buff, e),
           Link::TAG_BYTES => links.push(from_event_start_by_ref!(Link, reader, reader_buff, e)),
           Table::<C>::TAG_BYTES => {
             let table = from_event_start_by_ref!(Table, reader, reader_buff, e);
             self.push_sub_elem_by_ref(
               ResourceSubElem::from_table(table).set_links(mem::take(&mut links)),
             );
           }
           Resource::<C>::TAG_BYTES => {
             let resource = from_event_start_by_ref!(Resource, reader, reader_buff, e);
             self.push_sub_elem_by_ref(
               ResourceSubElem::from_resource(resource).set_links(mem::take(&mut links)),
             );
           }
           #[cfg(feature = "mivot")]
-          Vodml::TAG_BYTES => from_event_start_vodml_by_ref!(self, Vodml, reader, reader_buff, e),
+          Vodml::TAG_BYTES => set_from_event_start!(self, Vodml, reader, reader_buff, e),
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
@@ -860,18 +949,18 @@
             let info = Info::from_event_empty(e)?;
             if let Some(sub_elem) = self.sub_elems.last_mut() {
               sub_elem.push_info_by_ref(info)
             } else {
               self.infos.push(info)
             }
           }
-          TimeSys::TAG_BYTES => self.push_timesys_by_ref(TimeSys::from_event_empty(e)?),
-          CooSys::TAG_BYTES => self.push_coosys_by_ref(CooSys::from_event_empty(e)?),
-          Group::TAG_BYTES => self.push_group_by_ref(Group::from_event_empty(e)?),
-          Param::TAG_BYTES => self.push_param_by_ref(Param::from_event_empty(e)?),
+          TimeSys::TAG_BYTES => push_from_event_empty!(self, TimeSys, e),
+          CooSys::TAG_BYTES => push_from_event_empty!(self, CooSys, e),
+          Group::TAG_BYTES => push_from_event_empty!(self, Group, e),
+          Param::TAG_BYTES => push_from_event_empty!(self, Param, e),
           Link::TAG_BYTES => links.push(Link::from_event_empty(e)?),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
@@ -887,69 +976,59 @@
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    push2write_opt_string_attr!(self, tag, ID);
-    push2write_opt_string_attr!(self, tag, name);
-    push2write_opt_string_attr!(self, tag, type_, type);
-    push2write_opt_string_attr!(self, tag, utype);
-    push2write_extra!(self, tag);
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elements
     write_elem!(self, description, writer, context);
     write_elem_vec!(self, infos, writer, context);
     write_elem_vec_no_context!(self, elems, writer);
     write_elem_vec_no_context!(self, sub_elems, writer);
     #[cfg(feature = "mivot")]
     write_elem_vec!(self, vodml, writer, context);
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    Ok(())
   }
 }
 
 #[cfg(test)]
 mod tests {
   use crate::{
     impls::mem::InMemTableDataRows,
     resource::Resource,
     tests::{test_read, test_writer},
   };
 
   #[test]
   fn test_resource_read_write() {
-    let xml = r#"<RESOURCE ID="yCat_5147" name="V/147"><DESCRIPTION>The SDSS Photometric Catalogue, Release 12 (Alam+, 2015)</DESCRIPTION><INFO name="matches" value="50">matching records</INFO><INFO name="warning" value="No center provided++++"/><TABLE ID="V_147_sdss12" name="V/147/sdss12"><FIELD name="RA_ICRS" datatype="char" ucd="pos.eq.ra;meta.main"></FIELD><DATA><TABLEDATA><TR><TD>a</TD></TR></TABLEDATA></DATA></TABLE><TABLE ID="V_148_sdss12" name="V/148/sdss12"><FIELD name="DE_ICRS" datatype="char" ucd="pos.eq.dec;meta.main"></FIELD><DATA><TABLEDATA><TR><TD>b</TD></TR></TABLEDATA></DATA></TABLE></RESOURCE>"#; // Test read
+    let xml = r#"<RESOURCE ID="yCat_5147" name="V/147"><DESCRIPTION>The SDSS Photometric Catalogue, Release 12 (Alam+, 2015)</DESCRIPTION><INFO name="matches" value="50">matching records</INFO><INFO name="warning" value="No center provided++++"/><TABLE ID="V_147_sdss12" name="V/147/sdss12"><FIELD name="RA_ICRS" datatype="char" ucd="pos.eq.ra;meta.main"/><DATA><TABLEDATA><TR><TD>a</TD></TR></TABLEDATA></DATA></TABLE><TABLE ID="V_148_sdss12" name="V/148/sdss12"><FIELD name="DE_ICRS" datatype="char" ucd="pos.eq.dec;meta.main"/><DATA><TABLEDATA><TR><TD>b</TD></TR></TABLEDATA></DATA></TABLE></RESOURCE>"#; // Test read
     let resource = test_read::<Resource<InMemTableDataRows>>(xml);
     assert_eq!(resource.id.as_ref().unwrap().as_str(), "yCat_5147");
     assert_eq!(resource.name.as_ref().unwrap().as_str(), "V/147");
     assert_eq!(
-      resource.description.as_ref().unwrap().0,
+      resource
+        .description
+        .as_ref()
+        .unwrap()
+        .get_content_unwrapped(),
       "The SDSS Photometric Catalogue, Release 12 (Alam+, 2015)"
     );
     assert_eq!(resource.sub_elems.len(), 2);
     assert_eq!(resource.infos.get(0).unwrap().name, "matches");
     assert_eq!(resource.infos.get(1).unwrap().name, "warning");
     // Test write
     test_writer(resource, xml);
   }
 
   #[test]
   fn test_resource_read_write_w_end_info() {
-    let xml = r#"<RESOURCE ID="yCat_5147" name="V/147"><DESCRIPTION>The SDSS Photometric Catalogue, Release 12 (Alam+, 2015)</DESCRIPTION><TABLE ID="V_148_sdss12" name="V/148/sdss12"><FIELD name="DE_ICRS" datatype="char" ucd="pos.eq.dec;meta.main"></FIELD><DATA><TABLEDATA><TR><TD>b</TD></TR></TABLEDATA></DATA></TABLE><INFO name="matches" value="50">matching records</INFO><INFO name="warning" value="No center provided++++"/></RESOURCE>"#; // Test read
+    let xml = r#"<RESOURCE ID="yCat_5147" name="V/147"><DESCRIPTION>The SDSS Photometric Catalogue, Release 12 (Alam+, 2015)</DESCRIPTION><TABLE ID="V_148_sdss12" name="V/148/sdss12"><FIELD name="DE_ICRS" datatype="char" ucd="pos.eq.dec;meta.main"/><DATA><TABLEDATA><TR><TD>b</TD></TR></TABLEDATA></DATA></TABLE><INFO name="matches" value="50">matching records</INFO><INFO name="warning" value="No center provided++++"/></RESOURCE>"#; // Test read
     let resource = test_read::<Resource<InMemTableDataRows>>(xml);
     assert_eq!(resource.sub_elems[0].infos[0].name, "matches");
     assert_eq!(resource.sub_elems[0].infos[1].name, "warning");
   }
 }
```

### Comparing `votable_cli-0.5.0/src/table.rs` & `votable_cli-0.6.0/src/table.rs`

 * *Files 11% similar despite different names*

```diff
@@ -5,30 +5,30 @@
   io::{BufRead, Write},
   str,
 };
 
 use log::warn;
 use paste::paste;
 use quick_xml::{
-  events::{attributes::Attributes, BytesStart, Event},
+  events::{BytesStart, Event},
   Reader, Writer,
 };
 use serde_json::Value;
 
 use super::{
   data::Data,
   desc::Description,
   error::VOTableError,
   field::Field,
   group::TableGroup,
   info::Info,
   link::Link,
   param::Param,
   utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite, TableDataContent, VOTableVisitor,
+  HasSubElements, HasSubElems, QuickXmlReadWrite, TableDataContent, VOTableElement, VOTableVisitor,
 };
 
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 #[serde(tag = "elem_type")]
 pub enum TableElem {
   Field(Field),
   Param(Param),
@@ -51,14 +51,15 @@
       TableElem::Field(e) => e.visit(visitor),
       TableElem::Param(e) => e.visit(visitor),
       TableElem::TableGroup(e) => e.visit(visitor),
     }
   }
 }
 
+/// Struct corresponding to the `TABLE` XML tag.
 #[derive(Default, Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct Table<C: TableDataContent> {
   // attributes
   #[serde(skip_serializing_if = "Option::is_none")]
   pub id: Option<String>,
   #[serde(skip_serializing_if = "Option::is_none")]
   pub name: Option<String>,
@@ -98,15 +99,15 @@
   impl_builder_opt_string_attr!(ucd);
   impl_builder_opt_string_attr!(utype);
   impl_builder_opt_string_attr!(ref_, ref);
   impl_builder_opt_attr!(nrows, u64);
 
   impl_builder_insert_extra!();
 
-  impl_builder_opt_attr!(description, Description);
+  impl_builder_opt_subelem!(description, Description);
 
   impl_builder_push_elem!(Field, TableElem);
   impl_builder_push_elem!(Param, TableElem);
   impl_builder_push_elem!(TableGroup, TableElem);
 
   impl_builder_push!(Link);
 
@@ -117,42 +118,14 @@
 
   pub fn set_data_by_ref(&mut self, data: Data<C>) {
     self.data = Some(data);
   }
 
   impl_builder_push!(Info);
 
-  /// Calls a closure on each (key, value) attribute pairs.
-  pub fn for_each_attribute<F>(&self, mut f: F)
-  where
-    F: FnMut(&str, &str),
-  {
-    if let Some(id) = &self.id {
-      f("ID", id.as_str());
-    }
-    if let Some(name) = &self.name {
-      f("name", name.as_str());
-    }
-    if let Some(ucd) = &self.ucd {
-      f("ucd", ucd.as_str());
-    }
-    if let Some(utype) = &self.utype {
-      f("utype", utype.as_str());
-    }
-    if let Some(ref_) = &self.ref_ {
-      f("ref", ref_.as_str());
-    }
-    if let Some(nrows) = &self.nrows {
-      f("nrows", nrows.to_string().as_str());
-    }
-    for (k, v) in &self.extra {
-      f(k.as_str(), v.to_string().as_str());
-    }
-  }
-
   pub fn visit<V>(&mut self, visitor: &mut V) -> Result<(), V::E>
   where
     V: VOTableVisitor<C>,
   {
     visitor.visit_table_start(self)?;
     if let Some(description) = &mut self.description {
       visitor.visit_description(description)?;
@@ -185,17 +158,15 @@
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
   ) -> Result<Option<Data<C>>, VOTableError> {
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          Description::TAG_BYTES => {
-            from_event_start_desc_by_ref!(self, Description, reader, reader_buff, e)
-          }
+          Description::TAG_BYTES => set_desc_from_event_start!(self, reader, reader_buff, e),
           Field::TAG_BYTES => {
             self.push_field_by_ref(from_event_start_by_ref!(Field, reader, reader_buff, e))
           }
           Param::TAG_BYTES => {
             self.push_param_by_ref(from_event_start_by_ref!(Param, reader, reader_buff, e))
           }
           TableGroup::TAG_BYTES => self.push_tablegroup_by_ref(from_event_start_by_ref!(
@@ -203,18 +174,15 @@
             reader,
             reader_buff,
             e
           )),
           Link::TAG_BYTES => {
             self.push_link_by_ref(from_event_start_by_ref!(Link, reader, reader_buff, e))
           }
-          Data::<C>::TAG_BYTES => {
-            let data = Data::from_attributes(e.attributes())?;
-            return Ok(Some(data));
-          }
+          Data::<C>::TAG_BYTES => return Data::from_event_start(e).map(Some),
           Info::TAG_BYTES => {
             self.push_info_by_ref(from_event_start_by_ref!(Info, reader, reader_buff, e))
           }
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
@@ -250,21 +218,15 @@
     &mut self,
     writer: &mut Writer<W>,
     context: &(),
     stop_before_data: bool,
   ) -> Result<(), VOTableError> {
     let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
     // Write tag + attributes
-    push2write_opt_string_attr!(self, tag, ID);
-    push2write_opt_string_attr!(self, tag, name);
-    push2write_opt_string_attr!(self, tag, ucd);
-    push2write_opt_string_attr!(self, tag, utype);
-    push2write_opt_string_attr!(self, tag, ref_, ref);
-    push2write_opt_tostring_attr!(self, tag, nrows);
-    push2write_extra!(self, tag);
+    self.for_each_attribute(|k, v| tag.push_attribute((k, v)));
     writer
       .write_event(Event::Start(tag.to_borrowed()))
       .map_err(VOTableError::Write)?;
     // Write sub-elems
     write_elem!(self, description, writer, context);
     write_elem_vec_no_context!(self, elems, writer);
     write_elem_vec!(self, links, writer, context);
@@ -331,49 +293,84 @@
       })
     } else {
       Ok(())
     }
   }
 }
 
-impl<C: TableDataContent> QuickXmlReadWrite for Table<C> {
+impl<C: TableDataContent> VOTableElement for Table<C> {
   const TAG: &'static str = "TABLE";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut table = Self::new();
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      table = match attr.key {
-        b"ID" => table.set_id(value),
-        b"name" => table.set_name(value),
-        b"ucd" => table.set_ucd(value),
-        b"utype" => table.set_ucd(value),
-        b"ref" => table.set_ref(value),
-        b"nrows" => table.set_nrows(value.parse().map_err(VOTableError::ParseInt)?),
-        _ => table.insert_extra(
-          str::from_utf8(attr.key).map_err(VOTableError::Utf8)?,
-          Value::String(value.into()),
-        ),
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::default().set_attrs(attrs)
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key_str = key.as_ref();
+      match key_str {
+        "ID" => self.set_id_by_ref(val),
+        "name" => self.set_name_by_ref(val),
+        "ucd" => self.set_ucd_by_ref(val),
+        "utype" => self.set_ucd_by_ref(val),
+        "ref" => self.set_ref_by_ref(val),
+        "nrows" => self.set_nrows_by_ref(val.as_ref().parse().map_err(VOTableError::ParseInt)?),
+        _ => self.insert_extra_str_by_ref(key, val),
       }
     }
-    Ok(table)
+    Ok(())
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, context)
-      .map(|()| reader)
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    if let Some(id) = &self.id {
+      f("ID", id.as_str());
+    }
+    if let Some(name) = &self.name {
+      f("name", name.as_str());
+    }
+    if let Some(ucd) = &self.ucd {
+      f("ucd", ucd.as_str());
+    }
+    if let Some(utype) = &self.utype {
+      f("utype", utype.as_str());
+    }
+    if let Some(ref_) = &self.ref_ {
+      f("ref", ref_.as_str());
+    }
+    if let Some(nrows) = &self.nrows {
+      f("nrows", nrows.to_string().as_str());
+    }
+    for_each_extra_attribute!(self, f);
+  }
+}
+
+impl<C: TableDataContent> HasSubElements for Table<C> {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    self.description.is_none()
+      && self.elems.is_empty()
+      && self.links.is_empty()
+      && self.data.is_none()
+      && self.infos.is_empty()
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
@@ -381,17 +378,15 @@
     // If the full document is in memory, we could have use a Reader<'a [u8]> and then the method
     // `read_event_unbuffered` to avoid a copy.
     // But are more generic that this to be able to read in streaming mode
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          Description::TAG_BYTES => {
-            from_event_start_desc_by_ref!(self, Description, reader, reader_buff, e)
-          }
+          Description::TAG_BYTES => set_desc_from_event_start!(self, reader, reader_buff, e),
           Field::TAG_BYTES => {
             self.push_field_by_ref(from_event_start_by_ref!(Field, reader, reader_buff, e))
           }
           Param::TAG_BYTES => {
             self.push_param_by_ref(from_event_start_by_ref!(Param, reader, reader_buff, e))
           }
           TableGroup::TAG_BYTES => self.push_tablegroup_by_ref(from_event_start_by_ref!(
@@ -439,58 +434,41 @@
         Event::End(e) if e.local_name() == Self::TAG_BYTES => return Ok(()),
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
-  fn write<W: Write>(
+  fn write_sub_elements_by_ref<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
-    // Write tag + attributes
-    push2write_opt_string_attr!(self, tag, ID);
-    push2write_opt_string_attr!(self, tag, name);
-    push2write_opt_string_attr!(self, tag, ucd);
-    push2write_opt_string_attr!(self, tag, utype);
-    push2write_opt_string_attr!(self, tag, ref_, ref);
-    push2write_opt_tostring_attr!(self, tag, nrows);
-    push2write_extra!(self, tag);
-    writer
-      .write_event(Event::Start(tag.to_borrowed()))
-      .map_err(VOTableError::Write)?;
-    // Write sub-elems
     write_elem!(self, description, writer, context);
     write_elem_vec_no_context!(self, elems, writer);
     write_elem_vec!(self, links, writer, context);
     if let Some(elem) = &mut self.data {
       elem.write(writer, &self.elems)?;
     }
-    // write_elem!(self, data, writer, self.elems);
     write_elem_vec!(self, infos, writer, context);
-    // Close tag
-    writer
-      .write_event(Event::End(tag.to_end()))
-      .map_err(VOTableError::Write)
+    Ok(())
   }
 }
 
 #[cfg(test)]
 mod tests {
   use crate::{
     impls::mem::InMemTableDataRows,
     table::Table,
     tests::{test_read, test_writer},
   };
 
   #[test]
   fn test_table_read_write() {
-    let xml = r#"<TABLE ID="V_147_sdss12" name="V/147/sdss12" nrows="2"><FIELD name="RA_ICRS" datatype="char" ucd="pos.eq.ra;meta.main"></FIELD><FIELD name="RA_ICRS" datatype="char" ucd="pos.eq.ra;meta.main"></FIELD><DATA><TABLEDATA><TR><TD>a</TD><TD>b</TD></TR><TR><TD>a</TD><TD>b</TD></TR></TABLEDATA></DATA></TABLE>"#; // Test read
+    let xml = r#"<TABLE ID="V_147_sdss12" name="V/147/sdss12" nrows="2"><FIELD name="RA_ICRS" datatype="char" ucd="pos.eq.ra;meta.main"/><FIELD name="RA_ICRS" datatype="char" ucd="pos.eq.ra;meta.main"/><DATA><TABLEDATA><TR><TD>a</TD><TD>b</TD></TR><TR><TD>a</TD><TD>b</TD></TR></TABLEDATA></DATA></TABLE>"#; // Test read
     let table = test_read::<Table<InMemTableDataRows>>(xml);
     assert_eq!(table.id.as_ref().unwrap().as_str(), "V_147_sdss12");
     assert_eq!(table.name.as_ref().unwrap().as_str(), "V/147/sdss12");
     assert_eq!(table.nrows, Some(2));
     assert_eq!(table.elems.len(), 2);
     // Test write
     test_writer(table, xml);
```

### Comparing `votable_cli-0.5.0/src/timesys.rs` & `votable_cli-0.6.0/src/timesys.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 //! Module dedicated to the `TIMESYS` tag.
 
 use std::{
   fmt::{self, Debug},
-  io::{BufRead, Write},
   str::{self, FromStr},
 };
 
-use log::warn;
 use paste::paste;
-use quick_xml::{events::attributes::Attributes, Reader, Writer};
 
-use super::{error::VOTableError, QuickXmlReadWrite};
+use super::{error::VOTableError, utils::unexpected_attr_warn, EmptyElem, VOTableElement};
 
+/// Struct corresponding to the `TIMESYS` XML tag.
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct TimeSys {
   #[serde(rename = "ID")]
   pub id: String,
   /// Julian Date in MJD.
   /// * `MJD-origin` = 2400000.5
   /// *  `JD-origin` = 0.0
@@ -33,107 +31,97 @@
       id: id.into(),
       timeorigin: None,
       timescale,
       refposition,
     }
   }
 
-  /// Calls a closure on each (key, value) attribute pairs.
-  pub fn for_each_attribute<F>(&self, mut f: F)
-  where
-    F: FnMut(&str, &str),
-  {
-    f("ID", self.id.as_str());
-    if let Some(timeorigin) = self.timeorigin {
-      f("timeorigin", timeorigin.to_string().as_str());
-    }
-    f("timescale", self.timescale.to_string().as_str());
-    f("refposition", self.refposition.to_string().as_str());
-  }
-
+  impl_builder_mandatory_string_attr!(id);
   impl_builder_opt_attr!(timeorigin, f64);
+  impl_builder_mandatory_attr!(timescale, TimeScale);
+  impl_builder_mandatory_attr!(refposition, RefPosition);
 }
 
-impl QuickXmlReadWrite for TimeSys {
+impl VOTableElement for TimeSys {
   const TAG: &'static str = "TIMESYS";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
+  type MarkerType = EmptyElem;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
     let mut id: Option<String> = None;
     let mut timeorigin: Option<f64> = None;
     let mut timescale: Option<TimeScale> = None;
     let mut refposition: Option<RefPosition> = None;
-    // Look for attributes
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let value =
-        String::from_utf8(attr.value.as_ref().to_vec()).map_err(VOTableError::FromUtf8)?;
-      match attr.key {
-        b"ID" => id = Some(value),
-        b"timeorigin" => timeorigin = Some(value.parse().map_err(VOTableError::ParseFloat)?),
-        b"timescale" => timescale = Some(value.parse().map_err(VOTableError::Variant)?),
-        b"refposition" => refposition = Some(value.parse().map_err(VOTableError::Variant)?),
-        _ => {
-          warn!(
-            "Attribute {:?} in {} is ignored",
-            std::str::from_utf8(attr.key),
-            Self::TAG
-          );
-        }
+    // Look for attributes (especially mandatory attributes)
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "ID" => id = Some(val.into()),
+        "timeorigin" => timeorigin = Some(val.as_ref().parse().map_err(VOTableError::ParseFloat)?),
+        "timescale" => timescale = Some(val.as_ref().parse().map_err(VOTableError::Variant)?),
+        "refposition" => refposition = Some(val.as_ref().parse().map_err(VOTableError::Variant)?),
+        _ => unexpected_attr_warn(key, Self::TAG),
       }
     }
     // Set from found attributes
     if let (Some(id), Some(timescale), Some(refposition)) = (id, timescale, refposition) {
-      let mut timesys = TimeSys::new(id, timescale, refposition);
+      let mut timesys = Self::new(id, timescale, refposition);
       if let Some(timeorigin) = timeorigin {
-        timesys = timesys.set_timeorigin(timeorigin);
+        timesys.set_timeorigin_by_ref(timeorigin);
       }
       Ok(timesys)
     } else {
       Err(VOTableError::Custom(format!(
         "Attributes 'ID', 'timescale' and 'refposition' are mandatory in tag '{}'",
         Self::TAG
       )))
     }
   }
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    _reader: Reader<R>,
-    _reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    unreachable!()
-  }
-
-  fn read_sub_elements_by_ref<R: BufRead>(
-    &mut self,
-    _reader: &mut Reader<R>,
-    _reader_buff: &mut Vec<u8>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    todo!()
-  }
-
-  fn write<W: Write>(
-    &mut self,
-    writer: &mut Writer<W>,
-    _context: &Self::Context,
-  ) -> Result<(), VOTableError> {
-    let mut elem_writer = writer.create_element(Self::TAG_BYTES);
-    elem_writer = elem_writer.with_attribute(("ID", self.id.as_str()));
-    if let Some(timeorigin) = self.timeorigin {
-      elem_writer = elem_writer.with_attribute(("timeorigin", timeorigin.to_string().as_str()));
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key = key.as_ref();
+      match key {
+        "ID" => self.set_id_by_ref(val),
+        "timeorigin" => {
+          self.set_timeorigin_by_ref(val.as_ref().parse().map_err(VOTableError::ParseFloat)?)
+        }
+        "timescale" => {
+          self.set_timescale_by_ref(val.as_ref().parse().map_err(VOTableError::Variant)?)
+        }
+        "refposition" => {
+          self.set_refposition_by_ref(val.as_ref().parse().map_err(VOTableError::Variant)?)
+        }
+        _ => unexpected_attr_warn(key, Self::TAG),
+      }
     }
-    elem_writer = elem_writer.with_attribute(("timescale", self.timescale.to_string().as_str()));
-    elem_writer =
-      elem_writer.with_attribute(("refposition", self.refposition.to_string().as_str()));
-    elem_writer.write_empty().map_err(VOTableError::Write)?;
     Ok(())
   }
+
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    f("ID", self.id.as_str());
+    if let Some(timeorigin) = self.timeorigin {
+      f("timeorigin", timeorigin.to_string().as_str());
+    }
+    f("timescale", self.timescale.to_string().as_str());
+    f("refposition", self.refposition.to_string().as_str());
+  }
 }
 
 pub struct Info {
   pub label: &'static str,
   pub description: &'static str,
 }
 
@@ -175,15 +163,14 @@
                                  "Runs slower than TCB at a constant rate so as to remain approximately in step with TT. Therefore runs quasi-synchronously with TT, except for the relativistic effects introduced by variations in the Earth's velocity relative to the barycenter.",
 );
 const UNKNOWN_TIMESCALE_INFO: Info = Info::new("Unknown or unavailable timescale",
                                                "This value indicates clients cannot transform the times reliably. This is to be used for simulated data, free-running clocks, or data for which information on the time scale has been lost.",
 );
 
 /// See the [IVOA timescale vocabulary](https://www.ivoa.net/rdf/timescale/2019-03-15/timescale.html)
-// #[serde(tag = "timescale")]
 #[derive(Clone, PartialEq, Eq, Debug, serde::Serialize, serde::Deserialize)]
 pub enum TimeScale {
   TAI,
   TT,
   UT,
   UTC,
   GPS,
@@ -226,27 +213,14 @@
       _ => Err(format!("Unknown timescale variant. Actual: '{}'.", s)),
     }
   }
 }
 
 impl fmt::Display for TimeScale {
   fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
-    /*write!(f, "{}",
-           match self {
-             TimeScale::TAI => "tai",
-             TimeScale::TT => "tt",
-             TimeScale::UT => "ut",
-             TimeScale::UTC => "utc",
-             TimeScale::GPS => "gps",
-             TimeScale::TCG => "tcg",
-             TimeScale::TCB => "tcb",
-             TimeScale::TDB => "tdb",
-             TimeScale::UNKNOWN => "unknown"
-           }
-    )*/
     Debug::fmt(self, f)
   }
 }
 
 const TOPOCENTER_INFO: Info = Info::new(
   "Topocenter",
   "The location of the instrument that made the observation",
@@ -305,50 +279,40 @@
       _ => Err(format!("Unknown 'refposition' variant. Actual: '{}'.", s)),
     }
   }
 }
 
 impl fmt::Display for RefPosition {
   fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
-    /*write!(f, "{}",
-           match self {
-             RefPosition::TOPOCENTER => "topocenter",
-             RefPosition::GEOCENTER => "geocenter",
-             RefPosition::BARYCENTER => "barycenter",
-             RefPosition::HELIOCENTER => "heliocenter",
-             RefPosition::EMBARYCENTER => "embarycenter",
-             RefPosition::UNKNOWN => "unknown"
-           }
-    )*/
     Debug::fmt(self, f)
   }
 }
 
 #[cfg(test)]
 mod tests {
   use std::io::Cursor;
 
   use quick_xml::{events::Event, Reader, Writer};
 
   use crate::{
     timesys::{RefPosition, TimeScale, TimeSys},
-    QuickXmlReadWrite,
+    QuickXmlReadWrite, VOTableElement,
   };
 
   #[test]
   fn test_timesys_readwrite() {
     let xml = r#"<TIMESYS ID="time_frame" timeorigin="2455197.5" timescale="TCB" refposition="BARYCENTER"/>"#;
     // Test read
     let mut reader = Reader::from_reader(Cursor::new(xml.as_bytes()));
     let mut buff: Vec<u8> = Vec::with_capacity(xml.len());
     let mut timesys = loop {
       let mut event = reader.read_event(&mut buff).unwrap();
       match &mut event {
         Event::Empty(ref mut e) if e.local_name() == TimeSys::TAG_BYTES => {
-          let timesys = TimeSys::from_attributes(e.attributes()).unwrap();
+          let timesys = TimeSys::from_event_empty(e).unwrap();
           assert_eq!(timesys.id, "time_frame");
           assert_eq!(timesys.timeorigin, Some(2455197.5));
           assert_eq!(timesys.timescale, TimeScale::TCB);
           assert_eq!(timesys.refposition, RefPosition::BARYCENTER);
           break timesys;
         }
         Event::Text(ref mut e) if e.escaped().is_empty() => (), // First even read
```

### Comparing `votable_cli-0.5.0/src/utils.rs` & `votable_cli-0.6.0/src/utils.rs`

 * *Files 24% similar despite different names*

```diff
@@ -27,7 +27,19 @@
 pub(crate) fn discard_event(event: Event, tag: &str) {
   debug!("Discarded event in tag {}: {:?}", tag, event)
 }
 
 pub(crate) fn unexpected_event(event: Event, tag: &str) -> VOTableError {
   VOTableError::Custom(format!("Unexpected event in tag {}: {:?}", tag, event))
 }
+
+pub(crate) fn unexpected_attr_warn(attr_key: &str, tag: &str) {
+  warn!(
+    "Unexpected attribute in tag {}: '{:?}' is discarded",
+    tag, attr_key
+  )
+}
+
+#[cfg(feature = "mivot")]
+pub(crate) fn unexpected_attr_err(attr_key: &str, tag: &'static str) -> VOTableError {
+  VOTableError::UnexpectedAttr(attr_key.as_bytes().to_vec(), tag)
+}
```

### Comparing `votable_cli-0.5.0/src/votable.rs` & `votable_cli-0.6.0/src/votable.rs`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 };
 
 use log::{debug, warn};
 use paste::paste;
 use serde::{Deserialize, Serialize};
 use serde_json::Value;
 
-// Re-export the quick_xml elements
+// Re-export the quick_xml elements;
 pub use quick_xml::{
   events::{attributes::Attributes, BytesDecl, BytesEnd, BytesStart, Event},
   Reader, Writer,
 };
 
 use super::{
   coosys::CooSys,
@@ -28,15 +28,15 @@
   group::Group,
   info::Info,
   param::Param,
   resource::Resource,
   table::Table,
   timesys::TimeSys,
   utils::{discard_comment, discard_event, is_empty},
-  QuickXmlReadWrite, TableDataContent, VOTableVisitor,
+  HasSubElements, HasSubElems, QuickXmlReadWrite, TableDataContent, VOTableElement, VOTableVisitor,
 };
 
 pub fn new_xml_writer<W: Write>(
   writer: W,
   indent_char: Option<u8>,
   indent_size: Option<usize>,
 ) -> Writer<W> {
@@ -128,40 +128,37 @@
 #[serde(tag = "elem_type")]
 pub enum VOTableElem {
   CooSys(CooSys),
   TimeSys(TimeSys),
   Group(Group),
   Param(Param),
   Info(Info),
-  Definitions(Definitions), // Deprecated since v1.1
 }
 
 impl VOTableElem {
   pub fn visit<C, V>(&mut self, visitor: &mut V) -> Result<(), V::E>
   where
     C: TableDataContent,
     V: VOTableVisitor<C>,
   {
     match self {
       VOTableElem::CooSys(elem) => elem.visit(visitor),
       VOTableElem::TimeSys(elem) => visitor.visit_timesys(elem),
       VOTableElem::Group(elem) => elem.visit(visitor),
       VOTableElem::Param(elem) => elem.visit(visitor),
       VOTableElem::Info(elem) => visitor.visit_info(elem),
-      VOTableElem::Definitions(elem) => elem.visit(visitor),
     }
   }
   fn write<W: Write>(&mut self, writer: &mut Writer<W>) -> Result<(), VOTableError> {
     match self {
       VOTableElem::CooSys(elem) => elem.write(writer, &()),
       VOTableElem::TimeSys(elem) => elem.write(writer, &()),
       VOTableElem::Group(elem) => elem.write(writer, &()),
       VOTableElem::Param(elem) => elem.write(writer, &()),
       VOTableElem::Info(elem) => elem.write(writer, &()),
-      VOTableElem::Definitions(elem) => elem.write(writer, &()),
     }
   }
 }
 
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct VOTableWrapper<C: TableDataContent> {
   pub votable: VOTable<C>,
@@ -245,15 +242,22 @@
     let mut votable: Vec<u8> = Vec::new();
     self.to_ivoa_xml_writer(&mut votable)?;
     Ok(votable)
   }
 
   pub fn to_ivoa_xml_writer<W: Write>(&mut self, write: W) -> Result<(), VOTableError> {
     let mut write = Writer::new_with_indent(write, b' ', 4);
-    self.votable.write(&mut write, &())
+    write
+      .write(
+        r#"<?xml version="1.0" encoding="UTF-8"?>
+"#
+        .as_bytes(),
+      )
+      .map_err(VOTableError::Write)
+      .and_then(|()| self.votable.write(&mut write, &()))
   }
 }
 
 impl<C> VOTableWrapper<C>
 where
   C: TableDataContent + Serialize + for<'a> Deserialize<'a>,
 {
@@ -426,14 +430,15 @@
     pretty: bool,
   ) -> Result<(), VOTableError> {
     let bytes = self.to_toml_bytes(pretty)?;
     write.write_all(bytes.as_slice()).map_err(VOTableError::Io)
   }
 }
 
+/// Struct corresponding to the `VOTABLE` XML tag.
 #[derive(Clone, Debug, PartialEq, serde::Serialize, serde::Deserialize)]
 pub struct VOTable<C: TableDataContent> {
   // attributes
   #[serde(rename = "ID", skip_serializing_if = "Option::is_none")]
   pub id: Option<String>,
   pub version: Version,
   /// E.g. "http://www.ivoa.net/xml/VOTable/v1.3", see method in the `Version` enum.
@@ -446,14 +451,17 @@
   pub xsi_schema_location: Option<String>,
   // extra attributes
   #[serde(flatten, skip_serializing_if = "HashMap::is_empty")]
   pub extra: HashMap<String, Value>,
   // elements
   #[serde(skip_serializing_if = "Option::is_none")]
   pub description: Option<Description>,
+  #[serde(skip_serializing_if = "Option::is_none")]
+  /// `DEFINITIONS` is deprecated since VOTable 1.1
+  pub definitions: Option<Definitions>,
   #[serde(default, skip_serializing_if = "Vec::is_empty")]
   pub elems: Vec<VOTableElem>,
   #[serde(skip_serializing_if = "Vec::is_empty")]
   pub resources: Vec<Resource<C>>,
   #[serde(default, skip_serializing_if = "Vec::is_empty")]
   pub post_infos: Vec<Info>,
 }
@@ -488,14 +496,15 @@
       id: None,
       version,
       xmlns,
       xmlns_xsi: None,
       xsi_schema_location: None,
       extra: Default::default(),
       description: None,
+      definitions: None,
       elems: Default::default(),
       resources: Default::default(),
       post_infos: Default::default(),
     }
   }
 
   /// Create a new VOTable implementing the given `Version` and containing the given `Resource`.
@@ -514,14 +523,17 @@
   }
 
   pub fn visit<V: VOTableVisitor<C>>(&mut self, visitor: &mut V) -> Result<(), V::E> {
     visitor.visit_votable_start(self)?;
     if let Some(desc) = &mut self.description {
       visitor.visit_description(desc)?;
     }
+    if let Some(e) = &mut self.definitions {
+      e.visit(visitor)?;
+    }
     for e in self.elems.iter_mut() {
       e.visit(visitor)?;
     }
     for r in self.resources.iter_mut() {
       r.visit(visitor)?;
     }
     for i in self.post_infos.iter_mut() {
@@ -534,18 +546,17 @@
     let mut reader = Reader::from_reader(reader);
     let mut buff: Vec<u8> = Vec::with_capacity(1024);
     loop {
       let mut event = reader.read_event(&mut buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Decl(ref e) => check_declaration(e),
         Event::Start(ref mut e) if e.local_name() == VOTable::<C>::TAG_BYTES => {
-          let mut votable = VOTable::<C>::from_attributes(e.attributes())?;
-          votable.read_sub_elements_and_clean(reader, &mut buff, &())?;
-          // ignore the remaining of the reader !
-          return Ok(votable);
+          // Ignore the remaining of the reader !
+          return VOTable::<C>::from_event_start(e)
+            .and_then(|vot| vot.read_content(&mut reader, &mut buff, &()));
         }
         Event::Text(e) if is_empty(e) => {}
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
@@ -558,52 +569,57 @@
   ) -> Result<(VOTable<C>, Resource<C>, Reader<R>), VOTableError> {
     let mut reader = Reader::from_reader(reader);
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Decl(ref e) => check_declaration(e),
         Event::Start(ref mut e) if e.local_name() == VOTable::<C>::TAG_BYTES => {
-          let mut votable = VOTable::<C>::from_attributes(e.attributes())?;
-          let (resource, reader) = votable.read_till_next_resource(reader, reader_buff)?;
-          reader_buff.clear();
-          return Ok((votable, resource, reader));
+          return VOTable::<C>::from_event_start(e).and_then(|mut votable| {
+            votable
+              .read_till_next_resource(reader, reader_buff)
+              .map(|(resource, reader)| {
+                reader_buff.clear();
+                (votable, resource, reader)
+              })
+          });
         }
         Event::Text(e) if is_empty(e) => {}
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
   impl_builder_opt_string_attr!(id);
-
   impl_builder_mandatory_attr!(version, Version);
   impl_builder_mandatory_string_attr!(xmlns);
   impl_builder_opt_string_attr!(xmlns_xsi);
   impl_builder_opt_string_attr!(xsi_schema_location);
 
   impl_builder_insert_extra!();
 
-  impl_builder_opt_attr!(description, Description);
+  impl_builder_opt_subelem!(description, Description);
+  impl_builder_opt_subelem!(definitions, Definitions);
 
   impl_builder_push_elem!(CooSys, VOTableElem);
   impl_builder_push_elem!(TimeSys, VOTableElem);
   impl_builder_push_elem!(Group, VOTableElem);
   impl_builder_push_elem!(Param, VOTableElem);
   impl_builder_push_elem!(Info, VOTableElem);
-  impl_builder_push_elem!(Definitions, VOTableElem);
+
   pub fn push_elem(mut self, elem: VOTableElem) -> Self {
     self.push_elem_by_ref(elem);
     self
   }
   pub fn push_elem_by_ref(&mut self, elem: VOTableElem) {
     self.elems.push(elem);
   }
 
   impl_builder_push!(Resource, C);
+  impl_builder_prepend!(Resource, C);
 
   impl_builder_push_post_info!();
 
   /// Transforms the BINARY or BINARY2 tag in this VOTABLE into TABLEDATA.
   /// Do nothing if it already contains a TABLEDATA or if it contains a FITS.
   pub fn to_tabledata(&mut self) -> Result<(), VOTableError> {
     for resource in self.resources.iter_mut() {
@@ -682,62 +698,50 @@
     // If the full document is in memory, we could have use a Reader<'a [u8]> and then the method
     // `read_event_unbuffered` to avoid a copy.
     // But are more generic that this to be able to read in streaming mode
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          Description::TAG_BYTES => {
-            from_event_start_desc_by_ref!(self, Description, reader, reader_buff, e)
+          Description::TAG_BYTES => set_desc_from_event_start!(self, reader, reader_buff, e),
+          Definitions::TAG_BYTES => {
+            set_from_event_start!(self, Definitions, reader, reader_buff, e)
+          }
+          Info::TAG_BYTES if self.resources.is_empty() => {
+            push_from_event_start!(self, Info, reader, reader_buff, e)
           }
-          Info::TAG_BYTES if self.resources.is_empty() => self.elems.push(VOTableElem::Info(
-            from_event_start_by_ref!(Info, reader, reader_buff, e),
-          )),
-          Group::TAG_BYTES => self.elems.push(VOTableElem::Group(from_event_start_by_ref!(
-            Group,
-            reader,
-            reader_buff,
-            e
-          ))),
-          Param::TAG_BYTES => self.elems.push(VOTableElem::Param(from_event_start_by_ref!(
-            Param,
-            reader,
-            reader_buff,
-            e
-          ))),
+          Group::TAG_BYTES => push_from_event_start!(self, Group, reader, reader_buff, e),
+          Param::TAG_BYTES => push_from_event_start!(self, Param, reader, reader_buff, e),
           Resource::<C>::TAG_BYTES => {
-            let resource = Resource::<C>::from_attributes(e.attributes())?;
-            return Ok(Some(resource));
+            return Resource::<C>::from_event_start(e).map(Some);
           }
           Info::TAG_BYTES => {
-            self
-              .post_infos
-              .push(from_event_start_by_ref!(Info, reader, reader_buff, e))
+            self.push_post_info_by_ref(from_event_start_by_ref!(Info, reader, reader_buff, e))
           }
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
+          Definitions::TAG_BYTES => set_from_event_empty!(self, Definitions, e),
           Info::TAG_BYTES => {
             let info = Info::from_event_empty(e)?;
             if self.resources.is_empty() {
               self.push_info_by_ref(info);
             } else {
               self.push_post_info_by_ref(info);
             }
           }
-          CooSys::TAG_BYTES => self.push_coosys_by_ref(CooSys::from_event_empty(e)?),
-          TimeSys::TAG_BYTES => self.push_timesys_by_ref(TimeSys::from_event_empty(e)?),
-          Group::TAG_BYTES => self.push_group_by_ref(Group::from_event_empty(e)?),
-          Param::TAG_BYTES => self.push_param_by_ref(Param::from_event_empty(e)?),
-          Definitions::TAG_BYTES => self.push_definitions_by_ref(Definitions::from_event_empty(e)?),
+          CooSys::TAG_BYTES => push_from_event_empty!(self, CooSys, e),
+          TimeSys::TAG_BYTES => push_from_event_empty!(self, TimeSys, e),
+          Group::TAG_BYTES => push_from_event_empty!(self, Group, e),
+          Param::TAG_BYTES => push_from_event_empty!(self, Param, e),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
@@ -800,25 +804,21 @@
         r#"<?xml version="1.0" encoding="UTF-8"?>
 "#
         .as_bytes(),
       )
       .map_err(VOTableError::Write)?;
     let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
     // Write tag + attributes
-    push2write_opt_string_attr!(self, tag, ID);
-    push2write_mandatory_into_attr!(self, tag, version);
-    push2write_mandatory_string_attr!(self, tag, xmlns);
-    push2write_opt_string_attr!(self, tag, xmlns_xsi);
-    push2write_opt_string_attr!(self, tag, xsi_schema_location);
-    push2write_extra!(self, tag);
+    self.for_each_attribute(|k, v| tag.push_attribute((k, v)));
     writer
       .write_event(Event::Start(tag.to_borrowed()))
       .map_err(VOTableError::Write)?;
     // Write sub-elems
     write_elem!(self, description, writer, context);
+    write_elem!(self, definitions, writer, context);
     write_elem_vec_no_context!(self, elems, writer);
     for resource in self.resources.iter_mut() {
       if resource.write_to_data_beginning(writer, &(), stop_before_data)? {
         return Ok(true);
       }
     }
     // Reach this point only if no table has been found
@@ -878,51 +878,73 @@
     .unwrap_or_else(|| String::from("error"));
   debug!(
     "XML declaration. Version: {}; Encoding: {}; Standalone: {}.",
     version, encoding, standalone
   );
 }
 
-impl<C: TableDataContent> QuickXmlReadWrite for VOTable<C> {
+impl<C: TableDataContent> VOTableElement for VOTable<C> {
   const TAG: &'static str = "VOTABLE";
-  type Context = ();
 
-  fn from_attributes(attrs: Attributes) -> Result<Self, VOTableError> {
-    let mut votable = Self::new_empty(Version::V1_4);
-    for attr_res in attrs {
-      let attr = attr_res.map_err(VOTableError::Attr)?;
-      let unescaped = attr.unescaped_value().map_err(VOTableError::Read)?;
-      let value = str::from_utf8(unescaped.as_ref()).map_err(VOTableError::Utf8)?;
-      match attr.key {
-        b"ID" => votable.set_id_by_ref(value),
-        b"version" => {
-          votable.set_version_by_ref(Version::from_str(value).map_err(VOTableError::Custom)?)
-        }
-        b"xmlns" => votable.set_xmlns_by_ref(value.to_string()),
-        b"xmlns:xsi" => votable.set_xmlns_xsi_by_ref(value.to_string()),
-        b"xsi:schemaLocation" => votable.set_xsi_schema_location_by_ref(value.to_string()),
-        _ => votable.insert_extra_by_ref(
-          str::from_utf8(attr.key).map_err(VOTableError::Utf8)?,
-          Value::String(value.into()),
-        ),
+  type MarkerType = HasSubElems;
+
+  fn from_attrs<K, V, I>(attrs: I) -> Result<Self, VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    Self::new_empty(Version::V1_4).set_attrs(attrs)
+  }
+
+  fn set_attrs_by_ref<K, V, I>(&mut self, attrs: I) -> Result<(), VOTableError>
+  where
+    K: AsRef<str> + Into<String>,
+    V: AsRef<str> + Into<String>,
+    I: Iterator<Item = (K, V)>,
+  {
+    for (key, val) in attrs {
+      let key_str = key.as_ref();
+      match key_str {
+        "ID" => self.set_id_by_ref(val),
+        "version" => self.set_version_by_ref(val.as_ref().parse().map_err(VOTableError::Custom)?),
+        "xmlns" => self.set_xmlns_by_ref(val),
+        "xmlns:xsi" => self.set_xmlns_xsi_by_ref(val),
+        "xsi:schemaLocation" => self.set_xsi_schema_location_by_ref(val),
+        _ => self.insert_extra_str_by_ref(key, val),
       }
     }
+    Ok(())
+  }
 
-    Ok(votable)
+  fn for_each_attribute<F>(&self, mut f: F)
+  where
+    F: FnMut(&str, &str),
+  {
+    if let Some(id) = &self.id {
+      f("ID", id.as_str());
+    }
+    f("version", (&self.version).into());
+    f("xmlns", self.xmlns.as_str());
+    if let Some(xmlns_xsi) = &self.xmlns_xsi {
+      f("xmlns:xsi", xmlns_xsi.as_str());
+    }
+    if let Some(xsi_schema_location) = &self.xsi_schema_location {
+      f("xsi:schemaLocation", xsi_schema_location.as_str());
+    }
+    for_each_extra_attribute!(self, f);
   }
+}
 
-  fn read_sub_elements<R: BufRead>(
-    &mut self,
-    mut reader: Reader<R>,
-    reader_buff: &mut Vec<u8>,
-    context: &Self::Context,
-  ) -> Result<Reader<R>, VOTableError> {
-    self
-      .read_sub_elements_by_ref(&mut reader, reader_buff, context)
-      .map(|()| reader)
+impl<C: TableDataContent> HasSubElements for VOTable<C> {
+  type Context = ();
+
+  fn has_no_sub_elements(&self) -> bool {
+    // Must contain at least one resource
+    false
   }
 
   fn read_sub_elements_by_ref<R: BufRead>(
     &mut self,
     mut reader: &mut Reader<R>,
     mut reader_buff: &mut Vec<u8>,
     _context: &Self::Context,
@@ -930,73 +952,50 @@
     // If the full document is in memory, we could have use a Reader<'a [u8]> and then the method
     // `read_event_unbuffered` to avoid a copy.
     // But are more generic that this to be able to read in streaming mode
     loop {
       let mut event = reader.read_event(reader_buff).map_err(VOTableError::Read)?;
       match &mut event {
         Event::Start(ref e) => match e.local_name() {
-          Description::TAG_BYTES => {
-            from_event_start_desc_by_ref!(self, Description, reader, reader_buff, e)
-          }
-          Info::TAG_BYTES if self.resources.is_empty() => self.elems.push(VOTableElem::Info(
-            from_event_start_by_ref!(Info, reader, reader_buff, e),
-          )),
-          Group::TAG_BYTES => self.elems.push(VOTableElem::Group(from_event_start_by_ref!(
-            Group,
-            reader,
-            reader_buff,
-            e
-          ))),
-          Param::TAG_BYTES => self.elems.push(VOTableElem::Param(from_event_start_by_ref!(
-            Param,
-            reader,
-            reader_buff,
-            e
-          ))),
+          Description::TAG_BYTES => set_desc_from_event_start!(self, reader, reader_buff, e),
           Definitions::TAG_BYTES => {
-            self
-              .elems
-              .push(VOTableElem::Definitions(from_event_start_by_ref!(
-                Definitions,
-                reader,
-                reader_buff,
-                e
-              )))
+            set_from_event_start!(self, Definitions, reader, reader_buff, e)
           }
+          Info::TAG_BYTES if self.resources.is_empty() => {
+            push_from_event_start!(self, Info, reader, reader_buff, e)
+          }
+          Group::TAG_BYTES => push_from_event_start!(self, Group, reader, reader_buff, e),
+          Param::TAG_BYTES => push_from_event_start!(self, Param, reader, reader_buff, e),
           Resource::<C>::TAG_BYTES => {
-            self
-              .resources
-              .push(from_event_start_by_ref!(Resource, reader, reader_buff, e))
+            self.push_resource_by_ref(from_event_start_by_ref!(Resource, reader, reader_buff, e))
           }
           Info::TAG_BYTES => {
-            self
-              .post_infos
-              .push(from_event_start_by_ref!(Info, reader, reader_buff, e))
+            self.push_post_info_by_ref(from_event_start_by_ref!(Info, reader, reader_buff, e))
           }
           _ => {
             return Err(VOTableError::UnexpectedStartTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
         Event::Empty(ref e) => match e.local_name() {
+          Definitions::TAG_BYTES => set_from_event_empty!(self, Definitions, e),
           Info::TAG_BYTES => {
             let info = Info::from_event_empty(e)?;
             if self.resources.is_empty() {
               self.push_info_by_ref(info);
             } else {
               self.push_post_info_by_ref(info);
             }
           }
-          CooSys::TAG_BYTES => self.push_coosys_by_ref(CooSys::from_event_empty(e)?),
-          TimeSys::TAG_BYTES => self.push_timesys_by_ref(TimeSys::from_event_empty(e)?),
-          Group::TAG_BYTES => self.push_group_by_ref(Group::from_event_empty(e)?),
-          Param::TAG_BYTES => self.push_param_by_ref(Param::from_event_empty(e)?),
-          Definitions::TAG_BYTES => self.push_definitions_by_ref(Definitions::from_event_empty(e)?),
+          CooSys::TAG_BYTES => push_from_event_empty!(self, CooSys, e),
+          TimeSys::TAG_BYTES => push_from_event_empty!(self, TimeSys, e),
+          Group::TAG_BYTES => push_from_event_empty!(self, Group, e),
+          Param::TAG_BYTES => push_from_event_empty!(self, Param, e),
           _ => {
             return Err(VOTableError::UnexpectedEmptyTag(
               e.local_name().to_vec(),
               Self::TAG,
             ))
           }
         },
@@ -1013,48 +1012,53 @@
         Event::Eof => return Err(VOTableError::PrematureEOF(Self::TAG)),
         Event::Comment(e) => discard_comment(e, reader, Self::TAG),
         _ => discard_event(event, Self::TAG),
       }
     }
   }
 
+  fn write_sub_elements_by_ref<W: Write>(
+    &mut self,
+    writer: &mut Writer<W>,
+    context: &Self::Context,
+  ) -> Result<(), VOTableError> {
+    write_elem!(self, description, writer, context);
+    write_elem!(self, definitions, writer, context);
+    write_elem_vec_no_context!(self, elems, writer);
+    write_elem_vec!(self, resources, writer, context);
+    write_elem_vec!(self, post_infos, writer, context);
+    Ok(())
+  }
+}
+
+/*
+impl<C: TableDataContent> QuickXmlReadWrite<HasSubElems> for VOTable<C> {
+  type Context = ();
+
   fn write<W: Write>(
     &mut self,
     writer: &mut Writer<W>,
     context: &Self::Context,
   ) -> Result<(), VOTableError> {
-    writer
-      .write(
-        r#"<?xml version="1.0" encoding="UTF-8"?>
-"#
-        .as_bytes(),
-      )
-      .map_err(VOTableError::Write)?;
+    // We do not use the 'default' write impleemntation because of this first line.
+
     let mut tag = BytesStart::borrowed_name(Self::TAG_BYTES);
     // Write tag + attributes
-    push2write_opt_string_attr!(self, tag, ID);
-    push2write_mandatory_into_attr!(self, tag, version);
-    push2write_mandatory_string_attr!(self, tag, xmlns);
-    push2write_opt_string_attr!(self, tag, xmlns_xsi);
-    push2write_opt_string_attr!(self, tag, xsi_schema_location);
-    push2write_extra!(self, tag);
+    self.for_each_attribute(|k, v| tag.push_attribute((k, v)));
     writer
       .write_event(Event::Start(tag.to_borrowed()))
       .map_err(VOTableError::Write)?;
     // Write sub-elems
-    write_elem!(self, description, writer, context);
-    write_elem_vec_no_context!(self, elems, writer);
-    write_elem_vec!(self, resources, writer, context);
-    write_elem_vec!(self, post_infos, writer, context);
+    self.write_sub_elements_by_ref(writer, context)?;
     // Close tag
     writer
       .write_event(Event::End(tag.to_end()))
       .map_err(VOTableError::Write)
   }
-}
+}*/
 
 #[cfg(test)]
 mod tests {
   use crate::votable::VOTableWrapper;
   use crate::{
     impls::mem::{InMemTableDataRows, InMemTableDataStringRows},
     QuickXmlReadWrite,
```

### Comparing `votable_cli-0.5.0/crates/cli/Cargo.toml` & `votable_cli-0.6.0/crates/cli/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "votable-cli"
-version = "0.5.0"
+version = "0.6.0"
 authors = ["F.-X. Pineau <francois-xavier.pineau@astro.unistra.fr>"]
 description = "Command-line to extract information from IVOA VOTables and to convert VOTable  back and forth in XML, JSON, YAML, TOML (and to CSV) while preserving all elements (except in CSV)."
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 categories = ["command-line-utilities", "science", "data-structures"]
 keywords = ["ivoa", "votable", "xml"]
 documentation = "https://github.com/cds-astro/cds-votable-rust/tree/main/crates/cli"
@@ -19,15 +19,15 @@
 name = "vot"
 bench = false
 test = false
 
 [dependencies]
 votable = { package = "votable", path = "../..", features = ["mivot"] }
 clap = { version = "4.5", features = ["derive"] }
-log = "0.4"
+log = { version = "0.4", features = ["max_level_trace", "release_max_level_trace"] }
 env_logger = "0.11"
 crossbeam = "0.8"
 serde = "1.0"
 
 
 [features]
 default = []
```

### Comparing `votable_cli-0.5.0/crates/cli/CHANGELOG.md` & `votable_cli-0.6.0/crates/cli/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # `moc-cli` Change Log
 
+## 0.6.0
+
+Released 2023-04-05
+
+* Add sub-command 'edit' to modify a VOTable
+
+
 ## 0.5.0
 
 Released 2023-03-11
 
 * ⚠️  BREAKING: new options and hence new command layout
 * Add the 'convert' sub-command, and conversion from XML to CSV
 * Add the 'sconvert' sub-command for streaming conversion
```

### Comparing `votable_cli-0.5.0/crates/cli/LICENSE-APACHE` & `votable_cli-0.6.0/crates/cli/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/crates/cli/LICENSE-MIT` & `votable_cli-0.6.0/crates/cli/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/crates/cli/src/get.rs` & `votable_cli-0.6.0/crates/cli/src/get.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,32 +11,34 @@
 use super::{
   input::Input,
   visitors::{
     colnames::ColnamesVisitor, fieldarray::FieldArrayVisitor, votstruct::AsciiStructVisitor,
   },
 };
 
-/// Get information from a VOTable (sstreaming for XML files).
+/// Get information from a VOTable, like it structure or fields.
 #[derive(Debug, Args)]
 pub struct Get {
   #[command(flatten)]
   input: Input,
   /// Stop parsing before reading first data ('xml' input only).
   #[arg(short = 's', long = "early-stop")]
   stop_at_first_data: bool,
   #[command(subcommand)]
   action: GetAction,
 }
 impl Get {
   pub fn exec(self) -> Result<(), VOTableError> {
-    if self.input.get_fmt()?.is_xml() {
-      self.exec_streaming()
-    } else {
-      self.exec_in_mem()
-    }
+    self.input.is_streamable().and_then(|is_streamable| {
+      if is_streamable {
+        self.exec_streaming()
+      } else {
+        self.exec_in_mem()
+      }
+    })
   }
 
   /// Exec loading the full VOTable in memory in case of JSON/YAML/TOML
   pub fn exec_in_mem(self) -> Result<(), VOTableError> {
     self
       .input
       .load()
@@ -67,15 +69,15 @@
       .and_then(|vot| self.action.exec(vot))
     }
   }
 }
 
 #[derive(Debug, Subcommand)]
 enum GetAction {
-  /// Print the VOTable structure
+  /// Print the VOTable structure (useful to get Virtual IDs)
   Struct {
     /// Output line width (min=80)
     #[arg(short = 'w', long = "line-width", default_value = "120")]
     line_width: usize,
     /// Smaller possible size of 'content=xxx' when trying to fit on a single line.
     /// If larger, put on a new line (max=50% of line width)
     #[arg(short = 'c', long = "content-size-min", default_value = "30")]
```

### Comparing `votable_cli-0.5.0/crates/cli/src/input.rs` & `votable_cli-0.6.0/crates/cli/src/input.rs`

 * *Files 11% similar despite different names*

```diff
@@ -71,14 +71,18 @@
 }
 
 impl Input {
   pub fn is_stdin(&self) -> bool {
     self.input.is_none()
   }
 
+  pub fn is_streamable(&self) -> Result<bool, VOTableError> {
+    self.get_fmt().map(|f| f.is_xml())
+  }
+
   pub fn get_fmt(&self) -> Result<InputFormat, VOTableError> {
     match &self.input_fmt {
       Some(input_fmt) => Ok(*input_fmt),
       None => match &self.input {
         Some(path) => InputFormat::from_extension(path).map_err(VOTableError::Custom),
         None => Err(VOTableError::Custom(String::from(
           "Input format **must** be provided when reading from stdin.",
```

### Comparing `votable_cli-0.5.0/crates/cli/src/main.rs` & `votable_cli-0.6.0/crates/cli/src/main.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,41 @@
+use std::io::{stderr, stdout, Write};
+
 use clap::Parser;
 
 use votable::error::VOTableError;
-use votable_cli::{convert::Convert, get::Get, streaming::StreamConvert /*update::Update*/};
+use votable_cli::{convert::Convert, edit::Edit, get::Get, streaming::StreamConvert};
 
 #[derive(Debug, Parser)]
 #[clap(author, version, about, long_about = None)]
 pub enum CliArgs {
   Convert(Convert),
+  #[command(verbatim_doc_comment)]
   Sconvert(StreamConvert),
-  // Update(Update),
+  Edit(Edit),
   Get(Get),
 }
 
 impl CliArgs {
   pub fn exec(self) -> Result<(), VOTableError> {
     match self {
       Self::Convert(p) => p.exec(),
       Self::Sconvert(p) => p.exec(),
-      // Self::Update(p) => p.exec(),
+      Self::Edit(p) => p.exec(),
       Self::Get(p) => p.exec(),
     }
   }
 }
 
 fn main() -> Result<(), VOTableError> {
   let args = CliArgs::parse();
   env_logger::init();
-  args.exec()
+  args.exec().map_err(|e| {
+    if let Err(e) = stdout().flush() {
+      eprintln!("Error flushing stdout: {:?}", e);
+    }
+    if let Err(e) = stderr().flush() {
+      eprintln!("Error flushing stderr: {:?}", e);
+    }
+    e
+  })
 }
```

### Comparing `votable_cli-0.5.0/crates/cli/src/output.rs` & `votable_cli-0.6.0/crates/cli/src/output.rs`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,20 @@
         "Unrecognized format. Actual: '{}'. Expected: 'xml', 'xml-td', 'xml-bin', 'xml-bin2', 'json', 'yaml' or 'toml'",
         s
       )),
     }
   }
 }
 impl OutputFormat {
+  pub fn is_streamable(&self) -> bool {
+    match self {
+      Self::Xml | Self::XmlTabledata | Self::XmlBinary | Self::XmlBinary2 => true,
+      _ => false,
+    }
+  }
   fn put<W: Write>(
     self,
     mut vot: VOTableWrapper<InMemTableDataRows>,
     writer: W,
     pretty: bool,
   ) -> Result<(), VOTableError> {
     match self {
@@ -66,24 +72,28 @@
   }
 }
 
 #[derive(Debug, Args)]
 pub struct Output {
   /// Path of the output VOTable [default: write to stdout]
   #[clap(short = 'o', long = "out", value_name = "FILE")]
-  output: Option<PathBuf>,
+  pub output: Option<PathBuf>,
   /// Format of the output VOTable ('xml', 'xml-td', 'xml-bin', 'xml-bin2', 'json', 'yaml' or 'toml').
   #[clap(short = 'f', long = "out-fmt", value_enum)]
-  output_fmt: OutputFormat,
+  pub output_fmt: OutputFormat,
   /// Pretty print (for JSON and TOML)
   #[clap(short, long)]
-  pretty: bool,
+  pub pretty: bool,
 }
 
 impl Output {
+  pub fn is_streamable(&self) -> bool {
+    self.output_fmt.is_streamable()
+  }
+
   pub fn save(&self, vot: VOTableWrapper<InMemTableDataRows>) -> Result<(), VOTableError> {
     match &self.output {
       Some(path) => {
         let file = File::create(path).map_err(VOTableError::Io)?;
         let write = BufWriter::new(file);
         self.output_fmt.put(vot, write, self.pretty)
       }
```

### Comparing `votable_cli-0.5.0/crates/cli/src/streaming.rs` & `votable_cli-0.6.0/crates/cli/src/streaming.rs`

 * *Files 0% similar despite different names*

```diff
@@ -49,17 +49,16 @@
         "Unrecognized format. Actual: '{}'. Expected: 'xml-td', 'xml-bin', 'xml-bin2', or 'csv'",
         s
       )),
     }
   }
 }
 
-/// Convert a (large) single table VOTable in streaming mode.
-/// All information is preserved, even after the `</TABLE>` tag.
-/// The `TABLEDATA` to `CSV` conversion preserve fields formatting.
+/// Convert a single table XML VOTable in streaming mode.
+/// Tags after `</TABLE>` are preserved.
 #[derive(Debug, Args)]
 pub struct StreamConvert {
   /// Path of the input XML VOTable [default: read from stdin]
   #[clap(short = 'i', long = "in", value_name = "FILE")]
   input: Option<PathBuf>,
   /// Path of the output file [default: write to stdout]
   #[clap(short = 'o', long = "out", value_name = "FILE")]
@@ -72,17 +71,14 @@
   separator: char,
   /// Exec concurrently using N threads (row order not preserved!)
   #[arg(long, value_name = "N")]
   parallel: Option<usize>,
   /// Number of rows process by a same thread in `parallel` mode
   #[arg(long, default_value_t = 10_000_usize)]
   chunk_size: usize,
-  /// Robust TABLEDATA -> CSV conversion: to be used if rows contains comments or CDATA.
-  #[arg(short, long, value_name = "N")]
-  robust: bool,
 }
 
 impl StreamConvert {
   pub fn exec(self) -> Result<(), VOTableError> {
     self.choose_input_and_exec()
   }
```

### Comparing `votable_cli-0.5.0/crates/cli/src/visitors/colnames.rs` & `votable_cli-0.6.0/crates/cli/src/visitors/colnames.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/crates/cli/src/visitors/fieldarray.rs` & `votable_cli-0.6.0/crates/cli/src/visitors/fieldarray.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.5.0/crates/cli/src/visitors/viz_org_names.rs` & `votable_cli-0.6.0/crates/cli/src/visitors/viz_org_names.rs`

 * *Files 1% similar despite different names*

```diff
@@ -35,21 +35,21 @@
 impl VOTableVisitor<VoidTableDataContent> for ExplicitVizierOrgNamesVisitor {
   type E = StringError;
 
   type M = DoNothing<Self::E>;
 
   fn visit_votable_start(
     &mut self,
-    votable: &mut VOTable<VoidTableDataContent>,
+    _votable: &mut VOTable<VoidTableDataContent>,
   ) -> Result<(), Self::E> {
     Ok(())
   }
   fn visit_votable_ended(
     &mut self,
-    votable: &mut VOTable<VoidTableDataContent>,
+    _votable: &mut VOTable<VoidTableDataContent>,
   ) -> Result<(), Self::E> {
     Ok(())
   }
 
   fn visit_description(&mut self, _description: &mut Description) -> Result<(), Self::E> {
     Ok(())
   }
@@ -92,15 +92,15 @@
   }
   fn visit_param_ended(&mut self, _param: &mut Param) -> Result<(), Self::E> {
     Ok(())
   }
 
   fn visit_field_start(&mut self, field: &mut Field) -> Result<(), Self::E> {
     if let Some(desc) = &field.description {
-      let desc = desc.0.trim();
+      let desc = desc.get_content_unwrapped().trim();
       if desc.ends_with(')') {
         // Unwrap ok because we tested before that it ended with a ')'.
         if let Some((_, colname)) = desc.strip_suffix(')').unwrap().rsplit_once('(') {
           let colname = colname.trim();
           // No space (unlike in comments) and not an integer (unlike in note reference)
           if !colname.contains(' ') && colname.parse::<u16>().is_err() && colname != "J2000" {
             field.insert_extra_by_ref("vizier:org_name", colname.into());
```

### Comparing `votable_cli-0.5.0/crates/cli/src/visitors/votstruct.rs` & `votable_cli-0.6.0/crates/cli/src/visitors/votstruct.rs`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   param::Param,
   paramref::ParamRef,
   resource::Resource,
   table::Table,
   timesys::TimeSys,
   values::{Max, Min, Opt, Values},
   votable::VOTable,
-  TableDataContent, VOTableVisitor, VoidTableDataContent,
+  TableDataContent, VOTableElement, VOTableVisitor, VoidTableDataContent,
 };
 
 use super::{StringError, Tag};
 
 /// Indentation unit (2 spaces here).
 static INDENT: &str = "  ";
 /// String separing 2 `key=value` pairs
@@ -324,15 +324,15 @@
     let mut tagp = TagPrinter::new(
       self.line_width,
       self.indent.as_str(),
       TAG,
       vid.as_str(),
       self.content_size_min,
     );
-    tagp.set_content(description.0.as_str());
+    tagp.set_content(description.get_content_unwrapped());
     tagp.print()
   }
 
   fn visit_coosys_start(&mut self, coosys: &mut CooSys) -> Result<(), Self::E> {
     const TAG: Tag = Tag::COOSYS;
     let curr_indent = self.indent.clone();
     self.go_down(TAG, true);
@@ -668,44 +668,44 @@
       self.content_size_min,
     );
     values.for_each_attribute(|key: &str, val: &str| tagp.push_attr_mand(key, val));
     tagp.print()
   }
   fn visit_values_min(&mut self, min: &mut Min) -> Result<(), Self::E> {
     const TAG: Tag = Tag::MIN;
-    let vid = self.get_sub_elem_vid(TAG, true);
+    let vid = self.get_sub_elem_vid(TAG, false);
     let mut tagp = TagPrinter::new(
       self.line_width,
       self.indent.as_str(),
       TAG,
       vid.as_str(),
       self.content_size_min,
     );
     min.for_each_attribute(|key: &str, val: &str| tagp.push_attr_mand(key, val));
     tagp.print()
   }
 
   fn visit_values_max(&mut self, max: &mut Max) -> Result<(), Self::E> {
     const TAG: Tag = Tag::MAX;
-    let vid = self.get_sub_elem_vid(TAG, true);
+    let vid = self.get_sub_elem_vid(TAG, false);
     let mut tagp = TagPrinter::new(
       self.line_width,
       self.indent.as_str(),
       TAG,
       vid.as_str(),
       self.content_size_min,
     );
     max.for_each_attribute(|key: &str, val: &str| tagp.push_attr_mand(key, val));
     tagp.print()
   }
 
   fn visit_values_opt_start(&mut self, opt: &mut Opt) -> Result<(), Self::E> {
     const TAG: Tag = Tag::OPTION;
     let curr_indent = self.indent.clone();
-    self.go_down(TAG, false);
+    self.go_down(TAG, true);
     let mut tagp = TagPrinter::new(
       self.line_width,
       curr_indent.as_str(),
       TAG,
       self.get_vid(),
       self.content_size_min,
     );
```

### Comparing `votable_cli-0.5.0/Cargo.lock` & `votable_cli-0.6.0/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anstream"
 version = "0.6.13"
@@ -94,17 +94,17 @@
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "clap"
-version = "4.5.2"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b230ab84b0ffdf890d5a10abdbc8b83ae1c4918275daea1ab8801f71536b2651"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
 ]
 
 [[package]]
 name = "clap_builder"
@@ -116,17 +116,17 @@
  "anstyle",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.5.0"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "307bc0538d5f0f83b8248db3087aa92fe504e4691294d0c96c0eabc33f47ba47"
+checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "syn",
 ]
 
@@ -237,51 +237,51 @@
 name = "hashbrown"
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 
 [[package]]
 name = "heck"
-version = "0.4.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
 
 [[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "indexmap"
-version = "2.2.5"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b0b929d511467233429c45a44ac1dcaa21ba0f5ba11e4879e6ed28ddb4f9df4"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
@@ -289,17 +289,17 @@
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quick-error"
 version = "2.0.1"
@@ -328,17 +328,17 @@
 name = "radium"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
@@ -351,17 +351,17 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
@@ -383,17 +383,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
@@ -404,53 +404,53 @@
 checksum = "eb3622f419d1296904700073ea6cc23ad690adbd66f13ea683df73298736f0c1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_yaml"
-version = "0.9.32"
+version = "0.9.34+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8fd075d994154d4a774f95b51fb96bdc2832b0ea48425c92546073816cda1f2f"
+checksum = "6a8b1a1a2ebf674015cc02edccce75287f1a0130d394307b36743c2f5d504b47"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
 
 [[package]]
 name = "strsim"
-version = "0.11.0"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ee073c9e4cd00e28217186dbe12796d692868f432bf2e97ee73bed0c56dfa01"
+checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
 [[package]]
 name = "syn"
-version = "2.0.52"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
 name = "toml"
-version = "0.8.10"
+version = "0.8.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a9aad4a3066010876e8dcf5a8a06e70a558751117a145c6ce2b82c2e2054290"
+checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
@@ -461,17 +461,17 @@
 checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.22.6"
+version = "0.22.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c1b5fd4128cc8d3e0cb74d4ed9a9cc7c7284becd4df68f5f940e1ad123606f6"
+checksum = "8e40bb779c5187258fd7aad0eb68cb8706a0a81fa712fbea808ab43c4b8374c4"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
@@ -489,27 +489,27 @@
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unsafe-libyaml"
-version = "0.2.10"
+version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab4c90930b95a82d00dc9e9ac071b4991924390d46cbd0dfe566148667605e4b"
+checksum = "673aac59facbab8a9007c7f6108d11f63b603f7cabff99fabf650fea5c32b861"
 
 [[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "votable"
-version = "0.5.0"
+version = "0.6.0"
 dependencies = [
  "base64",
  "bitvec",
  "bstringify",
  "byteorder",
  "log",
  "memchr",
@@ -522,15 +522,15 @@
  "serde_yaml",
  "toml",
  "ucs2",
 ]
 
 [[package]]
 name = "votable-cli"
-version = "0.5.0"
+version = "0.6.0"
 dependencies = [
  "clap",
  "crossbeam",
  "env_logger",
  "log",
  "serde",
  "votable",
```

### Comparing `votable_cli-0.5.0/Cargo.toml` & `votable_cli-0.6.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "votable"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
   "F.-X. Pineau <francois-xavier.pineau@astro.unistra.fr>",
   "T. Dumortier <thibault.dumortier@astro.unistra.fr>"
 ]
 description = """
 Rust implementation of a VOTable serializer/deserializer with support for
 format other than XML, such as JSON, TOML or YAML.
@@ -49,14 +49,15 @@
 quick-error = "2.0" # To handke error more easily
 base64 = "0.21"
 ucs2 = "0.3"
 bitvec = { version = "1", features = ["std", "alloc", "serde"] }
 bstringify = "0.1"
 log = "0.4"
 
+
 [features]
 default = []
 
 # Provides MIVOT parsing support 
 mivot = []
 
 # Use:
```

### Comparing `votable_cli-0.5.0/pyproject.toml` & `votable_cli-0.6.0/pyproject.toml`

 * *Files identical despite different names*

