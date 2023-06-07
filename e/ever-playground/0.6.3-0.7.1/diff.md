# Comparing `tmp/ever_playground-0.6.3.tar.gz` & `tmp/ever_playground-0.7.1.tar.gz`

## Comparing `ever_playground-0.6.3.tar` & `ever_playground-0.7.1.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0      900 1970-01-01 00:00:00.000000 ever_playground-0.6.3/Cargo.toml
--rw-rw-r--   0     1000     1000       78 2023-05-15 13:10:44.000000 ever_playground-0.6.3/.gitignore
--rw-rw-r--   0     1000     1000      230 2023-06-02 10:45:36.000000 ever_playground-0.6.3/.vscode/settings.json
--rw-rw-r--   0     1000     1000      566 2023-05-17 11:44:03.000000 ever_playground-0.6.3/README.md
--rw-rw-r--   0     1000     1000     1062 2023-05-24 15:04:04.000000 ever_playground-0.6.3/create-param8.py
--rw-rw-r--   0     1000     1000     4916 2023-06-05 17:34:16.000000 ever_playground-0.6.3/ever_playground/__init__.py
--rw-rw-r--   0     1000     1000     7420 2023-06-05 17:25:46.000000 ever_playground-0.6.3/ever_playground/ever_playground.pyi
--rw-rw-r--   0     1000     1000     2245 2023-05-22 13:02:10.000000 ever_playground-0.6.3/examples/basics.py
--rw-rw-r--   0     1000     1000      821 2023-05-22 21:04:47.000000 ever_playground-0.6.3/examples/highload/generate.fif
--rwxrwxr-x   0     1000     1000     3399 2023-05-22 16:05:31.000000 ever_playground-0.6.3/examples/highload/highload-wallet-v2.fif
--rw-rw-r--   0     1000     1000     4688 2023-05-22 21:07:18.000000 ever_playground-0.6.3/examples/highload/highload-wallet-v2.py
--rw-------   0     1000     1000      180 2023-05-22 14:37:50.000000 ever_playground-0.6.3/examples/highload/order-list-fift
--rw-------   0     1000     1000      240 2023-05-22 21:04:58.000000 ever_playground-0.6.3/examples/highload/order-list-py
--rw-------   0     1000     1000       32 2023-05-22 14:37:50.000000 ever_playground-0.6.3/examples/highload/sample.pk
--rw-------   0     1000     1000       36 2023-05-22 14:37:50.000000 ever_playground-0.6.3/examples/highload/sample27172.addr
--rw-rw-r--   0     1000     1000     1487 2023-05-24 13:11:36.000000 ever_playground-0.6.3/examples/ifjmp-perf-eval.py
--rwxrwxr-x   0     1000     1000      870 2023-05-22 16:19:06.000000 ever_playground-0.6.3/examples/recover-stake.fif
--rw-rw-r--   0     1000     1000     1889 2023-05-22 16:19:27.000000 ever_playground-0.6.3/examples/recover-stake.py
--rw-rw-r--   0     1000     1000     2327 2023-05-22 13:04:32.000000 ever_playground-0.6.3/examples/runvm.py
--rwxrwxr-x   0     1000     1000     1187 2023-05-22 11:04:24.000000 ever_playground-0.6.3/examples/testgiver.fif
--rw-rw-r--   0     1000     1000     2864 2023-05-23 09:21:52.000000 ever_playground-0.6.3/examples/testgiver.py
--rwxrwxr-x   0     1000     1000     1645 2023-05-22 12:49:48.000000 ever_playground-0.6.3/examples/validator-elect-req.fif
--rw-rw-r--   0     1000     1000     3607 2023-05-20 15:28:34.000000 ever_playground-0.6.3/examples/validator-elect-req.py
--rw-rw-r--   0     1000     1000      946 2023-05-17 10:02:52.000000 ever_playground-0.6.3/pyproject.toml
--rwxrwxr-x   0     1000     1000     3030 2023-05-24 13:21:40.000000 ever_playground-0.6.3/run-examples.py
--rw-rw-r--   0     1000     1000    18724 2023-06-02 10:13:02.000000 ever_playground-0.6.3/src/lib.rs
--rw-rw-r--   0     1000     1000     1021 2023-06-05 17:30:59.000000 ever_playground-0.6.3/src/tests.rs
--rw-rw-r--   0     1000     1000     3689 2023-05-15 14:26:56.000000 ever_playground-0.6.3/src/utils.rs
--rw-rw-r--   0     1000     1000     3036 2023-06-02 16:56:59.000000 ever_playground-0.6.3/try-catch.py
--rw-rw-r--   0     1000     1000     3572 2023-06-05 17:22:15.000000 ever_playground-0.6.3/ttt.py
--rw-rw-r--   0     1000     1000    24716 2023-06-05 17:36:39.000000 ever_playground-0.6.3/Cargo.lock
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 ever_playground-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 ever_playground-0.7.1/Cargo.toml
+-rw-rw-r--   0     1000     1000       78 2023-05-15 13:10:44.000000 ever_playground-0.7.1/.gitignore
+-rw-rw-r--   0     1000     1000      230 2023-06-07 13:28:48.000000 ever_playground-0.7.1/.vscode/settings.json
+-rw-rw-r--   0     1000     1000      566 2023-05-17 11:44:03.000000 ever_playground-0.7.1/README.md
+-rw-rw-r--   0     1000     1000     1062 2023-05-24 15:04:04.000000 ever_playground-0.7.1/create-param8.py
+-rw-rw-r--   0     1000     1000     6298 2023-06-07 22:03:10.000000 ever_playground-0.7.1/ever_playground/__init__.py
+-rw-rw-r--   0     1000     1000     9717 2023-06-07 22:10:09.000000 ever_playground-0.7.1/ever_playground/ever_playground.pyi
+-rw-rw-r--   0     1000     1000     2226 2023-06-07 22:10:35.000000 ever_playground-0.7.1/examples/basics.py
+-rw-rw-r--   0     1000     1000      821 2023-05-22 21:04:47.000000 ever_playground-0.7.1/examples/highload/generate.fif
+-rwxrwxr-x   0     1000     1000     3399 2023-05-22 16:05:31.000000 ever_playground-0.7.1/examples/highload/highload-wallet-v2.fif
+-rw-rw-r--   0     1000     1000     4667 2023-06-06 14:21:08.000000 ever_playground-0.7.1/examples/highload/highload-wallet-v2.py
+-rw-------   0     1000     1000      180 2023-05-22 14:37:50.000000 ever_playground-0.7.1/examples/highload/order-list-fift
+-rw-------   0     1000     1000      240 2023-05-22 21:04:58.000000 ever_playground-0.7.1/examples/highload/order-list-py
+-rw-------   0     1000     1000       32 2023-05-22 14:37:50.000000 ever_playground-0.7.1/examples/highload/sample.pk
+-rw-------   0     1000     1000       36 2023-05-22 14:37:50.000000 ever_playground-0.7.1/examples/highload/sample27172.addr
+-rw-rw-r--   0     1000     1000     1540 2023-06-07 22:07:40.000000 ever_playground-0.7.1/examples/ifjmp-perf-eval.py
+-rwxrwxr-x   0     1000     1000      870 2023-05-22 16:19:06.000000 ever_playground-0.7.1/examples/recover-stake.fif
+-rw-rw-r--   0     1000     1000     1889 2023-05-22 16:19:27.000000 ever_playground-0.7.1/examples/recover-stake.py
+-rw-rw-r--   0     1000     1000     2371 2023-06-07 22:00:21.000000 ever_playground-0.7.1/examples/runvm.py
+-rwxrwxr-x   0     1000     1000     1187 2023-05-22 11:04:24.000000 ever_playground-0.7.1/examples/testgiver.fif
+-rw-rw-r--   0     1000     1000     2864 2023-05-23 09:21:52.000000 ever_playground-0.7.1/examples/testgiver.py
+-rwxrwxr-x   0     1000     1000     1645 2023-05-22 12:49:48.000000 ever_playground-0.7.1/examples/validator-elect-req.fif
+-rw-rw-r--   0     1000     1000     3607 2023-05-20 15:28:34.000000 ever_playground-0.7.1/examples/validator-elect-req.py
+-rw-rw-r--   0     1000     1000      946 2023-05-17 10:02:52.000000 ever_playground-0.7.1/pyproject.toml
+-rwxrwxr-x   0     1000     1000     3030 2023-05-24 13:21:40.000000 ever_playground-0.7.1/run-examples.py
+-rw-rw-r--   0     1000     1000     6460 2023-06-07 21:45:48.000000 ever_playground-0.7.1/src/continuations.rs
+-rw-rw-r--   0     1000     1000     1791 2023-06-07 20:27:47.000000 ever_playground-0.7.1/src/crypto.rs
+-rw-rw-r--   0     1000     1000    11665 2023-06-07 22:09:29.000000 ever_playground-0.7.1/src/lib.rs
+-rw-rw-r--   0     1000     1000      997 2023-06-07 09:59:08.000000 ever_playground-0.7.1/src/tests.rs
+-rw-rw-r--   0     1000     1000     5901 2023-06-07 20:27:22.000000 ever_playground-0.7.1/src/utils.rs
+-rw-rw-r--   0     1000     1000     4193 2023-06-07 21:56:26.000000 ever_playground-0.7.1/src/vm.rs
+-rw-rw-r--   0     1000     1000     3036 2023-06-02 16:56:59.000000 ever_playground-0.7.1/try-catch.py
+-rw-rw-r--   0     1000     1000     3613 2023-06-06 15:33:22.000000 ever_playground-0.7.1/ttt.py
+-rw-rw-r--   0     1000     1000    24799 2023-06-07 22:15:09.000000 ever_playground-0.7.1/Cargo.lock
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 ever_playground-0.7.1/PKG-INFO
```

### Comparing `ever_playground-0.6.3/Cargo.toml` & `ever_playground-0.7.1/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [package]
 name = "ever-playground"
-version = "0.6.3"
+version = "0.7.1"
 edition = "2021"
 
 [lib]
 name = "ever_playground"
 crate-type = ["cdylib"]
 
 [dependencies]
 ed25519-dalek = "1"
 num-bigint = "0.4"
-pyo3 = { version = "0.18.3", features = ["extension-module", "num-bigint"] }
+pyo3 = { version = "0.19.0", features = ["extension-module", "num-bigint"] }
 rand = "0.7"
 
-ton_block = { git = "https://github.com/tonlabs/ever-block.git", tag = "1.9.72" }
+ton_block = { git = "https://github.com/tonlabs/ever-block.git", tag = "1.9.74" }
 ton_types = { git = "https://github.com/tonlabs/ever-types.git", tag = "2.0.13" }
 ton_labs_assembler = { git = "https://github.com/tonlabs/ever-assembler", tag = "1.2.120" }
-ton_vm = { git = "https://github.com/tonlabs/ever-vm.git", tag = "1.8.164" }
+#ton_vm = { git = "https://github.com/tonlabs/ever-vm.git", tag = "1.8.172" }
+ton_vm = { git = "ssh://git@github.com/tonlabs/ever-vm-private.git", branch = "cc-ctrls-access" }
+
+[patch."ssh://git@github.com/tonlabs/ever-block-private.git"]
+ton_block = { git = "https://github.com/tonlabs/ever-block.git", tag = "1.9.72" }
 
-#[patch."ssh://git@github.com/tonlabs/ever-block-private.git"]
-#ton_block = { git = "https://github.com/tonlabs/ever-block.git", tag = "1.9.72" }
-#
-#[patch."ssh://git@github.com/tonlabs/ever-types-private.git"]
-#ton_types = { git = "https://github.com/tonlabs/ever-types.git", tag = "2.0.13" }
+[patch."ssh://git@github.com/tonlabs/ever-types-private.git"]
+ton_types = { git = "https://github.com/tonlabs/ever-types.git", tag = "2.0.13" }
```

### Comparing `ever_playground-0.6.3/README.md` & `ever_playground-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.3/create-param8.py` & `ever_playground-0.7.1/create-param8.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.3/ever_playground/__init__.py` & `ever_playground-0.7.1/ever_playground/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,71 @@
 from enum import Enum
 from typing import Optional, Tuple
 from fractions import Fraction
 
-from .ever_playground import Cell, Builder, Slice, Dictionary, assemble, runvm
+from .ever_playground import Cell, Builder, Slice, Dictionary, Gas, Continuation, ContinuationType, SaveList, VmState, VmResult, assemble, runvm_generic
 from .ever_playground import ed25519_new_keypair, ed25519_secret_to_public, ed25519_sign, ed25519_check_signature
 
 __all__ = [
     "Cell",
     "Builder",
     "Slice",
     "Dictionary",
     "ExceptionCode",
     "StateInit",
     "assemble",
+    "VmState",
+    "VmResult",
+    "runvm_generic",
     "runvm",
     "parse_smc_addr",
     "load_address",
     "parse_load_address",
     "parse_adnl_address",
     "ed25519_new_keypair",
     "ed25519_secret_to_public",
     "ed25519_sign",
     "ed25519_check_signature",
 ]
 
+def runvm(code, stack, **kwargs) -> VmResult:
+    cc = Continuation(
+        ContinuationType.create_ordinary(),
+        code,
+        stack,
+        SaveList(),
+        -1
+    )
+
+    regs = SaveList()
+    capabilities = 0
+    trace = False
+    gas_limit = 1000000000
+    gas_credit = 10000
+    for key, value in kwargs.items():
+        if key == "capabilities":
+            capabilities = int(value)
+        elif key == "trace":
+            trace = bool(value)
+        elif key == "c4":
+            regs.put(4, value)
+        elif key == "c7":
+            regs.put(7, value)
+        elif key == "gas_limit":
+            gas_limit = int(value)
+        elif key == "gas_credit":
+            gas_credit = int(value)
+        else:
+            raise Exception("Unknown parameter {}".format(key))
+
+    state = VmState(cc, regs, Gas(gas_limit, gas_credit))
+    return runvm_generic(state, capabilities, trace)
+
 class ExceptionCode(Enum):
+    """TVM exception code."""
     NormalTermination = 0
     AlternativeTermination = 1
     StackUnderflow = 2
     StackOverflow = 3
     IntegerOverflow = 4
     RangeCheckError = 5
     InvalidOpcode = 6
@@ -100,14 +137,15 @@
         self.tick = tick
         self.tock = tock
         self.code = code
         self.data = data
         self.library = library
 
     def deserialize(self, s: Slice):
+        """Deserializes StateInit from the ``s`` slice."""
         if s.u(1):
             self.split_depth = s.u(5)
         if s.u(1):
             self.tick = bool(s.u(1))
             self.tock = bool(s.u(1))
         else:
             self.tick = self.tock = False
@@ -116,14 +154,15 @@
         if s.u(1):
             self.data = s.r()
         if s.u(1):
             self.library = Dictionary.deserialize(256, s)
         return self
 
     def serialize(self) -> Builder:
+        """Serializes StateInit into Builder."""
         b = Builder()
         if self.split_depth is None:
             b.i(1, 0)
         else:
             b.i(1, 1).i(5, self.split_depth)
         if self.tick or self.tock:
             b.i(1, 1).i(1, self.tick).i(1, self.tock)
@@ -148,27 +187,30 @@
     value: int
 
     def __init__(self, value: int = 0):
         if value < 0 or value.bit_length() > 128:
             raise Exception("Currency value must be non-negative and fit into 128 bits")
         self.value = value
 
-    @staticmethod
-    def from_str(value: str):
+    @classmethod
+    def from_str(cls, value: str):
+        """Constructs a Currency object from a rational number represented by the ``value`` string."""
         return Currency(int(Fraction(value) * Currency.FACTOR))
 
     def deserialize(self, s: Slice):
+        """Deserializes Currency from the ``s`` slice."""
         len = s.u(4)
         if len == 0:
             self.value = 0
         else:
             self.value = s.u(len * 8)
         return self
 
     def serialize(self) -> Builder:
+        """Serializes Currency into Builder."""
         if self.value == 0:
             return Builder().i(4, 0)
         len = (self.value.bit_length() + 7) >> 3
         assert(len < 16)
         return Builder().i(4, len).i(len * 8, self.value)
 
     def __str__(self) -> str:
```

### Comparing `ever_playground-0.6.3/examples/basics.py` & `ever_playground-0.7.1/examples/basics.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 expect(False, s.is_empty())
 expect(val2, s.u(64))
 expect(True, s.is_empty())
 
 val3 = 0xffffffff
 s = S(B().i(32, val3).finalize())
 expect(-1, s.i(23))
-expect(9, len(s))
+expect(9, s.remaining_bits())
 
 d1_wc, d1_addr = parse_smc_addr("0:000169b042c37962027e58de0dbaa0b85f5d032f37d8333e3cdfdcc7918ae00a")
 d2_wc, d2_addr = parse_smc_addr("0:bc43df2056abee4c1a443fbfcfede0ba90d214c77322167fc08ce48920c17c1b")
 d3_wc, d3_addr = parse_smc_addr("0:d4a50c1a849a4742214e751977af268269e6eeae064ce800634acea241d430d3")
 
 s1 = B().i(32, d1_wc).i(256, d1_addr).slice()
 s2 = B().i(32, d2_wc).i(256, d2_addr).slice()
@@ -62,15 +62,14 @@
         C("bfc000b4d82161bcb1013f2c6f06dd505c2fae81979bec199f1e6fee63c8c570054_"),
         C("2_",
             C("bfbc43df2056abee4c1a443fbfcfede0ba90d214c77322167fc08ce48920c17c1b"),
             C("bf94a50c1a849a4742214e751977af268269e6eeae064ce800634acea241d430d3"))))
 expect(c, dict_cell1)
 
 dict_bytes = dict_cell1.write(0)
-dict_bytes = bytes(dict_cell1)
 dict_cell2 = C.read(dict_bytes)
 #print(dict_cell2)
 
 expect(dict_cell1, dict_cell2)
 
 #open("test.boc", "wb").write(dict_cell.write())
 #cell = C.read(open("test.boc", "rb").read())
```

### Comparing `ever_playground-0.6.3/examples/highload/generate.fif` & `ever_playground-0.7.1/examples/highload/generate.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.3/examples/highload/highload-wallet-v2.fif` & `ever_playground-0.7.1/examples/highload/highload-wallet-v2.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.3/examples/highload/highload-wallet-v2.py` & `ever_playground-0.7.1/examples/highload/highload-wallet-v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     print(f"Transferring {ng} to account {wc}:{addr:064x} bounce={bounce}")
     return create_int_msg(Builder().i(32, 0).finalize(), bounce, wc, addr, ng)
 
 def create_order(c: Cell, send_mode: int) -> Cell:
     return Builder().i(8, send_mode).r(c).finalize()
 
 def send(address: str, ng: Currency, bounce: bool):
-    global send_mode
     t = create_simple_transfer(address, ng, bounce)
     order = create_order(t, send_mode)
     add_order(Slice(order))
 
 with open(order_file, "r") as file:
     for line in file:
         chunks = line.split(" ")
```

### Comparing `ever_playground-0.6.3/examples/ifjmp-perf-eval.py` & `ever_playground-0.7.1/examples/ifjmp-perf-eval.py`

 * *Files 17% similar despite different names*

```diff
@@ -49,13 +49,16 @@
         code2 = assemble(text2)
 
         res1 = runvm(Slice(code1), [target_func_id])
         assert(res1.exit_code == 0)
         res2 = runvm(Slice(code2), [target_func_id])
         assert(res2.exit_code == 0)
 
-        ratio = float(res2.gas_used) / res1.gas_used
-        print(f"{i+1:<4} {len(code1):<2} {res1.gas_used:8}    {len(code2):<2} {res2.gas_used:<14} {ratio:.2f}")
+        gas1 = res1.state.gas.used
+        gas2 = res2.state.gas.used
+
+        ratio = float(gas2) / gas1
+        print(f"{i+1:<4} {code1.cells_count():<2} {gas1:8}    {code2.cells_count():<2} {gas2:<14} {ratio:.2f}")
 
 for i in [0, 16, 64]:
     print(f"ifjmp body has {i} nops before call")
     bench_by_cmps_count("NOP " * i)
```

### Comparing `ever_playground-0.6.3/examples/recover-stake.fif` & `ever_playground-0.7.1/examples/recover-stake.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.3/examples/recover-stake.py` & `ever_playground-0.7.1/examples/recover-stake.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.3/examples/runvm.py` & `ever_playground-0.7.1/examples/runvm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import time
 
 from ever_playground import Cell as C
 from ever_playground import Slice as S
 from ever_playground import ExceptionCode
-from ever_playground import StateInit, runvm, assemble
+from ever_playground import StateInit, VmState, runvm, assemble
 
 def expect(expected, v):
     if not expected == v:
         raise Exception("{} != {}".format(expected, v))
 
 add = assemble("""
     ADD
 """)
 res = runvm(S(add), [10, 20], capabilities = 0x1)
-expect([30], res.stack)
+expect([30], res.state.cc.stack)
 
 throw = assemble("THROW 100")
 res = runvm(S(throw), [10])
 expect(100, res.exit_code)
 expect(0, res.exception_value)
-expect([10], res.stack)
+expect([10], res.state.cc.stack)
 
 sib = StateInit(code = throw).serialize()
 #print(sib)
 sic = \
 C("24_",
     C("f2c064"))
 expect(sic, sib.finalize())
@@ -32,20 +32,20 @@
 si = StateInit().deserialize(S(sib.finalize()))
 expect(throw, si.code)
 
 throwargany = assemble("NEWC ENDC PUSHINT 100 THROWARGANY")
 res = runvm(S(throwargany), [], trace = True)
 expect(100, res.exit_code)
 expect(C(""), res.exception_value)
-expect([], res.stack)
+expect([], res.state.cc.stack)
 
 ctrls_ex = assemble("PUSHCTR c4")
 abc = C("abc")
 res = runvm(S(ctrls_ex), [], c4 = abc)
-expect([abc], res.stack)
+expect([abc], res.state.cc.stack)
 
 loop = """
     PUSHINT 0x8de120e0abffc55bf3fc723dee9e6d6bc01716064312a4e4be58be4e193fda8d
     PUSHSLICE xedf0554ee6f844bb7b08c91771d44c30dd69cc5b192ca2d8beff2e38b34f3d8f3c6e76b8c37c2a2fa3ea0bf082a128e2ae4c5befd941160ffcf4aed9e0d8f905
     PUSHINT 0xf5ec1345ad9adf191db35cdece12482e19a3a218e12f2d6c3e26e0ec6463d0a5
 
     PUSHINT {}
@@ -57,26 +57,26 @@
     REPEAT
 """
 
 chksignu_loop = assemble(loop.format(10000, "CHKSIGNU"))
 blkdrop2_loop = assemble(loop.format(1000000, "BLKDROP 2"))
 
 res = runvm(S(chksignu_loop), [], gas_limit = 100000)
-expect(ExceptionCode.OutOfGas.value, res.exit_code) # out of gas
+expect(ExceptionCode.OutOfGas.value, res.exit_code)
 
 def benchmark(name, code_cell, iters, steps = None, gas_used = None):
     print("running {}".format(name))
     t = time.time()
     res = runvm(S(code_cell), [])
     elapsed = time.time() - t
 
     expect(0, res.exit_code)
     if steps:
-        expect(steps, res.steps)
+        expect(steps, res.state.steps)
     if gas_used:
-        expect(gas_used, res.gas_used)
+        expect(gas_used, res.state.gas.used)
 
     print("total time {:.2f}s".format(elapsed))
     print("one iteration takes {:.2f}us".format(elapsed * 1000000 / iters))
 
 benchmark("chksignu loop", chksignu_loop, 10000, 40008, 750259)
 benchmark("blkdrop2 loop", blkdrop2_loop, 1000000, 4000008, 75000248)
```

### Comparing `ever_playground-0.6.3/examples/testgiver.fif` & `ever_playground-0.7.1/examples/testgiver.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.3/examples/testgiver.py` & `ever_playground-0.7.1/examples/testgiver.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.3/examples/validator-elect-req.fif` & `ever_playground-0.7.1/examples/validator-elect-req.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.3/examples/validator-elect-req.py` & `ever_playground-0.7.1/examples/validator-elect-req.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.3/pyproject.toml` & `ever_playground-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.3/run-examples.py` & `ever_playground-0.7.1/run-examples.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.3/src/tests.rs` & `ever_playground-0.7.1/src/tests.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #![cfg(test)]
 
-use crate::{InternalCell, dump_cell};
-use ton_types::SliceData;
+use crate::dump_cell;
+use ton_types::{Cell, SliceData};
 
-fn __(data: &str, refs: Vec<InternalCell>) -> ton_types::Result<InternalCell> {
+fn __(data: &str, refs: Vec<Cell>) -> ton_types::Result<Cell> {
     let mut b = SliceData::from_string(data)?.as_builder();
     for r in refs {
         b.checked_append_reference(r)?;
     }
     b.into_cell()
 }
```

### Comparing `ever_playground-0.6.3/try-catch.py` & `ever_playground-0.7.1/try-catch.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.3/ttt.py` & `ever_playground-0.7.1/ttt.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,20 @@
     cell = Cell.read(b)
     print(f"cells in total {cell.cells_count()}, unique {cell.unique_cells_count()}")
     #print(cell)
 
 info("/tonlabs/sol2tvm/tests2/5253a82a87b58db960a112b6a4be53f160c00fe5940b259979677cbba0ce5f73.tvc")
 info("/tonlabs/sol2tvm/tests2/test_mycode.tvc")
 
+from ever_playground import ed25519_new_keypair, Currency
+
+secret, public = ed25519_new_keypair()
+
+c = Currency.from_str("1/3")
+
 exit(0)
 
 text = """
     IFJMPREF {
         DUP
         PUSHINT 429793271
         EQUAL
@@ -148,10 +154,7 @@
         }
         IFJMP
     }
 """
 code = assemble(text)
 print(code)
 
-from ever_playground import ed25519_new_keypair
-
-secret, public = ed25519_new_keypair()
```

### Comparing `ever_playground-0.6.3/Cargo.lock` & `ever_playground-0.7.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -223,21 +223,21 @@
  "serde",
  "sha2 0.9.9",
  "zeroize",
 ]
 
 [[package]]
 name = "ever-playground"
-version = "0.6.3"
+version = "0.7.1"
 dependencies = [
  "ed25519-dalek",
  "num-bigint",
  "pyo3",
  "rand",
- "ton_block",
+ "ton_block 1.9.74",
  "ton_labs_assembler",
  "ton_types",
  "ton_vm",
 ]
 
 [[package]]
 name = "failure"
@@ -310,23 +310,23 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
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
 name = "lockfree"
@@ -334,32 +334,29 @@
 source = "git+https://github.com/tonlabs/lockfree.git#bfcb66587dc4ffed9e8e9248995ad2fe8dc3669e"
 dependencies = [
  "owned-alloc",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
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
 name = "miniz_oxide"
 version = "0.6.2"
@@ -454,26 +451,26 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "object"
-version = "0.30.3"
+version = "0.30.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea86265d3d3dcb6a27fc51bd29a4bf387fae9d2986b823079d4986af253eb439"
+checksum = "03b4680b86d9cfafba8fc491dc9b6df26b68cf40e9e6cd73909194759a63c385"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "opaque-debug"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
 
@@ -491,23 +488,23 @@
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
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
@@ -519,17 +516,17 @@
 checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
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
  "num-bigint",
  "parking_lot",
@@ -537,49 +534,49 @@
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
@@ -630,17 +627,17 @@
 checksum = "ca3129af7b92a17112d59ad498c6f81eaf463253766b90396d39ea7a39d6613c"
 dependencies = [
  "rand_core",
 ]
 
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
 name = "rustc-demangle"
 version = "0.1.23"
@@ -672,15 +669,15 @@
 name = "serde_derive"
 version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.17",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
@@ -741,17 +738,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.17"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45b6ddbb36c5b969c182aec3c4a0bce7df3fbad4b77114706a49aacc80567388"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -771,15 +768,33 @@
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "ton_block"
 version = "1.9.72"
-source = "git+https://github.com/tonlabs/ever-block.git?tag=1.9.72#9350ea08938d8ff5d4490defe78446d6de08ed7e"
+source = "git+https://github.com/tonlabs/ever-block.git?tag=1.9.72#c51dfb0ebd2655ad7003ca0cb732742ea23119a8"
+dependencies = [
+ "base64",
+ "crc",
+ "ed25519",
+ "ed25519-dalek",
+ "failure",
+ "hex",
+ "log",
+ "num",
+ "num-traits",
+ "sha2 0.10.6",
+ "ton_types",
+]
+
+[[package]]
+name = "ton_block"
+version = "1.9.74"
+source = "git+https://github.com/tonlabs/ever-block.git?tag=1.9.74#9db5a51519aa3d0edb00c598af6f93cc3db551d8"
 dependencies = [
  "base64",
  "crc",
  "ed25519",
  "ed25519-dalek",
  "failure",
  "hex",
@@ -804,15 +819,15 @@
  "serde_json",
  "ton_types",
 ]
 
 [[package]]
 name = "ton_types"
 version = "2.0.13"
-source = "git+https://github.com/tonlabs/ever-types.git?tag=2.0.13#c1dfeb2596b8226c0ef6e56ff4ff9b7d0d98aeae"
+source = "git+https://github.com/tonlabs/ever-types.git?tag=2.0.13#47689ce3f09cb95c7c3ebfec0005c41e7cee3330"
 dependencies = [
  "aes-ctr",
  "base64",
  "crc",
  "curve25519-dalek",
  "ed25519",
  "ed25519-dalek",
@@ -830,27 +845,27 @@
  "sha2 0.10.6",
  "smallvec",
  "x25519-dalek",
 ]
 
 [[package]]
 name = "ton_vm"
-version = "1.8.164"
-source = "git+https://github.com/tonlabs/ever-vm.git?tag=1.8.164#3e32cbfa36fd4e5ce0a059b24b023aa62caee84b"
+version = "1.8.172"
+source = "git+ssh://git@github.com/tonlabs/ever-vm-private.git?branch=cc-ctrls-access#23a4ca851f51d2235b479c3aa25b1eaca7fff0fd"
 dependencies = [
  "ed25519",
  "ed25519-dalek",
  "failure",
  "hex",
  "lazy_static",
  "log",
  "num",
  "num-traits",
  "rand",
- "ton_block",
+ "ton_block 1.9.72",
  "ton_types",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -883,78 +898,69 @@
 [[package]]
 name = "wasi"
 version = "0.9.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cccddf32554fecc6acb585f82a32a72e28b48f8c4c1883ddfeeeaa96f7d8e519"
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
-
-[[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
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
 
 [[package]]
 name = "x25519-dalek"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2392b6b94a576b4e2bf3c5b2757d63f10ada8020a2e4d08ac849ebcf6ea8e077"
 dependencies = [
@@ -976,9 +982,9 @@
 name = "zeroize_derive"
 version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.17",
+ "syn 2.0.18",
 ]
```

### Comparing `ever_playground-0.6.3/PKG-INFO` & `ever_playground-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ever-playground
-Version: 0.6.3
+Version: 0.7.1
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # ever-playground
 
 A tool alternative to Fift: play with Cells, Slices, Builders, and Dictionaries — native types of TVM; assemble and run TVM code.
```

