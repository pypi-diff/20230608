# Comparing `tmp/pycbpf-0.0.1.tar.gz` & `tmp/pycbpf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycbpf-0.0.1.tar", last modified: Sun May 21 13:44:27 2023, max compression
+gzip compressed data, was "pycbpf-0.0.2.tar", last modified: Thu Jun  8 11:08:13 2023, max compression
```

## Comparing `pycbpf-0.0.1.tar` & `pycbpf-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-21 13:44:27.180096 pycbpf-0.0.1/
--rw-r--r--   0 admin      (501) staff       (20)     1073 2023-05-21 13:37:05.000000 pycbpf-0.0.1/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)     2255 2023-05-21 13:44:27.179701 pycbpf-0.0.1/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     1767 2023-05-21 09:56:02.000000 pycbpf-0.0.1/README.md
--rw-r--r--   0 admin      (501) staff       (20)      632 2023-05-21 13:44:16.000000 pycbpf-0.0.1/pyproject.toml
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-05-21 13:44:27.180271 pycbpf-0.0.1/setup.cfg
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-21 13:44:27.169696 pycbpf-0.0.1/src/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-21 13:44:27.174528 pycbpf-0.0.1/src/pycbpf/
--rw-r--r--   0 admin      (501) staff       (20)       63 2023-05-21 13:38:24.000000 pycbpf-0.0.1/src/pycbpf/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     3020 2023-05-21 13:38:24.000000 pycbpf-0.0.1/src/pycbpf/c2ebpf.py
--rw-r--r--   0 admin      (501) staff       (20)    10705 2023-05-21 13:38:24.000000 pycbpf-0.0.1/src/pycbpf/cbpf2c.py
--rw-r--r--   0 admin      (501) staff       (20)     1015 2023-05-21 13:38:24.000000 pycbpf-0.0.1/src/pycbpf/filter2cbpf.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-21 13:44:27.177048 pycbpf-0.0.1/src/pycbpf.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     2255 2023-05-21 13:44:27.000000 pycbpf-0.0.1/src/pycbpf.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      306 2023-05-21 13:44:27.000000 pycbpf-0.0.1/src/pycbpf.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-05-21 13:44:27.000000 pycbpf-0.0.1/src/pycbpf.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)        7 2023-05-21 13:44:27.000000 pycbpf-0.0.1/src/pycbpf.egg-info/top_level.txt
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-05-21 13:44:27.178695 pycbpf-0.0.1/tests/
--rw-r--r--   0 admin      (501) staff       (20)     7456 2023-05-21 13:38:24.000000 pycbpf-0.0.1/tests/test_cbpf2c.py
--rw-r--r--   0 admin      (501) staff       (20)     1542 2023-05-21 13:38:24.000000 pycbpf-0.0.1/tests/test_filter2cbpf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:08:13.204147 pycbpf-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 11:07:42.000000 pycbpf-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-08 11:08:13.204147 pycbpf-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-08 11:07:42.000000 pycbpf-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:08:13.204147 pycbpf-0.0.2/pycbpf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:07:42.000000 pycbpf-0.0.2/pycbpf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-08 11:07:42.000000 pycbpf-0.0.2/pycbpf/c2ebpf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-06-08 11:07:42.000000 pycbpf-0.0.2/pycbpf/cbpf2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-08 11:07:42.000000 pycbpf-0.0.2/pycbpf/filter2cbpf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:08:13.204147 pycbpf-0.0.2/pycbpf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-08 11:08:13.000000 pycbpf-0.0.2/pycbpf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 11:08:13.000000 pycbpf-0.0.2/pycbpf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:08:13.000000 pycbpf-0.0.2/pycbpf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 11:08:13.000000 pycbpf-0.0.2/pycbpf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 11:08:13.000000 pycbpf-0.0.2/pycbpf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-08 11:07:42.000000 pycbpf-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:08:13.204147 pycbpf-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:08:13.204147 pycbpf-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-08 11:07:42.000000 pycbpf-0.0.2/tests/test_cbpf2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-08 11:07:42.000000 pycbpf-0.0.2/tests/test_filter2cbpf.py
```

### Comparing `pycbpf-0.0.1/LICENSE` & `pycbpf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycbpf-0.0.1/README.md` & `pycbpf-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,125 @@
 ### About pycbpf
 ---
 
 Inspired by [cbpfc](https://github.com/cloudflare/cbpfc).
 
-pycbpf2c converts tcpdump filter args to C code which can be injected to a BCC script.
+pycbpf2c converts tcpdump filter expression to C code which can be injected to a BCC script.
 
-This aims to provide native python support, so bcc can import it directly.
+This aims to provide native python support, so BCC can import it directly.
 
 And it provides a BCC script for dump filtered packet to pcap format.
 
+### Simple usecase
 
 You can save packets to a pcap file like below to sniffer packet from ```dev_queue_xmit```
 ```
 python3 -m pycbpf.c2ebpf -i eth0 -w file.pcap <tcpdump expresion>
 ```
 
-Or you can pipe output to stdout and use tcpdump analyze
+Or with no pcap file specified, you need to pipe output to tcpdump
 ```
-python3 -m pycbpf.c2ebpf -i eth0 <tcpdump expresion> | tcpdump -r -
+python3 -m pycbpf.c2ebpf -i eth0 <tcpdump expresion> | tcpdump -r - -nev
 ```
 
+### Examples of usage
 
-Of course you can generate a C program from tcpdump expresion and implement your own bcc script.
-Command line below will generate the C program, which can be used directly in BCC.
+Of course you can generate a C program from tcpdump expresion and implement your own BCC script.
+Cmdline below will generate the C program, which can be used directly in BCC.
 ```
 python3 -m pycbpf.cbpf2c <tcpdump expression>
 ```
-import package
+
+Steps to use it in python:
+
+1 - Install and import packages
+
+```
+pip3 install pycbpf
+```
+
 ```
 from bcc import BPF
 from pycbpf import cbpf2c, filter2cbpf
 ```
-generate cbpf and compile to C program, and enable BPF for trace
+2 - Generate cbpf and compile to C program, and enable BPF for trace. Write you test_text with space reserved for the generated code. Use the inline function ```cbpf_filter_func``` in you trace program and handle return value properly.
 ```
-prog = filter2cbpf.cbpf_prog(["ip"])
-prog_c = cbpf2c.cbpf_c(prog)
+test_text = """
+
+/* reserve space for the generated code cbpf_filter_func */
+%s
+
+your_func()
+{
+      u32 datalen = 0;
+      u32 ret = 0;
+      u8 *data;
+      ...
+
+      ret = cbpf_filter_func(data, data + datalen);
+      if (!ret) {
+            return 0;
+      }
+
+      filter_event.perf_submit(ctx, &e, sizeof(e));
+}
+
+"""
+
+prog = filter2cbpf.CbpfProg(["ip"])
+prog_c = cbpf2c.CbpfC(prog)
 cfun = prog_c.compile_cbpf_to_c()
 test_text = bpf_text%cfun
-bpf_ctx = BPF(text=test_text, debug=4)
+bpf_ctx = BPF(text=test_text, debug=0)
+```
+3 - write bcc perf event callback
+```
+def filter_events_cb(_cpu, data, _size):
+      # print some data
+      # or write to pcap files
+
+bctx['filter_event'].open_perf_buffer(filter_events_cb)
 ```
+---
+### Further explain
 
-For example, filter ```ip``` packets, will generate C program
+
+As for the code generated from cbpf, for example, filter ```ip``` packets, will generate C program:
 ```
 static inline u32
 cbpf_filter_func (const u8 *const data, const u8 *const data_end) {
       __attribute__((unused)) u32 A, X, M[16];
       __attribute__((unused)) const u8 *indirect;
 
       if (data + 12 > data_end) { return 0; }
       A = bpf_ntohs(*((u16 *)(data + 12)));
       if (A != 0x800) {goto label3;}
       return 262144;
 label3:
       return 0;
 }
 ```
-Use the inline function ```cbpf_filter_func``` in you trace program and handle return value properly.
 
-see ```c2ebpf.py``` as an example to save packets to pcap files
+It follows what cbpf code tells us to do:
+```
+(000) ldh      [12]
+(001) jeq      #0x800           jt 2	jf 3
+(002) ret      #262144
+(003) ret      #0
+```
+A little explain about the cbpf code and cbpf_filter_func above:
+
+First read 2 byte at offset 12.
+
+Test the data read, if equal to 0x0800, jump to 002, else jump to 003. We name the position to labelX, X is the PC value.
+
+If label is right after last instruction, it will be ignored.
+002 and 003 will return value and exit the function.
+
+
+see ```c2ebpf.py``` as an example to save packets to pcap files
+
+
+
+---
+### LICENSE
+pycbpf is MIT licensed, as found in the LICENSE file
```

### Comparing `pycbpf-0.0.1/pyproject.toml` & `pycbpf-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pycbpf"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="junka", email="wan.junjie@foxmail.com" },
 ]
 description = "convert cbpf code to C for BCC"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
 ]
+dependencies = [
+    "libpcap",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/junka/pycbpf"
 "Bug Tracker" = "https://github.com/junka/pycbpf/issues"
 
 [tool.pytest.ini_options]
-addopts = [
-    "--import-mode=importlib",
-]
+testpaths = [
+    "tests"
+]
+addopts = "--verbose"
+
+[tool.pylint."MESSAGES CONTROL"]
+disable = '''missing-function-docstring,
+        missing-module-docstring,
+'''
```

### Comparing `pycbpf-0.0.1/src/pycbpf/c2ebpf.py` & `pycbpf-0.0.2/pycbpf/c2ebpf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-
+"""
+The function captures packets from a network interface, applies a C Berkeley Packet Filter (cbpf) to
+filter packets, and saves the filtered packets to a pcap file.
+"""
 import time
 import ctypes
 import sys
 import argparse
 import libpcap as pcap
 from bcc import BPF
 
 
-from .cbpf2c import cbpf_c
-from .filter2cbpf import cbpf_prog
+from .cbpf2c import CbpfC
+from .filter2cbpf import CbpfProg
 
-bpftext = """
+BPFTEXT = """
 
 #include <linux/skbuff.h>
 
 #define MAX_PACKET_LEN (128)
 
 
 struct filter_packet {
@@ -51,71 +54,103 @@
 	filter_event.perf_submit(ctx, &e, sizeof(e));
 	return 0;
 }
 
 
 """
 
-class FilterPacket(ctypes.Structure):
+
+class FilterPacket(ctypes.Structure):  # pylint: disable=too-few-public-methods
+    """
+    The class `FilterPacket` defines a structure with a single field `packet` that is
+    an array of 128 unsigned bytes.
+    """
     _fields_ = [
         ("packet", ctypes.c_ubyte * 128)
     ]
 
 
-"""
-ref https://github.com/iovisor/bcc/blob/master/examples/networking/dns_matching/dns_matching.py
-ret https://github.com/iovisor/bcc/blob/master/examples/tracing/undump.py
-filter packet from a raw socket
-"""
 def main():
+    """
+    ref https://github.com/iovisor/bcc/blob/master/examples/networking/dns_matching/dns_matching.py
+    ret https://github.com/iovisor/bcc/blob/master/examples/tracing/undump.py
+    filter packet from a raw socket
+    """
     parser = argparse.ArgumentParser()
-    parser.add_argument("-i", "--interface", help="interface name to run tcpdump", required=True)
-    parser.add_argument("-w", "--file", help="pcap file to save packets")
+    parser.add_argument("-i", "--interface", dest="interface", required=True,
+                        help="interface name to run tcpdump")
+    parser.add_argument("-w", "--file", dest="file",
+                        default="-", help="pcap file to save packets")
+    parser.add_argument("-c", "--count", dest="count", type=int, default=sys.maxsize,
+                        help="number of packets to capture", )
     parser.add_argument('filter', nargs=argparse.REMAINDER)
     args = parser.parse_args()
 
     if args.filter is None or len(args.filter) == 0:
         cfun = """static inline u32
 cbpf_filter_func (const u8 *const data __attribute__((unused)), const u8 *const data_end __attribute__((unused))) {
 	return 1;
 }
 """
     else:
-        prog = cbpf_prog(args.filter)
-        prog_c = cbpf_c(prog)
+        prog = CbpfProg(args.filter)
+        prog_c = CbpfC(prog)
         cfun = prog_c.compile_cbpf_to_c()
 
-    if args.file is None:
-        args.file = '-'
-    text = bpftext%cfun
-    bctx = BPF(text = text, debug = 0)
+    text = BPFTEXT % cfun
+    bctx = BPF(text=text, debug=0)
 
     # func_name = "__netif_receive_skb"
     func_name = "dev_queue_xmit"
     bctx.attach_kprobe(event=func_name, fn_name="filter_packets")
-    pd = pcap.open_dead(pcap.DLT_EN10MB, 1000)
-    dumper = pcap.dump_open(pd, ctypes.c_char_p(args.file.encode("utf-8")))
-    if args.file != '-':
-        print("Capturing packets from %s... Hit Ctrl-C to end" % func_name)
+    pcap_dev = pcap.open_dead(pcap.DLT_EN10MB, 1000)
+    # if args.file == '-':
+    #     tmp = tempfile.NamedTemporaryFile()
+    #     dumper = pcap.dump_open(pcap_dev, ctypes.c_char_p(tmp.name.encode("utf-8")))
+    # else:
+    dumper = pcap.dump_open(
+        pcap_dev, ctypes.c_char_p(args.file.encode("utf-8")))
+
+    print("Capturing packets from {func_name}... Hit Ctrl-C to end")
+
+    counter = 0
 
     def filter_events_cb(_cpu, data, _size):
+        nonlocal counter
+        counter += 1
         event = ctypes.cast(data, ctypes.POINTER(FilterPacket)).contents
         now = time.time()
         sec = int(now)
         usec = int((now - sec) * 1e6)
         tval = pcap.timeval(sec, usec)
         hdr = pcap.pkthdr(tval, 100, 100)
-        pcap.dump(ctypes.cast(dumper, ctypes.POINTER(ctypes.c_ubyte)), hdr, event.packet)
+        pcap.dump(ctypes.cast(dumper, ctypes.POINTER(
+            ctypes.c_ubyte)), hdr, event.packet)
 
     bctx['filter_event'].open_perf_buffer(filter_events_cb)
 
-    while True:
+    # if args.file == '-':
+    #     proc = subprocess.Popen(["tcpdump", "-r", "-", "-nev"], stdin=tmp,
+    #                             stdout=subprocess.PIPE, shell=False)
+
+    while counter < args.count:
         try:
-            bctx.perf_buffer_poll()
-        except:
+            bctx.perf_buffer_poll(timeout=1000)
+            # if args.file == '-' and proc.poll() is None:
+            #     output = proc.communicate(tmp.read())[0]
+            #     print(output)
+            #     line = proc.stdout.readline().strip(b'\n')
+            #     print(line.decode())
+        except KeyboardInterrupt:
             pcap.dump_close(dumper)
-            pcap.close(pd)
+            pcap.close(pcap_dev)
+            # if args.file == '-':
+            #     proc.stdout.close()
+            #     tmp.close()
             sys.exit()
+    print("{counter} packets cpatured")
+    pcap.dump_close(dumper)
+    pcap.close(pcap_dev)
 
 
-if __name__ == '__main__' :
+if __name__ == '__main__':
     main()
```

### Comparing `pycbpf-0.0.1/src/pycbpf/cbpf2c.py` & `pycbpf-0.0.2/pycbpf/cbpf2c.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,258 +1,274 @@
+"""
+The above code defines a class `CbpfC` that can compile a BPF filter program into a C function, and
+includes a main function that takes command line arguments to generate and print the C function.
+"""
 import argparse
 import libpcap as pcap
-from .filter2cbpf import cbpf_prog
+from .filter2cbpf import CbpfProg
 
-"""
-BPF compile to C class
-ref https://www.kernel.org/doc/Documentation/networking/filter.txt
-The BPF architecture consists of the following basic elements:
-  Element          Description
-
-  A                32 bit wide accumulator
-  X                32 bit wide X register
-  M[]              16 x 32 bit wide misc registers aka "scratch memory
-                   store", addressable from 0 to 15
-
-A program, that is translated by bpf_asm into "opcodes" is an array that
-consists of the following elements (as already mentioned):
-
-  op:16, jt:8, jf:8, k:32
-
-The element op is a 16 bit wide opcode that has a particular instruction
-encoded. jt and jf are two 8 bit wide jump targets, one for condition
-"jump if true", the other one "jump if false". Eventually, element k
-contains a miscellaneous argument that can be interpreted in different
-ways depending on the given instruction in op.
-
-The instruction set consists of load, store, branch, alu, miscellaneous
-and return instructions that are also represented in bpf_asm syntax. This
-table lists all bpf_asm instructions available resp. what their underlying
-opcodes as defined in linux/filter.h stand for:
- Instruction      Addressing mode      Description
-
-  ld               1, 2, 3, 4, 12       Load word into A
-  ldi              4                    Load word into A
-  ldh              1, 2                 Load half-word into A
-  ldb              1, 2                 Load byte into A
-  ldx              3, 4, 5, 12          Load word into X
-  ldxi             4                    Load word into X
-  ldxb             5                    Load byte into X
-
-  st               3                    Store A into M[]
-  stx              3                    Store X into M[]
-
-  jmp              6                    Jump to label
-  ja               6                    Jump to label
-  jeq              7, 8, 9, 10          Jump on A == <x>
-  jneq             9, 10                Jump on A != <x>
-  jne              9, 10                Jump on A != <x>
-  jlt              9, 10                Jump on A <  <x>
-  jle              9, 10                Jump on A <= <x>
-  jgt              7, 8, 9, 10          Jump on A >  <x>
-  jge              7, 8, 9, 10          Jump on A >= <x>
-  jset             7, 8, 9, 10          Jump on A &  <x>
-
-  add              0, 4                 A + <x>
-  sub              0, 4                 A - <x>
-  mul              0, 4                 A * <x>
-  div              0, 4                 A / <x>
-  mod              0, 4                 A % <x>
-  neg                                   !A
-  and              0, 4                 A & <x>
-  or               0, 4                 A | <x>
-  xor              0, 4                 A ^ <x>
-  lsh              0, 4                 A << <x>
-  rsh              0, 4                 A >> <x>
 
-  tax                                   Copy A into X
-  txa                                   Copy X into A
+class CbpfC:  # pylint: disable=too-few-public-methods
+    """
+    BPF compile to C class
+    ref https://www.kernel.org/doc/Documentation/networking/filter.txt
+    The BPF architecture consists of the following basic elements:
+    Element          Description
+
+    A                32 bit wide accumulator
+    X                32 bit wide X register
+    M[]              16 x 32 bit wide misc registers aka "scratch memory
+                    store", addressable from 0 to 15
+
+    A program, that is translated by bpf_asm into "opcodes" is an array that
+    consists of the following elements (as already mentioned):
+
+    op:16, jt:8, jf:8, k:32
+
+    The element op is a 16 bit wide opcode that has a particular instruction
+    encoded. jt and jf are two 8 bit wide jump targets, one for condition
+    "jump if true", the other one "jump if false". Eventually, element k
+    contains a miscellaneous argument that can be interpreted in different
+    ways depending on the given instruction in op.
+
+    The instruction set consists of load, store, branch, alu, miscellaneous
+    and return instructions that are also represented in bpf_asm syntax. This
+    table lists all bpf_asm instructions available resp. what their underlying
+    opcodes as defined in linux/filter.h stand for:
+    Instruction      Addressing mode      Description
+
+    ld               1, 2, 3, 4, 12       Load word into A
+    ldi              4                    Load word into A
+    ldh              1, 2                 Load half-word into A
+    ldb              1, 2                 Load byte into A
+    ldx              3, 4, 5, 12          Load word into X
+    ldxi             4                    Load word into X
+    ldxb             5                    Load byte into X
+
+    st               3                    Store A into M[]
+    stx              3                    Store X into M[]
+
+    jmp              6                    Jump to label
+    ja               6                    Jump to label
+    jeq              7, 8, 9, 10          Jump on A == <x>
+    jneq             9, 10                Jump on A != <x>
+    jne              9, 10                Jump on A != <x>
+    jlt              9, 10                Jump on A <  <x>
+    jle              9, 10                Jump on A <= <x>
+    jgt              7, 8, 9, 10          Jump on A >  <x>
+    jge              7, 8, 9, 10          Jump on A >= <x>
+    jset             7, 8, 9, 10          Jump on A &  <x>
+
+    add              0, 4                 A + <x>
+    sub              0, 4                 A - <x>
+    mul              0, 4                 A * <x>
+    div              0, 4                 A / <x>
+    mod              0, 4                 A % <x>
+    neg                                   !A
+    and              0, 4                 A & <x>
+    or               0, 4                 A | <x>
+    xor              0, 4                 A ^ <x>
+    lsh              0, 4                 A << <x>
+    rsh              0, 4                 A >> <x>
+
+    tax                                   Copy A into X
+    txa                                   Copy X into A
+
+    ret              4, 11                Return
+    """
 
-  ret              4, 11                Return
-"""
-class cbpf_c:
     def __init__(self, bpf):
         self._pc = 0
-        self._jumpLabels = {}
-        self._aluOps = {
-            pcap.BPF_ADD : "+",
-            pcap.BPF_SUB : "-",
-            pcap.BPF_MUL : "*",
-            pcap.BPF_DIV : "/",
-            pcap.BPF_AND : "&",
-            pcap.BPF_LSH : "<<",
-            pcap.BPF_RSH : ">>",
-            pcap.BPF_MOD : "%",
-            pcap.BPF_XOR : "^",
+        self._jump_labels = {}
+        self._alu_ops = {
+            pcap.BPF_ADD: "+",
+            pcap.BPF_SUB: "-",
+            pcap.BPF_MUL: "*",
+            pcap.BPF_DIV: "/",
+            pcap.BPF_AND: "&",
+            pcap.BPF_LSH: "<<",
+            pcap.BPF_RSH: ">>",
+            pcap.BPF_MOD: "%",
+            pcap.BPF_XOR: "^",
         }
         self._bpf = bpf
 
     def _jump_label(self, pos):
-        self._jumpLabels[pos] = "label%d" % pos
-        return "label%d" % pos
+        self._jump_labels[pos] = f"label{pos}"
+        return f"label{pos}"
 
     def _jump_cases(self, ins, cond, neg):
         if ins.jf == 0:
-            return "if (A %s %s) {goto %s;}" % (cond, self._alu_src(ins),
-                                                self._jump_label(self._pc + 1 + ins.jt))
+            next_pc = self._pc + 1 + ins.jt
+            return f"if (A {cond} {self._alu_src(ins)}) {{goto {self._jump_label(next_pc)};}}"
         if ins.jt == 0:
-            return "if (A %s %s) {goto %s;}" % (neg, self._alu_src(ins),
-                                                self._jump_label(self._pc + 1 + ins.jf))
-        else:
-            return "if (A %s %s) {goto %s;} else { goto %s;}" % (cond, self._alu_src(ins),
-                                                    self._jump_label(self._pc + 1 + ins.jt),
-                                                    self._jump_label(self._pc + 1 + ins.jf))
+            next_pc = self._pc + 1 + ins.jf
+            return f"if (A {neg} {self._alu_src(ins)}) {{goto {self._jump_label(next_pc)};}}"
+        fstr = f"if (A {cond} {self._alu_src(ins)})"
+        fstr += f"{{goto {self._jump_label(self._pc + 1 + ins.jt)};}}"
+        fstr += f" else {{ goto {self._jump_label(self._pc + 1 + ins.jf)};}}"
+        return fstr
 
-    def _ld_dst(self, ins):
+    @classmethod
+    def _ld_dst(cls, ins):
         if pcap.BPF_CLASS(ins.code) == pcap.BPF_LD:
             return "A"
-        elif pcap.BPF_CLASS(ins.code) == pcap.BPF_LDX:
-            return "X"
+        # elif pcap.BPF_CLASS(ins.code) == pcap.BPF_LDX:
+        return "X"
 
-    def _alu_src(self, ins):
+    @classmethod
+    def _alu_src(cls, ins):
         if pcap.BPF_SRC(ins.code) == pcap.BPF_K:
-            return "0x%x" % ins.k
-        elif pcap.BPF_SRC(ins.code) == pcap.BPF_X:
-            return "X"
+            return f"0x{ins.k:x}"
+        # elif pcap.BPF_SRC(ins.code) == pcap.BPF_X:
+        return "X"
 
     def _load_data_size(self, ins, data):
         check = ""
         if pcap.BPF_SIZE(ins.code) == pcap.BPF_B:
             width = 1
         elif pcap.BPF_SIZE(ins.code) == pcap.BPF_H:
             width = 2
         elif pcap.BPF_SIZE(ins.code) == pcap.BPF_W:
             width = 4
         if data == "data":
-            check = "if (data + %d + %d > data_end) { return 0; }\n\t" % (ins.k, width)
+            check = f"if (data + {ins.k} + {width} > data_end) {{ return 0; }}\n\t"
         elif data == "indirect":
             # ref https://www.kernel.org/doc/Documentation/networking/filter.txt
             check = "if (data + X > data_end) {return 0;}\n\t"
             check += "indirect = data + X;\n\t"
-            check += "if (indirect + %d + %d > data_end) {return 0;}\n\t" % (ins.k, width)
+            check += f"if (indirect + {ins.k} + {width} > data_end) {{return 0;}}\n\t"
 
         if pcap.BPF_SIZE(ins.code) == pcap.BPF_B:
-            return "%s%s = *(%s + %d);" % (check, self._ld_dst(ins), data, ins.k)
-        elif pcap.BPF_SIZE(ins.code) == pcap.BPF_H:
-            return "%s%s = bpf_ntohs(*((u16 *)(%s + %d)));" % (check, self._ld_dst(ins),
-                                                               data, ins.k)
-        elif pcap.BPF_SIZE(ins.code) == pcap.BPF_W:
-            return "%s%s = bpf_ntohl(*((u32 *) (%s + %d)));" % (check, self._ld_dst(ins),
-                                                                data, ins.k)
-
+            return f"{check}{self._ld_dst(ins)} = *({data} + {ins.k});"
+        if pcap.BPF_SIZE(ins.code) == pcap.BPF_H:
+            return f"{check}{self._ld_dst(ins)} = bpf_ntohs(*((u16 *)({data} + {ins.k})));"
+        if pcap.BPF_SIZE(ins.code) == pcap.BPF_W:
+            return f"{check}{self._ld_dst(ins)} = bpf_ntohl(*((u32 *) ({data} + {ins.k})));"
+        return ""
 
-    # ref https://github.com/iovisor/bpf-docs/blob/master/eBPF.md
-    """
-    LD/LDX/ST/STX opcode structure:
-
-    msb      lsb
-    +---+--+---+
-    |mde|sz|cls|
-    +---+--+---+
-    BPF_SIZE
-    BPF_MODE
-    BPF_CLASS
-    The sz field specifies the size of the memory location. The mde field is the
-    memory access mode. uBPF only supports the generic "MEM" access mode.
-
-    ALU/ALU64/JMP opcode structure:
-
-    msb      lsb
-    +----+-+---+
-    |op  |s|cls|
-    +----+-+---+
-    BPF_OP
-    BPF_SRC
-    BPF_CLASS
-    If the s bit is zero, then the source operand is imm. If s is one, then the source
-    operand is src. The op field specifies which ALU or branch operation is to be performed.
-    """
     def compile_cbpf_to_c(self) -> str:
+        """
+        ref https://github.com/iovisor/bpf-docs/blob/master/eBPF.md
+        LD/LDX/ST/STX opcode structure:
+
+        msb      lsb
+        +---+--+---+
+        |mde|sz|cls|
+        +---+--+---+
+        BPF_SIZE
+        BPF_MODE
+        BPF_CLASS
+        The sz field specifies the size of the memory location. The mde field is the
+        memory access mode. uBPF only supports the generic "MEM" access mode.
+
+        ALU/ALU64/JMP opcode structure:
+
+        msb      lsb
+        +----+-+---+
+        |op  |s|cls|
+        +----+-+---+
+        BPF_OP
+        BPF_SRC
+        BPF_CLASS
+        If the s bit is zero, then the source operand is imm. If s is one, then the source
+        operand is src. The op field specifies which ALU or branch operation is to be performed.
+        """
         ctext = """\nstatic inline u32
 cbpf_filter_func (const u8 *const data, const u8 *const data_end) {
 	__attribute__((unused)) u32 A, X, M[16];
 	__attribute__((unused)) const u8 *indirect;
 """
         for ins in self._bpf.ins:
             ctext += "\n"
-            if self._jumpLabels.get(self._pc) is not None:
-                ctext += self._jumpLabels.get(self._pc) + ":\n"
-            ctext += "\t%s" % self._convert_insn(ins)
+            if self._jump_labels.get(self._pc) is not None:
+                ctext += self._jump_labels.get(self._pc) + ":\n"
+            ctext += "\t" + self._convert_insn(ins)
             self._pc += 1
         ctext += "\n}"
         return ctext
 
-    #ref https://github.com/the-tcpdump-group/libpcap/blob/master/bpf_filter.c
+    # ref https://github.com/the-tcpdump-group/libpcap/blob/master/bpf_filter.c
     # ref bpf(7) https://www3.physnet.uni-hamburg.de/physnet/Tru64-Unix/HTML/MAN/MAN7/0012____.HTM
-    def _convert_insn(self, ins) -> str:
-        # print("{0x%x, %d, %d, 0x%x}" % (ins.code, ins.jt, ins.jf, ins.k))
+    def _convert_insn(self, ins) -> str:  # pylint: disable=too-many-return-statements,too-many-branches
         if pcap.BPF_CLASS(ins.code) == pcap.BPF_LD or pcap.BPF_CLASS(ins.code) == pcap.BPF_LDX:
             if pcap.BPF_MODE(ins.code) == pcap.BPF_IMM:
-                return "%s = %u;" % (self._ld_dst(ins), ins.k)
-            if pcap.BPF_MODE(ins.code) == pcap.BPF_IND:
-                return self._load_data_size(ins, "indirect")
+                mstr = f"{self._ld_dst(ins)} = {ins.k};"
+            elif pcap.BPF_MODE(ins.code) == pcap.BPF_IND:
+                mstr = self._load_data_size(ins, "indirect")
             elif pcap.BPF_MODE(ins.code) == pcap.BPF_ABS:
-                return self._load_data_size(ins, "data")
+                mstr = self._load_data_size(ins, "data")
             elif pcap.BPF_MODE(ins.code) == pcap.BPF_MEM:
-                return "%s = M[%d];" % (self._ld_dst(ins), ins.k)
+                mstr = f"{self._ld_dst(ins)} = M[{ins.k}];"
             elif pcap.BPF_MODE(ins.code) == pcap.BPF_LEN:
-                return "%s = data_end - data;" % (self._ld_dst(ins))
+                mstr = f"{self._ld_dst(ins)} = data_end - data;"
             elif pcap.BPF_MODE(ins.code) == pcap.BPF_MSH:
-                return self._load_data_size(ins, "data") + "X = (X & 0xF)<< 2;"
+                mstr = self._load_data_size(ins, "data") + "X = (X & 0xF)<< 2;"
+            return mstr
 
-        elif pcap.BPF_CLASS(ins.code) == pcap.BPF_ST:
-            return "M[%d] = A;" % ins.k
-        elif pcap.BPF_CLASS(ins.code) == pcap.BPF_STX:
-            return "M[%d] = X;" % ins.k
+        if pcap.BPF_CLASS(ins.code) == pcap.BPF_ST:
+            return f"M[{ins.k}] = A;"
+        if pcap.BPF_CLASS(ins.code) == pcap.BPF_STX:
+            return f"M[{ins.k}] = X;"
 
-        elif pcap.BPF_CLASS(ins.code) == pcap.BPF_ALU:
+        if pcap.BPF_CLASS(ins.code) == pcap.BPF_ALU:
             if pcap.BPF_OP(ins.code) == pcap.BPF_NEG:
-                return "A = -A;"
+                alustr = "A = -A;"
             elif pcap.BPF_OP(ins.code) > pcap.BPF_XOR:
-                return "NOT Support"
-            return "A %s= %s;" % (self._aluOps.get(pcap.BPF_OP(ins.code)), self._alu_src(ins))
+                alustr = "NOT Support"
+            else:
+                alustr = f"A {self._alu_ops.get(pcap.BPF_OP(ins.code))}= {self._alu_src(ins)};"
+            return alustr
 
-        elif pcap.BPF_CLASS(ins.code) == pcap.BPF_JMP:
-            """
-            - Conditional jt/jf targets replaced with jt/fall-through:
-
-            While the original design has constructs such as "if (cond) jump_true;
-            else jump_false;", they are being replaced into alternative constructs like
-            "if (cond) jump_true; /* else fall-through */".
-            """
+        if pcap.BPF_CLASS(ins.code) == pcap.BPF_JMP:
+            #  Conditional jt/jf targets replaced with jt/fall-through:
+            # While the original design has constructs such as "if (cond) jump_true;
+            # else jump_false;", they are being replaced into alternative constructs like
+            # "if (cond) jump_true; /* else fall-through */".
             if pcap.BPF_OP(ins.code) == pcap.BPF_JA:
-                return "goto %s" % self._jump_label(ins.k)
-            if pcap.BPF_OP(ins.code) == pcap.BPF_JEQ:
-                return self._jump_cases(ins, "==", "!=")
-            if pcap.BPF_OP(ins.code) == pcap.BPF_JGT:
-                return self._jump_cases(ins, ">", "<=")
-            if pcap.BPF_OP(ins.code) == pcap.BPF_JGE:
-                return self._jump_cases(ins, ">=", "<")
-            if pcap.BPF_OP(ins.code) == pcap.BPF_JSET:
-                return self._jump_cases(ins, "&", "|")
+                jstr = f"goto {self._jump_label(ins.k)}"
+            elif pcap.BPF_OP(ins.code) == pcap.BPF_JEQ:
+                jstr = self._jump_cases(ins, "==", "!=")
+            elif pcap.BPF_OP(ins.code) == pcap.BPF_JGT:
+                jstr = self._jump_cases(ins, ">", "<=")
+            elif pcap.BPF_OP(ins.code) == pcap.BPF_JGE:
+                jstr = self._jump_cases(ins, ">=", "<")
+            elif pcap.BPF_OP(ins.code) == pcap.BPF_JSET:
+                jstr = self._jump_cases(ins, "&", "|")
+            return jstr
 
-        elif pcap.BPF_CLASS(ins.code) == pcap.BPF_RET:
+        if pcap.BPF_CLASS(ins.code) == pcap.BPF_RET:
             if pcap.BPF_RVAL(ins.code) == pcap.BPF_A:
-                return "return A;"
+                rstr = "return A;"
             else:
-                return "return %d;" % ins.k
+                rstr = f"return {ins.k};"
+            return rstr
 
-        elif pcap.BPF_CLASS(ins.code) == pcap.BPF_MISC:
-            if pcap.BPF_MISCOP(ins.code) == pcap.BPF_TAX:
-                return "X = A;"
-            elif pcap.BPF_MISCOP(ins.code) == pcap.BPF_TXA:
-                return "A = X;"
+        # if pcap.BPF_CLASS(ins.code) == pcap.BPF_MISC:
+        if pcap.BPF_MISCOP(ins.code) == pcap.BPF_TAX:
+            miscstr = "X = A;"
+        elif pcap.BPF_MISCOP(ins.code) == pcap.BPF_TXA:
+            miscstr = "A = X;"
+        else:
+            miscstr = "Invalid ins"
+        return miscstr
 
 
 def main():
+    """
+    This function takes command line arguments for running tcpdump and compiles
+    a C function for a given filter.
+    """
     parser = argparse.ArgumentParser()
-    parser.add_argument("-i", "--interface", help="interface name to run tcpdump")
+    parser.add_argument("-i", "--interface",
+                        help="interface name to run tcpdump")
     parser.add_argument('filter', nargs=argparse.REMAINDER)
     args = parser.parse_args()
     if args.filter and len(args.filter) > 0:
-        prog = cbpf_prog(args.filter)
-        prog_c = cbpf_c(prog)
+        prog = CbpfProg(args.filter)
+        prog_c = CbpfC(prog)
         cfun = prog_c.compile_cbpf_to_c()
         print(cfun)
 
+
 if __name__ == '__main__':
     main()
```

### Comparing `pycbpf-0.0.1/tests/test_cbpf2c.py` & `pycbpf-0.0.2/tests/test_cbpf2c.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ctypes
 import socket
 import struct
 
 from bcc import BPF, libbcc
 from pycbpf import cbpf2c, filter2cbpf
 
-bpf_text = """
+BPF_TEXT = """
 
 %s
 
 int xdp_test_filter(struct xdp_md *ctx) {
 	void *data = (void *)(long)ctx->data;
 	void *data_end = (void *)(long)ctx->data_end;
 	
@@ -18,197 +18,167 @@
 		return 0;
 	}
 	return 1;
 }
 """
 
 # Calculate the checksum of the ICMP header and data
+
+
 def checksum(data):
-    n = len(data)
-    m = n % 2
+    length = len(data)
+    left = length % 2
     csum = 0
-    for i in range(0, n - m , 2):
+    for i in range(0, length - left, 2):
         csum += (data[i]) + ((data[i+1]) << 8)
-    if m:
+    if left:
         csum += (data[-1])
     csum = (csum >> 16) + (csum & 0xffff)
     csum += (csum >> 16)
     answer = ~csum & 0xffff
     answer = answer >> 8 | (answer << 8 & 0xff00)
     return answer
 
+
 def packet_generate(src_ip, dst_ip, proto):
     ip_saddr = socket.inet_aton(src_ip)
     ip_daddr = socket.inet_aton(dst_ip)
 
-    ip_tos = 0
-    ip_tot_len = 40
-    ip_id = 54321
-    ip_frag_off = 0
-    ip_ttl = 64
-    ip_proto = proto
-    ip_check = 0
     eth_header = struct.pack("!6s6sH", b"\x8c\x98\xbf\xae\x54\x2c", b"\x8e\x92\xcc\xdd\xee\xff",
-                            0x0800)
-    ip_header = struct.pack("!BBHHHBBH4s4s", 0x45, ip_tos, ip_tot_len, ip_id,
-                            ip_frag_off, ip_ttl, ip_proto, ip_check, ip_saddr, ip_daddr)
+                             0x0800)
+    # ipvl, ip_tos, ip_tot_len, ip_id, ip_frag_off, ip_ttl, ip_proto, ip_check, ip_sa, ip_da
+    ip_header = struct.pack("!BBHHHBBH4s4s", 0x45, 0, 0, 54321, 0, 64, proto, 0, ip_saddr, ip_daddr)
 
     if socket.IPPROTO_ICMP == proto:
-        icmp_type = 8
-        icmp_code = 0
         icmp_check = 0
-        icmp_id = 1
-        icmp_seq = 1
         icmp_data = b"Hello world!"
-        icmp_header = struct.pack("!BBHHH", icmp_type, icmp_code, icmp_check, icmp_id, icmp_seq)
+        icmp_header = struct.pack(
+            "!BBHHH", 8, 0, icmp_check, 1, 1)
         icmp_check = checksum(icmp_header + icmp_data)
-        icmp_header = struct.pack("!BBHHH", icmp_type, icmp_code, icmp_check, icmp_id, icmp_seq)
+        icmp_header = struct.pack(
+            "!BBHHH", 8, 0, icmp_check, 1, 1)
         packet = eth_header + ip_header + icmp_header + icmp_data
     elif socket.IPPROTO_UDP == proto:
         # UDP header: src port ffff , dst port fffe , len c , check ffff
         udp_header = struct.pack("!HHHH", 21, 65534, 12, 65535)
         udp_data = b"Hello world!"
         packet = eth_header + ip_header + udp_header + udp_data
     return packet
 
-def run_filter_test(fd, pkt, retval_expect):
+
+def run_filter_test(func_fd, pkt, retval_expect):
     size = len(pkt)
     data = ctypes.create_string_buffer(pkt, size)
     data_out = ctypes.create_string_buffer(1500)
     size_out = ctypes.c_uint32()
     retval = ctypes.c_uint32()
     duration = ctypes.c_uint32()
 
-    ret = libbcc.lib.bpf_prog_test_run(fd, 1,
+    ret = libbcc.lib.bpf_prog_test_run(func_fd, 1,
                                        ctypes.byref(data), size,
                                        ctypes.byref(data_out),
                                        ctypes.byref(size_out),
                                        ctypes.byref(retval),
                                        ctypes.byref(duration))
     if ret != 0:
         return False
-    return (retval.value == retval_expect)
+    return retval.value == retval_expect
 
 
 def test_cbpf_2_c():
-    prog = filter2cbpf.cbpf_prog(["ip"])
-    prog_c = cbpf2c.cbpf_c(prog)
+    prog = filter2cbpf.CbpfProg(["ip"])
+    prog_c = cbpf2c.CbpfC(prog)
     cfun = prog_c.compile_cbpf_to_c()
-    test_text = bpf_text%cfun
+    test_text = BPF_TEXT % cfun
     bpf_ctx = BPF(text=test_text, debug=4)
-    func = bpf_ctx.load_func(func_name=b"xdp_test_filter", prog_type = BPF.XDP)
+    func = bpf_ctx.load_func(func_name=b"xdp_test_filter", prog_type=BPF.XDP)
 
     pkt = packet_generate("192.168.0.1", "10.23.12.33", socket.IPPROTO_ICMP)
     assert run_filter_test(func.fd, pkt, 1)
 
 
 def test_cbpf_2_c_host():
-    prog = filter2cbpf.cbpf_prog(["host", "192.168.0.1"])
-    prog_c = cbpf2c.cbpf_c(prog)
+    prog = filter2cbpf.CbpfProg(["host", "192.168.0.1"])
+    prog_c = cbpf2c.CbpfC(prog)
     cfun = prog_c.compile_cbpf_to_c()
-    test_text = bpf_text%cfun
+    test_text = BPF_TEXT % cfun
     bpf_ctx = BPF(text=test_text, debug=4)
-    func = bpf_ctx.load_func(func_name=b"xdp_test_filter", prog_type = BPF.XDP)
+    func = bpf_ctx.load_func(func_name=b"xdp_test_filter", prog_type=BPF.XDP)
 
     pkt = packet_generate("192.168.0.1", "10.23.12.33", socket.IPPROTO_ICMP)
     assert run_filter_test(func.fd, pkt, 1)
 
 
 def test_cbpf_2_c_host_not_match():
-    prog = filter2cbpf.cbpf_prog(["host", "192.168.0.2"])
-    prog_c = cbpf2c.cbpf_c(prog)
+    prog = filter2cbpf.CbpfProg(["host", "192.168.0.2"])
+    prog_c = cbpf2c.CbpfC(prog)
     cfun = prog_c.compile_cbpf_to_c()
-    test_text = bpf_text%cfun
+    test_text = BPF_TEXT % cfun
     bpf_ctx = BPF(text=test_text, debug=4)
-    func = bpf_ctx.load_func(func_name=b"xdp_test_filter", prog_type = BPF.XDP)
+    func = bpf_ctx.load_func(func_name=b"xdp_test_filter", prog_type=BPF.XDP)
 
     pkt = packet_generate("192.168.0.1", "10.23.12.33", socket.IPPROTO_ICMP)
     assert run_filter_test(func.fd, pkt, 0)
 
 
 def test_cbpf_2_c_icmp():
-    prog = filter2cbpf.cbpf_prog(["icmp[0]==8"])
-    prog_c = cbpf2c.cbpf_c(prog)
+    prog = filter2cbpf.CbpfProg(["icmp[0]==8"])
+    prog_c = cbpf2c.CbpfC(prog)
     cfun = prog_c.compile_cbpf_to_c()
-    test_text = bpf_text%cfun
+    test_text = BPF_TEXT % cfun
     bpf_ctx = BPF(text=test_text, debug=4)
-    func = bpf_ctx.load_func(func_name=b"xdp_test_filter", prog_type = BPF.XDP)
+    func = bpf_ctx.load_func(func_name=b"xdp_test_filter", prog_type=BPF.XDP)
 
     pkt = packet_generate("192.168.0.1", "10.23.12.33", socket.IPPROTO_ICMP)
     assert run_filter_test(func.fd, pkt, 1)
 
 
 # test portrange with BPF_JGE
 def test_cbpf_2_c_portrange():
-    prog = filter2cbpf.cbpf_prog(["portrange", "21-23"])
-    prog_c = cbpf2c.cbpf_c(prog)
+    prog = filter2cbpf.CbpfProg(["portrange", "21-23"])
+    prog_c = cbpf2c.CbpfC(prog)
     cfun = prog_c.compile_cbpf_to_c()
-    test_text = bpf_text%cfun
+    test_text = BPF_TEXT % cfun
     bpf_ctx = BPF(text=test_text, debug=4)
-    func = bpf_ctx.load_func(func_name=b"xdp_test_filter", prog_type = BPF.XDP)
+    func = bpf_ctx.load_func(func_name=b"xdp_test_filter", prog_type=BPF.XDP)
 
     pkt = packet_generate("192.168.0.1", "10.23.12.33", socket.IPPROTO_UDP)
     assert run_filter_test(func.fd, pkt, 1)
 
 
-#test geneve with st/stx
-def test_cbpf_2_c_geneve():
-    version = 0 # 2 bits
-    opt_len = 0 # 6 bits
-    oam = 0 # 1 bit
-    critical = 0 # 1 bit
-    reserved = 0 # 6 bits
-    protocol_type = 0x6558 # 16 bits
-    vni = 1234 # 24 bits
-    reserved2 = 0 # 8 bits
-    geneve_header = struct.pack(">BBHHHB", version << 6 | opt_len,
-                                oam << 7 | critical << 6 | reserved,
-                                protocol_type, vni >> 8, vni & 0xff, reserved2)
+# test geneve with st/stx
+def test_cbpf_2_c_geneve(): # pylint: disable=too-many-locals
+    geneve_header = struct.pack(">BBHHHB", 0, 0, 0x6558, 1234 >> 8, 1234 & 0xff, 0)
     payload = b"\x00\x01\x02\x03\x04\x05\x06\x07\x08\x09\x0a\x0b\x0c\x0d\x0e\x0f"
 
     geneve_packet = geneve_header + payload
 
-    dst_mac = b"\xaa\xbb\xcc\xdd\xee\xff" # 6 bytes
-    src_mac = b"\x11\x22\x33\x44\x55\x66" # 6 bytes
-    eth_type = 0x0800 # 2 bytes, IP protocol
-
-    eth_header = struct.pack(">6s6sH", dst_mac, src_mac, eth_type)
-
-    tos = 0 # 1 byte
-    total_length = 20 + 8 + len(geneve_packet)
-    identification = 0 # 2 bytes
-    flags = 0 # 3 bits
-    fragment_offset = 0 # 13 bits
-    ttl = 64 # 1 byte
-    protocol = 17 # 1 byte, UDP protocol
-    ip_checksum = 0 # 2 bytes, to be calculated later
-    src_ip = b"\xc0\xa8\x01\x01" # 4 bytes, 192.168.1.1
-    dst_ip = b"\xc0\xa8\x01\x02" # 4 bytes, 192.168.1.2
-    ip_header = struct.pack(">BBHHHBBH4s4s", 0x45, tos, total_length, identification,
-                            flags << 13 | fragment_offset, ttl, protocol, ip_checksum,
-                            src_ip, dst_ip)
-
-    src_port = 6081 # 2 bytes
-    dst_port = 6081 # 2 bytes
-    length = 8 + len(geneve_packet) # 2 bytes, UDP header + Geneve packet length
-    udp_checksum = 0
-    udp_header = struct.pack(">HHHH", src_port, dst_port, length, udp_checksum)
+    dst_mac = b"\xaa\xbb\xcc\xdd\xee\xff"  # 6 bytes
+    src_mac = b"\x11\x22\x33\x44\x55\x66"  # 6 bytes
+
+    eth_header = struct.pack(">6s6sH", dst_mac, src_mac, 0x0800)
+
+    src_ip = b"\xc0\xa8\x01\x01"  # 4 bytes, 192.168.1.1
+    dst_ip = b"\xc0\xa8\x01\x02"  # 4 bytes, 192.168.1.2
+    ip_header = struct.pack(">BBHHHBBH4s4s", 0x45, 0, 20 + 8 + len(geneve_packet), 0,
+                            0, 64, 17, 0, src_ip, dst_ip)
+
+    udp_header = struct.pack(">HHHH", 6081, 6081, 8 + len(geneve_packet), 0)
     outer_packet = eth_header + ip_header + udp_header + geneve_packet
-    prog = filter2cbpf.cbpf_prog(["geneve"])
-    prog_c = cbpf2c.cbpf_c(prog)
+    prog = filter2cbpf.CbpfProg(["geneve"])
+    prog_c = cbpf2c.CbpfC(prog)
     cfun = prog_c.compile_cbpf_to_c()
-    test_text = bpf_text%cfun
-    bpf_ctx = BPF(text=test_text, debug=4)
-    func = bpf_ctx.load_func(func_name=b"xdp_test_filter", prog_type = BPF.XDP)
+    bpf_ctx = BPF(text=BPF_TEXT % cfun, debug=4)
+    func = bpf_ctx.load_func(func_name=b"xdp_test_filter", prog_type=BPF.XDP)
     assert run_filter_test(func.fd, outer_packet, 1)
 
 
 def test_cbpf_2_c_len():
-    prog = filter2cbpf.cbpf_prog(["len<=100"])
-    prog_c = cbpf2c.cbpf_c(prog)
+    prog = filter2cbpf.CbpfProg(["len<=100"])
+    prog_c = cbpf2c.CbpfC(prog)
     cfun = prog_c.compile_cbpf_to_c()
-    test_text = bpf_text%cfun
+    test_text = BPF_TEXT % cfun
     bpf_ctx = BPF(text=test_text, debug=4)
-    func = bpf_ctx.load_func(func_name=b"xdp_test_filter", prog_type = BPF.XDP)
+    func = bpf_ctx.load_func(func_name=b"xdp_test_filter", prog_type=BPF.XDP)
 
     pkt = packet_generate("192.168.0.1", "10.23.12.33", socket.IPPROTO_UDP)
     assert run_filter_test(func.fd, pkt, 1)
```

### Comparing `pycbpf-0.0.1/tests/test_filter2cbpf.py` & `pycbpf-0.0.2/tests/test_filter2cbpf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 import subprocess
 import libpcap as pcap
 from pycbpf import filter2cbpf as fc
 
-def bpf_insn_eq(insa :pcap.bpf_insn, insb :pcap.bpf_insn):
+
+def bpf_insn_eq(insa: pcap.bpf_insn, insb: pcap.bpf_insn):
     if insa.code != insb.code:
         return False
     if insa.jt != insb.jt:
         return False
     if insa.jf != insb.jf:
         return False
     if insa.k != insb.k:
         return False
     return True
 
+
 def bpf_prog_eq(insa, insb):
     if len(insa) != len(insb):
         return False
     for i, j in zip(insa, insb):
         if bpf_insn_eq(i, j) is False:
             return False
     return True
 
+
 def tcpdump_args_to_bpf_insn(args):
     insn = []
-    proc = subprocess.Popen(["tcpdump", "-ddd"] + args, shell=False, stdout=subprocess.PIPE)
-    output, _ = proc.communicate()
-    _, ins_lines = output.splitlines()[0], output.splitlines()[1:]
+    ret = subprocess.run(["tcpdump", "-ddd"] + args,
+                            shell=False, stdout=subprocess.PIPE, check=True)
+    _, ins_lines = ret.stdout.splitlines()[0], ret.stdout.splitlines()[1:]
     for line in ins_lines:
-        code, jt, jf, k = line.split()
-        insn.append(pcap.bpf_insn(int(code), int(jt), int(jf), int(k)))
+        code, jump_t, jump_f, k = line.split()
+        insn.append(pcap.bpf_insn(int(code), int(jump_t), int(jump_f), int(k)))
     return insn
 
 
 def verify_cbpf_prog(args):
     largs = args.split()
-    prog = fc.cbpf_prog(largs)
+    prog = fc.CbpfProg(largs)
     ins = tcpdump_args_to_bpf_insn(largs)
     return bpf_prog_eq(prog.ins, ins)
 
 # test indirect ld
+
+
 def test_filter_2_cbpf():
     cases = ["ip", "ip6", "host 192.168.0.1", "udp port 4567", "net 192.168.0.0/24",
              "src 1.1.1.1 or 1.1.1.2", "src 1.1.1.1 and (dst 1.1.1.2 or host 1.1.1.3) and port 80",
              "ether proto 0x0806", "tcp[tcpflags] & (tcp-syn|tcp-ack) != 0",
              "icmp[0] != 8 and icmp[0] != 0", "udp[42:4]=0xAC100009"]
-    for c in cases:
-        assert verify_cbpf_prog(c)
+    for case in cases:
+        assert verify_cbpf_prog(case)
```

