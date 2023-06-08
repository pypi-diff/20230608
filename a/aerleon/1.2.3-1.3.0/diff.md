# Comparing `tmp/aerleon-1.2.3.tar.gz` & `tmp/aerleon-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aerleon-1.2.3.tar", max compression
+gzip compressed data, was "aerleon-1.3.0.tar", max compression
```

## Comparing `aerleon-1.2.3.tar` & `aerleon-1.3.0.tar`

### file list

```diff
@@ -1,63 +1,65 @@
--rw-r--r--   0        0        0    11358 2023-05-11 03:19:35.480076 aerleon-1.2.3/LICENSE
--rw-r--r--   0        0        0     6805 2023-05-11 03:19:35.480076 aerleon-1.2.3/README.md
--rw-r--r--   0        0        0       15 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/__init__.py
--rw-r--r--   0        0        0     4200 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/aclcheck_cmdline.py
--rw-r--r--   0        0        0    17921 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/aclgen.py
--rw-r--r--   0        0        0    13124 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/api.py
--rw-r--r--   0        0        0    11358 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/COPYING
--rw-r--r--   0        0        0       29 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/__init__.py
--rwxr-xr-x   0        0        0    11008 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/aclcheck.py
--rw-r--r--   0        0        0    24649 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/aclgenerator.py
--rw-r--r--   0        0        0     4517 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/addressbook.py
--rw-r--r--   0        0        0     2792 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/arista.py
--rw-r--r--   0        0        0    36176 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/arista_tp.py
--rw-r--r--   0        0        0    10035 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/aruba.py
--rw-r--r--   0        0        0     1116 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/brocade.py
--rw-r--r--   0        0        0    39710 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/cisco.py
--rw-r--r--   0        0        0    14390 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/ciscoasa.py
--rw-r--r--   0        0        0     2754 2023-05-11 03:19:35.480076 aerleon-1.2.3/aerleon/lib/cisconx.py
--rw-r--r--   0        0        0     2428 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/ciscoxr.py
--rw-r--r--   0        0        0     9968 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/cloudarmor.py
--rw-r--r--   0        0        0     7737 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/demo.py
--rw-r--r--   0        0        0    24978 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/gce.py
--rw-r--r--   0        0        0     4759 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/gcp.py
--rw-r--r--   0        0        0    24295 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/gcp_hf.py
--rw-r--r--   0        0        0     9076 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/ipset.py
--rw-r--r--   0        0        0    38752 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/iptables.py
--rw-r--r--   0        0        0    43950 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/juniper.py
--rw-r--r--   0        0        0     5090 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/juniperevo.py
--rw-r--r--   0        0        0    32101 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/junipermsmpc.py
--rw-r--r--   0        0        0    37947 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/junipersrx.py
--rw-r--r--   0        0        0    14344 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/k8s.py
--rw-r--r--   0        0        0    17897 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/nacaddr.py
--rw-r--r--   0        0        0    38706 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/naming.py
--rw-r--r--   0        0        0    33371 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/nftables.py
--rw-r--r--   0        0        0    24741 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/nsxv.py
--rw-r--r--   0        0        0     9988 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/openconfig.py
--rw-r--r--   0        0        0    23249 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/packetfilter.py
--rw-r--r--   0        0        0    49360 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/paloaltofw.py
--rw-r--r--   0        0        0    17077 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/pcap.py
--rw-r--r--   0        0        0     3411 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/plugin.py
--rw-r--r--   0        0        0    13283 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/plugin_supervisor.py
--rw-r--r--   0        0        0    97220 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/policy.py
--rw-r--r--   0        0        0    39221 2023-05-11 03:19:35.484076 aerleon-1.2.3/aerleon/lib/policy_builder.py
--rw-r--r--   0        0        0    21391 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/policy_simple.py
--rw-r--r--   0        0        0     9162 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/policyreader.py
--rw-r--r--   0        0        0     4948 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/port.py
--rw-r--r--   0        0        0    14617 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/recognizers.py
--rw-r--r--   0        0        0     1316 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/speedway.py
--rw-r--r--   0        0        0     2405 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/srxlo.py
--rw-r--r--   0        0        0     9069 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/summarizer.py
--rw-r--r--   0        0        0    14092 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/windows.py
--rw-r--r--   0        0        0     6118 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/windows_advfirewall.py
--rw-r--r--   0        0        0     9096 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/windows_ipsec.py
--rw-r--r--   0        0        0    12540 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/yaml.py
--rw-r--r--   0        0        0     1140 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/lib/yaml_loader.py
--rw-r--r--   0        0        0        0 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/utils/__init__.py
--rw-r--r--   0        0        0     3240 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/utils/config.py
--rw-r--r--   0        0        0     3592 2023-05-11 03:19:35.488076 aerleon-1.2.3/aerleon/utils/iputils.py
--rw-r--r--   0        0        0     2712 2023-05-11 03:19:35.492076 aerleon-1.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 03:19:35.540077 aerleon-1.2.3/tools/__init__.py
--rw-r--r--   0        0        0    16234 2023-05-11 03:19:35.540077 aerleon-1.2.3/tools/cgrep.py
--rw-r--r--   0        0        0     1794 2023-05-11 03:19:35.540077 aerleon-1.2.3/tools/iputilstools.py
--rw-r--r--   0        0        0     8210 1970-01-01 00:00:00.000000 aerleon-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-08 03:28:34.987944 aerleon-1.3.0/LICENSE
+-rw-r--r--   0        0        0     6656 2023-06-08 03:28:34.987944 aerleon-1.3.0/README.md
+-rw-r--r--   0        0        0       15 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/__main__.py
+-rw-r--r--   0        0        0     4399 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/aclcheck_cmdline.py
+-rw-r--r--   0        0        0    17930 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/aclgen.py
+-rw-r--r--   0        0        0    13124 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/api.py
+-rw-r--r--   0        0        0    11358 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/COPYING
+-rw-r--r--   0        0        0       29 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/__init__.py
+-rwxr-xr-x   0        0        0    11008 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/aclcheck.py
+-rw-r--r--   0        0        0    24649 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/aclgenerator.py
+-rw-r--r--   0        0        0     4517 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/addressbook.py
+-rw-r--r--   0        0        0     2792 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/arista.py
+-rw-r--r--   0        0        0    36176 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/arista_tp.py
+-rw-r--r--   0        0        0    10035 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/aruba.py
+-rw-r--r--   0        0        0     1116 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/brocade.py
+-rw-r--r--   0        0        0    39710 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/cisco.py
+-rw-r--r--   0        0        0    14390 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/ciscoasa.py
+-rw-r--r--   0        0        0     2754 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/cisconx.py
+-rw-r--r--   0        0        0     2428 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/ciscoxr.py
+-rw-r--r--   0        0        0     9968 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/cloudarmor.py
+-rw-r--r--   0        0        0     7737 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/demo.py
+-rw-r--r--   0        0        0      689 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/fqdn.py
+-rw-r--r--   0        0        0    24978 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/gce.py
+-rw-r--r--   0        0        0     4759 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/gcp.py
+-rw-r--r--   0        0        0    24295 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/gcp_hf.py
+-rw-r--r--   0        0        0     9076 2023-06-08 03:28:34.987944 aerleon-1.3.0/aerleon/lib/ipset.py
+-rw-r--r--   0        0        0    38752 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/iptables.py
+-rw-r--r--   0        0        0    43950 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/juniper.py
+-rw-r--r--   0        0        0     5090 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/juniperevo.py
+-rw-r--r--   0        0        0    32101 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/junipermsmpc.py
+-rw-r--r--   0        0        0    37947 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/junipersrx.py
+-rw-r--r--   0        0        0    14344 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/k8s.py
+-rw-r--r--   0        0        0    17897 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/nacaddr.py
+-rw-r--r--   0        0        0    39854 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/naming.py
+-rw-r--r--   0        0        0    33371 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/nftables.py
+-rw-r--r--   0        0        0    24741 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/nsxv.py
+-rw-r--r--   0        0        0     9988 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/openconfig.py
+-rw-r--r--   0        0        0    23249 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/packetfilter.py
+-rw-r--r--   0        0        0    49360 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/paloaltofw.py
+-rw-r--r--   0        0        0    17077 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/pcap.py
+-rw-r--r--   0        0        0     3411 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/plugin.py
+-rw-r--r--   0        0        0    13283 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/plugin_supervisor.py
+-rw-r--r--   0        0        0    97865 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/policy.py
+-rw-r--r--   0        0        0    39619 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/policy_builder.py
+-rw-r--r--   0        0        0    21391 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/policy_simple.py
+-rw-r--r--   0        0        0     9162 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/policyreader.py
+-rw-r--r--   0        0        0     4948 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/port.py
+-rw-r--r--   0        0        0    14617 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/recognizers.py
+-rw-r--r--   0        0        0     1316 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/speedway.py
+-rw-r--r--   0        0        0     2405 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/srxlo.py
+-rw-r--r--   0        0        0     9069 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/summarizer.py
+-rw-r--r--   0        0        0    14092 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/windows.py
+-rw-r--r--   0        0        0     6118 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/windows_advfirewall.py
+-rw-r--r--   0        0        0     9096 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/windows_ipsec.py
+-rw-r--r--   0        0        0    12540 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/yaml.py
+-rw-r--r--   0        0        0     1140 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/lib/yaml_loader.py
+-rw-r--r--   0        0        0        0 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/utils/__init__.py
+-rw-r--r--   0        0        0     3240 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/utils/config.py
+-rw-r--r--   0        0        0     3592 2023-06-08 03:28:34.991944 aerleon-1.3.0/aerleon/utils/iputils.py
+-rw-r--r--   0        0        0     2712 2023-06-08 03:28:34.995945 aerleon-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 03:28:35.039945 aerleon-1.3.0/tools/__init__.py
+-rw-r--r--   0        0        0    16269 2023-06-08 03:28:35.039945 aerleon-1.3.0/tools/cgrep.py
+-rw-r--r--   0        0        0     1794 2023-06-08 03:28:35.039945 aerleon-1.3.0/tools/iputilstools.py
+-rw-r--r--   0        0        0     7812 1970-01-01 00:00:00.000000 aerleon-1.3.0/PKG-INFO
```

### Comparing `aerleon-1.2.3/LICENSE` & `aerleon-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/README.md` & `aerleon-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 [![PyPI version](https://badge.fury.io/py/aerleon.svg)](https://badge.fury.io/py/aerleon) ![PyPI - Status](https://img.shields.io/pypi/status/aerleon) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aerleon) ![PyPI - Downloads](https://img.shields.io/pypi/dm/aerleon)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/aerleon/aerleon/release.yml) ![Snyk Vulnerabilities for GitHub Repo](https://img.shields.io/snyk/vulnerabilities/github/aerleon/aerleon) [![aerleon](https://snyk.io/advisor/python/aerleon/badge.svg)](https://snyk.io/advisor/python/aerleon) [![codecov](https://codecov.io/gh/aerleon/aerleon/branch/main/graph/badge.svg?token=C13SR6GMTD)](https://codecov.io/gh/aerleon/aerleon)
 
 # Aerleon
 
 Generate firewall configs for multiple firewall platforms from a single platform-agnostic configuration language through a command line tool and Python API.
 
-Aerleon is a fork of [Capirca](https://github.com/google/capirca) with the following enhancements:
+Aerleon is a fork of [Capirca](https://github.com/google/capirca) with the following major additions:
 
-- New platform generators can now be added as plugins. Users no longer need to fork the project to add support for new platforms. Common platform support is still built in.
-- YAML is now supported for policy files, network definitions, and service definitions.
-- A powerful new Generate API is added that accepts policies, network definitions, and service definitions as native Python data.
-- Performance in address book generation for SRX and Palo Alto targets is greatly improved.
-- A detailed regression test suite was added to the project.
-- Unit and regression tests run automatically on all pull requests.
-- New developer tools are integrated with the project: Poetry, PyProject, nox, Codecov, Sigstore.
+- YAML policy and network definitions files are supported. A [converter from Capirca's policy DSL to YAML](https://github.com/aerleon/pol2yaml) is available.
+- FQDN values are supported in network definitions.
+- Support for new firewall platforms can be added through plugins.
+- Typed Python APIs are provided for ACL generation and aclcheck queries.
+- A [SLSA-compatible verifiable release process](https://aerleon.readthedocs.io/en/latest/install/#verifying-installation).
+- A detailed regression test suite.
+- Many bug fixes and performance enhancements.
 
 ## Install
 
 Aerleon requires Python 3.7 or higher.
 
 ```bash
 pip install aerleon
```

### Comparing `aerleon-1.2.3/aerleon/aclcheck_cmdline.py` & `aerleon-1.3.0/aerleon/aclcheck_cmdline.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,30 +28,34 @@
         prog='aclcheck',
         description=aclcheck.AclCheck.__doc__.splitlines()[0],
         formatter_class=RawTextHelpFormatter,
     )
     _parser.add_argument(
         '-p',
         '--policy-file',
+        '--policy_file',
         dest='pol',
         help='The policy file to examine.',
         required=True,
     )
     _parser.add_argument(
         '--definitions-directory',
+        '--definitions_directory',
         dest='definitions_directory',
         help='The directory where network and service definition files can be found.',
     )
     _parser.add_argument(
         '--base-directory',
+        '--base_directory',
         dest='base_directory',
         help='The base directory to use when resolving policy include paths.',
     )
     _parser.add_argument(
         '--config-file',
+        '--config_file',
         dest='config_file',
         help='Change the location searched for the configuration YAML file.',
     )
     _parser.add_argument('-d', '--destination', dest='destination_ip', help='Destination IP.')
     _parser.add_argument(
         '-s',
         '--source',
@@ -61,17 +65,23 @@
     _parser.add_argument(
         '--proto',
         '--protocol',
         dest='protocol',
         help='Protocol (tcp, udp, icmp, etc.)',
     )
     _parser.add_argument(
-        '--dport', '--destination-port', dest='destination_port', help='Destination port.'
+        '--dport',
+        '--destination-port',
+        '--destination_port',
+        dest='destination_port',
+        help='Destination port.',
+    )
+    _parser.add_argument(
+        '--sport', '--source-port', '--source_port', dest='source_port', help='Source port.'
     )
-    _parser.add_argument('--sport', '--source-port', dest='source_port', help='Source port.')
     FLAGS = _parser.parse_args()
 
     default_flags = {
         'base_directory': './policies',
         'definitions_directory': './def',
         'pol': None,
         'config_file': None,
```

### Comparing `aerleon-1.2.3/aerleon/aclgen.py` & `aerleon-1.3.0/aerleon/aclgen.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,78 +31,75 @@
 
 
 def SetupFlags():
     """Read in configuration from CLI flags."""
     flags.DEFINE_string(
         'base_directory',
         None,
-        'The base directory to look for acls; '
-        'typically where you\'d find ./corp and ./prod\n(default: \'%s\')'
-        % config.defaults['base_directory'],
+        'The base directory to search recursively for policy files.\n'
+        'Relative policy imports are resolved against this directory.\n'
+        'If --policy_file is used, aclgen will not search this directory.\n'
+        'Default: \'%s\'' % config.defaults['base_directory'],
     )
     flags.DEFINE_string(
         'definitions_directory',
         None,
-        'Directory where the definitions can be found.\n(default: \'%s\')'
-        % config.defaults['definitions_directory'],
+        'Directory containing network and service definition files.\n'
+        'Default: \'%s\'' % config.defaults['definitions_directory'],
     )
     flags.DEFINE_string('policy_file', None, 'Individual policy file to generate.')
     flags.DEFINE_string(
         'output_directory',
         None,
-        'Directory to output the rendered acls.\n(default: \'%s\')'
+        'Directory to output the rendered acls.\nDefault: \'%s\''
         % config.defaults['output_directory'],
     )
     flags.DEFINE_boolean(
         'optimize',
         None,
-        'Turn on optimization.\n(default: \'%s\')' % config.defaults['optimize'],
+        'Turn on optimization.\nDefault: \'%s\'' % config.defaults['optimize'],
         short_name='o',
     )
     flags.DEFINE_boolean(
         'recursive',
         None,
-        'Descend recursively from the base directory rendering acls\n(default: \'%s\')'
-        % str(config.defaults['recursive']).lower(),
+        'UNUSED. '
+        'Recursive policy file search is always enabled except when using the --policy_file flag.',
     )
     flags.DEFINE_boolean(
-        'debug', None, 'Debug messages\n(default: \'%s\')' % str(config.defaults['debug']).lower()
-    )
-    flags.DEFINE_boolean(
-        'verbose',
+        'debug',
         None,
-        'Verbose messages\n(default: \'%s\')' % str(config.defaults['verbose']).lower(),
+        'Display detailed messages.\nDefault: \'%s\'' % str(config.defaults['debug']).lower(),
     )
+    flags.DEFINE_boolean('verbose', None, 'UNUSED. Use --debug instead.')
     flags.DEFINE_list(
         'ignore_directories',
         None,
-        'Don\'t descend into directories that look like this string\n(default: \'%s\')'
+        'Don\'t descend into directories that look like this string.\nDefault: \'%s\''
         % ','.join(config.defaults['ignore_directories']),
     )
     flags.DEFINE_integer(
         'max_renderers',
         None,
-        'Max number of rendering processes to use.\n(default: \'%s\')'
+        'Max number of rendering processes to use.\nDefault: \'%s\''
         % config.defaults['max_renderers'],
     )
     flags.DEFINE_boolean(
         'shade_check',
         None,
-        'Raise an error when a term is completely shaded by a prior term.\n(default: \'%s\')'
+        'Raise an error when a term is completely shaded by a prior term.\nDefault: \'%s\''
         % str(config.defaults['shade_check']).lower(),
     )
     flags.DEFINE_integer(
         'exp_info',
         None,
-        'Print a info message when a term is set to expire in that many weeks.\n(default: \'%s\')'
+        'Print a message when a term is set to expire in that many weeks.\nDefault: \'%s\''
         % str(config.defaults['exp_info']),
     )
-    flags.DEFINE_multi_string(
-        'config_file', None, 'A yaml file with the configuration options for aerleon'
-    )
+    flags.DEFINE_multi_string('config_file', None, 'A YAML file with configuration options')
 
 
 class Error(Exception):
     """Base Error class."""
 
 
 class P4WriteFileError(Error):
```

### Comparing `aerleon-1.2.3/aerleon/api.py` & `aerleon-1.3.0/aerleon/api.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/COPYING` & `aerleon-1.3.0/aerleon/lib/COPYING`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/aclcheck.py` & `aerleon-1.3.0/aerleon/lib/aclcheck.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/aclgenerator.py` & `aerleon-1.3.0/aerleon/lib/aclgenerator.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/addressbook.py` & `aerleon-1.3.0/aerleon/lib/addressbook.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/arista.py` & `aerleon-1.3.0/aerleon/lib/arista.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/arista_tp.py` & `aerleon-1.3.0/aerleon/lib/arista_tp.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/aruba.py` & `aerleon-1.3.0/aerleon/lib/aruba.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/brocade.py` & `aerleon-1.3.0/aerleon/lib/brocade.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/cisco.py` & `aerleon-1.3.0/aerleon/lib/cisco.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/ciscoasa.py` & `aerleon-1.3.0/aerleon/lib/ciscoasa.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/cisconx.py` & `aerleon-1.3.0/aerleon/lib/cisconx.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/ciscoxr.py` & `aerleon-1.3.0/aerleon/lib/ciscoxr.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/cloudarmor.py` & `aerleon-1.3.0/aerleon/lib/cloudarmor.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/demo.py` & `aerleon-1.3.0/aerleon/lib/demo.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/gce.py` & `aerleon-1.3.0/aerleon/lib/gce.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/gcp.py` & `aerleon-1.3.0/aerleon/lib/gcp.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/gcp_hf.py` & `aerleon-1.3.0/aerleon/lib/gcp_hf.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/ipset.py` & `aerleon-1.3.0/aerleon/lib/ipset.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/iptables.py` & `aerleon-1.3.0/aerleon/lib/iptables.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/juniper.py` & `aerleon-1.3.0/aerleon/lib/juniper.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/juniperevo.py` & `aerleon-1.3.0/aerleon/lib/juniperevo.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/junipermsmpc.py` & `aerleon-1.3.0/aerleon/lib/junipermsmpc.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/junipersrx.py` & `aerleon-1.3.0/aerleon/lib/junipersrx.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/k8s.py` & `aerleon-1.3.0/aerleon/lib/k8s.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/nacaddr.py` & `aerleon-1.3.0/aerleon/lib/nacaddr.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/naming.py` & `aerleon-1.3.0/aerleon/lib/naming.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
 import yaml
 from absl import logging
 from yaml import YAMLError
 
 from aerleon.lib import nacaddr
 from aerleon.lib import port as portlib
+from aerleon.lib.fqdn import FQDN
 from aerleon.lib.nacaddr import IPv4, IPv6
 from aerleon.lib.yaml_loader import SpanSafeYamlLoader
 
 DEF_TYPE_SERVICES = 'services'
 DEF_TYPE_NETWORKS = 'networks'
 
 
@@ -68,15 +69,15 @@
 
 
 class NamespaceCollisionError(Error):
     """Used to report on duplicate symbol names found while parsing."""
 
 
 class BadNetmaskTypeError(Error):
-    """Used to report on duplicate symbol names found while parsing."""
+    """Deprecated."""
 
 
 class NoDefinitionsError(Error):
     """Raised if no definitions are found."""
 
 
 class ParseError(Error):
@@ -103,14 +104,18 @@
     """A general syntax error for the definition."""
 
 
 class DefinitionFileTypeError(Error):
     """Invalid Definition File"""
 
 
+class EmptyDefinitionError(Error):
+    """A token returned no results."""
+
+
 # Consider making this span-oriented
 # (file > line > (start_ch, end_ch))
 class UserMessage:
     """A user-facing error message encountered during file processing.
 
     Users can be shown:
     * An error message only (user_message.message).
@@ -212,14 +217,15 @@
           naming_type: Optional. A string containing either 'service' or 'network'.
             This option is only needed if naming_file is provided and it refers to
             a non-YAML file.
         """
         self.current_symbol = None
         self.services = {}
         self.networks = {}
+        self.fqdn = {}
         self.unseen_services = {}
         self.unseen_networks = {}
         self.port_re = re.compile(r'(^\d+-\d+|^\d+)\/\w+$|^[\w\d-]+$', re.IGNORECASE | re.DOTALL)
         self.token_re = re.compile(r'(^[-_A-Z0-9]+$)', re.IGNORECASE)
 
         if naming_file:
             file_path = Path(naming_dir).joinpath(naming_file)
@@ -534,73 +540,107 @@
         for service in self.GetService(servicename):
             if service and '/' in service:
                 parts = service.split('/')
                 if parts[1].upper() == proto:
                     services_set.add(parts[0])
         return sorted(services_set)
 
-    def GetNetAddr(self, token: str) -> List[Union[IPv4, IPv6]]:
-        """Given a network token, return a list of nacaddr.IPv4 or nacaddr.IPv6 objects.
+    def GetFQDN(self, query: str) -> List[str]:
+        """Expand a network token into a list of FQDN objects.
 
         Args:
-          token: A name of a network definition, such as 'INTERNAL'
+          query: Network definition token. May include comment text
 
         Returns:
-          A list of nacaddr.IPv4 or nacaddr.IPv6 objects.
+          List of nacaddr.IPv4 or nacaddr.IPv6 objects
 
         Raises:
-          UndefinedAddressError: if the network name isn't defined.
+          UndefinedAddressError: Network token not defined
+          EmptyDefinitionError: No FQDN values found for this network token
         """
-        return self.GetNet(token)
+        results = self._GetFQDN(query)
+        if len(results) == 0:
+            raise EmptyDefinitionError(f"No FQDN values found for network: {query}")
+        return results
+
+    def _GetFQDN(self, query: str, level=0) -> List[str]:
+        returnlist = []
+        data = query.split('#')
+        token = data[0].split()[0]
+        if token not in self.fqdn:
+            raise UndefinedAddressError(f'UNDEFINED: {token}')
+        for i in self.fqdn[token].items:
+            comment = ''
+            if i.find('#') > -1:
+                (name, comment) = i.split('#', 1)
+            else:
+                name = i
+
+            name = name.strip()
+            if self.token_re.match(name):
+                returnlist.extend(self._GetFQDN(name))
+            else:
+                try:
+                    fqdn = FQDN(name, token, comment)
+                    fqdn.text = comment.lstrip()
+                    fqdn.token = token
+                    returnlist.append(fqdn)
+                except ValueError:
+                    pass
+        for i in returnlist:
+            i.parent_token = token
+        return returnlist
+
+    def GetNetAddr(self, query: str) -> List[Union[IPv4, IPv6]]:
+        """Alias of Naming.GetNet"""
+        return self.GetNet(query)
 
     def GetNet(self, query: str) -> List[Union[IPv4, IPv6]]:
         """Expand a network token into a list of nacaddr.IPv4 or nacaddr.IPv6 objects.
 
         Args:
-          query: Network definition token which may include comment text
-
-        Raises:
-          BadNetmaskTypeError: Results when an unknown netmask_type is
-          specified.  Acceptable values are 'cidr', 'netmask', and 'hostmask'.
+          query: Network definition token. May include comment text.
 
         Returns:
           List of nacaddr.IPv4 or nacaddr.IPv6 objects
 
         Raises:
-          UndefinedAddressError: for an undefined token value
+          UndefinedAddressError: Network token not defined
+          EmptyDefinitionError: No IP address values found for this network token
         """
+        results = self._GetNet(query)
+        if len(results) == 0:
+            raise EmptyDefinitionError(f"No IP addresses found for network: {query}")
+        return results
+
+    def _GetNet(self, query: str) -> List[Union[IPv4, IPv6]]:
         returnlist = []
-        data = []
-        token = ''
-        data = query.split('#')  # Get the token keyword and remove any comment
-        token = data[0].split()[0]  # Remove whitespace and cast from list to string
+        data = query.split('#')
+        token = data[0].split()[0]
         if token not in self.networks:
-            raise UndefinedAddressError('%s %s' % ('\nUNDEFINED:', str(token)))
+            raise UndefinedAddressError(f'UNDEFINED: {token}')
 
         for i in self.networks[token].items:
             comment = ''
             if i.find('#') > -1:
                 (net, comment) = i.split('#', 1)
             else:
                 net = i
 
             net = net.strip()
             if self.token_re.match(net):
                 returnlist.extend(self.GetNet(net))
             else:
                 try:
-                    # TODO(robankeny): Fix using error to continue processing.
                     addr = nacaddr.IP(net, strict=False)
                     addr.text = comment.lstrip()
                     addr.token = token
                     returnlist.append(addr)
                 except ValueError:
-                    # if net was something like 'FOO', or the name of another token which
-                    # needs to be dereferenced, nacaddr.IP() will return a ValueError
-                    returnlist.extend(self.GetNet(net))
+                    pass
         for i in returnlist:
             i.parent_token = token
         return returnlist
 
     def _Parse(self, definitions_directory: str) -> None:
         """Parse files for tokens and values.
 
@@ -681,21 +721,14 @@
         Raises:
           UnexpectedDefinitionTypeError: called with unexpected type of definitions.
           NamespaceCollisionError: when overlapping tokens are found.
           ParseError: If errors occur
           NamingSyntaxError: Syntax error parsing config.
         """
 
-        #
-        # NOTE: The "unseen name" logic defined in this function (_ParseLine) is duplicated in
-        # function ParseDefinitionsObject. Any changes to how "unseen name" checking is done
-        # need to be made in both places.
-        #
-        # TODO(jb): Consider splitting up _ParseLine so that it generates an intermediate
-        #  representation (ItemUnit) and "unseen name" checks are done on the IR (by both _Parse* flows).
         if definition_type not in ['services', 'networks']:
             raise UnexpectedDefinitionTypeError(
                 '%s %s' % ('Received an unexpected definition type:', definition_type)
             )
         line = line.strip()
         if not line or line.startswith('#'):  # Skip comments and blanks.
             return
@@ -766,32 +799,39 @@
                             if value_piece not in self.unseen_services:
                                 self.unseen_services[value_piece] = True
                     if definition_type == DEF_TYPE_NETWORKS:
                         if value_piece not in self.networks:
                             if value_piece not in self.unseen_networks:
                                 self.unseen_networks[value_piece] = True
 
-    def ParseYaml(self, file_handle: str, file_name: str) -> None:
-        """Load a definition yaml file as a string.
+    def ParseYaml(self, file: str, file_name: str) -> None:
+        """Load network and service definitions from YAML.
 
         Arguments:
             file: A string containing the file contents.
-            filename: The original filename of the file.
+            file_name: The original filename of the file.
         """
 
         try:
-            file_data = yaml.load(file_handle, Loader=SpanSafeYamlLoader(filename=file_name))
+            file_data = yaml.load(file, Loader=SpanSafeYamlLoader(filename=file_name))
         except YAMLError as yaml_error:
             raise DefinitionFileTypeError(
                 UserMessage("Unable to read file as YAML.", filename=file_name)
             ) from yaml_error
 
         self.ParseDefinitionsObject(file_data, file_name)
 
     def ParseDefinitionsObject(self, file_data: Dict[str, str], file_name: str) -> None:
+        """Load network and service definitions from a Python object.
+
+        Arguments:
+            file_data: A Python dict where file_data.networks contains network
+                data and/or file_data.services contains service data.
+            file_name: The original filename of the file.
+        """
         # Empty files are ignored with a warning
         if not file_data:
             logging.warning(UserMessage("Ignoring empty address book file.", filename=file_name))
             return
 
         # Check for at least one essential key, ignore with warning
         essential_keys = ['networks', 'services']
@@ -824,66 +864,79 @@
 
             if not ('values' in symbol_def and isinstance(symbol_def['values'], list)):
                 logging.info(
                     f'\nNetwork definition must be a list. Ignoring definition for network: {symbol}.'
                 )
                 continue
 
-            # TODO(jb) This check should be performed on the IR so we can hoist it from _ParseLine
             if not self.token_re.match(symbol):
                 logging.info(
                     f'\nNetwork name does not match recommended criteria: {symbol}\nOnly A-Z, a-z, 0-9, -, and _ allowed'
                 )
 
-            # TODO(jb) This check should be performed on the IR so we can hoist it from _ParseLine
             if symbol in self.networks:
                 raise NamespaceCollisionError(
                     f'\nMultiple definitions found for network: {symbol}'
                 )
 
-            unit = _ItemUnit(symbol)
+            addr_unit = _ItemUnit(symbol)
+            fqdn_unit = _ItemUnit(symbol)
 
-            # TODO(jb) This operation should be performed on the IR so we can hoist it from _ParseLine
-            self.networks[symbol] = unit
+            self.networks[symbol] = addr_unit
+            self.fqdn[symbol] = fqdn_unit
             if symbol in self.unseen_networks:
                 self.unseen_networks.pop(symbol)
 
             for item in symbol_def['values']:
                 # 'item' can be:
                 # 1. A string, understood as a network name reference
                 # 2. A dictionary, with these fields:
                 #    'address': A specific IP address or CIDR range
+                #    'hostname': A FQDN for use in DNS filtering.
                 #    'name': A network name reference
                 #    'comment': An optional comment
                 # 'address' or 'name' must be present in any dictionary item
                 value = None
                 network_ref = None
                 ip = None
                 comment = None
                 if isinstance(item, str):
                     value = network_ref = item
                 elif isinstance(item, dict):
                     if 'name' in item and isinstance(item['name'], str):
                         value = network_ref = item['name']
                     elif 'address' in item and isinstance(item['address'], str):
                         value = ip = item['address']
+                    elif 'fqdn' in item and isinstance(item['fqdn'], str):
+                        value = item['fqdn']
                     else:
                         logging.info(f'\nNetwork name or CIDR expected for: {symbol}')
                         continue
 
                     if 'comment' in item and isinstance(item['comment'], str):
                         comment = item['comment']
                 else:
                     logging.info(f'\nUnexpected symbol definition: {symbol}')
                     continue
-
                 if comment is None:
-                    unit.items.append(value)
+                    if network_ref:
+                        addr_unit.items.append(value)
+                        fqdn_unit.items.append(value)
+                    elif ip:
+                        addr_unit.items.append(value)
+                    else:
+                        fqdn_unit.items.append(value)
                 else:
-                    unit.items.append(f'{value} # {comment}')
+                    if network_ref:
+                        addr_unit.items.append(f'{value} # {comment}')
+                        fqdn_unit.items.append(f'{value} # {comment}')
+                    elif ip:
+                        addr_unit.items.append(f'{value} # {comment}')
+                    else:
+                        fqdn_unit.items.append(f'{value} # {comment}')
 
                 if network_ref and network_ref not in self.networks:
                     if network_ref not in self.unseen_networks:
                         self.unseen_networks[network_ref] = True
 
     def _ParseYamlServices(self, file_data: Dict[str, Any], file_name: str) -> None:
         if 'services' in file_data and not isinstance(file_data['services'], dict):
@@ -901,29 +954,26 @@
 
             if not isinstance(symbol_def, list):
                 logging.info(
                     f'\nService definition must be a list. Ignoring definition for service: {symbol}.'
                 )
                 continue
 
-            # TODO(jb) This check should be performed on the IR so we can hoist it from _ParseLine
             if not self.token_re.match(symbol):
                 logging.info(
                     f'\nService name does not match recommended criteria: {symbol}\nOnly A-Z, a-z, 0-9, -, and _ allowed'
                 )
 
-            # TODO(jb) This check should be performed on the IR so we can hoist it from _ParseLine
             if symbol in self.services:
                 raise NamespaceCollisionError(
                     f'\nMultiple definitions found for service: {symbol}'
                 )
 
             unit = _ItemUnit(symbol)
 
-            # TODO(jb) This operation should be performed on the IR so we can hoist it from _ParseLine
             self.services[symbol] = unit
             if symbol in self.unseen_services:
                 self.unseen_services.pop(symbol)
 
             for item in symbol_def:
                 # 'item' can be:
                 # 1. A string, understood as a service name reference
```

### Comparing `aerleon-1.2.3/aerleon/lib/nftables.py` & `aerleon-1.3.0/aerleon/lib/nftables.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/nsxv.py` & `aerleon-1.3.0/aerleon/lib/nsxv.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/openconfig.py` & `aerleon-1.3.0/aerleon/lib/openconfig.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/packetfilter.py` & `aerleon-1.3.0/aerleon/lib/packetfilter.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/paloaltofw.py` & `aerleon-1.3.0/aerleon/lib/paloaltofw.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/pcap.py` & `aerleon-1.3.0/aerleon/lib/pcap.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/plugin.py` & `aerleon-1.3.0/aerleon/lib/plugin.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/plugin_supervisor.py` & `aerleon-1.3.0/aerleon/lib/plugin_supervisor.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/policy.py` & `aerleon-1.3.0/aerleon/lib/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,14 +319,15 @@
       obj: an object of type VarType or a list of objects of type VarType
 
     members:
       address/source_address/destination_address/: list of
         VarType.(S|D)?ADDRESS's
       address_exclude/source_address_exclude/destination_address_exclude: list of
         VarType.(S|D)?ADDEXCLUDE's
+      source/destination_fqdn: list of VarType.(S|D)?FQDN's
       restrict-address-family: VarType.RESTRICT_ADDRESS_FAMILY
       port/source_port/destination_port: list of VarType.(S|D)?PORT's
       options: list of VarType.OPTION's.
       protocol: list of VarType.PROTOCOL's.
       counter: VarType.COUNTER
       traffic-class-count: VarType.TRAFFIC_CLASS_COUNT
       action: list of VarType.ACTION's
@@ -429,14 +430,15 @@
         self.address_exclude = []
         self.restrict_address_family = None
         self.comment = []
         self.counter = None
         self.expiration = None
         self.destination_address = []
         self.destination_address_exclude = []
+        self.destination_fqdn = []
         self.destination_port = []
         self.destination_prefix = []
         self.filter_term = None
         self.forwarding_class = []
         self.forwarding_class_except = []
         self.logging = []
         self.log_limit = None
@@ -450,14 +452,15 @@
         self.protocol = []
         self.protocol_except = []
         self.qos = None
         self.pan_application = []
         self.routing_instance = None
         self.source_address = []
         self.source_address_exclude = []
+        self.source_fqdn = []
         self.source_port = []
         self.source_prefix = []
         self.ttl = None
         self.verbatim = []
         # juniper specific.
         self.packet_length = None
         self.fragment_offset = None
@@ -711,25 +714,29 @@
         if self.source_address:
             ret_str.append('  source_address: %s' % self._SortAddressesByFamily('source_address'))
         if self.source_address_exclude:
             ret_str.append(
                 '  source_address_exclude: %s'
                 % self._SortAddressesByFamily('source_address_exclude')
             )
+        if self.source_fqdn:
+            ret_str.append(f'  source_fqdn: {self.source_fqdn}')
         if self.source_tag:
             ret_str.append('  source_tag: %s' % self.source_tag)
         if self.destination_address:
             ret_str.append(
                 '  destination_address: %s' % self._SortAddressesByFamily('destination_address')
             )
         if self.destination_address_exclude:
             ret_str.append(
                 '  destination_address_exclude: %s'
                 % self._SortAddressesByFamily('destination_address_exclude')
             )
+        if self.destination_fqdn:
+            ret_str.append(f'  destination_fqdn: {self.destination_fqdn}')
         if self.destination_tag:
             ret_str.append('  destination_tag: %s' % self.destination_tag)
         if self.target_resources:
             ret_str.append('  target_resources: %s' % self.target_resources)
         if self.target_service_accounts:
             ret_str.append('  target_service_accounts: %s' % self.target_service_accounts)
         if self.source_prefix:
@@ -1177,14 +1184,18 @@
                     self.target_resources.append(x.value)
                 elif x.var_type is VarType.TARGET_SERVICE_ACCOUNTS:
                     self.target_service_accounts.append(x.value)
                 elif x.var_type is VarType.SZONE:
                     self.source_zone.append(x.value)
                 elif x.var_type is VarType.DZONE:
                     self.destination_zone.append(x.value)
+                elif x.var_type is VarType.DESTINATION_FQDN:
+                    self.destination_fqdn.extend(DEFINITIONS.GetFQDN(x.value))
+                elif x.var_type is VarType.SOURCE_FQDN:
+                    self.source_fqdn.extend(DEFINITIONS.GetFQDN(x.value))
                 else:
                     raise TermObjectTypeError(
                         '%s isn\'t a type I know how to deal with (contains \'%s\')'
                         % (type(x), x.value)
                     )
         else:
             # stupid no switch statement in python
@@ -1614,14 +1625,16 @@
     TARGET_SERVICE_ACCOUNTS = 60
     ENCAPSULATE = 61
     FILTER_TERM = 62
     RESTRICT_ADDRESS_FAMILY = 63
     PORT_MIRROR = 64
     SZONE = 65
     DZONE = 66
+    SOURCE_FQDN = 67
+    DESTINATION_FQDN = 68
 
     def __init__(self, var_type: int, value: Any) -> None:
         self.var_type = var_type
         if self.var_type == self.COMMENT or self.var_type == self.LOG_NAME:
             # remove the double quotes
             val = str(value).strip('"')
             # make all of the lines start w/o leading whitespace.
```

### Comparing `aerleon-1.2.3/aerleon/lib/policy_builder.py` & `aerleon-1.3.0/aerleon/lib/policy_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         "address": WordList,
         "address-exclude": WordList,
         "restrict-address-family": str,
         "counter": str,
         "expiration": "datetime.date | str",
         "destination-address": WordList,
         "destination-exclude": WordList,
+        "destination-fqdn": WordList,
         "destination-port": WordList,
         "destination-prefix": WordList,
         "filter-term": str,
         "forwarding-class": "list[str]",
         "forwarding-class-except": "list[str]",
         "logging": WordList,
         "log-limit": str,
@@ -92,14 +93,15 @@
         "protocol": "str | list[int | str]",
         "protocol-except": "str | list[int | str]",
         "qos": str,
         "pan-application": WordList,
         "routing-instance": str,
         "source-address": WordList,
         "source-exclude": WordList,
+        "source-fqdn": WordList,
         "source-port": WordList,
         "source-prefix": WordList,
         "ttl": "int | str",
         "verbatim": "dict[str, str]",
         "packet-length": "int | str",
         "fragment-offset": "int | str",
         "hop-limit": "int | str",
@@ -446,14 +448,15 @@
     'address':                    TListStrCollapsible,
     'address-exclude':            TListStrCollapsible,
     'restrict-address-family':    TValue.WordString,
     'counter':                    TValue.WordString,
     'expiration':                 TValue.YearMonthDay,
     'destination-address':        TListStrCollapsible,
     'destination-exclude':        TListStrCollapsible,
+    'destination-fqdn':       TListStrCollapsible,
     'destination-port':           TListStrCollapsible,
     'destination-prefix':         TListStrCollapsible,
     'filter-term':                TValue.WordString,
     'forwarding-class':           TList(of=TValue.WordString),
     'forwarding-class-except':    TList(of=TValue.WordString),
     'logging':                    TListStrCollapsible,
     'log-limit':                  TValue.LogLimit,
@@ -467,14 +470,15 @@
     'protocol':                   TList(of=TUnion(of=[TValue.Integer, TValue.WordString]), collapsible=True),
     'protocol-except':            TList(of=TUnion(of=[TValue.Integer, TValue.WordString]), collapsible=True),
     'qos':                        TValue.WordString,
     'pan-application':            TListStrCollapsible,
     'routing-instance':           TValue.WordString,
     'source-address':             TListStrCollapsible,
     'source-exclude':             TListStrCollapsible,
+    'source-fqdn':            TListStrCollapsible,
     'source-port':                TListStrCollapsible,
     'source-prefix':              TListStrCollapsible,
     'ttl':                        TValue.Integer,
     'verbatim':                   TSection(of=[(TValue.WordString, TValue.AnyString)]),
     # juniper specific.           
     'packet-length':              TUnion(of=[TValue.Integer, TValue.IntegerRange]),
     'fragment-offset':            TUnion(of=[TValue.Integer, TValue.IntegerRange]),
@@ -586,14 +590,16 @@
         'timeout':                    (_CallType.SingleValue,  VarType.TIMEOUT),
         'dscp-set':                   (_CallType.SingleValue,  VarType.DSCP_SET),
         'ttl':                        (_CallType.SingleValue,  VarType.TTL),
         'filter-term':                (_CallType.SingleValue,  VarType.FILTER_TERM),
         'vpn':                        (_CallType.SingleValue,  VarType.VPN),
         'source-address':             (_CallType.SingleList,   VarType.SADDRESS),
         'destination-address':        (_CallType.SingleList,   VarType.DADDRESS),
+        'destination-fqdn':       (_CallType.SingleList,   VarType.DESTINATION_FQDN),
+        'source-fqdn':            (_CallType.SingleList,   VarType.SOURCE_FQDN),
         'address':                    (_CallType.SingleList,   VarType.ADDRESS),
         'source-exclude':             (_CallType.SingleList,   VarType.SADDREXCLUDE),
         'destination-exclude':        (_CallType.SingleList,   VarType.DADDREXCLUDE),
         'address-exclude':            (_CallType.SingleList,   VarType.ADDREXCLUDE),
         'port':                       (_CallType.SingleList,   VarType.PORT),
         'source-port':                (_CallType.SingleList,   VarType.SPORT),
         'destination-port':           (_CallType.SingleList,   VarType.DPORT),
@@ -876,14 +882,16 @@
             'source-interface',
             'destination-interface',
             'platform',
             'platform-exclude',
             'target-resources',
             'target-service-accounts',
             'timeout',
+            'destination-fqdn',
+            'source-fqdn',
         }
     )
 
     @classmethod
     def _NormalizeValues(cls, context: RecognizerContext, repr):
         """See BuiltinRecognizer.normalizeValues()."""
 
@@ -918,9 +926,8 @@
         elif context.keyword == "vpn":
             if 'name' not in repr:
                 raise TypeError("VPN: keyword 'name' is mising.")
             # Policy model expects each kv represented as a length-2 tuple.
             # The policy name field should be given as an empty string if not provided
             # by the user.
             repr = (repr['name'], repr.get('policy', ''))
-
         return repr
```

### Comparing `aerleon-1.2.3/aerleon/lib/policy_simple.py` & `aerleon-1.3.0/aerleon/lib/policy_simple.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/policyreader.py` & `aerleon-1.3.0/aerleon/lib/policyreader.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/port.py` & `aerleon-1.3.0/aerleon/lib/port.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/recognizers.py` & `aerleon-1.3.0/aerleon/lib/recognizers.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/speedway.py` & `aerleon-1.3.0/aerleon/lib/speedway.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/srxlo.py` & `aerleon-1.3.0/aerleon/lib/srxlo.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/summarizer.py` & `aerleon-1.3.0/aerleon/lib/summarizer.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/windows.py` & `aerleon-1.3.0/aerleon/lib/windows.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/windows_advfirewall.py` & `aerleon-1.3.0/aerleon/lib/windows_advfirewall.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/windows_ipsec.py` & `aerleon-1.3.0/aerleon/lib/windows_ipsec.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/yaml.py` & `aerleon-1.3.0/aerleon/lib/yaml.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/lib/yaml_loader.py` & `aerleon-1.3.0/aerleon/lib/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/utils/config.py` & `aerleon-1.3.0/aerleon/utils/config.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/aerleon/utils/iputils.py` & `aerleon-1.3.0/aerleon/utils/iputils.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/pyproject.toml` & `aerleon-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aerleon"
-version = "1.2.3"
+version = "1.3.0"
 description = "A firewall generation tool"
 authors = ["Rob Ankeny <ankenyr@gmail.com>", "Jason Benterou <jason.benterou@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/aerleon/aerleon"
 repository = "https://github.com/aerleon/aerleon"
 keywords = ["firewall", "networking", "security"]
```

### Comparing `aerleon-1.2.3/tools/cgrep.py` & `aerleon-1.3.0/tools/cgrep.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     parser = argparse.ArgumentParser(
         description='c[apirca]grep', formatter_class=argparse.RawTextHelpFormatter
     )
 
     parser.add_argument(
         '-d',
         '--def',
+        '--definitions_directory',
         dest='defs',
         help='Network Definitions directory location. \n',
         default='./def',
     )
 
     # -i and -t can be used together, but not with any other option.
     ip_group = parser.add_argument_group()
```

### Comparing `aerleon-1.2.3/tools/iputilstools.py` & `aerleon-1.3.0/tools/iputilstools.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.2.3/PKG-INFO` & `aerleon-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aerleon
-Version: 1.2.3
+Version: 1.3.0
 Summary: A firewall generation tool
 Home-page: https://github.com/aerleon/aerleon
 License: Apache-2.0
 Keywords: firewall,networking,security
 Author: Rob Ankeny
 Author-email: ankenyr@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -13,19 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Networking :: Firewalls
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: absl-py (>=1.2.0,<2.0.0)
 Requires-Dist: importlib-metadata (>=4.2,<5.0) ; python_version <= "3.10"
 Requires-Dist: ply (>=3.11,<4.0)
 Requires-Dist: typing_extensions (>=4.4.0,<5.0.0)
@@ -36,23 +31,23 @@
 [![PyPI version](https://badge.fury.io/py/aerleon.svg)](https://badge.fury.io/py/aerleon) ![PyPI - Status](https://img.shields.io/pypi/status/aerleon) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/aerleon) ![PyPI - Downloads](https://img.shields.io/pypi/dm/aerleon)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/aerleon/aerleon/release.yml) ![Snyk Vulnerabilities for GitHub Repo](https://img.shields.io/snyk/vulnerabilities/github/aerleon/aerleon) [![aerleon](https://snyk.io/advisor/python/aerleon/badge.svg)](https://snyk.io/advisor/python/aerleon) [![codecov](https://codecov.io/gh/aerleon/aerleon/branch/main/graph/badge.svg?token=C13SR6GMTD)](https://codecov.io/gh/aerleon/aerleon)
 
 # Aerleon
 
 Generate firewall configs for multiple firewall platforms from a single platform-agnostic configuration language through a command line tool and Python API.
 
-Aerleon is a fork of [Capirca](https://github.com/google/capirca) with the following enhancements:
+Aerleon is a fork of [Capirca](https://github.com/google/capirca) with the following major additions:
 
-- New platform generators can now be added as plugins. Users no longer need to fork the project to add support for new platforms. Common platform support is still built in.
-- YAML is now supported for policy files, network definitions, and service definitions.
-- A powerful new Generate API is added that accepts policies, network definitions, and service definitions as native Python data.
-- Performance in address book generation for SRX and Palo Alto targets is greatly improved.
-- A detailed regression test suite was added to the project.
-- Unit and regression tests run automatically on all pull requests.
-- New developer tools are integrated with the project: Poetry, PyProject, nox, Codecov, Sigstore.
+- YAML policy and network definitions files are supported. A [converter from Capirca's policy DSL to YAML](https://github.com/aerleon/pol2yaml) is available.
+- FQDN values are supported in network definitions.
+- Support for new firewall platforms can be added through plugins.
+- Typed Python APIs are provided for ACL generation and aclcheck queries.
+- A [SLSA-compatible verifiable release process](https://aerleon.readthedocs.io/en/latest/install/#verifying-installation).
+- A detailed regression test suite.
+- Many bug fixes and performance enhancements.
 
 ## Install
 
 Aerleon requires Python 3.7 or higher.
 
 ```bash
 pip install aerleon
```

