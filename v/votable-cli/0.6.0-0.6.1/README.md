# Comparing `tmp/votable_cli-0.6.0.tar.gz` & `tmp/votable_cli-0.6.1.tar.gz`

## Comparing `votable_cli-0.6.0.tar` & `votable_cli-0.6.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0     1001      127      310 2024-04-05 15:04:23.000000 votable_cli-0.6.0/.github/workflows/clitest.yml
--rw-r--r--   0     1001      127     5890 2024-04-05 15:04:23.000000 votable_cli-0.6.0/.github/workflows/deploy.yml
--rw-r--r--   0     1001      127      460 2024-04-05 15:04:23.000000 votable_cli-0.6.0/.github/workflows/libtest.yml
--rw-r--r--   0     1001      127     6049 2024-04-05 15:04:23.000000 votable_cli-0.6.0/.github/workflows/release.yml
--rw-r--r--   0     1001      127      454 2024-04-05 15:04:23.000000 votable_cli-0.6.0/.github/workflows/wasmtest.yml
--rw-r--r--   0     1001      127     3427 2024-04-05 15:04:23.000000 votable_cli-0.6.0/CHANGELOG.md
--rw-r--r--   0     1001      127    10852 2024-04-05 15:04:23.000000 votable_cli-0.6.0/LICENSE-APACHE
--rw-r--r--   0     1001      127     1076 2024-04-05 15:04:23.000000 votable_cli-0.6.0/LICENSE-MIT
--rw-r--r--   0     1001      127    20424 2024-04-05 15:04:23.000000 votable_cli-0.6.0/README.md
--rw-r--r--   0     1001      127       14 2024-04-05 15:04:23.000000 votable_cli-0.6.0/rustfmt.toml
--rw-r--r--   0     1001      127    21938 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/coosys.rs
--rw-r--r--   0     1001      127     5035 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/data/binary.rs
--rw-r--r--   0     1001      127     5043 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/data/binary2.rs
--rw-r--r--   0     1001      127     3922 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/data/fits.rs
--rw-r--r--   0     1001      127    12349 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/data/mod.rs
--rw-r--r--   0     1001      127     9557 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/data/stream.rs
--rw-r--r--   0     1001      127    10363 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/data/tabledata.rs
--rw-r--r--   0     1001      127     2159 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/datatype.rs
--rw-r--r--   0     1001      127     4529 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/definitions.rs
--rw-r--r--   0     1001      127     4019 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/desc.rs
--rw-r--r--   0     1001      127     3243 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/error.rs
--rw-r--r--   0     1001      127    24085 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/field.rs
--rw-r--r--   0     1001      127     3377 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/fieldref.rs
--rw-r--r--   0     1001      127    13983 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/group.rs
--rw-r--r--   0     1001      127      123 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/impls/b64/mod.rs
--rw-r--r--   0     1001      127    21027 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/impls/b64/read.rs
--rw-r--r--   0     1001      127    10026 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/impls/b64/write.rs
--rw-r--r--   0     1001      127    15678 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/impls/mem.rs
--rw-r--r--   0     1001      127    59686 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/impls/mod.rs
--rw-r--r--   0     1001      127     6445 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/impls/visitors.rs
--rw-r--r--   0     1001      127     7116 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/info.rs
--rw-r--r--   0     1001      127    10643 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/iter/elems.rs
--rw-r--r--   0     1001      127    43288 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/iter/mod.rs
--rw-r--r--   0     1001      127     1772 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/iter/strings.rs
--rw-r--r--   0     1001      127    34182 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/lib.rs
--rw-r--r--   0     1001      127     4955 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/link.rs
--rw-r--r--   0     1001      127    32733 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/macros.rs
--rw-r--r--   0     1001      127    14070 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/attribute.rs
--rw-r--r--   0     1001      127     6485 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/collection/instance.rs
--rw-r--r--   0     1001      127     9264 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/collection/mod.rs
--rw-r--r--   0     1001      127     2147 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/collection/reference.rs
--rw-r--r--   0     1001      127    11272 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/instance/collection/collection.rs
--rw-r--r--   0     1001      127    10606 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/instance/collection/mod.rs
--rw-r--r--   0     1001      127     5683 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/instance/instance.rs
--rw-r--r--   0     1001      127     6945 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/instance/mod.rs
--rw-r--r--   0     1001      127     3447 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/instance/primary_key.rs
--rw-r--r--   0     1001      127     2790 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/instance/reference.rs
--rw-r--r--   0     1001      127     5985 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/globals/mod.rs
--rw-r--r--   0     1001      127     8634 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/join/mod.rs
--rw-r--r--   0     1001      127     3587 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/join/where.rs
--rw-r--r--   0     1001      127     8218 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/mod.rs
--rw-r--r--   0     1001      127     3319 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/model.rs
--rw-r--r--   0     1001      127     3066 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/report.rs
--rw-r--r--   0     1001      127    11235 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/collection/collection.rs
--rw-r--r--   0     1001      127    10618 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/collection/mod.rs
--rw-r--r--   0     1001      127     7200 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/collection/reference.rs
--rw-r--r--   0     1001      127     5659 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/instance.rs
--rw-r--r--   0     1001      127     6848 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/mod.rs
--rw-r--r--   0     1001      127     4983 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/primary_key.rs
--rw-r--r--   0     1001      127     2491 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/reference/foreign_key.rs
--rw-r--r--   0     1001      127     8031 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/instance/reference/mod.rs
--rw-r--r--   0     1001      127     6510 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/mod.rs
--rw-r--r--   0     1001      127     2499 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/templates/where.rs
--rw-r--r--   0     1001      127     5529 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/visitors/donothing.rs
--rw-r--r--   0     1001      127       19 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/visitors/mod.rs
--rw-r--r--   0     1001      127    10659 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/mivot/vodml.rs
--rw-r--r--   0     1001      127     8247 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/param.rs
--rw-r--r--   0     1001      127     3333 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/paramref.rs
--rw-r--r--   0     1001      127    35855 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/resource.rs
--rw-r--r--   0     1001      127    15234 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/table.rs
--rw-r--r--   0     1001      127    11556 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/timesys.rs
--rw-r--r--   0     1001      127     1215 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/utils.rs
--rw-r--r--   0     1001      127    13247 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/values.rs
--rw-r--r--   0     1001      127    43953 2024-04-05 15:04:23.000000 votable_cli-0.6.0/src/votable.rs
--rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 votable_cli-0.6.0/crates/cli/Cargo.toml
--rw-r--r--   0     1001      127     1625 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/CHANGELOG.md
--rw-r--r--   0     1001      127      123 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/COPYING
--rw-r--r--   0     1001      127    10852 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/LICENSE-APACHE
--rw-r--r--   0     1001      127     1076 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/LICENSE-MIT
--rw-r--r--   0     1001      127    16159 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/README.md
--rw-r--r--   0     1001      127     1981 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/doc/vot.1.txt.tpl
--rwxr-xr-x   0     1001      127     1572 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/resource/test_edit.bash
--rw-r--r--   0     1001      127     8406 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/resource/test_edit.td.xml
--rw-r--r--   0     1001      127      432 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/convert.rs
--rw-r--r--   0     1001      127    26312 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/edit.rs
--rw-r--r--   0     1001      127     7370 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/get.rs
--rw-r--r--   0     1001      127     3786 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/input.rs
--rw-r--r--   0     1001      127      134 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/lib.rs
--rw-r--r--   0     1001      127      943 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/main.rs
--rw-r--r--   0     1001      127     2902 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/output.rs
--rw-r--r--   0     1001      127    27220 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/streaming.rs
--rw-r--r--   0     1001      127     5465 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/visitors/colnames.rs
--rw-r--r--   0     1001      127     9247 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/visitors/fieldarray.rs
--rw-r--r--   0     1001      127     4803 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/visitors/mod.rs
--rw-r--r--   0     1001      127    37629 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/visitors/update.rs
--rw-r--r--   0     1001      127     6160 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/visitors/viz_org_names.rs
--rw-r--r--   0     1001      127    22004 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/visitors/votstruct.rs
--rw-r--r--   0     1001      127    33344 2024-04-05 15:04:23.000000 votable_cli-0.6.0/crates/cli/src/wrappedelems.rs
--rw-r--r--   0        0        0    16181 2024-04-05 15:04:36.000000 votable_cli-0.6.0/Cargo.lock
--rw-r--r--   0        0        0     1999 1970-01-01 00:00:00.000000 votable_cli-0.6.0/Cargo.toml
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 votable_cli-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    16946 1970-01-01 00:00:00.000000 votable_cli-0.6.0/PKG-INFO
+-rw-r--r--   0     1001      127      310 2024-04-15 14:48:26.000000 votable_cli-0.6.1/.github/workflows/clitest.yml
+-rw-r--r--   0     1001      127     5890 2024-04-15 14:48:26.000000 votable_cli-0.6.1/.github/workflows/deploy.yml
+-rw-r--r--   0     1001      127      460 2024-04-15 14:48:26.000000 votable_cli-0.6.1/.github/workflows/libtest.yml
+-rw-r--r--   0     1001      127     6049 2024-04-15 14:48:26.000000 votable_cli-0.6.1/.github/workflows/release.yml
+-rw-r--r--   0     1001      127      454 2024-04-15 14:48:26.000000 votable_cli-0.6.1/.github/workflows/wasmtest.yml
+-rw-r--r--   0     1001      127     3517 2024-04-15 14:48:26.000000 votable_cli-0.6.1/CHANGELOG.md
+-rw-r--r--   0     1001      127    10852 2024-04-15 14:48:26.000000 votable_cli-0.6.1/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1076 2024-04-15 14:48:26.000000 votable_cli-0.6.1/LICENSE-MIT
+-rw-r--r--   0     1001      127    21131 2024-04-15 14:48:26.000000 votable_cli-0.6.1/README.md
+-rw-r--r--   0     1001      127       14 2024-04-15 14:48:26.000000 votable_cli-0.6.1/rustfmt.toml
+-rw-r--r--   0     1001      127    21938 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/coosys.rs
+-rw-r--r--   0     1001      127     5035 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/data/binary.rs
+-rw-r--r--   0     1001      127     5043 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/data/binary2.rs
+-rw-r--r--   0     1001      127     3922 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/data/fits.rs
+-rw-r--r--   0     1001      127    12349 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/data/mod.rs
+-rw-r--r--   0     1001      127     9557 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/data/stream.rs
+-rw-r--r--   0     1001      127    10363 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/data/tabledata.rs
+-rw-r--r--   0     1001      127     2159 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/datatype.rs
+-rw-r--r--   0     1001      127     4529 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/definitions.rs
+-rw-r--r--   0     1001      127     4019 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/desc.rs
+-rw-r--r--   0     1001      127     3243 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/error.rs
+-rw-r--r--   0     1001      127    24085 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/field.rs
+-rw-r--r--   0     1001      127     3377 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/fieldref.rs
+-rw-r--r--   0     1001      127    13983 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/group.rs
+-rw-r--r--   0     1001      127      123 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/impls/b64/mod.rs
+-rw-r--r--   0     1001      127    21027 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/impls/b64/read.rs
+-rw-r--r--   0     1001      127    10026 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/impls/b64/write.rs
+-rw-r--r--   0     1001      127    15678 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/impls/mem.rs
+-rw-r--r--   0     1001      127    59686 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/impls/mod.rs
+-rw-r--r--   0     1001      127     6445 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/impls/visitors.rs
+-rw-r--r--   0     1001      127     7116 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/info.rs
+-rw-r--r--   0     1001      127    10643 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/iter/elems.rs
+-rw-r--r--   0     1001      127    43288 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/iter/mod.rs
+-rw-r--r--   0     1001      127     1772 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/iter/strings.rs
+-rw-r--r--   0     1001      127    34182 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/lib.rs
+-rw-r--r--   0     1001      127     4955 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/link.rs
+-rw-r--r--   0     1001      127    32733 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/macros.rs
+-rw-r--r--   0     1001      127    14070 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/attribute.rs
+-rw-r--r--   0     1001      127     6485 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/globals/collection/instance.rs
+-rw-r--r--   0     1001      127     9264 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/globals/collection/mod.rs
+-rw-r--r--   0     1001      127     2147 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/globals/collection/reference.rs
+-rw-r--r--   0     1001      127    11272 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/globals/instance/collection/collection.rs
+-rw-r--r--   0     1001      127    10606 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/globals/instance/collection/mod.rs
+-rw-r--r--   0     1001      127     5683 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/globals/instance/instance.rs
+-rw-r--r--   0     1001      127     6945 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/globals/instance/mod.rs
+-rw-r--r--   0     1001      127     3447 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/globals/instance/primary_key.rs
+-rw-r--r--   0     1001      127     2790 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/globals/instance/reference.rs
+-rw-r--r--   0     1001      127     5985 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/globals/mod.rs
+-rw-r--r--   0     1001      127     8634 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/join/mod.rs
+-rw-r--r--   0     1001      127     3587 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/join/where.rs
+-rw-r--r--   0     1001      127     8218 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/mod.rs
+-rw-r--r--   0     1001      127     3319 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/model.rs
+-rw-r--r--   0     1001      127     3066 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/report.rs
+-rw-r--r--   0     1001      127    11235 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/templates/instance/collection/collection.rs
+-rw-r--r--   0     1001      127    10618 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/templates/instance/collection/mod.rs
+-rw-r--r--   0     1001      127     7200 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/templates/instance/collection/reference.rs
+-rw-r--r--   0     1001      127     5659 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/templates/instance/instance.rs
+-rw-r--r--   0     1001      127     6848 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/templates/instance/mod.rs
+-rw-r--r--   0     1001      127     4983 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/templates/instance/primary_key.rs
+-rw-r--r--   0     1001      127     2491 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/templates/instance/reference/foreign_key.rs
+-rw-r--r--   0     1001      127     8031 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/templates/instance/reference/mod.rs
+-rw-r--r--   0     1001      127     6510 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/templates/mod.rs
+-rw-r--r--   0     1001      127     2499 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/templates/where.rs
+-rw-r--r--   0     1001      127     5529 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/visitors/donothing.rs
+-rw-r--r--   0     1001      127       19 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/visitors/mod.rs
+-rw-r--r--   0     1001      127    10659 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/mivot/vodml.rs
+-rw-r--r--   0     1001      127     8247 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/param.rs
+-rw-r--r--   0     1001      127     3333 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/paramref.rs
+-rw-r--r--   0     1001      127    36458 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/resource.rs
+-rw-r--r--   0     1001      127    15234 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/table.rs
+-rw-r--r--   0     1001      127    11556 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/timesys.rs
+-rw-r--r--   0     1001      127     1215 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/utils.rs
+-rw-r--r--   0     1001      127    13247 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/values.rs
+-rw-r--r--   0     1001      127    43953 2024-04-15 14:48:26.000000 votable_cli-0.6.1/src/votable.rs
+-rw-r--r--   0        0        0     2033 1970-01-01 00:00:00.000000 votable_cli-0.6.1/crates/cli/Cargo.toml
+-rw-r--r--   0     1001      127     1890 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/CHANGELOG.md
+-rw-r--r--   0     1001      127      123 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/COPYING
+-rw-r--r--   0     1001      127    10852 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1076 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/LICENSE-MIT
+-rw-r--r--   0     1001      127    27131 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/README.md
+-rw-r--r--   0     1001      127     1981 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/doc/vot.1.txt.tpl
+-rwxr-xr-x   0     1001      127     1572 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/resource/test_edit.bash
+-rw-r--r--   0     1001      127     8406 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/resource/test_edit.td.xml
+-rw-r--r--   0     1001      127      432 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/convert.rs
+-rw-r--r--   0     1001      127    27315 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/edit.rs
+-rw-r--r--   0     1001      127     7110 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/get.rs
+-rw-r--r--   0     1001      127     3810 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/input.rs
+-rw-r--r--   0     1001      127      134 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/lib.rs
+-rw-r--r--   0     1001      127      687 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/main.rs
+-rw-r--r--   0     1001      127     2906 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/output.rs
+-rw-r--r--   0     1001      127    27829 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/streaming.rs
+-rw-r--r--   0     1001      127     5465 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/visitors/colnames.rs
+-rw-r--r--   0     1001      127     9247 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/visitors/fieldarray.rs
+-rw-r--r--   0     1001      127     4803 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/visitors/mod.rs
+-rw-r--r--   0     1001      127    37583 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/visitors/update.rs
+-rw-r--r--   0     1001      127     6111 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/visitors/viz_org_names.rs
+-rw-r--r--   0     1001      127    22004 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/visitors/votstruct.rs
+-rw-r--r--   0     1001      127    34343 2024-04-15 14:48:26.000000 votable_cli-0.6.1/crates/cli/src/wrappedelems.rs
+-rw-r--r--   0        0        0    16411 2024-04-15 14:48:39.000000 votable_cli-0.6.1/Cargo.lock
+-rw-r--r--   0        0        0     1999 1970-01-01 00:00:00.000000 votable_cli-0.6.1/Cargo.toml
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 votable_cli-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    27931 1970-01-01 00:00:00.000000 votable_cli-0.6.1/PKG-INFO
```

### Comparing `votable_cli-0.6.0/.github/workflows/deploy.yml` & `votable_cli-0.6.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/.github/workflows/release.yml` & `votable_cli-0.6.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/CHANGELOG.md` & `votable_cli-0.6.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # `votable` Change Log
 
+## 0.6.1
+
+Released 2024-04-15
+
+* Mainly changes in the cli
+* Minor README modifications
+
+
 ## 0.6.0
 
 Released 2024-04-05
 
 ### Changed
 
 * ⚠️  BREAKING: the tag is now in the `VOTableTrait` instead of the `QuickXmlReadWrite` trait
```

### Comparing `votable_cli-0.6.0/LICENSE-APACHE` & `votable_cli-0.6.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/LICENSE-MIT` & `votable_cli-0.6.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/README.md` & `votable_cli-0.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 <meta charset="utf-8"/>
 
 # `votable` or `VOTLibRust`
 
-Library to build, read and write [VOTables](https://www.ivoa.net/documents/VOTable/)
-in Rust and to convert them efficiently back and forth in JSON, YAML, TOML, XML-TABLEDATA, XML-BINARY and XML-BINARY2
+Library to build, edit, read and write [VOTables](https://www.ivoa.net/documents/VOTable/)
+in Rust and to convert them efficiently back and forth in standard XML-TABLEDATA, XML-BINARY, XML-BINARY2
+and non-standard JSON, YAML and TOML
 while preserving all elements (except comments) and their order.
 
 [![](https://img.shields.io/crates/v/votable.svg)](https://crates.io/crates/votable)
 [![](https://img.shields.io/crates/d/votable.svg)](https://crates.io/crates/votable)
 [![API Documentation on docs.rs](https://docs.rs/votable/badge.svg)](https://docs.rs/votable/)
 [![BenchLib](https://github.com/cds-astro/cds-votable-rust/actions/workflows/libtest.yml/badge.svg)](https://github.com/cds-astro/cds-moc-rust/actions/workflows/libtest.yml)
 
 VOT Lib Rust is used in:
 * [VOTCli](https://github.com/cds-astro/cds-votable-rust/tree/main/crates/cli) 
-  convert VOTables from the command line;
+  edit and convert VOTables from the command line;
 * [VOTWasm](https://github.com/cds-astro/cds-votable-rust/tree/main/crates/wasm) 
   read/write and convert VOTables in Web Browsers.
 * [Aladin Lite V3](https://github.com/cds-astro/aladin-lite)
 
 ## Status
 
 The code contains all main functionalities: 
 * supports BINARY, BINARY2 formats
 * supports CDATA in rows, StAX mode for streaming
 * supports MIVOT block parsing
 
-But it is far from been as clean and documented as I would like.
+But is not yet as clean and documented as I would like.
 If you want to use this crate in a Rust project, you should probably have a look 
 at the VOTCli code.
 
 We are still (reasonably) open to changes, e.g.:
 * we could flag attributes with a '@' prefix
 * we could use upper case elements tag names
 * we could remove the 's' suffix in elements arrays
@@ -102,14 +103,36 @@
 In JSON/TOML/YAML, there is no difference between attribute and sub-elements 
 names (all in camel case).
 
 ### WARNINGS
 
 * TOML does not support `null` (we so far convert `null` values by an empty string).
 * Conversions from/to TOML/JSON/YAML requires all data to be loaded in memory, it is not adapted for large files.
+* We do not support VOTable such as (example provided by Mark Taylor):
+```xml
+ <?xml version='1.0'?>
+<!DOCTYPE VOTABLE [ <!ENTITY td3 '<TD>4</TD>'> ]>
+<VOTABLE version="1.4" xmlns="http://www.ivoa.net/xml/VOTable/v1.3">
+  <RESOURCE>
+    <TABLE>
+      <FIELD datatype="int" name="i"/>
+      <DATA>
+        <TABLEDATA>
+          <TR><TD>0</TD></TR>
+          <TR><TD>1</TD></TR >
+          <TR><TD>2</TD></TR>
+          <TR>&td3;</TR>
+        </TABLEDATA>
+      </DATA>
+    </TABLE>
+  </RESOURCE>
+</VOTABLE> 
+```
+since [quick_xml](https://github.com/tafia/quick-xml) so far does not cope with declared entities, 
+see [this issue](https://github.com/tafia/quick-xml/issues/258).
 
 ## Other way to convert from VOTable to JSON
 
 The XML2JSON conversion has been exercised
 by [Laurent Michel](https://github.com/lmichel)
 in the context of the processing of model annotations in VOTables 
 ([the MIVOT](https://github.com/ivoa-std/ModelInstanceInVot)).
```

### Comparing `votable_cli-0.6.0/src/coosys.rs` & `votable_cli-0.6.1/src/coosys.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/data/binary.rs` & `votable_cli-0.6.1/src/data/binary.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/data/binary2.rs` & `votable_cli-0.6.1/src/data/binary2.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/data/fits.rs` & `votable_cli-0.6.1/src/data/fits.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/data/mod.rs` & `votable_cli-0.6.1/src/data/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/data/stream.rs` & `votable_cli-0.6.1/src/data/stream.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/data/tabledata.rs` & `votable_cli-0.6.1/src/data/tabledata.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/datatype.rs` & `votable_cli-0.6.1/src/datatype.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/definitions.rs` & `votable_cli-0.6.1/src/definitions.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/desc.rs` & `votable_cli-0.6.1/src/desc.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/error.rs` & `votable_cli-0.6.1/src/error.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/field.rs` & `votable_cli-0.6.1/src/field.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/fieldref.rs` & `votable_cli-0.6.1/src/fieldref.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/group.rs` & `votable_cli-0.6.1/src/group.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/impls/b64/read.rs` & `votable_cli-0.6.1/src/impls/b64/read.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/impls/b64/write.rs` & `votable_cli-0.6.1/src/impls/b64/write.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/impls/mem.rs` & `votable_cli-0.6.1/src/impls/mem.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/impls/mod.rs` & `votable_cli-0.6.1/src/impls/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/impls/visitors.rs` & `votable_cli-0.6.1/src/impls/visitors.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/info.rs` & `votable_cli-0.6.1/src/info.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/iter/elems.rs` & `votable_cli-0.6.1/src/iter/elems.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/iter/mod.rs` & `votable_cli-0.6.1/src/iter/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/iter/strings.rs` & `votable_cli-0.6.1/src/iter/strings.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/lib.rs` & `votable_cli-0.6.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/link.rs` & `votable_cli-0.6.1/src/link.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/macros.rs` & `votable_cli-0.6.1/src/macros.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/attribute.rs` & `votable_cli-0.6.1/src/mivot/attribute.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/globals/collection/instance.rs` & `votable_cli-0.6.1/src/mivot/globals/collection/instance.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/globals/collection/mod.rs` & `votable_cli-0.6.1/src/mivot/globals/collection/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/globals/collection/reference.rs` & `votable_cli-0.6.1/src/mivot/globals/collection/reference.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/globals/instance/collection/collection.rs` & `votable_cli-0.6.1/src/mivot/globals/instance/collection/collection.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/globals/instance/collection/mod.rs` & `votable_cli-0.6.1/src/mivot/globals/instance/collection/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/globals/instance/instance.rs` & `votable_cli-0.6.1/src/mivot/globals/instance/instance.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/globals/instance/mod.rs` & `votable_cli-0.6.1/src/mivot/globals/instance/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/globals/instance/primary_key.rs` & `votable_cli-0.6.1/src/mivot/globals/instance/primary_key.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/globals/instance/reference.rs` & `votable_cli-0.6.1/src/mivot/globals/instance/reference.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/globals/mod.rs` & `votable_cli-0.6.1/src/mivot/globals/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/join/mod.rs` & `votable_cli-0.6.1/src/mivot/join/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/join/where.rs` & `votable_cli-0.6.1/src/mivot/join/where.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/mod.rs` & `votable_cli-0.6.1/src/mivot/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/model.rs` & `votable_cli-0.6.1/src/mivot/model.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/report.rs` & `votable_cli-0.6.1/src/mivot/report.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/templates/instance/collection/collection.rs` & `votable_cli-0.6.1/src/mivot/templates/instance/collection/collection.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/templates/instance/collection/mod.rs` & `votable_cli-0.6.1/src/mivot/templates/instance/collection/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/templates/instance/collection/reference.rs` & `votable_cli-0.6.1/src/mivot/templates/instance/collection/reference.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/templates/instance/instance.rs` & `votable_cli-0.6.1/src/mivot/templates/instance/instance.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/templates/instance/mod.rs` & `votable_cli-0.6.1/src/mivot/templates/instance/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/templates/instance/primary_key.rs` & `votable_cli-0.6.1/src/mivot/templates/instance/primary_key.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/templates/instance/reference/foreign_key.rs` & `votable_cli-0.6.1/src/mivot/templates/instance/reference/foreign_key.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/templates/instance/reference/mod.rs` & `votable_cli-0.6.1/src/mivot/templates/instance/reference/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/templates/mod.rs` & `votable_cli-0.6.1/src/mivot/templates/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/templates/where.rs` & `votable_cli-0.6.1/src/mivot/templates/where.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/visitors/donothing.rs` & `votable_cli-0.6.1/src/mivot/visitors/donothing.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/mivot/vodml.rs` & `votable_cli-0.6.1/src/mivot/vodml.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/param.rs` & `votable_cli-0.6.1/src/param.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/paramref.rs` & `votable_cli-0.6.1/src/paramref.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/resource.rs` & `votable_cli-0.6.1/src/resource.rs`

 * *Files 2% similar despite different names*

```diff
@@ -271,40 +271,71 @@
 
 impl<C: TableDataContent> Resource<C> {
   pub fn new() -> Self {
     Default::default()
   }
 
   pub fn from_void_table_data_content(value: Resource<VoidTableDataContent>) -> Self {
-    let Resource {
-      id,
-      name,
-      type_,
-      utype,
-      extra,
-      description,
-      infos,
-      elems,
-      mut sub_elems,
-      vodml,
-    } = value;
-    Self {
-      id,
-      name,
-      type_,
-      utype,
-      extra,
-      description,
-      infos,
-      elems,
-      sub_elems: sub_elems
-        .drain(..)
-        .map(ResourceSubElem::from_void_table_data_content)
-        .collect(),
-      vodml,
+    #[cfg(feature = "mivot")]
+    {
+      let Resource {
+        id,
+        name,
+        type_,
+        utype,
+        extra,
+        description,
+        infos,
+        elems,
+        mut sub_elems,
+        vodml,
+      } = value;
+      Self {
+        id,
+        name,
+        type_,
+        utype,
+        extra,
+        description,
+        infos,
+        elems,
+        sub_elems: sub_elems
+          .drain(..)
+          .map(ResourceSubElem::from_void_table_data_content)
+          .collect(),
+        vodml,
+      }
+    }
+    #[cfg(not(feature = "mivot"))]
+    {
+      let Resource {
+        id,
+        name,
+        type_,
+        utype,
+        extra,
+        description,
+        infos,
+        elems,
+        mut sub_elems,
+      } = value;
+      Self {
+        id,
+        name,
+        type_,
+        utype,
+        extra,
+        description,
+        infos,
+        elems,
+        sub_elems: sub_elems
+          .drain(..)
+          .map(ResourceSubElem::from_void_table_data_content)
+          .collect(),
+      }
     }
   }
 
   // Optional attributes
   impl_builder_opt_string_attr!(id);
   impl_builder_opt_string_attr!(name);
   impl_builder_opt_string_attr!(type_, type);
```

### Comparing `votable_cli-0.6.0/src/table.rs` & `votable_cli-0.6.1/src/table.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/timesys.rs` & `votable_cli-0.6.1/src/timesys.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/utils.rs` & `votable_cli-0.6.1/src/utils.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/values.rs` & `votable_cli-0.6.1/src/values.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/src/votable.rs` & `votable_cli-0.6.1/src/votable.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/crates/cli/Cargo.toml` & `votable_cli-0.6.1/crates/cli/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 name = "votable-cli"
-version = "0.6.0"
+version = "0.6.1"
 authors = ["F.-X. Pineau <francois-xavier.pineau@astro.unistra.fr>"]
-description = "Command-line to extract information from IVOA VOTables and to convert VOTable  back and forth in XML, JSON, YAML, TOML (and to CSV) while preserving all elements (except in CSV)."
+description = "Command-line to extract/edit metadata from IVOA VOTables and to convert efficiently VOTable back and forth in XML-TABLEDATA, XML-BINARY, XML-BINARY2, non-standard JSON/YAML/TOML (and to CSV)."
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 categories = ["command-line-utilities", "science", "data-structures"]
 keywords = ["ivoa", "votable", "xml"]
 documentation = "https://github.com/cds-astro/cds-votable-rust/tree/main/crates/cli"
 homepage = "https://github.com/cds-astro/cds-votable-rust/tree/main/crates/cli"
 repository = "https://github.com/cds-astro/cds-votable-rust/tree/main/crates/cli"
@@ -43,17 +43,12 @@
 assets = [
     ["target/release/vot", "usr/bin/vot", "755"],
     ["COPYING", "usr/share/doc/vot/", "644"],
     ["LICENSE-MIT", "usr/share/doc/vot/", "644"],
     ["LICENSE-APACHE", "usr/share/doc/vot/", "644"],
     ["CHANGELOG.md", "usr/share/doc/vot/CHANGELOG", "644"],
     ["README.md", "usr/share/doc/vot/README", "644"],
-    #["FAQ.md", "usr/share/doc/vot/FAQ", "644"],
     ["doc/vot.1", "usr/share/man/man1/vot.1", "644"],
-    # Similarly for shell completions.
-    #["deployment/deb/vot.bash", "usr/share/bash-completion/completions/vot", "644"],
-    #["deployment/deb/vot.fish", "usr/share/fish/vendor_completions.d/vot.fish", "644"],
-    #["deployment/deb/_vot", "usr/share/zsh/vendor-completions/", "644"],
 ]
 extended-description = """\
-vot is a command-line to convert VOTable is various formats such as JSON, TOML and YAML and back to XML
+Command-line to extract/edit metadata from IVOA VOTables and to convert efficiently VOTable back and forth in XML-TABLEDATA, XML-BINARY, XML-BINARY2, non-standard JSON/YAML/TOML (and to CSV).
 """
```

### Comparing `votable_cli-0.6.0/crates/cli/CHANGELOG.md` & `votable_cli-0.6.1/crates/cli/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 # `moc-cli` Change Log
 
+## 0.6.1
+
+Released 2024-04-15
+
+* Reword/fix typo in the documentation/help messages
+* Row order is now preserved in `streaming` mode with `parallel` option
+* Add `vizier-org-names` option in `edit` command (visitor code was ready but we forget to add the option)
+
+
 ## 0.6.0
 
-Released 2023-04-05
+Released 2024-04-05
 
 * Add sub-command 'edit' to modify a VOTable
 
 
 ## 0.5.0
 
-Released 2023-03-11
+Released 2024-03-11
 
 * ⚠️  BREAKING: new options and hence new command layout
 * Add the 'convert' sub-command, and conversion from XML to CSV
 * Add the 'sconvert' sub-command for streaming conversion
     + add 'parallel' for multi-threaded streaming conversion
 * Add 'get' command to retrieve some metadata or the VOTable structure
 
 
 ## 0.4.0
 
-Released 2023-02-06
+Released 2024-02-06
 
 * Add logger to control stderr messages
 * Version and xmlns now mandatory in VOTable (with v1.4 as default)
 
 
 ## 0.3.0
 
-Released 2023-01-12
+Released 2024-01-12
 
 * Add conversions between TABLEDATA/BINARY/BINARY2
 * Supports VOTable 1.5
 * Add Mivot parsing (VODML tag)
 * For other changes/bug correction, see the `votable` crate changelog
```

### Comparing `votable_cli-0.6.0/crates/cli/LICENSE-APACHE` & `votable_cli-0.6.1/crates/cli/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/crates/cli/LICENSE-MIT` & `votable_cli-0.6.1/crates/cli/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/crates/cli/doc/vot.1.txt.tpl` & `votable_cli-0.6.1/crates/cli/doc/vot.1.txt.tpl`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/crates/cli/resource/test_edit.bash` & `votable_cli-0.6.1/crates/cli/resource/test_edit.bash`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/crates/cli/resource/test_edit.td.xml` & `votable_cli-0.6.1/crates/cli/resource/test_edit.td.xml`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/crates/cli/src/edit.rs` & `votable_cli-0.6.1/crates/cli/src/edit.rs`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 use votable::{
   data::TableOrBinOrBin2, error::VOTableError, iter::SimpleVOTableRowIterator,
   votable::new_xml_writer, CooSys, Description, Field, FieldRef, Group, Info, Link, Max, Min, Opt,
   Param, ParamRef, Resource, TableDataContent, TableGroup, TimeSys, VOTableElement, Values,
   VoidTableDataContent,
 };
 
+#[cfg(feature = "vizier")]
+use super::visitors::viz_org_names::ExplicitVizierOrgNamesVisitor;
 use super::{
   input::Input,
   output::{Output, OutputFormat},
   visitors::{update::UpdateVisitor, Tag},
   wrappedelems::{VOTableWrappedElem, VOTableWrappedElemMut},
 };
 
@@ -74,40 +76,57 @@
   ///   Those three commands do not lead to the same hierarchy:
   ///     `push_group ... @push_group ... @push_group @@push_group @push_group (@<)`
   ///     `push_group ... @push_group ... @push_group @@push_group @@push_group (@<@<)`
   ///     `push_group ... @push_group ... @push_group @@push_group @< @push_group`
   ///   Remark: `@@xxx` is a short version of `@> @xxx`.
   #[arg(short = 'e', long = "edit", verbatim_doc_comment)]
   elems: Vec<TagConditionAction>,
+  /// Extract original column names from VizieR description ending by '(org_name)' and put it inn
+  /// the non-standard 'viz:org_name' attribute, be aware of the risk of false-detections!
+  #[cfg(feature = "vizier")]
+  #[arg(short = 'z', long = "vizier-org-names")]
+  vizier_org_names: bool,
   /// Use streaming mode: only for large XML files with a single table, and if the input format
   /// is the same as the output format.
   #[arg(short, long)]
   streaming: bool,
 }
 
 impl Edit {
   pub fn exec(self) -> Result<(), VOTableError> {
     if self.streaming {
       if self.input.is_streamable()? {
         self.choose_input_and_exec()
       } else {
         Err(VOTableError::Custom(
-          "Only the 'xml' input format is supporting with option '--streaming'.".into(),
+          "Only the 'xml' input format is supported with option '--streaming'.".into(),
         ))
       }
     } else {
       self
         .input
         .load()
         .and_then(|vot| {
           let mut visitor = UpdateVisitor::new(self.elems);
           let mut vot = vot.unwrap();
           vot
             .visit(&mut visitor)
             .map_err(|e| VOTableError::Custom(e.to_string()))
+            .and_then(|_| {
+              #[cfg(feature = "vizier")]
+              if self.vizier_org_names {
+                vot
+                  .visit(&mut ExplicitVizierOrgNamesVisitor::new())
+                  .map_err(|e| VOTableError::Custom(e.to_string()))
+              } else {
+                Ok(())
+              }
+              #[cfg(not(feature = "vizier"))]
+              Ok(())
+            })
             .map(|_| vot.wrap())
         })
         .and_then(|vot| self.output.save(vot))
     }
   }
 
   pub fn choose_input_and_exec(self) -> Result<(), VOTableError> {
@@ -147,47 +166,53 @@
     it: SimpleVOTableRowIterator<R>,
     write: W,
   ) -> Result<(), VOTableError>
   where
     R: BufRead + Send,
     W: Write,
   {
-    let visitor = UpdateVisitor::new(self.elems);
     match (it.data_type(), self.output.output_fmt) {
-      (TableOrBinOrBin2::TableData, OutputFormat::XmlTabledata) => to_same(it, write, visitor),
-      (TableOrBinOrBin2::Binary, OutputFormat::XmlBinary) => to_same(it, write, visitor),
-      (TableOrBinOrBin2::Binary2, OutputFormat::XmlBinary2) => to_same(it, write, visitor),
+      (TableOrBinOrBin2::TableData, OutputFormat::XmlTabledata) => self.to_same(it, write),
+      (TableOrBinOrBin2::Binary, OutputFormat::XmlBinary) => self.to_same(it, write),
+      (TableOrBinOrBin2::Binary2, OutputFormat::XmlBinary2) => self.to_same(it, write),
       _ => Err(VOTableError::Custom(format!(
         "Input format '{:?}' not compatible with output format '{:?}'",
         it.data_type(),
         self.output.output_fmt
       ))),
     }
   }
-}
 
-fn to_same<R: BufRead, W: Write>(
-  mut it: SimpleVOTableRowIterator<R>,
-  write: W,
-  mut visitor: UpdateVisitor,
-) -> Result<(), VOTableError> {
-  let mut writer = new_xml_writer(write, None, None);
-  let mut vot = it.votable.clone();
-  vot.visit(&mut visitor)?; // Modif and write the cloned version to avoid destructive modifications
-  if vot.write_to_data_beginning(&mut writer, &(), false)? {
-    it.copy_remaining_data(&mut writer.inner())
-      .and_then(|_| it.read_to_end())
-      .and_then(|mut out_vot| {
-        out_vot
-          .visit(&mut visitor) // Re-visit the full VOTable before writting its tail
-          .and_then(|()| out_vot.write_from_data_end(&mut writer, &(), false))
-      })
-  } else {
-    // No table in the VOTable
-    Ok(())
+  fn to_same<R: BufRead, W: Write>(
+    self,
+    mut it: SimpleVOTableRowIterator<R>,
+    write: W,
+  ) -> Result<(), VOTableError> {
+    let mut writer = new_xml_writer(write, None, None);
+    let mut vot = it.votable.clone();
+    let mut visitor = UpdateVisitor::new(self.elems);
+    vot.visit(&mut visitor)?; // Modif and write the cloned version to avoid destructive modifications
+    #[cfg(feature = "vizier")]
+    if self.vizier_org_names {
+      vot
+        .visit(&mut ExplicitVizierOrgNamesVisitor::new())
+        .map_err(|e| VOTableError::Custom(e.to_string()))?;
+    }
+    if vot.write_to_data_beginning(&mut writer, &(), false)? {
+      it.copy_remaining_data(&mut writer.inner())
+        .and_then(|_| it.read_to_end())
+        .and_then(|mut out_vot| {
+          out_vot
+            .visit(&mut visitor) // Re-visit the full VOTable before writting its tail
+            .and_then(|()| out_vot.write_from_data_end(&mut writer, &(), false))
+        })
+    } else {
+      // No table in the VOTable
+      Ok(())
+    }
   }
 }
 
 #[derive(Debug, Clone)]
 pub struct TagConditionAction {
   pub tag: Tag,
   pub condition: Condition,
@@ -330,15 +355,15 @@
     let mut it = s.split('=');
     if let Some(first_key) = it.next() {
       let mut key = first_key.trim();
       while let Some(rem) = it.next() {
         if let Some((val, next_key)) = rem.rsplit_once(' ') {
           kv.push((key.to_string(), val.trim().to_string()));
           key = next_key.trim();
-        } else if !it.next().is_none() {
+        } else if it.next().is_some() {
           panic!("Unable to parse value and key in {}", rem)
         } else {
           kv.push((key.to_string(), rem.trim().to_string()));
         }
       }
     }
     kv
```

### Comparing `votable_cli-0.6.0/crates/cli/src/get.rs` & `votable_cli-0.6.1/crates/cli/src/get.rs`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 use super::{
   input::Input,
   visitors::{
     colnames::ColnamesVisitor, fieldarray::FieldArrayVisitor, votstruct::AsciiStructVisitor,
   },
 };
 
-/// Get information from a VOTable, like it structure or fields.
+/// Get information from a VOTable: e.g. its structure or fields metadata.
 #[derive(Debug, Args)]
 pub struct Get {
   #[command(flatten)]
   input: Input,
-  /// Stop parsing before reading first data ('xml' input only).
+  /// Stop parsing before reading first data ('xml' input only): useful for large single-table files.
   #[arg(short = 's', long = "early-stop")]
   stop_at_first_data: bool,
   #[command(subcommand)]
   action: GetAction,
 }
 impl Get {
   pub fn exec(self) -> Result<(), VOTableError> {
@@ -69,45 +69,40 @@
       .and_then(|vot| self.action.exec(vot))
     }
   }
 }
 
 #[derive(Debug, Subcommand)]
 enum GetAction {
-  /// Print the VOTable structure (useful to get Virtual IDs)
+  /// Print the VOTable structure: useful to get Virtual IDs used in edition.
   Struct {
     /// Output line width (min=80)
     #[arg(short = 'w', long = "line-width", default_value = "120")]
     line_width: usize,
     /// Smaller possible size of 'content=xxx' when trying to fit on a single line.
     /// If larger, put on a new line (max=50% of line width)
     #[arg(short = 'c', long = "content-size-min", default_value = "30")]
     content_size_min: usize,
   },
-  /// Print column names, one separated values line per table.
-  ///
-  /// TIP to get the list of the columns of a single table as a column on Linux:
-  ///   vot -i myvot.xml get -s colnames | tr '▮' '\n' | egrep -v '^$'
-  /// or (if no ',' in any names):
-  ///   vot -i myvot.xml get -s colnames -s , | tr ',' '\n'
+  /// Print column names, one line per table.
   #[command(verbatim_doc_comment)]
   Colnames {
-    /// Separator use between each column names.
+    /// Column names separator.
     #[arg(short, long, default_value_t = '▮')]
     separator: char,
   },
   /// Print selected field information as an array
   FieldsArray {
     /// Coma separated list of columns we want in the array of fields attributes
     #[arg(value_enum, value_delimiter(','))]
     fields: Vec<FieldElem>,
-    /// Separator use between each column
+    /// Column separator
     #[arg(short, long, default_value_t = ' ')]
     separator: char,
-    /// Do not requires columns to be aligned
+    /// Do not align columns
     #[arg(short, long)]
     not_aligned: bool,
   },
 }
 
 #[derive(Debug, Copy, Clone, PartialEq, Eq, PartialOrd, Ord, ValueEnum)]
 pub enum FieldElem {
```

### Comparing `votable_cli-0.6.0/crates/cli/src/input.rs` & `votable_cli-0.6.1/crates/cli/src/input.rs`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 /// General VOTable input arguments.
 #[derive(Debug, Args)]
 pub struct Input {
   /// Path of the input VOTable [default: read from stdin]
   #[clap(short = 'i', long = "in", value_name = "FILE")]
   pub input: Option<PathBuf>,
-  /// Format of the input VOTable ('xml', 'json', 'yaml' or 'toml') [default: guess from file extension]
+  /// Format of the input VOTable (standard: 'xml'; not standard: 'json', 'yaml' or 'toml') [default: guess from file extension]
   #[clap(short = 't', long = "in-fmt", value_enum)]
   pub input_fmt: Option<InputFormat>,
 }
 
 impl Input {
   pub fn is_stdin(&self) -> bool {
     self.input.is_none()
```

### Comparing `votable_cli-0.6.0/crates/cli/src/main.rs` & `votable_cli-0.6.1/crates/cli/src/main.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-use std::io::{stderr, stdout, Write};
-
 use clap::Parser;
 
 use votable::error::VOTableError;
 use votable_cli::{convert::Convert, edit::Edit, get::Get, streaming::StreamConvert};
 
 #[derive(Debug, Parser)]
 #[clap(author, version, about, long_about = None)]
@@ -25,17 +23,9 @@
     }
   }
 }
 
 fn main() -> Result<(), VOTableError> {
   let args = CliArgs::parse();
   env_logger::init();
-  args.exec().map_err(|e| {
-    if let Err(e) = stdout().flush() {
-      eprintln!("Error flushing stdout: {:?}", e);
-    }
-    if let Err(e) = stderr().flush() {
-      eprintln!("Error flushing stderr: {:?}", e);
-    }
-    e
-  })
+  args.exec()
 }
```

### Comparing `votable_cli-0.6.0/crates/cli/src/output.rs` & `votable_cli-0.6.1/crates/cli/src/output.rs`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,18 @@
         s
       )),
     }
   }
 }
 impl OutputFormat {
   pub fn is_streamable(&self) -> bool {
-    match self {
-      Self::Xml | Self::XmlTabledata | Self::XmlBinary | Self::XmlBinary2 => true,
-      _ => false,
-    }
+    matches!(
+      self,
+      Self::Xml | Self::XmlTabledata | Self::XmlBinary | Self::XmlBinary2
+    )
   }
   fn put<W: Write>(
     self,
     mut vot: VOTableWrapper<InMemTableDataRows>,
     writer: W,
     pretty: bool,
   ) -> Result<(), VOTableError> {
@@ -73,15 +73,15 @@
 }
 
 #[derive(Debug, Args)]
 pub struct Output {
   /// Path of the output VOTable [default: write to stdout]
   #[clap(short = 'o', long = "out", value_name = "FILE")]
   pub output: Option<PathBuf>,
-  /// Format of the output VOTable ('xml', 'xml-td', 'xml-bin', 'xml-bin2', 'json', 'yaml' or 'toml').
+  /// Format of the output VOTable (standard: 'xml', 'xml-td', 'xml-bin', 'xml-bin2'; not standard: 'json', 'yaml', 'toml').
   #[clap(short = 'f', long = "out-fmt", value_enum)]
   pub output_fmt: OutputFormat,
   /// Pretty print (for JSON and TOML)
   #[clap(short, long)]
   pub pretty: bool,
 }
```

### Comparing `votable_cli-0.6.0/crates/cli/src/streaming.rs` & `votable_cli-0.6.1/crates/cli/src/streaming.rs`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   io::{stdin, stdout, BufRead, BufReader, BufWriter, Cursor, Write},
   path::PathBuf,
   str::FromStr,
   thread::scope,
 };
 
 use clap::Args;
-use crossbeam::channel::bounded;
+use crossbeam::channel::{bounded, Receiver, Sender};
 use serde::{de::DeserializeSeed, Deserializer};
 
 use votable::{
   data::{tabledata::FieldIteratorUnbuffered, TableOrBinOrBin2},
   error::VOTableError,
   impls::{
     b64::{
@@ -50,30 +50,29 @@
         s
       )),
     }
   }
 }
 
 /// Convert a single table XML VOTable in streaming mode.
-/// Tags after `</TABLE>` are preserved.
 #[derive(Debug, Args)]
 pub struct StreamConvert {
   /// Path of the input XML VOTable [default: read from stdin]
   #[clap(short = 'i', long = "in", value_name = "FILE")]
   input: Option<PathBuf>,
   /// Path of the output file [default: write to stdout]
   #[clap(short = 'o', long = "out", value_name = "FILE")]
   output: Option<PathBuf>,
   /// Format of the output file ('xml-td', 'xml-bin', 'xml-bin2' or 'csv').
   #[clap(short = 'f', long = "out-fmt", value_enum)]
   output_fmt: OutputFormat,
   /// Separator used for the 'csv' format.
   #[arg(short, long, default_value_t = ',')]
   separator: char,
-  /// Exec concurrently using N threads (row order not preserved!)
+  /// Exec concurrently using N threads
   #[arg(long, value_name = "N")]
   parallel: Option<usize>,
   /// Number of rows process by a same thread in `parallel` mode
   #[arg(long, default_value_t = 10_000_usize)]
   chunk_size: usize,
 }
 
@@ -120,16 +119,14 @@
     mut write: W,
   ) -> Result<(), VOTableError>
   where
     R: BufRead + Send,
     W: Write,
   {
     match it.data_type() {
-      // In binary64, 6 bit  -> 1 ASCII Char
-      //   3 bytes = 24 bits -> 4 ASCII Chars
       TableOrBinOrBin2::TableData => {
         match self.output_fmt {
           OutputFormat::XmlTabledata => to_same(it, write),
           OutputFormat::XmlBinary => match self.parallel {
             None => to_binary(it, write),
             Some(n_threads) => td_to_binary_par(it, write, n_threads, self.chunk_size),
           },
@@ -836,58 +833,75 @@
   n_threads: usize,
   chunk_size: usize,
 ) -> Result<(), VOTableError>
 where
   I: Iterator<Item = Result<Vec<u8>, VOTableError>> + Send,
   W: Write,
 {
-  let schema = schema;
-  // Usage of crossbeam from https://rust-lang-nursery.github.io/rust-cookbook/concurrency/threads.html
-  let (snd1, rcv1) = bounded(1);
-  let (snd2, rcv2) = bounded(1);
+  let n_threads = n_threads.max(1);
+  // Here we decided to create one (sender, receiver) pairs per thread and iterate on the
+  // ordered sender/receiver to preserve the original row order.
+  // See previous state of the code (before 2024/04/15) for a version which does not preserve
+  // raw order.
+  let (mut senders1, receivers1): (Vec<Sender<_>>, Vec<Receiver<_>>) =
+    (0..n_threads).map(|_| bounded(1)).unzip();
+  let (mut senders2, receivers2): (Vec<Sender<_>>, Vec<Receiver<_>>) =
+    (0..n_threads).map(|_| bounded(1)).unzip();
   scope(|s| {
     // Producer thread
     s.spawn(|| {
-      let mut rows_chunk = load_n(raw_row_it, chunk_size);
-      while !rows_chunk.is_empty() {
-        snd1
-          .send(rows_chunk)
-          .expect("Unexpected error sending raw rows");
-        rows_chunk = load_n(raw_row_it, chunk_size);
+      {
+        let mut rows_chunk = load_n(raw_row_it, chunk_size);
+        let mut senders_it = senders1.iter().cycle();
+        while !rows_chunk.is_empty() {
+          senders_it
+            .next()
+            .unwrap()
+            .send(rows_chunk)
+            .expect("Unexpected error sending raw rows");
+          rows_chunk = load_n(raw_row_it, chunk_size);
+        }
       }
-      // Close the channel, otherwise sink will never exit the for-loop
-      drop(snd1);
+      // Close the channels, otherwise sink will never exit the for-loop
+      senders1.drain(..).for_each(drop);
     });
     // Parallel processing by n_threads
-    for _ in 0..n_threads {
-      // Send to sink, receive from source
-      let (sendr, recvr) = (snd2.clone(), rcv1.clone());
+    for (sendr2, recvr1) in senders2.iter().cloned().zip(receivers1.iter().cloned()) {
+      // Send to sink, receive from producer
       let schema = schema.clone();
       // Spawn workers in separate threads
       s.spawn(move || {
         // Receive until channel closes
-        for raw_rows_chunk in recvr.iter() {
+        for raw_rows_chunk in recvr1.iter() {
           let converted_raw_rows_chunk = raw_rows_chunk
             .iter()
             .map(|raw_row| convert(raw_row, &schema, separator))
             .collect::<Vec<Box<[u8]>>>();
-          sendr
+          sendr2
             .send(converted_raw_rows_chunk)
             .expect("Unexpected error sending converted rows");
         }
       });
     }
     // Close the channel, otherwise sink will never exit the for-loop
-    drop(snd2);
-    // Sink
-    for raw_rows in rcv2.iter() {
-      for raw_row in raw_rows {
-        match write.write_all(&raw_row) {
-          Ok(()) => (),
-          Err(e) => panic!("Error writing in parallel: {:?}", e),
+    senders2.drain(..).for_each(drop);
+    // Sink in the current thread
+    for recvr2 in receivers2.iter().cycle() {
+      match recvr2.recv() {
+        Ok(raw_rows) => {
+          for raw_row in raw_rows {
+            match write.write_all(&raw_row) {
+              Ok(()) => (),
+              Err(e) => panic!("Error writing in parallel: {:?}", e),
+            }
+          }
+        }
+        Err(_) => {
+          // No more data to be written
+          break;
         }
       }
     }
   });
   Ok(())
 }
```

### Comparing `votable_cli-0.6.0/crates/cli/src/visitors/colnames.rs` & `votable_cli-0.6.1/crates/cli/src/visitors/colnames.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/crates/cli/src/visitors/fieldarray.rs` & `votable_cli-0.6.1/crates/cli/src/visitors/fieldarray.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/crates/cli/src/visitors/mod.rs` & `votable_cli-0.6.1/crates/cli/src/visitors/mod.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/crates/cli/src/visitors/update.rs` & `votable_cli-0.6.1/crates/cli/src/visitors/update.rs`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     }
     unsafe { from_utf8_unchecked(&bytes[from + 1..to]) }
       .parse::<usize>()
       .unwrap()
   }
 }
 
-fn append_to_rm_list(tagvid_to_rm_stack: &mut Vec<Vec<(Tag, String)>>, tag: Tag, vid: String) {
+fn append_to_rm_list(tagvid_to_rm_stack: &mut [Vec<(Tag, String)>], tag: Tag, vid: String) {
   tagvid_to_rm_stack.last_mut().unwrap().push((tag, vid));
 }
 
 impl<C: TableDataContent> VOTableVisitor<C> for UpdateVisitor {
   type E = VOTableError;
 
   type M = DoNothing<Self::E>;
@@ -1044,20 +1044,17 @@
   }
 
   fn visit_values_opt_ended(&mut self, opt: &mut Opt) -> Result<(), Self::E> {
     const TAG: Tag = Tag::OPTION;
     // Going reverse, we do not change the vid of the elements before the ones already removed
     for (tag_to_rm, vid_to_rm) in self.tagvid_to_rm_stack.pop().unwrap().into_iter().rev() {
       trace!("In {}, rm tag {} vid={}", opt.tag(), tag_to_rm, vid_to_rm);
-      match tag_to_rm {
-        Tag::OPTION => {
-          let index = Self::extract_last_digit(vid_to_rm.as_str()) - 1;
-          opt.opts.remove(index);
-        }
-        _ => {}
+      if tag_to_rm == Tag::OPTION {
+        let index = Self::extract_last_digit(vid_to_rm.as_str()) - 1;
+        opt.opts.remove(index);
       }
     }
     // First remove, and then apply other modifications
     let vid = self.get_vid();
     for e in &self.updates_by_tag[TAG.index()] {
       if e.condition.is_ok(vid, None, opt.name.as_ref()) {
         e.action.clone().apply_on_wrapped_elem_mut(
```

### Comparing `votable_cli-0.6.0/crates/cli/src/visitors/viz_org_names.rs` & `votable_cli-0.6.1/crates/cli/src/visitors/viz_org_names.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 //! Retrieve original column name from VizieR column description.
 
+use std::marker::PhantomData;
 use votable::{
   coosys::CooSys,
   data::{fits::Fits, stream::Stream, tabledata::TableData, Data},
   definitions::Definitions,
   desc::Description,
   field::Field,
   fieldref::FieldRef,
@@ -15,42 +16,46 @@
   param::Param,
   paramref::ParamRef,
   resource::Resource,
   table::Table,
   timesys::TimeSys,
   values::{Max, Min, Opt, Values},
   votable::VOTable,
-  VOTableVisitor,
+  TableDataContent, VOTableVisitor,
 };
 
 use super::StringError;
 
 /// Retrieve original column name from VizieR column description and put it
-/// in the 'vizier:org_namee' attribute.
+/// in the 'viz:org_name' attribute.
 /// # Warning
 /// * Based on the content of the parenthesis at the end of the description.
 /// * Use **only** if you are sure that the table description contain the original names
 /// * Else, the ending parenthesis may contain other information (like 'J2000') so you will get rubbish...
-struct ExplicitVizierOrgNamesVisitor;
+pub struct ExplicitVizierOrgNamesVisitor<C: TableDataContent> {
+  _phantom_data: PhantomData<C>,
+}
+
+impl<C: TableDataContent> ExplicitVizierOrgNamesVisitor<C> {
+  pub fn new() -> Self {
+    Self {
+      _phantom_data: PhantomData,
+    }
+  }
+}
 
-impl VOTableVisitor<VoidTableDataContent> for ExplicitVizierOrgNamesVisitor {
+impl<C: TableDataContent> VOTableVisitor<C> for ExplicitVizierOrgNamesVisitor<C> {
   type E = StringError;
 
   type M = DoNothing<Self::E>;
 
-  fn visit_votable_start(
-    &mut self,
-    _votable: &mut VOTable<VoidTableDataContent>,
-  ) -> Result<(), Self::E> {
+  fn visit_votable_start(&mut self, _votable: &mut VOTable<C>) -> Result<(), Self::E> {
     Ok(())
   }
-  fn visit_votable_ended(
-    &mut self,
-    _votable: &mut VOTable<VoidTableDataContent>,
-  ) -> Result<(), Self::E> {
+  fn visit_votable_ended(&mut self, _votable: &mut VOTable<C>) -> Result<(), Self::E> {
     Ok(())
   }
 
   fn visit_description(&mut self, _description: &mut Description) -> Result<(), Self::E> {
     Ok(())
   }
   fn visit_coosys_start(&mut self, _coosys: &mut CooSys) -> Result<(), Self::E> {
@@ -99,15 +104,15 @@
       let desc = desc.get_content_unwrapped().trim();
       if desc.ends_with(')') {
         // Unwrap ok because we tested before that it ended with a ')'.
         if let Some((_, colname)) = desc.strip_suffix(')').unwrap().rsplit_once('(') {
           let colname = colname.trim();
           // No space (unlike in comments) and not an integer (unlike in note reference)
           if !colname.contains(' ') && colname.parse::<u16>().is_err() && colname != "J2000" {
-            field.insert_extra_by_ref("vizier:org_name", colname.into());
+            field.insert_extra_by_ref("viz:org_name", colname.into());
           }
         }
       }
     }
     Ok(())
   }
   fn visit_field_ended(&mut self, _field: &mut Field) -> Result<(), Self::E> {
@@ -120,24 +125,18 @@
   fn visit_definitions_start(&mut self, _coosys: &mut Definitions) -> Result<(), Self::E> {
     Ok(())
   }
   fn visit_definitions_ended(&mut self, _coosys: &mut Definitions) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_resource_start(
-    &mut self,
-    _resource: &mut Resource<VoidTableDataContent>,
-  ) -> Result<(), Self::E> {
+  fn visit_resource_start(&mut self, _resource: &mut Resource<C>) -> Result<(), Self::E> {
     Ok(())
   }
-  fn visit_resource_ended(
-    &mut self,
-    _resource: &mut Resource<VoidTableDataContent>,
-  ) -> Result<(), Self::E> {
+  fn visit_resource_ended(&mut self, _resource: &mut Resource<C>) -> Result<(), Self::E> {
     Ok(())
   }
 
   fn visit_post_info(&mut self, _info: &mut Info) -> Result<(), Self::E> {
     Ok(())
   }
 
@@ -148,44 +147,35 @@
     Ok(())
   }
 
   fn visit_link(&mut self, _link: &mut Link) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_table_start(&mut self, _table: &mut Table<VoidTableDataContent>) -> Result<(), Self::E> {
+  fn visit_table_start(&mut self, _table: &mut Table<C>) -> Result<(), Self::E> {
     Ok(())
   }
-  fn visit_table_ended(&mut self, _table: &mut Table<VoidTableDataContent>) -> Result<(), Self::E> {
+  fn visit_table_ended(&mut self, _table: &mut Table<C>) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_data_start(&mut self, _table: &mut Data<VoidTableDataContent>) -> Result<(), Self::E> {
+  fn visit_data_start(&mut self, _table: &mut Data<C>) -> Result<(), Self::E> {
     Ok(())
   }
-  fn visit_data_ended(&mut self, _table: &mut Data<VoidTableDataContent>) -> Result<(), Self::E> {
+  fn visit_data_ended(&mut self, _table: &mut Data<C>) -> Result<(), Self::E> {
     Ok(())
   }
 
-  fn visit_tabledata(
-    &mut self,
-    _table: &mut TableData<VoidTableDataContent>,
-  ) -> Result<(), Self::E> {
+  fn visit_tabledata(&mut self, _table: &mut TableData<C>) -> Result<(), Self::E> {
     Ok(())
   }
-  fn visit_binary_stream(
-    &mut self,
-    _stream: &mut Stream<VoidTableDataContent>,
-  ) -> Result<(), Self::E> {
+  fn visit_binary_stream(&mut self, _stream: &mut Stream<C>) -> Result<(), Self::E> {
     Ok(())
   }
-  fn visit_binary2_stream(
-    &mut self,
-    _stream: &mut Stream<VoidTableDataContent>,
-  ) -> Result<(), Self::E> {
+  fn visit_binary2_stream(&mut self, _stream: &mut Stream<C>) -> Result<(), Self::E> {
     Ok(())
   }
   fn visit_fits_start(&mut self, _fits: &mut Fits) -> Result<(), Self::E> {
     Ok(())
   }
   fn visit_fits_stream(
     &mut self,
```

### Comparing `votable_cli-0.6.0/crates/cli/src/visitors/votstruct.rs` & `votable_cli-0.6.1/crates/cli/src/visitors/votstruct.rs`

 * *Files identical despite different names*

### Comparing `votable_cli-0.6.0/crates/cli/src/wrappedelems.rs` & `votable_cli-0.6.1/crates/cli/src/wrappedelems.rs`

 * *Files 2% similar despite different names*

```diff
@@ -710,334 +710,421 @@
       Self::FieldRef(e) => e.set_attrs_by_ref(attrs),
       Self::ParamRef(e) => e.set_attrs_by_ref(attrs),
     }
   }
 
   pub fn set_content<S: Into<String>>(self, content: S) -> Result<(), VOTableError> {
     match self {
-      Self::Description(e) => Ok(e.set_content_by_ref(content)),
-      Self::Info(e) => Ok(e.set_content_by_ref(content)),
-      Self::Link(e) => Ok(e.set_content_by_ref(content)),
-      Self::ParamRef(e) => Ok(e.set_content_by_ref(content)),
-      Self::FieldRef(e) => Ok(e.set_content_by_ref(content)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot have a content.",
-        self.tag(),
-      ))),
+      Self::Description(e) => e.set_content_by_ref(content),
+      Self::Info(e) => e.set_content_by_ref(content),
+      Self::Link(e) => e.set_content_by_ref(content),
+      Self::ParamRef(e) => e.set_content_by_ref(content),
+      Self::FieldRef(e) => e.set_content_by_ref(content),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot have a content.",
+          self.tag(),
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn set_description(self, description: Description) -> Result<(), VOTableError> {
     match self {
-      Self::VOTable(e) => Ok(e.reset_description_by_ref(description)),
-      Self::Resource(e) => Ok(e.reset_description_by_ref(description)),
-      Self::Table(e) => Ok(e.reset_description_by_ref(description)),
-      Self::Field(e) => Ok(e.reset_description_by_ref(description)),
-      Self::Param(e) => Ok(e.reset_description_by_ref(description)),
-      Self::Group(e) => Ok(e.reset_description_by_ref(description)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        description.tag()
-      ))),
+      Self::VOTable(e) => e.reset_description_by_ref(description),
+      Self::Resource(e) => e.reset_description_by_ref(description),
+      Self::Table(e) => e.reset_description_by_ref(description),
+      Self::Field(e) => e.reset_description_by_ref(description),
+      Self::Param(e) => e.reset_description_by_ref(description),
+      Self::Group(e) => e.reset_description_by_ref(description),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          description.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn set_definitions(self, definitions: Definitions) -> Result<(), VOTableError> {
     match self {
-      Self::VOTable(e) => Ok(e.reset_definitions_by_ref(definitions)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        definitions.tag()
-      ))),
+      Self::VOTable(e) => e.reset_definitions_by_ref(definitions),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          definitions.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn set_values(self, values: Values) -> Result<(), VOTableError> {
     match self {
-      Self::Field(e) => Ok(e.reset_values_by_ref(values)),
-      Self::Param(e) => Ok(e.reset_values_by_ref(values)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        values.tag()
-      ))),
+      Self::Field(e) => e.reset_values_by_ref(values),
+      Self::Param(e) => e.reset_values_by_ref(values),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          values.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn set_min(self, min: Min) -> Result<(), VOTableError> {
     match self {
-      Self::Values(e) => Ok(e.reset_min_by_ref(min)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        min.tag()
-      ))),
+      Self::Values(e) => e.reset_min_by_ref(min),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          min.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn set_max(self, max: Max) -> Result<(), VOTableError> {
     match self {
-      Self::Values(e) => Ok(e.reset_max_by_ref(max)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        max.tag()
-      ))),
+      Self::Values(e) => e.reset_max_by_ref(max),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          max.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn push_option(self, opt: Opt) -> Result<(), VOTableError> {
     match self {
-      Self::Values(e) => Ok(e.push_opt_by_ref(opt)),
-      Self::Option(e) => Ok(e.push_opt_by_ref(opt)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        opt.tag()
-      ))),
+      Self::Values(e) => e.push_opt_by_ref(opt),
+      Self::Option(e) => e.push_opt_by_ref(opt),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          opt.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn push_info(self, info: Info) -> Result<(), VOTableError> {
     match self {
-      Self::VOTable(e) => Ok(e.push_info_by_ref(info)),
-      Self::Resource(e) => Ok(e.push_info_by_ref(info)),
-      Self::Table(e) => Ok(e.push_info_by_ref(info)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        info.tag()
-      ))),
+      Self::VOTable(e) => e.push_info_by_ref(info),
+      Self::Resource(e) => e.push_info_by_ref(info),
+      Self::Table(e) => e.push_info_by_ref(info),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          info.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn push_post_info(self, info: Info) -> Result<(), VOTableError> {
     match self {
-      Self::VOTable(e) => Ok(e.push_post_info_by_ref(info)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a post-{} tag.",
-        self.tag(),
-        info.tag()
-      ))),
+      Self::VOTable(e) => e.push_post_info_by_ref(info),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a post-{} tag.",
+          self.tag(),
+          info.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn push_coosys(self, coosys: CooSys) -> Result<(), VOTableError> {
     match self {
-      Self::VOTable(e) => Ok(e.push_coosys_by_ref(coosys)),
-      Self::Resource(e) => Ok(e.push_coosys_by_ref(coosys)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {} tag.",
-        self.tag(),
-        coosys.tag()
-      ))),
+      Self::VOTable(e) => e.push_coosys_by_ref(coosys),
+      Self::Resource(e) => e.push_coosys_by_ref(coosys),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {} tag.",
+          self.tag(),
+          coosys.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn push_timesys(self, timesys: TimeSys) -> Result<(), VOTableError> {
     match self {
-      Self::VOTable(e) => Ok(e.push_timesys_by_ref(timesys)),
-      Self::Resource(e) => Ok(e.push_timesys_by_ref(timesys)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        timesys.tag()
-      ))),
+      Self::VOTable(e) => e.push_timesys_by_ref(timesys),
+      Self::Resource(e) => e.push_timesys_by_ref(timesys),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          timesys.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn push_link(self, link: Link) -> Result<(), VOTableError> {
     match self {
       Self::Resource(e) => e.push_link_by_ref(link),
-      Self::Table(e) => Ok(e.push_link_by_ref(link)),
-      Self::Field(e) => Ok(e.push_link_by_ref(link)),
-      Self::Param(e) => Ok(e.push_link_by_ref(link)),
+      Self::Table(e) => {
+        e.push_link_by_ref(link);
+        Ok(())
+      }
+      Self::Field(e) => {
+        e.push_link_by_ref(link);
+        Ok(())
+      }
+      Self::Param(e) => {
+        e.push_link_by_ref(link);
+        Ok(())
+      }
       _ => Err(VOTableError::Custom(format!(
         "Tag '{}' cannot contain a {}.",
         self.tag(),
         link.tag()
       ))),
     }
   }
 
   pub fn push_field(self, field: Field) -> Result<(), VOTableError> {
     match self {
-      Self::Table(e) => Ok(e.push_field_by_ref(field)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        field.tag()
-      ))),
+      Self::Table(e) => e.push_field_by_ref(field),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          field.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn push_param(self, param: Param) -> Result<(), VOTableError> {
     match self {
-      Self::VOTable(e) => Ok(e.push_param_by_ref(param)),
-      Self::Resource(e) => Ok(e.push_param_by_ref(param)),
-      Self::Table(e) => Ok(e.push_param_by_ref(param)),
-      Self::Group(e) => Ok(e.push_param_by_ref(param)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        param.tag()
-      ))),
+      Self::VOTable(e) => e.push_param_by_ref(param),
+      Self::Resource(e) => e.push_param_by_ref(param),
+      Self::Table(e) => e.push_param_by_ref(param),
+      Self::Group(e) => e.push_param_by_ref(param),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          param.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn push_fieldref(self, fieldref: FieldRef) -> Result<(), VOTableError> {
     match self {
-      Self::CooSys(e) => Ok(e.push_fieldref_by_ref(fieldref)),
-      Self::TableGroup(e) => Ok(e.push_fieldref_by_ref(fieldref)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        fieldref.tag()
-      ))),
+      Self::CooSys(e) => e.push_fieldref_by_ref(fieldref),
+      Self::TableGroup(e) => e.push_fieldref_by_ref(fieldref),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          fieldref.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn push_paramref(self, paramref: ParamRef) -> Result<(), VOTableError> {
     match self {
-      Self::CooSys(e) => Ok(e.push_paramref_by_ref(paramref)),
-      Self::Group(e) => Ok(e.push_paramref_by_ref(paramref)),
-      Self::TableGroup(e) => Ok(e.push_paramref_by_ref(paramref)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        paramref.tag()
-      ))),
+      Self::CooSys(e) => e.push_paramref_by_ref(paramref),
+      Self::Group(e) => e.push_paramref_by_ref(paramref),
+      Self::TableGroup(e) => e.push_paramref_by_ref(paramref),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          paramref.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn push_group(self, group: Group) -> Result<(), VOTableError> {
     match self {
-      Self::VOTable(e) => Ok(e.push_group_by_ref(group)),
-      Self::Resource(e) => Ok(e.push_group_by_ref(group)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        group.tag()
-      ))),
+      Self::VOTable(e) => e.push_group_by_ref(group),
+      Self::Resource(e) => e.push_group_by_ref(group),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          group.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn push_tablegroup(self, group: TableGroup) -> Result<(), VOTableError> {
     match self {
-      Self::Table(e) => Ok(e.push_tablegroup_by_ref(group)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        group.tag()
-      ))),
+      Self::Table(e) => e.push_tablegroup_by_ref(group),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          group.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn push_resource(self, resource: Resource<C>) -> Result<(), VOTableError> {
     match self {
-      Self::VOTable(e) => Ok(e.push_resource_by_ref(resource)),
-      Self::Resource(e) => Ok(e.push_resource_by_ref(resource)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        resource.tag()
-      ))),
+      Self::VOTable(e) => e.push_resource_by_ref(resource),
+      Self::Resource(e) => e.push_resource_by_ref(resource),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          resource.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn prepend_resource(self, resource: Resource<C>) -> Result<(), VOTableError> {
     match self {
-      Self::VOTable(e) => Ok(e.prepend_resource_by_ref(resource)),
-      Self::Resource(e) => Ok(e.prepend_resource_by_ref(resource)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        resource.tag()
-      ))),
+      Self::VOTable(e) => e.prepend_resource_by_ref(resource),
+      Self::Resource(e) => e.prepend_resource_by_ref(resource),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          resource.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn push_table(self, table: Table<C>) -> Result<(), VOTableError> {
     match self {
-      Self::Resource(e) => Ok(e.push_table_by_ref(table)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        table.tag()
-      ))),
+      Self::Resource(e) => e.push_table_by_ref(table),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          table.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn set_data(self, data: Data<C>) -> Result<(), VOTableError> {
     match self {
-      Self::Table(e) => Ok(e.set_data_by_ref(data)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        data.tag()
-      ))),
+      Self::Table(e) => e.set_data_by_ref(data),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          data.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn set_binary(self, binary: Binary<C>) -> Result<(), VOTableError> {
     match self {
-      Self::Data(e) => Ok(e.set_binary_by_ref(binary)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        binary.tag()
-      ))),
+      Self::Data(e) => e.set_binary_by_ref(binary),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          binary.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn set_binary2(self, binary: Binary2<C>) -> Result<(), VOTableError> {
     match self {
-      Self::Data(e) => Ok(e.set_binary2_by_ref(binary)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        binary.tag()
-      ))),
+      Self::Data(e) => e.set_binary2_by_ref(binary),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          binary.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn set_fits(self, fits: Fits) -> Result<(), VOTableError> {
     match self {
-      Self::Data(e) => Ok(e.set_fits_by_ref(fits)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        fits.tag()
-      ))),
+      Self::Data(e) => e.set_fits_by_ref(fits),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          fits.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn set_stream(self, stream: Stream<C>) -> Result<(), VOTableError> {
     match self {
-      Self::Binary(e) => Ok(e.set_stream_by_ref(stream)),
-      Self::Binary2(e) => Ok(e.set_stream_by_ref(stream)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        stream.tag()
-      ))),
+      Self::Binary(e) => e.set_stream_by_ref(stream),
+      Self::Binary2(e) => e.set_stream_by_ref(stream),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          stream.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn set_fits_stream(self, stream: Stream<VoidTableDataContent>) -> Result<(), VOTableError> {
     match self {
-      Self::Fits(e) => Ok(e.set_stream_by_ref(stream)),
-      _ => Err(VOTableError::Custom(format!(
-        "Tag '{}' cannot contain a {}.",
-        self.tag(),
-        stream.tag()
-      ))),
+      Self::Fits(e) => e.set_stream_by_ref(stream),
+      _ => {
+        return Err(VOTableError::Custom(format!(
+          "Tag '{}' cannot contain a {}.",
+          self.tag(),
+          stream.tag()
+        )))
+      }
     }
+    Ok(())
   }
 
   pub fn push(self, elem: VOTableWrappedElem<C>) -> Result<(), VOTableError> {
     match elem {
       VOTableWrappedElem::<C>::VOTable(_) => Err(VOTableError::Custom(
         "A VOTable cannot be pushed into another element.".into(),
       )),
```

### Comparing `votable_cli-0.6.0/Cargo.lock` & `votable_cli-0.6.1/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -289,17 +289,17 @@
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quick-error"
 version = "2.0.1"
@@ -313,17 +313,17 @@
 checksum = "11bafc859c6815fbaffbbbf4229ecb767ac913fecb27f9ad4343662e9ef099ea"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -423,17 +423,17 @@
 name = "strsim"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -474,17 +474,17 @@
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
 name = "ucs2"
-version = "0.3.2"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bad643914094137d475641b6bab89462505316ec2ce70907ad20102d28a79ab8"
+checksum = "df79298e11f316400c57ec268f3c2c29ac3c4d4777687955cd3d4f3a35ce7eba"
 dependencies = [
  "bit_field",
 ]
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
@@ -501,15 +501,15 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "votable"
-version = "0.6.0"
+version = "0.6.1"
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
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
  "clap",
  "crossbeam",
  "env_logger",
  "log",
  "serde",
  "votable",
@@ -543,74 +543,81 @@
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
+ "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
-version = "0.6.5"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dffa400e67ed5a4dd237983829e66475f0a4a26938c4b04c21baede6262215b8"
+checksum = "f0c976aaaa0e1f90dbb21e9587cdaf1d9679a1cde8875c0d6bd83ab96a208352"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "wyz"
 version = "0.5.1"
```

### Comparing `votable_cli-0.6.0/Cargo.toml` & `votable_cli-0.6.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "votable"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   "F.-X. Pineau <francois-xavier.pineau@astro.unistra.fr>",
   "T. Dumortier <thibault.dumortier@astro.unistra.fr>"
 ]
 description = """
 Rust implementation of a VOTable serializer/deserializer with support for
 format other than XML, such as JSON, TOML or YAML.
```

### Comparing `votable_cli-0.6.0/pyproject.toml` & `votable_cli-0.6.1/pyproject.toml`

 * *Files identical despite different names*

