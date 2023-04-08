# Comparing `tmp/xmodits_py-0.2.2.tar.gz` & `tmp/xmodits_py-0.2.3.tar.gz`

## Comparing `xmodits_py-0.2.2.tar` & `xmodits_py-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 xmodits_py-0.2.2/Cargo.toml
--rw-r--r--   0     1001      123     2794 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      775 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/.gitignore
--rw-r--r--   0     1001      123    42803 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/LICENSE
--rw-r--r--   0     1001      123     3380 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/README.md
--rw-r--r--   0     1001      123        0 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/examples/example_1.md
--rw-r--r--   0     1001      123      214 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/examples/example_1.py
--rw-r--r--   0     1001      123        0 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/examples/example_2.md
--rw-r--r--   0     1001      123      250 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/examples/example_2.py
--rw-r--r--   0     1001      123        0 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/examples/example_3.md
--rw-r--r--   0     1001      123      253 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/examples/example_3.py
--rw-r--r--   0     1001      123        0 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/examples/example_4.md
--rw-r--r--   0     1001      123      253 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/examples/example_4.py
--rw-r--r--   0     1001      123        0 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/examples/example_5.md
--rw-r--r--   0     1001      123      238 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/examples/example_5.py
--rw-r--r--   0     1001      123        0 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/examples/example_6.md
--rw-r--r--   0     1001      123      504 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/examples/example_6.py
--rw-r--r--   0     1001      123      638 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/pyproject.toml
--rw-r--r--   0     1001      123     1772 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/src/api.rs
--rw-r--r--   0     1001      123     2987 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/src/error.rs
--rw-r--r--   0     1001      123     1179 2023-04-03 19:07:26.000000 xmodits_py-0.2.2/src/lib.rs
--rw-r--r--   0     1001      123     9264 2023-04-03 19:08:47.000000 xmodits_py-0.2.2/Cargo.lock
--rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 xmodits_py-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 xmodits_py-0.2.3/Cargo.toml
+-rw-r--r--   0     1001      123     2794 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      775 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/.gitignore
+-rw-r--r--   0     1001      123    42803 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/LICENSE
+-rw-r--r--   0     1001      123     3380 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/README.md
+-rw-r--r--   0     1001      123        0 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_1.md
+-rw-r--r--   0     1001      123      214 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_1.py
+-rw-r--r--   0     1001      123        0 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_2.md
+-rw-r--r--   0     1001      123      250 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_2.py
+-rw-r--r--   0     1001      123        0 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_3.md
+-rw-r--r--   0     1001      123      253 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_3.py
+-rw-r--r--   0     1001      123        0 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_4.md
+-rw-r--r--   0     1001      123      253 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_4.py
+-rw-r--r--   0     1001      123        0 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_5.md
+-rw-r--r--   0     1001      123      238 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_5.py
+-rw-r--r--   0     1001      123        0 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_6.md
+-rw-r--r--   0     1001      123      504 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/examples/example_6.py
+-rw-r--r--   0     1001      123      638 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/pyproject.toml
+-rw-r--r--   0     1001      123     1772 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/src/api.rs
+-rw-r--r--   0     1001      123     2987 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/src/error.rs
+-rw-r--r--   0     1001      123     1179 2023-04-08 19:52:28.000000 xmodits_py-0.2.3/src/lib.rs
+-rw-r--r--   0     1001      123    11664 2023-04-08 19:53:35.000000 xmodits_py-0.2.3/Cargo.lock
+-rw-r--r--   0        0        0     3934 1970-01-01 00:00:00.000000 xmodits_py-0.2.3/PKG-INFO
```

### Comparing `xmodits_py-0.2.2/Cargo.toml` & `xmodits_py-0.2.3/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [package]
 name = "xmodits_py"
 authors = ["B0ney - https://github.com/B0ney"]
 description = "Extract samples from tracker modules. Supports IT, XM, S3M, MOD, UMX, MPTM"
-version = "0.2.2"
+version = "0.2.3"
 edition = "2021"
 license = "LGPLv3"
 readme = "README.md"
 repository = "https://github.com/B0ney/xmodits-py"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "xmodits"
 crate-type = ["cdylib"]
 
 [dependencies]
-xmodits-lib = { git = "https://github.com/B0ney/xmodits-lib", rev = "1b0a5348d2b2d5374f7743f2583e7cc0db4462bb"}
+xmodits-lib = { git = "https://github.com/B0ney/xmodits-lib", rev = "fbaa2bd80e94150e9e8a25e4874fd52c38f785c5"}
 
 [dependencies.pyo3]
 version = "0.18.1"
 features = ["extension-module", "abi3-py37", "anyhow"]
 
 [profile.release]
 strip = true
```

### Comparing `xmodits_py-0.2.2/.github/workflows/CI.yml` & `xmodits_py-0.2.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.2/.gitignore` & `xmodits_py-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.2/LICENSE` & `xmodits_py-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.2/README.md` & `xmodits_py-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.2/pyproject.toml` & `xmodits_py-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.2/src/api.rs` & `xmodits_py-0.2.3/src/api.rs`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.2/src/error.rs` & `xmodits_py-0.2.3/src/error.rs`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.2/src/lib.rs` & `xmodits_py-0.2.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `xmodits_py-0.2.2/Cargo.lock` & `xmodits_py-0.2.3/Cargo.lock`

 * *Files 12% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -66,14 +66,42 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "num-complex"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
+name = "num-integer"
+version = "0.1.45"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+dependencies = [
+ "autocfg",
+ "num-traits",
+]
+
+[[package]]
+name = "num-traits"
+version = "0.2.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "parking_lot"
@@ -95,14 +123,23 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
+name = "primal-check"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9df7f93fd637f083201473dab4fee2db4c429d32e55e3299980ab3957ab916a0"
+dependencies = [
+ "num-integer",
+]
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
@@ -174,35 +211,77 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "realfft"
+version = "3.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "93d6b8e8f0c6d2234aa58048d7290c60bf92cd36fd2888cd8331c66ad4f2e1d2"
+dependencies = [
+ "rustfft",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "rubato"
+version = "0.12.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cd70209c27d5b08f5528bdc779ea3ffb418954e28987f9f9775c6eac41003f9c"
+dependencies = [
+ "num-complex",
+ "num-integer",
+ "num-traits",
+ "realfft",
+]
+
+[[package]]
+name = "rustfft"
+version = "6.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e17d4f6cbdb180c9f4b2a26bbf01c4e647f1e1dea22fe8eb9db54198b32f9434"
+dependencies = [
+ "num-complex",
+ "num-integer",
+ "num-traits",
+ "primal-check",
+ "strength_reduce",
+ "transpose",
+ "version_check",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
+name = "strength_reduce"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fe895eb47f22e2ddd4dabc02bce419d2e643c8e3b585c78158b349195bc24d82"
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -243,26 +322,42 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.13",
 ]
 
 [[package]]
+name = "transpose"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6522d49d03727ffb138ae4cbc1283d3774f0d10aa7f9bf52e6784c45daf9b23"
+dependencies = [
+ "num-integer",
+ "strength_reduce",
+]
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "version_check"
+version = "0.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
+
+[[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets",
 ]
@@ -323,21 +418,22 @@
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "xmodits-lib"
 version = "0.6.0"
-source = "git+https://github.com/B0ney/xmodits-lib?rev=1b0a5348d2b2d5374f7743f2583e7cc0db4462bb#1b0a5348d2b2d5374f7743f2583e7cc0db4462bb"
+source = "git+https://github.com/B0ney/xmodits-lib?rev=fbaa2bd80e94150e9e8a25e4874fd52c38f785c5#fbaa2bd80e94150e9e8a25e4874fd52c38f785c5"
 dependencies = [
  "bytemuck",
  "extended",
+ "rubato",
  "thiserror",
 ]
 
 [[package]]
 name = "xmodits_py"
-version = "0.2.2"
+version = "0.2.3"
 dependencies = [
  "pyo3",
  "xmodits-lib",
 ]
```

### Comparing `xmodits_py-0.2.2/PKG-INFO` & `xmodits_py-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmodits_py
-Version: 0.2.2
+Version: 0.2.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Extract samples from tracker modules. Supports IT, XM, S3M, MOD, UMX, MPTM
 Author: B0ney - https://github.com/B0ney
 License: LGPLv3
```

