# Comparing `tmp/moss_decoder-0.3.1.tar.gz` & `tmp/moss_decoder-0.4.0.tar.gz`

## Comparing `moss_decoder-0.3.1.tar` & `moss_decoder-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 moss_decoder-0.3.1/Cargo.toml
--rw-r--r--   0     1001      123      601 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/.CERN-gitlab-ci.yml
--rw-r--r--   0     1001      123     2835 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      714 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/.gitignore
--rw-r--r--   0     1001      123      757 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     2800 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/README.md
--rw-r--r--   0     1001      123      560 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/moss_decoder.pyi
--rw-r--r--   0     1001      123      641 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/pyproject.toml
--rw-r--r--   0     1001      123  4458776 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/python310.dll
--rw-r--r--   0     1001      123     8378 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/src/lib.rs
--rw-r--r--   0     1001      123     1298 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/src/moss_protocol/moss_hit.rs
--rw-r--r--   0     1001      123     1386 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/src/moss_protocol/moss_packet.rs
--rw-r--r--   0     1001      123     1668 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/src/moss_protocol.rs
--rwxr-xr-x   0     1001      123      427 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/tests/bench_dev_vs_prod.sh
--rw-r--r--   0     1001      123     6055 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/tests/integration.py
--rw-r--r--   0     1001      123     4843 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/tests/integration_test.rs
--rw-r--r--   0     1001      123  9582576 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/tests/moss_noise.raw
--rwxr-xr-x   0     1001      123     1156 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/tests/performance_dev_py.sh
--rwxr-xr-x   0     1001      123      820 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/tests/performance_prod_py.sh
--rw-r--r--   0     1001      123      895 2023-07-25 14:03:59.000000 moss_decoder-0.3.1/tests/utils.sh
--rw-r--r--   0     1001      123     8066 2023-07-25 14:04:05.000000 moss_decoder-0.3.1/Cargo.lock
--rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 moss_decoder-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 moss_decoder-0.4.0/Cargo.toml
+-rw-r--r--   0     1001      123      601 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/.CERN-gitlab-ci.yml
+-rw-r--r--   0     1001      123     2835 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      714 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/.gitignore
+-rw-r--r--   0     1001      123      757 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     2800 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/README.md
+-rw-r--r--   0     1001      123      560 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/moss_decoder.pyi
+-rw-r--r--   0     1001      123      641 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/pyproject.toml
+-rw-r--r--   0     1001      123  4458776 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/python310.dll
+-rw-r--r--   0     1001      123     8390 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/src/lib.rs
+-rw-r--r--   0     1001      123     1880 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/src/moss_protocol/moss_hit.rs
+-rw-r--r--   0     1001      123     1843 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/src/moss_protocol/moss_packet.rs
+-rw-r--r--   0     1001      123     1668 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/src/moss_protocol.rs
+-rwxr-xr-x   0     1001      123      427 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/tests/bench_dev_vs_prod.sh
+-rw-r--r--   0     1001      123     7098 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/tests/integration.py
+-rw-r--r--   0     1001      123     4858 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/tests/integration_test.rs
+-rw-r--r--   0     1001      123  9582576 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/tests/moss_noise.raw
+-rwxr-xr-x   0     1001      123     1156 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/tests/performance_dev_py.sh
+-rwxr-xr-x   0     1001      123      820 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/tests/performance_prod_py.sh
+-rw-r--r--   0     1001      123      895 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/tests/utils.sh
+-rw-r--r--   0     1001      123     8066 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/Cargo.lock
+-rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 moss_decoder-0.4.0/PKG-INFO
```

### Comparing `moss_decoder-0.3.1/Cargo.toml` & `moss_decoder-0.4.0/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "moss_decoder"
-version = "0.3.1"
+version = "0.4.0"
 edition = "2021"
 authors = ["Marc Beck König <mbkj@tutamail.com>"]
 license = "MIT OR Apache-2.0"
 description = "Python module providing a decoder for the MOSS chip protocol."
 categories = ["python-module"]
```

### Comparing `moss_decoder-0.3.1/.CERN-gitlab-ci.yml` & `moss_decoder-0.4.0/.CERN-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.3.1/.github/workflows/CI.yml` & `moss_decoder-0.4.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.3.1/.gitignore` & `moss_decoder-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.3.1/.pre-commit-config.yaml` & `moss_decoder-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.3.1/README.md` & `moss_decoder-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.3.1/moss_decoder.pyi` & `moss_decoder-0.4.0/moss_decoder.pyi`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.3.1/pyproject.toml` & `moss_decoder-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.3.1/python310.dll` & `moss_decoder-0.4.0/python310.dll`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.3.1/src/lib.rs` & `moss_decoder-0.4.0/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
 const READER_BUFFER_CAPACITY: usize = 10 * 1024 * 1024; // 10 MiB
 
 #[pyfunction]
 /// Decodes a file containing raw MOSS data into a list of [MossPacket]s
 ///
 /// The file is read in chunks of 10 MiB until the end of the file is reached.
-pub fn decode_from_file(path: String) -> PyResult<Vec<MossPacket>> {
+pub fn decode_from_file(path: std::path::PathBuf) -> PyResult<Vec<MossPacket>> {
     // Open file (get file descriptor)
     let file = match std::fs::File::open(path) {
         Ok(file) => file,
         Err(e) => return Err(PyFileNotFoundError::new_err(e.to_string())),
     };
 
     // Create buffered reader with 1MB capacity to minimize syscalls to read
```

### Comparing `moss_decoder-0.3.1/src/moss_protocol/moss_hit.rs` & `moss_decoder-0.4.0/src/moss_protocol/moss_hit.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 //! struct representation of a single hit from a MOSS region.
 use pyo3::prelude::*;
+use pyo3::pyclass::CompareOp;
 use std::fmt::write;
 use std::fmt::Display;
 
 #[pyclass(get_all)]
-#[derive(Debug, Default, Clone, Copy, PartialEq)]
+#[derive(Debug, Default, Clone, Copy, PartialEq, PartialOrd, Eq, Ord)]
 /// A single hit from a MOSS region.
 pub struct MossHit {
     /// The region ID of the hit.
     pub region: u8,
     /// The row of the hit.
     pub row: u16,
     /// The column of the hit.
@@ -22,18 +23,35 @@
         Self {
             region,
             row,
             column,
         }
     }
 
+    fn __repr__(slf: &PyCell<Self>) -> PyResult<String> {
+        let class_name: &str = slf.get_type().name()?;
+        Ok(format!(
+            "{}({} {} {})",
+            class_name,
+            slf.borrow().region,
+            slf.borrow().row,
+            slf.borrow().column
+        ))
+    }
+
     /// Returns a string representation of the [MossHit] instance.
     pub fn __str__(&self) -> String {
         self.to_string()
     }
+
+    fn __richcmp__(&self, other: &Self, op: CompareOp) -> bool {
+        op.matches(self.region.cmp(&other.region))
+            && op.matches(self.row.cmp(&other.row))
+            && op.matches(self.column.cmp(&other.column))
+    }
 }
 
 impl Display for MossHit {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write(
             f,
             format_args!(
```

### Comparing `moss_decoder-0.3.1/src/moss_protocol.rs` & `moss_decoder-0.4.0/src/moss_protocol.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.3.1/tests/integration.py` & `moss_decoder-0.4.0/tests/integration.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Integration tests. Uses the `moss_decoder` package
 from python and allows benchmarks."""
 import sys  # Don't want to depend on `argparse`
 import time
 from pathlib import Path
 import moss_decoder
-from moss_decoder import MossPacket, decode_event
+from moss_decoder import MossPacket, decode_event, MossHit
 
 FILE_PATH = Path("tests/moss_noise.raw")
 
 
 def read_bytes_from_file(file_path: Path) -> bytes:
     """Open file at `file_path` and read as binary, return `bytes`"""
     with open(file_path, "rb") as readout_file:
@@ -167,22 +167,61 @@
 
     assert (
         remainder_count == 1
     ), f"Expected last trailer found at index 1, got: {remainder_count}"
     print("==> Test OK\n\n")
 
 
+def test_fundamental_class_comparisons():
+    """Test fundamental class functionality"""
+
+    print("=== Comparing MossHit attributes ===\n")
+    hit_a = MossHit(0, 1, 2)
+    hit_b = MossHit(0, 1, 2)
+    assert hit_a == hit_b, f"{hit_a} != {hit_b}"
+    print("__eq__ is OK")
+
+    print(repr(hit_a) + " == " + repr(hit_a))
+    assert repr(hit_a) == repr(hit_b)
+    print("__repr__ is OK")
+
+    print(str(hit_a) + " == " + str(hit_b))
+    assert str(hit_a) == str(hit_b)
+
+    print("__str__ is OK")
+    print("==> MossHit is OK\n\n")
+
+    print("=== Comparing MossPacket attributes ===\n")
+    pack_a = MossPacket(1)
+    pack_b = MossPacket(1)
+    assert pack_a == pack_b, f"{pack_a} != {pack_b}"
+    print("__eq__ is OK")
+
+    print(repr(pack_a) + " == " + repr(pack_b))
+    assert repr(pack_a) == repr(pack_b)
+    print("__repr__ is OK")
+
+    print(str(pack_a) + " == " + str(pack_b))
+    assert str(pack_a) == str(pack_b)
+    print("__str__ is OK")
+
+    print("==> MossPacket is OK\n\n")
+
+
 if __name__ == "__main__":
     args = sys.argv
 
     if len(args) > 1:
         if args[1] == "benchmark":
             # Just run this and then exit
             test_decode_multi_event()
             sys.exit(0)
+
+    test_fundamental_class_comparisons()
+
     start = time.time()
     test_decode_multi_event()
     print(f"Done in: {time.time()-start:.3f} s\n")
     start = time.time()
     test_moss_packet_print()
     print(f"Done in: {time.time()-start:.3f} s\n")
     start = time.time()
```

### Comparing `moss_decoder-0.3.1/tests/integration_test.rs` & `moss_decoder-0.4.0/tests/integration_test.rs`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,16 @@
     assert_eq!(p.len(), 100000, "Expected 100k packets, got {}", p.len());
 }
 
 #[test]
 fn test_decode_from_file() {
     let time = std::time::Instant::now();
 
-    let packets = moss_decoder::decode_from_file("tests/moss_noise.raw".to_string()).unwrap();
+    let packets =
+        moss_decoder::decode_from_file("tests/moss_noise.raw".to_string().into()).unwrap();
     println!("Decoded in: {t:?}\n", t = time.elapsed());
 
     println!("Got: {packets}", packets = packets.len());
 
     assert_eq!(
         packets.len(),
         100000,
```

### Comparing `moss_decoder-0.3.1/tests/moss_noise.raw` & `moss_decoder-0.4.0/tests/moss_noise.raw`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.3.1/tests/performance_dev_py.sh` & `moss_decoder-0.4.0/tests/performance_dev_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.3.1/tests/performance_prod_py.sh` & `moss_decoder-0.4.0/tests/performance_prod_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.3.1/tests/utils.sh` & `moss_decoder-0.4.0/tests/utils.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.3.1/Cargo.lock` & `moss_decoder-0.4.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "moss_decoder"
-version = "0.3.1"
+version = "0.4.0"
 dependencies = [
  "pretty_assertions",
  "pyo3",
 ]
 
 [[package]]
 name = "once_cell"
```

### Comparing `moss_decoder-0.3.1/PKG-INFO` & `moss_decoder-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moss_decoder
-Version: 0.3.1
+Version: 0.4.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python package implemented in Rust to decode MOSS readout data
 Author: Marc Beck König
 Author-email: marc.beck.konig@cern.ch
 Maintainer-email: Marc Beck König <marc.beck.konig@cern.ch>
```

