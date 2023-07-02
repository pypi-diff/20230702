# Comparing `tmp/neuromorphic_drivers-0.1.0.tar.gz` & `tmp/neuromorphic_drivers-0.2.0.tar.gz`

## Comparing `neuromorphic_drivers-0.1.0.tar` & `neuromorphic_drivers-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,39 @@
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.1.0/local_dependencies/neuromorphic-drivers/Cargo.toml
--rw-r--r--   0      501       20     1046 2023-05-07 02:21:43.000000 neuromorphic_drivers-0.1.0/local_dependencies/neuromorphic-drivers/src/devices/prophesee_evk4.rs
--rw-r--r--   0      501       20       24 2023-05-07 00:01:38.000000 neuromorphic_drivers-0.1.0/local_dependencies/neuromorphic-drivers/src/devices.rs
--rw-r--r--   0      501       20        0 2023-05-07 00:34:56.000000 neuromorphic_drivers-0.1.0/local_dependencies/neuromorphic-drivers/src/event.rs
--rw-r--r--   0      501       20       37 2023-05-07 00:48:57.000000 neuromorphic_drivers-0.1.0/local_dependencies/neuromorphic-drivers/src/lib.rs
--rw-r--r--   0      501       20      207 2023-05-07 00:48:36.000000 neuromorphic_drivers-0.1.0/local_dependencies/neuromorphic-drivers/src/properties.rs
--rw-r--r--   0      501       20       52 2023-05-07 00:15:03.000000 neuromorphic_drivers-0.1.0/local_dependencies/neuromorphic-drivers/src/traits.rs
--rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.1.0/Cargo.toml
--rw-r--r--   0      501       20     1102 2023-05-07 03:24:50.000000 neuromorphic_drivers-0.1.0/LICENSE
--rw-r--r--   0      501       20       23 2023-05-07 03:25:08.000000 neuromorphic_drivers-0.1.0/README.md
--rw-r--r--   0      501       20      632 2023-05-07 03:37:51.000000 neuromorphic_drivers-0.1.0/pyproject.toml
--rw-r--r--   0      501       20      134 2023-05-07 02:39:57.000000 neuromorphic_drivers-0.1.0/src/lib.rs
--rw-r--r--   0      501       20    12002 2023-05-07 03:39:33.000000 neuromorphic_drivers-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/Cargo.toml
+-rw-r--r--   0     1001      123    18887 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/de.rs
+-rw-r--r--   0     1001      123     5021 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/error.rs
+-rw-r--r--   0     1001      123    25754 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/format.rs
+-rw-r--r--   0     1001      123    14340 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/lib.rs
+-rw-r--r--   0     1001      123    14435 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/ser.rs
+-rw-r--r--   0     1001      123    11374 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/trace.rs
+-rw-r--r--   0     1001      123    10825 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/local_dependencies/reflect/src/value.rs
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123       58 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/.gitignore
+-rw-r--r--   0     1001      123     1102 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/LICENSE
+-rw-r--r--   0     1001      123      115 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/README.md
+-rw-r--r--   0     1001      123    34780 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/build.rs
+-rw-r--r--   0     1001      123      948 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123     2765 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/__init__.py
+-rw-r--r--   0     1001      123      802 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/device.py
+-rw-r--r--   0     1001      123     5842 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/generated/devices/prophesee_evk3_hd.py
+-rw-r--r--   0     1001      123     6204 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/generated/devices/prophesee_evk4.py
+-rw-r--r--   0     1001      123     8330 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/generated/devices_types.py
+-rw-r--r--   0     1001      123      400 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/generated/enums.py
+-rw-r--r--   0     1001      123      680 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/generated/unions.py
+-rw-r--r--   0     1001      123     4481 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/mask.py
+-rw-r--r--   0     1001      123       91 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/serde/__init__.py
+-rw-r--r--   0     1001      123    15358 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/serde/binary.py
+-rw-r--r--   0     1001      123     2296 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/serde/bincode.py
+-rw-r--r--   0     1001      123     1547 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/serde/type.py
+-rw-r--r--   0     1001      123     1091 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/status.py
+-rw-r--r--   0     1001      123     1858 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/python/neuromorphic_drivers/udev.py
+-rw-r--r--   0     1001      123     4497 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/src/adapters.rs
+-rw-r--r--   0     1001      123     1675 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/src/bytes.rs
+-rw-r--r--   0     1001      123    14237 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123     4091 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/src/structured_array.rs
+-rw-r--r--   0     1001      123     6177 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/tests/display.py
+-rw-r--r--   0     1001      123     1961 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/tests/external_synchronization.py
+-rw-r--r--   0     1001      123      608 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/tests/read_many.py
+-rw-r--r--   0     1001      123      583 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/tests/record_raw.py
+-rw-r--r--   0     1001      123      336 2023-07-02 21:13:12.000000 neuromorphic_drivers-0.2.0/tests/test.py
+-rw-r--r--   0     1001      123    19206 2023-07-02 21:13:23.000000 neuromorphic_drivers-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 neuromorphic_drivers-0.2.0/PKG-INFO
```

### Comparing `neuromorphic_drivers-0.1.0/LICENSE` & `neuromorphic_drivers-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuromorphic_drivers-0.1.0/Cargo.lock` & `neuromorphic_drivers-0.2.0/Cargo.lock`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,33 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "anyhow"
+version = "1.0.71"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+
+[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "bincode"
+version = "1.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
+dependencies = [
+ "serde",
+]
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "cc"
@@ -23,30 +38,80 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "getrandom"
+version = "0.2.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "wasi",
+]
+
+[[package]]
+name = "glob"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+
+[[package]]
+name = "heck"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d621efb26863f0e9924c6ac577e8275e5e6b77455db64ffa6c65c904e9e132c"
+dependencies = [
+ "unicode-segmentation",
+]
+
+[[package]]
+name = "include_dir"
+version = "0.6.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "24b56e147e6187d61e9d0f039f10e070d0c0a887e24fe0bb9ca3f29bfde62cab"
+dependencies = [
+ "glob",
+ "include_dir_impl",
+ "proc-macro-hack",
+]
+
+[[package]]
+name = "include_dir_impl"
+version = "0.6.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0a0c890c85da4bab7bce4204c707396bbd3c6c8a681716a51c8814cfc2b682df"
+dependencies = [
+ "anyhow",
+ "proc-macro-hack",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "libc"
-version = "0.2.143"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "edc207893e85c5d6be840e969b496b53d94cec8be2d501b214f50daa97fa8024"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libusb1-sys"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9d0e2afce4245f2c9a418511e5af8718bcaf2fa408aefb259504d1a9cb25f27"
 dependencies = [
@@ -54,17 +119,17 @@
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "matrixmultiply"
@@ -74,17 +139,17 @@
 dependencies = [
  "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "ndarray"
 version = "0.15.6"
@@ -96,31 +161,51 @@
  "num-integer",
  "num-traits",
  "rawpointer",
 ]
 
 [[package]]
 name = "neuromorphic-drivers"
-version = "0.1.1"
+version = "0.4.0"
 dependencies = [
- "neuromorphic-types 0.1.1 (registry+https://github.com/rust-lang/crates.io-index)",
+ "bincode",
+ "libc",
+ "libusb1-sys",
+ "neuromorphic-types 0.4.0 (registry+https://github.com/rust-lang/crates.io-index)",
+ "paste",
  "rusb",
  "serde",
- "serde_json",
+ "thiserror",
+]
+
+[[package]]
+name = "neuromorphic-drivers"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eb6ec4b708513230e570689d32109906cdb90ff1fa31d68cda24968b25ed0d5e"
+dependencies = [
+ "bincode",
+ "libc",
+ "libusb1-sys",
+ "neuromorphic-types 0.4.0 (registry+https://github.com/rust-lang/crates.io-index)",
+ "paste",
+ "rusb",
+ "serde",
+ "thiserror",
 ]
 
 [[package]]
 name = "neuromorphic-types"
-version = "0.1.1"
+version = "0.4.0"
 
 [[package]]
 name = "neuromorphic-types"
-version = "0.1.1"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3578673effd250cd8202be5fa025c879ce7868d9faea12881f351ea1e477ea5a"
+checksum = "2ae9a302788a6d1758106d19192a20e4e65366545c34892b7e0bacc26009a84e"
 
 [[package]]
 name = "num-complex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
 dependencies = [
@@ -143,313 +228,518 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "numpy"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "437213adf41bbccf4aeae535fbfcdad0f6fed241e1ae182ebe97fa1f3ce19389"
+dependencies = [
+ "libc",
+ "ndarray",
+ "num-complex",
+ "num-integer",
+ "num-traits",
+ "pyo3",
+ "rustc-hash",
+]
+
+[[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
+]
+
+[[package]]
+name = "paste"
+version = "1.0.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
+
+[[package]]
+name = "phf"
+version = "0.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fabbf1ead8a5bcbc20f5f8b939ee3f5b0f6f281b6ad3468b84656b658b455259"
+dependencies = [
+ "phf_macros",
+ "phf_shared",
+ "proc-macro-hack",
+]
+
+[[package]]
+name = "phf_generator"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5d5285893bb5eb82e6aaf5d59ee909a06a16737a8970984dd7746ba9283498d6"
+dependencies = [
+ "phf_shared",
+ "rand",
+]
+
+[[package]]
+name = "phf_macros"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "58fdf3184dd560f160dd73922bea2d5cd6e8f064bf4b13110abd81b03697b4e0"
+dependencies = [
+ "phf_generator",
+ "phf_shared",
+ "proc-macro-hack",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "phf_shared"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6796ad771acdc0123d2a88dc428b5e38ef24456743ddb1744ed628f9815c096"
+dependencies = [
+ "siphasher",
 ]
 
 [[package]]
 name = "pkg-config"
 version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
+name = "ppv-lite86"
+version = "0.2.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
+
+[[package]]
+name = "proc-macro-hack"
+version = "0.5.20+deprecated"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "python"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
- "ndarray",
- "neuromorphic-drivers",
+ "bincode",
+ "cc",
+ "neuromorphic-drivers 0.4.0 (registry+https://github.com/rust-lang/crates.io-index)",
+ "numpy",
+ "paste",
  "pyo3",
+ "reflect",
+ "serde",
+ "serde-generate",
+ "serde_json",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "rand"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
+dependencies = [
+ "libc",
+ "rand_chacha",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_chacha"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
+dependencies = [
+ "ppv-lite86",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_core"
+version = "0.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
+dependencies = [
+ "getrandom",
+]
+
+[[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "reflect"
+version = "0.1.0"
+dependencies = [
+ "once_cell",
+ "serde",
+ "thiserror",
+]
+
+[[package]]
 name = "rusb"
 version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44a8c36914f9b1a3be712c1dfa48c9b397131f9a75707e570a391735f785c5d1"
 dependencies = [
  "libc",
  "libusb1-sys",
 ]
 
 [[package]]
+name = "rustc-hash"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
+
+[[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.162"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71b2f6e1ab5c2b98c05f0f35b236b22e8df7ead6ffbf51d7808da7f8817e7ab6"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
+name = "serde-generate"
+version = "0.25.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8c9331265d81c61212dc75df7b0836544ed8e32dba77a522f113805ff9a948e"
+dependencies = [
+ "heck",
+ "include_dir",
+ "phf",
+ "serde",
+ "serde-reflection",
+ "textwrap",
+]
+
+[[package]]
+name = "serde-reflection"
+version = "0.3.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f05a5f801ac62a51a49d378fdb3884480041b99aced450b28990673e8ff99895"
+dependencies = [
+ "once_cell",
+ "serde",
+ "thiserror",
+]
+
+[[package]]
 name = "serde_derive"
-version = "1.0.162"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2a0814352fd64b58489904a44ea8d90cb1a91dcb6b4f5ebabc32c8318e93cb6"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.99"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "siphasher"
+version = "0.3.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
+
+[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
+name = "smawk"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f67ad224767faa3c7d8b6d91985b78e70a1324408abcb1cfcc2be4c06bc06043"
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "59fb7d6d8281a51045d62b8eb3a7d1ce347b76f312af50cd3dc0af39c87c1737"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
+
+[[package]]
+name = "textwrap"
+version = "0.13.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cd05616119e612a8041ef58f2b578906cc2531a6069047ae092cfb86a325d835"
+dependencies = [
+ "smawk",
+ "unicode-width",
+]
+
+[[package]]
+name = "thiserror"
+version = "1.0.40"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+dependencies = [
+ "thiserror-impl",
+]
+
+[[package]]
+name = "thiserror-impl"
+version = "1.0.40"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.23",
+]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+
+[[package]]
+name = "unicode-segmentation"
+version = "1.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
+
+[[package]]
+name = "unicode-width"
+version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
+name = "wasi"
+version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
+checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `neuromorphic_drivers-0.1.0/PKG-INFO` & `neuromorphic_drivers-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: neuromorphic_drivers
-Version: 0.1.0
-Requires-Dist: numpy>=1.24
+Version: 0.2.0
+Requires-Dist: numpy >=1.24
 License-File: LICENSE
 Summary: Neuromorphic devices drivers
 Author: International Centre for Neuromorphic Systems, Alexandre Marcireau
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: homepage, https://github.com/neuromorphicsystems/neuromorphic-rs/
 Project-URL: repository, https://github.com/neuromorphicsystems/neuromorphic-rs/
 Project-URL: documentation, https://github.com/neuromorphicsystems/neuromorphic-rs/
-Project-URL: homepage, https://github.com/neuromorphicsystems/neuromorphic-rs/
 
 # neuromorphic_drivers
 
+See https://github.com/neuromorphicsystems/neuromorphic-rs for documentation and examples.
+
```

