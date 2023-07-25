# Comparing `tmp/moss_decoder-0.1.3.tar.gz` & `tmp/moss_decoder-0.3.0.tar.gz`

## Comparing `moss_decoder-0.1.3.tar` & `moss_decoder-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 moss_decoder-0.1.3/Cargo.toml
--rw-r--r--   0     1001      123     2835 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      713 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/.gitignore
--rw-r--r--   0     1001      123     1395 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/README.md
--rw-r--r--   0     1001      123      641 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/pyproject.toml
--rw-r--r--   0     1001      123  4458776 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/python310.dll
--rw-r--r--   0     1001      123     4806 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/src/lib.rs
--rw-r--r--   0     1001      123     1039 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/src/moss_protocol/moss_hit.rs
--rw-r--r--   0     1001      123     1220 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/src/moss_protocol/moss_packet.rs
--rw-r--r--   0     1001      123     1536 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/src/moss_protocol.rs
--rw-r--r--   0     1001      123     2773 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/tests/integration.py
--rw-r--r--   0     1001      123     4416 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/tests/integration_test.rs
--rw-r--r--   0     1001      123  9582576 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/tests/moss_noise.raw
--rwxr-xr-x   0     1001      123      660 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/tests/performance_dev_py.sh
--rwxr-xr-x   0     1001      123      620 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/tests/performance_prod_py.sh
--rw-r--r--   0     1001      123     8066 2023-07-24 12:50:35.000000 moss_decoder-0.1.3/Cargo.lock
--rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 moss_decoder-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 moss_decoder-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123      601 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/.CERN-gitlab-ci.yml
+-rw-r--r--   0     1001      123     2835 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      714 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/.gitignore
+-rw-r--r--   0     1001      123      757 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     2800 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/README.md
+-rw-r--r--   0     1001      123      560 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/moss_decoder.pyi
+-rw-r--r--   0     1001      123      641 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123  4458776 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/python310.dll
+-rw-r--r--   0     1001      123     8220 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123     1039 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/src/moss_protocol/moss_hit.rs
+-rw-r--r--   0     1001      123     1220 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/src/moss_protocol/moss_packet.rs
+-rw-r--r--   0     1001      123     1578 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/src/moss_protocol.rs
+-rwxr-xr-x   0     1001      123      427 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/tests/bench_dev_vs_prod.sh
+-rw-r--r--   0     1001      123     5869 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/tests/integration.py
+-rw-r--r--   0     1001      123     4843 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/tests/integration_test.rs
+-rw-r--r--   0     1001      123  9582576 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/tests/moss_noise.raw
+-rwxr-xr-x   0     1001      123     1156 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/tests/performance_dev_py.sh
+-rwxr-xr-x   0     1001      123      820 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/tests/performance_prod_py.sh
+-rw-r--r--   0     1001      123      895 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/tests/utils.sh
+-rw-r--r--   0     1001      123     8066 2023-07-25 13:10:47.000000 moss_decoder-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 moss_decoder-0.3.0/PKG-INFO
```

### Comparing `moss_decoder-0.1.3/Cargo.toml` & `moss_decoder-0.3.0/Cargo.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "moss_decoder"
-version = "0.1.3"
+version = "0.3.0"
 edition = "2021"
 authors = ["Marc Beck König <mbkj@tutamail.com>"]
 license = "MIT OR Apache-2.0"
 description = "Python module providing a decoder for the MOSS chip protocol."
 categories = ["python-module"]
```

### Comparing `moss_decoder-0.1.3/.github/workflows/CI.yml` & `moss_decoder-0.3.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.1.3/.gitignore` & `moss_decoder-0.3.0/.gitignore`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,8 @@
 # PyCharm
 .idea/
 
 # VSCode
 .vscode/
 
 # Pyenv
-.python-version
+.python-version
```

### Comparing `moss_decoder-0.1.3/pyproject.toml` & `moss_decoder-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.1.3/python310.dll` & `moss_decoder-0.3.0/python310.dll`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.1.3/src/moss_protocol/moss_hit.rs` & `moss_decoder-0.3.0/src/moss_protocol/moss_hit.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.1.3/src/moss_protocol/moss_packet.rs` & `moss_decoder-0.3.0/src/moss_protocol/moss_packet.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.1.3/src/moss_protocol.rs` & `moss_decoder-0.3.0/src/moss_protocol.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 pub mod moss_hit;
 pub mod moss_packet;
 pub use moss_hit::MossHit;
 pub use moss_packet::MossPacket;
 
+#[derive(Debug, PartialEq)]
 pub(crate) enum MossWord {
     Idle,
     UnitFrameHeader,
     UnitFrameTrailer,
     RegionHeader,
     Data0,
     Data1,
@@ -23,19 +24,19 @@
     const DATA_1: u8 = 0b0100_0000; // 01_<hit_row_pos[2:0]>_<hit_col_pos[8:6]>
     const DATA_2: u8 = 0b1000_0000; // 10_<hit_col_pos[5:0]>
     const DELIMITER: u8 = 0xFA; // subject to change (FPGA implementation detail)
 
     pub fn from_byte(b: u8) -> MossWord {
         match b {
             // Exact matches
-            Self::IDLE => Self::Idle,
-            Self::UNIT_FRAME_TRAILER => Self::UnitFrameTrailer,
-            six_msb if six_msb & 0b1111_1100 == Self::REGION_HEADER => Self::RegionHeader,
-            four_msb if four_msb & 0b1111_0000 == Self::UNIT_FRAME_HEADER => Self::UnitFrameHeader,
+            Self::IDLE => MossWord::Idle,
+            Self::UNIT_FRAME_TRAILER => MossWord::UnitFrameTrailer,
+            six_msb if six_msb & 0xFC == Self::REGION_HEADER => MossWord::RegionHeader,
+            four_msb if four_msb & 0xF0 == Self::UNIT_FRAME_HEADER => MossWord::UnitFrameHeader,
             Self::DELIMITER => Self::Delimiter,
-            two_msb if two_msb & 0b1100_0000 == Self::DATA_0 => Self::Data0,
-            two_msb if two_msb & 0b1100_0000 == Self::DATA_1 => Self::Data1,
-            two_msb if two_msb & 0b1100_0000 == Self::DATA_2 => Self::Data2,
+            two_msb if two_msb & 0b1100_0000 == Self::DATA_0 => MossWord::Data0,
+            two_msb if two_msb & 0b1100_0000 == Self::DATA_1 => MossWord::Data1,
+            two_msb if two_msb & 0b1100_0000 == Self::DATA_2 => MossWord::Data2,
             val => unreachable!("Unreachable: {val}"),
         }
     }
 }
```

### Comparing `moss_decoder-0.1.3/tests/integration_test.rs` & `moss_decoder-0.3.0/tests/integration_test.rs`

 * *Files 4% similar despite different names*

```diff
@@ -174,17 +174,34 @@
         cnt = f.len()
     );
 
     println!("Decoding content...");
     let (p, last_trailer_idx) = decode_multiple_events(&f).unwrap();
     println!("Decoded in: {t:?}\n", t = time.elapsed());
 
-    println!("Got: {packets}", packets = p.len());
+    println!("Got: {packets} packets", packets = p.len());
     println!("Last trailer at index: {last_trailer_idx}");
 
     assert_eq!(
         last_trailer_idx,
         f.len() - 2,
         "All bytes were not processed!"
     );
     assert_eq!(p.len(), 100000, "Expected 100k packets, got {}", p.len());
 }
+
+#[test]
+fn test_decode_from_file() {
+    let time = std::time::Instant::now();
+
+    let packets = moss_decoder::decode_from_file("tests/moss_noise.raw".to_string()).unwrap();
+    println!("Decoded in: {t:?}\n", t = time.elapsed());
+
+    println!("Got: {packets}", packets = packets.len());
+
+    assert_eq!(
+        packets.len(),
+        100000,
+        "Expected 100k packets, got {}",
+        packets.len()
+    );
+}
```

### Comparing `moss_decoder-0.1.3/tests/moss_noise.raw` & `moss_decoder-0.3.0/tests/moss_noise.raw`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.1.3/Cargo.lock` & `moss_decoder-0.3.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "moss_decoder"
-version = "0.1.3"
+version = "0.3.0"
 dependencies = [
  "pretty_assertions",
  "pyo3",
 ]
 
 [[package]]
 name = "once_cell"
```

### Comparing `moss_decoder-0.1.3/PKG-INFO` & `moss_decoder-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moss_decoder
-Version: 0.1.3
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python package implemented in Rust to decode MOSS readout data
 Author: Marc Beck König
 Author-email: marc.beck.konig@cern.ch
 Maintainer-email: Marc Beck König <marc.beck.konig@cern.ch>
@@ -15,14 +15,21 @@
 # MOSS Decoder
 [![CI](https://github.com/CramBL/moss_decoder/actions/workflows/CI.yml/badge.svg)](https://github.com/CramBL/moss_decoder/actions/workflows/CI.yml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/moss-decoder)
 ![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/m/crambl/moss_decoder)
 
 
 Python module implemented in Rust for decoding raw data from the MOSS chip (Stitched Monolithic Pixel Sensor prototype).
+
+- [MOSS Decoder](#moss-decoder)
+  - [Installation](#installation)
+  - [Motivation \& Purpose](#motivation--purpose)
+  - [@CERN Gitlab installation for CentOS and similar distributions from local build](#cern-gitlab-installation-for-centos-and-similar-distributions-from-local-build)
+    - [Troubleshooting](#troubleshooting)
+
 ## Installation
 ```shell
 $ pip install moss-decoder
 ```
 Import in python and use for decoding raw data.
 ```python
 import moss_decoder
@@ -36,7 +43,23 @@
 Decoding the 10 MB MOSS readout data. Performed on CentOS Stream 9 with Python 3.11
 
 | Command                                          |       Mean [s] | Min [s] | Max [s] |      Relative |
 | :----------------------------------------------- | -------------: | ------: | ------: | ------------: |
 | `python moss_test/util/decoder_native_python.py` | 36.319 ± 0.175 |  36.057 |  36.568 | 228.19 ± 2.70 |
 | `python moss_test/util/decoder_rust_package.py`  |  0.159 ± 0.002 |   0.157 |   0.165 |          1.00 |
 
+## @CERN Gitlab installation for CentOS and similar distributions from local build
+
+If you update the package source code and want to build and install without publishing and fetching from PyPI, you can follow these steps.
+
+The `.CERN-gitlab-ci.yml` file contains a `build-centos` manual job which will build the MOSS decoder package from source and saves the package as an artifact.
+
+1. Start the job, download the artifacts.
+2. Unzip the artifacts and you will find a `wheels` package in `/target/wheels/` with the `.whl` extension
+3. Run `python -m pip install <wheels package>.whl`
+4. Confirm the installation with `python -m pip freeze | grep moss`, it should display something containing `moss_decoder @ file:<your-path-to-wheels-package>`
+
+### Troubleshooting
+if you get `ERROR: Could not find a version that satisfies the requirement ...` make sure to add `.whl` when performing step 3 above.
+
+if you don't see the expected message at step 4, try running the installation command in step 3 with any or all of these options `--upgrade --no-cache-dir --force-reinstall`.
+
```

