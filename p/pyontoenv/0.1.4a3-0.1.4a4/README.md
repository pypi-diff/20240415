# Comparing `tmp/pyontoenv-0.1.4a3.tar.gz` & `tmp/pyontoenv-0.1.4a4.tar.gz`

## Comparing `pyontoenv-0.1.4a3.tar` & `pyontoenv-0.1.4a4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0      501       20      776 2024-04-05 16:43:55.000000 pyontoenv-0.1.4a3/lib/Cargo.toml
--rw-r--r--   0      501       20     5324 2024-04-14 16:26:59.000000 pyontoenv-0.1.4a3/lib/src/config.rs
--rw-r--r--   0      501       20     2071 2024-04-06 02:39:54.000000 pyontoenv-0.1.4a3/lib/src/consts.rs
--rw-r--r--   0      501       20     3267 2024-04-05 19:54:52.000000 pyontoenv-0.1.4a3/lib/src/doctor.rs
--rw-r--r--   0      501       20      350 2024-04-14 15:35:07.000000 pyontoenv-0.1.4a3/lib/src/errors.rs
--rw-r--r--   0      501       20    39347 2024-04-14 16:49:50.000000 pyontoenv-0.1.4a3/lib/src/lib.rs
--rw-r--r--   0      501       20    13633 2024-04-14 04:36:13.000000 pyontoenv-0.1.4a3/lib/src/ontology.rs
--rw-r--r--   0      501       20     3521 2024-04-05 19:55:30.000000 pyontoenv-0.1.4a3/lib/src/policy.rs
--rw-r--r--   0      501       20     6428 2024-04-14 16:50:33.000000 pyontoenv-0.1.4a3/lib/src/util.rs
--rw-r--r--   0      501       20  1689944 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/Brick-1.3.ttl
--rw-r--r--   0      501       20     1248 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/model
--rw-r--r--   0      501       20      321 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/model.n3
--rw-r--r--   0      501       20      537 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/model.nt
--rw-r--r--   0      501       20     1248 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/model.ttl
--rw-r--r--   0      501       20      789 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/model.xml
--rw-r--r--   0      501       20      909 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl
--rw-r--r--   0      501       20   146214 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
--rw-r--r--   0      501       20    30521 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
--rw-r--r--   0      501       20   163975 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
--rw-r--r--   0      501       20    18438 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl
--rw-r--r--   0      501       20    18438 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
--rw-r--r--   0      501       20  1323794 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
--rw-r--r--   0      501       20    17472 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
--rw-r--r--   0      501       20  1456008 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
--rw-r--r--   0      501       20   104496 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
--rw-r--r--   0      501       20  1255550 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/bacnet.ttl
--rw-r--r--   0      501       20    44502 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/brickpatches.ttl
--rw-r--r--   0      501       20    81761 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/rec.ttl
--rw-r--r--   0      501       20     4069 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/recimports.ttl
--rw-r--r--   0      501       20    11876 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/lib/tests/data/support/ref-schema.ttl
--rw-r--r--   0      501       20     1160 2024-04-09 16:33:12.000000 pyontoenv-0.1.4a3/lib/tests/data2/ont1.ttl
--rw-r--r--   0      501       20     1132 2024-04-09 16:33:13.000000 pyontoenv-0.1.4a3/lib/tests/data2/ont2.ttl
--rw-r--r--   0      501       20     1135 2024-04-09 16:33:29.000000 pyontoenv-0.1.4a3/lib/tests/data2/ont3.ttl
--rw-r--r--   0      501       20     1106 2024-04-09 16:33:46.000000 pyontoenv-0.1.4a3/lib/tests/data2/ont4.ttl
--rw-r--r--   0      501       20     1248 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a3/lib/tests/fileendings/model
--rw-r--r--   0      501       20      321 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a3/lib/tests/fileendings/model.n3
--rw-r--r--   0      501       20      537 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a3/lib/tests/fileendings/model.nt
--rw-r--r--   0      501       20     1248 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a3/lib/tests/fileendings/model.ttl
--rw-r--r--   0      501       20      789 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a3/lib/tests/fileendings/model.xml
--rw-r--r--   0      501       20  1689944 2024-04-03 15:52:01.000000 pyontoenv-0.1.4a3/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl
--rw-r--r--   0      501       20     1160 2024-04-09 19:04:23.000000 pyontoenv-0.1.4a3/lib/tests/updates/v1/ont1.ttl
--rw-r--r--   0      501       20     1132 2024-04-09 19:04:23.000000 pyontoenv-0.1.4a3/lib/tests/updates/v1/ont2.ttl
--rw-r--r--   0      501       20     1135 2024-04-09 19:04:48.000000 pyontoenv-0.1.4a3/lib/tests/updates/v1/ont3.ttl
--rw-r--r--   0      501       20     1106 2024-04-09 19:05:31.000000 pyontoenv-0.1.4a3/lib/tests/updates/v1/ont4.ttl
--rw-r--r--   0      501       20     1135 2024-04-09 19:05:07.000000 pyontoenv-0.1.4a3/lib/tests/updates/v2/ont3.ttl
--rw-r--r--   0      501       20     1129 2024-04-10 00:42:38.000000 pyontoenv-0.1.4a3/lib/tests/updates/v2/ont5.ttl
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.4a3/python/Cargo.toml
--rw-r--r--   0      501       20     2886 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/python/.github/workflows/CI.yml
--rw-r--r--   0      501       20      686 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/python/.gitignore
--rw-r--r--   0      501       20       71 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a3/python/build.rs
--rw-r--r--   0      501       20     5241 2024-04-14 04:04:40.000000 pyontoenv-0.1.4a3/python/poetry.lock
--rw-r--r--   0      501       20       71 2024-04-05 23:45:30.000000 pyontoenv-0.1.4a3/python/requirements.dev.txt
--rw-r--r--   0      501       20    11344 2024-04-14 19:53:50.000000 pyontoenv-0.1.4a3/python/src/lib.rs
--rw-r--r--   0      501       20      452 2024-04-14 18:03:51.000000 pyontoenv-0.1.4a3/python/test.py
--rw-r--r--   0      501       20      206 2024-04-13 23:20:44.000000 pyontoenv-0.1.4a3/python/token
--rw-r--r--   0      501       20    73476 2024-04-14 19:51:01.000000 pyontoenv-0.1.4a3/Cargo.lock
--rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 pyontoenv-0.1.4a3/Cargo.toml
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 pyontoenv-0.1.4a3/pyproject.toml
--rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 pyontoenv-0.1.4a3/PKG-INFO
+-rw-r--r--   0      501       20      776 2024-04-05 16:43:55.000000 pyontoenv-0.1.4a4/lib/Cargo.toml
+-rw-r--r--   0      501       20     5324 2024-04-14 16:26:59.000000 pyontoenv-0.1.4a4/lib/src/config.rs
+-rw-r--r--   0      501       20     2071 2024-04-06 02:39:54.000000 pyontoenv-0.1.4a4/lib/src/consts.rs
+-rw-r--r--   0      501       20     3267 2024-04-05 19:54:52.000000 pyontoenv-0.1.4a4/lib/src/doctor.rs
+-rw-r--r--   0      501       20      350 2024-04-14 15:35:07.000000 pyontoenv-0.1.4a4/lib/src/errors.rs
+-rw-r--r--   0      501       20    39347 2024-04-14 16:49:50.000000 pyontoenv-0.1.4a4/lib/src/lib.rs
+-rw-r--r--   0      501       20    13633 2024-04-14 04:36:13.000000 pyontoenv-0.1.4a4/lib/src/ontology.rs
+-rw-r--r--   0      501       20     3521 2024-04-05 19:55:30.000000 pyontoenv-0.1.4a4/lib/src/policy.rs
+-rw-r--r--   0      501       20     6428 2024-04-14 16:50:33.000000 pyontoenv-0.1.4a4/lib/src/util.rs
+-rw-r--r--   0      501       20  1689944 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/Brick-1.3.ttl
+-rw-r--r--   0      501       20     1248 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/model
+-rw-r--r--   0      501       20      321 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/model.n3
+-rw-r--r--   0      501       20      537 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/model.nt
+-rw-r--r--   0      501       20     1248 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/model.ttl
+-rw-r--r--   0      501       20      789 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/model.xml
+-rw-r--r--   0      501       20      909 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl
+-rw-r--r--   0      501       20   146214 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
+-rw-r--r--   0      501       20    30521 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
+-rw-r--r--   0      501       20   163975 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
+-rw-r--r--   0      501       20    18438 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl
+-rw-r--r--   0      501       20    18438 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
+-rw-r--r--   0      501       20  1323794 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
+-rw-r--r--   0      501       20    17472 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0      501       20  1456008 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0      501       20   104496 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
+-rw-r--r--   0      501       20  1255550 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/bacnet.ttl
+-rw-r--r--   0      501       20    44502 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/brickpatches.ttl
+-rw-r--r--   0      501       20    81761 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/rec.ttl
+-rw-r--r--   0      501       20     4069 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/recimports.ttl
+-rw-r--r--   0      501       20    11876 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/lib/tests/data/support/ref-schema.ttl
+-rw-r--r--   0      501       20     1160 2024-04-09 16:33:12.000000 pyontoenv-0.1.4a4/lib/tests/data2/ont1.ttl
+-rw-r--r--   0      501       20     1132 2024-04-09 16:33:13.000000 pyontoenv-0.1.4a4/lib/tests/data2/ont2.ttl
+-rw-r--r--   0      501       20     1135 2024-04-09 16:33:29.000000 pyontoenv-0.1.4a4/lib/tests/data2/ont3.ttl
+-rw-r--r--   0      501       20     1106 2024-04-09 16:33:46.000000 pyontoenv-0.1.4a4/lib/tests/data2/ont4.ttl
+-rw-r--r--   0      501       20     1248 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a4/lib/tests/fileendings/model
+-rw-r--r--   0      501       20      321 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a4/lib/tests/fileendings/model.n3
+-rw-r--r--   0      501       20      537 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a4/lib/tests/fileendings/model.nt
+-rw-r--r--   0      501       20     1248 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a4/lib/tests/fileendings/model.ttl
+-rw-r--r--   0      501       20      789 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a4/lib/tests/fileendings/model.xml
+-rw-r--r--   0      501       20  1689944 2024-04-03 15:52:01.000000 pyontoenv-0.1.4a4/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl
+-rw-r--r--   0      501       20     1160 2024-04-09 19:04:23.000000 pyontoenv-0.1.4a4/lib/tests/updates/v1/ont1.ttl
+-rw-r--r--   0      501       20     1132 2024-04-09 19:04:23.000000 pyontoenv-0.1.4a4/lib/tests/updates/v1/ont2.ttl
+-rw-r--r--   0      501       20     1135 2024-04-09 19:04:48.000000 pyontoenv-0.1.4a4/lib/tests/updates/v1/ont3.ttl
+-rw-r--r--   0      501       20     1106 2024-04-09 19:05:31.000000 pyontoenv-0.1.4a4/lib/tests/updates/v1/ont4.ttl
+-rw-r--r--   0      501       20     1135 2024-04-09 19:05:07.000000 pyontoenv-0.1.4a4/lib/tests/updates/v2/ont3.ttl
+-rw-r--r--   0      501       20     1129 2024-04-10 00:42:38.000000 pyontoenv-0.1.4a4/lib/tests/updates/v2/ont5.ttl
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.4a4/python/Cargo.toml
+-rw-r--r--   0      501       20     2886 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/python/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      686 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/python/.gitignore
+-rw-r--r--   0      501       20       71 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a4/python/build.rs
+-rw-r--r--   0      501       20     5241 2024-04-14 04:04:40.000000 pyontoenv-0.1.4a4/python/poetry.lock
+-rw-r--r--   0      501       20       71 2024-04-05 23:45:30.000000 pyontoenv-0.1.4a4/python/requirements.dev.txt
+-rw-r--r--   0      501       20    11375 2024-04-14 20:02:30.000000 pyontoenv-0.1.4a4/python/src/lib.rs
+-rw-r--r--   0      501       20      452 2024-04-14 18:03:51.000000 pyontoenv-0.1.4a4/python/test.py
+-rw-r--r--   0      501       20      206 2024-04-13 23:20:44.000000 pyontoenv-0.1.4a4/python/token
+-rw-r--r--   0      501       20    73476 2024-04-14 21:12:36.000000 pyontoenv-0.1.4a4/Cargo.lock
+-rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 pyontoenv-0.1.4a4/Cargo.toml
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 pyontoenv-0.1.4a4/pyproject.toml
+-rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 pyontoenv-0.1.4a4/PKG-INFO
```

### Comparing `pyontoenv-0.1.4a3/lib/Cargo.toml` & `pyontoenv-0.1.4a4/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/src/config.rs` & `pyontoenv-0.1.4a4/lib/src/config.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/src/consts.rs` & `pyontoenv-0.1.4a4/lib/src/consts.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/src/doctor.rs` & `pyontoenv-0.1.4a4/lib/src/doctor.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/src/lib.rs` & `pyontoenv-0.1.4a4/lib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/src/ontology.rs` & `pyontoenv-0.1.4a4/lib/src/ontology.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/src/policy.rs` & `pyontoenv-0.1.4a4/lib/src/policy.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/src/util.rs` & `pyontoenv-0.1.4a4/lib/src/util.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/Brick-1.3.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/Brick-1.3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/model` & `pyontoenv-0.1.4a4/lib/tests/data/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/model.nt` & `pyontoenv-0.1.4a4/lib/tests/data/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/model.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/model.xml` & `pyontoenv-0.1.4a4/lib/tests/data/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/bacnet.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/bacnet.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/brickpatches.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/brickpatches.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/rec.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/rec.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/recimports.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/recimports.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data/support/ref-schema.ttl` & `pyontoenv-0.1.4a4/lib/tests/data/support/ref-schema.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data2/ont1.ttl` & `pyontoenv-0.1.4a4/lib/tests/data2/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data2/ont2.ttl` & `pyontoenv-0.1.4a4/lib/tests/data2/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data2/ont3.ttl` & `pyontoenv-0.1.4a4/lib/tests/data2/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/data2/ont4.ttl` & `pyontoenv-0.1.4a4/lib/tests/data2/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/fileendings/model` & `pyontoenv-0.1.4a4/lib/tests/fileendings/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/fileendings/model.nt` & `pyontoenv-0.1.4a4/lib/tests/fileendings/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/fileendings/model.ttl` & `pyontoenv-0.1.4a4/lib/tests/fileendings/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/fileendings/model.xml` & `pyontoenv-0.1.4a4/lib/tests/fileendings/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl` & `pyontoenv-0.1.4a4/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/updates/v1/ont1.ttl` & `pyontoenv-0.1.4a4/lib/tests/updates/v1/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/updates/v1/ont2.ttl` & `pyontoenv-0.1.4a4/lib/tests/updates/v1/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/updates/v1/ont3.ttl` & `pyontoenv-0.1.4a4/lib/tests/updates/v1/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/updates/v1/ont4.ttl` & `pyontoenv-0.1.4a4/lib/tests/updates/v1/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/updates/v2/ont3.ttl` & `pyontoenv-0.1.4a4/lib/tests/updates/v2/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/lib/tests/updates/v2/ont5.ttl` & `pyontoenv-0.1.4a4/lib/tests/updates/v2/ont5.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/python/Cargo.toml` & `pyontoenv-0.1.4a4/python/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/python/.github/workflows/CI.yml` & `pyontoenv-0.1.4a4/python/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/python/.gitignore` & `pyontoenv-0.1.4a4/python/.gitignore`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/python/poetry.lock` & `pyontoenv-0.1.4a4/python/poetry.lock`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a3/python/src/lib.rs` & `pyontoenv-0.1.4a4/python/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -283,14 +283,15 @@
     fn add(&mut self, _py: Python, location: &Bound<'_, PyAny>) -> PyResult<()> {
         let location =
             OntologyLocation::from_str(&location.to_string()).map_err(anyhow_to_pyerr)?;
         self.inner.add(location).map_err(anyhow_to_pyerr)?;
         Ok(())
     }
 
+    #[pyo3(signature = (uri))]
     fn get_graph(&self, py: Python, uri: &Bound<'_, PyString>) -> PyResult<Py<PyAny>> {
         let rdflib = py.import_bound("rdflib")?;
         let iri = NamedNode::new(uri.to_string())
             .map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(e.to_string()))?;
         let graph = self
             .inner
             .get_graph_by_name(iri.as_ref())
```

### Comparing `pyontoenv-0.1.4a3/Cargo.lock` & `pyontoenv-0.1.4a4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1400,15 +1400,15 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "ontoenv"
-version = "0.1.4-alpha3"
+version = "0.1.4-alpha4"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "derive_builder",
  "env_logger",
  "glob",
@@ -1426,15 +1426,15 @@
  "tempdir",
  "tempfile",
  "walkdir",
 ]
 
 [[package]]
 name = "ontoenv-cli"
-version = "0.1.4-alpha3"
+version = "0.1.4-alpha4"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "env_logger",
  "ontoenv",
  "oxigraph",
@@ -1794,15 +1794,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyontoenv"
-version = "0.1.4-alpha3"
+version = "0.1.4-alpha4"
 dependencies = [
  "anyhow",
  "env_logger",
  "log",
  "ontoenv",
  "oxigraph",
  "pyo3",
```

### Comparing `pyontoenv-0.1.4a3/Cargo.toml` & `pyontoenv-0.1.4a4/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["python"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.4-alpha3"
+version = "0.1.4-alpha4"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "BSD-3-Clause"
 edition = "2021"
 rust-version = "1.70"
 repository = "https://github.com/gtfierro/ontoenv-rs"
 homepage = "https://github.com/gtfierro/ontoenv-rs"
 description = "A tool for managing ontologies and their dependencies"
@@ -26,8 +26,8 @@
 glob = "0.3.1"
 chrono = { version = "0.4.33", features = ["serde"] }
 petgraph = { version = "0.6.4", features = ["serde-1"] }
 clap = { version = "4.4.18", features = ["derive"] }
 derive_builder = "0.13.0"
 oxigraph = "0.3.22"
 
-ontoenv = { version = "0.1.4-alpha2", path = "lib" }
+ontoenv = { version = "0.1.4-alpha4", path = "lib" }
```

### Comparing `pyontoenv-0.1.4a3/pyproject.toml` & `pyontoenv-0.1.4a4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 manifest-path = "python/Cargo.toml"
 
 [tool.poetry]
 name = "ontoenv"
-version = "0.1.4a3"
+version = "0.1.4a4"
 description = "Python bindings for the OntoEnv Rust library. Manages ontology-based environments for building knowledge graphs."
 license = "bsd-3-clause"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pyontoenv-0.1.4a3/PKG-INFO` & `pyontoenv-0.1.4a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyontoenv
-Version: 0.1.4a3
+Version: 0.1.4a4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Command line tool to manage ontologies and their imports in a local environment
 Home-Page: https://github.com/gtfierro/ontoenv-rs
 Author: Gabe Fierro <gtfierro@mines.edu>
 Author-email: Gabe Fierro <gtfierro@mines.edu>
```

