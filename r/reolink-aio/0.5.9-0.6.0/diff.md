# Comparing `tmp/reolink_aio-0.5.9.tar.gz` & `tmp/reolink_aio-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reolink_aio-0.5.9.tar", last modified: Fri Mar 31 15:05:48 2023, max compression
+gzip compressed data, was "reolink_aio-0.6.0.tar", last modified: Thu Jun  8 13:22:18 2023, max compression
```

## Comparing `reolink_aio-0.5.9.tar` & `reolink_aio-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-31 15:05:48.760459 reolink_aio-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-03-31 15:05:37.000000 reolink_aio-0.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4113 2023-03-31 15:05:48.760459 reolink_aio-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3305 2023-03-31 15:05:37.000000 reolink_aio-0.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-31 15:05:48.756459 reolink_aio-0.5.9/reolink_aio/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-03-31 15:05:37.000000 reolink_aio-0.5.9/reolink_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   168286 2023-03-31 15:05:37.000000 reolink_aio-0.5.9/reolink_aio/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-03-31 15:05:37.000000 reolink_aio-0.5.9/reolink_aio/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-03-31 15:05:37.000000 reolink_aio-0.5.9/reolink_aio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8014 2023-03-31 15:05:37.000000 reolink_aio-0.5.9/reolink_aio/software_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     4713 2023-03-31 15:05:37.000000 reolink_aio-0.5.9/reolink_aio/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)      590 2023-03-31 15:05:37.000000 reolink_aio-0.5.9/reolink_aio/typings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-31 15:05:48.760459 reolink_aio-0.5.9/reolink_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4113 2023-03-31 15:05:48.000000 reolink_aio-0.5.9/reolink_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-03-31 15:05:48.000000 reolink_aio-0.5.9/reolink_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-31 15:05:48.000000 reolink_aio-0.5.9/reolink_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-31 15:05:48.000000 reolink_aio-0.5.9/reolink_aio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-03-31 15:05:48.000000 reolink_aio-0.5.9/reolink_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-03-31 15:05:48.000000 reolink_aio-0.5.9/reolink_aio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-31 15:05:48.760459 reolink_aio-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-03-31 15:05:37.000000 reolink_aio-0.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-31 15:05:48.760459 reolink_aio-0.5.9/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-03-31 15:05:37.000000 reolink_aio-0.5.9/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 13:22:18.230997 reolink_aio-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-08 13:22:18.230997 reolink_aio-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 13:22:18.230997 reolink_aio-0.6.0/reolink_aio/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   187483 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1377 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/software_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4713 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15190 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/typings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/reolink_aio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 13:22:18.230997 reolink_aio-0.6.0/reolink_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-08 13:22:18.000000 reolink_aio-0.6.0/reolink_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-06-08 13:22:18.000000 reolink_aio-0.6.0/reolink_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 13:22:18.000000 reolink_aio-0.6.0/reolink_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 13:22:18.000000 reolink_aio-0.6.0/reolink_aio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-08 13:22:18.000000 reolink_aio-0.6.0/reolink_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-08 13:22:18.000000 reolink_aio-0.6.0/reolink_aio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-08 13:22:18.230997 reolink_aio-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 13:22:18.230997 reolink_aio-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-06-08 13:22:04.000000 reolink_aio-0.6.0/tests/test.py
```

### Comparing `reolink_aio-0.5.9/LICENSE` & `reolink_aio-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.5.9/PKG-INFO` & `reolink_aio-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7265 6f6c  : 2.1.Name: reol
 00000020: 696e 6b5f 6169 6f0a 5665 7273 696f 6e3a  ink_aio.Version:
-00000030: 2030 2e35 2e39 0a53 756d 6d61 7279 3a20   0.5.9.Summary: 
+00000030: 2030 2e36 2e30 0a53 756d 6d61 7279 3a20   0.6.0.Summary: 
 00000040: 5265 6f6c 696e 6b20 4e56 522f 6361 6d65  Reolink NVR/came
 00000050: 7261 7320 4150 4920 7061 636b 6167 650a  ras API package.
 00000060: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
 00000070: 3a2f 2f67 6974 6875 622e 636f 6d2f 7374  ://github.com/st
 00000080: 6172 6b69 6c6c 6572 4f47 2f72 656f 6c69  arkillerOG/reoli
 00000090: 6e6b 5f61 696f 0a41 7574 686f 723a 2073  nk_aio.Author: s
 000000a0: 7461 726b 696c 6c65 724f 470a 4175 7468  tarkillerOG.Auth
@@ -71,188 +71,216 @@
 00000460: 6869 656c 6473 2e69 6f2f 7374 6174 6963  hields.io/static
 00000470: 2f76 313f 6c61 6265 6c3d 5370 6f6e 736f  /v1?label=Sponso
 00000480: 7226 6d65 7373 6167 653d 2545 3225 3944  r&message=%E2%9D
 00000490: 2541 3426 6c6f 676f 3d47 6974 4875 6226  %A4&logo=GitHub&
 000004a0: 636f 6c6f 723d 2532 3366 6538 6538 3622  color=%23fe8e86"
 000004b0: 2061 6c74 3d22 5370 6f6e 736f 7222 3e3c   alt="Sponsor"><
 000004c0: 2f61 3e0a 2020 3c61 2068 7265 663d 2268  /a>.  <a href="h
-000004d0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-000004e0: 7072 6f6a 6563 742f 7265 6f6c 696e 6b2d  project/reolink-
-000004f0: 6169 6f22 3e3c 696d 6720 7372 633d 2268  aio"><img src="h
-00000500: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000510: 6473 2e69 6f2f 7079 7069 2f64 6d2f 7265  ds.io/pypi/dm/re
-00000520: 6f6c 696e 6b2d 6169 6f22 3e3c 2f61 3e0a  olink-aio"></a>.
-00000530: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000540: 3a2f 2f67 6974 6875 622e 636f 6d2f 7374  ://github.com/st
-00000550: 6172 6b69 6c6c 6572 4f47 2f72 656f 6c69  arkillerOG/reoli
-00000560: 6e6b 5f61 696f 2f72 656c 6561 7365 7322  nk_aio/releases"
-00000570: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00000580: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000590: 6f2f 6769 7468 7562 2f76 2f72 656c 6561  o/github/v/relea
-000005a0: 7365 2f53 7461 726b 696c 6c65 724f 472f  se/StarkillerOG/
-000005b0: 7265 6f6c 696e 6b5f 6169 6f3f 6469 7370  reolink_aio?disp
-000005c0: 6c61 795f 6e61 6d65 3d74 6167 2669 6e63  lay_name=tag&inc
-000005d0: 6c75 6465 5f70 7265 7265 6c65 6173 6573  lude_prereleases
-000005e0: 2673 6f72 743d 7365 6d76 6572 2220 616c  &sort=semver" al
-000005f0: 743d 2243 7572 7265 6e74 2076 6572 7369  t="Current versi
-00000600: 6f6e 223e 3c2f 613e 0a3c 2f70 3e0a 0a54  on"></a>.</p>..T
-00000610: 6865 2060 7265 6f6c 696e 6b5f 6169 6f60  he `reolink_aio`
-00000620: 2050 7974 686f 6e20 7061 636b 6167 6520   Python package 
-00000630: 616c 6c6f 7773 2079 6f75 2074 6f20 696e  allows you to in
-00000640: 7465 6772 6174 6520 796f 7572 205b 5265  tegrate your [Re
-00000650: 6f6c 696e 6b5d 2868 7474 7073 3a2f 2f77  olink](https://w
-00000660: 7777 2e72 656f 6c69 6e6b 2e63 6f6d 2f29  ww.reolink.com/)
-00000670: 2064 6576 6963 6573 2028 4e56 522f 6361   devices (NVR/ca
-00000680: 6d65 7261 7329 2069 6e20 796f 7572 2061  meras) in your a
-00000690: 7070 6c69 6361 7469 6f6e 2e0a 0a23 2323  pplication...###
-000006a0: 2044 6573 6372 6970 7469 6f6e 0a0a 5468   Description..Th
-000006b0: 6973 2069 7320 6120 7061 636b 6167 6520  is is a package 
-000006c0: 696d 706c 656d 656e 7469 6e67 2052 656f  implementing Reo
-000006d0: 6c69 6e6b 2049 5020 4e56 5220 616e 6420  link IP NVR and 
-000006e0: 6361 6d65 7261 2041 5049 2e20 416c 736f  camera API. Also
-000006f0: 2069 74e2 8099 7320 7072 6f76 6964 696e   it...s providin
-00000700: 6720 6120 7761 7920 746f 2073 7562 7363  g a way to subsc
-00000710: 7269 6265 2074 6f20 5265 6f6c 696e 6b20  ribe to Reolink 
-00000720: 4f4e 5649 4620 5357 4e20 6576 656e 7473  ONVIF SWN events
-00000730: 2c20 736f 2074 6861 7420 7265 616c 2d74  , so that real-t
-00000740: 696d 6520 6576 656e 7473 2063 616e 2062  ime events can b
-00000750: 6520 7265 6365 6976 6564 206f 6e20 6120  e received on a 
-00000760: 7765 6268 6f6f 6b2e 0a0a 2323 2320 5072  webhook...### Pr
-00000770: 6572 6571 7569 7369 7465 730a 0a2d 2050  erequisites..- P
-00000780: 7974 686f 6e20 332e 390a 0a23 2323 2049  ython 3.9..### I
-00000790: 6e73 7461 6c6c 6174 696f 6e0a 0a60 6060  nstallation..```
-000007a0: 0a70 6970 3320 696e 7374 616c 6c20 7265  .pip3 install re
-000007b0: 6f6c 696e 6b2d 6169 6f0a 6060 600a 0a6f  olink-aio.```..o
-000007c0: 7220 6d61 6e75 616c 6c79 3a0a 6060 6060  r manually:.````
-000007d0: 0a67 6974 2063 6c6f 6e65 2068 7474 7073  .git clone https
-000007e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5374  ://github.com/St
-000007f0: 6172 6b69 6c6c 6572 4f47 2f72 656f 6c69  arkillerOG/reoli
-00000800: 6e6b 5f61 696f 0a63 6420 7265 6f6c 696e  nk_aio.cd reolin
-00000810: 6b5f 6169 6f2f 0a70 6970 3320 696e 7374  k_aio/.pip3 inst
-00000820: 616c 6c20 2e0a 6060 6060 0a0a 2323 2320  all ..````..### 
-00000830: 5573 6167 650a 0a60 6060 600a 6672 6f6d  Usage..````.from
-00000840: 2072 656f 6c69 6e6b 5f61 696f 2e61 7069   reolink_aio.api
-00000850: 2069 6d70 6f72 7420 486f 7374 0a69 6d70   import Host.imp
-00000860: 6f72 7420 6173 796e 6369 6f0a 0a23 2043  ort asyncio..# C
-00000870: 7265 6174 6520 6120 686f 7374 2d6f 626a  reate a host-obj
-00000880: 6563 7420 2872 6570 7265 7365 6e74 696e  ect (representin
-00000890: 6720 6569 7468 6572 2061 2063 616d 6572  g either a camer
-000008a0: 612c 206f 7220 4e56 5220 7769 7468 2073  a, or NVR with s
-000008b0: 6576 6572 616c 2063 6861 6e6e 656c 7329  everal channels)
-000008c0: 0a68 6f73 7420 3d20 486f 7374 2827 3139  .host = Host('19
-000008d0: 322e 3136 382e 312e 3130 272c 2038 302c  2.168.1.10', 80,
-000008e0: 2027 7573 6572 272c 2027 6d79 7061 7373   'user', 'mypass
-000008f0: 776f 7264 2729 0a0a 2320 4f62 7461 696e  word')..# Obtain
-00000900: 2f63 6163 6865 204e 5652 206f 7220 6361  /cache NVR or ca
-00000910: 6d65 7261 2073 6574 7469 6e67 7320 616e  mera settings an
-00000920: 6420 6361 7061 6269 6c69 7469 6573 2c20  d capabilities, 
-00000930: 6c69 6b65 206d 6f64 656c 206e 616d 652c  like model name,
-00000940: 2070 6f72 7473 2c20 4844 4420 7369 7a65   ports, HDD size
-00000950: 2c20 6574 633a 0a61 7761 6974 2068 6f73  , etc:.await hos
-00000960: 742e 6765 745f 686f 7374 5f64 6174 6128  t.get_host_data(
-00000970: 290a 0a23 2047 6574 2074 6865 2073 7562  )..# Get the sub
-00000980: 7363 7269 6274 696f 6e20 706f 7274 2061  scribtion port a
-00000990: 6e64 2068 6f73 742d 6465 7669 6365 206e  nd host-device n
-000009a0: 616d 653a 0a73 7562 7363 7269 6274 696f  ame:.subscribtio
-000009b0: 6e5f 706f 7274 203d 2020 686f 7374 2e6f  n_port =  host.o
-000009c0: 6e76 6966 5f70 6f72 740a 6e61 6d65 203d  nvif_port.name =
-000009d0: 2068 6f73 742e 6e76 725f 6e61 6d65 0a0a   host.nvr_name..
-000009e0: 2320 4f62 7461 696e 2f63 6163 6865 2073  # Obtain/cache s
-000009f0: 7461 7465 7320 6f66 2066 6561 7475 7265  tates of feature
-00000a00: 733a 0a61 7761 6974 2068 6f73 742e 6765  s:.await host.ge
-00000a10: 745f 7374 6174 6573 2829 0a0a 2320 5072  t_states()..# Pr
-00000a20: 696e 7420 736f 6d65 2073 7461 7465 2076  int some state v
-00000a30: 616c 7565 206f 6e20 7468 6520 6368 616e  alue on the chan
-00000a40: 6e65 6c20 7769 7468 2069 6e64 6578 2030  nel with index 0
-00000a50: 3a0a 7072 696e 7428 686f 7374 2e69 725f  :.print(host.ir_
-00000a60: 656e 6162 6c65 6428 3029 290a 0a23 2045  enabled(0))..# E
-00000a70: 6e61 626c 6520 7468 6520 696e 6672 6172  nable the infrar
-00000a80: 6564 206c 6967 6874 7320 6f6e 2074 6865  ed lights on the
-00000a90: 2063 6861 6e6e 656c 2077 6974 6820 696e   channel with in
-00000aa0: 6465 7820 313a 0a61 7761 6974 2068 6f73  dex 1:.await hos
-00000ab0: 742e 7365 745f 6972 5f6c 6967 6874 7328  t.set_ir_lights(
-00000ac0: 312c 2054 7275 6529 0a0a 2320 456e 6162  1, True)..# Enab
-00000ad0: 6c65 2074 6865 2073 706f 746c 6967 6874  le the spotlight
-00000ae0: 206f 6e20 7468 6520 6368 616e 6e65 6c20   on the channel 
-00000af0: 7769 7468 2069 6e64 6578 2031 3a0a 6177  with index 1:.aw
-00000b00: 6169 7420 686f 7374 2e73 6574 5f73 706f  ait host.set_spo
-00000b10: 746c 6967 6874 2831 2c20 5472 7565 290a  tlight(1, True).
-00000b20: 0a23 2045 6e61 626c 6520 7468 6520 7369  .# Enable the si
-00000b30: 7265 6e20 6f6e 2074 6865 2063 6861 6e6e  ren on the chann
-00000b40: 656c 2077 6974 6820 696e 6465 7820 303a  el with index 0:
-00000b50: 0a61 7761 6974 2068 6f73 742e 7365 745f  .await host.set_
-00000b60: 7369 7265 6e28 302c 2054 7275 6529 0a0a  siren(0, True)..
-00000b70: 2320 4e6f 7720 7375 6273 6372 6962 6520  # Now subscribe 
-00000b80: 746f 2065 7665 6e74 732c 2073 7570 706f  to events, suppo
-00000b90: 7365 206f 7572 2077 6562 686f 6f6b 2075  se our webhook u
-00000ba0: 726c 2069 7320 6874 7470 3a2f 2f31 3932  rl is http://192
-00000bb0: 2e31 3638 2e31 2e31 312f 7765 6268 6f6f  .168.1.11/webhoo
-00000bc0: 6b31 3233 0a61 7761 6974 2068 6f73 742e  k123.await host.
-00000bd0: 7375 6273 6372 6962 6528 2768 7474 703a  subscribe('http:
-00000be0: 2f2f 3139 322e 3136 382e 312e 3131 2f77  //192.168.1.11/w
-00000bf0: 6562 686f 6f6b 3132 3327 290a 0a23 2041  ebhook123')..# A
-00000c00: 6674 6572 2073 6f6d 6520 6d69 6e75 7465  fter some minute
-00000c10: 7320 6368 6563 6b20 7468 6520 7265 6e65  s check the rene
-00000c20: 7720 7469 6d65 7220 286b 6565 7020 7468  w timer (keep th
-00000c30: 6520 6576 656e 7469 6e67 2061 6c69 7665  e eventing alive
-00000c40: 293a 0a69 6620 2868 6f73 742e 7265 6e65  ):.if (host.rene
-00000c50: 7754 696d 6572 203c 3d20 3130 3029 3a0a  wTimer <= 100):.
-00000c60: 2020 2020 6177 6169 7420 686f 7374 2e72      await host.r
-00000c70: 656e 6577 2829 0a0a 2320 4c6f 676f 7574  enew()..# Logout
-00000c80: 2061 6e64 2064 6973 636f 6e6e 6563 740a   and disconnect.
-00000c90: 6177 6169 7420 686f 7374 2e64 6973 636f  await host.disco
-00000ca0: 6e6e 6563 7428 290a 6060 6060 0a0a 2323  nnect().````..##
-00000cb0: 2320 4578 616d 706c 650a 0a54 6869 7320  # Example..This 
-00000cc0: 6973 2061 6e20 6578 616d 706c 6520 6f66  is an example of
-00000cd0: 2074 6865 2075 7361 6765 206f 6620 7468   the usage of th
-00000ce0: 6520 4150 492e 2049 6e20 7468 6973 2063  e API. In this c
-00000cf0: 6173 6520 7765 2077 616e 7420 746f 2072  ase we want to r
-00000d00: 6574 7269 7665 2061 6e64 2070 7269 6e74  etrive and print
-00000d10: 2074 6865 204d 6163 2041 6464 7265 7373   the Mac Address
-00000d20: 206f 6620 7468 6520 4e56 522e 0a60 6060   of the NVR..```
-00000d30: 600a 6672 6f6d 2072 656f 6c69 6e6b 5f61  `.from reolink_a
-00000d40: 696f 2e61 7069 2069 6d70 6f72 7420 486f  io.api import Ho
-00000d50: 7374 0a69 6d70 6f72 7420 6173 796e 6369  st.import asynci
-00000d60: 6f0a 0a61 7379 6e63 2064 6566 2070 7269  o..async def pri
-00000d70: 6e74 5f6d 6163 5f61 6464 7265 7373 2829  nt_mac_address()
-00000d80: 3a0a 2020 2020 2320 696e 6974 6961 6c69  :.    # initiali
-00000d90: 7a65 2074 6865 2068 6f73 740a 2020 2020  ze the host.    
-00000da0: 686f 7374 203d 2048 6f73 7428 2731 3932  host = Host('192
-00000db0: 2e31 3638 2e31 2e31 3039 272c 2761 646d  .168.1.109','adm
-00000dc0: 696e 272c 2027 6164 6d69 6e31 3233 3427  in', 'admin1234'
-00000dd0: 2c20 706f 7274 3d38 3029 0a20 2020 2023  , port=80).    #
-00000de0: 2063 6f6e 6e65 6374 2061 6e64 206f 6274   connect and obt
-00000df0: 6169 6e2f 6361 6368 6520 6465 7669 6365  ain/cache device
-00000e00: 2073 6574 7469 6e67 7320 616e 6420 6361   settings and ca
-00000e10: 7061 6269 6c69 7469 6573 0a20 2020 2061  pabilities.    a
-00000e20: 7761 6974 2068 6f73 742e 6765 745f 686f  wait host.get_ho
-00000e30: 7374 5f64 6174 6128 290a 2020 2020 2320  st_data().    # 
-00000e40: 6368 6563 6b20 6966 2069 7420 6973 2061  check if it is a
-00000e50: 2063 616d 6572 6120 6f72 2061 6e20 4e56   camera or an NV
-00000e60: 520a 2020 2020 7072 696e 7428 2249 7420  R.    print("It 
-00000e70: 6973 2061 6e20 4e56 523a 2025 732c 206e  is an NVR: %s, n
-00000e80: 756d 6265 7220 6f66 2063 6861 6e6e 656c  umber of channel
-00000e90: 733a 2025 7322 2c20 686f 7374 2e69 735f  s: %s", host.is_
-00000ea0: 6e76 722c 2068 6f73 742e 6e75 6d5f 6368  nvr, host.num_ch
-00000eb0: 616e 6e65 6c73 290a 2020 2020 2320 7072  annels).    # pr
-00000ec0: 696e 7420 6d61 6320 6164 6472 6573 730a  int mac address.
-00000ed0: 2020 2020 7072 696e 7428 686f 7374 2e6d      print(host.m
-00000ee0: 6163 5f61 6464 7265 7373 290a 2020 2020  ac_address).    
-00000ef0: 2320 636c 6f73 6520 7468 6520 6465 7669  # close the devi
-00000f00: 6365 2063 6f6e 6e65 6374 696f 6e0a 2020  ce connection.  
-00000f10: 2020 6177 6169 7420 686f 7374 2e6c 6f67    await host.log
-00000f20: 6f75 7428 290a 0a69 6620 5f5f 6e61 6d65  out()..if __name
-00000f30: 5f5f 203d 3d20 225f 5f6d 6169 6e5f 5f22  __ == "__main__"
-00000f40: 3a0a 2020 2020 6173 796e 6369 6f2e 7275  :.    asyncio.ru
-00000f50: 6e28 7072 696e 745f 6d61 635f 6164 6472  n(print_mac_addr
-00000f60: 6573 7328 2929 0a60 6060 600a 0a23 2323  ess()).````..###
-00000f70: 2041 636b 6e6f 776c 6564 676d 656e 740a   Acknowledgment.
-00000f80: 5468 6973 206c 6962 7261 7279 2069 7320  This library is 
-00000f90: 6261 7365 6420 6f6e 2074 6865 2077 6f72  based on the wor
-00000fa0: 6b20 6f66 3a0a 2d20 6677 6573 7465 6e62  k of:.- fwestenb
-00000fb0: 6572 673a 2068 7474 7073 3a2f 2f67 6974  erg: https://git
-00000fc0: 6875 622e 636f 6d2f 6677 6573 7465 6e62  hub.com/fwestenb
-00000fd0: 6572 672f 7265 6f6c 696e 6b5f 6465 760a  erg/reolink_dev.
-00000fe0: 2d20 4a69 6d53 7461 723a 2068 7474 7073  - JimStar: https
-00000ff0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a69  ://github.com/Ji
-00001000: 6d53 7461 722f 7265 6f6c 696e 6b5f 6970  mStar/reolink_ip
-00001010: 0a                                       .
+000004d0: 7474 7073 3a2f 2f72 656f 6c69 6e6b 2e70  ttps://reolink.p
+000004e0: 7866 2e69 6f2f 7134 3451 5771 223e 3c69  xf.io/q44QWq"><i
+000004f0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000500: 696d 672e 7368 6965 6c64 732e 696f 2f73  img.shields.io/s
+00000510: 7461 7469 632f 7631 3f6c 6162 656c 3d41  tatic/v1?label=A
+00000520: 6666 696c 6961 7465 206c 696e 6b26 6d65  ffiliate link&me
+00000530: 7373 6167 653d 2545 3225 3944 2541 3426  ssage=%E2%9D%A4&
+00000540: 636f 6c6f 723d 2532 3366 6538 6538 3622  color=%23fe8e86"
+00000550: 2061 6c74 3d22 4166 6669 6c69 6174 6520   alt="Affiliate 
+00000560: 6c69 6e6b 223e 3c2f 613e 0a20 203c 6120  link"></a>.  <a 
+00000570: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00000580: 7069 2e6f 7267 2f70 726f 6a65 6374 2f72  pi.org/project/r
+00000590: 656f 6c69 6e6b 2d61 696f 223e 3c69 6d67  eolink-aio"><img
+000005a0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+000005b0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+000005c0: 692f 646d 2f72 656f 6c69 6e6b 2d61 696f  i/dm/reolink-aio
+000005d0: 223e 3c2f 613e 0a20 203c 6120 6872 6566  "></a>.  <a href
+000005e0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+000005f0: 2e63 6f6d 2f73 7461 726b 696c 6c65 724f  .com/starkillerO
+00000600: 472f 7265 6f6c 696e 6b5f 6169 6f2f 7265  G/reolink_aio/re
+00000610: 6c65 6173 6573 223e 3c69 6d67 2073 7263  leases"><img src
+00000620: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000630: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000640: 762f 7265 6c65 6173 652f 5374 6172 6b69  v/release/Starki
+00000650: 6c6c 6572 4f47 2f72 656f 6c69 6e6b 5f61  llerOG/reolink_a
+00000660: 696f 3f64 6973 706c 6179 5f6e 616d 653d  io?display_name=
+00000670: 7461 6726 696e 636c 7564 655f 7072 6572  tag&include_prer
+00000680: 656c 6561 7365 7326 736f 7274 3d73 656d  eleases&sort=sem
+00000690: 7665 7222 2061 6c74 3d22 4375 7272 656e  ver" alt="Curren
+000006a0: 7420 7665 7273 696f 6e22 3e3c 2f61 3e0a  t version"></a>.
+000006b0: 3c2f 703e 0a0a 5468 6520 6072 656f 6c69  </p>..The `reoli
+000006c0: 6e6b 5f61 696f 6020 5079 7468 6f6e 2070  nk_aio` Python p
+000006d0: 6163 6b61 6765 2061 6c6c 6f77 7320 796f  ackage allows yo
+000006e0: 7520 746f 2069 6e74 6567 7261 7465 2079  u to integrate y
+000006f0: 6f75 7220 5b52 656f 6c69 6e6b 5d28 6874  our [Reolink](ht
+00000700: 7470 733a 2f2f 7777 772e 7265 6f6c 696e  tps://www.reolin
+00000710: 6b2e 636f 6d2f 2920 6465 7669 6365 7320  k.com/) devices 
+00000720: 284e 5652 2f63 616d 6572 6173 2920 696e  (NVR/cameras) in
+00000730: 2079 6f75 7220 6170 706c 6963 6174 696f   your applicatio
+00000740: 6e2e 0a0a 2323 2320 4465 7363 7269 7074  n...### Descript
+00000750: 696f 6e0a 0a54 6869 7320 6973 2061 2070  ion..This is a p
+00000760: 6163 6b61 6765 2069 6d70 6c65 6d65 6e74  ackage implement
+00000770: 696e 6720 5265 6f6c 696e 6b20 4950 204e  ing Reolink IP N
+00000780: 5652 2061 6e64 2063 616d 6572 6120 4150  VR and camera AP
+00000790: 492e 2041 6c73 6f20 6974 e280 9973 2070  I. Also it...s p
+000007a0: 726f 7669 6469 6e67 2061 2077 6179 2074  roviding a way t
+000007b0: 6f20 7375 6273 6372 6962 6520 746f 2052  o subscribe to R
+000007c0: 656f 6c69 6e6b 204f 4e56 4946 2053 574e  eolink ONVIF SWN
+000007d0: 2065 7665 6e74 732c 2073 6f20 7468 6174   events, so that
+000007e0: 2072 6561 6c2d 7469 6d65 2065 7665 6e74   real-time event
+000007f0: 7320 6361 6e20 6265 2072 6563 6569 7665  s can be receive
+00000800: 6420 6f6e 2061 2077 6562 686f 6f6b 2e0a  d on a webhook..
+00000810: 0a23 2323 2053 686f 7720 796f 7572 2061  .### Show your a
+00000820: 7070 7265 6369 6174 696f 6e0a 0a49 6620  ppreciation..If 
+00000830: 796f 7520 6170 7072 6563 6961 7465 2074  you appreciate t
+00000840: 6865 2072 656f 6c69 6e6b 2069 6e74 6567  he reolink integ
+00000850: 7261 7469 6f6e 2061 6e64 2077 616e 7420  ration and want 
+00000860: 746f 2073 7570 706f 7274 2069 7473 2064  to support its d
+00000870: 6576 656c 6f70 6d65 6e74 2c20 706c 6561  evelopment, plea
+00000880: 7365 2063 6f6e 7369 6465 7220 5b73 706f  se consider [spo
+00000890: 6e73 6572 696e 675d 2868 7474 7073 3a2f  nsering](https:/
+000008a0: 2f67 6974 6875 622e 636f 6d2f 7370 6f6e  /github.com/spon
+000008b0: 736f 7273 2f73 7461 726b 696c 6c65 724f  sors/starkillerO
+000008c0: 4729 2074 6865 2075 7073 7472 6561 6d20  G) the upstream 
+000008d0: 6c69 6272 6172 7920 6f72 2070 7572 6368  library or purch
+000008e0: 6173 6520 5265 6f6c 696e 6b20 7072 6f64  ase Reolink prod
+000008f0: 7563 7473 2074 6872 6f75 6768 205b 7468  ucts through [th
+00000900: 6973 2061 6666 696c 6961 7465 206c 696e  is affiliate lin
+00000910: 6b5d 2868 7474 7073 3a2f 2f72 656f 6c69  k](https://reoli
+00000920: 6e6b 2e70 7866 2e69 6f2f 7134 3451 5771  nk.pxf.io/q44QWq
+00000930: 292e 0a0a 2323 2320 5072 6572 6571 7569  )...### Prerequi
+00000940: 7369 7465 730a 0a2d 2050 7974 686f 6e20  sites..- Python 
+00000950: 332e 390a 0a23 2323 2049 6e73 7461 6c6c  3.9..### Install
+00000960: 6174 696f 6e0a 0a60 6060 0a70 6970 3320  ation..```.pip3 
+00000970: 696e 7374 616c 6c20 7265 6f6c 696e 6b2d  install reolink-
+00000980: 6169 6f0a 6060 600a 0a6f 7220 6d61 6e75  aio.```..or manu
+00000990: 616c 6c79 3a0a 6060 6060 0a67 6974 2063  ally:.````.git c
+000009a0: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+000009b0: 6875 622e 636f 6d2f 5374 6172 6b69 6c6c  hub.com/Starkill
+000009c0: 6572 4f47 2f72 656f 6c69 6e6b 5f61 696f  erOG/reolink_aio
+000009d0: 0a63 6420 7265 6f6c 696e 6b5f 6169 6f2f  .cd reolink_aio/
+000009e0: 0a70 6970 3320 696e 7374 616c 6c20 2e0a  .pip3 install ..
+000009f0: 6060 6060 0a0a 2323 2320 5573 6167 650a  ````..### Usage.
+00000a00: 0a60 6060 600a 6672 6f6d 2072 656f 6c69  .````.from reoli
+00000a10: 6e6b 5f61 696f 2e61 7069 2069 6d70 6f72  nk_aio.api impor
+00000a20: 7420 486f 7374 0a69 6d70 6f72 7420 6173  t Host.import as
+00000a30: 796e 6369 6f0a 0a23 2043 7265 6174 6520  yncio..# Create 
+00000a40: 6120 686f 7374 2d6f 626a 6563 7420 2872  a host-object (r
+00000a50: 6570 7265 7365 6e74 696e 6720 6569 7468  epresenting eith
+00000a60: 6572 2061 2063 616d 6572 612c 206f 7220  er a camera, or 
+00000a70: 4e56 5220 7769 7468 2073 6576 6572 616c  NVR with several
+00000a80: 2063 6861 6e6e 656c 7329 0a68 6f73 7420   channels).host 
+00000a90: 3d20 486f 7374 2827 3139 322e 3136 382e  = Host('192.168.
+00000aa0: 312e 3130 272c 2038 302c 2027 7573 6572  1.10', 80, 'user
+00000ab0: 272c 2027 6d79 7061 7373 776f 7264 2729  ', 'mypassword')
+00000ac0: 0a0a 2320 4f62 7461 696e 2f63 6163 6865  ..# Obtain/cache
+00000ad0: 204e 5652 206f 7220 6361 6d65 7261 2073   NVR or camera s
+00000ae0: 6574 7469 6e67 7320 616e 6420 6361 7061  ettings and capa
+00000af0: 6269 6c69 7469 6573 2c20 6c69 6b65 206d  bilities, like m
+00000b00: 6f64 656c 206e 616d 652c 2070 6f72 7473  odel name, ports
+00000b10: 2c20 4844 4420 7369 7a65 2c20 6574 633a  , HDD size, etc:
+00000b20: 0a61 7761 6974 2068 6f73 742e 6765 745f  .await host.get_
+00000b30: 686f 7374 5f64 6174 6128 290a 0a23 2047  host_data()..# G
+00000b40: 6574 2074 6865 2073 7562 7363 7269 6274  et the subscribt
+00000b50: 696f 6e20 706f 7274 2061 6e64 2068 6f73  ion port and hos
+00000b60: 742d 6465 7669 6365 206e 616d 653a 0a73  t-device name:.s
+00000b70: 7562 7363 7269 6274 696f 6e5f 706f 7274  ubscribtion_port
+00000b80: 203d 2020 686f 7374 2e6f 6e76 6966 5f70   =  host.onvif_p
+00000b90: 6f72 740a 6e61 6d65 203d 2068 6f73 742e  ort.name = host.
+00000ba0: 6e76 725f 6e61 6d65 0a0a 2320 4f62 7461  nvr_name..# Obta
+00000bb0: 696e 2f63 6163 6865 2073 7461 7465 7320  in/cache states 
+00000bc0: 6f66 2066 6561 7475 7265 733a 0a61 7761  of features:.awa
+00000bd0: 6974 2068 6f73 742e 6765 745f 7374 6174  it host.get_stat
+00000be0: 6573 2829 0a0a 2320 5072 696e 7420 736f  es()..# Print so
+00000bf0: 6d65 2073 7461 7465 2076 616c 7565 206f  me state value o
+00000c00: 6e20 7468 6520 6368 616e 6e65 6c20 7769  n the channel wi
+00000c10: 7468 2069 6e64 6578 2030 3a0a 7072 696e  th index 0:.prin
+00000c20: 7428 686f 7374 2e69 725f 656e 6162 6c65  t(host.ir_enable
+00000c30: 6428 3029 290a 0a23 2045 6e61 626c 6520  d(0))..# Enable 
+00000c40: 7468 6520 696e 6672 6172 6564 206c 6967  the infrared lig
+00000c50: 6874 7320 6f6e 2074 6865 2063 6861 6e6e  hts on the chann
+00000c60: 656c 2077 6974 6820 696e 6465 7820 313a  el with index 1:
+00000c70: 0a61 7761 6974 2068 6f73 742e 7365 745f  .await host.set_
+00000c80: 6972 5f6c 6967 6874 7328 312c 2054 7275  ir_lights(1, Tru
+00000c90: 6529 0a0a 2320 456e 6162 6c65 2074 6865  e)..# Enable the
+00000ca0: 2073 706f 746c 6967 6874 206f 6e20 7468   spotlight on th
+00000cb0: 6520 6368 616e 6e65 6c20 7769 7468 2069  e channel with i
+00000cc0: 6e64 6578 2031 3a0a 6177 6169 7420 686f  ndex 1:.await ho
+00000cd0: 7374 2e73 6574 5f73 706f 746c 6967 6874  st.set_spotlight
+00000ce0: 2831 2c20 5472 7565 290a 0a23 2045 6e61  (1, True)..# Ena
+00000cf0: 626c 6520 7468 6520 7369 7265 6e20 6f6e  ble the siren on
+00000d00: 2074 6865 2063 6861 6e6e 656c 2077 6974   the channel wit
+00000d10: 6820 696e 6465 7820 303a 0a61 7761 6974  h index 0:.await
+00000d20: 2068 6f73 742e 7365 745f 7369 7265 6e28   host.set_siren(
+00000d30: 302c 2054 7275 6529 0a0a 2320 4e6f 7720  0, True)..# Now 
+00000d40: 7375 6273 6372 6962 6520 746f 2065 7665  subscribe to eve
+00000d50: 6e74 732c 2073 7570 706f 7365 206f 7572  nts, suppose our
+00000d60: 2077 6562 686f 6f6b 2075 726c 2069 7320   webhook url is 
+00000d70: 6874 7470 3a2f 2f31 3932 2e31 3638 2e31  http://192.168.1
+00000d80: 2e31 312f 7765 6268 6f6f 6b31 3233 0a61  .11/webhook123.a
+00000d90: 7761 6974 2068 6f73 742e 7375 6273 6372  wait host.subscr
+00000da0: 6962 6528 2768 7474 703a 2f2f 3139 322e  ibe('http://192.
+00000db0: 3136 382e 312e 3131 2f77 6562 686f 6f6b  168.1.11/webhook
+00000dc0: 3132 3327 290a 0a23 2041 6674 6572 2073  123')..# After s
+00000dd0: 6f6d 6520 6d69 6e75 7465 7320 6368 6563  ome minutes chec
+00000de0: 6b20 7468 6520 7265 6e65 7720 7469 6d65  k the renew time
+00000df0: 7220 286b 6565 7020 7468 6520 6576 656e  r (keep the even
+00000e00: 7469 6e67 2061 6c69 7665 293a 0a69 6620  ting alive):.if 
+00000e10: 2868 6f73 742e 7265 6e65 7754 696d 6572  (host.renewTimer
+00000e20: 203c 3d20 3130 3029 3a0a 2020 2020 6177   <= 100):.    aw
+00000e30: 6169 7420 686f 7374 2e72 656e 6577 2829  ait host.renew()
+00000e40: 0a0a 2320 4c6f 676f 7574 2061 6e64 2064  ..# Logout and d
+00000e50: 6973 636f 6e6e 6563 740a 6177 6169 7420  isconnect.await 
+00000e60: 686f 7374 2e64 6973 636f 6e6e 6563 7428  host.disconnect(
+00000e70: 290a 6060 6060 0a0a 2323 2320 4578 616d  ).````..### Exam
+00000e80: 706c 650a 0a54 6869 7320 6973 2061 6e20  ple..This is an 
+00000e90: 6578 616d 706c 6520 6f66 2074 6865 2075  example of the u
+00000ea0: 7361 6765 206f 6620 7468 6520 4150 492e  sage of the API.
+00000eb0: 2049 6e20 7468 6973 2063 6173 6520 7765   In this case we
+00000ec0: 2077 616e 7420 746f 2072 6574 7269 7665   want to retrive
+00000ed0: 2061 6e64 2070 7269 6e74 2074 6865 204d   and print the M
+00000ee0: 6163 2041 6464 7265 7373 206f 6620 7468  ac Address of th
+00000ef0: 6520 4e56 522e 0a60 6060 600a 6672 6f6d  e NVR..````.from
+00000f00: 2072 656f 6c69 6e6b 5f61 696f 2e61 7069   reolink_aio.api
+00000f10: 2069 6d70 6f72 7420 486f 7374 0a69 6d70   import Host.imp
+00000f20: 6f72 7420 6173 796e 6369 6f0a 0a61 7379  ort asyncio..asy
+00000f30: 6e63 2064 6566 2070 7269 6e74 5f6d 6163  nc def print_mac
+00000f40: 5f61 6464 7265 7373 2829 3a0a 2020 2020  _address():.    
+00000f50: 2320 696e 6974 6961 6c69 7a65 2074 6865  # initialize the
+00000f60: 2068 6f73 740a 2020 2020 686f 7374 203d   host.    host =
+00000f70: 2048 6f73 7428 2731 3932 2e31 3638 2e31   Host('192.168.1
+00000f80: 2e31 3039 272c 2761 646d 696e 272c 2027  .109','admin', '
+00000f90: 6164 6d69 6e31 3233 3427 2c20 706f 7274  admin1234', port
+00000fa0: 3d38 3029 0a20 2020 2023 2063 6f6e 6e65  =80).    # conne
+00000fb0: 6374 2061 6e64 206f 6274 6169 6e2f 6361  ct and obtain/ca
+00000fc0: 6368 6520 6465 7669 6365 2073 6574 7469  che device setti
+00000fd0: 6e67 7320 616e 6420 6361 7061 6269 6c69  ngs and capabili
+00000fe0: 7469 6573 0a20 2020 2061 7761 6974 2068  ties.    await h
+00000ff0: 6f73 742e 6765 745f 686f 7374 5f64 6174  ost.get_host_dat
+00001000: 6128 290a 2020 2020 2320 6368 6563 6b20  a().    # check 
+00001010: 6966 2069 7420 6973 2061 2063 616d 6572  if it is a camer
+00001020: 6120 6f72 2061 6e20 4e56 520a 2020 2020  a or an NVR.    
+00001030: 7072 696e 7428 2249 7420 6973 2061 6e20  print("It is an 
+00001040: 4e56 523a 2025 732c 206e 756d 6265 7220  NVR: %s, number 
+00001050: 6f66 2063 6861 6e6e 656c 733a 2025 7322  of channels: %s"
+00001060: 2c20 686f 7374 2e69 735f 6e76 722c 2068  , host.is_nvr, h
+00001070: 6f73 742e 6e75 6d5f 6368 616e 6e65 6c73  ost.num_channels
+00001080: 290a 2020 2020 2320 7072 696e 7420 6d61  ).    # print ma
+00001090: 6320 6164 6472 6573 730a 2020 2020 7072  c address.    pr
+000010a0: 696e 7428 686f 7374 2e6d 6163 5f61 6464  int(host.mac_add
+000010b0: 7265 7373 290a 2020 2020 2320 636c 6f73  ress).    # clos
+000010c0: 6520 7468 6520 6465 7669 6365 2063 6f6e  e the device con
+000010d0: 6e65 6374 696f 6e0a 2020 2020 6177 6169  nection.    awai
+000010e0: 7420 686f 7374 2e6c 6f67 6f75 7428 290a  t host.logout().
+000010f0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
+00001100: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
+00001110: 6173 796e 6369 6f2e 7275 6e28 7072 696e  asyncio.run(prin
+00001120: 745f 6d61 635f 6164 6472 6573 7328 2929  t_mac_address())
+00001130: 0a60 6060 600a 0a23 2323 2041 636b 6e6f  .````..### Ackno
+00001140: 776c 6564 676d 656e 740a 5468 6973 206c  wledgment.This l
+00001150: 6962 7261 7279 2069 7320 6261 7365 6420  ibrary is based 
+00001160: 6f6e 2074 6865 2077 6f72 6b20 6f66 3a0a  on the work of:.
+00001170: 2d20 6677 6573 7465 6e62 6572 673a 2068  - fwestenberg: h
+00001180: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001190: 6d2f 6677 6573 7465 6e62 6572 672f 7265  m/fwestenberg/re
+000011a0: 6f6c 696e 6b5f 6465 760a 2d20 4a69 6d53  olink_dev.- JimS
+000011b0: 7461 723a 2068 7474 7073 3a2f 2f67 6974  tar: https://git
+000011c0: 6875 622e 636f 6d2f 4a69 6d53 7461 722f  hub.com/JimStar/
+000011d0: 7265 6f6c 696e 6b5f 6970 0a              reolink_ip.
```

### Comparing `reolink_aio-0.5.9/README.md` & `reolink_aio-0.6.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,24 +3,29 @@
   <br>
   <i>Reolink NVR/cameras API package</i>
   <br>
 </h2>
 
 <p align="center">
   <a href="https://github.com/sponsors/starkillerOG"><img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86" alt="Sponsor"></a>
+  <a href="https://reolink.pxf.io/q44QWq"><img src="https://img.shields.io/static/v1?label=Affiliate link&message=%E2%9D%A4&color=%23fe8e86" alt="Affiliate link"></a>
   <a href="https://pypi.org/project/reolink-aio"><img src="https://img.shields.io/pypi/dm/reolink-aio"></a>
   <a href="https://github.com/starkillerOG/reolink_aio/releases"><img src="https://img.shields.io/github/v/release/StarkillerOG/reolink_aio?display_name=tag&include_prereleases&sort=semver" alt="Current version"></a>
 </p>
 
 The `reolink_aio` Python package allows you to integrate your [Reolink](https://www.reolink.com/) devices (NVR/cameras) in your application.
 
 ### Description
 
 This is a package implementing Reolink IP NVR and camera API. Also it’s providing a way to subscribe to Reolink ONVIF SWN events, so that real-time events can be received on a webhook.
 
+### Show your appreciation
+
+If you appreciate the reolink integration and want to support its development, please consider [sponsering](https://github.com/sponsors/starkillerOG) the upstream library or purchase Reolink products through [this affiliate link](https://reolink.pxf.io/q44QWq).
+
 ### Prerequisites
 
 - Python 3.9
 
 ### Installation
 
 ```
```

### Comparing `reolink_aio-0.5.9/reolink_aio/api.py` & `reolink_aio-0.6.0/reolink_aio/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import base64
 import hashlib
 import json
 import logging
 import ssl
 import traceback
 import uuid
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, tzinfo
 from os.path import basename
 from typing import Any, Literal, Optional, overload
 from urllib import parse
 from xml.etree import ElementTree as XML
 from statistics import mean
 
 import aiohttp
@@ -27,23 +27,26 @@
     InvalidParameterError,
     LoginError,
     NoDataError,
     NotSupportedError,
     ReolinkError,
     SubscriptionError,
     UnexpectedDataError,
+    ReolinkConnectionError,
+    ReolinkTimeoutError,
 )
-from .software_version import SoftwareVersion, MINIMUM_FIRMWARE
-from .typings import reolink_json
+from .software_version import SoftwareVersion, NewSoftwareVersion, MINIMUM_FIRMWARE
+from .utils import datetime_to_reolink_time, reolink_time_to_datetime
 
 MANUFACTURER = "Reolink"
 DEFAULT_STREAM = "sub"
 DEFAULT_PROTOCOL = "rtmp"
 DEFAULT_TIMEOUT = 60
 RETRY_ATTEMPTS = 3
+MAX_CHUNK_ITEMS = 40
 DEFAULT_RTMP_AUTH_METHOD = "PASSWORD"
 SUBSCRIPTION_TERMINATION_TIME = 15
 
 MOTION_DETECTION_TYPE = "motion"
 FACE_DETECTION_TYPE = "face"
 PERSON_DETECTION_TYPE = "person"
 VEHICLE_DETECTION_TYPE = "vehicle"
@@ -57,22 +60,18 @@
 SSL_CONTEXT.set_ciphers("DEFAULT")
 SSL_CONTEXT.check_hostname = False
 SSL_CONTEXT.verify_mode = ssl.CERT_NONE
 
 DUAL_LENS_MODELS: set[str] = {
     "Reolink Duo PoE",
     "Reolink Duo WiFi",
-    "Reolink Duo 2 PoE",
-    "Reolink Duo 2 WiFi",
-    "Reolink Duo Floodlight PoE",
-    "Reolink Duo Floodlight WiFi",
     "Reolink TrackMix PoE",
     "Reolink TrackMix WiFi",
     "RLC-81MA",
-}
+}  # with 2 streaming channels
 
 
 ##########################################################################################################################################################
 # API class
 ##########################################################################################################################################################
 class Host:
     """Reolink network API class."""
@@ -129,14 +128,16 @@
         self._nvr_name: str = ""
         self._nvr_serial: Optional[str] = None
         self._nvr_model: Optional[str] = None
         self._nvr_num_channels: int = 0
         self._nvr_hw_version: Optional[str] = None
         self._nvr_sw_version: Optional[str] = None
         self._nvr_sw_version_object: Optional[SoftwareVersion] = None
+        self._nvr_sw_hardware_id: Optional[int] = None
+        self._nvr_sw_model_id: Optional[int] = None
 
         ##############################################################################
         # Channels of cameras, used in this NVR ([0] for a directly connected camera)
         self._GetChannelStatus_present: bool = False
         self._GetChannelStatus_has_name: bool = False
         self._channels: list[int] = []
         self._stream_channels: list[int] = []
@@ -168,27 +169,29 @@
         self._local_link: Optional[dict] = None
         self._users: Optional[dict] = None
 
         ##############################################################################
         # Saved settings response-blocks
         # Host-level
         self._time_settings: Optional[dict] = None
+        self._host_time_difference: float = 0
         self._ntp_settings: Optional[dict] = None
         self._netport_settings: Optional[dict] = None
         # Camera-level
         self._zoom_focus_settings: dict[int, dict] = {}
         self._zoom_focus_range: dict[int, dict] = {}
         self._auto_focus_settings: dict[int, dict] = {}
         self._isp_settings: dict[int, dict] = {}
         self._ftp_settings: dict[int, dict] = {}
         self._osd_settings: dict[int, dict] = {}
         self._push_settings: dict[int, dict] = {}
         self._enc_settings: dict[int, dict] = {}
         self._ptz_presets_settings: dict[int, dict] = {}
         self._ptz_guard_settings: dict[int, dict] = {}
+        self._ptz_position: dict[int, dict] = {}
         self._email_settings: dict[int, dict] = {}
         self._ir_settings: dict[int, dict] = {}
         self._status_led_settings: dict[int, dict] = {}
         self._whiteled_settings: dict[int, dict] = {}
         self._recording_settings: dict[int, dict] = {}
         self._md_alarm_settings: dict[int, dict] = {}
         self._ai_alarm_settings: dict[int, dict] = {}
@@ -285,14 +288,21 @@
         return self._nvr_name
 
     @property
     def sw_version(self) -> Optional[str]:
         return self._nvr_sw_version
 
     @property
+    def sw_version_object(self) -> SoftwareVersion:
+        if self._nvr_sw_version_object is None:
+            return SoftwareVersion(None)
+
+        return self._nvr_sw_version_object
+
+    @property
     def sw_version_required(self) -> SoftwareVersion:
         """Return the minimum required firmware version for proper operation of this library"""
         if self.model is None or self.hardware_version is None:
             return SoftwareVersion(None)
 
         return SoftwareVersion(MINIMUM_FIRMWARE.get(self.model, {}).get(self.hardware_version))
 
@@ -374,14 +384,48 @@
     def is_admin(self) -> bool:
         """
         Check if the user has admin authorisation.
         Only admin users can change camera settings, not everything will work if account is not admin
         """
         return self.user_level == "admin"
 
+    def timezone(self) -> Optional[tzinfo]:
+        """Get the timezone of the device
+
+        Returns None if there is no current time information
+        """
+        if self._time_settings is None:
+            return None
+        return typings.Reolink_timezone(self._time_settings)
+
+    def time(self) -> Optional[datetime]:
+        """Get the approximate "current" time of the device using existing data.
+
+        Returns None if there is no current time information.
+
+        When None is returned async_get_time can be used to request the current camera time
+        """
+        if self._time_settings is None:
+            return None
+        # the _host_time_difference is basically the diff in "localtime" between the system and the device
+        # so we will add that then set the tzinfo to our timezone rule so the resulting time
+        # can be converted to other timezones correctly
+        return (datetime.now() + timedelta(seconds=self._host_time_difference)).replace(tzinfo=self.timezone())
+
+    async def async_get_time(self) -> datetime:
+        """Get the current time of the device
+
+        The preferred method is to check get_time first, and if it returns none; call this, to save
+        an async round trip to the device.
+        """
+        await self.get_state("GetTime")
+        if self._time_settings is None:
+            raise NotSupportedError(f"get_time: failed to retrieve current time settings from {self._host}:{self._port}")
+        return reolink_time_to_datetime(self._time_settings["Time"]).replace(tzinfo=self.timezone())
+
     ##############################################################################
     # Channel-level getters/setters
 
     def camera_name(self, channel: int | None) -> Optional[str]:
         if channel is None:
             return self.nvr_name
 
@@ -400,18 +444,14 @@
             return "Unknown"
         return self._channel_models[channel]
 
     def is_doorbell(self, channel: int) -> bool:
         """Wether or not the camera is a doorbell"""
         return channel in self._is_doorbell and self._is_doorbell[channel]
 
-    def is_doorbell_enabled(self, channel: int) -> bool:
-        """Needs to be depricated"""
-        return self.is_doorbell(channel)
-
     def motion_detected(self, channel: int) -> bool:
         """Return the motion detection state (polled)."""
         return channel in self._motion_detection_states and self._motion_detection_states[channel]
 
     def ai_detected(self, channel: int, object_type: str) -> bool:
         """Return the AI object detection state (polled)."""
         if channel not in self._ai_detection_states or self._ai_detection_states[channel] is None:
@@ -490,71 +530,71 @@
 
             return all(self._ftp_settings[ch]["Ftp"]["schedule"]["enable"] == 1 for ch in self._channels)
 
         if channel not in self._ftp_settings:
             return False
 
         if self.api_version("GetFtp") >= 1:
-            return self._ftp_settings[channel]["Ftp"]["enable"] == 1
+            return self._ftp_settings[channel]["Ftp"]["scheduleEnable"] == 1
 
         return self._ftp_settings[channel]["Ftp"]["schedule"]["enable"] == 1
 
     def email_enabled(self, channel: int | None = None) -> bool:
         if channel is None:
             if self.api_version("GetEmail") >= 1:
                 return all(self._email_settings[ch]["Email"]["enable"] == 1 for ch in self._channels)
 
             return all(self._email_settings[ch]["Email"]["schedule"]["enable"] == 1 for ch in self._channels)
 
         if channel not in self._email_settings:
             return False
 
         if self.api_version("GetEmail") >= 1:
-            return self._email_settings[channel]["Email"]["enable"] == 1
+            return self._email_settings[channel]["Email"]["scheduleEnable"] == 1
 
         return self._email_settings[channel]["Email"]["schedule"]["enable"] == 1
 
     def push_enabled(self, channel: int | None = None) -> bool:
         if channel is None:
             if self.api_version("GetPush") >= 1:
                 return all(self._push_settings[ch]["Push"]["enable"] == 1 for ch in self._channels)
 
             return all(self._push_settings[ch]["Push"]["schedule"]["enable"] == 1 for ch in self._channels)
 
         if channel not in self._push_settings:
             return False
 
         if self.api_version("GetPush") >= 1:
-            return self._push_settings[channel]["Push"]["enable"] == 1
+            return self._push_settings[channel]["Push"]["scheduleEnable"] == 1
 
         return self._push_settings[channel]["Push"]["schedule"]["enable"] == 1
 
     def recording_enabled(self, channel: int | None = None) -> bool:
         if channel is None:
             if self.api_version("GetRec") >= 1:
                 return all(self._recording_settings[ch]["Rec"]["enable"] == 1 for ch in self._channels)
 
             return all(self._recording_settings[ch]["Rec"]["schedule"]["enable"] == 1 for ch in self._channels)
 
         if channel not in self._recording_settings:
             return False
 
         if self.api_version("GetRec") >= 1:
-            return self._recording_settings[channel]["Rec"]["enable"] == 1
+            return self._recording_settings[channel]["Rec"]["scheduleEnable"] == 1
 
         return self._recording_settings[channel]["Rec"]["schedule"]["enable"] == 1
 
     def buzzer_enabled(self, channel: int | None = None) -> bool:
         if channel is None:
             return all(self._buzzer_settings[ch]["Buzzer"]["enable"] == 1 for ch in self._channels)
 
         if channel not in self._buzzer_settings:
             return False
 
-        return self._buzzer_settings[channel]["Buzzer"]["enable"] == 1
+        return self._buzzer_settings[channel]["Buzzer"]["scheduleEnable"] == 1
 
     def whiteled_state(self, channel: int) -> bool:
         return channel in self._whiteled_settings and self._whiteled_settings[channel]["WhiteLed"]["state"] == 1
 
     def whiteled_mode(self, channel: int) -> Optional[int]:
         if channel not in self._whiteled_settings:
             return None
@@ -683,26 +723,33 @@
             await self._login_try_ports()
             return  # succes
 
         if self._token is not None and self._lease_time is not None and self._lease_time > (datetime.now() + timedelta(seconds=300)):
             return  # succes
 
         await self._login_mutex.acquire()
-
         try:
+            if self._token is not None and self._lease_time is not None and self._lease_time > (datetime.now() + timedelta(seconds=300)):
+                _LOGGER.debug(
+                    "Host %s:%s, after login mutex aquired, login already completed by another coroutine",
+                    self._host,
+                    self._port,
+                )
+                return  # succes, in case multiple async coroutine are waiting on login_mutex.acquire
+
             await self.logout(login_mutex_owned=True)  # Ensure there would be no "max session" error
 
             _LOGGER.debug(
                 "Host %s:%s, trying to login with user %s...",
                 self._host,
                 self._port,
                 self._username,
             )
 
-            body: reolink_json = [
+            body: typings.reolink_json = [
                 {
                     "cmd": "Login",
                     "action": 0,
                     "param": {
                         "User": {
                             "userName": self._username,
                             "password": self._password,
@@ -712,15 +759,15 @@
             ]
             param = {"cmd": "Login"}
 
             try:
                 json_data = await self.send(body, param, expected_response_type="json")
             except ApiError as err:
                 raise LoginError(f"API error during login of host {self._host}:{self._port}: {str(err)}") from err
-            except aiohttp.ClientConnectorError as err:
+            except ReolinkConnectionError as err:
                 raise LoginError(f"Client connector error during login of host {self._host}:{self._port}: {str(err)}") from err
             except InvalidContentTypeError as err:
                 raise LoginError(f"Invalid content error during login of host {self._host}:{self._port}: {str(err)}") from err
             except NoDataError as err:
                 raise LoginError(f"Error receiving Reolink login response of host {self._host}:{self._port}") from err
 
             _LOGGER.debug("Got login response from %s:%s: %s", self._host, self._port, json_data)
@@ -803,14 +850,18 @@
         self._token = None
         self._lease_time = None
 
     def construct_capabilities(self, warnings=True) -> None:
         """Construct the capabilities list of the NVR/camera."""
         # Host capabilities
         self._capabilities["Host"] = []
+        if self.sw_version_object.date > datetime(year=2021, month=6, day=1):
+            # Check if this camera publishes its inital state upon ONVIF subscription
+            self._capabilities["Host"].append("initial_ONVIF_state")
+
         if self._ftp_settings:
             self._capabilities["Host"].append("ftp")
 
         if self._push_settings:
             self._capabilities["Host"].append("push")
 
         if self._recording_settings:
@@ -873,14 +924,15 @@
             if (self.api_version("supportAudioFileList", channel) > 0 and self.api_version("supportAutoReply", channel) > 0) or (
                 not self.is_nvr and self.api_version("supportAudioFileList") > 0 and self.api_version("supportAutoReply") > 0
             ):
                 self._capabilities[channel].append("quick_reply")
 
             if channel in self._audio_alarm_settings:
                 self._capabilities[channel].append("siren")
+                self._capabilities[channel].append("siren_play")  # if self.api_version("supportAoAdjust", channel) > 0
 
             if self.audio_record(channel) is not None:
                 self._capabilities[channel].append("audio")
 
             ptz_ver = self.api_version("ptzType", channel)
             if ptz_ver != 0:
                 self._capabilities[channel].append("ptz")
@@ -893,19 +945,24 @@
                             _LOGGER.warning("Camera %s reported to support zoom, but zoom range not available", self.camera_name(channel))
                     else:
                         self._capabilities[channel].append("zoom")
                         self._capabilities[channel].append("focus")
                         if self.api_version("disableAutoFocus", channel) > 0:
                             self._capabilities[channel].append("auto_focus")
                 if ptz_ver in [2, 3, 5]:
+                    self._capabilities[channel].append("tilt")
+                if ptz_ver in [2, 3, 5, 7]:
                     self._capabilities[channel].append("pan_tilt")
+                    self._capabilities[channel].append("pan")
                     if self.api_version("supportPtzCalibration", channel) > 0 or self.api_version("supportPtzCheck", channel) > 0:
                         self._capabilities[channel].append("ptz_callibrate")
                     if self.api_version("GetPtzGuard", channel) > 0:
                         self._capabilities[channel].append("ptz_guard")
+                    if self.api_version("GetPtzCurPos", channel) > 0:
+                        self._capabilities[channel].append("ptz_position")
                 if ptz_ver in [2, 3]:
                     self._capabilities[channel].append("ptz_speed")
                 if channel in self._ptz_presets and len(self._ptz_presets[channel]) != 0:
                     self._capabilities[channel].append("ptz_presets")
 
             if self.api_version("supportDigitalZoom", channel) > 0 and "zoom" not in self._capabilities[channel]:
                 self._capabilities[channel].append("zoom_basic")
@@ -936,14 +993,25 @@
 
             if self.api_version("supportAiSensitivity", channel) > 0:
                 self._capabilities[channel].append("ai_sensitivity")
 
             if channel in self._motion_detection_states:
                 self._capabilities[channel].append("motion_detection")
 
+            if self.api_version("ispHue", channel) > 0:
+                self._capabilities[channel].append("isp_hue")
+            if self.api_version("ispSatruation", channel) > 0:
+                self._capabilities[channel].append("isp_satruation")
+            if self.api_version("ispSharpen", channel) > 0:
+                self._capabilities[channel].append("isp_sharpen")
+            if self.api_version("ispContrast", channel) > 0:
+                self._capabilities[channel].append("isp_contrast")
+            if self.api_version("ispBright", channel) > 0:
+                self._capabilities[channel].append("isp_bright")
+
             if self.daynight_state(channel) is not None:
                 self._capabilities[channel].append("dayNight")
 
             if self.backlight_state(channel) is not None:
                 self._capabilities[channel].append("backLight")
 
     def supported(self, channel: int | None, capability: str) -> bool:
@@ -995,14 +1063,16 @@
                 ch_body = [{"cmd": "GetPtzPreset", "action": 0, "param": {"channel": channel}}]
             elif cmd == "GetAutoFocus":
                 ch_body = [{"cmd": "GetAutoFocus", "action": 0, "param": {"channel": channel}}]
             elif cmd == "GetZoomFocus":
                 ch_body = [{"cmd": "GetZoomFocus", "action": 0, "param": {"channel": channel}}]
             elif cmd == "GetPtzGuard":
                 ch_body = [{"cmd": "GetPtzGuard", "action": 0, "param": {"channel": channel}}]
+            elif cmd == "GetPtzCurPos":
+                ch_body = [{"cmd": "GetPtzCurPos", "action": 0, "param": {"PtzCurPos": {"channel": channel}}}]
             elif cmd == "GetAiCfg":
                 ch_body = [{"cmd": "GetAiCfg", "action": 0, "param": {"channel": channel}}]
             elif cmd == "GetPtzTraceSection":
                 ch_body = [{"cmd": "GetPtzTraceSection", "action": 0, "param": {"PtzTraceSection": {"channel": channel}}}]
             elif cmd == "GetAudioCfg":
                 ch_body = [{"cmd": "GetAudioCfg", "action": 0, "param": {"channel": channel}}]
             elif cmd == "GetAudioFileList":
@@ -1116,14 +1186,17 @@
 
             if self.supported(channel, "auto_focus"):
                 ch_body.append({"cmd": "GetAutoFocus", "action": 0, "param": {"channel": channel}})
 
             if self.supported(channel, "ptz_guard"):
                 ch_body.append({"cmd": "GetPtzGuard", "action": 0, "param": {"channel": channel}})
 
+            if self.supported(channel, "ptz_position"):
+                ch_body.append({"cmd": "GetPtzCurPos", "action": 0, "param": {"PtzCurPos": {"channel": channel}}})
+
             if self.supported(channel, "auto_track"):
                 ch_body.append({"cmd": "GetAiCfg", "action": 0, "param": {"channel": channel}})
 
             if self.supported(channel, "auto_track_limit"):
                 ch_body.append({"cmd": "GetPtzTraceSection", "action": 0, "param": {"PtzTraceSection": {"channel": channel}}})
 
             if self.supported(channel, "volume"):
@@ -1169,26 +1242,34 @@
             if self.supported(channel, "ai_sensitivity"):
                 for ai_type in self.ai_supported_types(channel):
                     ch_body.append({"cmd": "GetAiAlarm", "action": 0, "param": {"channel": channel, "ai_type": ai_type}})
 
             body.extend(ch_body)
             channels.extend([channel] * len(ch_body))
 
+        if not body:
+            _LOGGER.debug(
+                "Host %s:%s: get_states, no channels connected so skipping request.",
+                self._host,
+                self._port,
+            )
+            return
+
         try:
             json_data = await self.send(body, expected_response_type="json")
         except InvalidContentTypeError as err:
             raise InvalidContentTypeError(f"channel-state: {str(err)}") from err
         except NoDataError as err:
             raise NoDataError(f"Host: {self._host}:{self._port}: error obtaining channel-state response") from err
 
         self.map_channels_json_response(json_data, channels)
 
     async def get_host_data(self) -> None:
         """Fetch the host settings/capabilities."""
-        body: reolink_json = [
+        body: typings.reolink_json = [
             {"cmd": "Getchannelstatus"},
             {"cmd": "GetDevInfo", "action": 0, "param": {}},
             {"cmd": "GetLocalLink", "action": 0, "param": {}},
             {"cmd": "GetNetPort", "action": 0, "param": {}},
             {"cmd": "GetHddInfo", "action": 0, "param": {}},
             {"cmd": "GetUser", "action": 0, "param": {}},
             {"cmd": "GetNtp", "action": 0, "param": {}},
@@ -1202,18 +1283,18 @@
             raise InvalidContentTypeError(f"Get host-settings error: {str(err)}") from err
         except NoDataError as err:
             raise NoDataError(f"Host: {self._host}:{self._port}: returned no data when obtaining host-settings") from err
 
         self.map_host_json_response(json_data)
         self.construct_capabilities(warnings=False)
 
-        if self.model in DUAL_LENS_MODELS:
-            self._stream_channels = [0, 1]
-        elif not self.is_nvr and self.api_version("supportAutoTrackStream", 0) > 0:
+        if self.model in DUAL_LENS_MODELS or (not self.is_nvr and self.api_version("supportAutoTrackStream", 0) > 0):
             self._stream_channels = [0, 1]
+            self._nvr_num_channels = 1
+            self._channels = [0]
         else:
             self._stream_channels = self._channels
 
         body = []
         channels = []
         for channel in self._stream_channels:
             ch_body = [
@@ -1221,14 +1302,16 @@
                 {"cmd": "GetRtspUrl", "action": 0, "param": {"channel": channel}},
             ]
             body.extend(ch_body)
             channels.extend([channel] * len(ch_body))
 
         for channel in self._channels:
             ch_body = [
+                {"cmd": "GetChnTypeInfo", "action": 0, "param": {"channel": channel}},
+                {"cmd": "GetMdState", "action": 0, "param": {"channel": channel}},
                 {"cmd": "GetAiState", "action": 0, "param": {"channel": channel}},  # to capture AI capabilities
                 {"cmd": "GetEvents", "action": 0, "param": {"channel": channel}},
                 {"cmd": "GetWhiteLed", "action": 0, "param": {"channel": channel}},
                 {"cmd": "GetIsp", "action": 0, "param": {"channel": channel}},
                 {"cmd": "GetIrLights", "action": 0, "param": {"channel": channel}},
                 {"cmd": "GetAudioCfg", "action": 0, "param": {"channel": channel}},
             ]
@@ -1238,32 +1321,52 @@
                 ch_body.append({"cmd": "GetAudioFileList", "action": 0, "param": {"channel": channel}})
             # checking range
             if self.supported(channel, "zoom_basic"):
                 ch_body.append({"cmd": "GetZoomFocus", "action": 1, "param": {"channel": channel}})
             if self.supported(channel, "pan_tilt") and self.api_version("ptzPreset", channel) >= 1:
                 ch_body.append({"cmd": "GetPtzPreset", "action": 0, "param": {"channel": channel}})
                 ch_body.append({"cmd": "GetPtzGuard", "action": 0, "param": {"channel": channel}})
+                ch_body.append({"cmd": "GetPtzCurPos", "action": 0, "param": {"PtzCurPos": {"channel": channel}}})
             if self.supported(channel, "auto_track"):
                 ch_body.append({"cmd": "GetAiCfg", "action": 1, "param": {"channel": channel}})
             # checking API versions
             if self.api_version("scheduleVersion") >= 1:
                 ch_body.extend(
                     [
                         {"cmd": "GetEmailV20", "action": 0, "param": {"channel": channel}},
                         {"cmd": "GetPushV20", "action": 0, "param": {"channel": channel}},
                         {"cmd": "GetFtpV20", "action": 0, "param": {"channel": channel}},
                         {"cmd": "GetRecV20", "action": 0, "param": {"channel": channel}},
                         {"cmd": "GetAudioAlarmV20", "action": 0, "param": {"channel": channel}},
                         {"cmd": "GetMdAlarm", "action": 0, "param": {"channel": channel}},
                     ]
                 )
+            else:
+                ch_body.extend(
+                    [
+                        {"cmd": "GetEmail", "action": 0, "param": {"channel": channel}},
+                        {"cmd": "GetPush", "action": 0, "param": {"channel": channel}},
+                        {"cmd": "GetFtp", "action": 0, "param": {"channel": channel}},
+                        {"cmd": "GetRec", "action": 0, "param": {"channel": channel}},
+                        {"cmd": "GetAudioAlarm", "action": 0, "param": {"channel": channel}},
+                        {"cmd": "GetAlarm", "action": 0, "param": {"Alarm": {"channel": channel, "type": "md"}}},
+                    ]
+                )
 
             body.extend(ch_body)
             channels.extend([channel] * len(ch_body))
 
+        if not body:
+            _LOGGER.debug(
+                "Host %s:%s: get_host_data, no channels connected so skipping channel specific requests.",
+                self._host,
+                self._port,
+            )
+            return
+
         try:
             json_data = await self.send(body, expected_response_type="json")
         except InvalidContentTypeError as err:
             raise InvalidContentTypeError(f"Channel-settings: {str(err)}") from err
         except NoDataError as err:
             raise NoDataError(f"Host: {self._host}:{self._port}: returned no data when obtaining initial channel-settings") from err
 
@@ -1276,14 +1379,15 @@
                     return 1
             return 0
 
         self._api_version["GetEvents"] = check_command_exists("GetEvents")
         self._api_version["GetWhiteLed"] = check_command_exists("GetWhiteLed")
         self._api_version["GetAudioCfg"] = check_command_exists("GetAudioCfg")
         self._api_version["GetPtzGuard"] = check_command_exists("GetPtzGuard")
+        self._api_version["GetPtzCurPos"] = check_command_exists("GetPtzCurPos")
         if self.api_version("scheduleVersion") >= 1:
             self._api_version["GetEmail"] = check_command_exists("GetEmailV20")
             self._api_version["GetPush"] = check_command_exists("GetPushV20")
             self._api_version["GetFtp"] = check_command_exists("GetFtpV20")
             self._api_version["GetRec"] = check_command_exists("GetRecV20")
             self._api_version["GetAudioAlarm"] = check_command_exists("GetAudioAlarmV20")
             self._api_version["GetMdAlarm"] = check_command_exists("GetMdAlarm")
@@ -1455,14 +1559,22 @@
             else:
                 ch_body = [{"cmd": "GetMdState", "action": 0, "param": {"channel": channel}}]
                 if self.ai_supported(channel):
                     ch_body.append({"cmd": "GetAiState", "action": 0, "param": {"channel": channel}})
             body.extend(ch_body)
             channels.extend([channel] * len(ch_body))
 
+        if not body:
+            _LOGGER.debug(
+                "Host %s:%s: get_motion_state_all_ch, no channels connected so skipping request.",
+                self._host,
+                self._port,
+            )
+            return True
+
         try:
             json_data = await self.send(body, expected_response_type="json")
         except InvalidContentTypeError as err:
             _LOGGER.error(
                 "Host %s:%s: error translating All Motion States response: %s",
                 self._host,
                 self._port,
@@ -1482,45 +1594,84 @@
                 self._motion_detection_states[channel] = False
                 self._ai_detection_states[channel] = {}
             return False
 
         self.map_channels_json_response(json_data, channels)
         return True
 
-    async def check_new_firmware(self) -> bool | str:
-        """check for new firmware, returns False if no new firmware available."""
-        if not self.supported(None, "update"):
-            raise NotSupportedError(f"check_new_firmware: not supported by {self.nvr_name}")
+    async def _check_reolink_firmware(self) -> NewSoftwareVersion:
+        """Check for new firmware from reolink.com"""
+        if self._nvr_sw_hardware_id is None or self._nvr_sw_model_id is None:
+            request_URL = "https://reolink.com/wp-json/reo-v2/download/hardware-version/selection-list"
+            json_data = await self.send_reolink_com(request_URL)
+
+            for device in json_data["data"]:
+                if device["title"] == self.hardware_version and device["dlProduct"]["title"].startswith(self.model):
+                    self._nvr_sw_hardware_id = device["id"]
+                    self._nvr_sw_model_id = device["dlProduct"]["id"]
+                    break
 
-        body: reolink_json = [
-            {"cmd": "CheckFirmware"},
-            {"cmd": "GetDevInfo", "action": 0, "param": {}},
-        ]
+        if self._nvr_sw_hardware_id is None or self._nvr_sw_model_id is None:
+            raise UnexpectedDataError(f"Could not find model '{self.model}' hardware '{self.hardware_version}' in list from reolink.com")
 
-        try:
-            json_data = await self.send(body, expected_response_type="json")
-        except InvalidContentTypeError as err:
-            raise InvalidContentTypeError(f"Check firmware: {str(err)}") from err
-        except NoDataError as err:
-            raise NoDataError(f"Host: {self._host}:{self._port}: error obtaining CheckFirmware response") from err
+        request_URL = f"https://reolink.com/wp-json/reo-v2/download/firmware/?dlProductId={self._nvr_sw_model_id}&hardwareVersion={self._nvr_sw_hardware_id}&lang=en"
+        json_data = await self.send_reolink_com(request_URL)
 
-        self.map_host_json_response(json_data)
+        firmware_info = json_data["data"][0]["firmwares"][0]
+        hw_ver = firmware_info["hardwareVersion"][0]["title"]
+        mod_ver = firmware_info["hardwareVersion"][0]["dlProduct"]["title"]
+        if hw_ver != self.hardware_version or not mod_ver.startswith(self.model):
+            raise UnexpectedDataError(
+                f"Hardware version of firmware info from reolink.com does not match: '{hw_ver}' != '{self.hardware_version}' or '{mod_ver}' != '{self.model}'"
+            )
 
-        try:
-            new_firmware = json_data[0]["value"]["newFirmware"]
-        except KeyError as err:
-            raise UnexpectedDataError(f"Host {self._host}:{self._port}: received an unexpected response from check_new_firmware: {json_data}") from err
+        return NewSoftwareVersion(firmware_info["version"], download_url=firmware_info["url"], release_notes=firmware_info["new"])
 
-        if new_firmware == 0:
-            return False
+    async def check_new_firmware(self) -> bool | NewSoftwareVersion | str:
+        """check for new firmware using camera API, returns False if no new firmware available."""
+        new_firmware = 0
+        if self.supported(None, "update"):
+            body: typings.reolink_json = [
+                {"cmd": "CheckFirmware"},
+                {"cmd": "GetDevInfo", "action": 0, "param": {}},
+            ]
 
-        if new_firmware == 1:
-            return "New firmware available"
+            try:
+                json_data = await self.send(body, expected_response_type="json")
+            except InvalidContentTypeError as err:
+                raise InvalidContentTypeError(f"Check firmware: {str(err)}") from err
+            except NoDataError as err:
+                raise NoDataError(f"Host: {self._host}:{self._port}: error obtaining CheckFirmware response") from err
 
-        return str(new_firmware)
+            self.map_host_json_response(json_data)
+
+            try:
+                new_firmware = json_data[0]["value"]["newFirmware"]
+            except KeyError as err:
+                raise UnexpectedDataError(f"Host {self._host}:{self._port}: received an unexpected response from check_new_firmware: {json_data}") from err
+
+        try:
+            latest_software_version = await self._check_reolink_firmware()
+        except ReolinkError as err:
+            _LOGGER.debug(err)
+            if new_firmware == 0:
+                return False
+            if new_firmware == 1:
+                return "New firmware available"
+            return str(new_firmware)
+
+        if self._nvr_sw_version_object is None or self._nvr_sw_version_object >= latest_software_version:
+            if new_firmware == 0:
+                return False
+            if new_firmware == 1:
+                return "New firmware available"
+            return str(new_firmware)
+
+        latest_software_version.online_update_available = new_firmware == 1
+        return latest_software_version
 
     async def update_firmware(self) -> None:
         """check for new firmware."""
         if not self.supported(None, "update"):
             raise NotSupportedError(f"update_firmware: not supported by {self.nvr_name}")
 
         body = [{"cmd": "UpgradeOnline"}]
@@ -1563,15 +1714,15 @@
             stream = stream.removeprefix("snapshots_")
 
         if stream not in ["main", "sub"]:
             stream = "main"
 
         param["snapType"] = stream
 
-        body: reolink_json = [{}]
+        body: typings.reolink_json = [{}]
         response = await self.send(body, param, expected_response_type="image/jpeg")
         if response is None or response == b"":
             _LOGGER.error(
                 "Host: %s:%s: error obtaining still image response for channel %s.",
                 self._host,
                 self._port,
                 channel,
@@ -1726,25 +1877,41 @@
         file = filename.replace("/", "%20")
         # Looks like it only works with login/password method, not with token
         return (
             "application/x-mpegURL",
             f"rtmp://{self._host}:{self._rtmp_port}/vod/{file}?channel={channel}&stream={stream_type}&user={self._username}&password={self._password}",
         )
 
-    def map_host_json_response(self, json_data: reolink_json):
+    async def download_vod(self, filename: str, wanted_filename: Optional[str] = None) -> typings.VOD_download:
+        if wanted_filename is None:
+            wanted_filename = filename.replace("/", "_")
+
+        param: dict[str, Any] = {"cmd": "Download", "source": filename, "output": wanted_filename}
+        body: typings.reolink_json = [{}]
+        response = await self.send(body, param, expected_response_type="application/octet-stream")
+
+        if response.content_length is None:
+            response.release()
+            raise UnexpectedDataError(f"Host {self._host}:{self._port}: Download VOD: no 'content_length' in the response")
+        if response.content_disposition is None or response.content_disposition.filename is None:
+            response.release()
+            raise UnexpectedDataError(f"Host {self._host}:{self._port}: Download VOD: no 'content_disposition.filename' in the response")
+
+        return typings.VOD_download(response.content_length, response.content_disposition.filename, response.content, response.headers.get("ETag"))
+
+    def map_host_json_response(self, json_data: typings.reolink_json):
         """Map the JSON objects to internal cache-objects."""
         for data in json_data:
             try:
                 if data["code"] == 1:  # Error, like "ability error"
                     continue
 
                 if data["cmd"] == "GetChannelstatus":
                     if not self._GetChannelStatus_present and (self._nvr_num_channels == 0 or len(self._channels) == 0):
                         self._channels.clear()
-                        self._channel_models.clear()
                         self._is_doorbell.clear()
 
                         cur_value = data["value"]
                         self._nvr_num_channels = cur_value["count"]
 
                         if self._nvr_num_channels > 0:
                             cur_status = cur_value["status"]
@@ -1759,16 +1926,18 @@
                             for ch_info in cur_status:
                                 if ch_info["online"] == 1:
                                     cur_channel = ch_info["channel"]
 
                                     if self._GetChannelStatus_has_name:
                                         self._channel_names[cur_channel] = ch_info["name"]
 
-                                    self._channel_models[cur_channel] = ch_info.get("typeInfo", "Unknown")  # Not all Reolink devices respond with "typeInfo" attribute.
-                                    self._is_doorbell[cur_channel] = "Doorbell" in self._channel_models[cur_channel]
+                                    if "typeInfo" in ch_info:  # Not all Reolink devices respond with "typeInfo" attribute.
+                                        self._channel_models[cur_channel] = ch_info["typeInfo"]
+                                        self._is_doorbell[cur_channel] = "Doorbell" in self._channel_models[cur_channel]
+
                                     self._channels.append(cur_channel)
                         else:
                             self._channel_names.clear()
                     elif self._GetChannelStatus_has_name:
                         cur_status = data["value"]["status"]
                         for ch_info in cur_status:
                             if ch_info["online"] == 1:
@@ -1804,36 +1973,32 @@
                     self._nvr_sw_version = dev_info["firmVer"]
                     if self._nvr_sw_version is not None:
                         self._nvr_sw_version_object = SoftwareVersion(self._nvr_sw_version)
 
                     # In case the "GetChannelStatus" command not supported by the device.
                     if not self._GetChannelStatus_present and self._nvr_num_channels == 0:
                         self._channels.clear()
-                        self._channel_models.clear()
-                        self._is_doorbell.clear()
 
                         self._nvr_num_channels = dev_info["channelNum"]
 
                         if self._is_nvr:
                             _LOGGER.warning(
                                 "Your %s NVR doesn't support the 'Getchannelstatus' command. "
                                 "Probably you need to update your firmware.\n"
                                 "No way to recognize active channels, all %s channels will be considered 'active' as a result",
                                 self._nvr_name,
                                 self._nvr_num_channels,
                             )
 
-                        if self._nvr_num_channels > 0 and self._nvr_model is not None:
-                            is_doorbell = "Doorbell" in self._nvr_model
-                            for i in range(self._nvr_num_channels):
-                                self._channel_models[i] = self._nvr_model
-                                self._is_doorbell[i] = is_doorbell
-                                self._channels.append(i)
-                        else:
-                            self._channel_names.clear()
+                        if self._nvr_num_channels > 0:
+                            for ch in range(self._nvr_num_channels):
+                                self._channels.append(ch)
+                                if ch not in self._channel_models and self._nvr_model is not None:
+                                    self._channel_models[ch] = self._nvr_model
+                                    self._is_doorbell[ch] = "Doorbell" in self._nvr_model
 
                 elif data["cmd"] == "GetHddInfo":
                     self._hdd_info = data["value"]["HddInfo"]
 
                 elif data["cmd"] == "GetLocalLink":
                     self._local_link = data["value"]
                     self._mac_address = data["value"]["LocalLink"]["mac"]
@@ -1852,14 +2017,18 @@
                 elif data["cmd"] == "GetUser":
                     self._users = data["value"]["User"]
 
                 elif data["cmd"] == "GetNtp":
                     self._ntp_settings = data["value"]
 
                 elif data["cmd"] == "GetTime":
+                    time_diffrence = (datetime.now() - reolink_time_to_datetime(data["value"]["Time"])).total_seconds()
+                    if abs(time_diffrence) < 10:
+                        time_diffrence = 0
+                    self._host_time_difference = time_diffrence
                     self._time_settings = data["value"]
 
                 elif data["cmd"] == "GetAbility":
                     self._abilities = data["value"]["Ability"]
 
             except Exception as err:  # pylint: disable=bare-except
                 _LOGGER.error(
@@ -1890,14 +2059,18 @@
         response_channel = channel
         for data in json_data:
             try:
                 if data["code"] == 1:  # -->Error, like "ability error"
                     _LOGGER.debug("Host %s:%s received response error code: %s", self._host, self._port, data)
                     continue
 
+                if data["cmd"] == "GetChnTypeInfo":
+                    self._channel_models[channel] = data["value"]["typeInfo"]
+                    self._is_doorbell[channel] = "Doorbell" in self._channel_models[channel]
+
                 if data["cmd"] == "GetEvents":
                     response_channel = data["value"]["channel"]
                     if response_channel != channel:
                         _LOGGER.error("Host %s:%s: GetEvents response channel %s does not equal requested channel %s", self._host, self._port, response_channel, channel)
                         continue
                     if "ai" in data["value"]:
                         self._ai_detection_states[channel] = {}
@@ -1986,15 +2159,16 @@
                 elif data["cmd"] == "GetPush":
                     self._push_settings[channel] = data["value"]
 
                 elif data["cmd"] == "GetPushV20":
                     self._push_settings[channel] = data["value"]
 
                 elif data["cmd"] == "GetEnc":
-                    response_channel = data["value"]["Enc"]["channel"]
+                    # GetEnc returns incorrect channel for DUO camera
+                    # response_channel = data["value"]["Enc"]["channel"]
                     self._enc_settings[channel] = data["value"]
 
                 elif data["cmd"] == "GetRtspUrl":
                     response_channel = data["value"]["rtspUrl"]["channel"]
                     password = parse.quote(self._password)
                     mainStream = data["value"]["rtspUrl"]["mainStream"]
                     subStream = data["value"]["rtspUrl"]["subStream"]
@@ -2040,14 +2214,17 @@
                             preset_name = preset["name"]
                             preset_id = int(preset["id"])
                             self._ptz_presets[channel][preset_name] = preset_id
 
                 elif data["cmd"] == "GetPtzGuard":
                     self._ptz_guard_settings[channel] = data["value"]
 
+                elif data["cmd"] == "GetPtzCurPos":
+                    self._ptz_position[channel] = data["value"]
+
                 elif data["cmd"] == "GetAiCfg":
                     self._auto_track_settings[channel] = data["value"]
                     if "range" in data:
                         self._auto_track_range[channel] = data["range"]
 
                 elif data["cmd"] == "GetPtzTraceSection":
                     self._auto_track_limits[channel] = data["value"]
@@ -2097,15 +2274,15 @@
         """Set Network Port parameters on the host (NVR or camera)."""
         if self._netport_settings is None:
             await self.get_state("GetNetPort")
 
         if self._netport_settings is None:
             raise NotSupportedError(f"set_net_port: failed to retrieve current NetPort settings from {self._host}:{self._port}")
 
-        body: reolink_json = [{"cmd": "SetNetPort", "param": self._netport_settings}]
+        body: typings.reolink_json = [{"cmd": "SetNetPort", "param": self._netport_settings}]
 
         if enable_onvif is not None:
             body[0]["param"]["NetPort"]["onvifEnable"] = 1 if enable_onvif else 0
         if enable_rtmp is not None:
             body[0]["param"]["NetPort"]["rtmpEnable"] = 1 if enable_rtmp else 0
         if enable_rtsp is not None:
             body[0]["param"]["NetPort"]["rtspEnable"] = 1 if enable_rtsp else 0
@@ -2121,15 +2298,15 @@
         tzoffset (int) Timezone offset versus UTC in seconds
 
         Always get current time first"""
         await self.get_state("GetTime")
         if self._time_settings is None:
             raise NotSupportedError(f"set_time: failed to retrieve current time settings from {self._host}:{self._port}")
 
-        body: reolink_json = [{"cmd": "SetTime", "action": 0, "param": self._time_settings}]
+        body: typings.reolink_json = [{"cmd": "SetTime", "action": 0, "param": self._time_settings}]
 
         if dateFmt is not None:
             if dateFmt in ["DD/MM/YYYY", "MM/DD/YYYY", "YYYY/MM/DD"]:
                 body[0]["param"]["Time"]["timeFmt"] = dateFmt
             else:
                 raise InvalidParameterError(f"set_time: date format {dateFmt} not in ['DD/MM/YYYY', 'MM/DD/YYYY', 'YYYY/MM/DD']")
 
@@ -2159,15 +2336,15 @@
         """
         if self._ntp_settings is None:
             await self.get_state("GetNtp")
 
         if self._ntp_settings is None:
             raise NotSupportedError(f"set_ntp: failed to retrieve current NTP settings from {self._host}:{self._port}")
 
-        body: reolink_json = [{"cmd": "SetNtp", "action": 0, "param": self._ntp_settings}]
+        body: typings.reolink_json = [{"cmd": "SetNtp", "action": 0, "param": self._ntp_settings}]
 
         if enable is not None:
             if enable:
                 body[0]["param"]["Ntp"]["enable"] = 1
             else:
                 body[0]["param"]["Ntp"]["enable"] = 0
 
@@ -2194,15 +2371,15 @@
         """Sync date and time on the host via NTP now."""
         if self._ntp_settings is None:
             await self.get_state("GetNtp")
 
         if self._ntp_settings is None:
             raise NotSupportedError(f"set_ntp: failed to retrieve current NTP settings from {self._host}:{self._port}")
 
-        body: reolink_json = [{"cmd": "SetNtp", "action": 0, "param": self._ntp_settings}]
+        body: typings.reolink_json = [{"cmd": "SetNtp", "action": 0, "param": self._ntp_settings}]
         body[0]["param"]["Ntp"]["interval"] = 0
 
         await self.send_setting(body)
 
     def get_focus(self, channel: int) -> None:
         """Get absolute focus value."""
         if channel not in self._channels:
@@ -2249,15 +2426,15 @@
     async def set_autofocus(self, channel: int, enable: bool) -> None:
         """Enable/Disable AutoFocus on a camera."""
         if channel not in self._channels:
             raise InvalidParameterError(f"set_autofocus: no camera connected to channel '{channel}'")
         if channel not in self._auto_focus_settings:
             raise NotSupportedError(f"set_autofocus: AutoFocus on camera {self.camera_name(channel)} is not available")
 
-        body: reolink_json = [{"cmd": "SetAutoFocus", "action": 0, "param": {"AutoFocus": {"disable": 0 if enable else 1, "channel": channel}}}]
+        body: typings.reolink_json = [{"cmd": "SetAutoFocus", "action": 0, "param": {"AutoFocus": {"disable": 0 if enable else 1, "channel": channel}}}]
         await self.send_setting(body)
 
     def get_zoom(self, channel: int):
         """Get absolute zoom value."""
         if channel not in self._channels:
             raise InvalidParameterError(f"get_zoom: no camera connected to channel '{channel}'")
         if channel not in self._zoom_focus_settings or not self._zoom_focus_settings[channel]:
@@ -2319,29 +2496,36 @@
                 preset = self.ptz_presets(channel)[preset]
             if not isinstance(preset, int):
                 raise InvalidParameterError(f"set_ptz_command: preset {preset} is not integer")
 
         if command is None:
             raise InvalidParameterError("set_ptz_command: No command or preset specified.")
 
-        body: reolink_json = [
+        body: typings.reolink_json = [
             {
                 "cmd": "PtzCtrl",
                 "action": 0,
                 "param": {"channel": channel, "op": command},
             }
         ]
 
         if speed:
             body[0]["param"]["speed"] = speed
         if preset:
             body[0]["param"]["id"] = preset
 
         await self.send_setting(body)
 
+    def ptz_pan_position(self, channel: int) -> int:
+        """pan position"""
+        if channel not in self._ptz_position:
+            return 0
+
+        return self._ptz_position[channel]["PtzCurPos"]["Ppos"]
+
     def ptz_guard_enabled(self, channel: int) -> bool:
         if channel not in self._ptz_guard_settings:
             return False
 
         values = self._ptz_guard_settings[channel]["PtzGuard"]
         return values["benable"] == 1 and values["bexistPos"] == 1
 
@@ -2371,30 +2555,33 @@
         if command is None:
             params["cmdStr"] = "setPos"
         if enable is not None:
             params["benable"] = 1 if enable else 0
         if time is not None:
             params["timeout"] = time
 
-        body: reolink_json = [{"cmd": "SetPtzGuard", "action": 0, "param": {"PtzGuard": params}}]
+        body: typings.reolink_json = [{"cmd": "SetPtzGuard", "action": 0, "param": {"PtzGuard": params}}]
         await self.send_setting(body)
 
     async def ptz_callibrate(self, channel: int) -> None:
         """Callibrate PTZ of the camera."""
         if channel not in self._channels:
             raise InvalidParameterError(f"ptz_callibrate: no camera connected to channel '{channel}'")
 
-        body: reolink_json = [{"cmd": "PtzCheck", "action": 0, "param": {"channel": channel}}]
+        body: typings.reolink_json = [{"cmd": "PtzCheck", "action": 0, "param": {"channel": channel}}]
         await self.send_setting(body)
 
     def auto_track_enabled(self, channel: int) -> bool:
         if channel not in self._auto_track_settings:
             return False
 
-        return self._auto_track_settings[channel]["bSmartTrack"] == 1
+        if "bSmartTrack" in self._auto_track_settings[channel]:
+            return self._auto_track_settings[channel]["bSmartTrack"] == 1
+
+        return self._auto_track_settings[channel]["aiTrack"] == 1
 
     def auto_track_disappear_time(self, channel: int) -> int:
         if channel not in self._auto_track_settings:
             return -1
 
         return self._auto_track_settings[channel].get("aiDisappearBackTime", -1)
 
@@ -2416,15 +2603,18 @@
         if channel not in self._channels:
             raise InvalidParameterError(f"set_auto_tracking: no camera connected to channel '{channel}'")
         if not self.supported(channel, "auto_track"):
             raise NotSupportedError(f"set_auto_tracking: Auto tracking on camera {self.camera_name(channel)} is not available")
 
         params = {"channel": channel}
         if enable is not None:
-            params["bSmartTrack"] = 1 if enable else 0
+            if "bSmartTrack" in self._auto_track_settings[channel]:
+                params["bSmartTrack"] = 1 if enable else 0
+            else:
+                params["aiTrack"] = 1 if enable else 0
         if disappear_time is not None:
             params["aiDisappearBackTime"] = disappear_time
         if stop_time is not None:
             params["aiStopBackTime"] = stop_time
         if method is not None:
             if isinstance(method, str):
                 method_int = TrackMethodEnum[method].value
@@ -2496,15 +2686,15 @@
             raise InvalidParameterError(f"set_osd: no camera connected to channel '{channel}'")
 
         await self.get_state("GetOsd")
 
         if channel not in self._osd_settings or not self._osd_settings[channel]:
             raise NotSupportedError(f"set_osd: OSD on camera {self.camera_name(channel)} is not available")
 
-        body: reolink_json = [{"cmd": "SetOsd", "action": 0, "param": self._osd_settings[channel]}]
+        body: typings.reolink_json = [{"cmd": "SetOsd", "action": 0, "param": self._osd_settings[channel]}]
 
         if namePos is not None:
             if namePos == "Off":
                 body[0]["param"]["Osd"]["osdChannel"]["enable"] = 0
             else:
                 if not self.validate_osd_pos(namePos):
                     raise InvalidParameterError(f"set_osd: Invalid name OSD position specified '{namePos}'")
@@ -2535,15 +2725,15 @@
         await self.send_setting(body)
 
     async def set_push(self, channel: int | None, enable: bool) -> None:
         """Set the PUSH-notifications parameter."""
         if not self.supported(channel, "push"):
             raise NotSupportedError(f"set_push: push-notifications on camera {self.camera_name(channel)} are not available")
 
-        body: reolink_json
+        body: typings.reolink_json
         on_off = 1 if enable else 0
         if channel is None:
             if self.api_version("GetPush") >= 1:
                 body = [{"cmd": "SetPushV20", "action": 0, "param": {"Push": {"enable": on_off}}}]
                 await self.send_setting(body)
                 return
 
@@ -2553,26 +2743,26 @@
                     await self.send_setting(body)
             return
 
         if channel not in self._channels:
             raise InvalidParameterError(f"set_push: no camera connected to channel '{channel}'")
 
         if self.api_version("GetPush") >= 1:
-            body = [{"cmd": "SetPushV20", "action": 0, "param": {"Push": {"enable": on_off, "schedule": {"channel": channel}}}}]
+            body = [{"cmd": "SetPushV20", "action": 0, "param": {"Push": {"scheduleEnable": on_off, "schedule": {"channel": channel}}}}]
         else:
             body = [{"cmd": "SetPush", "action": 0, "param": {"Push": {"schedule": {"enable": on_off, "channel": channel}}}}]
 
         await self.send_setting(body)
 
     async def set_ftp(self, channel: int | None, enable: bool) -> None:
         """Set the FTP-notifications parameter."""
         if not self.supported(channel, "ftp"):
             raise NotSupportedError(f"set_ftp: FTP on camera {self.camera_name(channel)} is not available")
 
-        body: reolink_json
+        body: typings.reolink_json
         on_off = 1 if enable else 0
         if channel is None:
             if self.api_version("GetFtp") >= 1:
                 body = [{"cmd": "SetFtpV20", "action": 0, "param": {"Ftp": {"enable": on_off}}}]
                 await self.send_setting(body)
                 return
 
@@ -2582,25 +2772,25 @@
                     await self.send_setting(body)
             return
 
         if channel not in self._channels:
             raise InvalidParameterError(f"set_ftp: no camera connected to channel '{channel}'")
 
         if self.api_version("GetFtp") >= 1:
-            body = [{"cmd": "SetFtpV20", "action": 0, "param": {"Ftp": {"enable": on_off, "schedule": {"channel": channel}}}}]
+            body = [{"cmd": "SetFtpV20", "action": 0, "param": {"Ftp": {"scheduleEnable": on_off, "schedule": {"channel": channel}}}}]
         else:
             body = [{"cmd": "SetFtp", "action": 0, "param": {"Ftp": {"schedule": {"enable": on_off, "channel": channel}}}}]
 
         await self.send_setting(body)
 
     async def set_email(self, channel: int | None, enable: bool) -> None:
         if not self.supported(channel, "email"):
             raise NotSupportedError(f"set_email: Email on camera {self.camera_name(channel)} is not available")
 
-        body: reolink_json
+        body: typings.reolink_json
         on_off = 1 if enable else 0
         if channel is None:
             if self.api_version("GetEmail") >= 1:
                 body = [{"cmd": "SetEmailV20", "action": 0, "param": {"Email": {"enable": on_off}}}]
                 await self.send_setting(body)
                 return
 
@@ -2610,26 +2800,26 @@
                     await self.send_setting(body)
             return
 
         if channel not in self._channels:
             raise InvalidParameterError(f"set_email: no camera connected to channel '{channel}'")
 
         if self.api_version("GetEmail") >= 1:
-            body = [{"cmd": "SetEmailV20", "action": 0, "param": {"Email": {"enable": on_off, "schedule": {"channel": channel}}}}]
+            body = [{"cmd": "SetEmailV20", "action": 0, "param": {"Email": {"scheduleEnable": on_off, "schedule": {"channel": channel}}}}]
         else:
             body = [{"cmd": "SetEmail", "action": 0, "param": {"Email": {"schedule": {"enable": on_off, "channel": channel}}}}]
 
         await self.send_setting(body)
 
     async def set_recording(self, channel: int | None, enable: bool) -> None:
         """Set the recording parameter."""
         if not self.supported(channel, "recording"):
             raise NotSupportedError(f"set_recording: recording on camera {self.camera_name(channel)} is not available")
 
-        body: reolink_json
+        body: typings.reolink_json
         on_off = 1 if enable else 0
         if channel is None:
             if self.api_version("GetRec") >= 1:
                 body = [{"cmd": "SetRecV20", "action": 0, "param": {"Rec": {"enable": on_off}}}]
                 await self.send_setting(body)
                 return
 
@@ -2639,58 +2829,58 @@
                     await self.send_setting(body)
             return
 
         if channel not in self._channels:
             raise InvalidParameterError(f"set_recording: no camera connected to channel '{channel}'")
 
         if self.api_version("GetRec") >= 1:
-            body = [{"cmd": "SetRecV20", "action": 0, "param": {"Rec": {"enable": on_off, "schedule": {"channel": channel}}}}]
+            body = [{"cmd": "SetRecV20", "action": 0, "param": {"Rec": {"scheduleEnable": on_off, "schedule": {"channel": channel}}}}]
         else:
             body = [{"cmd": "SetRec", "action": 0, "param": {"Rec": {"schedule": {"enable": on_off, "channel": channel}}}}]
 
         await self.send_setting(body)
 
     async def set_buzzer(self, channel: int | None, enable: bool) -> None:
         """Set the NVR buzzer parameter."""
         if not self.supported(channel, "buzzer"):
             raise NotSupportedError(f"set_buzzer: NVR buzzer on camera {self.camera_name(channel)} is not available")
 
-        body: reolink_json
+        body: typings.reolink_json
         on_off = 1 if enable else 0
         if channel is None:
             body = [{"cmd": "SetBuzzerAlarmV20", "action": 0, "param": {"Buzzer": {"enable": on_off}}}]
             await self.send_setting(body)
             return
 
         if channel not in self._channels:
             raise InvalidParameterError(f"set_recording: no camera connected to channel '{channel}'")
 
-        body = [{"cmd": "SetBuzzerAlarmV20", "action": 0, "param": {"Buzzer": {"enable": on_off, "schedule": {"channel": channel}}}}]
+        body = [{"cmd": "SetBuzzerAlarmV20", "action": 0, "param": {"Buzzer": {"scheduleEnable": on_off, "schedule": {"channel": channel}}}}]
         await self.send_setting(body)
 
     async def set_audio(self, channel: int, enable: bool) -> None:
         if channel not in self._channels:
             raise InvalidParameterError(f"set_audio: no camera connected to channel '{channel}'")
         await self.get_state(cmd="GetEnc")
         if channel not in self._enc_settings:
             raise NotSupportedError(f"set_audio: Audio on camera {self.camera_name(channel)} is not available")
 
-        body: reolink_json = [{"cmd": "SetEnc", "action": 0, "param": self._enc_settings[channel]}]
+        body: typings.reolink_json = [{"cmd": "SetEnc", "action": 0, "param": self._enc_settings[channel]}]
         body[0]["param"]["Enc"]["audio"] = 1 if enable else 0
 
         await self.send_setting(body)
 
     async def set_ir_lights(self, channel: int, enable: bool) -> None:
         if channel not in self._channels:
             raise InvalidParameterError(f"set_ir_lights: no camera connected to channel '{channel}'")
         if channel not in self._ir_settings:
             raise NotSupportedError(f"set_ir_lights: IR light on camera {self.camera_name(channel)} is not available")
 
         state = "Auto" if enable else "Off"
-        body: reolink_json = [
+        body: typings.reolink_json = [
             {
                 "cmd": "SetIrLights",
                 "action": 0,
                 "param": {"IrLights": {"channel": channel, "state": state}},
             }
         ]
 
@@ -2712,15 +2902,15 @@
             raise InvalidParameterError(f"set_status_led: value {value} not in {val_list}")
 
         if self.is_doorbell(channel):
             param = {"channel": channel, "eDoorbellLightState": value}
         else:
             param = {"channel": channel, "state": value}
 
-        body: reolink_json = [{"cmd": "SetPowerLed", "action": 0, "param": {"PowerLed": param}}]
+        body: typings.reolink_json = [{"cmd": "SetPowerLed", "action": 0, "param": {"PowerLed": param}}]
         await self.send_setting(body)
 
     async def set_whiteled(self, channel: int, state: bool | None = None, brightness: int | None = None, mode: int | str | None = None) -> None:
         """
         Set the WhiteLed parameter.
         with Reolink Duo GetWhiteLed returns an error state
         SetWhiteLed appears to require 4 parameters
@@ -2884,15 +3074,15 @@
 
     async def set_audio_alarm(self, channel: int, enable: bool) -> None:
         # fairly basic only either turns it off or on
         # called in its simple form by set_siren
 
         if channel not in self._channels:
             raise InvalidParameterError(f"set_audio_alarm: no camera connected to channel '{channel}'")
-        if channel not in self._audio_alarm_settings or not self._audio_alarm_settings[channel]:
+        if not self.supported(channel, "siren"):
             raise NotSupportedError(f"set_audio_alarm: AudioAlarm on camera {self.camera_name(channel)} is not available")
 
         if self.api_version("GetAudioAlarm") >= 1:
             body = [{"cmd": "SetAudioAlarmV20", "param": {"Audio": {"enable": 1 if enable else 0, "schedule": {"channel": channel}}}}]
         else:
             body = [
                 {
@@ -2914,14 +3104,16 @@
         # Uses API AudioAlarmPlay with manual switch
         # uncertain if there may be a glitch - dont know if there is API I have yet to find
         # which sets AudioLevel
         if channel not in self._channels:
             raise InvalidParameterError(f"set_siren: no camera connected to channel '{channel}'")
         if duration is not None and not isinstance(duration, int):
             raise InvalidParameterError(f"set_siren: duration '{duration}' is not integer")
+        if not self.supported(channel, "siren_play"):
+            raise NotSupportedError(f"set_siren: AudioAlarmPlay on camera {self.camera_name(channel)} is not available")
 
         if enable:
             if duration is not None:
                 params = {
                     "alarm_mode": "times",
                     "times": duration,
                     "channel": channel,
@@ -2956,42 +3148,42 @@
         if channel not in self._isp_settings or not self._isp_settings[channel]:
             raise NotSupportedError(f"set_daynight: ISP on camera {self.camera_name(channel)} is not available")
 
         val_list = [val.value for val in DayNightEnum]
         if value not in val_list:
             raise InvalidParameterError(f"set_daynight: value {value} not in {val_list}")
 
-        body: reolink_json = [{"cmd": "SetIsp", "action": 0, "param": self._isp_settings[channel]}]
+        body: typings.reolink_json = [{"cmd": "SetIsp", "action": 0, "param": self._isp_settings[channel]}]
         body[0]["param"]["Isp"]["dayNight"] = value
 
         await self.send_setting(body)
 
     async def set_backlight(self, channel: int, value: str) -> None:
         if channel not in self._channels:
             raise InvalidParameterError(f"set_backlight: no camera connected to channel '{channel}'")
         await self.get_state(cmd="GetIsp")
         if channel not in self._isp_settings or not self._isp_settings[channel]:
             raise NotSupportedError(f"set_backlight: ISP on camera {self.camera_name(channel)} is not available")
 
         if value not in ["BackLightControl", "DynamicRangeControl", "Off"]:
             raise InvalidParameterError(f"set_backlight: value {value} not in ['BackLightControl', 'DynamicRangeControl', 'Off']")
 
-        body: reolink_json = [{"cmd": "SetIsp", "action": 0, "param": self._isp_settings[channel]}]
+        body: typings.reolink_json = [{"cmd": "SetIsp", "action": 0, "param": self._isp_settings[channel]}]
         body[0]["param"]["Isp"]["backLight"] = value
 
         await self.send_setting(body)
 
     async def set_motion_detection(self, channel: int, enable: bool) -> None:
         """Set the motion detection parameter."""
         if channel not in self._channels:
             raise InvalidParameterError(f"set_motion_detection: no camera connected to channel '{channel}'")
         if channel not in self._md_alarm_settings:
             raise NotSupportedError(f"set_motion_detection: alarm on camera {self.camera_name(channel)} is not available")
 
-        body: reolink_json = [{"cmd": "SetAlarm", "action": 0, "param": self._md_alarm_settings[channel]}]
+        body: typings.reolink_json = [{"cmd": "SetAlarm", "action": 0, "param": self._md_alarm_settings[channel]}]
         body[0]["param"]["Alarm"]["enable"] = 1 if enable else 0
 
         await self.send_setting(body)
 
     async def set_md_sensitivity(self, channel: int, value: int) -> None:
         """Set motion detection sensitivity.
         Here the camera web and windows application show a completely different value than set.
@@ -3002,15 +3194,15 @@
         if channel not in self._md_alarm_settings:
             raise NotSupportedError(f"set_md_sensitivity: md sensitivity on camera {self.camera_name(channel)} is not available")
         if not isinstance(value, int):
             raise InvalidParameterError(f"set_md_sensitivity: sensitivity '{value}' is not integer")
         if value < 1 or value > 50:
             raise InvalidParameterError(f"set_md_sensitivity: sensitivity {value} not in range 1...50")
 
-        body: reolink_json
+        body: typings.reolink_json
         if self.api_version("GetMdAlarm") >= 1:
             body = [{"cmd": "SetMdAlarm", "action": 0, "param": {"MdAlarm": {"channel": channel, "useNewSens": 1, "newSens": {"sensDef": int(51 - value)}}}}]
         else:
             body = [
                 {
                     "cmd": "SetAlarm",
                     "action": 0,
@@ -3037,57 +3229,97 @@
         if not isinstance(value, int):
             raise InvalidParameterError(f"set_ai_sensitivity: sensitivity '{value}' is not integer")
         if value < 0 or value > 100:
             raise InvalidParameterError(f"set_ai_sensitivity: sensitivity {value} not in range 0...100")
         if ai_type not in self.ai_supported_types(channel):
             raise InvalidParameterError(f"set_ai_sensitivity: ai type '{ai_type}' not supported for channel {channel}, suppored types are {self.ai_supported_types(channel)}")
 
-        body: reolink_json = [{"cmd": "SetAiAlarm", "action": 0, "param": {"AiAlarm": {"channel": channel, "ai_type": ai_type, "sensitivity": value}}}]
+        body: typings.reolink_json = [{"cmd": "SetAiAlarm", "action": 0, "param": {"AiAlarm": {"channel": channel, "ai_type": ai_type, "sensitivity": value}}}]
+        await self.send_setting(body)
+
+    async def set_image(
+        self, channel: int, bright: int | None = None, contrast: int | None = None, saturation: int | None = None, hue: int | None = None, sharpen: int | None = None
+    ) -> None:
+        """Set image adjustments."""
+        _image = {"Image": {"channel": channel}}
+
+        if bright is not None:
+            if not self.supported(channel, "isp_bright"):
+                raise NotSupportedError(f"set_image: bright on camera {self.camera_name(channel)} is not available")
+            if not isinstance(bright, int):
+                raise InvalidParameterError(f"set_image: bright '{bright}' is not integer")
+            if bright < 0 or bright > 255:
+                raise InvalidParameterError(f"set_image: bright {bright} not in range 0...255")
+            _image["Image"]["bright"] = bright
+
+        if contrast is not None:
+            if not self.supported(channel, "isp_contrast"):
+                raise NotSupportedError(f"set_image: bright on camera {self.camera_name(channel)} is not available")
+            if not isinstance(contrast, int):
+                raise InvalidParameterError(f"set_image: contrast '{contrast}' is not integer")
+            if contrast < 0 or contrast > 255:
+                raise InvalidParameterError(f"set_image: contrast {contrast} not in range 0...255")
+            _image["Image"]["contrast"] = contrast
+
+        if saturation is not None:
+            if not self.supported(channel, "isp_satruation"):
+                raise NotSupportedError(f"set_image: bright on camera {self.camera_name(channel)} is not available")
+            if not isinstance(saturation, int):
+                raise InvalidParameterError(f"set_image: saturation '{saturation}' is not integer")
+            if saturation < 0 or saturation > 255:
+                raise InvalidParameterError(f"set_image: saturation {saturation} not in range 0...255")
+            _image["Image"]["saturation"] = saturation
+
+        if hue is not None:
+            if not self.supported(channel, "isp_hue"):
+                raise NotSupportedError(f"set_image: bright on camera {self.camera_name(channel)} is not available")
+            if not isinstance(hue, int):
+                raise InvalidParameterError(f"set_image: hue '{hue}' is not integer")
+            if hue < 0 or hue > 255:
+                raise InvalidParameterError(f"set_image: hue {hue} not in range 0...255")
+            _image["Image"]["hue"] = hue
+
+        if sharpen is not None:
+            if not self.supported(channel, "isp_sharpen"):
+                raise NotSupportedError(f"set_image: bright on camera {self.camera_name(channel)} is not available")
+            if not isinstance(sharpen, int):
+                raise InvalidParameterError(f"set_image: sharpen '{sharpen}' is not integer")
+            if sharpen < 0 or sharpen > 255:
+                raise InvalidParameterError(f"set_image: sharpen {sharpen} not in range 0...255")
+            _image["Image"]["sharpen"] = sharpen
+
+        body: typings.reolink_json = [{"cmd": "SetImage", "param": _image}]
         await self.send_setting(body)
 
     async def request_vod_files(
         self,
         channel: int,
         start: datetime,
         end: datetime,
         status_only: bool = False,
         stream: Optional[str] = None,
-    ) -> tuple[list[typings.SearchStatus], list[typings.SearchFile]]:
+    ) -> tuple[list[typings.VOD_search_status], list[typings.VOD_file]]:
         """Send search VOD-files command."""
-        if channel not in self._channels:
+        if channel not in self._stream_channels:
             raise InvalidParameterError(f"Request VOD files: no camera connected to channel '{channel}'")
 
         if stream is None:
             stream = self._stream
 
         body = [
             {
                 "cmd": "Search",
                 "action": 0,
                 "param": {
                     "Search": {
                         "channel": channel,
                         "onlyStatus": 1 if status_only else 0,
                         "streamType": stream,
-                        "StartTime": {
-                            "year": start.year,
-                            "mon": start.month,
-                            "day": start.day,
-                            "hour": start.hour,
-                            "min": start.minute,
-                            "sec": start.second,
-                        },
-                        "EndTime": {
-                            "year": end.year,
-                            "mon": end.month,
-                            "day": end.day,
-                            "hour": end.hour,
-                            "min": end.minute,
-                            "sec": end.second,
-                        },
+                        "StartTime": datetime_to_reolink_time(start),
+                        "EndTime": datetime_to_reolink_time(end),
                     }
                 },
             }
         ]
 
         try:
             json_data = await self.send(body, {"cmd": "Search"}, expected_response_type="json")
@@ -3099,23 +3331,25 @@
         if json_data[0].get("code", -1) != 0:
             raise ApiError(f"Host: {self._host}:{self._port}: Request VOD files: API returned error code {json_data[0].get('code', -1)}, response: {json_data}")
 
         search_result = json_data[0].get("value", {}).get("SearchResult", {})
         if "Status" not in search_result:
             raise UnexpectedDataError(f"Host {self._host}:{self._port}: Request VOD files: no 'Status' in the response: {json_data}")
 
+        statuses = [typings.VOD_search_status(status) for status in search_result["Status"]]
         if status_only:
-            return search_result["Status"], []
+            return statuses, []
 
         if "File" not in search_result:
-            raise UnexpectedDataError(f"Host {self._host}:{self._port}: Request VOD files: no file data in the response: {json_data}")
+            # When there are now recordings available in the indicated time window, "File" will not be in the response.
+            return statuses, []
 
-        return search_result["Status"], search_result["File"]
+        return statuses, [typings.VOD_file(file, self.timezone()) for file in search_result["File"]]
 
-    async def send_setting(self, body: reolink_json, wait_before_get: int = 0) -> None:
+    async def send_setting(self, body: typings.reolink_json, wait_before_get: int = 0) -> None:
         command = body[0]["cmd"]
         _LOGGER.debug(
             'Sending command: "%s" to: %s:%s with body: %s',
             command,
             self._host,
             self._port,
             body,
@@ -3131,95 +3365,178 @@
         _LOGGER.debug("Response from cmd '%s' from %s:%s: %s", command, self._host, self._port, json_data)
 
         try:
             if json_data[0]["code"] != 0 or json_data[0].get("value", {}).get("rspCode", -1) != 200:
                 _LOGGER.debug("ApiError for command '%s', response: %s", command, json_data)
                 rspCode = json_data[0].get("value", json_data[0]["error"])["rspCode"]
                 detail = json_data[0].get("value", json_data[0]["error"]).get("detail", "")
-                raise ApiError(f"cmd '{command}': API returned error code {json_data[0]['code']}, " f"response code {rspCode}/{detail}")
+                raise ApiError(f"cmd '{command}': API returned error code {json_data[0]['code']}, response code {rspCode}/{detail}")
         except KeyError as err:
             raise UnexpectedDataError(f"Host {self._host}:{self._port}: received an unexpected response from command '{command}': {json_data}") from err
 
         if command[:3] == "Set":
             getcmd = command.replace("Set", "Get")
             if wait_before_get > 0:
                 await asyncio.sleep(wait_before_get)
             await self.get_state(cmd=getcmd)
 
     @overload
     async def send(
         self,
-        body: reolink_json,
+        body: typings.reolink_json,
         param: dict[str, Any] | None,
         expected_response_type: Literal["json"],
         retry: int = RETRY_ATTEMPTS,
-    ) -> reolink_json:
+    ) -> typings.reolink_json:
         ...
 
     @overload
     async def send(
         self,
-        body: reolink_json,
+        body: typings.reolink_json,
         param: dict[str, Any] | None,
         expected_response_type: Literal["image/jpeg"],
         retry: int = RETRY_ATTEMPTS,
     ) -> bytes:
         ...
 
     @overload
     async def send(
         self,
-        body: reolink_json,
+        body: typings.reolink_json,
         param: dict[str, Any] | None,
         expected_response_type: Literal["text/html"],
         retry: int = RETRY_ATTEMPTS,
     ) -> str:
         ...
 
     @overload
     async def send(
         self,
-        body: reolink_json,
+        body: typings.reolink_json,
+        param: dict[str, Any] | None,
+        expected_response_type: Literal["application/octet-stream"],
+        retry: int = RETRY_ATTEMPTS,
+    ) -> aiohttp.ClientResponse:
+        ...
+
+    @overload
+    async def send(
+        self,
+        body: typings.reolink_json,
         *,
         expected_response_type: Literal["json"],
         retry: int = RETRY_ATTEMPTS,
-    ) -> reolink_json:
+    ) -> typings.reolink_json:
         ...
 
     @overload
     async def send(
         self,
-        body: reolink_json,
+        body: typings.reolink_json,
         *,
         expected_response_type: Literal["image/jpeg"],
         retry: int = RETRY_ATTEMPTS,
     ) -> bytes:
         ...
 
     @overload
     async def send(
         self,
-        body: reolink_json,
+        body: typings.reolink_json,
         *,
         expected_response_type: Literal["text/html"],
         retry: int = RETRY_ATTEMPTS,
     ) -> str:
         ...
 
+    @overload
     async def send(
         self,
-        body: reolink_json,
+        body: typings.reolink_json,
+        *,
+        expected_response_type: Literal["application/octet-stream"],
+        retry: int = RETRY_ATTEMPTS,
+    ) -> aiohttp.ClientResponse:
+        ...
+
+    async def send(
+        self,
+        body: typings.reolink_json,
         param: dict[str, Any] | None = None,
-        expected_response_type: Literal["json"] | Literal["image/jpeg"] | Literal["text/html"] = "json",
+        expected_response_type: Literal["json"] | Literal["image/jpeg"] | Literal["text/html"] | Literal["application/octet-stream"] = "json",
         retry: int = RETRY_ATTEMPTS,
-    ) -> reolink_json | bytes | str:
+    ) -> typings.reolink_json | bytes | str | aiohttp.ClientResponse:
+        """
+        If a body contains more than MAX_CHUNK_ITEMS requests, split it up in chunks.
+        Otherwise you get a 'error': {'detail': 'send failed', 'rspCode': -16} response.
+        """
+        len_body = len(body)
+        if len_body <= MAX_CHUNK_ITEMS or expected_response_type != "json":
+            return await self.send_chunk(body, param, expected_response_type, retry)
+
+        response: typings.reolink_json = []
+        for chunk in range(0, len_body, MAX_CHUNK_ITEMS):
+            chunk_end = min(chunk + MAX_CHUNK_ITEMS, len_body)
+            _LOGGER.debug("sending chunks %i:%i of total %i requests", chunk + 1, chunk_end, len_body)
+            response.extend(await self.send_chunk(body[chunk:chunk_end], param, expected_response_type, retry))
+
+        return response
+
+    @overload
+    async def send_chunk(
+        self,
+        body: typings.reolink_json,
+        param: dict[str, Any] | None,
+        expected_response_type: Literal["json"],
+        retry: int,
+    ) -> typings.reolink_json:
+        ...
+
+    @overload
+    async def send_chunk(
+        self,
+        body: typings.reolink_json,
+        param: dict[str, Any] | None,
+        expected_response_type: Literal["image/jpeg"],
+        retry: int,
+    ) -> bytes:
+        ...
+
+    @overload
+    async def send_chunk(
+        self,
+        body: typings.reolink_json,
+        param: dict[str, Any] | None,
+        expected_response_type: Literal["text/html"],
+        retry: int,
+    ) -> str:
+        ...
+
+    @overload
+    async def send_chunk(
+        self,
+        body: typings.reolink_json,
+        param: dict[str, Any] | None,
+        expected_response_type: Literal["application/octet-stream"],
+        retry: int,
+    ) -> aiohttp.ClientResponse:
+        ...
+
+    async def send_chunk(
+        self,
+        body: typings.reolink_json,
+        param: dict[str, Any] | None,
+        expected_response_type: Literal["json"] | Literal["image/jpeg"] | Literal["text/html"] | Literal["application/octet-stream"],
+        retry: int,
+    ) -> typings.reolink_json | bytes | str | aiohttp.ClientResponse:
         """Generic send method."""
         retry = retry - 1
 
-        if expected_response_type == "image/jpeg":
+        if expected_response_type in ["image/jpeg", "application/octet-stream"]:
             cur_command = "" if param is None else param.get("cmd", "")
             is_login_logout = False
         else:
             cur_command = "" if len(body) == 0 else body[0].get("cmd", "")
             is_login_logout = cur_command in ["Login", "Logout"]
 
         if not is_login_logout:
@@ -3240,38 +3557,44 @@
         try:
             data: bytes | str
             if expected_response_type == "image/jpeg":
                 async with self._send_mutex:
                     response = await self._aiohttp_session.get(url=self._url, params=param, allow_redirects=False)
 
                 data = await response.read()  # returns bytes
+            elif expected_response_type == "application/octet-stream":
+                async with self._send_mutex:
+                    response = await self._aiohttp_session.get(url=self._url, params=param, allow_redirects=False)
+
+                data = ""  # Response will be a file and be large, pass the response instead of reading it here.
             else:
                 _LOGGER.debug("%s/%s:%s::send() HTTP Request body =\n%s\n", self.nvr_name, self._host, self._port, str(body).replace(self._password, "<password>"))
 
                 async with self._send_mutex:
                     response = await self._aiohttp_session.post(url=self._url, json=body, params=param, allow_redirects=False)
 
                 data = await response.text(encoding="utf-8")  # returns str
 
             _LOGGER.debug("%s/%s:%s::send() HTTP Response status = %s, content-type = (%s).", self.nvr_name, self._host, self._port, response.status, response.content_type)
             if cur_command == "Search" and len(data) > 500:
                 _LOGGER_DATA.debug("%s/%s:%s::send() HTTP Response (VOD search) data scrapped because it's too large.", self.nvr_name, self._host, self._port)
-            elif cur_command == "Snap":
-                _LOGGER_DATA.debug("%s/%s:%s::send() HTTP Response (snapshot) data scrapped because it's too large.", self.nvr_name, self._host, self._port)
+            elif cur_command in ["Snap", "Download"]:
+                _LOGGER_DATA.debug("%s/%s:%s::send() HTTP Response (snapshot/download) data scrapped because it's too large.", self.nvr_name, self._host, self._port)
             else:
                 _LOGGER_DATA.debug("%s/%s:%s::send() HTTP Response data:\n%s\n", self.nvr_name, self._host, self._port, data)
 
             if len(data) < 500 and response.content_type == "text/html":
                 if isinstance(data, bytes):
                     login_err = b'"detail" : "invalid user"' in data or b'"detail" : "login failed"' in data or b'detail" : "please login first' in data
                 else:
                     login_err = (
                         '"detail" : "invalid user"' in data or '"detail" : "login failed"' in data or 'detail" : "please login first' in data
                     ) and cur_command != "Logout"
                 if login_err:
+                    response.release()
                     if is_login_logout:
                         raise CredentialsInvalidError()
 
                     if retry <= 0:
                         raise CredentialsInvalidError()
                     _LOGGER.debug(
                         'Host %s:%s: "invalid login" response, trying to login again and retry the command.',
@@ -3280,23 +3603,27 @@
                     )
                     await self.expire_session()
                     return await self.send(body, param, expected_response_type, retry)
 
             expected_content_type: str = expected_response_type
             if expected_response_type == "json":
                 expected_content_type = "text/html"
-            if response.content_type != expected_content_type:
+            # Reolink typo "apolication/octet-stream" instead of "application/octet-stream"
+            if response.content_type not in [expected_content_type, "apolication/octet-stream"]:
+                response.release()
                 raise InvalidContentTypeError(f"Expected type '{expected_content_type}' but received '{response.content_type}'")
 
             if response.status == 502 and retry > 0:
                 _LOGGER.debug("Host %s:%s: 502/Bad Gateway response, trying to login again and retry the command.", self._host, self._port)
+                response.release()
                 await self.expire_session()
                 return await self.send(body, param, expected_response_type, retry)
 
             if response.status >= 400 or (is_login_logout and response.status != 200):
+                response.release()
                 raise ApiError(f"API returned HTTP status ERROR code {response.status}/{response.reason}")
 
             if expected_response_type == "json" and isinstance(data, str):
                 try:
                     json_data = json.loads(data)
                 except (TypeError, json.JSONDecodeError) as err:
                     if retry <= 0:
@@ -3314,27 +3641,32 @@
 
             if expected_response_type == "image/jpeg" and isinstance(data, bytes):
                 return data
 
             if expected_response_type == "text/html" and isinstance(data, str):
                 return data
 
+            if expected_response_type == "application/octet-stream":
+                # response needs to be read or released from the calling function
+                return response
+
+            response.release()
             raise InvalidContentTypeError(f"Expected {expected_response_type}, unexpected data received: {data!r}")
         except aiohttp.ClientConnectorError as err:
             await self.expire_session()
             _LOGGER.error("Host %s:%s: connection error: %s", self._host, self._port, str(err))
-            raise err
+            raise ReolinkConnectionError(f"Host {self._host}:{self._port}: connection error: {str(err)}") from err
         except asyncio.TimeoutError as err:
             await self.expire_session()
             _LOGGER.error(
                 "Host %s:%s: connection timeout exception. Please check the connection to this host.",
                 self._host,
                 self._port,
             )
-            raise err
+            raise ReolinkTimeoutError(f"Host {self._host}:{self._port}: Timeout error: {str(err)}") from err
         except ApiError as err:
             await self.expire_session()
             _LOGGER.error("Host %s:%s: API error: %s.", self._host, self._port, str(err))
             raise err
         except CredentialsInvalidError as err:
             await self.expire_session()
             _LOGGER.error("Host %s:%s: login attempt failed.", self._host, self._port)
@@ -3344,14 +3676,60 @@
             _LOGGER.debug("Host %s:%s: content type error: %s.", self._host, self._port, str(err))
             raise err
         except Exception as err:
             await self.expire_session()
             _LOGGER.error('Host %s:%s: unknown exception "%s" occurred, traceback:\n%s\n', self._host, self._port, str(err), traceback.format_exc())
             raise err
 
+    async def send_reolink_com(
+        self,
+        URL: str,
+        expected_response_type: Literal["application/json"] = "application/json",
+    ) -> dict[str, Any]:
+        """Generic send method for reolink.com site."""
+
+        if self._aiohttp_session.closed:
+            self._aiohttp_session = self._get_aiohttp_session()
+
+        try:
+            response = await self._aiohttp_session.get(url=URL)
+        except aiohttp.ClientConnectorError as err:
+            raise ReolinkConnectionError(f"Connetion error to {URL}: {str(err)}") from err
+        except asyncio.TimeoutError as err:
+            raise ReolinkTimeoutError(f"Timeout requesting {URL}: {str(err)}") from err
+
+        if response.status != 200:
+            response.release()
+            raise ApiError(f"Request to {URL} returned HTTP status ERROR code {response.status}/{response.reason}")
+
+        if response.content_type != expected_response_type:
+            response.release()
+            raise InvalidContentTypeError(f"Request to {URL}, expected type '{expected_response_type}' but received '{response.content_type}'")
+
+        try:
+            data = await response.text()
+        except aiohttp.ClientConnectorError as err:
+            raise ReolinkConnectionError(f"Connetion error reading response from {URL}: {str(err)}") from err
+        except asyncio.TimeoutError as err:
+            raise ReolinkTimeoutError(f"Timeout reading response from {URL}: {str(err)}") from err
+
+        try:
+            json_data = json.loads(data)
+        except (TypeError, json.JSONDecodeError) as err:
+            raise InvalidContentTypeError(f"Error translating JSON response: {str(err)}, from {URL}, " f"content type '{response.content_type}', data:\n{data}\n") from err
+
+        if json_data is None:
+            raise NoDataError(f"Request to {URL} returned no data: {data}")
+
+        resp_code = json_data.get("result", {}).get("code")
+        if resp_code != 0:
+            raise ApiError(f"Request to {URL} returned error code {resp_code}, data:\n{json_data}")
+
+        return json_data
+
     ##############################################################################
     # SUBSCRIPTION managing
     @property
     def renewtimer(self) -> int:
         """Return the renew time in seconds. Negative if expired."""
         if self._subscription_time_difference is None or self._subscription_termination_time is None:
             return -1
@@ -3642,15 +4020,15 @@
             xml = template.format(**parameters)
             await self.subscription_send(headers, xml, logger=False)
 
         return True
 
     async def ONVIF_event_callback(self, data: str) -> list[int] | None:
         """Handle incoming ONVIF event from the webhook called by the Reolink device."""
-        _LOGGER_DATA.debug("ONVIF event callback received payload:\n%s", data)
+        _LOGGER_DATA.debug("ONVIF event callback from '%s' received payload:\n%s", self.nvr_name, data)
 
         event_channels: list[int] = []
         contains_channels = False
 
         root = XML.fromstring(data)
         for message in root.iter("{http://docs.oasis-open.org/wsn/b-2}NotificationMessage"):
             channel = None
```

### Comparing `reolink_aio-0.5.9/reolink_aio/enums.py` & `reolink_aio-0.6.0/reolink_aio/enums.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.5.9/reolink_aio/software_version.py` & `reolink_aio-0.6.0/reolink_aio/software_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,14 +29,17 @@
         "IPC_515SD6": "v3.0.0.1107_22070508",
     },
     "RLC-410": {
         "IPC-515B16M5M": "V3.0.0.136_20121100",
         "IPC_51316M": "V3.0.0.136_20121100",
         "IPC_51516M5M": "V3.0.0.136_20121100",
     },
+    "RLC-410-5MP": {
+        "IPC_51516M5M": "V3.0.0.136_20121100",
+    },
     "RLC-410W": {
         "IPC_30K128M4MP": "v3.1.0.739_22042505",
         "IPC_51516M5M": "v3.0.0.136_20121102",
         "IPC_515B16M5M": "v3.0.0.136_20121102",
     },
     "RLC-420": {
         "IPC_51316M": "v3.0.0.136_20121101",
@@ -79,14 +82,20 @@
     },
     "RLC-822A": {
         "IPC_523128M8MP": "v3.1.0.989_22081907",
     },
     "RLC-823A": {
         "IPC_523128M8MP": "v3.1.0.989_22051911_v1.0.0.30",
     },
+    "Reolink Video Doorbell PoE": {
+        "DB_566128M5MP_P": "v3.0.0.2033_23041302",
+    },
+    "Reolink Video Doorbell WiFi": {
+        "DB_566128M5MP_W": "v3.0.0.2033_23041300",
+    },
     "Reolink TrackMix PoE": {
         "IPC_529SD78MP": "v3.0.0.1817_23022700",
     },
     "Reolink TrackMix WiFi": {
         "IPC_529SD78MP": "v3.0.0.1817_23022701",
     },
     "Reolink Duo PoE": {
@@ -99,50 +108,56 @@
         "IPC_529B17B8MP": "v3.0.0.1337_22091900",
     },
     "Reolink Duo 2 WiFi": {
         "IPC_529B17B8MP": "v3.0.0.1337_22091901",
     },
 }
 
+DEFAULT_VERSION_DATA = datetime(2000, 1, 1, 0, 0)  # 2000-01-01 00:00
 
 version_regex = re.compile(r"^v(?P<major>[0-9]+)\.(?P<middle>[0-9]+)\.(?P<minor>[0-9]+).(?P<build>[0-9]+)_(?P<date>[0-9]+)")
+version_regex_no_date = re.compile(r"^v(?P<major>[0-9]+)\.(?P<middle>[0-9]+)\.(?P<minor>[0-9]+).(?P<build>[0-9]+)")
 
 
 class SoftwareVersion:
     """SoftwareVersion class"""
 
     def __init__(self, version_string: str | None):
         self.is_unknown = False
         self.major = 0
         self.middle = 0
         self.minor = 0
         self.build = 0
-        self.date = datetime.strptime("00010100", "%y%m%d%H")
+        self.date = DEFAULT_VERSION_DATA
 
         if version_string is None:
             self.is_unknown = True
             return
 
         self.version_string = version_string.lower()
         if self.version_string == "unknown":
             self.is_unknown = True
             return
 
         match = version_regex.match(self.version_string)
-
         if match is None:
-            raise UnexpectedDataError(f"version_string has invalid version format: {version_string}")
+            match = version_regex_no_date.match(self.version_string)
+            if match is None:
+                raise UnexpectedDataError(f"version_string has invalid version format: {version_string}")
 
         self.major = int(match.group("major"))
         self.middle = int(match.group("middle"))
         self.minor = int(match.group("minor"))
         build = match.group("build")
         if build is not None:
             self.build = int(build)
-        date = match.group("date")
+        try:
+            date = match.group("date")
+        except IndexError:
+            date = None
         if date is not None:
             try:
                 self.date = datetime.strptime(date, "%y%m%d%M")
             except ValueError:
                 pass
 
     def __repr__(self):
@@ -158,15 +173,15 @@
                 if self.minor > target_version.minor:
                     return True
                 if target_version.minor == self.minor:
                     if self.build > target_version.build:
                         return True
 
         # for beta firmware releases
-        if self.date > target_version.date:
+        if self.date > target_version.date and self.date != DEFAULT_VERSION_DATA and target_version.date != DEFAULT_VERSION_DATA:
             return True
 
         return False
 
     def is_greater_or_equal_than(self, target_version: "SoftwareVersion"):
         if self.major > target_version.major:
             return True
@@ -177,15 +192,15 @@
                 if self.minor > target_version.minor:
                     return True
                 if target_version.minor == self.minor:
                     if self.build >= target_version.build:
                         return True
 
         # for beta firmware releases
-        if self.date >= target_version.date:
+        if self.date >= target_version.date and self.date != DEFAULT_VERSION_DATA and target_version.date != DEFAULT_VERSION_DATA:
             return True
 
         return False
 
     def is_lower_than(self, target_version: "SoftwareVersion"):
         if self.major < target_version.major:
             return True
@@ -196,15 +211,15 @@
                 if self.minor < target_version.minor:
                     return True
                 if target_version.minor == self.minor:
                     if self.build < target_version.build:
                         return True
 
         # for beta firmware releases
-        if self.date < target_version.date:
+        if self.date < target_version.date and self.date != DEFAULT_VERSION_DATA and target_version.date != DEFAULT_VERSION_DATA:
             return True
 
         return False
 
     def is_lower_or_equal_than(self, target_version: "SoftwareVersion"):
         if self.major < target_version.major:
             return True
@@ -215,15 +230,15 @@
                 if self.minor < target_version.minor:
                     return True
                 if target_version.minor == self.minor:
                     if self.build <= target_version.build:
                         return True
 
         # for beta firmware releases
-        if self.date <= target_version.date:
+        if self.date <= target_version.date and self.date != DEFAULT_VERSION_DATA and target_version.date != DEFAULT_VERSION_DATA:
             return True
 
         return False
 
     def equals(self, target_version: "SoftwareVersion"):
         if (
             target_version.major == self.major
@@ -250,7 +265,17 @@
     def __eq__(self, target_version):
         if target_version.major == self.major and target_version.middle == self.middle and target_version.minor == self.minor and target_version.build == self.build:
             return True
         return False
 
     def generate_str_from_numbers(self):
         return f"{self.major}.{self.middle}.{self.minor}-{self.build}"
+
+
+class NewSoftwareVersion(SoftwareVersion):
+    """SoftwareVersion class for available software updates"""
+
+    def __init__(self, version_string: str | None, download_url: str | None = None, release_notes: str = "", online_update_available: bool = False):
+        self.download_url = download_url
+        self.release_notes = release_notes
+        self.online_update_available = online_update_available
+        super().__init__(version_string)
```

### Comparing `reolink_aio-0.5.9/reolink_aio/templates.py` & `reolink_aio-0.6.0/reolink_aio/templates.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.5.9/reolink_aio.egg-info/PKG-INFO` & `reolink_aio-0.6.0/reolink_aio.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7265 6f6c  : 2.1.Name: reol
 00000020: 696e 6b2d 6169 6f0a 5665 7273 696f 6e3a  ink-aio.Version:
-00000030: 2030 2e35 2e39 0a53 756d 6d61 7279 3a20   0.5.9.Summary: 
+00000030: 2030 2e36 2e30 0a53 756d 6d61 7279 3a20   0.6.0.Summary: 
 00000040: 5265 6f6c 696e 6b20 4e56 522f 6361 6d65  Reolink NVR/came
 00000050: 7261 7320 4150 4920 7061 636b 6167 650a  ras API package.
 00000060: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
 00000070: 3a2f 2f67 6974 6875 622e 636f 6d2f 7374  ://github.com/st
 00000080: 6172 6b69 6c6c 6572 4f47 2f72 656f 6c69  arkillerOG/reoli
 00000090: 6e6b 5f61 696f 0a41 7574 686f 723a 2073  nk_aio.Author: s
 000000a0: 7461 726b 696c 6c65 724f 470a 4175 7468  tarkillerOG.Auth
@@ -71,188 +71,216 @@
 00000460: 6869 656c 6473 2e69 6f2f 7374 6174 6963  hields.io/static
 00000470: 2f76 313f 6c61 6265 6c3d 5370 6f6e 736f  /v1?label=Sponso
 00000480: 7226 6d65 7373 6167 653d 2545 3225 3944  r&message=%E2%9D
 00000490: 2541 3426 6c6f 676f 3d47 6974 4875 6226  %A4&logo=GitHub&
 000004a0: 636f 6c6f 723d 2532 3366 6538 6538 3622  color=%23fe8e86"
 000004b0: 2061 6c74 3d22 5370 6f6e 736f 7222 3e3c   alt="Sponsor"><
 000004c0: 2f61 3e0a 2020 3c61 2068 7265 663d 2268  /a>.  <a href="h
-000004d0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-000004e0: 7072 6f6a 6563 742f 7265 6f6c 696e 6b2d  project/reolink-
-000004f0: 6169 6f22 3e3c 696d 6720 7372 633d 2268  aio"><img src="h
-00000500: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000510: 6473 2e69 6f2f 7079 7069 2f64 6d2f 7265  ds.io/pypi/dm/re
-00000520: 6f6c 696e 6b2d 6169 6f22 3e3c 2f61 3e0a  olink-aio"></a>.
-00000530: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000540: 3a2f 2f67 6974 6875 622e 636f 6d2f 7374  ://github.com/st
-00000550: 6172 6b69 6c6c 6572 4f47 2f72 656f 6c69  arkillerOG/reoli
-00000560: 6e6b 5f61 696f 2f72 656c 6561 7365 7322  nk_aio/releases"
-00000570: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00000580: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000590: 6f2f 6769 7468 7562 2f76 2f72 656c 6561  o/github/v/relea
-000005a0: 7365 2f53 7461 726b 696c 6c65 724f 472f  se/StarkillerOG/
-000005b0: 7265 6f6c 696e 6b5f 6169 6f3f 6469 7370  reolink_aio?disp
-000005c0: 6c61 795f 6e61 6d65 3d74 6167 2669 6e63  lay_name=tag&inc
-000005d0: 6c75 6465 5f70 7265 7265 6c65 6173 6573  lude_prereleases
-000005e0: 2673 6f72 743d 7365 6d76 6572 2220 616c  &sort=semver" al
-000005f0: 743d 2243 7572 7265 6e74 2076 6572 7369  t="Current versi
-00000600: 6f6e 223e 3c2f 613e 0a3c 2f70 3e0a 0a54  on"></a>.</p>..T
-00000610: 6865 2060 7265 6f6c 696e 6b5f 6169 6f60  he `reolink_aio`
-00000620: 2050 7974 686f 6e20 7061 636b 6167 6520   Python package 
-00000630: 616c 6c6f 7773 2079 6f75 2074 6f20 696e  allows you to in
-00000640: 7465 6772 6174 6520 796f 7572 205b 5265  tegrate your [Re
-00000650: 6f6c 696e 6b5d 2868 7474 7073 3a2f 2f77  olink](https://w
-00000660: 7777 2e72 656f 6c69 6e6b 2e63 6f6d 2f29  ww.reolink.com/)
-00000670: 2064 6576 6963 6573 2028 4e56 522f 6361   devices (NVR/ca
-00000680: 6d65 7261 7329 2069 6e20 796f 7572 2061  meras) in your a
-00000690: 7070 6c69 6361 7469 6f6e 2e0a 0a23 2323  pplication...###
-000006a0: 2044 6573 6372 6970 7469 6f6e 0a0a 5468   Description..Th
-000006b0: 6973 2069 7320 6120 7061 636b 6167 6520  is is a package 
-000006c0: 696d 706c 656d 656e 7469 6e67 2052 656f  implementing Reo
-000006d0: 6c69 6e6b 2049 5020 4e56 5220 616e 6420  link IP NVR and 
-000006e0: 6361 6d65 7261 2041 5049 2e20 416c 736f  camera API. Also
-000006f0: 2069 74e2 8099 7320 7072 6f76 6964 696e   it...s providin
-00000700: 6720 6120 7761 7920 746f 2073 7562 7363  g a way to subsc
-00000710: 7269 6265 2074 6f20 5265 6f6c 696e 6b20  ribe to Reolink 
-00000720: 4f4e 5649 4620 5357 4e20 6576 656e 7473  ONVIF SWN events
-00000730: 2c20 736f 2074 6861 7420 7265 616c 2d74  , so that real-t
-00000740: 696d 6520 6576 656e 7473 2063 616e 2062  ime events can b
-00000750: 6520 7265 6365 6976 6564 206f 6e20 6120  e received on a 
-00000760: 7765 6268 6f6f 6b2e 0a0a 2323 2320 5072  webhook...### Pr
-00000770: 6572 6571 7569 7369 7465 730a 0a2d 2050  erequisites..- P
-00000780: 7974 686f 6e20 332e 390a 0a23 2323 2049  ython 3.9..### I
-00000790: 6e73 7461 6c6c 6174 696f 6e0a 0a60 6060  nstallation..```
-000007a0: 0a70 6970 3320 696e 7374 616c 6c20 7265  .pip3 install re
-000007b0: 6f6c 696e 6b2d 6169 6f0a 6060 600a 0a6f  olink-aio.```..o
-000007c0: 7220 6d61 6e75 616c 6c79 3a0a 6060 6060  r manually:.````
-000007d0: 0a67 6974 2063 6c6f 6e65 2068 7474 7073  .git clone https
-000007e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5374  ://github.com/St
-000007f0: 6172 6b69 6c6c 6572 4f47 2f72 656f 6c69  arkillerOG/reoli
-00000800: 6e6b 5f61 696f 0a63 6420 7265 6f6c 696e  nk_aio.cd reolin
-00000810: 6b5f 6169 6f2f 0a70 6970 3320 696e 7374  k_aio/.pip3 inst
-00000820: 616c 6c20 2e0a 6060 6060 0a0a 2323 2320  all ..````..### 
-00000830: 5573 6167 650a 0a60 6060 600a 6672 6f6d  Usage..````.from
-00000840: 2072 656f 6c69 6e6b 5f61 696f 2e61 7069   reolink_aio.api
-00000850: 2069 6d70 6f72 7420 486f 7374 0a69 6d70   import Host.imp
-00000860: 6f72 7420 6173 796e 6369 6f0a 0a23 2043  ort asyncio..# C
-00000870: 7265 6174 6520 6120 686f 7374 2d6f 626a  reate a host-obj
-00000880: 6563 7420 2872 6570 7265 7365 6e74 696e  ect (representin
-00000890: 6720 6569 7468 6572 2061 2063 616d 6572  g either a camer
-000008a0: 612c 206f 7220 4e56 5220 7769 7468 2073  a, or NVR with s
-000008b0: 6576 6572 616c 2063 6861 6e6e 656c 7329  everal channels)
-000008c0: 0a68 6f73 7420 3d20 486f 7374 2827 3139  .host = Host('19
-000008d0: 322e 3136 382e 312e 3130 272c 2038 302c  2.168.1.10', 80,
-000008e0: 2027 7573 6572 272c 2027 6d79 7061 7373   'user', 'mypass
-000008f0: 776f 7264 2729 0a0a 2320 4f62 7461 696e  word')..# Obtain
-00000900: 2f63 6163 6865 204e 5652 206f 7220 6361  /cache NVR or ca
-00000910: 6d65 7261 2073 6574 7469 6e67 7320 616e  mera settings an
-00000920: 6420 6361 7061 6269 6c69 7469 6573 2c20  d capabilities, 
-00000930: 6c69 6b65 206d 6f64 656c 206e 616d 652c  like model name,
-00000940: 2070 6f72 7473 2c20 4844 4420 7369 7a65   ports, HDD size
-00000950: 2c20 6574 633a 0a61 7761 6974 2068 6f73  , etc:.await hos
-00000960: 742e 6765 745f 686f 7374 5f64 6174 6128  t.get_host_data(
-00000970: 290a 0a23 2047 6574 2074 6865 2073 7562  )..# Get the sub
-00000980: 7363 7269 6274 696f 6e20 706f 7274 2061  scribtion port a
-00000990: 6e64 2068 6f73 742d 6465 7669 6365 206e  nd host-device n
-000009a0: 616d 653a 0a73 7562 7363 7269 6274 696f  ame:.subscribtio
-000009b0: 6e5f 706f 7274 203d 2020 686f 7374 2e6f  n_port =  host.o
-000009c0: 6e76 6966 5f70 6f72 740a 6e61 6d65 203d  nvif_port.name =
-000009d0: 2068 6f73 742e 6e76 725f 6e61 6d65 0a0a   host.nvr_name..
-000009e0: 2320 4f62 7461 696e 2f63 6163 6865 2073  # Obtain/cache s
-000009f0: 7461 7465 7320 6f66 2066 6561 7475 7265  tates of feature
-00000a00: 733a 0a61 7761 6974 2068 6f73 742e 6765  s:.await host.ge
-00000a10: 745f 7374 6174 6573 2829 0a0a 2320 5072  t_states()..# Pr
-00000a20: 696e 7420 736f 6d65 2073 7461 7465 2076  int some state v
-00000a30: 616c 7565 206f 6e20 7468 6520 6368 616e  alue on the chan
-00000a40: 6e65 6c20 7769 7468 2069 6e64 6578 2030  nel with index 0
-00000a50: 3a0a 7072 696e 7428 686f 7374 2e69 725f  :.print(host.ir_
-00000a60: 656e 6162 6c65 6428 3029 290a 0a23 2045  enabled(0))..# E
-00000a70: 6e61 626c 6520 7468 6520 696e 6672 6172  nable the infrar
-00000a80: 6564 206c 6967 6874 7320 6f6e 2074 6865  ed lights on the
-00000a90: 2063 6861 6e6e 656c 2077 6974 6820 696e   channel with in
-00000aa0: 6465 7820 313a 0a61 7761 6974 2068 6f73  dex 1:.await hos
-00000ab0: 742e 7365 745f 6972 5f6c 6967 6874 7328  t.set_ir_lights(
-00000ac0: 312c 2054 7275 6529 0a0a 2320 456e 6162  1, True)..# Enab
-00000ad0: 6c65 2074 6865 2073 706f 746c 6967 6874  le the spotlight
-00000ae0: 206f 6e20 7468 6520 6368 616e 6e65 6c20   on the channel 
-00000af0: 7769 7468 2069 6e64 6578 2031 3a0a 6177  with index 1:.aw
-00000b00: 6169 7420 686f 7374 2e73 6574 5f73 706f  ait host.set_spo
-00000b10: 746c 6967 6874 2831 2c20 5472 7565 290a  tlight(1, True).
-00000b20: 0a23 2045 6e61 626c 6520 7468 6520 7369  .# Enable the si
-00000b30: 7265 6e20 6f6e 2074 6865 2063 6861 6e6e  ren on the chann
-00000b40: 656c 2077 6974 6820 696e 6465 7820 303a  el with index 0:
-00000b50: 0a61 7761 6974 2068 6f73 742e 7365 745f  .await host.set_
-00000b60: 7369 7265 6e28 302c 2054 7275 6529 0a0a  siren(0, True)..
-00000b70: 2320 4e6f 7720 7375 6273 6372 6962 6520  # Now subscribe 
-00000b80: 746f 2065 7665 6e74 732c 2073 7570 706f  to events, suppo
-00000b90: 7365 206f 7572 2077 6562 686f 6f6b 2075  se our webhook u
-00000ba0: 726c 2069 7320 6874 7470 3a2f 2f31 3932  rl is http://192
-00000bb0: 2e31 3638 2e31 2e31 312f 7765 6268 6f6f  .168.1.11/webhoo
-00000bc0: 6b31 3233 0a61 7761 6974 2068 6f73 742e  k123.await host.
-00000bd0: 7375 6273 6372 6962 6528 2768 7474 703a  subscribe('http:
-00000be0: 2f2f 3139 322e 3136 382e 312e 3131 2f77  //192.168.1.11/w
-00000bf0: 6562 686f 6f6b 3132 3327 290a 0a23 2041  ebhook123')..# A
-00000c00: 6674 6572 2073 6f6d 6520 6d69 6e75 7465  fter some minute
-00000c10: 7320 6368 6563 6b20 7468 6520 7265 6e65  s check the rene
-00000c20: 7720 7469 6d65 7220 286b 6565 7020 7468  w timer (keep th
-00000c30: 6520 6576 656e 7469 6e67 2061 6c69 7665  e eventing alive
-00000c40: 293a 0a69 6620 2868 6f73 742e 7265 6e65  ):.if (host.rene
-00000c50: 7754 696d 6572 203c 3d20 3130 3029 3a0a  wTimer <= 100):.
-00000c60: 2020 2020 6177 6169 7420 686f 7374 2e72      await host.r
-00000c70: 656e 6577 2829 0a0a 2320 4c6f 676f 7574  enew()..# Logout
-00000c80: 2061 6e64 2064 6973 636f 6e6e 6563 740a   and disconnect.
-00000c90: 6177 6169 7420 686f 7374 2e64 6973 636f  await host.disco
-00000ca0: 6e6e 6563 7428 290a 6060 6060 0a0a 2323  nnect().````..##
-00000cb0: 2320 4578 616d 706c 650a 0a54 6869 7320  # Example..This 
-00000cc0: 6973 2061 6e20 6578 616d 706c 6520 6f66  is an example of
-00000cd0: 2074 6865 2075 7361 6765 206f 6620 7468   the usage of th
-00000ce0: 6520 4150 492e 2049 6e20 7468 6973 2063  e API. In this c
-00000cf0: 6173 6520 7765 2077 616e 7420 746f 2072  ase we want to r
-00000d00: 6574 7269 7665 2061 6e64 2070 7269 6e74  etrive and print
-00000d10: 2074 6865 204d 6163 2041 6464 7265 7373   the Mac Address
-00000d20: 206f 6620 7468 6520 4e56 522e 0a60 6060   of the NVR..```
-00000d30: 600a 6672 6f6d 2072 656f 6c69 6e6b 5f61  `.from reolink_a
-00000d40: 696f 2e61 7069 2069 6d70 6f72 7420 486f  io.api import Ho
-00000d50: 7374 0a69 6d70 6f72 7420 6173 796e 6369  st.import asynci
-00000d60: 6f0a 0a61 7379 6e63 2064 6566 2070 7269  o..async def pri
-00000d70: 6e74 5f6d 6163 5f61 6464 7265 7373 2829  nt_mac_address()
-00000d80: 3a0a 2020 2020 2320 696e 6974 6961 6c69  :.    # initiali
-00000d90: 7a65 2074 6865 2068 6f73 740a 2020 2020  ze the host.    
-00000da0: 686f 7374 203d 2048 6f73 7428 2731 3932  host = Host('192
-00000db0: 2e31 3638 2e31 2e31 3039 272c 2761 646d  .168.1.109','adm
-00000dc0: 696e 272c 2027 6164 6d69 6e31 3233 3427  in', 'admin1234'
-00000dd0: 2c20 706f 7274 3d38 3029 0a20 2020 2023  , port=80).    #
-00000de0: 2063 6f6e 6e65 6374 2061 6e64 206f 6274   connect and obt
-00000df0: 6169 6e2f 6361 6368 6520 6465 7669 6365  ain/cache device
-00000e00: 2073 6574 7469 6e67 7320 616e 6420 6361   settings and ca
-00000e10: 7061 6269 6c69 7469 6573 0a20 2020 2061  pabilities.    a
-00000e20: 7761 6974 2068 6f73 742e 6765 745f 686f  wait host.get_ho
-00000e30: 7374 5f64 6174 6128 290a 2020 2020 2320  st_data().    # 
-00000e40: 6368 6563 6b20 6966 2069 7420 6973 2061  check if it is a
-00000e50: 2063 616d 6572 6120 6f72 2061 6e20 4e56   camera or an NV
-00000e60: 520a 2020 2020 7072 696e 7428 2249 7420  R.    print("It 
-00000e70: 6973 2061 6e20 4e56 523a 2025 732c 206e  is an NVR: %s, n
-00000e80: 756d 6265 7220 6f66 2063 6861 6e6e 656c  umber of channel
-00000e90: 733a 2025 7322 2c20 686f 7374 2e69 735f  s: %s", host.is_
-00000ea0: 6e76 722c 2068 6f73 742e 6e75 6d5f 6368  nvr, host.num_ch
-00000eb0: 616e 6e65 6c73 290a 2020 2020 2320 7072  annels).    # pr
-00000ec0: 696e 7420 6d61 6320 6164 6472 6573 730a  int mac address.
-00000ed0: 2020 2020 7072 696e 7428 686f 7374 2e6d      print(host.m
-00000ee0: 6163 5f61 6464 7265 7373 290a 2020 2020  ac_address).    
-00000ef0: 2320 636c 6f73 6520 7468 6520 6465 7669  # close the devi
-00000f00: 6365 2063 6f6e 6e65 6374 696f 6e0a 2020  ce connection.  
-00000f10: 2020 6177 6169 7420 686f 7374 2e6c 6f67    await host.log
-00000f20: 6f75 7428 290a 0a69 6620 5f5f 6e61 6d65  out()..if __name
-00000f30: 5f5f 203d 3d20 225f 5f6d 6169 6e5f 5f22  __ == "__main__"
-00000f40: 3a0a 2020 2020 6173 796e 6369 6f2e 7275  :.    asyncio.ru
-00000f50: 6e28 7072 696e 745f 6d61 635f 6164 6472  n(print_mac_addr
-00000f60: 6573 7328 2929 0a60 6060 600a 0a23 2323  ess()).````..###
-00000f70: 2041 636b 6e6f 776c 6564 676d 656e 740a   Acknowledgment.
-00000f80: 5468 6973 206c 6962 7261 7279 2069 7320  This library is 
-00000f90: 6261 7365 6420 6f6e 2074 6865 2077 6f72  based on the wor
-00000fa0: 6b20 6f66 3a0a 2d20 6677 6573 7465 6e62  k of:.- fwestenb
-00000fb0: 6572 673a 2068 7474 7073 3a2f 2f67 6974  erg: https://git
-00000fc0: 6875 622e 636f 6d2f 6677 6573 7465 6e62  hub.com/fwestenb
-00000fd0: 6572 672f 7265 6f6c 696e 6b5f 6465 760a  erg/reolink_dev.
-00000fe0: 2d20 4a69 6d53 7461 723a 2068 7474 7073  - JimStar: https
-00000ff0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a69  ://github.com/Ji
-00001000: 6d53 7461 722f 7265 6f6c 696e 6b5f 6970  mStar/reolink_ip
-00001010: 0a                                       .
+000004d0: 7474 7073 3a2f 2f72 656f 6c69 6e6b 2e70  ttps://reolink.p
+000004e0: 7866 2e69 6f2f 7134 3451 5771 223e 3c69  xf.io/q44QWq"><i
+000004f0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000500: 696d 672e 7368 6965 6c64 732e 696f 2f73  img.shields.io/s
+00000510: 7461 7469 632f 7631 3f6c 6162 656c 3d41  tatic/v1?label=A
+00000520: 6666 696c 6961 7465 206c 696e 6b26 6d65  ffiliate link&me
+00000530: 7373 6167 653d 2545 3225 3944 2541 3426  ssage=%E2%9D%A4&
+00000540: 636f 6c6f 723d 2532 3366 6538 6538 3622  color=%23fe8e86"
+00000550: 2061 6c74 3d22 4166 6669 6c69 6174 6520   alt="Affiliate 
+00000560: 6c69 6e6b 223e 3c2f 613e 0a20 203c 6120  link"></a>.  <a 
+00000570: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00000580: 7069 2e6f 7267 2f70 726f 6a65 6374 2f72  pi.org/project/r
+00000590: 656f 6c69 6e6b 2d61 696f 223e 3c69 6d67  eolink-aio"><img
+000005a0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+000005b0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+000005c0: 692f 646d 2f72 656f 6c69 6e6b 2d61 696f  i/dm/reolink-aio
+000005d0: 223e 3c2f 613e 0a20 203c 6120 6872 6566  "></a>.  <a href
+000005e0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+000005f0: 2e63 6f6d 2f73 7461 726b 696c 6c65 724f  .com/starkillerO
+00000600: 472f 7265 6f6c 696e 6b5f 6169 6f2f 7265  G/reolink_aio/re
+00000610: 6c65 6173 6573 223e 3c69 6d67 2073 7263  leases"><img src
+00000620: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000630: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000640: 762f 7265 6c65 6173 652f 5374 6172 6b69  v/release/Starki
+00000650: 6c6c 6572 4f47 2f72 656f 6c69 6e6b 5f61  llerOG/reolink_a
+00000660: 696f 3f64 6973 706c 6179 5f6e 616d 653d  io?display_name=
+00000670: 7461 6726 696e 636c 7564 655f 7072 6572  tag&include_prer
+00000680: 656c 6561 7365 7326 736f 7274 3d73 656d  eleases&sort=sem
+00000690: 7665 7222 2061 6c74 3d22 4375 7272 656e  ver" alt="Curren
+000006a0: 7420 7665 7273 696f 6e22 3e3c 2f61 3e0a  t version"></a>.
+000006b0: 3c2f 703e 0a0a 5468 6520 6072 656f 6c69  </p>..The `reoli
+000006c0: 6e6b 5f61 696f 6020 5079 7468 6f6e 2070  nk_aio` Python p
+000006d0: 6163 6b61 6765 2061 6c6c 6f77 7320 796f  ackage allows yo
+000006e0: 7520 746f 2069 6e74 6567 7261 7465 2079  u to integrate y
+000006f0: 6f75 7220 5b52 656f 6c69 6e6b 5d28 6874  our [Reolink](ht
+00000700: 7470 733a 2f2f 7777 772e 7265 6f6c 696e  tps://www.reolin
+00000710: 6b2e 636f 6d2f 2920 6465 7669 6365 7320  k.com/) devices 
+00000720: 284e 5652 2f63 616d 6572 6173 2920 696e  (NVR/cameras) in
+00000730: 2079 6f75 7220 6170 706c 6963 6174 696f   your applicatio
+00000740: 6e2e 0a0a 2323 2320 4465 7363 7269 7074  n...### Descript
+00000750: 696f 6e0a 0a54 6869 7320 6973 2061 2070  ion..This is a p
+00000760: 6163 6b61 6765 2069 6d70 6c65 6d65 6e74  ackage implement
+00000770: 696e 6720 5265 6f6c 696e 6b20 4950 204e  ing Reolink IP N
+00000780: 5652 2061 6e64 2063 616d 6572 6120 4150  VR and camera AP
+00000790: 492e 2041 6c73 6f20 6974 e280 9973 2070  I. Also it...s p
+000007a0: 726f 7669 6469 6e67 2061 2077 6179 2074  roviding a way t
+000007b0: 6f20 7375 6273 6372 6962 6520 746f 2052  o subscribe to R
+000007c0: 656f 6c69 6e6b 204f 4e56 4946 2053 574e  eolink ONVIF SWN
+000007d0: 2065 7665 6e74 732c 2073 6f20 7468 6174   events, so that
+000007e0: 2072 6561 6c2d 7469 6d65 2065 7665 6e74   real-time event
+000007f0: 7320 6361 6e20 6265 2072 6563 6569 7665  s can be receive
+00000800: 6420 6f6e 2061 2077 6562 686f 6f6b 2e0a  d on a webhook..
+00000810: 0a23 2323 2053 686f 7720 796f 7572 2061  .### Show your a
+00000820: 7070 7265 6369 6174 696f 6e0a 0a49 6620  ppreciation..If 
+00000830: 796f 7520 6170 7072 6563 6961 7465 2074  you appreciate t
+00000840: 6865 2072 656f 6c69 6e6b 2069 6e74 6567  he reolink integ
+00000850: 7261 7469 6f6e 2061 6e64 2077 616e 7420  ration and want 
+00000860: 746f 2073 7570 706f 7274 2069 7473 2064  to support its d
+00000870: 6576 656c 6f70 6d65 6e74 2c20 706c 6561  evelopment, plea
+00000880: 7365 2063 6f6e 7369 6465 7220 5b73 706f  se consider [spo
+00000890: 6e73 6572 696e 675d 2868 7474 7073 3a2f  nsering](https:/
+000008a0: 2f67 6974 6875 622e 636f 6d2f 7370 6f6e  /github.com/spon
+000008b0: 736f 7273 2f73 7461 726b 696c 6c65 724f  sors/starkillerO
+000008c0: 4729 2074 6865 2075 7073 7472 6561 6d20  G) the upstream 
+000008d0: 6c69 6272 6172 7920 6f72 2070 7572 6368  library or purch
+000008e0: 6173 6520 5265 6f6c 696e 6b20 7072 6f64  ase Reolink prod
+000008f0: 7563 7473 2074 6872 6f75 6768 205b 7468  ucts through [th
+00000900: 6973 2061 6666 696c 6961 7465 206c 696e  is affiliate lin
+00000910: 6b5d 2868 7474 7073 3a2f 2f72 656f 6c69  k](https://reoli
+00000920: 6e6b 2e70 7866 2e69 6f2f 7134 3451 5771  nk.pxf.io/q44QWq
+00000930: 292e 0a0a 2323 2320 5072 6572 6571 7569  )...### Prerequi
+00000940: 7369 7465 730a 0a2d 2050 7974 686f 6e20  sites..- Python 
+00000950: 332e 390a 0a23 2323 2049 6e73 7461 6c6c  3.9..### Install
+00000960: 6174 696f 6e0a 0a60 6060 0a70 6970 3320  ation..```.pip3 
+00000970: 696e 7374 616c 6c20 7265 6f6c 696e 6b2d  install reolink-
+00000980: 6169 6f0a 6060 600a 0a6f 7220 6d61 6e75  aio.```..or manu
+00000990: 616c 6c79 3a0a 6060 6060 0a67 6974 2063  ally:.````.git c
+000009a0: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+000009b0: 6875 622e 636f 6d2f 5374 6172 6b69 6c6c  hub.com/Starkill
+000009c0: 6572 4f47 2f72 656f 6c69 6e6b 5f61 696f  erOG/reolink_aio
+000009d0: 0a63 6420 7265 6f6c 696e 6b5f 6169 6f2f  .cd reolink_aio/
+000009e0: 0a70 6970 3320 696e 7374 616c 6c20 2e0a  .pip3 install ..
+000009f0: 6060 6060 0a0a 2323 2320 5573 6167 650a  ````..### Usage.
+00000a00: 0a60 6060 600a 6672 6f6d 2072 656f 6c69  .````.from reoli
+00000a10: 6e6b 5f61 696f 2e61 7069 2069 6d70 6f72  nk_aio.api impor
+00000a20: 7420 486f 7374 0a69 6d70 6f72 7420 6173  t Host.import as
+00000a30: 796e 6369 6f0a 0a23 2043 7265 6174 6520  yncio..# Create 
+00000a40: 6120 686f 7374 2d6f 626a 6563 7420 2872  a host-object (r
+00000a50: 6570 7265 7365 6e74 696e 6720 6569 7468  epresenting eith
+00000a60: 6572 2061 2063 616d 6572 612c 206f 7220  er a camera, or 
+00000a70: 4e56 5220 7769 7468 2073 6576 6572 616c  NVR with several
+00000a80: 2063 6861 6e6e 656c 7329 0a68 6f73 7420   channels).host 
+00000a90: 3d20 486f 7374 2827 3139 322e 3136 382e  = Host('192.168.
+00000aa0: 312e 3130 272c 2038 302c 2027 7573 6572  1.10', 80, 'user
+00000ab0: 272c 2027 6d79 7061 7373 776f 7264 2729  ', 'mypassword')
+00000ac0: 0a0a 2320 4f62 7461 696e 2f63 6163 6865  ..# Obtain/cache
+00000ad0: 204e 5652 206f 7220 6361 6d65 7261 2073   NVR or camera s
+00000ae0: 6574 7469 6e67 7320 616e 6420 6361 7061  ettings and capa
+00000af0: 6269 6c69 7469 6573 2c20 6c69 6b65 206d  bilities, like m
+00000b00: 6f64 656c 206e 616d 652c 2070 6f72 7473  odel name, ports
+00000b10: 2c20 4844 4420 7369 7a65 2c20 6574 633a  , HDD size, etc:
+00000b20: 0a61 7761 6974 2068 6f73 742e 6765 745f  .await host.get_
+00000b30: 686f 7374 5f64 6174 6128 290a 0a23 2047  host_data()..# G
+00000b40: 6574 2074 6865 2073 7562 7363 7269 6274  et the subscribt
+00000b50: 696f 6e20 706f 7274 2061 6e64 2068 6f73  ion port and hos
+00000b60: 742d 6465 7669 6365 206e 616d 653a 0a73  t-device name:.s
+00000b70: 7562 7363 7269 6274 696f 6e5f 706f 7274  ubscribtion_port
+00000b80: 203d 2020 686f 7374 2e6f 6e76 6966 5f70   =  host.onvif_p
+00000b90: 6f72 740a 6e61 6d65 203d 2068 6f73 742e  ort.name = host.
+00000ba0: 6e76 725f 6e61 6d65 0a0a 2320 4f62 7461  nvr_name..# Obta
+00000bb0: 696e 2f63 6163 6865 2073 7461 7465 7320  in/cache states 
+00000bc0: 6f66 2066 6561 7475 7265 733a 0a61 7761  of features:.awa
+00000bd0: 6974 2068 6f73 742e 6765 745f 7374 6174  it host.get_stat
+00000be0: 6573 2829 0a0a 2320 5072 696e 7420 736f  es()..# Print so
+00000bf0: 6d65 2073 7461 7465 2076 616c 7565 206f  me state value o
+00000c00: 6e20 7468 6520 6368 616e 6e65 6c20 7769  n the channel wi
+00000c10: 7468 2069 6e64 6578 2030 3a0a 7072 696e  th index 0:.prin
+00000c20: 7428 686f 7374 2e69 725f 656e 6162 6c65  t(host.ir_enable
+00000c30: 6428 3029 290a 0a23 2045 6e61 626c 6520  d(0))..# Enable 
+00000c40: 7468 6520 696e 6672 6172 6564 206c 6967  the infrared lig
+00000c50: 6874 7320 6f6e 2074 6865 2063 6861 6e6e  hts on the chann
+00000c60: 656c 2077 6974 6820 696e 6465 7820 313a  el with index 1:
+00000c70: 0a61 7761 6974 2068 6f73 742e 7365 745f  .await host.set_
+00000c80: 6972 5f6c 6967 6874 7328 312c 2054 7275  ir_lights(1, Tru
+00000c90: 6529 0a0a 2320 456e 6162 6c65 2074 6865  e)..# Enable the
+00000ca0: 2073 706f 746c 6967 6874 206f 6e20 7468   spotlight on th
+00000cb0: 6520 6368 616e 6e65 6c20 7769 7468 2069  e channel with i
+00000cc0: 6e64 6578 2031 3a0a 6177 6169 7420 686f  ndex 1:.await ho
+00000cd0: 7374 2e73 6574 5f73 706f 746c 6967 6874  st.set_spotlight
+00000ce0: 2831 2c20 5472 7565 290a 0a23 2045 6e61  (1, True)..# Ena
+00000cf0: 626c 6520 7468 6520 7369 7265 6e20 6f6e  ble the siren on
+00000d00: 2074 6865 2063 6861 6e6e 656c 2077 6974   the channel wit
+00000d10: 6820 696e 6465 7820 303a 0a61 7761 6974  h index 0:.await
+00000d20: 2068 6f73 742e 7365 745f 7369 7265 6e28   host.set_siren(
+00000d30: 302c 2054 7275 6529 0a0a 2320 4e6f 7720  0, True)..# Now 
+00000d40: 7375 6273 6372 6962 6520 746f 2065 7665  subscribe to eve
+00000d50: 6e74 732c 2073 7570 706f 7365 206f 7572  nts, suppose our
+00000d60: 2077 6562 686f 6f6b 2075 726c 2069 7320   webhook url is 
+00000d70: 6874 7470 3a2f 2f31 3932 2e31 3638 2e31  http://192.168.1
+00000d80: 2e31 312f 7765 6268 6f6f 6b31 3233 0a61  .11/webhook123.a
+00000d90: 7761 6974 2068 6f73 742e 7375 6273 6372  wait host.subscr
+00000da0: 6962 6528 2768 7474 703a 2f2f 3139 322e  ibe('http://192.
+00000db0: 3136 382e 312e 3131 2f77 6562 686f 6f6b  168.1.11/webhook
+00000dc0: 3132 3327 290a 0a23 2041 6674 6572 2073  123')..# After s
+00000dd0: 6f6d 6520 6d69 6e75 7465 7320 6368 6563  ome minutes chec
+00000de0: 6b20 7468 6520 7265 6e65 7720 7469 6d65  k the renew time
+00000df0: 7220 286b 6565 7020 7468 6520 6576 656e  r (keep the even
+00000e00: 7469 6e67 2061 6c69 7665 293a 0a69 6620  ting alive):.if 
+00000e10: 2868 6f73 742e 7265 6e65 7754 696d 6572  (host.renewTimer
+00000e20: 203c 3d20 3130 3029 3a0a 2020 2020 6177   <= 100):.    aw
+00000e30: 6169 7420 686f 7374 2e72 656e 6577 2829  ait host.renew()
+00000e40: 0a0a 2320 4c6f 676f 7574 2061 6e64 2064  ..# Logout and d
+00000e50: 6973 636f 6e6e 6563 740a 6177 6169 7420  isconnect.await 
+00000e60: 686f 7374 2e64 6973 636f 6e6e 6563 7428  host.disconnect(
+00000e70: 290a 6060 6060 0a0a 2323 2320 4578 616d  ).````..### Exam
+00000e80: 706c 650a 0a54 6869 7320 6973 2061 6e20  ple..This is an 
+00000e90: 6578 616d 706c 6520 6f66 2074 6865 2075  example of the u
+00000ea0: 7361 6765 206f 6620 7468 6520 4150 492e  sage of the API.
+00000eb0: 2049 6e20 7468 6973 2063 6173 6520 7765   In this case we
+00000ec0: 2077 616e 7420 746f 2072 6574 7269 7665   want to retrive
+00000ed0: 2061 6e64 2070 7269 6e74 2074 6865 204d   and print the M
+00000ee0: 6163 2041 6464 7265 7373 206f 6620 7468  ac Address of th
+00000ef0: 6520 4e56 522e 0a60 6060 600a 6672 6f6d  e NVR..````.from
+00000f00: 2072 656f 6c69 6e6b 5f61 696f 2e61 7069   reolink_aio.api
+00000f10: 2069 6d70 6f72 7420 486f 7374 0a69 6d70   import Host.imp
+00000f20: 6f72 7420 6173 796e 6369 6f0a 0a61 7379  ort asyncio..asy
+00000f30: 6e63 2064 6566 2070 7269 6e74 5f6d 6163  nc def print_mac
+00000f40: 5f61 6464 7265 7373 2829 3a0a 2020 2020  _address():.    
+00000f50: 2320 696e 6974 6961 6c69 7a65 2074 6865  # initialize the
+00000f60: 2068 6f73 740a 2020 2020 686f 7374 203d   host.    host =
+00000f70: 2048 6f73 7428 2731 3932 2e31 3638 2e31   Host('192.168.1
+00000f80: 2e31 3039 272c 2761 646d 696e 272c 2027  .109','admin', '
+00000f90: 6164 6d69 6e31 3233 3427 2c20 706f 7274  admin1234', port
+00000fa0: 3d38 3029 0a20 2020 2023 2063 6f6e 6e65  =80).    # conne
+00000fb0: 6374 2061 6e64 206f 6274 6169 6e2f 6361  ct and obtain/ca
+00000fc0: 6368 6520 6465 7669 6365 2073 6574 7469  che device setti
+00000fd0: 6e67 7320 616e 6420 6361 7061 6269 6c69  ngs and capabili
+00000fe0: 7469 6573 0a20 2020 2061 7761 6974 2068  ties.    await h
+00000ff0: 6f73 742e 6765 745f 686f 7374 5f64 6174  ost.get_host_dat
+00001000: 6128 290a 2020 2020 2320 6368 6563 6b20  a().    # check 
+00001010: 6966 2069 7420 6973 2061 2063 616d 6572  if it is a camer
+00001020: 6120 6f72 2061 6e20 4e56 520a 2020 2020  a or an NVR.    
+00001030: 7072 696e 7428 2249 7420 6973 2061 6e20  print("It is an 
+00001040: 4e56 523a 2025 732c 206e 756d 6265 7220  NVR: %s, number 
+00001050: 6f66 2063 6861 6e6e 656c 733a 2025 7322  of channels: %s"
+00001060: 2c20 686f 7374 2e69 735f 6e76 722c 2068  , host.is_nvr, h
+00001070: 6f73 742e 6e75 6d5f 6368 616e 6e65 6c73  ost.num_channels
+00001080: 290a 2020 2020 2320 7072 696e 7420 6d61  ).    # print ma
+00001090: 6320 6164 6472 6573 730a 2020 2020 7072  c address.    pr
+000010a0: 696e 7428 686f 7374 2e6d 6163 5f61 6464  int(host.mac_add
+000010b0: 7265 7373 290a 2020 2020 2320 636c 6f73  ress).    # clos
+000010c0: 6520 7468 6520 6465 7669 6365 2063 6f6e  e the device con
+000010d0: 6e65 6374 696f 6e0a 2020 2020 6177 6169  nection.    awai
+000010e0: 7420 686f 7374 2e6c 6f67 6f75 7428 290a  t host.logout().
+000010f0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
+00001100: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
+00001110: 6173 796e 6369 6f2e 7275 6e28 7072 696e  asyncio.run(prin
+00001120: 745f 6d61 635f 6164 6472 6573 7328 2929  t_mac_address())
+00001130: 0a60 6060 600a 0a23 2323 2041 636b 6e6f  .````..### Ackno
+00001140: 776c 6564 676d 656e 740a 5468 6973 206c  wledgment.This l
+00001150: 6962 7261 7279 2069 7320 6261 7365 6420  ibrary is based 
+00001160: 6f6e 2074 6865 2077 6f72 6b20 6f66 3a0a  on the work of:.
+00001170: 2d20 6677 6573 7465 6e62 6572 673a 2068  - fwestenberg: h
+00001180: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001190: 6d2f 6677 6573 7465 6e62 6572 672f 7265  m/fwestenberg/re
+000011a0: 6f6c 696e 6b5f 6465 760a 2d20 4a69 6d53  olink_dev.- JimS
+000011b0: 7461 723a 2068 7474 7073 3a2f 2f67 6974  tar: https://git
+000011c0: 6875 622e 636f 6d2f 4a69 6d53 7461 722f  hub.com/JimStar/
+000011d0: 7265 6f6c 696e 6b5f 6970 0a              reolink_ip.
```

### Comparing `reolink_aio-0.5.9/setup.py` & `reolink_aio-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='reolink_aio',
-      version='0.5.9',
+      version='0.6.0',
       description='Reolink NVR/cameras API package',
       long_description=README,
       long_description_content_type="text/markdown",
       url='https://github.com/starkillerOG/reolink_aio',
       author='starkillerOG',
       author_email='starkiller.og@gmail.com',
       license='MIT',
```

### Comparing `reolink_aio-0.5.9/tests/test.py` & `reolink_aio-0.6.0/tests/test.py`

 * *Files identical despite different names*

