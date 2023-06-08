# Comparing `tmp/insights-core-3.1.9.tar.gz` & `tmp/insights-core-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/insights-core-3.1.9.tar", last modified: Thu Feb 23 12:26:14 2023, max compression
+gzip compressed data, was "dist/insights-core-3.2.0.tar", last modified: Thu Jun  8 07:16:07 2023, max compression
```

## Comparing `insights-core-3.1.9.tar` & `insights-core-3.2.0.tar`

### file list

```diff
@@ -1,1500 +1,1526 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/examples/cluster_rules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/examples/cluster_rules/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6054 2023-02-23 12:13:26.000000 insights-core-3.1.9/examples/cluster_rules/allnodes_cpu.py
--rwxr-xr-x   0 root         (0) root         (0)     1975 2023-02-23 12:13:26.000000 insights-core-3.1.9/examples/cluster_rules/bash_version.py
--rwxr-xr-x   0 root         (0) root         (0)     2588 2023-02-23 12:13:26.000000 insights-core-3.1.9/examples/cluster_rules/ntp_compare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/examples/rules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/examples/rules/__init__.py
--rw-r--r--   0 root         (0) root         (0)      541 2023-02-23 12:13:26.000000 insights-core-3.1.9/examples/rules/bash_version.py
--rwxr-xr-x   0 root         (0) root         (0)     1406 2023-02-23 12:13:26.000000 insights-core-3.1.9/examples/rules/hostname_rel.py
--rwxr-xr-x   0 root         (0) root         (0)      862 2023-02-23 12:13:26.000000 insights-core-3.1.9/examples/rules/sample_script.py
--rwxr-xr-x   0 root         (0) root         (0)     5084 2023-02-23 12:13:26.000000 insights-core-3.1.9/examples/rules/skip_component.py
--rwxr-xr-x   0 root         (0) root         (0)     2746 2023-02-23 12:13:26.000000 insights-core-3.1.9/examples/rules/stand_alone.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/client/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/client/apps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/client/apps/ansible/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/
--rw-r--r--   0 root         (0) root         (0)     2163 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/__init__.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/anchor.py
--rw-r--r--   0 root         (0) root         (0)    35216 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/comments.py
--rw-r--r--   0 root         (0) root         (0)     8726 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/compat.py
--rw-r--r--   0 root         (0) root         (0)     8304 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/composer.py
--rw-r--r--   0 root         (0) root         (0)      345 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/configobjwalker.py
--rw-r--r--   0 root         (0) root         (0)    70571 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/constructor.py
--rw-r--r--   0 root         (0) root         (0)     6596 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/cyaml.py
--rw-r--r--   0 root         (0) root         (0)     6640 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/dumper.py
--rw-r--r--   0 root         (0) root         (0)    64442 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/emitter.py
--rw-r--r--   0 root         (0) root         (0)     8982 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/error.py
--rw-r--r--   0 root         (0) root         (0)     3902 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/events.py
--rw-r--r--   0 root         (0) root         (0)     2972 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/loader.py
--rw-r--r--   0 root         (0) root         (0)    54172 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/main.py
--rw-r--r--   0 root         (0) root         (0)     3716 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/nodes.py
--rw-r--r--   0 root         (0) root         (0)    33260 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/parser.py
--rw-r--r--   0 root         (0) root         (0)    10885 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/reader.py
--rw-r--r--   0 root         (0) root         (0)    48762 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/representer.py
--rw-r--r--   0 root         (0) root         (0)    15356 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/resolver.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarbool.py
--rw-r--r--   0 root         (0) root         (0)     4409 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarfloat.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarint.py
--rw-r--r--   0 root         (0) root         (0)     4548 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarstring.py
--rw-r--r--   0 root         (0) root         (0)    72204 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scanner.py
--rw-r--r--   0 root         (0) root         (0)     8430 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/serializer.py
--rw-r--r--   0 root         (0) root         (0)     1792 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/timestamp.py
--rw-r--r--   0 root         (0) root         (0)     7471 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/tokens.py
--rw-r--r--   0 root         (0) root         (0)     6127 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/util.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/__init__.py
--rw-r--r--   0 root         (0) root         (0)    61772 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/gnupg.py
--rw-r--r--   0 root         (0) root         (0)     1560 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/oyaml.py
--rw-r--r--   0 root         (0) root         (0)     8508 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/__init__.py
--rw-r--r--   0 root         (0) root         (0)      768 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/__main__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/ansible/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/client/apps/compliance/
--rw-r--r--   0 root         (0) root         (0)    12054 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/compliance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/client/apps/malware_detection/
--rw-r--r--   0 root         (0) root         (0)    80650 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/malware_detection/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2709 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/apps/manifests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/client/phase/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/phase/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12866 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/phase/v1.py
--rw-r--r--   0 root         (0) root         (0)    28791 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10067 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/archive.py
--rw-r--r--   0 root         (0) root         (0)    10030 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/auto_config.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/cert_auth.py
--rw-r--r--   0 root         (0) root         (0)    13273 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/client.py
--rw-r--r--   0 root         (0) root         (0)    19417 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/collection_rules.py
--rw-r--r--   0 root         (0) root         (0)    31590 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/config.py
--rw-r--r--   0 root         (0) root         (0)    46142 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/connection.py
--rw-r--r--   0 root         (0) root         (0)     4406 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/constants.py
--rw-r--r--   0 root         (0) root         (0)     3622 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/core_collector.py
--rw-r--r--   0 root         (0) root         (0)    20807 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/data_collector.py
--rw-r--r--   0 root         (0) root         (0)     5541 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/insights_spec.py
--rw-r--r--   0 root         (0) root         (0)     6237 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/map_components.py
--rw-r--r--   0 root         (0) root         (0)     5281 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/schedule.py
--rw-r--r--   0 root         (0) root         (0)      521 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/subp.py
--rw-r--r--   0 root         (0) root         (0)     6896 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/support.py
--rw-r--r--   0 root         (0) root         (0)     1391 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/client/url_cache.py
--rw-r--r--   0 root         (0) root         (0)    14480 2023-02-23 12:15:15.000000 insights-core-3.1.9/insights/client/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/combiners/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3470 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/ansible_info.py
--rw-r--r--   0 root         (0) root         (0)     1295 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/ceph_osd_tree.py
--rw-r--r--   0 root         (0) root         (0)     2930 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/ceph_version.py
--rw-r--r--   0 root         (0) root         (0)     3199 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/cloud_instance.py
--rw-r--r--   0 root         (0) root         (0)    16645 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/cloud_provider.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/cpu_vulns_all.py
--rw-r--r--   0 root         (0) root         (0)     4877 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/crio_conf.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/cryptsetup.py
--rw-r--r--   0 root         (0) root         (0)     2739 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/dmesg.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/dnsmasq_conf_all.py
--rw-r--r--   0 root         (0) root         (0)     1183 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/du.py
--rw-r--r--   0 root         (0) root         (0)     8050 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/grub_conf.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/hostname.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/httpd_conf.py
--rw-r--r--   0 root         (0) root         (0)     4319 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/ipcs_semaphores.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/ipcs_shared_memory.py
--rw-r--r--   0 root         (0) root         (0)     6463 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/ipv6.py
--rw-r--r--   0 root         (0) root         (0)    10422 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/journald_conf.py
--rw-r--r--   0 root         (0) root         (0)     4962 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/krb5.py
--rw-r--r--   0 root         (0) root         (0)     2808 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/limits_conf.py
--rw-r--r--   0 root         (0) root         (0)     5296 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/logrotate_conf.py
--rw-r--r--   0 root         (0) root         (0)     6883 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/lspci.py
--rw-r--r--   0 root         (0) root         (0)    13715 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/lvm.py
--rw-r--r--   0 root         (0) root         (0)     1060 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/md5check.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/mlx4_port.py
--rw-r--r--   0 root         (0) root         (0)     3936 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/modinfo.py
--rw-r--r--   0 root         (0) root         (0)     3735 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/modprobe.py
--rw-r--r--   0 root         (0) root         (0)     6028 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/mounts.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/multinode.py
--rw-r--r--   0 root         (0) root         (0)     3725 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/netstat.py
--rw-r--r--   0 root         (0) root         (0)     5551 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/nfs_exports.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/nginx_conf.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/nmcli_dev_show.py
--rw-r--r--   0 root         (0) root         (0)     5079 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/os_release.py
--rw-r--r--   0 root         (0) root         (0)     9951 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/ps.py
--rw-r--r--   0 root         (0) root         (0)     3590 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/redhat_release.py
--rw-r--r--   0 root         (0) root         (0)     3512 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/rhel_for_edge.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/rhsm_release.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/rsyslog_confs.py
--rw-r--r--   0 root         (0) root         (0)     6349 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/sap.py
--rw-r--r--   0 root         (0) root         (0)     8754 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/satellite_version.py
--rw-r--r--   0 root         (0) root         (0)     4702 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/selinux.py
--rw-r--r--   0 root         (0) root         (0)     3245 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/services.py
--rw-r--r--   0 root         (0) root         (0)     2837 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/smt.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/ssl_certificate.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/sudoers.py
--rw-r--r--   0 root         (0) root         (0)     1371 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/sys_vmbus_devices.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/sysctl_conf.py
--rw-r--r--   0 root         (0) root         (0)     2809 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/tmpfilesd.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/tomcat_virtual_dir_context.py
--rw-r--r--   0 root         (0) root         (0)     2472 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/user_namespaces.py
--rw-r--r--   0 root         (0) root         (0)     3545 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/virt_what.py
--rw-r--r--   0 root         (0) root         (0)     4583 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/virt_who_conf.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/combiners/x86_page_branch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/components/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)      885 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/components/ceph.py
--rw-r--r--   0 root         (0) root         (0)     1926 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/components/cloud_provider.py
--rw-r--r--   0 root         (0) root         (0)     2208 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/components/cryptsetup.py
--rw-r--r--   0 root         (0) root         (0)     1000 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/components/openstack.py
--rw-r--r--   0 root         (0) root         (0)     2934 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/components/rhel_version.py
--rw-r--r--   0 root         (0) root         (0)     4134 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/components/satellite.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/components/virtualization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/contrib/
--rw-r--r--   0 root         (0) root         (0)      338 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/contrib/ConfigParser.py
--rw-r--r--   0 root         (0) root         (0)     9473 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/contrib/ElementPath.py
--rw-r--r--   0 root         (0) root         (0)    57035 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/contrib/ElementTree.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/contrib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1327 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/contrib/importlib.py
--rw-r--r--   0 root         (0) root         (0)    72089 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/contrib/ipaddress.py
--rw-r--r--   0 root         (0) root         (0)     6260 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/contrib/magic.py
--rw-r--r--   0 root         (0) root         (0)     5441 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/contrib/nginxparser.py
--rw-r--r--   0 root         (0) root         (0)   164313 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/contrib/pyparsing.py
--rw-r--r--   0 root         (0) root         (0)    37769 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/contrib/soscleaner.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/contrib/toposort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/core/
--rw-r--r--   0 root         (0) root         (0)    68933 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3281 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/archives.py
--rw-r--r--   0 root         (0) root         (0)      628 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/blacklist.py
--rwxr-xr-x   0 root         (0) root         (0)     2712 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/cluster.py
--rw-r--r--   0 root         (0) root         (0)     7213 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/context.py
--rw-r--r--   0 root         (0) root         (0)    36072 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/dr.py
--rw-r--r--   0 root         (0) root         (0)     6053 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/evaluators.py
--rw-r--r--   0 root         (0) root         (0)     3118 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     6959 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/filters.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/hydration.py
--rw-r--r--   0 root         (0) root         (0)     8412 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/ls_parser.py
--rw-r--r--   0 root         (0) root         (0)     1350 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/marshalling.py
--rw-r--r--   0 root         (0) root         (0)    23719 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/plugins.py
--rw-r--r--   0 root         (0) root         (0)     5120 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/remote_resource.py
--rw-r--r--   0 root         (0) root         (0)     8432 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/serde.py
--rw-r--r--   0 root         (0) root         (0)    47657 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/spec_factory.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/core/taglang.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/formats/
--rw-r--r--   0 root         (0) root         (0)     6957 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/formats/__init__.py
--rw-r--r--   0 root         (0) root         (0)      738 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/formats/_json.py
--rw-r--r--   0 root         (0) root         (0)     9124 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/formats/_markdown.py
--rw-r--r--   0 root         (0) root         (0)     4414 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/formats/_syslog.py
--rw-r--r--   0 root         (0) root         (0)      874 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/formats/_yaml.py
--rw-r--r--   0 root         (0) root         (0)     5570 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/formats/html.py
--rw-r--r--   0 root         (0) root         (0)     3778 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/formats/simple_html.py
--rw-r--r--   0 root         (0) root         (0)     3835 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/formats/template.py
--rw-r--r--   0 root         (0) root         (0)     9919 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/formats/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/parsers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/parsers/systemd/
--rw-r--r--   0 root         (0) root         (0)      223 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/systemd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6703 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/systemd/config.py
--rw-r--r--   0 root         (0) root         (0)    11202 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/systemd/unitfiles.py
--rw-r--r--   0 root         (0) root         (0)    23917 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3275 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/abrt_ccpp.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/abrt_status_bare.py
--rw-r--r--   0 root         (0) root         (0)     7334 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/alternatives.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/amq_broker.py
--rw-r--r--   0 root         (0) root         (0)     5722 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/audit_log.py
--rw-r--r--   0 root         (0) root         (0)     3936 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/auditctl.py
--rw-r--r--   0 root         (0) root         (0)     2377 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/auditctl_status.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/auditd_conf.py
--rw-r--r--   0 root         (0) root         (0)     1873 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/authselect.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/autofs_conf.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/avc_cache_threshold.py
--rw-r--r--   0 root         (0) root         (0)     1883 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/avc_hash_stats.py
--rw-r--r--   0 root         (0) root         (0)     4912 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/aws_instance_id.py
--rw-r--r--   0 root         (0) root         (0)     3208 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/awx_manage.py
--rw-r--r--   0 root         (0) root         (0)     5062 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/azure_instance.py
--rw-r--r--   0 root         (0) root         (0)     2778 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/azure_instance_plan.py
--rw-r--r--   0 root         (0) root         (0)     2841 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/azure_instance_type.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/bdi_read_ahead_kb.py
--rw-r--r--   0 root         (0) root         (0)      766 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/blacklisted.py
--rw-r--r--   0 root         (0) root         (0)     3279 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/blkid.py
--rw-r--r--   0 root         (0) root         (0)    10936 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/bond.py
--rw-r--r--   0 root         (0) root         (0)     1968 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/bond_dynamic_lb.py
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/branch_info.py
--rw-r--r--   0 root         (0) root         (0)     4389 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/brctl_show.py
--rw-r--r--   0 root         (0) root         (0)      814 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/candlepin_broker.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/catalina_log.py
--rw-r--r--   0 root         (0) root         (0)     2231 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cciss.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ceilometer_conf.py
--rw-r--r--   0 root         (0) root         (0)    18304 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ceilometer_log.py
--rw-r--r--   0 root         (0) root         (0)     5234 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ceph_cmd_json_parsing.py
--rw-r--r--   0 root         (0) root         (0)     2503 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ceph_conf.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ceph_insights.py
--rw-r--r--   0 root         (0) root         (0)     3026 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ceph_log.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ceph_osd_log.py
--rw-r--r--   0 root         (0) root         (0)     3923 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ceph_osd_tree_text.py
--rw-r--r--   0 root         (0) root         (0)    10372 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ceph_version.py
--rw-r--r--   0 root         (0) root         (0)     3688 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/certificates_enddate.py
--rw-r--r--   0 root         (0) root         (0)     3338 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cgroups.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/checkin_conf.py
--rw-r--r--   0 root         (0) root         (0)     6685 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/chkconfig.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cib.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cinder_conf.py
--rw-r--r--   0 root         (0) root         (0)     2478 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cinder_log.py
--rw-r--r--   0 root         (0) root         (0)     1724 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cloud_cfg.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cloud_init_custom_network.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cloud_init_log.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cluster_conf.py
--rw-r--r--   0 root         (0) root         (0)     2655 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cmdline.py
--rw-r--r--   0 root         (0) root         (0)     1790 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cni_podman_bridge_conf.py
--rw-r--r--   0 root         (0) root         (0)      958 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cobbler_modules_conf.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cobbler_settings.py
--rw-r--r--   0 root         (0) root         (0)     2999 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/config_file_perms.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/containers_inspect.py
--rw-r--r--   0 root         (0) root         (0)     1556 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/containers_policy.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/corosync.py
--rw-r--r--   0 root         (0) root         (0)     2108 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/corosync_cmapctl.py
--rw-r--r--   0 root         (0) root         (0)     1854 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cpu_online.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cpu_vulns.py
--rw-r--r--   0 root         (0) root         (0)     9935 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cpuinfo.py
--rw-r--r--   0 root         (0) root         (0)     4554 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cpupower_frequency_info.py
--rw-r--r--   0 root         (0) root         (0)     2420 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cpuset_cpus.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/crictl_logs.py
--rw-r--r--   0 root         (0) root         (0)     1969 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/crio_conf.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cron_daily_rhsmd.py
--rw-r--r--   0 root         (0) root         (0)     7528 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cron_jobs.py
--rw-r--r--   0 root         (0) root         (0)     8175 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/crontab.py
--rw-r--r--   0 root         (0) root         (0)     4615 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/crypto_policies.py
--rw-r--r--   0 root         (0) root         (0)     6401 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cryptsetup_luksDump.py
--rw-r--r--   0 root         (0) root         (0)     2159 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/cups_ppd.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/current_clocksource.py
--rw-r--r--   0 root         (0) root         (0)     7701 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/date.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/db2.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dcbtool_gc_dcb.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/designate_conf.py
--rw-r--r--   0 root         (0) root         (0)    15843 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/df.py
--rw-r--r--   0 root         (0) root         (0)     5253 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dig.py
--rw-r--r--   0 root         (0) root         (0)     4672 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dirsrv_logs.py
--rw-r--r--   0 root         (0) root         (0)     5551 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dmesg.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dmesg_log.py
--rw-r--r--   0 root         (0) root         (0)     6945 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dmidecode.py
--rw-r--r--   0 root         (0) root         (0)    10764 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dmsetup.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dnf_conf.py
--rw-r--r--   0 root         (0) root         (0)    11733 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dnf_module.py
--rw-r--r--   0 root         (0) root         (0)      764 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dnf_modules.py
--rw-r--r--   0 root         (0) root         (0)     2267 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dnsmasq_config.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/docker_host_machine_id.py
--rw-r--r--   0 root         (0) root         (0)     3776 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/docker_inspect.py
--rw-r--r--   0 root         (0) root         (0)     6667 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/docker_list.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dockerinfo.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dotnet.py
--rw-r--r--   0 root         (0) root         (0)     4504 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/doveconf.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dracut_modules.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dse_ldif_simple.py
--rw-r--r--   0 root         (0) root         (0)     3050 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/du.py
--rw-r--r--   0 root         (0) root         (0)     2555 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/dumpe2fs_h.py
--rw-r--r--   0 root         (0) root         (0)     6803 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/engine_config.py
--rw-r--r--   0 root         (0) root         (0)     1832 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/engine_db_query.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/engine_log.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/etcd_conf.py
--rw-r--r--   0 root         (0) root         (0)    31741 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ethtool.py
--rw-r--r--   0 root         (0) root         (0)     1928 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/facter.py
--rw-r--r--   0 root         (0) root         (0)     1135 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/fapolicyd_rules.py
--rw-r--r--   0 root         (0) root         (0)     2241 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/fc_match.py
--rw-r--r--   0 root         (0) root         (0)     6495 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/fcoeadm_i.py
--rw-r--r--   0 root         (0) root         (0)     4695 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/findmnt.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/firewall_cmd.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/firewall_config.py
--rw-r--r--   0 root         (0) root         (0)    11442 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/foreman_log.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/foreman_proxy_conf.py
--rw-r--r--   0 root         (0) root         (0)     3073 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/foreman_rake_db_migrate_status.py
--rw-r--r--   0 root         (0) root         (0)     2624 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/freeipa_healthcheck_log.py
--rw-r--r--   0 root         (0) root         (0)     8069 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/fstab.py
--rw-r--r--   0 root         (0) root         (0)     5792 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/fwupdagent.py
--rw-r--r--   0 root         (0) root         (0)     2028 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/galera_cnf.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/gcp_instance_type.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/gcp_license_codes.py
--rw-r--r--   0 root         (0) root         (0)     6240 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/getcert_list.py
--rw-r--r--   0 root         (0) root         (0)     1038 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/getconf_pagesize.py
--rw-r--r--   0 root         (0) root         (0)      580 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/getenforce.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/getsebool.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/gfs2_file_system_block_size.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/glance_log.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/gluster_peer_status.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/gluster_vol.py
--rw-r--r--   0 root         (0) root         (0)     3913 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/gnocchi.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/greenboot_status.py
--rw-r--r--   0 root         (0) root         (0)    16140 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/grub_conf.py
--rw-r--r--   0 root         (0) root         (0)     2243 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/grubby.py
--rw-r--r--   0 root         (0) root         (0)     4019 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/grubenv.py
--rw-r--r--   0 root         (0) root         (0)     3642 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/hammer_ping.py
--rw-r--r--   0 root         (0) root         (0)     6471 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/hammer_task_list.py
--rw-r--r--   0 root         (0) root         (0)     3748 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/haproxy_cfg.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/heat_conf.py
--rw-r--r--   0 root         (0) root         (0)     5719 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/heat_log.py
--rw-r--r--   0 root         (0) root         (0)      814 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/host_vdsm_id.py
--rw-r--r--   0 root         (0) root         (0)     3209 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/hostname.py
--rw-r--r--   0 root         (0) root         (0)     3770 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/hosts.py
--rw-r--r--   0 root         (0) root         (0)     3215 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/hponcfg.py
--rw-r--r--   0 root         (0) root         (0)     3014 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/httpd_M.py
--rw-r--r--   0 root         (0) root         (0)     4359 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/httpd_V.py
--rw-r--r--   0 root         (0) root         (0)     6074 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/httpd_conf.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/httpd_log.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/httpd_open_nfs.py
--rw-r--r--   0 root         (0) root         (0)     2136 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ibm_proc.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ifcfg.py
--rw-r--r--   0 root         (0) root         (0)     2867 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/imagemagick_policy.py
--rw-r--r--   0 root         (0) root         (0)     1637 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/init_process_cgroup.py
--rw-r--r--   0 root         (0) root         (0)     3456 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/initscript.py
--rw-r--r--   0 root         (0) root         (0)     1324 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/insights_client_conf.py
--rw-r--r--   0 root         (0) root         (0)     3397 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/installed_product_ids.py
--rw-r--r--   0 root         (0) root         (0)    22541 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/installed_rpms.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/interrupts.py
--rw-r--r--   0 root         (0) root         (0)    23657 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ip.py
--rw-r--r--   0 root         (0) root         (0)     3235 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ip_netns_exec_namespace_lsof.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ipaupgrade_log.py
--rw-r--r--   0 root         (0) root         (0)     6116 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ipcs.py
--rw-r--r--   0 root         (0) root         (0)     3265 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ipsec_conf.py
--rw-r--r--   0 root         (0) root         (0)     8316 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/iptables.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ironic_conf.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ironic_inspector_log.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/iscsiadm_mode_session.py
--rw-r--r--   0 root         (0) root         (0)    11140 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/jboss_domain_log.py
--rw-r--r--   0 root         (0) root         (0)     2293 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/jboss_standalone_main_conf.py
--rw-r--r--   0 root         (0) root         (0)     4053 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/jboss_version.py
--rw-r--r--   0 root         (0) root         (0)     2351 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/journal_all.py
--rw-r--r--   0 root         (0) root         (0)     2439 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/journal_since_boot.py
--rw-r--r--   0 root         (0) root         (0)     5079 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/journalctl.py
--rw-r--r--   0 root         (0) root         (0)     3049 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/journald_conf.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/katello_service_status.py
--rw-r--r--   0 root         (0) root         (0)     9893 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/kdump.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/kernel_config.py
--rw-r--r--   0 root         (0) root         (0)     1259 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/keystone.py
--rw-r--r--   0 root         (0) root         (0)     2929 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/keystone_log.py
--rw-r--r--   0 root         (0) root         (0)     2304 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/kpatch_list.py
--rw-r--r--   0 root         (0) root         (0)     6657 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/krb5.py
--rw-r--r--   0 root         (0) root         (0)     3270 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/krb5kdc_log.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ksmstate.py
--rw-r--r--   0 root         (0) root         (0)      872 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ktimer_lockless.py
--rw-r--r--   0 root         (0) root         (0)     1291 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/kubepods_cpu_quota.py
--rw-r--r--   0 root         (0) root         (0)     2003 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ld_library_path.py
--rw-r--r--   0 root         (0) root         (0)     5357 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ldif_config.py
--rw-r--r--   0 root         (0) root         (0)     3342 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/libssh_config.py
--rw-r--r--   0 root         (0) root         (0)     2771 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/libvirtd_log.py
--rw-r--r--   0 root         (0) root         (0)     7063 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/limits_conf.py
--rw-r--r--   0 root         (0) root         (0)     8553 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/logrotate_conf.py
--rw-r--r--   0 root         (0) root         (0)     2267 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/losetup.py
--rw-r--r--   0 root         (0) root         (0)     4117 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/lpstat.py
--rw-r--r--   0 root         (0) root         (0)     1317 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_boot.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_dev.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_disk.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_docker_volumes.py
--rw-r--r--   0 root         (0) root         (0)     1179 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_edac_mc.py
--rw-r--r--   0 root         (0) root         (0)     4965 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_etc.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_ipa_idoverride_memberof.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_krb5_sssd.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_lib_firmware.py
--rw-r--r--   0 root         (0) root         (0)     1462 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_ocp_cni_openshift_sdn.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_origin_local_volumes_pods.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_osroot.py
--rw-r--r--   0 root         (0) root         (0)     1573 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_sys_firmware.py
--rw-r--r--   0 root         (0) root         (0)     3893 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_systemd_units.py
--rw-r--r--   0 root         (0) root         (0)     2356 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_tmp.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_usr_bin.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_usr_lib64.py
--rw-r--r--   0 root         (0) root         (0)     1785 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_usr_sbin.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_var_cache_pulp.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_var_lib_mongodb.py
--rw-r--r--   0 root         (0) root         (0)     5642 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_var_lib_nova_instances.py
--rw-r--r--   0 root         (0) root         (0)     1076 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_var_lib_pcp.py
--rw-r--r--   0 root         (0) root         (0)      822 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_var_lib_rsyslog.py
--rw-r--r--   0 root         (0) root         (0)     1873 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_var_log.py
--rw-r--r--   0 root         (0) root         (0)      857 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_var_opt_mssql.py
--rw-r--r--   0 root         (0) root         (0)      686 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_var_opt_mssql_log.py
--rw-r--r--   0 root         (0) root         (0)     1120 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_var_run.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_var_spool_clientmq.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_var_spool_postfix_maildrop.py
--rw-r--r--   0 root         (0) root         (0)      995 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_var_tmp.py
--rw-r--r--   0 root         (0) root         (0)     1579 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ls_var_www_perms.py
--rw-r--r--   0 root         (0) root         (0)    13204 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/lsblk.py
--rw-r--r--   0 root         (0) root         (0)     2293 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/lscpu.py
--rw-r--r--   0 root         (0) root         (0)     5399 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/lsinitrd.py
--rw-r--r--   0 root         (0) root         (0)     2099 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/lsmod.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/lsof.py
--rw-r--r--   0 root         (0) root         (0)     6819 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/lspci.py
--rw-r--r--   0 root         (0) root         (0)     4040 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/lssap.py
--rw-r--r--   0 root         (0) root         (0)     3726 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/lsscsi.py
--rw-r--r--   0 root         (0) root         (0)     3544 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/luksmeta.py
--rw-r--r--   0 root         (0) root         (0)     4792 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/lvdisplay.py
--rw-r--r--   0 root         (0) root         (0)    30358 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/lvm.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/manila_conf.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/mariadb_log.py
--rw-r--r--   0 root         (0) root         (0)     1793 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/max_uid.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/md5check.py
--rw-r--r--   0 root         (0) root         (0)     2204 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/mdadm.py
--rw-r--r--   0 root         (0) root         (0)    13622 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/mdstat.py
--rw-r--r--   0 root         (0) root         (0)     7657 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/meminfo.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/messages.py
--rw-r--r--   0 root         (0) root         (0)      261 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/metadata.py
--rw-r--r--   0 root         (0) root         (0)     2360 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/mistral_log.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/mlx4_port.py
--rw-r--r--   0 root         (0) root         (0)    14947 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/modinfo.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/modprobe.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/mokutil_sbstate.py
--rw-r--r--   0 root         (0) root         (0)     6047 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/mongod_conf.py
--rw-r--r--   0 root         (0) root         (0)    17003 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/mount.py
--rw-r--r--   0 root         (0) root         (0)     1097 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/mpirun.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/mssql_api_assessment.py
--rw-r--r--   0 root         (0) root         (0)      901 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/mssql_conf.py
--rw-r--r--   0 root         (0) root         (0)     2144 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/multicast_querier.py
--rw-r--r--   0 root         (0) root         (0)     8381 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/multipath_conf.py
--rw-r--r--   0 root         (0) root         (0)    11281 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/multipath_v4_ll.py
--rw-r--r--   0 root         (0) root         (0)     2088 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/mysql_log.py
--rw-r--r--   0 root         (0) root         (0)     4351 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/mysqladmin.py
--rw-r--r--   0 root         (0) root         (0)     6968 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/named_checkconf.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/named_conf.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ndctl_list.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/net_namespace.py
--rw-r--r--   0 root         (0) root         (0)    35383 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/netstat.py
--rw-r--r--   0 root         (0) root         (0)      842 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/networkmanager_config.py
--rw-r--r--   0 root         (0) root         (0)     3245 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/networkmanager_dhclient.py
--rw-r--r--   0 root         (0) root         (0)     2020 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/neutron_conf.py
--rw-r--r--   0 root         (0) root         (0)     1477 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/neutron_dhcp_agent_conf.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/neutron_l3_agent_conf.py
--rw-r--r--   0 root         (0) root         (0)     1401 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/neutron_l3_agent_log.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/neutron_metadata_agent_conf.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/neutron_metadata_agent_log.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/neutron_ml2_conf.py
--rw-r--r--   0 root         (0) root         (0)     2424 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/neutron_ovs_agent_log.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/neutron_plugin.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/neutron_server_log.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/neutron_sriov_agent.py
--rw-r--r--   0 root         (0) root         (0)     2602 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/nfnetlink_queue.py
--rw-r--r--   0 root         (0) root         (0)     2002 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/nfs_conf.py
--rw-r--r--   0 root         (0) root         (0)     6583 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/nfs_exports.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/nginx_conf.py
--rw-r--r--   0 root         (0) root         (0)     8952 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/nginx_log.py
--rw-r--r--   0 root         (0) root         (0)     7561 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/nmcli.py
--rw-r--r--   0 root         (0) root         (0)     2818 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/nova_conf.py
--rw-r--r--   0 root         (0) root         (0)      716 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/nova_log.py
--rw-r--r--   0 root         (0) root         (0)     2266 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/nova_user_ids.py
--rw-r--r--   0 root         (0) root         (0)     5859 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/nscd_conf.py
--rw-r--r--   0 root         (0) root         (0)     1281 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/nss_rhel7.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/nsswitch_conf.py
--rw-r--r--   0 root         (0) root         (0)     5862 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ntp_sources.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/numa_cpus.py
--rw-r--r--   0 root         (0) root         (0)     2595 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/numeric_user_group_name.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/nvme_core_io_timeout.py
--rw-r--r--   0 root         (0) root         (0)     5310 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/octavia.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/od_cpu_dma_latency.py
--rw-r--r--   0 root         (0) root         (0)     3084 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/odbc.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/open_vm_tools.py
--rw-r--r--   0 root         (0) root         (0)     1134 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/openshift_configuration.py
--rw-r--r--   0 root         (0) root         (0)     8565 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/openshift_get.py
--rw-r--r--   0 root         (0) root         (0)     6322 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/openshift_get_with_config.py
--rw-r--r--   0 root         (0) root         (0)     6410 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/openshift_hosts.py
--rw-r--r--   0 root         (0) root         (0)     2644 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/openvswitch_logs.py
--rw-r--r--   0 root         (0) root         (0)     1352 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/openvswitch_other_config.py
--rw-r--r--   0 root         (0) root         (0)     1995 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/oracle.py
--rw-r--r--   0 root         (0) root         (0)     1756 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/os_release.py
--rw-r--r--   0 root         (0) root         (0)     4166 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/osa_dispatcher_log.py
--rw-r--r--   0 root         (0) root         (0)      339 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ovirt_engine_confd.py
--rw-r--r--   0 root         (0) root         (0)    10113 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ovirt_engine_log.py
--rw-r--r--   0 root         (0) root         (0)     2521 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ovs_appctl_fdb_show_bridge.py
--rw-r--r--   0 root         (0) root         (0)     3192 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ovs_ofctl_dump_flows.py
--rw-r--r--   0 root         (0) root         (0)     3111 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ovs_vsctl.py
--rw-r--r--   0 root         (0) root         (0)     2254 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ovs_vsctl_list_bridge.py
--rw-r--r--   0 root         (0) root         (0)     4161 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ovs_vsctl_show.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/pacemaker_log.py
--rw-r--r--   0 root         (0) root         (0)     2724 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/package_provides.py
--rw-r--r--   0 root         (0) root         (0)    15886 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/pam.py
--rw-r--r--   0 root         (0) root         (0)     9969 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/parted.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/partitions.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/passenger_status.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/password.py
--rw-r--r--   0 root         (0) root         (0)     5810 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/pci_rport_target_disk_paths.py
--rw-r--r--   0 root         (0) root         (0)     1039 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/pcp_openmetrics_log.py
--rw-r--r--   0 root         (0) root         (0)     5734 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/pcs_config.py
--rw-r--r--   0 root         (0) root         (0)     3031 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/pcs_quorum_status.py
--rw-r--r--   0 root         (0) root         (0)     7577 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/pcs_status.py
--rw-r--r--   0 root         (0) root         (0)     6155 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/php_ini.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/pluginconf_d.py
--rw-r--r--   0 root         (0) root         (0)     4095 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/pmlog_summary.py
--rw-r--r--   0 root         (0) root         (0)     2833 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/pmrep.py
--rw-r--r--   0 root         (0) root         (0)     3852 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/podman_inspect.py
--rw-r--r--   0 root         (0) root         (0)     3502 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/podman_list.py
--rw-r--r--   0 root         (0) root         (0)     2921 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/postconf.py
--rw-r--r--   0 root         (0) root         (0)     6788 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/postgresql_conf.py
--rw-r--r--   0 root         (0) root         (0)     1807 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/postgresql_log.py
--rw-r--r--   0 root         (0) root         (0)     2634 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/proc_environ.py
--rw-r--r--   0 root         (0) root         (0)     4659 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/proc_keys.py
--rw-r--r--   0 root         (0) root         (0)     5230 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/proc_limits.py
--rw-r--r--   0 root         (0) root         (0)     6847 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/proc_stat.py
--rw-r--r--   0 root         (0) root         (0)    20696 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ps.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/pulp_worker_defaults.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/puppet_ca_cert_expire_date.py
--rw-r--r--   0 root         (0) root         (0)     1802 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/qemu_conf.py
--rw-r--r--   0 root         (0) root         (0)    13011 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/qemu_xml.py
--rw-r--r--   0 root         (0) root         (0)    12343 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/qpid_stat.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/qpidd_conf.py
--rw-r--r--   0 root         (0) root         (0)    10449 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     4623 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rabbitmq_log.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rc_local.py
--rw-r--r--   0 root         (0) root         (0)     2185 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rdma_config.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/readlink_e_mtab.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/readlink_openshift_certs.py
--rw-r--r--   0 root         (0) root         (0)     4095 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/redhat_release.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/resolv_conf.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rhev_data_center.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rhn_charsets.py
--rw-r--r--   0 root         (0) root         (0)     2434 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rhn_conf.py
--rw-r--r--   0 root         (0) root         (0)     3553 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rhn_entitlement_cert_xml.py
--rw-r--r--   0 root         (0) root         (0)      678 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rhn_hibernate_conf.py
--rw-r--r--   0 root         (0) root         (0)     7383 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rhn_logs.py
--rw-r--r--   0 root         (0) root         (0)     6474 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rhn_schema_stats.py
--rw-r--r--   0 root         (0) root         (0)      771 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rhn_schema_version.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rhosp_release.py
--rw-r--r--   0 root         (0) root         (0)     2803 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rhsm_conf.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rhsm_log.py
--rw-r--r--   0 root         (0) root         (0)     2139 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rhsm_releasever.py
--rw-r--r--   0 root         (0) root         (0)      575 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rhv_log_collector_analyzer.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rndc_status.py
--rw-r--r--   0 root         (0) root         (0)     4953 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ros_config.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/route.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rpm_ostree_status.py
--rw-r--r--   0 root         (0) root         (0)     1431 2023-02-23 12:17:09.000000 insights-core-3.1.9/insights/parsers/rpm_pkgs.py
--rw-r--r--   0 root         (0) root         (0)     2068 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rpm_v_packages.py
--rw-r--r--   0 root         (0) root         (0)     3922 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rpm_vercmp.py
--rw-r--r--   0 root         (0) root         (0)     3019 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/rsyslog_conf.py
--rw-r--r--   0 root         (0) root         (0)     6879 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/samba.py
--rw-r--r--   0 root         (0) root         (0)     2817 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/samba_logs.py
--rw-r--r--   0 root         (0) root         (0)     8418 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sap_dev_trace_files.py
--rw-r--r--   0 root         (0) root         (0)     3032 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sap_hana_python_script.py
--rw-r--r--   0 root         (0) root         (0)     3202 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sap_hdb_version.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sap_host_profile.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sapcontrol.py
--rw-r--r--   0 root         (0) root         (0)     4363 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/saphostctrl.py
--rw-r--r--   0 root         (0) root         (0)     5522 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/saphostexec.py
--rw-r--r--   0 root         (0) root         (0)     1505 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sat5_insights_properties.py
--rw-r--r--   0 root         (0) root         (0)     1473 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/satellite_content_hosts_count.py
--rw-r--r--   0 root         (0) root         (0)     1433 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/satellite_enabled_features.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/satellite_installer_configurations.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/satellite_missed_queues.py
--rw-r--r--   0 root         (0) root         (0)     3452 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/satellite_mongodb.py
--rw-r--r--   0 root         (0) root         (0)    15063 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/satellite_postgresql_query.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/satellite_version.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/satellite_yaml.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     3501 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/scsi.py
--rw-r--r--   0 root         (0) root         (0)     1823 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/scsi_eh_deadline.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/scsi_fwver.py
--rw-r--r--   0 root         (0) root         (0)    14838 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sctp.py
--rw-r--r--   0 root         (0) root         (0)     4408 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sealert.py
--rw-r--r--   0 root         (0) root         (0)     1544 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/secure.py
--rw-r--r--   0 root         (0) root         (0)     1538 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/selinux_config.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/semanage.py
--rw-r--r--   0 root         (0) root         (0)     3426 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sendq_recvq_socket_buffer.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sestatus.py
--rw-r--r--   0 root         (0) root         (0)     2759 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/setup_named_chroot.py
--rw-r--r--   0 root         (0) root         (0)     5122 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/slabinfo.py
--rw-r--r--   0 root         (0) root         (0)     8746 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/smartctl.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/smartpdc_settings.py
--rw-r--r--   0 root         (0) root         (0)     4384 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/smbstatus.py
--rw-r--r--   0 root         (0) root         (0)     4801 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/smt.py
--rw-r--r--   0 root         (0) root         (0)     5214 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/snmp.py
--rw-r--r--   0 root         (0) root         (0)     3672 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sockstat.py
--rw-r--r--   0 root         (0) root         (0)     6210 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/softnet_stat.py
--rw-r--r--   0 root         (0) root         (0)     2017 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/software_collections_list.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sos_conf.py
--rw-r--r--   0 root         (0) root         (0)     1758 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/spamassassin_channels.py
--rw-r--r--   0 root         (0) root         (0)     9175 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ssh.py
--rw-r--r--   0 root         (0) root         (0)    12585 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ssh_client_config.py
--rw-r--r--   0 root         (0) root         (0)    12225 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/ssl_certificate.py
--rw-r--r--   0 root         (0) root         (0)     3663 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sssd_conf.py
--rw-r--r--   0 root         (0) root         (0)     3178 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sssd_logs.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/subscription_manager.py
--rw-r--r--   0 root         (0) root         (0)     8374 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/subscription_manager_list.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/subscription_manager_release.py
--rw-r--r--   0 root         (0) root         (0)     4041 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sudoers.py
--rw-r--r--   0 root         (0) root         (0)     4353 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/swift_conf.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/swift_log.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sys_bus.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sys_fs_cgroup_memory.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sys_fs_cgroup_memory_tasks_number.py
--rw-r--r--   0 root         (0) root         (0)     2183 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sys_kernel.py
--rwxr-xr-x   0 root         (0) root         (0)     5878 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sys_module.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sys_vmbus.py
--rw-r--r--   0 root         (0) root         (0)    21345 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sysconfig.py
--rw-r--r--   0 root         (0) root         (0)     5165 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/sysctl.py
--rw-r--r--   0 root         (0) root         (0)    10809 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/system_time.py
--rw-r--r--   0 root         (0) root         (0)     9992 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/systemctl_show.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/systemctl_status_all.py
--rw-r--r--   0 root         (0) root         (0)     3352 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/systemd_analyze.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/systemid.py
--rw-r--r--   0 root         (0) root         (0)     5051 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/systool.py
--rw-r--r--   0 root         (0) root         (0)      225 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/tags.py
--rw-r--r--   0 root         (0) root         (0)     1974 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/teamdctl_config_dump.py
--rw-r--r--   0 root         (0) root         (0)     2112 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/teamdctl_state_dump.py
--rw-r--r--   0 root         (0) root         (0)     2405 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/tmpfilesd.py
--rw-r--r--   0 root         (0) root         (0)     3111 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/tomcat_virtual_dir_context.py
--rw-r--r--   0 root         (0) root         (0)     6264 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/tomcat_xml.py
--rw-r--r--   0 root         (0) root         (0)     2185 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/transparent_hugepage.py
--rw-r--r--   0 root         (0) root         (0)     2317 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/tuned.py
--rw-r--r--   0 root         (0) root         (0)     1244 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/tuned_conf.py
--rw-r--r--   0 root         (0) root         (0)     3974 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/udev_rules.py
--rw-r--r--   0 root         (0) root         (0)    21241 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/uname.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/up2date_log.py
--rw-r--r--   0 root         (0) root         (0)     4786 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/upstart.py
--rw-r--r--   0 root         (0) root         (0)     3585 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/uptime.py
--rw-r--r--   0 root         (0) root         (0)     2271 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/user_group.py
--rw-r--r--   0 root         (0) root         (0)     6983 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/vdo_status.py
--rw-r--r--   0 root         (0) root         (0)     2515 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/vdsm_conf.py
--rw-r--r--   0 root         (0) root         (0)    11713 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/vdsm_log.py
--rw-r--r--   0 root         (0) root         (0)     1552 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/version_info.py
--rw-r--r--   0 root         (0) root         (0)     6436 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/vgdisplay.py
--rw-r--r--   0 root         (0) root         (0)     4794 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/virsh_list_all.py
--rw-r--r--   0 root         (0) root         (0)      626 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/virt_uuid_facts.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/virt_what.py
--rw-r--r--   0 root         (0) root         (0)     1776 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/virt_who_conf.py
--rw-r--r--   0 root         (0) root         (0)     3341 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/virtlogd_conf.py
--rw-r--r--   0 root         (0) root         (0)     1129 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/vma_ra_enabled_s390x.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/vmcore_dmesg.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/vmware_tools_conf.py
--rw-r--r--   0 root         (0) root         (0)     3679 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/vsftpd.py
--rw-r--r--   0 root         (0) root         (0)     1467 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/wc_proc_1_mountinfo.py
--rw-r--r--   0 root         (0) root         (0)     3436 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/x86_debug.py
--rw-r--r--   0 root         (0) root         (0)     8459 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/xfs_info.py
--rw-r--r--   0 root         (0) root         (0)     3833 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/xinetd_conf.py
--rw-r--r--   0 root         (0) root         (0)     7932 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/yum.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/yum_conf.py
--rw-r--r--   0 root         (0) root         (0)     7787 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/yum_list.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/yum_repos_d.py
--rw-r--r--   0 root         (0) root         (0)     1391 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/yum_updateinfo.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/yum_updates.py
--rw-r--r--   0 root         (0) root         (0)     5405 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/yumlog.py
--rw-r--r--   0 root         (0) root         (0)     3895 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/zdump_v.py
--rw-r--r--   0 root         (0) root         (0)     4535 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsers/zipl_conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/parsr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/parsr/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/parsr/examples/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/tests/test_arith.py
--rw-r--r--   0 root         (0) root         (0)     4256 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/tests/test_corosync.py
--rw-r--r--   0 root         (0) root         (0)     4826 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/tests/test_httpd.py
--rw-r--r--   0 root         (0) root         (0)     2956 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/tests/test_kvpairs.py
--rw-r--r--   0 root         (0) root         (0)     1933 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/tests/test_logrotate.py
--rw-r--r--   0 root         (0) root         (0)     3966 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/tests/test_multipath.py
--rw-r--r--   0 root         (0) root         (0)     5747 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/tests/test_nginx.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/arith.py
--rw-r--r--   0 root         (0) root         (0)     1318 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/corosync_conf.py
--rw-r--r--   0 root         (0) root         (0)     1478 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/httpd_conf.py
--rw-r--r--   0 root         (0) root         (0)     2201 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/iniparser.py
--rw-r--r--   0 root         (0) root         (0)      898 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/json_parser.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/kvpairs.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/logrotate_conf.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/multipath_conf.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/examples/nginx_conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/parsr/query/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/parsr/query/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/query/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/query/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     4076 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/query/tests/test_choose.py
--rw-r--r--   0 root         (0) root         (0)     1118 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/query/tests/test_compile_queries.py
--rw-r--r--   0 root         (0) root         (0)     3301 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/query/tests/test_crumbs.py
--rw-r--r--   0 root         (0) root         (0)     1083 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/query/tests/test_find.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/query/tests/test_query.py
--rw-r--r--   0 root         (0) root         (0)     3171 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/query/tests/test_where.py
--rw-r--r--   0 root         (0) root         (0)    30926 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4602 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/query/boolean.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/parsr/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      210 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)      151 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/tests/test_forward.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/tests/test_function_error.py
--rw-r--r--   0 root         (0) root         (0)     1975 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/tests/test_iniparser.py
--rw-r--r--   0 root         (0) root         (0)      453 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/tests/test_keep.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/tests/test_literal.py
--rw-r--r--   0 root         (0) root         (0)     1226 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/tests/test_many.py
--rw-r--r--   0 root         (0) root         (0)      351 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/tests/test_number.py
--rw-r--r--   0 root         (0) root         (0)      220 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/tests/test_opt.py
--rw-r--r--   0 root         (0) root         (0)     1798 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/tests/test_pos_marker.py
--rw-r--r--   0 root         (0) root         (0)      522 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/tests/test_string.py
--rw-r--r--   0 root         (0) root         (0)      161 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/tests/test_until.py
--rw-r--r--   0 root         (0) root         (0)    40965 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4197 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/parsr/iniparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      151 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/plugins/always_fires.py
--rw-r--r--   0 root         (0) root         (0)      268 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/plugins/info.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/plugins/insights_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)      194 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/plugins/never_fires.py
--rw-r--r--   0 root         (0) root         (0)      513 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/plugins/ps_rule_fakes.py
--rw-r--r--   0 root         (0) root         (0)      492 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/plugins/returns_none.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/plugins/rules_fixture_plugin.py
--rw-r--r--   0 root         (0) root         (0)      257 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/plugins/vulnerable_kernel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/specs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/specs/datasources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/specs/datasources/container/
--rw-r--r--   0 root         (0) root         (0)     2842 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/container/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4064 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/container/containers_inspect.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/container/nginx_conf.py
--rw-r--r--   0 root         (0) root         (0)     1955 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1444 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/aws.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/awx_manage.py
--rw-r--r--   0 root         (0) root         (0)     3252 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/candlepin_broker.py
--rw-r--r--   0 root         (0) root         (0)     2905 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/cloud_init.py
--rw-r--r--   0 root         (0) root         (0)     1140 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/corosync.py
--rw-r--r--   0 root         (0) root         (0)      521 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/dir_list.py
--rw-r--r--   0 root         (0) root         (0)     3158 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/ethernet.py
--rw-r--r--   0 root         (0) root         (0)     2139 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/httpd.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/ipcs.py
--rw-r--r--   0 root         (0) root         (0)      571 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/kernel.py
--rw-r--r--   0 root         (0) root         (0)      860 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/kernel_module_list.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/lpstat.py
--rw-r--r--   0 root         (0) root         (0)     4104 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/luks_devices.py
--rw-r--r--   0 root         (0) root         (0)     1928 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/malware_detection.py
--rw-r--r--   0 root         (0) root         (0)      574 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/md5chk.py
--rw-r--r--   0 root         (0) root         (0)     2753 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/package_provides.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/pcp.py
--rw-r--r--   0 root         (0) root         (0)     4469 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/ps.py
--rw-r--r--   0 root         (0) root         (0)     3892 2023-02-23 12:17:09.000000 insights-core-3.1.9/insights/specs/datasources/rpm_pkgs.py
--rw-r--r--   0 root         (0) root         (0)     2770 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/sap.py
--rw-r--r--   0 root         (0) root         (0)     4542 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/satellite_missed_queues.py
--rw-r--r--   0 root         (0) root         (0)     1733 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/semanage.py
--rw-r--r--   0 root         (0) root         (0)     3498 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/ssl_certificate.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/sys_fs_cgroup_memory.py
--rw-r--r--   0 root         (0) root         (0)     1786 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/sys_fs_cgroup_memory_tasks_number.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/user_group.py
--rw-r--r--   0 root         (0) root         (0)     7773 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/datasources/yum_updates.py
--rw-r--r--   0 root         (0) root         (0)    35287 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/core3_archive.py
--rw-r--r--   0 root         (0) root         (0)    48375 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/default.py
--rw-r--r--   0 root         (0) root         (0)    24800 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/insights_archive.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/jdr_archive.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/must_gather_archive.py
--rw-r--r--   0 root         (0) root         (0)    24450 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/specs/sos_archive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/tests/combiners/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2465 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_ansible_info.py
--rw-r--r--   0 root         (0) root         (0)     7843 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_ceph_osd_tree.py
--rw-r--r--   0 root         (0) root         (0)     4682 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_ceph_version.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_cloud_instance.py
--rw-r--r--   0 root         (0) root         (0)    20466 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_cloud_provider.py
--rw-r--r--   0 root         (0) root         (0)     4405 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_cpu_vulns_all.py
--rw-r--r--   0 root         (0) root         (0)     1808 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_crio_conf.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_cryptsetup.py
--rw-r--r--   0 root         (0) root         (0)     3170 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_dmesg.py
--rw-r--r--   0 root         (0) root         (0)     3781 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_dnsmasq_conf_all.py
--rw-r--r--   0 root         (0) root         (0)     1003 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_du.py
--rw-r--r--   0 root         (0) root         (0)    30578 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_grub_conf.py
--rw-r--r--   0 root         (0) root         (0)     3236 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_hostname.py
--rw-r--r--   0 root         (0) root         (0)    30446 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_httpd_conf_tree.py
--rw-r--r--   0 root         (0) root         (0)     4690 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_ipcs_semaphores.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_ipcs_shared_memory.py
--rw-r--r--   0 root         (0) root         (0)     6424 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_ipv6.py
--rw-r--r--   0 root         (0) root         (0)    17768 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_journald_conf.py
--rw-r--r--   0 root         (0) root         (0)     3276 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_krb5.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_limits_conf.py
--rw-r--r--   0 root         (0) root         (0)     4294 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_logrotate_conf.py
--rw-r--r--   0 root         (0) root         (0)     2546 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_logrotate_conf_tree.py
--rw-r--r--   0 root         (0) root         (0)     9507 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_lspci.py
--rw-r--r--   0 root         (0) root         (0)    62274 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_lvm.py
--rw-r--r--   0 root         (0) root         (0)     1136 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_md5check.py
--rw-r--r--   0 root         (0) root         (0)     1132 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_mlx4_port.py
--rw-r--r--   0 root         (0) root         (0)     1600 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_modinfo.py
--rw-r--r--   0 root         (0) root         (0)     3503 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_modprobe.py
--rw-r--r--   0 root         (0) root         (0)    11117 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_mounts.py
--rw-r--r--   0 root         (0) root         (0)     8578 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_netstat.py
--rw-r--r--   0 root         (0) root         (0)     4681 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_nfs_exports.py
--rw-r--r--   0 root         (0) root         (0)    11093 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_nginx_conf.py
--rw-r--r--   0 root         (0) root         (0)     5480 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_nmcli_dev_show.py
--rw-r--r--   0 root         (0) root         (0)    11557 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_os_release.py
--rw-r--r--   0 root         (0) root         (0)    14650 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_ps.py
--rw-r--r--   0 root         (0) root         (0)     2410 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_redhat_release.py
--rw-r--r--   0 root         (0) root         (0)    13944 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_rhel_for_edge.py
--rw-r--r--   0 root         (0) root         (0)     1324 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_rhsm_release.py
--rw-r--r--   0 root         (0) root         (0)     6262 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_rsyslog_confs.py
--rw-r--r--   0 root         (0) root         (0)     9437 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_sap.py
--rw-r--r--   0 root         (0) root         (0)     9872 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_satellite_version.py
--rw-r--r--   0 root         (0) root         (0)    16559 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_selinux.py
--rw-r--r--   0 root         (0) root         (0)     3149 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_services.py
--rw-r--r--   0 root         (0) root         (0)     5788 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_smt.py
--rw-r--r--   0 root         (0) root         (0)     5198 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_ssl_certificate.py
--rw-r--r--   0 root         (0) root         (0)     2547 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_sudoers.py
--rw-r--r--   0 root         (0) root         (0)     2443 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_sys_vmbus_devices.py
--rw-r--r--   0 root         (0) root         (0)     2957 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_sysctl_conf.py
--rw-r--r--   0 root         (0) root         (0)     4392 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_tmpfilesd.py
--rw-r--r--   0 root         (0) root         (0)     5802 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_tomcat_virtual_dir_context.py
--rw-r--r--   0 root         (0) root         (0)     4553 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_user_namespaces.py
--rw-r--r--   0 root         (0) root         (0)    11989 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_virt_what.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_virt_who_conf.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/combiners/test_x86_page_branch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/tests/components/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/components/test_ceph.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/components/test_cloud_provider.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/components/test_cryptsetup.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/components/test_openstack.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/components/test_rhel_version.py
--rw-r--r--   0 root         (0) root         (0)     4052 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/components/test_satellite.py
--rw-r--r--   0 root         (0) root         (0)      543 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/components/test_virtualization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/tests/datasources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/tests/datasources/container/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/container/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44018 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/container/test_containers_inspect.py
--rw-r--r--   0 root         (0) root         (0)     2501 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/container/test_nginx_conf.py
--rw-r--r--   0 root         (0) root         (0)     5189 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/container/test_running_rhel_containers.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/__init__.py
--rw-r--r--   0 root         (0) root         (0)      854 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_aws.py
--rw-r--r--   0 root         (0) root         (0)     3306 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_awx_manage.py
--rw-r--r--   0 root         (0) root         (0)    10281 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_candlepin_broker.py
--rw-r--r--   0 root         (0) root         (0)     3572 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_cloud_init.py
--rw-r--r--   0 root         (0) root         (0)     1538 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_corosync.py
--rw-r--r--   0 root         (0) root         (0)     4168 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_datasource_timeout.py
--rw-r--r--   0 root         (0) root         (0)      882 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_dir_list.py
--rw-r--r--   0 root         (0) root         (0)     3702 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_ethernet.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_get_running_commands.py
--rw-r--r--   0 root         (0) root         (0)     2365 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_httpd.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_ipcs.py
--rw-r--r--   0 root         (0) root         (0)      840 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_kernel.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_kernel_module_list.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_lpstat.py
--rw-r--r--   0 root         (0) root         (0)     7739 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_luks_devices.py
--rw-r--r--   0 root         (0) root         (0)     5915 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_package_provides.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_pcp.py
--rw-r--r--   0 root         (0) root         (0)     4895 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_ps.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-02-23 12:17:09.000000 insights-core-3.1.9/insights/tests/datasources/test_rpm_pkgs.py
--rw-r--r--   0 root         (0) root         (0)     8411 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_sap.py
--rw-r--r--   0 root         (0) root         (0)    17158 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_satellite_missed_queues.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_semanage.py
--rw-r--r--   0 root         (0) root         (0)     9201 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_ssl_certificate.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_sys_fs_cgroup_memory.py
--rw-r--r--   0 root         (0) root         (0)     3680 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_sys_fs_cgroup_memory_tasks_number.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_user_group.py
--rw-r--r--   0 root         (0) root         (0)     2266 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/datasources/test_yum_updates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/tests/parsers/
--rw-r--r--   0 root         (0) root         (0)     2167 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6755 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/lvm_test_data.py
--rw-r--r--   0 root         (0) root         (0)     3035 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_abrt_ccpp.py
--rw-r--r--   0 root         (0) root         (0)      768 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_abrt_status_bare.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_alternatives.py
--rw-r--r--   0 root         (0) root         (0)    11425 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_amq_broker.py
--rw-r--r--   0 root         (0) root         (0)     6787 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     3439 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_auditctl.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_auditctl_status.py
--rw-r--r--   0 root         (0) root         (0)     3399 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_auditd_conf.py
--rw-r--r--   0 root         (0) root         (0)     1362 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_authselect.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_autofs_conf.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_avc_cache_threshold.py
--rw-r--r--   0 root         (0) root         (0)      732 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_avc_hash_stats.py
--rw-r--r--   0 root         (0) root         (0)     8434 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_aws_instance_id.py
--rw-r--r--   0 root         (0) root         (0)     3799 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_awx_manage.py
--rw-r--r--   0 root         (0) root         (0)     5966 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_azure_instance.py
--rw-r--r--   0 root         (0) root         (0)     2684 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_azure_instance_plan.py
--rw-r--r--   0 root         (0) root         (0)     2731 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_azure_instance_type.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_bdi_read_ahead_kb.py
--rw-r--r--   0 root         (0) root         (0)      716 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_blacklisted.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_blkid.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_bond.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_bond_dynamic_lb.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_branch_info.py
--rw-r--r--   0 root         (0) root         (0)     2928 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_brctl_show.py
--rw-r--r--   0 root         (0) root         (0)     5960 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_candlepin_broker.py
--rw-r--r--   0 root         (0) root         (0)    16098 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_catalina_log.py
--rw-r--r--   0 root         (0) root         (0)     1455 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cciss.py
--rw-r--r--   0 root         (0) root         (0)    24431 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ceilometer_conf.py
--rw-r--r--   0 root         (0) root         (0)    13733 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ceilometer_log.py
--rw-r--r--   0 root         (0) root         (0)    26668 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ceph_cmd_json_parsing.py
--rw-r--r--   0 root         (0) root         (0)     2222 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ceph_conf.py
--rw-r--r--   0 root         (0) root         (0)    40877 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ceph_insights.py
--rw-r--r--   0 root         (0) root         (0)     2986 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ceph_log.py
--rw-r--r--   0 root         (0) root         (0)     1973 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ceph_osd_log.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ceph_osd_tree_text.py
--rw-r--r--   0 root         (0) root         (0)     4128 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ceph_version.py
--rw-r--r--   0 root         (0) root         (0)     4602 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_certificates_enddate.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cgroups.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_checkin_conf.py
--rw-r--r--   0 root         (0) root         (0)     3865 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_chkconfig.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cib.py
--rw-r--r--   0 root         (0) root         (0)    32878 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cinder_conf.py
--rw-r--r--   0 root         (0) root         (0)     3937 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cinder_log.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cloud_cfg.py
--rw-r--r--   0 root         (0) root         (0)      987 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cloud_init_custom_network.py
--rw-r--r--   0 root         (0) root         (0)     1034 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cloud_init_log.py
--rw-r--r--   0 root         (0) root         (0)     1619 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cluster_conf.py
--rw-r--r--   0 root         (0) root         (0)     2356 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cmdline.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cni_podman_bridge_conf.py
--rw-r--r--   0 root         (0) root         (0)     3467 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cobbler_modules_conf.py
--rw-r--r--   0 root         (0) root         (0)    15451 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cobbler_settings.py
--rw-r--r--   0 root         (0) root         (0)     1859 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_config_file_perms.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_containers_inspect.py
--rw-r--r--   0 root         (0) root         (0)     1538 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_containers_policy.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_corosync.py
--rw-r--r--   0 root         (0) root         (0)     4540 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_corosync_cmapctl.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cpu_online.py
--rw-r--r--   0 root         (0) root         (0)     6120 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cpu_vulns.py
--rw-r--r--   0 root         (0) root         (0)    63388 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cpuinfo.py
--rw-r--r--   0 root         (0) root         (0)     6646 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cpupower_frequency_info.py
--rw-r--r--   0 root         (0) root         (0)     1305 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cpuset_cpus.py
--rw-r--r--   0 root         (0) root         (0)     1233 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_crictl_logs.py
--rw-r--r--   0 root         (0) root         (0)     2296 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_crio_conf.py
--rw-r--r--   0 root         (0) root         (0)     1076 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cron_daily_rhsmd.py
--rw-r--r--   0 root         (0) root         (0)     4957 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cron_jobs.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_crontab.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_crypto_policies_bind.py
--rw-r--r--   0 root         (0) root         (0)     1339 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_crypto_policies_config.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_crypto_policies_doc_examples.py
--rw-r--r--   0 root         (0) root         (0)     6003 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_crypto_policies_opensshserver.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_crypto_policies_state_current.py
--rw-r--r--   0 root         (0) root         (0)     5541 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cryptsetup_luksDump.py
--rw-r--r--   0 root         (0) root         (0)     1838 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_cups_ppd.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_current_clocksource.py
--rw-r--r--   0 root         (0) root         (0)     6691 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_date.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_db2.py
--rw-r--r--   0 root         (0) root         (0)      835 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dcbtool_gc_dcb.py
--rw-r--r--   0 root         (0) root         (0)     1191 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_designate_conf.py
--rw-r--r--   0 root         (0) root         (0)    13735 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_df.py
--rw-r--r--   0 root         (0) root         (0)     6069 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dig.py
--rw-r--r--   0 root         (0) root         (0)     3480 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dirsrv_logs.py
--rw-r--r--   0 root         (0) root         (0)     4406 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dmesg.py
--rw-r--r--   0 root         (0) root         (0)     1798 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dmesg_log.py
--rw-r--r--   0 root         (0) root         (0)    18156 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dmidecode.py
--rw-r--r--   0 root         (0) root         (0)     8736 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dmsetup.py
--rw-r--r--   0 root         (0) root         (0)     2206 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dnf_conf.py
--rw-r--r--   0 root         (0) root         (0)    13198 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dnf_module.py
--rw-r--r--   0 root         (0) root         (0)      879 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dnf_modules.py
--rw-r--r--   0 root         (0) root         (0)     1267 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dnsmasq_config.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_docker_host_machine-id.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_docker_info.py
--rw-r--r--   0 root         (0) root         (0)    10340 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_docker_inspect.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_docker_list.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dotnet.py
--rw-r--r--   0 root         (0) root         (0)     4820 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_doveconf.py
--rw-r--r--   0 root         (0) root         (0)     1321 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dracut_modules.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dse_ldif_simple.py
--rw-r--r--   0 root         (0) root         (0)     4313 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_du.py
--rw-r--r--   0 root         (0) root         (0)     1993 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_dumpe2fs_h.py
--rw-r--r--   0 root         (0) root         (0)    22800 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_engine_config.py
--rw-r--r--   0 root         (0) root         (0)     3364 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_engine_db_query.py
--rw-r--r--   0 root         (0) root         (0)     2040 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_engine_log.py
--rw-r--r--   0 root         (0) root         (0)      940 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_etcd_conf.py
--rw-r--r--   0 root         (0) root         (0)    24647 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ethtool.py
--rw-r--r--   0 root         (0) root         (0)     3276 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_facter.py
--rw-r--r--   0 root         (0) root         (0)     1109 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_fapolicyd_rules.py
--rw-r--r--   0 root         (0) root         (0)     1132 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_fc_match.py
--rw-r--r--   0 root         (0) root         (0)     3449 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_fcoeadm_i.py
--rw-r--r--   0 root         (0) root         (0)    14400 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_findmnt.py
--rw-r--r--   0 root         (0) root         (0)     4134 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_firewall_cmd.py
--rw-r--r--   0 root         (0) root         (0)    25804 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_foreman_log.py
--rw-r--r--   0 root         (0) root         (0)     1090 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_firewall_config.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_foreman_proxy_conf.py
--rw-r--r--   0 root         (0) root         (0)     2776 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_foreman_rake_db_migrate_status.py
--rw-r--r--   0 root         (0) root         (0)     3949 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_freeipa_healthcheck_log.py
--rw-r--r--   0 root         (0) root         (0)     7434 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_fstab.py
--rw-r--r--   0 root         (0) root         (0)     5701 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_fwupdagent.py
--rw-r--r--   0 root         (0) root         (0)     1317 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_galera_cnf.py
--rw-r--r--   0 root         (0) root         (0)     2659 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_gcp_instance_type.py
--rw-r--r--   0 root         (0) root         (0)     2422 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_gcp_license_codes.py
--rw-r--r--   0 root         (0) root         (0)     4706 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_getcert_list.py
--rw-r--r--   0 root         (0) root         (0)      723 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_getconf_pagesize.py
--rw-r--r--   0 root         (0) root         (0)      584 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_getenforce.py
--rw-r--r--   0 root         (0) root         (0)     1244 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_getsebool.py
--rw-r--r--   0 root         (0) root         (0)     1281 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_gfs2_file_system_block_size.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_glance_log.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_gluster_peer_status.py
--rw-r--r--   0 root         (0) root         (0)    12420 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_gluster_vol.py
--rw-r--r--   0 root         (0) root         (0)     3049 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_gnocchi.py
--rw-r--r--   0 root         (0) root         (0)     5284 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_greenboot_status.py
--rw-r--r--   0 root         (0) root         (0)    13468 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_grub_conf.py
--rw-r--r--   0 root         (0) root         (0)     4751 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_grub_conf_efi.py
--rw-r--r--   0 root         (0) root         (0)    17510 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_grub_conf_kdump.py
--rw-r--r--   0 root         (0) root         (0)    11788 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_grub_conf_missing_boot_files.py
--rw-r--r--   0 root         (0) root         (0)     2156 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_grubby.py
--rw-r--r--   0 root         (0) root         (0)     3318 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_grubenv.py
--rw-r--r--   0 root         (0) root         (0)     7224 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_hammer_ping.py
--rw-r--r--   0 root         (0) root         (0)    11359 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_hammer_task_list.py
--rw-r--r--   0 root         (0) root         (0)    10536 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_haproxy_cfg.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_heat_conf.py
--rw-r--r--   0 root         (0) root         (0)     2467 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_heat_log.py
--rw-r--r--   0 root         (0) root         (0)      333 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_host_vdsm_id.py
--rw-r--r--   0 root         (0) root         (0)     2385 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_hostname.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_hosts.py
--rw-r--r--   0 root         (0) root         (0)      667 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_hponcfg.py
--rw-r--r--   0 root         (0) root         (0)     3006 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_httpd_M.py
--rw-r--r--   0 root         (0) root         (0)     4517 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_httpd_V.py
--rw-r--r--   0 root         (0) root         (0)     6631 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_httpd_conf.py
--rw-r--r--   0 root         (0) root         (0)     7486 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_httpd_log.py
--rw-r--r--   0 root         (0) root         (0)      954 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_httpd_open_nfs.py
--rw-r--r--   0 root         (0) root         (0)     1276 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ibm_proc.py
--rw-r--r--   0 root         (0) root         (0)     8986 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ifcfg.py
--rw-r--r--   0 root         (0) root         (0)     3653 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_imagemagick_policy.py
--rw-r--r--   0 root         (0) root         (0)     3366 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_init_process_cgroup.py
--rw-r--r--   0 root         (0) root         (0)     4537 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_initscript.py
--rw-r--r--   0 root         (0) root         (0)     1069 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_insights_client_conf.py
--rw-r--r--   0 root         (0) root         (0)     2516 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_installed_product_ids.py
--rw-r--r--   0 root         (0) root         (0)    27054 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_installed_rpms.py
--rw-r--r--   0 root         (0) root         (0)     6378 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_interrupts.py
--rw-r--r--   0 root         (0) root         (0)    40045 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ip.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ip_netns_exec_namespace_lsof.py
--rw-r--r--   0 root         (0) root         (0)      722 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ipaupgrade_log.py
--rw-r--r--   0 root         (0) root         (0)     3777 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ipcs.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ipsec_conf.py
--rw-r--r--   0 root         (0) root         (0)     9241 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_iptables.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ironic_conf.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ironic_inspector_log.py
--rw-r--r--   0 root         (0) root         (0)     1234 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_iscsiadm_mode_session.py
--rw-r--r--   0 root         (0) root         (0)    14359 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_jboss_domain_log.py
--rw-r--r--   0 root         (0) root         (0)     3625 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_jboss_standalone_main_conf.py
--rw-r--r--   0 root         (0) root         (0)     3674 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_jboss_version.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_journal_all.py
--rw-r--r--   0 root         (0) root         (0)     1683 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_journal_since_boot.py
--rw-r--r--   0 root         (0) root         (0)    12906 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_journalctl.py
--rw-r--r--   0 root         (0) root         (0)     3654 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_journald_conf.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_katello_service_status.py
--rw-r--r--   0 root         (0) root         (0)     6049 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_kdump.py
--rw-r--r--   0 root         (0) root         (0)     1981 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_kernel_config.py
--rw-r--r--   0 root         (0) root         (0)     1394 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_keystone.py
--rw-r--r--   0 root         (0) root         (0)      928 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_keystone_log.py
--rw-r--r--   0 root         (0) root         (0)     2131 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_kpatch_list.py
--rw-r--r--   0 root         (0) root         (0)     4951 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_krb5.py
--rw-r--r--   0 root         (0) root         (0)     4524 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_krb5kdc_log.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ksmstate.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ktimer_lockless.py
--rw-r--r--   0 root         (0) root         (0)     1138 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_kubepods_cpu_quota.py
--rw-r--r--   0 root         (0) root         (0)     1780 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ld_library_path.py
--rw-r--r--   0 root         (0) root         (0)    10693 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ldif_config.py
--rw-r--r--   0 root         (0) root         (0)     1232 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_libssh_config.py
--rw-r--r--   0 root         (0) root         (0)     3176 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_libvirtd_log.py
--rw-r--r--   0 root         (0) root         (0)     3919 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_limits_conf.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_logrotate_conf.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_losetup.py
--rw-r--r--   0 root         (0) root         (0)     3578 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_lpstat.py
--rw-r--r--   0 root         (0) root         (0)     1842 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_boot.py
--rw-r--r--   0 root         (0) root         (0)     2895 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_dev.py
--rw-r--r--   0 root         (0) root         (0)     5200 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_disk.py
--rw-r--r--   0 root         (0) root         (0)     1538 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_docker_volumes.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_edac_mc.py
--rw-r--r--   0 root         (0) root         (0)    13104 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_etc.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_ipa_idoverride_memberof.py
--rw-r--r--   0 root         (0) root         (0)     1084 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_krb5_sssd.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_lib_firmware.py
--rw-r--r--   0 root         (0) root         (0)     1716 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_ocp_nci_openshift_sdn.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_origin_local_volumes_pods.py
--rw-r--r--   0 root         (0) root         (0)     2259 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_osroot.py
--rw-r--r--   0 root         (0) root         (0)      985 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_sys_firmware.py
--rw-r--r--   0 root         (0) root         (0)    48952 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_systemd_units.py
--rw-r--r--   0 root         (0) root         (0)     2077 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_tmp.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_usr_bin.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_usr_lib64.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_usr_sbin.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_var_cache_pulp.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_var_lib_mongodb.py
--rw-r--r--   0 root         (0) root         (0)     4555 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_var_lib_nova_instances.py
--rw-r--r--   0 root         (0) root         (0)     1006 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_var_lib_pcp.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_var_lib_rsyslog.py
--rw-r--r--   0 root         (0) root         (0)     5504 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_var_log.py
--rw-r--r--   0 root         (0) root         (0)     2314 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_var_opt_mssql.py
--rw-r--r--   0 root         (0) root         (0)     1310 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_var_opt_mssql_log.py
--rw-r--r--   0 root         (0) root         (0)     1470 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_var_run.py
--rw-r--r--   0 root         (0) root         (0)     8813 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_lsof.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_var_spool_clientmq.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_var_spool_postfix_maildrop.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_var_tmp.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ls_var_www_perms.py
--rw-r--r--   0 root         (0) root         (0)    14261 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_lsblk.py
--rw-r--r--   0 root         (0) root         (0)     5279 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_lscpu.py
--rw-r--r--   0 root         (0) root         (0)    10360 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_lsinitrd.py
--rw-r--r--   0 root         (0) root         (0)     1069 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_lsmod.py
--rw-r--r--   0 root         (0) root         (0)    14803 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_lspci.py
--rw-r--r--   0 root         (0) root         (0)     7350 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_lssap.py
--rw-r--r--   0 root         (0) root         (0)     2606 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_lsscsi.py
--rw-r--r--   0 root         (0) root         (0)     2343 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_luksmeta.py
--rw-r--r--   0 root         (0) root         (0)     2739 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_lvdisplay.py
--rw-r--r--   0 root         (0) root         (0)    13145 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_lvm.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_lvm_conf.py
--rw-r--r--   0 root         (0) root         (0)    34981 2023-02-23 12:15:15.000000 insights-core-3.1.9/insights/tests/parsers/test_lvs.py
--rw-r--r--   0 root         (0) root         (0)    65919 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_manila_conf.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_mariadb_log.py
--rw-r--r--   0 root         (0) root         (0)      672 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_max_uid.py
--rw-r--r--   0 root         (0) root         (0)     1637 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_md5check.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_mdadm.py
--rw-r--r--   0 root         (0) root         (0)    11140 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_mdstat.py
--rw-r--r--   0 root         (0) root         (0)     3699 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_meminfo.py
--rw-r--r--   0 root         (0) root         (0)     1988 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_messages.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_mistral_log.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_mlx4_port.py
--rw-r--r--   0 root         (0) root         (0)     9959 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_modinfo.py
--rw-r--r--   0 root         (0) root         (0)     2823 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_modprobe.py
--rw-r--r--   0 root         (0) root         (0)      869 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_mokutil_sbstate.py
--rw-r--r--   0 root         (0) root         (0)     3734 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_mongod_conf.py
--rw-r--r--   0 root         (0) root         (0)    15441 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_mount.py
--rw-r--r--   0 root         (0) root         (0)     1580 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_mpirun.py
--rw-r--r--   0 root         (0) root         (0)     1856 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_mssql_api_assessment.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_mssql_conf.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_multicast_querier.py
--rw-r--r--   0 root         (0) root         (0)     3572 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_multipath_conf.py
--rw-r--r--   0 root         (0) root         (0)    12704 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_multipath_v4_ll.py
--rw-r--r--   0 root         (0) root         (0)     1953 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_mysql_log.py
--rw-r--r--   0 root         (0) root         (0)     7696 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_mysqladmin.py
--rw-r--r--   0 root         (0) root         (0)     6065 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_named_checkconf.py
--rw-r--r--   0 root         (0) root         (0)     6304 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_named_conf.py
--rw-r--r--   0 root         (0) root         (0)     1433 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ndctl_list.py
--rw-r--r--   0 root         (0) root         (0)     1824 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_net_namespace.py
--rw-r--r--   0 root         (0) root         (0)    48046 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_netstat.py
--rw-r--r--   0 root         (0) root         (0)     5114 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_networkmanager_config.py
--rw-r--r--   0 root         (0) root         (0)     3166 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_networkmanager_dhclient.py
--rw-r--r--   0 root         (0) root         (0)     1537 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_neutron_conf.py
--rw-r--r--   0 root         (0) root         (0)     1183 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_neutron_dhcp_agent_conf.py
--rw-r--r--   0 root         (0) root         (0)     3574 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_neutron_l3_agent_conf.py
--rw-r--r--   0 root         (0) root         (0)     1372 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_neutron_l3_agent_log.py
--rw-r--r--   0 root         (0) root         (0)     3591 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_neutron_metadata_agent_conf.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_neutron_metadata_agent_log.py
--rw-r--r--   0 root         (0) root         (0)     1263 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_neutron_ml2_conf.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_neutron_ovs_agent_log.py
--rw-r--r--   0 root         (0) root         (0)     5875 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_neutron_plugin.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_neutron_server_log.py
--rw-r--r--   0 root         (0) root         (0)     1252 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_neutron_sriov_agent.py
--rw-r--r--   0 root         (0) root         (0)     2725 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_nfnetlink_queue.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_nfs_conf.py
--rw-r--r--   0 root         (0) root         (0)     5175 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_nfs_exports.py
--rw-r--r--   0 root         (0) root         (0)     5954 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_nginx_conf.py
--rw-r--r--   0 root         (0) root         (0)     4721 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_nginx_log.py
--rw-r--r--   0 root         (0) root         (0)    11761 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_nmcli.py
--rw-r--r--   0 root         (0) root         (0)     3257 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_nova_conf.py
--rw-r--r--   0 root         (0) root         (0)     1587 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_nova_log.py
--rw-r--r--   0 root         (0) root         (0)     2075 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_nova_user_ids.py
--rw-r--r--   0 root         (0) root         (0)     6071 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_nscd_conf.py
--rw-r--r--   0 root         (0) root         (0)     1219 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_nss_rhel7.py
--rw-r--r--   0 root         (0) root         (0)     2028 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_nsswitch_conf.py
--rw-r--r--   0 root         (0) root         (0)     4355 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ntp_sources.py
--rw-r--r--   0 root         (0) root         (0)     2377 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_numa_cpus.py
--rw-r--r--   0 root         (0) root         (0)     3512 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_numeric_user_group_name.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_nvme_core_io_timeout.py
--rw-r--r--   0 root         (0) root         (0)    27919 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_octavia.py
--rw-r--r--   0 root         (0) root         (0)      778 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_od_cpu_dma_latency.py
--rw-r--r--   0 root         (0) root         (0)     2082 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_odbc.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_open_vm_tools.py
--rw-r--r--   0 root         (0) root         (0)     5948 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_openshift_configuration.py
--rw-r--r--   0 root         (0) root         (0)    50122 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_openshift_get.py
--rw-r--r--   0 root         (0) root         (0)    14879 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_openshift_get_with_config.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_openshift_hosts.py
--rw-r--r--   0 root         (0) root         (0)     3230 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_openvswitch_logs.py
--rw-r--r--   0 root         (0) root         (0)     1641 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_openvswitch_other_config.py
--rw-r--r--   0 root         (0) root         (0)    14564 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_oracle.py
--rw-r--r--   0 root         (0) root         (0)     2429 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_os_release.py
--rw-r--r--   0 root         (0) root         (0)     4247 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_osa_dispatcher_log.py
--rw-r--r--   0 root         (0) root         (0)      825 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ovirt_engine_confd.py
--rw-r--r--   0 root         (0) root         (0)    18312 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ovirt_engine_log.py
--rw-r--r--   0 root         (0) root         (0)     1778 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ovs_appctl_fdb_show_bridge.py
--rw-r--r--   0 root         (0) root         (0)     5864 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ovs_ofctl_dump_flows.py
--rw-r--r--   0 root         (0) root         (0)     4322 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ovs_vsctl.py
--rw-r--r--   0 root         (0) root         (0)     4355 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ovs_vsctl_list_bridge.py
--rw-r--r--   0 root         (0) root         (0)     3416 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ovs_vsctl_show.py
--rw-r--r--   0 root         (0) root         (0)     1870 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_pacemaker_log.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_package_provides.py
--rw-r--r--   0 root         (0) root         (0)     9823 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_pam.py
--rw-r--r--   0 root         (0) root         (0)    24589 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_parsers_module.py
--rw-r--r--   0 root         (0) root         (0)    11758 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_parted.py
--rw-r--r--   0 root         (0) root         (0)     2830 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4289 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_passenger_status.py
--rw-r--r--   0 root         (0) root         (0)     2281 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_password.py
--rw-r--r--   0 root         (0) root         (0)     2861 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_pci_rport_target_disk_paths.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_pcp_openmetrics_log.py
--rw-r--r--   0 root         (0) root         (0)     5271 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_pcs_config.py
--rw-r--r--   0 root         (0) root         (0)     2661 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_pcs_quorum_status.py
--rw-r--r--   0 root         (0) root         (0)    17328 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_pcs_status.py
--rw-r--r--   0 root         (0) root         (0)     4104 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_php_ini.py
--rw-r--r--   0 root         (0) root         (0)      954 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_pluginconf_d.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_pmlog_summary.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_pmrep.py
--rw-r--r--   0 root         (0) root         (0)    19834 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_podman_inspect.py
--rw-r--r--   0 root         (0) root         (0)     5155 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_podman_list.py
--rw-r--r--   0 root         (0) root         (0)     2258 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_postconf.py
--rw-r--r--   0 root         (0) root         (0)     9240 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_postgresql_conf.py
--rw-r--r--   0 root         (0) root         (0)      801 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_postgresql_log.py
--rw-r--r--   0 root         (0) root         (0)     5888 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_proc_environ.py
--rw-r--r--   0 root         (0) root         (0)     2163 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_proc_keys.py
--rw-r--r--   0 root         (0) root         (0)     2934 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_proc_limits.py
--rw-r--r--   0 root         (0) root         (0)     2709 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_proc_stat.py
--rw-r--r--   0 root         (0) root         (0)    27171 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ps.py
--rw-r--r--   0 root         (0) root         (0)      887 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_pulp_worker_defaults.py
--rw-r--r--   0 root         (0) root         (0)     1949 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_puppet_ca_cert_expire_date.py
--rw-r--r--   0 root         (0) root         (0)    27712 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_pvs.py
--rw-r--r--   0 root         (0) root         (0)      995 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_qemu_conf.py
--rw-r--r--   0 root         (0) root         (0)    26811 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_qemu_xml.py
--rw-r--r--   0 root         (0) root         (0)    14000 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_qpid_stat.py
--rw-r--r--   0 root         (0) root         (0)     1011 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_qpidd_conf.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rabbit_users.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rabbitmq_env.py
--rw-r--r--   0 root         (0) root         (0)     2141 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rabbitmq_log.py
--rw-r--r--   0 root         (0) root         (0)     2872 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rabbitmq_queues.py
--rw-r--r--   0 root         (0) root         (0)     8812 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rabbitmq_report.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rc_local.py
--rw-r--r--   0 root         (0) root         (0)     2524 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rdma_config.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_readlink_mtab.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_readlink_openshift_certs.py
--rw-r--r--   0 root         (0) root         (0)     6066 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_redhat_release.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_resolv_conf.py
--rw-r--r--   0 root         (0) root         (0)     1786 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rhev_data_center.py
--rw-r--r--   0 root         (0) root         (0)      773 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rhn_charsets.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rhn_conf.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rhn_entitlement_cert_xml.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rhn_hibernate_conf.py
--rw-r--r--   0 root         (0) root         (0)     7464 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rhn_logs.py
--rw-r--r--   0 root         (0) root         (0)     8028 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rhn_schema_stats.py
--rw-r--r--   0 root         (0) root         (0)      491 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rhn_schema_version.py
--rw-r--r--   0 root         (0) root         (0)      858 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rhosp_release.py
--rw-r--r--   0 root         (0) root         (0)     2336 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rhsm_conf.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rhsm_log.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rhsm_releasever.py
--rw-r--r--   0 root         (0) root         (0)     5570 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rhv_log_collector_analyzer.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rndc_status.py
--rw-r--r--   0 root         (0) root         (0)     2730 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ros_config.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_route.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rpm_ostree_status.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-02-23 12:17:09.000000 insights-core-3.1.9/insights/tests/parsers/test_rpm_pkgs.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rpm_v_packages.py
--rw-r--r--   0 root         (0) root         (0)     4484 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rpm_vercmp.py
--rw-r--r--   0 root         (0) root         (0)     1780 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_rsyslog_conf.py
--rw-r--r--   0 root         (0) root         (0)     8606 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_samba.py
--rw-r--r--   0 root         (0) root         (0)     2312 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_samba_logs.py
--rw-r--r--   0 root         (0) root         (0)     3202 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sap_dev_trace_files.py
--rw-r--r--   0 root         (0) root         (0)     5156 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sap_hana_python_script.py
--rw-r--r--   0 root         (0) root         (0)     2653 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sap_hdb_version.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sap_host_profile.py
--rw-r--r--   0 root         (0) root         (0)     1758 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sapcontrol.py
--rw-r--r--   0 root         (0) root         (0)     7207 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_saphostctrl.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_saphostexec.py
--rw-r--r--   0 root         (0) root         (0)     1079 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sat5_insights_properties.py
--rw-r--r--   0 root         (0) root         (0)     1584 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_satellite_content_hosts_count.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_satellite_enabled_features.py
--rw-r--r--   0 root         (0) root         (0)     1969 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_satellite_installer_configurations.py
--rw-r--r--   0 root         (0) root         (0)     2718 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_satellite_missed_queues.py
--rw-r--r--   0 root         (0) root         (0)     3166 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_satellite_mongodb.py
--rw-r--r--   0 root         (0) root         (0)    11929 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_satellite_postgresql_query.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_satellite_version.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_satellite_yaml.py
--rw-r--r--   0 root         (0) root         (0)     2499 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     3584 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_scsi.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_scsi_eh_deadline.py
--rw-r--r--   0 root         (0) root         (0)     1486 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_scsi_fwver.py
--rw-r--r--   0 root         (0) root         (0)    12986 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sctp.py
--rw-r--r--   0 root         (0) root         (0)     5819 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sealert.py
--rw-r--r--   0 root         (0) root         (0)     2347 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_secure.py
--rw-r--r--   0 root         (0) root         (0)      918 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_selinux_config.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_semanage.py
--rw-r--r--   0 root         (0) root         (0)     1758 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sendq_recvq_socket_buffer.py
--rw-r--r--   0 root         (0) root         (0)     4770 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sestatus.py
--rw-r--r--   0 root         (0) root         (0)     4222 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_setup_named_chroot.py
--rw-r--r--   0 root         (0) root         (0)    16872 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_slabinfo.py
--rw-r--r--   0 root         (0) root         (0)    13335 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_smartctl.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_smartpdc_settings.py
--rw-r--r--   0 root         (0) root         (0)     4530 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_smbstatus.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_smt.py
--rw-r--r--   0 root         (0) root         (0)     6178 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_snmp.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sockstat.py
--rw-r--r--   0 root         (0) root         (0)     5695 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_softnet_stat.py
--rw-r--r--   0 root         (0) root         (0)     2002 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_software_collections_list.py
--rw-r--r--   0 root         (0) root         (0)      819 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sos_conf.py
--rw-r--r--   0 root         (0) root         (0)     2351 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_spamassassin_channels.py
--rw-r--r--   0 root         (0) root         (0)     4513 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3721 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ssh_client_config.py
--rw-r--r--   0 root         (0) root         (0)     8503 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_ssl_certificate.py
--rw-r--r--   0 root         (0) root         (0)     2442 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sssd_conf.py
--rw-r--r--   0 root         (0) root         (0)     3147 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sssd_logs.py
--rw-r--r--   0 root         (0) root         (0)     1255 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_subscription_manager.py
--rw-r--r--   0 root         (0) root         (0)     4145 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_subscription_manager_list.py
--rw-r--r--   0 root         (0) root         (0)     2405 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_subscription_manager_release.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sudoers.py
--rw-r--r--   0 root         (0) root         (0)     4449 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_swift_conf.py
--rw-r--r--   0 root         (0) root         (0)     3821 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_swift_log.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sys_bus.py
--rw-r--r--   0 root         (0) root         (0)      516 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sys_fs_cgroup_memory.py
--rw-r--r--   0 root         (0) root         (0)      389 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sys_fs_cgroup_memory_tasks_number.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sys_kernel.py
--rw-r--r--   0 root         (0) root         (0)     4947 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sys_module.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sys_vmbus.py
--rw-r--r--   0 root         (0) root         (0)      308 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_chronyd.py
--rw-r--r--   0 root         (0) root         (0)      756 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_corosync.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_dirsrv.py
--rwxr-xr-x   0 root         (0) root         (0)     7988 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_doc_examples.py
--rw-r--r--   0 root         (0) root         (0)     2303 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_docker.py
--rw-r--r--   0 root         (0) root         (0)     1158 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_docker_storage.py
--rw-r--r--   0 root         (0) root         (0)     1483 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_docker_storage_setup.py
--rw-r--r--   0 root         (0) root         (0)      766 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_grub.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_httpd.py
--rw-r--r--   0 root         (0) root         (0)     1317 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_ifcfg_static_route.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_irqbalance.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_kdump.py
--rw-r--r--   0 root         (0) root         (0)     2637 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_libvirt_guests.py
--rw-r--r--   0 root         (0) root         (0)      678 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_memcached.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_mongod.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_netconsole.py
--rw-r--r--   0 root         (0) root         (0)      445 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_network.py
--rw-r--r--   0 root         (0) root         (0)     1807 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_nfs.py
--rw-r--r--   0 root         (0) root         (0)      298 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_ntpd.py
--rw-r--r--   0 root         (0) root         (0)     1260 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_oracleasm.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_prelink.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_puppetserver.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_sshd.py
--rw-r--r--   0 root         (0) root         (0)     3816 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_up2date.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysconfig_virt_who.py
--rw-r--r--   0 root         (0) root         (0)     3503 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_sysctl.py
--rw-r--r--   0 root         (0) root         (0)    12610 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_system_time.py
--rw-r--r--   0 root         (0) root         (0)    12392 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_systemctl_show.py
--rw-r--r--   0 root         (0) root         (0)     1587 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_systemctl_status_all.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_systemd_analyze.py
--rw-r--r--   0 root         (0) root         (0)     9023 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_systemd_config.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_systemid.py
--rw-r--r--   0 root         (0) root         (0)     6146 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_systool.py
--rw-r--r--   0 root         (0) root         (0)      991 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_tags.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_teamdctl_config_dump.py
--rw-r--r--   0 root         (0) root         (0)     3165 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_teamdctl_state_dump.py
--rw-r--r--   0 root         (0) root         (0)     1856 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_tmpfilesd.py
--rw-r--r--   0 root         (0) root         (0)     3432 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_tomcat_virtual_dir_context.py
--rw-r--r--   0 root         (0) root         (0)    55650 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_tomcat_xml.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_transparent_hugepage.py
--rw-r--r--   0 root         (0) root         (0)     4020 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_tuned.py
--rw-r--r--   0 root         (0) root         (0)     2813 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_tuned_conf.py
--rw-r--r--   0 root         (0) root         (0)     5122 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_udev_rules.py
--rw-r--r--   0 root         (0) root         (0)    20347 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_uname.py
--rw-r--r--   0 root         (0) root         (0)    37286 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_unitfiles.py
--rw-r--r--   0 root         (0) root         (0)     3046 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_up2date_log.py
--rw-r--r--   0 root         (0) root         (0)     2697 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_upstart.py
--rw-r--r--   0 root         (0) root         (0)     2496 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_uptime.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_user_group.py
--rw-r--r--   0 root         (0) root         (0)    21095 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_vdo_status.py
--rw-r--r--   0 root         (0) root         (0)     3063 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_vdsm_conf.py
--rw-r--r--   0 root         (0) root         (0)    21905 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_vdsm_log.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_version_info.py
--rw-r--r--   0 root         (0) root         (0)    14025 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_vgdisplay.py
--rw-r--r--   0 root         (0) root         (0)     4743 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_vgs.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_virsh_list_all.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_virt_uuid_facts.py
--rw-r--r--   0 root         (0) root         (0)     1162 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_virt_what.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_virt_who_conf.py
--rw-r--r--   0 root         (0) root         (0)     2717 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_virtlogd_conf.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_vma_ra_enabled_s390x.py
--rw-r--r--   0 root         (0) root         (0)     2821 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_vmcore_dmesg.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_vmware_tools_conf.py
--rw-r--r--   0 root         (0) root         (0)     2941 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_vsftpd.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_wc_proc_1_mountinfo.py
--rw-r--r--   0 root         (0) root         (0)     3189 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_x86_debug.py
--rw-r--r--   0 root         (0) root         (0)     7664 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_xfs_info.py
--rw-r--r--   0 root         (0) root         (0)     4295 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_xinetd_conf.py
--rw-r--r--   0 root         (0) root         (0)     3427 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_yum_conf.py
--rw-r--r--   0 root         (0) root         (0)     4987 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_yum_list_available.py
--rw-r--r--   0 root         (0) root         (0)    12812 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_yum_repolist.py
--rw-r--r--   0 root         (0) root         (0)     2066 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_yum_repos_d.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_yum_updateinfo.py
--rw-r--r--   0 root         (0) root         (0)     1093 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_yum_updates.py
--rw-r--r--   0 root         (0) root         (0)     3025 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_yumlog.py
--rw-r--r--   0 root         (0) root         (0)     4629 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_zdump_v.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/parsers/test_zipl_conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/tests/test_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      183 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_plugins/test_plugin.py
--rw-r--r--   0 root         (0) root         (0)     2564 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_plugins/test_returns_none.py
--rw-r--r--   0 root         (0) root         (0)      110 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_plugins/tina_loves_butts.py
--rw-r--r--   0 root         (0) root         (0)    12205 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/integration.py
--rw-r--r--   0 root         (0) root         (0)     3022 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/mock_web_server.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/spec_tests.py
--rw-r--r--   0 root         (0) root         (0)      341 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_add_component.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_add_exception.py
--rw-r--r--   0 root         (0) root         (0)      292 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_always_fires.py
--rw-r--r--   0 root         (0) root         (0)     3396 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_canonical_facts.py
--rw-r--r--   0 root         (0) root         (0)     1433 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_collect.py
--rw-r--r--   0 root         (0) root         (0)     1111 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_command_parser.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_commandparser.py
--rw-r--r--   0 root         (0) root         (0)      556 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_component_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3815 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_config_parser.py
--rw-r--r--   0 root         (0) root         (0)     2547 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_context.py
--rw-r--r--   0 root         (0) root         (0)      810 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_context_wrap.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_determine_components.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_doc_examples.py
--rw-r--r--   0 root         (0) root         (0)     1011 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_dr_enabled.py
--rw-r--r--   0 root         (0) root         (0)     5447 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_dr_run.py
--rw-r--r--   0 root         (0) root         (0)     9093 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_evaluators.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_extractors.py
--rw-r--r--   0 root         (0) root         (0)    13568 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_file_listing.py
--rw-r--r--   0 root         (0) root         (0)     5942 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_file_permissions.py
--rw-r--r--   0 root         (0) root         (0)     3179 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_filters.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_find.py
--rw-r--r--   0 root         (0) root         (0)     2693 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_formats.py
--rw-r--r--   0 root         (0) root         (0)     1858 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_fs.py
--rw-r--r--   0 root         (0) root         (0)     4753 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_get_dependency_specs.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_insights_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_integration_support.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_json_parser.py
--rw-r--r--   0 root         (0) root         (0)    16221 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_logfileoutput.py
--rw-r--r--   0 root         (0) root         (0)    12368 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_ls_parser.py
--rw-r--r--   0 root         (0) root         (0)     1816 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_parser_class.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_parser_continue_on_error.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_query.py
--rw-r--r--   0 root         (0) root         (0)     2228 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_remote_resource.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_rules_fixture.py
--rw-r--r--   0 root         (0) root         (0)     3994 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_scannable.py
--rw-r--r--   0 root         (0) root         (0)     6783 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_serde.py
--rw-r--r--   0 root         (0) root         (0)     8905 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_soscleaner.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_spec_serialization.py
--rw-r--r--   0 root         (0) root         (0)     3968 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_specs.py
--rw-r--r--   0 root         (0) root         (0)      586 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_subproc.py
--rw-r--r--   0 root         (0) root         (0)     3281 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_sysconfig_options.py
--rw-r--r--   0 root         (0) root         (0)     2129 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_syslog.py
--rw-r--r--   0 root         (0) root         (0)     2865 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_taglang.py
--rw-r--r--   0 root         (0) root         (0)     1306 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_test.py
--rw-r--r--   0 root         (0) root         (0)     7395 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_util.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_vulnerable_kernel.py
--rw-r--r--   0 root         (0) root         (0)     1883 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_xmlparser.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tests/test_yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1481 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tools/apply_spec_filters.py
--rwxr-xr-x   0 root         (0) root         (0)     5247 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tools/cat.py
--rwxr-xr-x   0 root         (0) root         (0)     1497 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tools/dupkeycheck.py
--rwxr-xr-x   0 root         (0) root         (0)     7791 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tools/insights_inspect.py
--rwxr-xr-x   0 root         (0) root         (0)    12650 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/tools/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/util/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights/util/autology/
--rw-r--r--   0 root         (0) root         (0)      125 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/util/autology/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19015 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/util/autology/datasources.py
--rw-r--r--   0 root         (0) root         (0)     8727 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5062 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/util/canonical_facts.py
--rw-r--r--   0 root         (0) root         (0)     4703 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/util/command.py
--rw-r--r--   0 root         (0) root         (0)     4777 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/util/component_graph.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/util/content_type.py
--rw-r--r--   0 root         (0) root         (0)    14369 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/util/file_permissions.py
--rw-r--r--   0 root         (0) root         (0)     2742 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/util/fs.py
--rwxr-xr-x   0 root         (0) root         (0)     2114 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/util/mangle.py
--rw-r--r--   0 root         (0) root         (0)     3945 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/util/specs_catalog.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/util/streams.py
--rw-r--r--   0 root         (0) root         (0)     6335 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/util/subproc.py
--rw-r--r--   0 root         (0) root         (0)       12 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/COMMIT
--rw-r--r--   0 root         (0) root         (0)       14 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/NAME
--rw-r--r--   0 root         (0) root         (0)        2 2023-02-23 12:15:15.000000 insights-core-3.1.9/insights/RELEASE
--rw-r--r--   0 root         (0) root         (0)        6 2023-02-23 12:21:19.000000 insights-core-3.1.9/insights/VERSION
--rw-r--r--   0 root         (0) root         (0)    18283 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/__init__.py
--rw-r--r--   0 root         (0) root         (0)       82 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)    18057 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/collect.py
--rw-r--r--   0 root         (0) root         (0)     3671 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/command_parser.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)     2492 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/ocp.py
--rwxr-xr-x   0 root         (0) root         (0)     2151 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/ocpshell.py
--rw-r--r--   0 root         (0) root         (0)     1446 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/settings.py
--rw-r--r--   0 root         (0) root         (0)    32867 2023-02-23 12:13:26.000000 insights-core-3.1.9/insights/shell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7667 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    57728 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      399 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights_core.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     3538 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-02-23 12:26:14.000000 insights-core-3.1.9/insights_core.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    11357 2023-02-23 12:13:26.000000 insights-core-3.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      221 2023-02-23 12:13:26.000000 insights-core-3.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5370 2023-02-23 12:13:26.000000 insights-core-3.1.9/README.rst
--rw-r--r--   0 root         (0) root         (0)      398 2023-02-23 12:26:14.000000 insights-core-3.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4399 2023-02-23 12:21:19.000000 insights-core-3.1.9/setup.py
--rw-r--r--   0 root         (0) root         (0)     7667 2023-02-23 12:26:14.000000 insights-core-3.1.9/PKG-INFO
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/examples/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/examples/cluster_rules/
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/examples/cluster_rules/__init__.py
+-rwxrwxr-x   0 release   (1002) release   (1002)     6054 2023-06-08 07:07:17.000000 insights-core-3.2.0/examples/cluster_rules/allnodes_cpu.py
+-rwxrwxr-x   0 release   (1002) release   (1002)     1975 2023-06-08 07:07:17.000000 insights-core-3.2.0/examples/cluster_rules/bash_version.py
+-rwxrwxr-x   0 release   (1002) release   (1002)     2588 2023-06-08 07:07:17.000000 insights-core-3.2.0/examples/cluster_rules/ntp_compare.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/examples/rules/
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/examples/rules/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)      541 2023-06-08 07:07:17.000000 insights-core-3.2.0/examples/rules/bash_version.py
+-rwxrwxr-x   0 release   (1002) release   (1002)     1406 2023-06-08 07:07:17.000000 insights-core-3.2.0/examples/rules/hostname_rel.py
+-rwxrwxr-x   0 release   (1002) release   (1002)      862 2023-06-08 07:07:17.000000 insights-core-3.2.0/examples/rules/sample_script.py
+-rwxrwxr-x   0 release   (1002) release   (1002)     5084 2023-06-08 07:07:17.000000 insights-core-3.2.0/examples/rules/skip_component.py
+-rwxrwxr-x   0 release   (1002) release   (1002)     2746 2023-06-08 07:07:17.000000 insights-core-3.2.0/examples/rules/stand_alone.py
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/examples/__init__.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/client/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/client/apps/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/client/apps/ansible/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/
+-rw-rw-r--   0 release   (1002) release   (1002)     2163 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)      500 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/anchor.py
+-rw-rw-r--   0 release   (1002) release   (1002)    35216 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/comments.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8726 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/compat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8304 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/composer.py
+-rw-rw-r--   0 release   (1002) release   (1002)      345 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/configobjwalker.py
+-rw-rw-r--   0 release   (1002) release   (1002)    70571 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/constructor.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6596 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/cyaml.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6640 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/dumper.py
+-rw-rw-r--   0 release   (1002) release   (1002)    64442 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/emitter.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8982 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/error.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3902 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/events.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2972 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/loader.py
+-rw-rw-r--   0 release   (1002) release   (1002)    54172 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/main.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3716 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/nodes.py
+-rw-rw-r--   0 release   (1002) release   (1002)    33260 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/parser.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10885 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/reader.py
+-rw-rw-r--   0 release   (1002) release   (1002)    48762 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/representer.py
+-rw-rw-r--   0 release   (1002) release   (1002)    15356 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/resolver.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1534 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarbool.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4409 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarfloat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4465 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarint.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4548 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarstring.py
+-rw-rw-r--   0 release   (1002) release   (1002)    72204 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scanner.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8430 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/serializer.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1792 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/timestamp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7471 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/tokens.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6127 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/util.py
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)    61772 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/gnupg.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1560 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/oyaml.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8506 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)      768 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/__main__.py
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/ansible/__init__.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/client/apps/compliance/
+-rw-rw-r--   0 release   (1002) release   (1002)    12427 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/compliance/__init__.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/client/apps/malware_detection/
+-rw-rw-r--   0 release   (1002) release   (1002)    81712 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/malware_detection/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2709 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/apps/manifests.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/client/phase/
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/phase/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)    12866 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/phase/v1.py
+-rw-rw-r--   0 release   (1002) release   (1002)    28791 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10067 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/archive.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10030 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/auto_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1964 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/cert_auth.py
+-rw-rw-r--   0 release   (1002) release   (1002)    13273 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/client.py
+-rw-rw-r--   0 release   (1002) release   (1002)    19417 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/collection_rules.py
+-rw-rw-r--   0 release   (1002) release   (1002)    31590 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/config.py
+-rw-rw-r--   0 release   (1002) release   (1002)    46822 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/connection.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4406 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/constants.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3662 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/core_collector.py
+-rw-rw-r--   0 release   (1002) release   (1002)    20948 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/data_collector.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5541 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/insights_spec.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6237 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/map_components.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5281 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/schedule.py
+-rw-rw-r--   0 release   (1002) release   (1002)      521 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/subp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6896 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/support.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1391 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/client/url_cache.py
+-rw-rw-r--   0 release   (1002) release   (1002)    14480 2023-06-08 07:10:24.000000 insights-core-3.2.0/insights/client/utilities.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/combiners/
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3470 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/ansible_info.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1295 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/ceph_osd_tree.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2930 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/ceph_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3199 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/cloud_instance.py
+-rw-rw-r--   0 release   (1002) release   (1002)    16645 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/cloud_provider.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1341 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/cpu_vulns_all.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4877 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/crio_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1656 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/cryptsetup.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2739 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/dmesg.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1813 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/dnsmasq_conf_all.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1183 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/du.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8050 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/grub_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1849 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/hostname.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2449 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/httpd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9246 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/identity_domain.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2901 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/ipa.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4319 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/ipcs_semaphores.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2001 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/ipcs_shared_memory.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6463 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/ipv6.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10422 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/journald_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6416 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/krb5.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2808 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/limits_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5296 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/logrotate_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6883 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/lspci.py
+-rw-rw-r--   0 release   (1002) release   (1002)    13715 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/lvm.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1060 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/md5check.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1048 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/mlx4_port.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1468 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/modinfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3735 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/modprobe.py
+-rw-rw-r--   0 release   (1002) release   (1002)      875 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/multinode.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3725 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/netstat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5551 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/nfs_exports.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2048 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/nginx_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1476 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/nmcli_dev_show.py
+-rw-rw-r--   0 release   (1002) release   (1002)    11114 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/os_release.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9951 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/ps.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3590 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/redhat_release.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3512 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/rhel_for_edge.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1534 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/rhsm_release.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1590 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/rsyslog_confs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6349 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/sap.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8754 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/satellite_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4702 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/selinux.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3245 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/services.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2837 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/smt.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4124 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/ssl_certificate.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1876 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/sudoers.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1371 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/sys_vmbus_devices.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2138 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/sysctl_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2809 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/tmpfilesd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1553 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/tomcat_virtual_dir_context.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2472 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/user_namespaces.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3545 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/virt_what.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4583 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/virt_who_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1542 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/combiners/x86_page_branch.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/components/
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/components/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)      885 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/components/ceph.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1926 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/components/cloud_provider.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2208 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/components/cryptsetup.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1000 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/components/openstack.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2934 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/components/rhel_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4134 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/components/satellite.py
+-rw-rw-r--   0 release   (1002) release   (1002)      852 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/components/virtualization.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/contrib/
+-rw-rw-r--   0 release   (1002) release   (1002)      338 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/contrib/ConfigParser.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9473 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/contrib/ElementPath.py
+-rw-rw-r--   0 release   (1002) release   (1002)    57035 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/contrib/ElementTree.py
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/contrib/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1327 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/contrib/importlib.py
+-rw-rw-r--   0 release   (1002) release   (1002)    72089 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/contrib/ipaddress.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6260 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/contrib/magic.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5441 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/contrib/nginxparser.py
+-rw-rw-r--   0 release   (1002) release   (1002)   164313 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/contrib/pyparsing.py
+-rw-rw-r--   0 release   (1002) release   (1002)    37830 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/contrib/soscleaner.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3093 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/contrib/toposort.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/core/
+-rw-rw-r--   0 release   (1002) release   (1002)    68933 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3281 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/archives.py
+-rw-rw-r--   0 release   (1002) release   (1002)      628 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/blacklist.py
+-rwxrwxr-x   0 release   (1002) release   (1002)     2712 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/cluster.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7213 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/context.py
+-rw-rw-r--   0 release   (1002) release   (1002)    36482 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/dr.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6131 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/evaluators.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3118 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/exceptions.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7060 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/filters.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2358 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/hydration.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8412 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/ls_parser.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1350 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/marshalling.py
+-rw-rw-r--   0 release   (1002) release   (1002)    23719 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/plugins.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5120 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/remote_resource.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8432 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/serde.py
+-rw-rw-r--   0 release   (1002) release   (1002)    50303 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/spec_factory.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3971 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/core/taglang.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights/formats/
+-rw-rw-r--   0 release   (1002) release   (1002)     6957 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/formats/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)      738 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/formats/_json.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9124 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/formats/_markdown.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4414 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/formats/_syslog.py
+-rw-rw-r--   0 release   (1002) release   (1002)      874 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/formats/_yaml.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5570 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/formats/html.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3778 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/formats/simple_html.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3835 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/formats/template.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10240 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/formats/text.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/parsers/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/parsers/systemd/
+-rw-rw-r--   0 release   (1002) release   (1002)      223 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/systemd/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6703 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/systemd/config.py
+-rw-rw-r--   0 release   (1002) release   (1002)    11202 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/systemd/unitfiles.py
+-rw-rw-r--   0 release   (1002) release   (1002)    23917 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3275 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/abrt_ccpp.py
+-rw-rw-r--   0 release   (1002) release   (1002)      709 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/abrt_status_bare.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7334 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/alternatives.py
+-rw-rw-r--   0 release   (1002) release   (1002)      630 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/amq_broker.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5722 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/audit_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3936 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/auditctl.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2139 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/auditd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1873 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/authselect.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1021 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/autofs_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1139 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/avc_cache_threshold.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1883 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/avc_hash_stats.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7085 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/aws_instance_id.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3208 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/awx_manage.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6322 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/azure_instance.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2778 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/azure_instance_plan.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2841 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/azure_instance_type.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1283 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/bdi_read_ahead_kb.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1239 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/blacklisted.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3279 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/blkid.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10936 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/bond.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1968 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/bond_dynamic_lb.py
+-rw-rw-r--   0 release   (1002) release   (1002)      667 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/branch_info.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4389 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/brctl_show.py
+-rw-rw-r--   0 release   (1002) release   (1002)      814 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/candlepin_broker.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4473 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/catalina_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2231 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cciss.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1747 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ceilometer_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    18304 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ceilometer_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5234 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ceph_cmd_json_parsing.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2503 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ceph_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3287 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ceph_insights.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3026 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ceph_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1773 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ceph_osd_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3923 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ceph_osd_tree_text.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10372 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ceph_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3688 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/certificates_enddate.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3338 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cgroups.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1784 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/checkin_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6685 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/chkconfig.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2014 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cib.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2035 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cinder_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2478 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cinder_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5388 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/client_metadata.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1724 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cloud_cfg.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1125 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cloud_init_custom_network.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1105 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cloud_init_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)      703 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cluster_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2655 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cmdline.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1790 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cni_podman_bridge_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)      958 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cobbler_modules_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)      693 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cobbler_settings.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2999 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/config_file_perms.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1553 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/containers_inspect.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1556 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/containers_policy.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3286 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/corosync.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2108 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/corosync_cmapctl.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1854 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cpu_online.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1730 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cpu_vulns.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10183 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cpuinfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4554 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cpupower_frequency_info.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2420 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cpuset_cpus.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1082 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/crictl_logs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1969 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/crio_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)      968 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cron_daily_rhsmd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7528 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cron_jobs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8175 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/crontab.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4615 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/crypto_policies.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6401 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cryptsetup_luksDump.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3953 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cups_confs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2159 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/cups_ppd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1596 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/current_clocksource.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7701 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/date.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1635 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/db2.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1977 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dcbtool_gc_dcb.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1567 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/designate_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    15843 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/df.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5253 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dig.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4672 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dirsrv_logs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5551 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dmesg.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1497 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dmesg_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6945 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dmidecode.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10764 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dmsetup.py
+-rw-rw-r--   0 release   (1002) release   (1002)      955 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dnf_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    15637 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dnf_module.py
+-rw-rw-r--   0 release   (1002) release   (1002)      764 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dnf_modules.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2267 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dnsmasq_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)      953 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/docker_host_machine_id.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3776 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/docker_inspect.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6667 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/docker_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2449 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dockerinfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2212 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dotnet.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4504 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/doveconf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1485 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dracut_modules.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2824 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dse_ldif_simple.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3050 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/du.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2555 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/dumpe2fs_h.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6803 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/engine_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1832 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/engine_db_query.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2727 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/engine_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)      889 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/etc_machine_id.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1159 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/etcd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    31741 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ethtool.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1928 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/facter.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1135 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/fapolicyd_rules.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2241 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/fc_match.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6495 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/fcoeadm_i.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4695 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/findmnt.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4266 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/firewall_cmd.py
+-rw-rw-r--   0 release   (1002) release   (1002)      960 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/firewall_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)    11442 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/foreman_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2065 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/foreman_proxy_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3073 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/foreman_rake_db_migrate_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2624 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/freeipa_healthcheck_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7929 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/fstab.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5792 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/fwupdagent.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2028 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/galera_cnf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2364 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/gcp_instance_type.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1971 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/gcp_license_codes.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2477 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/gcp_network_interfaces.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6240 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/getcert_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1038 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/getconf_pagesize.py
+-rw-rw-r--   0 release   (1002) release   (1002)      580 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/getenforce.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1398 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/getsebool.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1258 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/gfs2_file_system_block_size.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2005 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/glance_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2223 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/gluster_peer_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6337 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/gluster_vol.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3913 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/gnocchi.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1137 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/greenboot_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)    16140 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/grub_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3046 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/grubby.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4019 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/grubenv.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3642 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/hammer_ping.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6471 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/hammer_task_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3748 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/haproxy_cfg.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1280 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/heat_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5719 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/heat_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)      814 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/host_vdsm_id.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3209 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/hostname.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3770 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/hosts.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3215 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/hponcfg.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3014 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/httpd_M.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4359 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/httpd_V.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6074 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/httpd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1917 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/httpd_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1346 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/httpd_open_nfs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2136 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ibm_proc.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4818 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ifcfg.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2867 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/imagemagick_policy.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1637 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/init_process_cgroup.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3456 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/initscript.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1324 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/insights_client_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3397 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/installed_product_ids.py
+-rw-rw-r--   0 release   (1002) release   (1002)    22961 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/installed_rpms.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3732 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/interrupts.py
+-rw-rw-r--   0 release   (1002) release   (1002)    23848 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ip.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3235 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ip_netns_exec_namespace_lsof.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5111 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ipa_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1280 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ipaupgrade_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6116 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ipcs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3265 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ipsec_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8316 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/iptables.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1527 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ironic_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1646 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ironic_inspector_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2719 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/iscsiadm_mode_session.py
+-rw-rw-r--   0 release   (1002) release   (1002)    11140 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/jboss_domain_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2293 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/jboss_standalone_main_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4053 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/jboss_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5079 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/journalctl.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3049 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/journald_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1569 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/katello_service_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9893 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/kdump.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1782 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/kernel_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1259 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/keystone.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2929 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/keystone_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2304 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/kpatch_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7340 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/krb5.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3270 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/krb5kdc_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1456 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ksmstate.py
+-rw-rw-r--   0 release   (1002) release   (1002)      872 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ktimer_lockless.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1291 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/kubepods_cpu_quota.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2003 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ld_library_path.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5357 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ldif_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)      936 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/leapp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3342 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/libssh_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2771 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/libvirtd_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7063 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/limits_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8553 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/logrotate_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2267 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/losetup.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4117 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/lpstat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1317 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_boot.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2054 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_dev.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2942 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_disk.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1660 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_docker_volumes.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1179 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_edac_mc.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4965 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_etc.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1389 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_ipa_idoverride_memberof.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1425 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_krb5_sssd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2105 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_lib_firmware.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1462 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_ocp_cni_openshift_sdn.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1523 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_origin_local_volumes_pods.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2095 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_osroot.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1511 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_rsyslog_errorfile.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1573 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_sys_firmware.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3893 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_systemd_units.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2356 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_tmp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1691 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_usr_bin.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1313 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_usr_lib64.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1785 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_usr_sbin.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1203 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_var_cache_pulp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1160 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_var_lib_mongodb.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5642 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_var_lib_nova_instances.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1076 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_var_lib_pcp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1242 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_var_lib_rpm.py
+-rw-rw-r--   0 release   (1002) release   (1002)      822 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_var_lib_rsyslog.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1873 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_var_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)      857 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_var_opt_mssql.py
+-rw-rw-r--   0 release   (1002) release   (1002)      686 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_var_opt_mssql_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1120 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_var_run.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1203 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_var_spool_clientmq.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1249 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_var_spool_postfix_maildrop.py
+-rw-rw-r--   0 release   (1002) release   (1002)      995 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_var_tmp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1579 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ls_var_www_perms.py
+-rw-rw-r--   0 release   (1002) release   (1002)    13204 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/lsblk.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2293 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/lscpu.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6149 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/lsinitrd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2099 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/lsmod.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6722 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/lsof.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6819 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/lspci.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4040 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/lssap.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3726 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/lsscsi.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3544 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/luksmeta.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4792 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/lvdisplay.py
+-rw-rw-r--   0 release   (1002) release   (1002)    30358 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/lvm.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1452 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/machine_id.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1661 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/manila_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2104 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/mariadb_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1793 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/max_uid.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1567 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/md5check.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2204 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/mdadm.py
+-rw-rw-r--   0 release   (1002) release   (1002)    13622 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/mdstat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7657 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/meminfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1708 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/messages.py
+-rw-rw-r--   0 release   (1002) release   (1002)      261 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/metadata.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2360 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/mistral_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)      926 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/mlx4_port.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8178 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/modinfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3038 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/modprobe.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1124 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/mokutil_sbstate.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6047 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/mongod_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    17003 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/mount.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1097 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/mpirun.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4182 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/mssql_api_assessment.py
+-rw-rw-r--   0 release   (1002) release   (1002)      901 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/mssql_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2144 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/multicast_querier.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8381 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/multipath_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    11281 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/multipath_v4_ll.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2088 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/mysql_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4351 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/mysqladmin.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6968 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/named_checkconf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2052 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/named_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2468 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ndctl_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1399 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/net_namespace.py
+-rw-rw-r--   0 release   (1002) release   (1002)    35383 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/netstat.py
+-rw-rw-r--   0 release   (1002) release   (1002)      842 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/networkmanager_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3245 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/networkmanager_dhclient.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2020 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/neutron_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1477 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/neutron_dhcp_agent_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1312 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/neutron_l3_agent_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1401 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/neutron_l3_agent_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1386 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/neutron_metadata_agent_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1977 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/neutron_metadata_agent_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1148 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/neutron_ml2_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2424 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/neutron_ovs_agent_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1264 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/neutron_plugin.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2236 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/neutron_server_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1527 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/neutron_sriov_agent.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2602 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/nfnetlink_queue.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2002 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/nfs_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6583 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/nfs_exports.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5703 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/nginx_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8952 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/nginx_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7561 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/nmcli.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2818 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/nova_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)      716 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/nova_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2266 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/nova_user_ids.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5859 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/nscd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1281 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/nss_rhel7.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2055 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/nsswitch_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5862 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ntp_sources.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2915 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/numa_cpus.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2595 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/numeric_user_group_name.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1285 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/nvme_core_io_timeout.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5310 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/octavia.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1146 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/od_cpu_dma_latency.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3084 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/odbc.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1559 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/open_vm_tools.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1134 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/openshift_configuration.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8565 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/openshift_get.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6322 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/openshift_get_with_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6410 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/openshift_hosts.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2644 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/openvswitch_logs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1352 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/openvswitch_other_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1995 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/oracle.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1756 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/os_release.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4166 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/osa_dispatcher_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)      339 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ovirt_engine_confd.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10113 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ovirt_engine_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2521 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ovs_appctl_fdb_show_bridge.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3192 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ovs_ofctl_dump_flows.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3111 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ovs_vsctl.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2254 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ovs_vsctl_list_bridge.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4161 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ovs_vsctl_show.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1603 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/pacemaker_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2724 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/package_provides.py
+-rw-rw-r--   0 release   (1002) release   (1002)    15886 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/pam.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10040 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/parted.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1813 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/partitions.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4153 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/passenger_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)      214 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/password.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5810 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/pci_rport_target_disk_paths.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1039 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/pcp_openmetrics_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5734 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/pcs_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3031 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/pcs_quorum_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7577 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/pcs_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6139 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/php_ini.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1592 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/pluginconf_d.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4095 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/pmlog_summary.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2833 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/pmrep.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3852 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/podman_inspect.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3502 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/podman_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2921 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/postconf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6788 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/postgresql_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1807 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/postgresql_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2634 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/proc_environ.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4659 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/proc_keys.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3182 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/proc_keyusers.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5230 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/proc_limits.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6847 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/proc_stat.py
+-rw-rw-r--   0 release   (1002) release   (1002)    20696 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ps.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1334 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/pulp_worker_defaults.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1829 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/puppet_ca_cert_expire_date.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1802 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/qemu_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    13011 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/qemu_xml.py
+-rw-rw-r--   0 release   (1002) release   (1002)    12343 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/qpid_stat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1466 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/qpidd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10449 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rabbitmq.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4623 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rabbitmq_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1190 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rc_local.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2185 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rdma_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)      983 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/readlink_e_mtab.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2687 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/readlink_openshift_certs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4095 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/redhat_release.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4279 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/repquota.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2910 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/resolv_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2138 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rhev_data_center.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1692 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rhn_charsets.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2434 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rhn_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3553 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rhn_entitlement_cert_xml.py
+-rw-rw-r--   0 release   (1002) release   (1002)      678 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rhn_hibernate_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7383 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rhn_logs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6474 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rhn_schema_stats.py
+-rw-rw-r--   0 release   (1002) release   (1002)      771 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rhn_schema_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1488 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rhosp_release.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2803 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rhsm_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1759 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rhsm_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2139 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rhsm_releasever.py
+-rw-rw-r--   0 release   (1002) release   (1002)      575 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rhv_log_collector_analyzer.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1909 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rndc_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4953 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ros_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1542 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/route.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2774 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rpm_ostree_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1953 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rpm_pkgs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2068 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rpm_v_packages.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3922 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rpm_vercmp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3019 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/rsyslog_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6879 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/samba.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2817 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/samba_logs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8418 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sap_dev_trace_files.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3032 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sap_hana_python_script.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3202 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sap_hdb_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1670 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sap_host_profile.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2600 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sapcontrol.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4363 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/saphostctrl.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5522 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/saphostexec.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1505 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sat5_insights_properties.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1473 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/satellite_content_hosts_count.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1433 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/satellite_enabled_features.py
+-rw-rw-r--   0 release   (1002) release   (1002)      953 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/satellite_installer_configurations.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1814 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/satellite_missed_queues.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3452 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/satellite_mongodb.py
+-rw-rw-r--   0 release   (1002) release   (1002)    14831 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/satellite_postgresql_query.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1818 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/satellite_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)      800 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/satellite_yaml.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1818 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/scheduler.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3501 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/scsi.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1823 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/scsi_eh_deadline.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1510 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/scsi_fwver.py
+-rw-rw-r--   0 release   (1002) release   (1002)    14838 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sctp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4408 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sealert.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1544 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/secure.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1538 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/selinux_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1086 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/semanage.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3426 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sendq_recvq_socket_buffer.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2984 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sestatus.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2759 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/setup_named_chroot.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5122 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/slabinfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8746 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/smartctl.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1313 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/smartpdc_settings.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4384 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/smbstatus.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4801 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/smt.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5214 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/snmp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3672 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sockstat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6210 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/softnet_stat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2017 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/software_collections_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)      999 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sos_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1758 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/spamassassin_channels.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9175 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ssh.py
+-rw-rw-r--   0 release   (1002) release   (1002)    12585 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ssh_client_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)    12225 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/ssl_certificate.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3694 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sssd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3178 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sssd_logs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1534 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/subscription_manager.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8374 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/subscription_manager_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2605 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/subscription_manager_release.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4041 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sudoers.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4353 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/swift_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1359 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/swift_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1520 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sys_block.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1640 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sys_bus.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1817 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sys_fs_cgroup_memory.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1315 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sys_fs_cgroup_memory_tasks_number.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2183 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sys_kernel.py
+-rwxrwxr-x   0 release   (1002) release   (1002)     5878 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sys_module.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2057 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sys_vmbus.py
+-rw-rw-r--   0 release   (1002) release   (1002)    21345 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sysconfig.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5165 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/sysctl.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10809 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/system_time.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9992 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/systemctl_show.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2565 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/systemctl_status_all.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3352 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/systemd_analyze.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2674 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/systemid.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5051 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/systool.py
+-rw-rw-r--   0 release   (1002) release   (1002)      623 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/tags.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1974 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/teamdctl_config_dump.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2112 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/teamdctl_state_dump.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2405 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/tmpfilesd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3111 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/tomcat_virtual_dir_context.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6264 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/tomcat_xml.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2185 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/transparent_hugepage.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2317 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/tuned.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1244 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/tuned_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3974 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/udev_rules.py
+-rw-rw-r--   0 release   (1002) release   (1002)    21950 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/uname.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1557 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/up2date_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4786 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/upstart.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3585 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/uptime.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2271 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/user_group.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6983 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/vdo_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2515 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/vdsm_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    11713 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/vdsm_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2110 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/version_info.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6436 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/vgdisplay.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4794 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/virsh_list_all.py
+-rw-rw-r--   0 release   (1002) release   (1002)      626 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/virt_uuid_facts.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2235 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/virt_what.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1776 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/virt_who_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3341 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/virtlogd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1129 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/vma_ra_enabled_s390x.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2332 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/vmcore_dmesg.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1278 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/vmware_tools_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3679 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/vsftpd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1467 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/wc_proc_1_mountinfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3436 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/x86_debug.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8459 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/xfs_info.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3833 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/xinetd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7932 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/yum.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2453 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/yum_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7787 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/yum_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2737 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/yum_repos_d.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1391 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/yum_updateinfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1603 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/yum_updates.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5405 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/yumlog.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3895 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/zdump_v.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4535 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsers/zipl_conf.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/parsr/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/parsr/examples/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/parsr/examples/tests/
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/tests/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)      499 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/tests/test_arith.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4256 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/tests/test_corosync.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4826 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/tests/test_httpd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2956 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/tests/test_json.py
+-rw-rw-r--   0 release   (1002) release   (1002)      466 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/tests/test_kvpairs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1933 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/tests/test_logrotate.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3966 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/tests/test_multipath.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5747 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/tests/test_nginx.py
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2097 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/arith.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1318 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/corosync_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1478 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/httpd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2201 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/iniparser.py
+-rw-rw-r--   0 release   (1002) release   (1002)      898 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/json_parser.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2050 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/kvpairs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1826 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/logrotate_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1251 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/multipath_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1131 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/examples/nginx_conf.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/parsr/query/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/parsr/query/tests/
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/query/tests/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)      519 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/query/tests/test_boolean.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4076 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/query/tests/test_choose.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1118 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/query/tests/test_compile_queries.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3301 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/query/tests/test_crumbs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1083 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/query/tests/test_find.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1614 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/query/tests/test_query.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3171 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/query/tests/test_where.py
+-rw-rw-r--   0 release   (1002) release   (1002)    30926 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/query/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4602 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/query/boolean.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/parsr/tests/
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/tests/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)      210 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/tests/test_boolean.py
+-rw-rw-r--   0 release   (1002) release   (1002)      151 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/tests/test_forward.py
+-rw-rw-r--   0 release   (1002) release   (1002)      208 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/tests/test_function_error.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1975 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/tests/test_iniparser.py
+-rw-rw-r--   0 release   (1002) release   (1002)      453 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/tests/test_keep.py
+-rw-rw-r--   0 release   (1002) release   (1002)      432 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/tests/test_literal.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1226 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/tests/test_many.py
+-rw-rw-r--   0 release   (1002) release   (1002)      351 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/tests/test_number.py
+-rw-rw-r--   0 release   (1002) release   (1002)      220 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/tests/test_opt.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1798 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/tests/test_pos_marker.py
+-rw-rw-r--   0 release   (1002) release   (1002)      522 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/tests/test_string.py
+-rw-rw-r--   0 release   (1002) release   (1002)      161 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/tests/test_until.py
+-rw-rw-r--   0 release   (1002) release   (1002)    40965 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4197 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/parsr/iniparser.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/plugins/
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/plugins/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)      151 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/plugins/always_fires.py
+-rw-rw-r--   0 release   (1002) release   (1002)      268 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/plugins/info.py
+-rw-rw-r--   0 release   (1002) release   (1002)      369 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/plugins/insights_heartbeat.py
+-rw-rw-r--   0 release   (1002) release   (1002)      194 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/plugins/never_fires.py
+-rw-rw-r--   0 release   (1002) release   (1002)      513 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/plugins/ps_rule_fakes.py
+-rw-rw-r--   0 release   (1002) release   (1002)      492 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/plugins/returns_none.py
+-rw-rw-r--   0 release   (1002) release   (1002)      519 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/plugins/rules_fixture_plugin.py
+-rw-rw-r--   0 release   (1002) release   (1002)      257 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/plugins/vulnerable_kernel.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/specs/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/specs/datasources/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/specs/datasources/container/
+-rw-rw-r--   0 release   (1002) release   (1002)     2842 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/container/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4064 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/container/containers_inspect.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1285 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/container/nginx_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1955 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1444 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/aws.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2512 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/awx_manage.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3252 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/candlepin_broker.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2905 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/cloud_init.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1140 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/corosync.py
+-rw-rw-r--   0 release   (1002) release   (1002)      521 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/dir_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3158 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/ethernet.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2139 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/httpd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1160 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/ipcs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1365 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/kernel.py
+-rw-rw-r--   0 release   (1002) release   (1002)      860 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/kernel_module_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2049 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/leapp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1590 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/lpstat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4104 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/luks_devices.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2334 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/machine_ids.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2008 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/malware_detection.py
+-rw-rw-r--   0 release   (1002) release   (1002)      574 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/md5chk.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2753 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/package_provides.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2455 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/pcp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4469 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/ps.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3831 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/rpm_pkgs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1250 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/rsyslog_confs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2770 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/sap.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4542 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/satellite_missed_queues.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1733 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/semanage.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3498 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/ssl_certificate.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1419 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/sys_fs_cgroup_memory.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1786 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/sys_fs_cgroup_memory_tasks_number.py
+-rw-rw-r--   0 release   (1002) release   (1002)      726 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/user_group.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7773 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/datasources/yum_updates.py
+-rw-rw-r--   0 release   (1002) release   (1002)    35932 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)      703 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/core3_archive.py
+-rw-rw-r--   0 release   (1002) release   (1002)    49715 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/default.py
+-rw-rw-r--   0 release   (1002) release   (1002)    24865 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/insights_archive.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2106 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/jdr_archive.py
+-rw-rw-r--   0 release   (1002) release   (1002)      416 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/must_gather_archive.py
+-rw-rw-r--   0 release   (1002) release   (1002)    24582 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/specs/sos_archive.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/tests/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/tests/combiners/
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2465 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_ansible_info.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7843 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_ceph_osd_tree.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4682 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_ceph_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3344 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_cloud_instance.py
+-rw-rw-r--   0 release   (1002) release   (1002)    20466 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_cloud_provider.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4405 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_cpu_vulns_all.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1808 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_crio_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6147 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_cryptsetup.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3170 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_dmesg.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3781 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_dnsmasq_conf_all.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1003 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_du.py
+-rw-rw-r--   0 release   (1002) release   (1002)    30578 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_grub_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3236 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_hostname.py
+-rw-rw-r--   0 release   (1002) release   (1002)    30446 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_httpd_conf_tree.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5725 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_identity_domain.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3204 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_ipa.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4690 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_ipcs_semaphores.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1691 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_ipcs_shared_memory.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6424 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_ipv6.py
+-rw-rw-r--   0 release   (1002) release   (1002)    17768 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_journald_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3701 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_krb5.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2297 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_limits_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4294 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_logrotate_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2546 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_logrotate_conf_tree.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9507 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_lspci.py
+-rw-rw-r--   0 release   (1002) release   (1002)    62274 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_lvm.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1136 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_md5check.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1132 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_mlx4_port.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1179 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_modinfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3503 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_modprobe.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8578 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_netstat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4681 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_nfs_exports.py
+-rw-rw-r--   0 release   (1002) release   (1002)    11093 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_nginx_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5480 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_nmcli_dev_show.py
+-rw-rw-r--   0 release   (1002) release   (1002)    21820 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_os_release.py
+-rw-rw-r--   0 release   (1002) release   (1002)    14650 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_ps.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2410 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_redhat_release.py
+-rw-rw-r--   0 release   (1002) release   (1002)    13944 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_rhel_for_edge.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1324 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_rhsm_release.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6262 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_rsyslog_confs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9437 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_sap.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9872 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_satellite_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)    16559 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_selinux.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3149 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_services.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5788 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_smt.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5198 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_ssl_certificate.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2547 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_sudoers.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2443 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_sys_vmbus_devices.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2957 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_sysctl_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4392 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_tmpfilesd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5802 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_tomcat_virtual_dir_context.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4553 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_user_namespaces.py
+-rw-rw-r--   0 release   (1002) release   (1002)    11989 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_virt_what.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4124 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_virt_who_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1839 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/combiners/test_x86_page_branch.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/tests/components/
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/components/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1476 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/components/test_ceph.py
+-rw-rw-r--   0 release   (1002) release   (1002)      894 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/components/test_cloud_provider.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1285 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/components/test_cryptsetup.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2140 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/components/test_openstack.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3023 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/components/test_rhel_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4052 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/components/test_satellite.py
+-rw-rw-r--   0 release   (1002) release   (1002)      543 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/components/test_virtualization.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/tests/datasources/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/tests/datasources/container/
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/container/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)    44018 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/container/test_containers_inspect.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2501 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/container/test_nginx_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5189 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/container/test_running_rhel_containers.py
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)      854 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_aws.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3306 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_awx_manage.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10281 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_candlepin_broker.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3572 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_cloud_init.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1538 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_corosync.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4168 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_datasource_timeout.py
+-rw-rw-r--   0 release   (1002) release   (1002)      882 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_dir_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3702 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_ethernet.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4915 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_get_running_commands.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2365 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_httpd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1368 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_ipcs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1545 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_kernel.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1950 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_kernel_module_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1729 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_leapp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1633 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_lpstat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7739 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_luks_devices.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6901 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_machine_ids.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5915 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_package_provides.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4596 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_pcp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4895 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_ps.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2006 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_rpm_pkgs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3460 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_rsyslog_confs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8411 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_sap.py
+-rw-rw-r--   0 release   (1002) release   (1002)    17158 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_satellite_missed_queues.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3120 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_semanage.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9201 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_ssl_certificate.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3531 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_sys_fs_cgroup_memory.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3680 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_sys_fs_cgroup_memory_tasks_number.py
+-rw-rw-r--   0 release   (1002) release   (1002)      823 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_user_group.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2266 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/datasources/test_yum_updates.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/tests/parsers/
+-rw-rw-r--   0 release   (1002) release   (1002)     2167 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6755 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/lvm_test_data.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3035 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_abrt_ccpp.py
+-rw-rw-r--   0 release   (1002) release   (1002)      768 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_abrt_status_bare.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8278 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_alternatives.py
+-rw-rw-r--   0 release   (1002) release   (1002)    11425 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_amq_broker.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6787 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_audit_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3439 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_auditctl.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4451 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_auditd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1362 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_authselect.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1819 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_autofs_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)      972 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_avc_cache_threshold.py
+-rw-rw-r--   0 release   (1002) release   (1002)      732 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_avc_hash_stats.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9160 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_aws_instance_id.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3799 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_awx_manage.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7098 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_azure_instance.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2684 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_azure_instance_plan.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2731 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_azure_instance_type.py
+-rw-rw-r--   0 release   (1002) release   (1002)      873 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_bdi_read_ahead_kb.py
+-rw-rw-r--   0 release   (1002) release   (1002)      716 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_blacklisted.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3374 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_blkid.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9105 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_bond.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1806 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_bond_dynamic_lb.py
+-rw-rw-r--   0 release   (1002) release   (1002)      388 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_branch_info.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2928 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_brctl_show.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5960 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_candlepin_broker.py
+-rw-rw-r--   0 release   (1002) release   (1002)    16098 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_catalina_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1455 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cciss.py
+-rw-rw-r--   0 release   (1002) release   (1002)    24431 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ceilometer_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    13733 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ceilometer_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)    26668 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ceph_cmd_json_parsing.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2222 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ceph_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    40877 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ceph_insights.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2986 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ceph_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1973 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ceph_osd_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2969 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ceph_osd_tree_text.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4128 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ceph_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4602 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_certificates_enddate.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1004 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cgroups.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1399 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_checkin_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3865 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_chkconfig.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1512 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cib.py
+-rw-rw-r--   0 release   (1002) release   (1002)    32878 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cinder_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3937 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cinder_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3844 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_client_metadata.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1026 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cloud_cfg.py
+-rw-rw-r--   0 release   (1002) release   (1002)      987 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cloud_init_custom_network.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1034 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cloud_init_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1619 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cluster_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2356 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cmdline.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1744 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cni_podman_bridge_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3467 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cobbler_modules_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    15451 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cobbler_settings.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1859 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_config_file_perms.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1340 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_containers_inspect.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1538 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_containers_policy.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2032 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_corosync.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4540 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_corosync_cmapctl.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1073 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cpu_online.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6120 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cpu_vulns.py
+-rw-rw-r--   0 release   (1002) release   (1002)    63388 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cpuinfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6646 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cpupower_frequency_info.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1305 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cpuset_cpus.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1233 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_crictl_logs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2296 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_crio_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1076 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cron_daily_rhsmd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4957 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cron_jobs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3780 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_crontab.py
+-rw-rw-r--   0 release   (1002) release   (1002)      937 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_crypto_policies_bind.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1339 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_crypto_policies_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1029 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_crypto_policies_doc_examples.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6003 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_crypto_policies_opensshserver.py
+-rw-rw-r--   0 release   (1002) release   (1002)      497 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_crypto_policies_state_current.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5541 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cryptsetup_luksDump.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4479 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cups_confs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1838 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_cups_ppd.py
+-rw-rw-r--   0 release   (1002) release   (1002)      330 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_current_clocksource.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6691 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_date.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1479 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_db2.py
+-rw-rw-r--   0 release   (1002) release   (1002)      835 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dcbtool_gc_dcb.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1191 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_designate_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    13735 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_df.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6069 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dig.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3480 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dirsrv_logs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4406 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dmesg.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1798 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dmesg_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)    18156 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dmidecode.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8736 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dmsetup.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2206 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dnf_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    15275 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dnf_module.py
+-rw-rw-r--   0 release   (1002) release   (1002)      879 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dnf_modules.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1267 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dnsmasq_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)      393 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_docker_host_machine-id.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2623 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_docker_info.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10340 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_docker_inspect.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5843 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_docker_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2559 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dotnet.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4820 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_doveconf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1321 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dracut_modules.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5969 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dse_ldif_simple.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4313 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_du.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1993 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_dumpe2fs_h.py
+-rw-rw-r--   0 release   (1002) release   (1002)    22800 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_engine_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3364 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_engine_db_query.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2040 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_engine_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)      987 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_etc_machine_id.py
+-rw-rw-r--   0 release   (1002) release   (1002)      940 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_etcd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    24647 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ethtool.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3276 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_facter.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1109 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_fapolicyd_rules.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1132 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_fc_match.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3449 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_fcoeadm_i.py
+-rw-rw-r--   0 release   (1002) release   (1002)    44765 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ip.py
+-rw-rw-r--   0 release   (1002) release   (1002)    14400 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_findmnt.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4134 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_firewall_cmd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1090 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_firewall_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)    25804 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_foreman_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1450 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_foreman_proxy_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2776 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_foreman_rake_db_migrate_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3949 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_freeipa_healthcheck_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8164 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_fstab.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5701 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_fwupdagent.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1317 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_galera_cnf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2659 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_gcp_instance_type.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2422 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_gcp_license_codes.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1591 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_gcp_network_interfaces.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4706 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_getcert_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)      723 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_getconf_pagesize.py
+-rw-rw-r--   0 release   (1002) release   (1002)      584 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_getenforce.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1244 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_getsebool.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1281 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_gfs2_file_system_block_size.py
+-rw-rw-r--   0 release   (1002) release   (1002)      775 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_glance_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1962 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_gluster_peer_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)    12420 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_gluster_vol.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3049 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_gnocchi.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5284 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_greenboot_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)    13468 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_grub_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4751 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_grub_conf_efi.py
+-rw-rw-r--   0 release   (1002) release   (1002)    17510 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_grub_conf_kdump.py
+-rw-rw-r--   0 release   (1002) release   (1002)    11788 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_grub_conf_missing_boot_files.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4164 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_grubby.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3318 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_grubenv.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7224 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_hammer_ping.py
+-rw-rw-r--   0 release   (1002) release   (1002)    11359 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_hammer_task_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10536 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_haproxy_cfg.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1662 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_heat_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2467 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_heat_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)      333 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_host_vdsm_id.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2385 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_hostname.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3595 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_hosts.py
+-rw-rw-r--   0 release   (1002) release   (1002)      667 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_hponcfg.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3006 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_httpd_M.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4517 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_httpd_V.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6631 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_httpd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7486 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_httpd_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)      954 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_httpd_open_nfs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1276 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ibm_proc.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8986 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ifcfg.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3653 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_imagemagick_policy.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3366 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_init_process_cgroup.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4537 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_initscript.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1069 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_insights_client_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2516 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_installed_product_ids.py
+-rw-rw-r--   0 release   (1002) release   (1002)    32303 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_installed_rpms.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6378 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_interrupts.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1644 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ip_netns_exec_namespace_lsof.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1823 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ipa_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)      722 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ipaupgrade_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3777 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ipcs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2048 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ipsec_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9241 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_iptables.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2428 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ironic_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2907 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ironic_inspector_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1234 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_iscsiadm_mode_session.py
+-rw-rw-r--   0 release   (1002) release   (1002)    14359 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_jboss_domain_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3625 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_jboss_standalone_main_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3674 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_jboss_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)    12906 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_journalctl.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3654 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_journald_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1454 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_katello_service_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6049 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_kdump.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1981 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_kernel_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1394 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_keystone.py
+-rw-rw-r--   0 release   (1002) release   (1002)      928 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_keystone_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2131 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_kpatch_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5604 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_krb5.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4524 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_krb5kdc_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1127 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ksmstate.py
+-rw-rw-r--   0 release   (1002) release   (1002)      862 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ktimer_lockless.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1138 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_kubepods_cpu_quota.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1780 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ld_library_path.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10693 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ldif_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1049 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_leapp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1232 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_libssh_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3176 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_libvirtd_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3919 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_limits_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4805 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_logrotate_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2212 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_losetup.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3578 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_lpstat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1842 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_boot.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2895 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_dev.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5200 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_disk.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1538 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_docker_volumes.py
+-rw-rw-r--   0 release   (1002) release   (1002)      875 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_edac_mc.py
+-rw-rw-r--   0 release   (1002) release   (1002)    13104 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_etc.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1156 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_ipa_idoverride_memberof.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1084 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_krb5_sssd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3344 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_lib_firmware.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1716 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_ocp_nci_openshift_sdn.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1605 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_origin_local_volumes_pods.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2259 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_osroot.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1949 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_rsyslog_errorfile.py
+-rw-rw-r--   0 release   (1002) release   (1002)      985 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_sys_firmware.py
+-rw-rw-r--   0 release   (1002) release   (1002)    48952 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_systemd_units.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2077 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_tmp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1643 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_usr_bin.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1542 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_usr_lib64.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1500 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_usr_sbin.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1314 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_var_cache_pulp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1465 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_var_lib_mongodb.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4555 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_var_lib_nova_instances.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1006 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_var_lib_pcp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2932 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_var_lib_rpm.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1113 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_var_lib_rsyslog.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5504 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_var_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2314 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_var_opt_mssql.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1310 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_var_opt_mssql_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1470 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_var_run.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1581 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_var_spool_clientmq.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1274 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_var_spool_postfix_maildrop.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1314 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_var_tmp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2124 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ls_var_www_perms.py
+-rw-rw-r--   0 release   (1002) release   (1002)    14261 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_lsblk.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5279 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_lscpu.py
+-rw-rw-r--   0 release   (1002) release   (1002)    10777 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_lsinitrd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1069 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_lsmod.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8813 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_lsof.py
+-rw-rw-r--   0 release   (1002) release   (1002)    14803 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_lspci.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7350 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_lssap.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2606 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_lsscsi.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2343 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_luksmeta.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2739 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_lvdisplay.py
+-rw-rw-r--   0 release   (1002) release   (1002)    13145 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_lvm.py
+-rw-rw-r--   0 release   (1002) release   (1002)      836 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_lvm_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    34981 2023-06-08 07:10:24.000000 insights-core-3.2.0/insights/tests/parsers/test_lvs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1303 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_machine_id.py
+-rw-rw-r--   0 release   (1002) release   (1002)    65919 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_manila_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)      746 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_mariadb_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)      672 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_max_uid.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1637 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_md5check.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1525 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_mdadm.py
+-rw-rw-r--   0 release   (1002) release   (1002)    11140 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_mdstat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3699 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_meminfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1988 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_messages.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4165 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_mistral_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)      780 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_mlx4_port.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9729 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_modinfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2823 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_modprobe.py
+-rw-rw-r--   0 release   (1002) release   (1002)      869 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_mokutil_sbstate.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3734 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_mongod_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    15441 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_mount.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1580 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_mpirun.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2798 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_mssql_api_assessment.py
+-rw-rw-r--   0 release   (1002) release   (1002)      597 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_mssql_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)      524 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_multicast_querier.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3572 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_multipath_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    12704 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_multipath_v4_ll.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1953 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_mysql_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7696 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_mysqladmin.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6065 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_named_checkconf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6304 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_named_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1433 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ndctl_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1824 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_net_namespace.py
+-rw-rw-r--   0 release   (1002) release   (1002)    48046 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_netstat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5114 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_networkmanager_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3166 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_networkmanager_dhclient.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1537 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_neutron_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1183 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_neutron_dhcp_agent_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3574 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_neutron_l3_agent_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1372 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_neutron_l3_agent_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3591 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_neutron_metadata_agent_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1964 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_neutron_metadata_agent_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1263 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_neutron_ml2_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1077 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_neutron_ovs_agent_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5875 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_neutron_plugin.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1575 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_neutron_server_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1252 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_neutron_sriov_agent.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2725 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_nfnetlink_queue.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2431 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_nfs_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5175 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_nfs_exports.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5954 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_nginx_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4721 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_nginx_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)    11761 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_nmcli.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3257 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_nova_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1587 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_nova_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2075 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_nova_user_ids.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6071 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_nscd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1219 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_nss_rhel7.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2028 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_nsswitch_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4355 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ntp_sources.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2377 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_numa_cpus.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3512 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_numeric_user_group_name.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1180 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_nvme_core_io_timeout.py
+-rw-rw-r--   0 release   (1002) release   (1002)    27919 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_octavia.py
+-rw-rw-r--   0 release   (1002) release   (1002)      778 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_od_cpu_dma_latency.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2082 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_odbc.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1144 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_open_vm_tools.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5948 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_openshift_configuration.py
+-rw-rw-r--   0 release   (1002) release   (1002)    50122 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_openshift_get.py
+-rw-rw-r--   0 release   (1002) release   (1002)    14879 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_openshift_get_with_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2468 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_openshift_hosts.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3230 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_openvswitch_logs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1641 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_openvswitch_other_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)    14564 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_oracle.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2429 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_os_release.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4247 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_osa_dispatcher_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)      825 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ovirt_engine_confd.py
+-rw-rw-r--   0 release   (1002) release   (1002)    18312 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ovirt_engine_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1778 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ovs_appctl_fdb_show_bridge.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5864 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ovs_ofctl_dump_flows.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4322 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ovs_vsctl.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4355 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ovs_vsctl_list_bridge.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3416 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ovs_vsctl_show.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1870 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_pacemaker_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1636 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_package_provides.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9823 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_pam.py
+-rw-rw-r--   0 release   (1002) release   (1002)    24589 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_parsers_module.py
+-rw-rw-r--   0 release   (1002) release   (1002)    12335 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_parted.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2830 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_partitions.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4289 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_passenger_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2281 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_password.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2861 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_pci_rport_target_disk_paths.py
+-rw-rw-r--   0 release   (1002) release   (1002)      960 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_pcp_openmetrics_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5271 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_pcs_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2661 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_pcs_quorum_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)    17328 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_pcs_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4104 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_php_ini.py
+-rw-rw-r--   0 release   (1002) release   (1002)      954 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_pluginconf_d.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2236 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_pmlog_summary.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3337 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_pmrep.py
+-rw-rw-r--   0 release   (1002) release   (1002)    19834 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_podman_inspect.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5155 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_podman_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2258 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_postconf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9240 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_postgresql_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)      801 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_postgresql_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5888 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_proc_environ.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2163 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_proc_keys.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2291 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_proc_keyusers.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2934 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_proc_limits.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2709 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_proc_stat.py
+-rw-rw-r--   0 release   (1002) release   (1002)    27171 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ps.py
+-rw-rw-r--   0 release   (1002) release   (1002)      887 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_pulp_worker_defaults.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1949 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_puppet_ca_cert_expire_date.py
+-rw-rw-r--   0 release   (1002) release   (1002)    27712 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_pvs.py
+-rw-rw-r--   0 release   (1002) release   (1002)      995 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_qemu_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    26811 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_qemu_xml.py
+-rw-rw-r--   0 release   (1002) release   (1002)    14000 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_qpid_stat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1011 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_qpidd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1036 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rabbit_users.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2399 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rabbitmq_env.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2141 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rabbitmq_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2872 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rabbitmq_queues.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8812 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rabbitmq_report.py
+-rw-rw-r--   0 release   (1002) release   (1002)      680 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rc_local.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2524 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rdma_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)      827 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_readlink_mtab.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1752 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_readlink_openshift_certs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6066 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_redhat_release.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2742 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_repquota.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1430 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_resolv_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1786 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rhev_data_center.py
+-rw-rw-r--   0 release   (1002) release   (1002)      773 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rhn_charsets.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1159 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rhn_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2004 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rhn_entitlement_cert_xml.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1817 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rhn_hibernate_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7464 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rhn_logs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8028 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rhn_schema_stats.py
+-rw-rw-r--   0 release   (1002) release   (1002)      491 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rhn_schema_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)      858 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rhosp_release.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2336 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rhsm_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2433 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rhsm_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1944 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rhsm_releasever.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5570 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rhv_log_collector_analyzer.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1662 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rndc_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2730 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ros_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)      957 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_route.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1702 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rpm_ostree_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)      898 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rpm_pkgs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1871 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rpm_v_packages.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4484 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rpm_vercmp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1780 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_rsyslog_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8606 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_samba.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2312 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_samba_logs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3202 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sap_dev_trace_files.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5156 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sap_hana_python_script.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2653 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sap_hdb_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1396 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sap_host_profile.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1758 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sapcontrol.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7207 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_saphostctrl.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3100 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_saphostexec.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1079 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sat5_insights_properties.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1584 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_satellite_content_hosts_count.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1137 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_satellite_enabled_features.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1969 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_satellite_installer_configurations.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2718 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_satellite_missed_queues.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3166 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_satellite_mongodb.py
+-rw-rw-r--   0 release   (1002) release   (1002)    11401 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_satellite_postgresql_query.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1063 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_satellite_version.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1744 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_satellite_yaml.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2499 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_scheduler.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3584 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_scsi.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1528 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_scsi_eh_deadline.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1486 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_scsi_fwver.py
+-rw-rw-r--   0 release   (1002) release   (1002)    12986 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sctp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5819 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sealert.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2347 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_secure.py
+-rw-rw-r--   0 release   (1002) release   (1002)      918 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_selinux_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)      704 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_semanage.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1758 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sendq_recvq_socket_buffer.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4770 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sestatus.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4222 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_setup_named_chroot.py
+-rw-rw-r--   0 release   (1002) release   (1002)    16872 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_slabinfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)    13335 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_smartctl.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1256 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_smartpdc_settings.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4530 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_smbstatus.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2489 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_smt.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6178 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_snmp.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1592 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sockstat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5695 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_softnet_stat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2002 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_software_collections_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)      819 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sos_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2351 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_spamassassin_channels.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4513 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ssh.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3721 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ssh_client_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8503 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_ssl_certificate.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2442 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sssd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3147 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sssd_logs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1255 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_subscription_manager.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4145 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_subscription_manager_list.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2405 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_subscription_manager_release.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1285 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sudoers.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4449 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_swift_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3821 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_swift_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1081 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sys_block.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1148 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sys_bus.py
+-rw-rw-r--   0 release   (1002) release   (1002)      516 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sys_fs_cgroup_memory.py
+-rw-rw-r--   0 release   (1002) release   (1002)      389 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sys_fs_cgroup_memory_tasks_number.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1225 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sys_kernel.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4947 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sys_module.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2695 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sys_vmbus.py
+-rw-rw-r--   0 release   (1002) release   (1002)      308 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_chronyd.py
+-rw-rw-r--   0 release   (1002) release   (1002)      756 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_corosync.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1088 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_dirsrv.py
+-rwxrwxr-x   0 release   (1002) release   (1002)     7988 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_doc_examples.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2303 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_docker.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1158 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_docker_storage.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1483 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_docker_storage_setup.py
+-rw-rw-r--   0 release   (1002) release   (1002)      766 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_grub.py
+-rw-rw-r--   0 release   (1002) release   (1002)      998 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_httpd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1317 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_ifcfg_static_route.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1323 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_irqbalance.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2140 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_kdump.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2637 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_libvirt_guests.py
+-rw-rw-r--   0 release   (1002) release   (1002)      678 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_memcached.py
+-rw-rw-r--   0 release   (1002) release   (1002)      507 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_mongod.py
+-rw-rw-r--   0 release   (1002) release   (1002)      963 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_netconsole.py
+-rw-rw-r--   0 release   (1002) release   (1002)      445 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_network.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1807 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_nfs.py
+-rw-rw-r--   0 release   (1002) release   (1002)      298 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_ntpd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1260 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_oracleasm.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1909 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_prelink.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1753 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_puppetserver.py
+-rw-rw-r--   0 release   (1002) release   (1002)      863 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_sshd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3816 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_up2date.py
+-rw-rw-r--   0 release   (1002) release   (1002)      602 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysconfig_virt_who.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3503 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_sysctl.py
+-rw-rw-r--   0 release   (1002) release   (1002)    12610 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_system_time.py
+-rw-rw-r--   0 release   (1002) release   (1002)    12392 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_systemctl_show.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1637 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_systemctl_status_all.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1479 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_systemd_analyze.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9023 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_systemd_config.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2226 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_systemid.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6146 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_systool.py
+-rw-rw-r--   0 release   (1002) release   (1002)      991 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_tags.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1336 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_teamdctl_config_dump.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3165 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_teamdctl_state_dump.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1856 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_tmpfilesd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3432 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_tomcat_virtual_dir_context.py
+-rw-rw-r--   0 release   (1002) release   (1002)    55650 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_tomcat_xml.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1533 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_transparent_hugepage.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4020 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_tuned.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2813 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_tuned_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5122 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_udev_rules.py
+-rw-rw-r--   0 release   (1002) release   (1002)    21242 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_uname.py
+-rw-rw-r--   0 release   (1002) release   (1002)    37286 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_unitfiles.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3046 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_up2date_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2697 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_upstart.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2496 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_uptime.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1018 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_user_group.py
+-rw-rw-r--   0 release   (1002) release   (1002)    21095 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_vdo_status.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3063 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_vdsm_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)    21905 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_vdsm_log.py
+-rw-rw-r--   0 release   (1002) release   (1002)      953 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_version_info.py
+-rw-rw-r--   0 release   (1002) release   (1002)    14025 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_vgdisplay.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4743 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_vgs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2490 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_virsh_list_all.py
+-rw-rw-r--   0 release   (1002) release   (1002)      994 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_virt_uuid_facts.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1162 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_virt_what.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1748 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_virt_who_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2717 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_virtlogd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1264 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_vma_ra_enabled_s390x.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2821 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_vmcore_dmesg.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1001 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_vmware_tools_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2941 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_vsftpd.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1457 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_wc_proc_1_mountinfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3189 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_x86_debug.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7664 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_xfs_info.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4295 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_xinetd_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3427 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_yum_conf.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4987 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_yum_list_available.py
+-rw-rw-r--   0 release   (1002) release   (1002)    12812 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_yum_repolist.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2066 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_yum_repos_d.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1841 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_yum_updateinfo.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1093 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_yum_updates.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3025 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_yumlog.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4629 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_zdump_v.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3036 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/parsers/test_zipl_conf.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/tests/test_plugins/
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_plugins/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)      183 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_plugins/test_plugin.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2564 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_plugins/test_returns_none.py
+-rw-rw-r--   0 release   (1002) release   (1002)      110 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_plugins/tina_loves_butts.py
+-rw-rw-r--   0 release   (1002) release   (1002)    13893 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3075 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/helpers.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1604 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/integration.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3022 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/mock_web_server.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1328 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/spec_tests.py
+-rw-rw-r--   0 release   (1002) release   (1002)      341 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_add_component.py
+-rw-rw-r--   0 release   (1002) release   (1002)      292 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_always_fires.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2193 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_broker_exceptions.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3396 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_canonical_facts.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1433 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_collect.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1111 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_command_parser.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1752 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_commandparser.py
+-rw-rw-r--   0 release   (1002) release   (1002)      556 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_component_metadata.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3815 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_config_parser.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2547 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_context.py
+-rw-rw-r--   0 release   (1002) release   (1002)      810 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_context_wrap.py
+-rw-rw-r--   0 release   (1002) release   (1002)      816 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_determine_components.py
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_doc_examples.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1011 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_dr_enabled.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5447 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_dr_run.py
+-rw-rw-r--   0 release   (1002) release   (1002)     9093 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_evaluators.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1279 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_extractors.py
+-rw-rw-r--   0 release   (1002) release   (1002)    13568 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_file_listing.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5942 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_file_permissions.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4005 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_filters.py
+-rw-rw-r--   0 release   (1002) release   (1002)      947 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_find.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2693 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_formats.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1858 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_fs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4753 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_get_dependency_specs.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1082 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_insights_heartbeat.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1279 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_integration_support.py
+-rw-rw-r--   0 release   (1002) release   (1002)      927 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_json_parser.py
+-rw-rw-r--   0 release   (1002) release   (1002)    16221 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_logfileoutput.py
+-rw-rw-r--   0 release   (1002) release   (1002)    12368 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_ls_parser.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1816 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_parser_class.py
+-rw-rw-r--   0 release   (1002) release   (1002)      701 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_parser_continue_on_error.py
+-rw-rw-r--   0 release   (1002) release   (1002)      718 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_query.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2228 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_remote_resource.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1416 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_rules_fixture.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3994 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_scannable.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6783 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_serde.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8905 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_soscleaner.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1323 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_spec_serialization.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3968 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_specs.py
+-rw-rw-r--   0 release   (1002) release   (1002)      586 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_subproc.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3281 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_sysconfig_options.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2129 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_syslog.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2865 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_taglang.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1306 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_test.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8754 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_util.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1943 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_vulnerable_kernel.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1883 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_xmlparser.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1784 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tests/test_yaml_parser.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/tools/
+-rw-rw-r--   0 release   (1002) release   (1002)        0 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tools/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1481 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tools/apply_spec_filters.py
+-rwxrwxr-x   0 release   (1002) release   (1002)     5247 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tools/cat.py
+-rwxrwxr-x   0 release   (1002) release   (1002)     1497 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tools/dupkeycheck.py
+-rwxrwxr-x   0 release   (1002) release   (1002)     7791 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tools/insights_inspect.py
+-rwxrwxr-x   0 release   (1002) release   (1002)    12650 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/tools/query.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/util/
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights/util/autology/
+-rw-rw-r--   0 release   (1002) release   (1002)      125 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/util/autology/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)    19015 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/util/autology/datasources.py
+-rw-rw-r--   0 release   (1002) release   (1002)     8727 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/util/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)     5062 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/util/canonical_facts.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4703 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/util/command.py
+-rw-rw-r--   0 release   (1002) release   (1002)     4777 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/util/component_graph.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1264 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/util/content_type.py
+-rw-rw-r--   0 release   (1002) release   (1002)    14369 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/util/file_permissions.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2742 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/util/fs.py
+-rwxrwxr-x   0 release   (1002) release   (1002)     2114 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/util/mangle.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3945 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/util/specs_catalog.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3293 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/util/streams.py
+-rw-rw-r--   0 release   (1002) release   (1002)     6335 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/util/subproc.py
+-rw-rw-r--   0 release   (1002) release   (1002)       12 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/COMMIT
+-rw-rw-r--   0 release   (1002) release   (1002)       14 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/NAME
+-rw-rw-r--   0 release   (1002) release   (1002)        2 2023-06-08 07:10:24.000000 insights-core-3.2.0/insights/RELEASE
+-rw-rw-r--   0 release   (1002) release   (1002)        6 2023-06-08 07:12:59.000000 insights-core-3.2.0/insights/VERSION
+-rw-rw-r--   0 release   (1002) release   (1002)    18283 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/__init__.py
+-rw-rw-r--   0 release   (1002) release   (1002)       82 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/__main__.py
+-rwxrwxr-x   0 release   (1002) release   (1002)    16727 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/collect.py
+-rw-rw-r--   0 release   (1002) release   (1002)     3671 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/command_parser.py
+-rw-rw-r--   0 release   (1002) release   (1002)     2840 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/defaults.yaml
+-rw-rw-r--   0 release   (1002) release   (1002)     2492 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/ocp.py
+-rwxrwxr-x   0 release   (1002) release   (1002)     2151 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/ocpshell.py
+-rw-rw-r--   0 release   (1002) release   (1002)     1446 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/settings.py
+-rw-rw-r--   0 release   (1002) release   (1002)    32867 2023-06-08 07:07:17.000000 insights-core-3.2.0/insights/shell.py
+drwxrwxr-x   0 release   (1002) release   (1002)        0 2023-06-08 07:16:07.000000 insights-core-3.2.0/insights_core.egg-info/
+-rw-rw-r--   0 release   (1002) release   (1002)     7667 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights_core.egg-info/PKG-INFO
+-rw-rw-r--   0 release   (1002) release   (1002)    58757 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 release   (1002) release   (1002)        1 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 release   (1002) release   (1002)      399 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights_core.egg-info/entry_points.txt
+-rw-rw-r--   0 release   (1002) release   (1002)     3538 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights_core.egg-info/requires.txt
+-rw-rw-r--   0 release   (1002) release   (1002)       18 2023-06-08 07:16:06.000000 insights-core-3.2.0/insights_core.egg-info/top_level.txt
+-rw-rw-r--   0 release   (1002) release   (1002)    11357 2023-06-08 07:07:17.000000 insights-core-3.2.0/LICENSE
+-rw-rw-r--   0 release   (1002) release   (1002)      221 2023-06-08 07:07:17.000000 insights-core-3.2.0/MANIFEST.in
+-rw-rw-r--   0 release   (1002) release   (1002)     5370 2023-06-08 07:07:17.000000 insights-core-3.2.0/README.rst
+-rw-rw-r--   0 release   (1002) release   (1002)      398 2023-06-08 07:16:07.000000 insights-core-3.2.0/setup.cfg
+-rw-rw-r--   0 release   (1002) release   (1002)     4399 2023-06-08 07:12:59.000000 insights-core-3.2.0/setup.py
+-rw-rw-r--   0 release   (1002) release   (1002)     7667 2023-06-08 07:16:07.000000 insights-core-3.2.0/PKG-INFO
```

### Comparing `insights-core-3.1.9/examples/cluster_rules/allnodes_cpu.py` & `insights-core-3.2.0/examples/cluster_rules/allnodes_cpu.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/examples/cluster_rules/bash_version.py` & `insights-core-3.2.0/examples/cluster_rules/bash_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/examples/cluster_rules/ntp_compare.py` & `insights-core-3.2.0/examples/cluster_rules/ntp_compare.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/examples/rules/bash_version.py` & `insights-core-3.2.0/examples/rules/bash_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/examples/rules/hostname_rel.py` & `insights-core-3.2.0/examples/rules/hostname_rel.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/examples/rules/sample_script.py` & `insights-core-3.2.0/examples/rules/sample_script.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/examples/rules/skip_component.py` & `insights-core-3.2.0/examples/rules/skip_component.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/examples/rules/stand_alone.py` & `insights-core-3.2.0/examples/rules/stand_alone.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/__init__.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/comments.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/comments.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/compat.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/compat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/composer.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/constructor.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/cyaml.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/dumper.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/emitter.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/error.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/error.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/events.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/events.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/loader.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/main.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/main.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/nodes.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/parser.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/reader.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/representer.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/resolver.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarbool.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarbool.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarfloat.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarfloat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarint.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarint.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarstring.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scalarstring.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scanner.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/serializer.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/timestamp.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/timestamp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/tokens.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/util.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/ruamel_yaml/ruamel/yaml/util.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/gnupg.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/gnupg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/contrib/oyaml.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/contrib/oyaml.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/__init__.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,18 +219,18 @@
         if isinstance(value, CommentedMap):
             new[key] = CommentedMap(normalizeSnippet(value))
         elif isinstance(value, CommentedSeq):
             new_sequence = CommentedSeq()
             for item in value:
                 if isinstance(item, six.text_type):
                     new_sequence.append(item.encode('ascii', 'ignore'))
-                if not isinstance(item, CommentedMap):
-                    new_sequence.append(item)
-                else:
+                elif isinstance(item, CommentedMap):
                     new_sequence.append(normalizeSnippet(item))
+                else:
+                    new_sequence.append(item)
             new[key] = new_sequence
         elif isinstance(value, six.text_type):
             new[key] = value.encode('ascii', 'ignore')
         elif isinstance(value, ScalarInt):
             new[key] = int(value)
         else:
             new[key] = value
```

### Comparing `insights-core-3.1.9/insights/client/apps/ansible/playbook_verifier/__main__.py` & `insights-core-3.2.0/insights/client/apps/ansible/playbook_verifier/__main__.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/apps/compliance/__init__.py` & `insights-core-3.2.0/insights/client/apps/compliance/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,19 +25,21 @@
 else:
     try:
         import defusedxml.ElementTree as ET
     except:
         import xml.etree.ElementTree as ET
 
 NONCOMPLIANT_STATUS = 2
+OUT_OF_MEMORY_STATUS = -9  # 247
 COMPLIANCE_CONTENT_TYPE = 'application/vnd.redhat.compliance.something+tgz'
 POLICY_FILE_LOCATION = '/usr/share/xml/scap/ssg/content/'
 SCAP_DATASTREAMS_PATH = '/usr/share/xml/scap/'
 SSG_PACKAGE = 'scap-security-guide'
 REQUIRED_PACKAGES = [SSG_PACKAGE, 'openscap-scanner', 'openscap']
+OOM_ERROR_LINK = 'https://access.redhat.com/articles/6999111'
 
 # SSG versions that need the <version> in XML repaired
 VERSIONS_FOR_REPAIR = '0.1.18 0.1.19 0.1.21 0.1.25'.split()
 SNIPPET_TO_FIX = '<version>0.9</version>'
 
 logger = getLogger(__name__)
 
@@ -148,15 +150,15 @@
     def os_major_version(self):
         return findall("^[6-9]", self.os_release())[0]
 
     def os_minor_version(self):
         return findall("\d+$", self.os_release())[0]
 
     def profile_files(self):
-        return glob("{0}*rhel{1}*.xml".format(POLICY_FILE_LOCATION, self.os_major_version()))
+        return glob("{0}*rhel{1}-ds.xml".format(POLICY_FILE_LOCATION, self.os_major_version()))
 
     def find_scap_policy(self, profile_ref_id):
         grepcmd = 'grep -H ' + profile_ref_id + ' ' + ' '.join(self.profile_files())
         if not six.PY3:
             grepcmd = grepcmd.encode()
         rc, grep = call(grepcmd, keep_rc=True)
         if rc:
@@ -181,16 +183,23 @@
         logger.info('Running scan for {0}... this may take a while'.format(profile_ref_id))
         env = os.environ.copy()
         env.update({'TZ': 'UTC'})
         oscap_command = self.build_oscap_command(profile_ref_id, policy_xml, output_path, tailoring_file_path)
         if not six.PY3:
             oscap_command = oscap_command.encode()
         rc, oscap = call(oscap_command, keep_rc=True, env=env)
+
+        if rc and rc == OUT_OF_MEMORY_STATUS:
+            logger.error('Scan failed due to insufficient memory')
+            logger.error('More information can be found here: {0}'.format(OOM_ERROR_LINK))
+            exit(constants.sig_kill_bad)
+
         if rc and rc != NONCOMPLIANT_STATUS:
             logger.error('Scan failed')
+            logger.error(rc)
             logger.error(oscap)
             exit(constants.sig_kill_bad)
 
     @property
     def ssg_version(self):
         if not self._ssg_version:
             self._ssg_version = self.get_ssg_version()
```

### Comparing `insights-core-3.1.9/insights/client/apps/malware_detection/__init__.py` & `insights-core-3.2.0/insights/client/apps/malware_detection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -638,15 +638,15 @@
         signatures_file = 'signatures.yar'
         signatures_file += '?yara_version=' + self.yara_version if hasattr(self, 'yara_version') else ''
         if not self.rules_location:
             self.rules_location = 'https://console.redhat.com/api/malware-detection/v1/' + signatures_file
             if '/redhat_access/' in self.insights_config.base_url:
                 # Satellite URLs have '/redhat_access/' in the base_url config option
                 self.rules_location = self.insights_config.base_url + '/malware-detection/v1/' + signatures_file
-            elif '.stage.redhat.com' in self.insights_config.base_url:
+            elif any([url in self.insights_config.base_url for url in ['console.stage.', 'cloud.stage.']]):
                 # For downloading rules in the stage environment, use the URL of base_url (after finding it)
                 base_url = urlparse(self.insights_config.base_url)
                 self.rules_location = base_url.netloc or base_url.scheme or base_url.path.split('/')[0] or 'cert.console.stage.redhat.com'
                 self.rules_location += '/api/malware-detection/v1/' + signatures_file
 
         # Make sure the rules_location starts with https://
         if not re.match('^https?://', self.rules_location):
@@ -665,34 +665,52 @@
 
         # If doing a test scan, replace signatures.yar (or any other file suffix) with test-rule.yar
         log_rule_contents = False
         if self.test_scan:
             self.rules_location = self._get_test_rule_location(self.rules_location)
             log_rule_contents = True
 
+        # If a custom CA cert is being used, eg on a Satellite, then SSL errors may occur when downloading the rules
+        # The CA cert needs to be added to a CA bundle (with update-ca-trust) and the bundle used for cert verification
+        ca_cert = None
+        ca_bundles = ['/etc/pki/ca-trust/extracted/pem/tls-ca-bundle.pem', '/etc/pki/tls/certs/ca-bundle.crt']
+        for ca_bundle in ca_bundles:
+            if os.path.isfile(ca_bundle):
+                ca_cert = ca_bundle
+                break
+
         logger.debug("Downloading rules from: %s", self.rules_location)
         self.insights_config.cert_verify = True
         conn = InsightsConnection(self.insights_config)
 
         for attempt in range(1, self.insights_config.retries + 1):
             try:
-                response = conn.get(self.rules_location, log_response_text=log_rule_contents)
+                response = conn.get(
+                    self.rules_location,
+                    log_response_text=log_rule_contents,
+                    verify=self.insights_config.cert_verify
+                )
                 if response.status_code != 200:
                     raise Exception("%s %s: %s" % (response.status_code, response.reason, response.text))
                 break
             except Exception as e:
                 if attempt < self.insights_config.retries:
                     logger.debug("Unable to download rules from %s: %s", self.rules_location, str(e))
                     retry_delay = attempt ** 2
                     logger.debug("Trying again in %d seconds ...", retry_delay)
                     time.sleep(retry_delay)
                 else:
                     logger.error("Unable to download rules from %s: %s", self.rules_location, str(e))
                     exit(constants.sig_kill_bad)
 
+                if re.search('SSL.*verify.failed', str(e), re.IGNORECASE):
+                    # SSL error occurred, possibly due to a custom CA cert, try using a CA bundle for cert verification
+                    self.insights_config.cert_verify = self._get_config_option('ca_cert', ca_cert)
+                    logger.debug("Trying cert_verify value %s ...", self.insights_config.cert_verify)
+
         self.temp_rules_file = NamedTemporaryFile(prefix='.tmpmdsigs', mode='wb', delete=True)
         self.temp_rules_file.write(response.content)
         self.temp_rules_file.flush()
         return self.temp_rules_file.name
 
     def _build_yara_command(self):
         """
```

### Comparing `insights-core-3.1.9/insights/client/apps/manifests.py` & `insights-core-3.2.0/insights/client/apps/manifests.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/phase/v1.py` & `insights-core-3.2.0/insights/client/phase/v1.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/__init__.py` & `insights-core-3.2.0/insights/client/__init__.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/archive.py` & `insights-core-3.2.0/insights/client/archive.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/auto_config.py` & `insights-core-3.2.0/insights/client/auto_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/cert_auth.py` & `insights-core-3.2.0/insights/client/cert_auth.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/client.py` & `insights-core-3.2.0/insights/client/client.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/collection_rules.py` & `insights-core-3.2.0/insights/client/collection_rules.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/config.py` & `insights-core-3.2.0/insights/client/config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/connection.py` & `insights-core-3.2.0/insights/client/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -637,14 +637,18 @@
         systems = {'machine_id': generate_machine_id()}
         self.group_systems(group_id, systems)
 
     # -LEGACY-
     def _legacy_api_registration_check(self):
         '''
         Check registration status through API
+            True    system exists in inventory
+            False   connection or parsing response error
+            None    system is not yet registered
+            string system is unregistered
         '''
         logger.debug('Checking registration status...')
         machine_id = generate_machine_id()
         try:
             url = self.api_url + '/v1/systems/' + machine_id
             res = self.get(url)
         except requests.ConnectionError:
@@ -654,32 +658,39 @@
             return False
         # had to do a quick bugfix changing this around,
         #   which makes the None-False-True dichotomy seem weird
         #   TODO: reconsider what gets returned, probably this:
         #       True for registered
         #       False for unregistered
         #       None for system 404
-        self.handle_fail_rcs(res)
-        try:
-            # check the 'unregistered_at' key of the response
-            unreg_status = json.loads(res.content).get('unregistered_at', 'undefined')
-            # set the global account number
-            self.config.account_number = json.loads(res.content).get('account_number', 'undefined')
-        except ValueError:
-            # bad response, no json object
+        if res.status_code != 200:
+            self.handle_fail_rcs(res)
+        if res.status_code not in (200, 404):
+            # Network error returns False
             return False
-        if unreg_status == 'undefined':
-            # key not found, machine not yet registered
-            return None
-        elif unreg_status is None:
-            # unregistered_at = null, means this machine IS registered
-            return True
         else:
-            # machine has been unregistered, this is a timestamp
-            return unreg_status
+            try:
+                # check the 'unregistered_at' key of the response
+                unreg_status = json.loads(res.content).get('unregistered_at', 'undefined')
+                # set the global account number
+                self.config.account_number = json.loads(res.content).get('account_number', 'undefined')
+            except ValueError:
+                # bad response, no json object
+                return False
+            if unreg_status == 'undefined':
+                # key not found, machine not yet registered
+                return None
+            elif unreg_status is None:
+                # unregistered_at = null, means this machine IS registered
+                return True
+            else:
+                # machine has been unregistered, this is a timestamp
+                # This is done for legacy servers that responded with the timestamp of disconnection
+                # TODO: consider to remove this condition
+                return unreg_status
 
     def _fetch_system_by_machine_id(self):
         '''
         Get a system by machine ID
         Returns
             dict    system exists in inventory
             False   system does not exist in inventory
@@ -1091,15 +1102,15 @@
         if content is None:
             return None
 
         host_details = json.loads(content)
         if host_details["total"] < 1:
             _host_not_found()
         if host_details["total"] > 1:
-            raise Exception("Error: multiple hosts detected (insights_id = %s)" % generate_machine_id())
+            raise Exception("Error: multiple hosts detected (insights_id = %s). To fix this error, run command: insights-client --unregister && insights-client --register" % generate_machine_id())
 
         if not os.path.exists("/var/lib/insights"):
             os.makedirs("/var/lib/insights", mode=0o755)
 
         with open("/var/lib/insights/host-details.json", mode="w+b") as f:
             f.write(content)
             logger.debug("Wrote \"/var/lib/insights/host-details.json\"")
```

### Comparing `insights-core-3.1.9/insights/client/constants.py` & `insights-core-3.2.0/insights/client/constants.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/core_collector.py` & `insights-core-3.2.0/insights/client/core_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,9 +90,10 @@
         logger.debug('Collecting metadata...')
         self._write_branch_info(branch_info)
         self._write_display_name()
         self._write_ansible_host()
         self._write_version_info()
         self._write_tags()
         self._write_blacklist_report(blacklist_report)
+        self._write_blacklisted_specs()
         self._write_egg_release()
         logger.debug('Metadata collection finished.')
```

### Comparing `insights-core-3.1.9/insights/client/data_collector.py` & `insights-core-3.2.0/insights/client/data_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,17 +129,20 @@
             self.archive.add_metadata_to_archive(json.dumps(t), '/tags.json')
 
     def _write_blacklist_report(self, blacklist_report):
         logger.debug("Writing blacklist report to archive...")
         self.archive.add_metadata_to_archive(
             json.dumps(blacklist_report), '/blacklist_report')
 
+    def _write_blacklisted_specs(self):
+        logger.debug("Writing blacklisted specs to archive...")
+
         if BLACKLISTED_SPECS:
             self.archive.add_metadata_to_archive(
-                json.dumps({"specs": BLACKLISTED_SPECS}), '/blacklisted_specs.txt')
+                json.dumps({"specs": BLACKLISTED_SPECS}), '/blacklisted_specs')
 
     def _write_egg_release(self):
         logger.debug("Writing egg release to archive...")
         egg_release = ''
         try:
             with open(constants.egg_release_file) as fil:
                 egg_release = fil.read()
@@ -392,14 +395,15 @@
         logger.debug('Collecting metadata...')
         self._write_branch_info(branch_info)
         self._write_display_name()
         self._write_ansible_host()
         self._write_version_info()
         self._write_tags()
         self._write_blacklist_report(blacklist_report)
+        self._write_blacklisted_specs()
         self._write_egg_release()
         self._write_collection_stats(collection_stats)
         logger.debug('Metadata collection finished.')
 
     def redact(self, rm_conf):
         '''
         Perform data redaction (password sed command and patterns),
```

### Comparing `insights-core-3.1.9/insights/client/insights_spec.py` & `insights-core-3.2.0/insights/client/insights_spec.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/map_components.py` & `insights-core-3.2.0/insights/client/map_components.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/schedule.py` & `insights-core-3.2.0/insights/client/schedule.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/subp.py` & `insights-core-3.2.0/insights/client/subp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/support.py` & `insights-core-3.2.0/insights/client/support.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/url_cache.py` & `insights-core-3.2.0/insights/client/url_cache.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/client/utilities.py` & `insights-core-3.2.0/insights/client/utilities.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/ansible_info.py` & `insights-core-3.2.0/insights/combiners/ansible_info.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/ceph_osd_tree.py` & `insights-core-3.2.0/insights/combiners/ceph_osd_tree.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/ceph_version.py` & `insights-core-3.2.0/insights/combiners/ceph_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/cloud_instance.py` & `insights-core-3.2.0/insights/combiners/cloud_instance.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/cloud_provider.py` & `insights-core-3.2.0/insights/combiners/cloud_provider.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/cpu_vulns_all.py` & `insights-core-3.2.0/insights/combiners/cpu_vulns_all.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/crio_conf.py` & `insights-core-3.2.0/insights/combiners/crio_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/cryptsetup.py` & `insights-core-3.2.0/insights/combiners/cryptsetup.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/dmesg.py` & `insights-core-3.2.0/insights/combiners/dmesg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/dnsmasq_conf_all.py` & `insights-core-3.2.0/insights/combiners/dnsmasq_conf_all.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/du.py` & `insights-core-3.2.0/insights/combiners/du.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/grub_conf.py` & `insights-core-3.2.0/insights/combiners/grub_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/hostname.py` & `insights-core-3.2.0/insights/combiners/hostname.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/httpd_conf.py` & `insights-core-3.2.0/insights/combiners/httpd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/ipcs_semaphores.py` & `insights-core-3.2.0/insights/combiners/ipcs_semaphores.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/ipcs_shared_memory.py` & `insights-core-3.2.0/insights/combiners/ipcs_shared_memory.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/ipv6.py` & `insights-core-3.2.0/insights/combiners/ipv6.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/journald_conf.py` & `insights-core-3.2.0/insights/combiners/journald_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/krb5.py` & `insights-core-3.2.0/insights/combiners/krb5.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ==================
 The krb5 files are normally available to rules as a list of
 Krb5Configuration objects.
 """
 from copy import deepcopy
 from insights.core import LegacyItemAccess
 from insights.core.plugins import combiner
-from insights.parsers.krb5 import Krb5Configuration
+from insights.parsers.krb5 import Krb5Configuration, _handle_krb5_bool
 
 
 @combiner(Krb5Configuration)
 class AllKrb5Conf(LegacyItemAccess):
     """
     Combiner for accessing all the krb5 configuration files, the format is dict.
     There may be multi files for krb5 configuration, and the main config file is
@@ -64,14 +64,18 @@
         includedir (list): The directory list that `krb5.conf` includes via
             `includedir` directive
         include (list): The configuration file list that `krb5.conf` includes
             via `include` directive
         module (list): The module list that `krb5.conf` specifed via 'module'
             directive
         files (list): The list of configuration file names.
+        dns_lookup_realm (bool): is Kerberos realm DNS lookup enabled?
+        dns_lookup_kdc (bool): is Kerberos KDC DNS lookup enabled?
+        default_realm (str/None): default realm for clients
+        realms (set): realm names from [realms] block
 
     """
     def __init__(self, krb5configs):
         self.data = {}
         main_data = {}
         self.includedir = []
         self.include = []
@@ -91,14 +95,38 @@
         # from main configuration, but different options in same section will be kept.
         for key, value in main_data.items():
             if key in self.data.keys():
                 self.data[key].update(value)
             else:
                 self.data[key] = value
 
+        def _getbool(option, default=None):
+            if not self.has_option("libdefaults", option):
+                return default
+            return self.getboolean("libdefaults", option)
+
+        self.dns_lookup_realm = _getbool("dns_lookup_realm", True)
+        self.dns_lookup_kdc = _getbool("dns_lookup_kdc", True)
+        if self.has_option("libdefaults", "default_realm"):
+            self.default_realm = self["libdefaults"]["default_realm"]
+        else:
+            self.default_realm = None
+
+        self.realms = set()
+        if self.has_section("realms"):
+            r = self["realms"]
+            for name, value in r.items():
+                if (
+                    # realm entries must be dicts
+                    isinstance(value, dict) and
+                    # realm names look like "UPPER-CASE.COM"
+                    not any(c.islower() or c == "_" for c in name)
+                ):
+                    self.realms.add(name)
+
         super(AllKrb5Conf, self).__init__()
 
     def sections(self):
         """
         Return a list of section names.
         """
         return self.data.keys()
@@ -121,14 +149,22 @@
         Check for the existence of a given option in a given section.
         Return True if the given option is present, and False if not present.
         """
         if section not in self.data:
             return False
         return option in self.data[section]
 
+    def getboolean(self, section, option):
+        """Parse option as bool
+
+        Returns None is not a krb5.conf boolean string.
+        """
+        value = self.data[section][option]
+        return _handle_krb5_bool(value)
+
 
 def dict_deep_merge(tgt, src):
     """
     Utility function to merge the source dictionary `src` to the target
     dictionary recursively
 
     Note:
```

### Comparing `insights-core-3.1.9/insights/combiners/limits_conf.py` & `insights-core-3.2.0/insights/combiners/limits_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/logrotate_conf.py` & `insights-core-3.2.0/insights/combiners/logrotate_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/lspci.py` & `insights-core-3.2.0/insights/combiners/lspci.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/lvm.py` & `insights-core-3.2.0/insights/combiners/lvm.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/md5check.py` & `insights-core-3.2.0/insights/combiners/md5check.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/mlx4_port.py` & `insights-core-3.2.0/insights/combiners/mlx4_port.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/modprobe.py` & `insights-core-3.2.0/insights/combiners/modprobe.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/multinode.py` & `insights-core-3.2.0/insights/combiners/multinode.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/netstat.py` & `insights-core-3.2.0/insights/combiners/netstat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/nfs_exports.py` & `insights-core-3.2.0/insights/combiners/nfs_exports.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/nginx_conf.py` & `insights-core-3.2.0/insights/combiners/nginx_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/nmcli_dev_show.py` & `insights-core-3.2.0/insights/combiners/nmcli_dev_show.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/ps.py` & `insights-core-3.2.0/insights/combiners/ps.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/redhat_release.py` & `insights-core-3.2.0/insights/combiners/redhat_release.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/rhel_for_edge.py` & `insights-core-3.2.0/insights/combiners/rhel_for_edge.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/rhsm_release.py` & `insights-core-3.2.0/insights/combiners/rhsm_release.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/rsyslog_confs.py` & `insights-core-3.2.0/insights/combiners/rsyslog_confs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/sap.py` & `insights-core-3.2.0/insights/combiners/sap.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/satellite_version.py` & `insights-core-3.2.0/insights/combiners/satellite_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/selinux.py` & `insights-core-3.2.0/insights/combiners/selinux.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/services.py` & `insights-core-3.2.0/insights/combiners/services.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/smt.py` & `insights-core-3.2.0/insights/combiners/smt.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/ssl_certificate.py` & `insights-core-3.2.0/insights/combiners/ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/sudoers.py` & `insights-core-3.2.0/insights/combiners/sudoers.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/sys_vmbus_devices.py` & `insights-core-3.2.0/insights/combiners/sys_vmbus_devices.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/sysctl_conf.py` & `insights-core-3.2.0/insights/combiners/sysctl_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/tmpfilesd.py` & `insights-core-3.2.0/insights/combiners/tmpfilesd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/tomcat_virtual_dir_context.py` & `insights-core-3.2.0/insights/combiners/tomcat_virtual_dir_context.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/user_namespaces.py` & `insights-core-3.2.0/insights/combiners/user_namespaces.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/virt_what.py` & `insights-core-3.2.0/insights/combiners/virt_what.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/virt_who_conf.py` & `insights-core-3.2.0/insights/combiners/virt_who_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/combiners/x86_page_branch.py` & `insights-core-3.2.0/insights/combiners/x86_page_branch.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/components/ceph.py` & `insights-core-3.2.0/insights/components/ceph.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/components/cloud_provider.py` & `insights-core-3.2.0/insights/components/cloud_provider.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/components/cryptsetup.py` & `insights-core-3.2.0/insights/components/cryptsetup.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/components/openstack.py` & `insights-core-3.2.0/insights/components/openstack.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/components/rhel_version.py` & `insights-core-3.2.0/insights/components/rhel_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/components/satellite.py` & `insights-core-3.2.0/insights/components/satellite.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/components/virtualization.py` & `insights-core-3.2.0/insights/components/virtualization.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/contrib/ElementPath.py` & `insights-core-3.2.0/insights/contrib/ElementPath.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/contrib/ElementTree.py` & `insights-core-3.2.0/insights/contrib/ElementTree.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/contrib/importlib.py` & `insights-core-3.2.0/insights/contrib/importlib.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/contrib/ipaddress.py` & `insights-core-3.2.0/insights/contrib/ipaddress.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/contrib/magic.py` & `insights-core-3.2.0/insights/contrib/magic.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/contrib/nginxparser.py` & `insights-core-3.2.0/insights/contrib/nginxparser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/contrib/pyparsing.py` & `insights-core-3.2.0/insights/contrib/pyparsing.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/contrib/soscleaner.py` & `insights-core-3.2.0/insights/contrib/soscleaner.py`

 * *Files 0% similar despite different names*

```diff
@@ -737,16 +737,16 @@
                 with open(file_path) as file:
                     meta_data = json.load(file)
                 if meta_data["name"] in self.excluded_specs:
                     if isinstance(meta_data["results"], list):
                         results = meta_data["results"]
                     else:
                         results = [meta_data["results"]]
-                    relative_paths = [result["object"]["relative_path"] for result in results]
-                    excluded_files.extend(relative_paths)
+                    relative_paths = [result["object"]["relative_path"] for result in results if result and 'object' in result]
+                    excluded_files.extend(relative_paths) if relative_paths else None
         return excluded_files
 
     def clean_report(self, options, sosreport): # pragma: no cover
         '''this is the primary function, to put everything together and analyze an sosreport'''
 
         if options.report_dir: # override the default location for artifacts (/tmp)
             if os.path.isdir(options.report_dir):
```

### Comparing `insights-core-3.1.9/insights/contrib/toposort.py` & `insights-core-3.2.0/insights/contrib/toposort.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/core/__init__.py` & `insights-core-3.2.0/insights/core/__init__.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/core/archives.py` & `insights-core-3.2.0/insights/core/archives.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/core/blacklist.py` & `insights-core-3.2.0/insights/core/blacklist.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/core/cluster.py` & `insights-core-3.2.0/insights/core/cluster.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/core/context.py` & `insights-core-3.2.0/insights/core/context.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/core/dr.py` & `insights-core-3.2.0/insights/core/dr.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,16 @@
 
 from collections import defaultdict
 from functools import reduce as _reduce
 
 from insights.contrib import importlib
 from insights.contrib.toposort import toposort_flatten
 from insights.core.blacklist import BLACKLISTED_SPECS
-from insights.core.exceptions import BlacklistedSpec, MissingRequirements, ParseException, SkipComponent
+from insights.core.context import SerializedArchiveContext
+from insights.core.exceptions import BlacklistedSpec, MissingRequirements, SkipComponent
 from insights.util import defaults, enum, KeyPassingDefaultDict
 
 log = logging.getLogger(__name__)
 
 GROUPS = enum("single", "cluster")
 
 MODULE_NAMES = {}
@@ -1045,27 +1046,26 @@
             broker.add_exception(component, bs, traceback.format_exc())
         except MissingRequirements as mr:
             if log.isEnabledFor(logging.DEBUG):
                 name = get_name(component)
                 reqs = stringify_requirements(mr.requirements)
                 log.debug("%s missing requirements %s" % (name, reqs))
             broker.add_exception(component, mr)
-        except ParseException as pe:
-            log.warning(pe)
-            broker.add_exception(component, pe, traceback.format_exc())
         except SkipComponent as sc:
             if broker.store_skips:
-                log.warning(sc)
+                log.debug(sc)
                 broker.add_exception(component, sc, traceback.format_exc())
             else:
                 pass
         except Exception as ex:
+            log.debug(ex)
             tb = traceback.format_exc()
-            log.warning(tb)
             broker.add_exception(component, ex, tb)
+            for reg_spec in get_registry_points(component):
+                broker.add_exception(reg_spec, ex, tb)
         finally:
             broker.exec_times[component] = time.time() - start
             broker.fire_observers(component)
 
     return broker
 
 
@@ -1084,14 +1084,22 @@
             initial dependency.
     Returns:
         Broker: The broker after evaluation.
     """
     components = components or COMPONENTS[GROUPS.single]
     components = determine_components(components)
     broker = broker or Broker()
+    # If a SerializedArchiveContext then data found in the archive's
+    # ./meta_data directory are prepopulated in the broker as Specs so
+    # no need to collect them again
+    if broker.get(SerializedArchiveContext) is not None:
+        for comp in list(components):
+            if comp in broker:
+                for dep in components[comp]:
+                    components.pop(dep, None)
     return run_components(run_order(components), components, broker)
 
 
 def generate_incremental(components=None, broker=None):
     components = components or COMPONENTS[GROUPS.single]
     components = determine_components(components)
     for graph in get_subgraphs(components):
```

### Comparing `insights-core-3.1.9/insights/core/evaluators.py` & `insights-core-3.2.0/insights/core/evaluators.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,18 +151,18 @@
         self.branch_info = {}
         self.product = "rhel"
         self.type = "host"
         self.release = None
 
     def observer(self, comp, broker):
         super(InsightsEvaluator, self).observer(comp, broker)
-        if self.system_id is None and Specs.machine_id in broker:
+        if self.system_id is None and Specs.machine_id in broker and broker[Specs.machine_id].content:
             self.system_id = broker[Specs.machine_id].content[0].strip()
 
-        if self.release is None and Specs.redhat_release in broker:
+        if self.release is None and Specs.redhat_release in broker and broker[Specs.redhat_release].content:
             self.release = broker[Specs.redhat_release].content[0].strip()
 
         if not self.branch_info and BranchInfo in broker:
             self.branch_info = broker[BranchInfo].data
 
         if comp is Specs.metadata_json and comp in broker:
             md = broker[comp]
```

### Comparing `insights-core-3.1.9/insights/core/exceptions.py` & `insights-core-3.2.0/insights/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/core/filters.py` & `insights-core-3.2.0/insights/core/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,18 @@
         component (a datasource): The target datasource
 
     Returns:
         set: The set of filters defined for the datasource
     """
     def inner(c, filters=None):
         filters = filters or set()
+
+        if hasattr(c, 'filterable') and c.filterable is False:
+            return filters
+
         if not ENABLED:
             return filters
 
         if not plugins.is_datasource(c):
             return filters
 
         if c in FILTERS:
@@ -184,18 +188,18 @@
         loads(stream.read())
     else:
         data = pkgutil.get_data(insights.__name__, _filename)
         return loads(data) if data else None
 
 
 def dumps():
-    """Returns a string representation of the FILTERS dictionary."""
+    """Returns a string representation of the sorted FILTERS dictionary."""
     d = {}
     for k, v in FILTERS.items():
-        d[dr.get_name(k)] = list(v)
+        d[dr.get_name(k)] = sorted(v)
     return _dumps(d)
 
 
 def dump(stream=None):
     """
     Dumps a string representation of `FILTERS` to a stream, normally an
     open file. If none is passed, `FILTERS` is dumped to a default location
```

### Comparing `insights-core-3.1.9/insights/core/hydration.py` & `insights-core-3.2.0/insights/core/hydration.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/core/ls_parser.py` & `insights-core-3.2.0/insights/core/ls_parser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/core/marshalling.py` & `insights-core-3.2.0/insights/core/marshalling.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/core/plugins.py` & `insights-core-3.2.0/insights/core/plugins.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/core/remote_resource.py` & `insights-core-3.2.0/insights/core/remote_resource.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/core/serde.py` & `insights-core-3.2.0/insights/core/serde.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/core/spec_factory.py` & `insights-core-3.2.0/insights/core/spec_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import traceback
 
 from collections import defaultdict
 from glob import glob
 from subprocess import call
 
 from insights.core import blacklist, dr
-from insights.core.context import ExecutionContext, FSRoots, HostContext
+from insights.core.context import FSRoots, ExecutionContext, HostContext, SerializedArchiveContext
 from insights.core.exceptions import BlacklistedSpec, ContentException, SkipComponent
 from insights.core.filters import _add_filter, get_filters
 from insights.core.plugins import component, datasource, is_datasource
 from insights.core.serde import deserializer, serializer
 from insights.util import fs, streams, which
 from insights.util.mangle import mangle_command
 from insights.util.subproc import Pipeline
@@ -37,22 +37,15 @@
 }
 """
 A minimal set of environment variables for use in subprocess calls
 """
 if "LANG" in os.environ:
     SAFE_ENV["LANG"] = os.environ["LANG"]
 
-
-def enc(s):
-    escape_encoding = "string_escape" if six.PY2 else "unicode_escape"
-    return s.encode(escape_encoding)
-
-
-def escape(s):
-    return re.sub(r"([=\(\)|\-_!@*~\"&/\\\^\$\=])", r"\\\1", s)
+safe_open = open if six.PY3 else codecs.open
 
 
 class ContentProvider(object):
     def __init__(self):
         self.cmd = None
         self.args = None
         self.rc = None
@@ -131,22 +124,30 @@
     def load(self):
         return self.content
 
 
 class FileProvider(ContentProvider):
     def __init__(self, relative_path, root="/", ds=None, ctx=None):
         super(FileProvider, self).__init__()
-        self.root = root
+        self.ds = ds
+        self.ctx = ctx
+        self._set_root(root)
         self.relative_path = relative_path.lstrip("/")
         self.file_name = os.path.basename(self.path)
 
-        self.ds = ds
-        self.ctx = ctx
         self.validate()
 
+    def _set_root(self, root):
+        if (isinstance(self.ctx, SerializedArchiveContext) and os.path.basename(root) != 'data'):
+            # For core-collection (SerializedArchiveContext) archive, data are
+            # in `/data` directory
+            self.root = os.path.join(root, 'data')
+        else:
+            self.root = root
+
     def validate(self):
         if not blacklist.allow_file("/" + self.relative_path):
             log.warning("WARNING: Skipping file %s", "/" + self.relative_path)
             raise BlacklistedSpec()
 
         if not os.path.exists(self.path):
             raise ContentException("%s does not exist." % self.path)
@@ -159,14 +160,51 @@
         if not os.access(self.path, os.R_OK):
             raise ContentException("Cannot access %s" % self.path)
 
     def __repr__(self):
         return '%s("%r")' % (self.__class__.__name__, self.path)
 
 
+class MetadataProvider(FileProvider):
+    """
+    Class used for insights-core built-in files.  These files should not
+    be filtered, redacted or blocked.
+    """
+    def _stream(self):
+        """
+        Returns a generator of lines instead of a list of lines.
+        """
+        if self._exception:
+            raise self._exception
+        try:
+            with safe_open(self.path, "r", encoding="utf-8", errors="surrogateescape") as f:
+                yield f
+        except StopIteration:
+            raise
+        except Exception as ex:
+            self._exception = ex
+            raise ContentException(str(ex))
+
+    def validate(self):
+        # Validate built-in metedata files only when insights-run
+        if not isinstance(self.ctx, HostContext):
+            super(MetadataProvider, self).validate()
+        # But DO NOT validate them when core-collecting
+
+    def load(self):
+        self.loaded = True
+        with safe_open(self.path, "r", encoding="utf-8", errors="surrogateescape") as f:
+            return [l.rstrip("\n") for l in f]
+
+    def write(self, dst):
+        # TODO: the built-ine metadata files can also be collected via
+        #       core-collection
+        pass
+
+
 class RawFileProvider(FileProvider):
     """
     Class used in datasources that returns the contents of a file a single
     string. The file is not filtered.
     """
 
     def load(self):
@@ -211,20 +249,17 @@
     def load(self):
         self.loaded = True
         args = self.create_args()
         if args:
             rc, out = self.ctx.shell_out(args, keep_rc=True, env=SAFE_ENV)
             self.rc = rc
             return out
-        if six.PY3:
-            with open(self.path, "r", encoding="utf-8", errors="surrogateescape") as f:
-                return [l.rstrip("\n") for l in f]
-        else:
-            with codecs.open(self.path, "r", encoding="utf-8", errors="surrogateescape") as f:
-                return [l.rstrip("\n") for l in f]
+
+        with safe_open(self.path, "r", encoding="utf-8", errors="surrogateescape") as f:
+            return [l.rstrip("\n") for l in f]
 
     def _stream(self):
         """
         Returns a generator of lines instead of a list of lines.
         """
         if self._exception:
             raise self._exception
@@ -233,20 +268,16 @@
                 yield self._content
             else:
                 args = self.create_args()
                 if args:
                     with streams.connect(*args, env=SAFE_ENV) as s:
                         yield s
                 else:
-                    if six.PY3:
-                        with open(self.path, "r", encoding="utf-8", errors="surrogateescape") as f:
-                            yield f
-                    else:
-                        with codecs.open(self.path, "r", encoding="utf-8", errors="surrogateescape") as f:
-                            yield f
+                    with safe_open(self.path, "r", encoding="utf-8", errors="surrogateescape") as f:
+                        yield f
         except StopIteration:
             raise
         except Exception as ex:
             self._exception = ex
             raise ContentException(str(ex))
 
     def write(self, dst):
@@ -686,41 +717,67 @@
 
 class listdir(object):
     """
     Execute a simple directory listing of all the files and directories in
     path.
 
     Args:
-        path (str): directory or glob pattern to list.
+        path (str): directory to list.
         context (ExecutionContext): the context under which the datasource
             should run.
-        ignore (str): regular expression defining paths to ignore.
+        ignore (str): regular expression defining names to ignore.
 
     Returns:
-        function: A datasource that returns the list of files and directories
-            in the directory specified by path
+        function: A datasource that returns a sorted list of file and directory
+            names in the directory specified by path. The list will be empty when
+            the directory is empty or all names get ignored.
     """
 
     def __init__(self, path, context=None, ignore=None, deps=[]):
         self.path = path
         self.context = context or FSRoots
         self.ignore = ignore
         self.ignore_func = re.compile(ignore).search if ignore else lambda x: False
         self.__name__ = self.__class__.__name__
         datasource(self.context, *deps)(self)
 
     def __call__(self, broker):
         ctx = _get_context(self.context, broker)
         p = os.path.join(ctx.root, self.path.lstrip('/'))
         p = ctx.locate_path(p)
-        result = sorted(os.listdir(p)) if os.path.isdir(p) else sorted(glob(p))
+        try:
+            result = os.listdir(p)
+        except OSError as e:
+            raise ContentException(str(e))
+        return sorted([r for r in result if not self.ignore_func(r)])
 
-        if result:
-            return [os.path.basename(r) for r in result if not self.ignore_func(r)]
-        raise ContentException("Can't list %s or nothing there." % p)
+
+class listglob(listdir):
+    """
+    List paths matching a glob pattern.
+
+    Args:
+        pattern (str): glob pattern to list.
+        context (ExecutionContext): the context under which the datasource
+            should run.
+        ignore (str): regular expression defining paths to ignore.
+
+    Returns:
+        function: A datasource that returns the list of paths that match
+            the given glob pattern. The list will be empty when nothing matches.
+    """
+    def __call__(self, broker):
+        ctx = _get_context(self.context, broker)
+        p = os.path.join(ctx.root, self.path.lstrip('/'))
+        p = ctx.locate_path(p)
+        result = glob(p)
+        # generator expression; we don't need the full list at this step
+        result = (os.path.relpath(r, start=ctx.root) for r in result)
+        result = sorted([r for r in result if not self.ignore_func(r)])
+        return result
 
 
 class simple_command(object):
     """
     Execute a simple command that has no dynamic arguments
 
     Args:
@@ -1235,14 +1292,31 @@
 
 
 @deserializer(DatasourceProvider)
 def deserialize_datasource_provider(_type, data, root):
     return SerializedOutputProvider(data["relative_path"], root)
 
 
+@serializer(MetadataProvider)
+def serialize_metadata_provider(obj, root):
+    # Built-in metadata files are put in the root instead of '/data'
+    root = os.path.dirname(root) if os.path.basename(root) == 'data' else root
+    dst = os.path.join(root, obj.relative_path.lstrip("/"))
+    fs.ensure_path(os.path.dirname(dst))
+    obj.write(dst)
+    return {"relative_path": obj.relative_path}
+
+
+@deserializer(MetadataProvider)
+def deserialize_metadata_provider(_type, data, root):
+    # Built-in metadata files are put in the root instead of '/data'
+    root = os.path.dirname(root) if os.path.basename(root) == 'data' else root
+    return SerializedOutputProvider(data["relative_path"], root)
+
+
 @serializer(ContainerFileProvider)
 def serialize_container_file_output(obj, root):
     rel = os.path.join("insights_containers", obj.relative_path)
     dst = os.path.join(root, rel)
     rc = obj.write(dst)
     return {
         "relative_path": rel,
```

### Comparing `insights-core-3.1.9/insights/core/taglang.py` & `insights-core-3.2.0/insights/core/taglang.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/formats/__init__.py` & `insights-core-3.2.0/insights/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/formats/_json.py` & `insights-core-3.2.0/insights/formats/_json.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/formats/_markdown.py` & `insights-core-3.2.0/insights/formats/_markdown.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/formats/_syslog.py` & `insights-core-3.2.0/insights/formats/_syslog.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/formats/_yaml.py` & `insights-core-3.2.0/insights/formats/_yaml.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/formats/html.py` & `insights-core-3.2.0/insights/formats/html.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/formats/simple_html.py` & `insights-core-3.2.0/insights/formats/simple_html.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/formats/template.py` & `insights-core-3.2.0/insights/formats/template.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/formats/text.py` & `insights-core-3.2.0/insights/formats/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,20 +86,22 @@
         stream (file-like): Output is written to stream. Defaults to sys.stdout.
     """
     def __init__(self, broker,
             missing=False,
             tracebacks=False,
             dropped=False,
             show_rules=None,
+            no_details=False,
             stream=sys.stdout):
         super(HumanReadableFormat, self).__init__(broker, stream=stream)
         self.missing = missing
         self.tracebacks = tracebacks
         self.dropped = dropped
         self.show_rules = [] if show_rules is None else show_rules
+        self.no_details = no_details
 
     def print_header(self, header, color):
         ln = len(header)
         print(color + '-' * ln, file=self.stream)
         print(header, file=self.stream)
         print('-' * ln + Style.RESET_ALL, file=self.stream)
 
@@ -171,14 +173,16 @@
 
         def printit(c, v):
             resp = self.responses[v["type"]]
             name = "[%s] %s" % (resp.label, dr.get_name(c))
             underline = "-" * len(name)
             name = "%s%s%s" % (resp.color, name, Style.RESET_ALL)
             print(name, file=self.stream)
+            if self.no_details:
+                return
             print(underline, file=self.stream)
             if v.get('type') != 'none':
                 print(render_links(c), file=self.stream)
                 print(render(c, v), file=self.stream)
             print(file=self.stream)
 
         for c in sorted(self.broker.get_by_type(rule), key=dr.get_name):
@@ -226,19 +230,21 @@
         p.add_argument("-S", "--show-rules", default=[], nargs="+",
                        choices=["fail", "info", "pass", "none", "metadata", "fingerprint"],
                        metavar="TYPE",
                        help="Show results per rule's type: 'fail', 'info', 'pass', 'none', 'metadata', and 'fingerprint'")
         p.add_argument("-F", "--fail-only",
                        help="Show FAIL results only. Conflict with '-m', will be dropped when using them together. This option is deprecated by '-S fail'",
                        action="store_true")
+        p.add_argument("--no-details", help="Hide the details and show result only, for TEXT format only", action="store_true")
 
     def __init__(self, args=None):
         self.tracebacks = args.tracebacks
         self.dropped = args.dropped
         self.missing = args.missing
+        self.no_details = args.no_details
         fail_only = args.fail_only
         if self.missing and fail_only:
             print(Fore.YELLOW + 'Options conflict: -m and -F, drops -F', file=sys.stderr)
             fail_only = None
         self.show_rules = []  # Empty by default, means show ALL types (excludes "none")
         if not args.show_rules and fail_only:
             self.show_rules = ['rule']
@@ -248,12 +254,13 @@
     def preprocess(self, broker):
         self.formatter = HumanReadableFormat(
             broker,
             self.missing,
             self.tracebacks,
             self.dropped,
             self.show_rules,
+            self.no_details,
         )
         self.formatter.preprocess()
 
     def postprocess(self, broker):
         self.formatter.postprocess()
```

### Comparing `insights-core-3.1.9/insights/parsers/systemd/config.py` & `insights-core-3.2.0/insights/parsers/systemd/config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/systemd/unitfiles.py` & `insights-core-3.2.0/insights/parsers/systemd/unitfiles.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/__init__.py` & `insights-core-3.2.0/insights/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/abrt_ccpp.py` & `insights-core-3.2.0/insights/parsers/abrt_ccpp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/abrt_status_bare.py` & `insights-core-3.2.0/insights/parsers/abrt_status_bare.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/alternatives.py` & `insights-core-3.2.0/insights/parsers/alternatives.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/amq_broker.py` & `insights-core-3.2.0/insights/parsers/amq_broker.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/audit_log.py` & `insights-core-3.2.0/insights/parsers/audit_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/auditctl.py` & `insights-core-3.2.0/insights/parsers/auditctl.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/auditctl_status.py` & `insights-core-3.2.0/insights/parsers/lscpu.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,74 @@
 """
-AuditctlStatus - Report auditd status
-=====================================
-"""
+LsCPU - command ``lscpu``
+=========================
 
-from insights.core import CommandParser, LegacyItemAccess
-from insights.core.exceptions import ParseException
+This module provides the information about the CPU architecture using the output of the command ``lscpu``.
+"""
+from insights.core import CommandParser
+from insights.core.exceptions import SkipComponent
 from insights.core.plugins import parser
 from insights.specs import Specs
-from insights.util import deprecated
 
 
-@parser(Specs.auditctl_status)
-class AuditctlStatus(LegacyItemAccess, CommandParser):
-    """
-    .. warning::
-        This parser is deprecated, please use
-        :py:class:`insights.parsers.auditctl.AuditdStatus` instead.
-
-    Module for parsing the output of the ``auditctl -s`` command.
-
-    Typical output on RHEL6 looks like::
-
-        AUDIT_STATUS: enabled=1 flag=1 pid=1483 rate_limit=0 backlog_limit=8192 lost=3 backlog=0
-
-    , while on RHEL7 the output changes to::
-
-        enabled 1
-        failure 1
-        pid 947
-        rate_limit 0
-        backlog_limit 320
-        lost 0
-        backlog 0
-        loginuid_immutable 0 unlocked
-
-    Example:
-        >>> type(auds)
-        <class 'insights.parsers.auditctl_status.AuditctlStatus'>
-        >>> "enabled" in auds
-        True
-        >>> auds['enabled']
-        1
-    """
-    def __init__(self, context):
-        deprecated(
-            AuditctlStatus,
-            "Please use the :class:`insights.parsers.auditctl.AuditdStatus` instead.",
-            "3.1.25"
-        )
-        super(AuditctlStatus, self).__init__(context)
+@parser(Specs.lscpu)
+class LsCPU(CommandParser):
+    """Parse the output of ``/usr/bin/lscpu``. It uses the ``CommandParser`` as the
+    base class. The ``parse_content`` method also converts plural keys for
+    better accessibility.
+
+    Ex: "CPU(s)" is converted to "CPUs"
+
+    Typical output of ``lscpu`` command is::
+
+        Architecture:          x86_64
+        CPU op-mode(s):        32-bit, 64-bit
+        Byte Order:            Little Endian
+        CPU(s):                2
+        On-line CPU(s) list:   0,1
+        Thread(s) per core:    2
+        Core(s) per socket:    1
+        Socket(s):             1
+        NUMA node(s):          1
+        Vendor ID:             GenuineIntel
+        CPU family:            6
+        Model:                 60
+        Model name:            Intel Core Processor (Haswell, no TSX)
+        Stepping:              1
+        CPU MHz:               2793.530
+        BogoMIPS:              5587.06
+        Hypervisor vendor:     KVM
+        Virtualization type:   full
+        L1d cache:             32K
+        L1i cache:             32K
+        L2 cache:              4096K
+        NUMA node0 CPU(s):     0,1
+
+    Examples:
+
+        >>> output.info['Architecture']
+        'x86_64'
+        >>> len(output.info)
+        22
+        >>> output.info['CPUs']
+        '2'
+        >>> output.info['Threads per core']
+        '2'
+        >>> output.info['Cores per socket']
+        '1'
+        >>> output.info['Sockets']
+        '1'
 
+    """
     def parse_content(self, content):
         if not content:
-            raise ParseException("Input content is empty.")
-        self.data = {}
-        if len(content) > 1:
-            for line in content:
-                k, v = line.split(None, 1)
-                # Mind the 'loginuid_immutable' on RHEL7
-                if k.strip() == "loginuid_immutable":
-                    self.data[k.strip()] = v.strip()
-                else:
-                    try:
-                        self.data[k.strip()] = int(v.strip())
-                    except ValueError:
-                        continue
-        if len(content) == 1:
-            line = list(content)[0].strip()
-            if line.startswith("AUDIT_STATUS:"):
-                for item in line.split(None)[1:]:
-                    try:
-                        k, v = item.split('=')
-                        self.data[k.strip()] = int(v.strip())
-                    except ValueError:
-                        continue
+            raise SkipComponent("No data.")
+        self.info = {}
+        split_on = ":"
+        for line in content:
+            # On R9 they added indentation and section headers,
+            # so make sure the split len is 2 otherwise skip.
+            kv = line.split(split_on, 1)
+            if len(kv) != 2:
+                continue
+
+            self.info[kv[0].replace("(s)", "s").strip()] = kv[1].strip()
```

### Comparing `insights-core-3.1.9/insights/parsers/authselect.py` & `insights-core-3.2.0/insights/parsers/authselect.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/autofs_conf.py` & `insights-core-3.2.0/insights/parsers/autofs_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/avc_cache_threshold.py` & `insights-core-3.2.0/insights/parsers/avc_cache_threshold.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/avc_hash_stats.py` & `insights-core-3.2.0/insights/parsers/avc_hash_stats.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/awx_manage.py` & `insights-core-3.2.0/insights/parsers/awx_manage.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/azure_instance.py` & `insights-core-3.2.0/insights/parsers/azure_instance.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 ------------------------------------------
 
 AzureInstanceType - 'vmSize' of Azure Instance
 ----------------------------------------------
 
 AzureInstancePlan - 'plan' of Azure Instance
 --------------------------------------------
+
+AzurePublicIpv4Addresses - list of public IPv4 addresses
+--------------------------------------------------------
 """
 import json
 
 from insights.core import CommandParser
 from insights.core.exceptions import ParseException, SkipComponent
 from insights.core.plugins import parser
 from insights.specs import Specs
@@ -155,7 +158,45 @@
         self.product = plan["product"] if plan["product"] != "" else None
         self.publisher = plan["publisher"] if plan["publisher"] != "" else None
 
     def __repr__(self):
         return "<azure_plan_name: {n}, product: {pr}, publisher: {pu}, raw: {r}".format(
             n=self.name, pr=self.product, pu=self.publisher, r=self.raw
         )
+
+
+@parser(Specs.azure_load_balancer)
+class AzurePublicIpv4Addresses(CommandParser, list):
+    """
+    Class for parsing the Azure load balancer JSON data returned by command
+
+        curl -sH "Metadata:true" --connect-timeout 5 \
+            "http://169.254.169.254/metadata/loadbalancer?api-version=2021-12-13&format=json"
+
+    Typical Output of this command is::
+
+        {
+          "loadbalancer": {
+            "publicIpAddresses": [
+              {
+                "frontendIpAddress": "137.116.118.209",
+                "privateIpAddress": "10.0.0.4"
+              }
+            ],
+            "inboundRules": [],
+            "outboundRules": []
+          }
+        }
+
+    Raises:
+        SkipComponent: When content is empty or curl returned an error.
+        ParseException: On JSON parsing error.
+    """
+    def parse_content(self, content):
+        validate_content(content)
+
+        try:
+            plan = json.loads(' '.join(content))
+            for pair in plan["loadbalancer"]["publicIpAddresses"]:
+                self.append(pair["frontendIpAddress"])
+        except:
+            raise ParseException("Unable to parse JSON")
```

### Comparing `insights-core-3.1.9/insights/parsers/azure_instance_plan.py` & `insights-core-3.2.0/insights/parsers/azure_instance_plan.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/azure_instance_type.py` & `insights-core-3.2.0/insights/parsers/azure_instance_type.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/bdi_read_ahead_kb.py` & `insights-core-3.2.0/insights/parsers/bdi_read_ahead_kb.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/blkid.py` & `insights-core-3.2.0/insights/parsers/blkid.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/bond.py` & `insights-core-3.2.0/insights/parsers/bond.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/bond_dynamic_lb.py` & `insights-core-3.2.0/insights/parsers/bond_dynamic_lb.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/brctl_show.py` & `insights-core-3.2.0/insights/parsers/brctl_show.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/candlepin_broker.py` & `insights-core-3.2.0/insights/parsers/candlepin_broker.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/catalina_log.py` & `insights-core-3.2.0/insights/parsers/catalina_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cciss.py` & `insights-core-3.2.0/insights/parsers/cciss.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ceilometer_conf.py` & `insights-core-3.2.0/insights/parsers/ceilometer_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ceilometer_log.py` & `insights-core-3.2.0/insights/parsers/ceilometer_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ceph_cmd_json_parsing.py` & `insights-core-3.2.0/insights/parsers/ceph_cmd_json_parsing.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ceph_conf.py` & `insights-core-3.2.0/insights/parsers/ceph_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ceph_insights.py` & `insights-core-3.2.0/insights/parsers/ceph_insights.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ceph_log.py` & `insights-core-3.2.0/insights/parsers/ceph_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ceph_osd_log.py` & `insights-core-3.2.0/insights/parsers/ceph_osd_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ceph_osd_tree_text.py` & `insights-core-3.2.0/insights/parsers/ceph_osd_tree_text.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ceph_version.py` & `insights-core-3.2.0/insights/parsers/ceph_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/certificates_enddate.py` & `insights-core-3.2.0/insights/parsers/certificates_enddate.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cgroups.py` & `insights-core-3.2.0/insights/parsers/cgroups.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/checkin_conf.py` & `insights-core-3.2.0/insights/parsers/checkin_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/chkconfig.py` & `insights-core-3.2.0/insights/parsers/chkconfig.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cib.py` & `insights-core-3.2.0/insights/parsers/cib.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cinder_conf.py` & `insights-core-3.2.0/insights/parsers/cinder_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cinder_log.py` & `insights-core-3.2.0/insights/parsers/cinder_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cloud_cfg.py` & `insights-core-3.2.0/insights/parsers/cloud_cfg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cloud_init_custom_network.py` & `insights-core-3.2.0/insights/parsers/cloud_init_custom_network.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cloud_init_log.py` & `insights-core-3.2.0/insights/parsers/cloud_init_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cluster_conf.py` & `insights-core-3.2.0/insights/parsers/cluster_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cmdline.py` & `insights-core-3.2.0/insights/parsers/cmdline.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cni_podman_bridge_conf.py` & `insights-core-3.2.0/insights/parsers/cni_podman_bridge_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cobbler_modules_conf.py` & `insights-core-3.2.0/insights/parsers/cobbler_modules_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cobbler_settings.py` & `insights-core-3.2.0/insights/parsers/cobbler_settings.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/config_file_perms.py` & `insights-core-3.2.0/insights/parsers/config_file_perms.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/containers_inspect.py` & `insights-core-3.2.0/insights/parsers/containers_inspect.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/containers_policy.py` & `insights-core-3.2.0/insights/parsers/containers_policy.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/corosync.py` & `insights-core-3.2.0/insights/parsers/corosync.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/corosync_cmapctl.py` & `insights-core-3.2.0/insights/parsers/corosync_cmapctl.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cpu_online.py` & `insights-core-3.2.0/insights/parsers/cpu_online.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cpu_vulns.py` & `insights-core-3.2.0/insights/parsers/cpu_vulns.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cpuinfo.py` & `insights-core-3.2.0/insights/parsers/cpuinfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,17 +64,18 @@
     >>> cpu_info.get_processor_by_index(0)['cpus']
     '0'
     >>> cpu_info.get_processor_by_index(0)['vendors']
     'GenuineIntel'
     >>> cpu_info.microcode
     '1808'
 """
+import warnings
 
 from collections import defaultdict
-from .. import Parser, parser, defaults, get_active_lines, LegacyItemAccess
+from insights import Parser, parser, defaults, get_active_lines, LegacyItemAccess
 from insights.specs import Specs
 
 
 @parser(Specs.cpuinfo)
 class CpuInfo(LegacyItemAccess, Parser):
     """
     CpuInfo parser - able to be used as a dictionary through the
@@ -265,18 +266,19 @@
     @property
     @defaults()
     def core_total(self):
         """
         int: Returns the total number of cores for the server if available, else None.
 
         .. warning::
-            This function is deprecated.  Please use the
+            This method is deprecated, and will be removed after 3.2.25. Please use
             :py:class:`insights.parsers.lscpu.LsCPU` class attribute
             ``info['Cores per socket']`` and ``info['Sockets']`` values instead.
         """
+        warnings.warn("`is_hypervisor` is deprecated and will be removed after 3.2.25: Use `virt_what.VirtWhat` which uses the command `virt-what` to check the hypervisor type.", DeprecationWarning)
         if self.data and 'cpu_cores' in self.data:
             # I guess we can't get this fancey on older versions of RHEL
             # return sum({e['sockets']: int(e['cpu_cores']) for e in self}.values())
             physical_dict = {}
             for e in self:
                 # we should rename sockets here to physical_ids as cpuinfo
                 # has it there can be many physical_ids per socket
```

### Comparing `insights-core-3.1.9/insights/parsers/cpupower_frequency_info.py` & `insights-core-3.2.0/insights/parsers/cpupower_frequency_info.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cpuset_cpus.py` & `insights-core-3.2.0/insights/parsers/cpuset_cpus.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/crictl_logs.py` & `insights-core-3.2.0/insights/parsers/crictl_logs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/crio_conf.py` & `insights-core-3.2.0/insights/parsers/crio_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cron_daily_rhsmd.py` & `insights-core-3.2.0/insights/parsers/cron_daily_rhsmd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cron_jobs.py` & `insights-core-3.2.0/insights/parsers/cron_jobs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/crontab.py` & `insights-core-3.2.0/insights/parsers/crontab.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/crypto_policies.py` & `insights-core-3.2.0/insights/parsers/crypto_policies.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cryptsetup_luksDump.py` & `insights-core-3.2.0/insights/parsers/cryptsetup_luksDump.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/cups_ppd.py` & `insights-core-3.2.0/insights/parsers/cups_ppd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/current_clocksource.py` & `insights-core-3.2.0/insights/parsers/current_clocksource.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/date.py` & `insights-core-3.2.0/insights/parsers/date.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/db2.py` & `insights-core-3.2.0/insights/parsers/db2.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dcbtool_gc_dcb.py` & `insights-core-3.2.0/insights/parsers/dcbtool_gc_dcb.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/designate_conf.py` & `insights-core-3.2.0/insights/parsers/designate_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/df.py` & `insights-core-3.2.0/insights/parsers/df.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dig.py` & `insights-core-3.2.0/insights/parsers/dig.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dirsrv_logs.py` & `insights-core-3.2.0/insights/parsers/dirsrv_logs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dmesg.py` & `insights-core-3.2.0/insights/parsers/dmesg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dmesg_log.py` & `insights-core-3.2.0/insights/parsers/dmesg_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dmidecode.py` & `insights-core-3.2.0/insights/parsers/dmidecode.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dmsetup.py` & `insights-core-3.2.0/insights/parsers/dmsetup.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dnf_conf.py` & `insights-core-3.2.0/insights/parsers/dnf_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dnf_modules.py` & `insights-core-3.2.0/insights/parsers/dnf_modules.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dnsmasq_config.py` & `insights-core-3.2.0/insights/parsers/dnsmasq_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/docker_host_machine_id.py` & `insights-core-3.2.0/insights/parsers/docker_host_machine_id.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/docker_inspect.py` & `insights-core-3.2.0/insights/parsers/docker_inspect.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/docker_list.py` & `insights-core-3.2.0/insights/parsers/docker_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dockerinfo.py` & `insights-core-3.2.0/insights/parsers/dockerinfo.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dotnet.py` & `insights-core-3.2.0/insights/parsers/dotnet.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/doveconf.py` & `insights-core-3.2.0/insights/parsers/doveconf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dracut_modules.py` & `insights-core-3.2.0/insights/parsers/dracut_modules.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dse_ldif_simple.py` & `insights-core-3.2.0/insights/parsers/dse_ldif_simple.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/du.py` & `insights-core-3.2.0/insights/parsers/du.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/dumpe2fs_h.py` & `insights-core-3.2.0/insights/parsers/dumpe2fs_h.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/engine_config.py` & `insights-core-3.2.0/insights/parsers/engine_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/engine_db_query.py` & `insights-core-3.2.0/insights/parsers/engine_db_query.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/engine_log.py` & `insights-core-3.2.0/insights/parsers/engine_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/etcd_conf.py` & `insights-core-3.2.0/insights/parsers/etcd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ethtool.py` & `insights-core-3.2.0/insights/parsers/ethtool.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/facter.py` & `insights-core-3.2.0/insights/parsers/facter.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/fapolicyd_rules.py` & `insights-core-3.2.0/insights/parsers/fapolicyd_rules.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/fc_match.py` & `insights-core-3.2.0/insights/parsers/fc_match.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/fcoeadm_i.py` & `insights-core-3.2.0/insights/parsers/fcoeadm_i.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/findmnt.py` & `insights-core-3.2.0/insights/parsers/findmnt.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/firewall_cmd.py` & `insights-core-3.2.0/insights/parsers/firewall_cmd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/firewall_config.py` & `insights-core-3.2.0/insights/parsers/firewall_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/foreman_log.py` & `insights-core-3.2.0/insights/parsers/foreman_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/foreman_proxy_conf.py` & `insights-core-3.2.0/insights/parsers/foreman_proxy_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/foreman_rake_db_migrate_status.py` & `insights-core-3.2.0/insights/parsers/foreman_rake_db_migrate_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/freeipa_healthcheck_log.py` & `insights-core-3.2.0/insights/parsers/freeipa_healthcheck_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/fstab.py` & `insights-core-3.2.0/insights/parsers/fstab.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,31 +119,29 @@
         for row in self.data:
             yield row
 
     def parse_content(self, content):
         """
         Parse each line in the file ``/etc/fstab``.
         """
-        fstab_output = parse_delimited_table([FS_HEADINGS] + get_active_lines(content))
+        fstab_output = parse_delimited_table([FS_HEADINGS] + get_active_lines(content), raw_line_key='raw')
         self.data = []
         for line in fstab_output:
             line['fs_spec'] = line.get('fs_spec', '')
             line['fs_vfstype'] = line.get('fs_vfstype', '')
             # Decode fs_file to transfer the '\040' to ' '.
             # Encode first and then decode works for both Python2 and Python3.
             line['fs_file'] = line.get('fs_file', '').encode().decode("unicode-escape")
             line['fs_freq'] = int(line.get('fs_freq', '0'))
             line['fs_passno'] = int(line.get('fs_passno', '0'))
             # if there is no mntops, it is defaults.
             # (/dev/foo /foo somefs defaults   0 0) and (/dev/foo /foo somefs) are same
             line['raw_fs_mntops'] = line.get('raw_fs_mntops', 'defaults')
             # optlist_to_dict converts 'key=value' to key: value and 'key' to key: True
             line['fs_mntops'] = MountOpts(optlist_to_dict(line.get('raw_fs_mntops')))
-            # add `raw` here for displaying convenience on front-end
-            line['raw'] = [l for l in content if l.strip().startswith(line['fs_spec'])][0]
             self.data.append(FSTabEntry(line))
         # assert: all mount points of valid entries are unique by definition
         self.mounted_on = dict((row.fs_file, row) for row in self.data)
 
     def search(self, **kwargs):
         """
         Search for the given key/value pairs in the data.  Please refer to the
```

### Comparing `insights-core-3.1.9/insights/parsers/fwupdagent.py` & `insights-core-3.2.0/insights/parsers/fwupdagent.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/galera_cnf.py` & `insights-core-3.2.0/insights/parsers/galera_cnf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/gcp_instance_type.py` & `insights-core-3.2.0/insights/parsers/gcp_instance_type.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/gcp_license_codes.py` & `insights-core-3.2.0/insights/parsers/gcp_license_codes.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/getcert_list.py` & `insights-core-3.2.0/insights/parsers/getcert_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/getconf_pagesize.py` & `insights-core-3.2.0/insights/parsers/getconf_pagesize.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/getenforce.py` & `insights-core-3.2.0/insights/parsers/getenforce.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/getsebool.py` & `insights-core-3.2.0/insights/parsers/getsebool.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/gfs2_file_system_block_size.py` & `insights-core-3.2.0/insights/parsers/gfs2_file_system_block_size.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/glance_log.py` & `insights-core-3.2.0/insights/parsers/glance_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/gluster_peer_status.py` & `insights-core-3.2.0/insights/parsers/gluster_peer_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,14 @@
     """
     def _grouper(self, iterable, n, fillvalue=None):
         "Collect data into fixed-length chunks or blocks"
         args = [iter(iterable)] * n
         return zip_longest(*args, fillvalue=fillvalue)
 
     def parse_content(self, content):
-        if not content:
+        if not content or "Connection failed" in content[0]:
             raise SkipComponent("No data.")
 
         self.status = {'peers': 0, 'hosts': []}
         self.status['peers'] = int(content[0].split(':')[-1].strip())
         for group in list(self._grouper(list(filter(lambda x: x != '', content[2:])), 3)):
             self.status['hosts'].append(split_kv_pairs(group, split_on=':'))
```

### Comparing `insights-core-3.1.9/insights/parsers/gluster_vol.py` & `insights-core-3.2.0/insights/parsers/gluster_vol.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/gnocchi.py` & `insights-core-3.2.0/insights/parsers/gnocchi.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/greenboot_status.py` & `insights-core-3.2.0/insights/parsers/greenboot_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/grub_conf.py` & `insights-core-3.2.0/insights/parsers/grub_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/grubby.py` & `insights-core-3.2.0/insights/parsers/grubby.py`

 * *Files 12% similar despite different names*

```diff
@@ -65,10 +65,29 @@
 
     Attributes:
         default_kernel(str): The default kernel name for next boot
     """
     def parse_content(self, content):
         if not content:
             raise SkipComponent('Empty output')
-        if len(content) != 1 or len(content[0].split()) > 1:
-            raise ParseException('Invalid output: {0}', content)
-        self.default_kernel = content[0].strip()
+
+        # Skip the error lines to find the real default-kernel line.
+        # Typically, the default-kernel line is the last line in content.
+        default_kernel_str = None
+
+        if len(content) == 1:
+            default_kernel_str = content[0].strip()
+        else:
+            for idx in range(len(content) - 1, -1, -1):
+                line = content[idx]
+                if line.startswith('/boot/') and '/boot/vmlinuz-' in line:
+                    if not default_kernel_str:
+                        default_kernel_str = line.strip()
+                    else:
+                        raise ParseException('Invalid output: duplicate kernel lines: {0}', content)
+
+        if not default_kernel_str:
+            raise ParseException('Invalid output: no kernel line: {0}', content)
+        if len(default_kernel_str.split()) > 1:
+            raise ParseException('Invalid output: unparsable kernel line: {0}', content)
+
+        self.default_kernel = default_kernel_str
```

### Comparing `insights-core-3.1.9/insights/parsers/grubenv.py` & `insights-core-3.2.0/insights/parsers/grubenv.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/hammer_ping.py` & `insights-core-3.2.0/insights/parsers/hammer_ping.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/hammer_task_list.py` & `insights-core-3.2.0/insights/parsers/hammer_task_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/haproxy_cfg.py` & `insights-core-3.2.0/insights/parsers/haproxy_cfg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/heat_conf.py` & `insights-core-3.2.0/insights/parsers/heat_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/heat_log.py` & `insights-core-3.2.0/insights/parsers/heat_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/host_vdsm_id.py` & `insights-core-3.2.0/insights/parsers/host_vdsm_id.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/hostname.py` & `insights-core-3.2.0/insights/parsers/hostname.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/hosts.py` & `insights-core-3.2.0/insights/parsers/hosts.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/hponcfg.py` & `insights-core-3.2.0/insights/parsers/hponcfg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/httpd_M.py` & `insights-core-3.2.0/insights/parsers/httpd_M.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/httpd_V.py` & `insights-core-3.2.0/insights/parsers/httpd_V.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/httpd_conf.py` & `insights-core-3.2.0/insights/parsers/httpd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/httpd_log.py` & `insights-core-3.2.0/insights/parsers/httpd_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/httpd_open_nfs.py` & `insights-core-3.2.0/insights/parsers/httpd_open_nfs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ibm_proc.py` & `insights-core-3.2.0/insights/parsers/ibm_proc.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ifcfg.py` & `insights-core-3.2.0/insights/parsers/ifcfg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/imagemagick_policy.py` & `insights-core-3.2.0/insights/parsers/imagemagick_policy.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/init_process_cgroup.py` & `insights-core-3.2.0/insights/parsers/init_process_cgroup.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/initscript.py` & `insights-core-3.2.0/insights/parsers/initscript.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/insights_client_conf.py` & `insights-core-3.2.0/insights/parsers/insights_client_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/installed_product_ids.py` & `insights-core-3.2.0/insights/parsers/installed_product_ids.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/installed_rpms.py` & `insights-core-3.2.0/insights/parsers/installed_rpms.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 
 InstalledRpms - command ``rpm -qa``
 -----------------------------------
 ContainerInstalledRpms - command ``rpm -qa`` for containers
 -----------------------------------------------------------
 """
 
-from collections import defaultdict
 import json
 import re
 import six
 import warnings
 
+from collections import defaultdict
+
 from insights import ContainerParser, parser, CommandParser
 from insights.core.exceptions import SkipComponent
 from insights.parsers.rpm_vercmp import rpm_version_compare
 from insights.specs import Specs
 from insights.util import rsplit
 
 
@@ -141,20 +142,20 @@
         else:
             return min(self.packages[package_name])
 
     @property
     def is_hypervisor(self):
         """
         .. warning::
-           This method is deprecated, please use
+           This method is deprecated, and will be removed after 3.2.25. Please use
            :py:class:`insights.parsers.virt_what.VirtWhat` which uses the command `virt-what` to check the hypervisor type.
 
         bool: True if ".el[6|7]ev" exists in "vdsm".release, else False.
         """
-        warnings.warn("`is_hypervisor` is deprecated: Use `virt_what.VirtWhat` which uses the command `virt-what` to check the hypervisor type.", DeprecationWarning)
+        warnings.warn("`is_hypervisor` is deprecated and will be removed after 3.2.25: Use `virt_what.VirtWhat` which uses the command `virt-what` to check the hypervisor type.", DeprecationWarning)
         rpm = self.get_max("vdsm")
         return (True if rpm and rpm.release.endswith((".el6ev", ".el7ev")) else
                 False)
 
     # re-export get_max/min with more descriptive names
     newest = get_max
     oldest = get_min
@@ -248,31 +249,29 @@
 
                 >>> if rpms.packages and "pkg_name" not in rpms.packages:
                 >>>     pass
         """
         super(InstalledRpms, self).__init__(*args, **kwargs)
 
     def parse_content(self, content):
-        packages = defaultdict(list)
         if content and (not content[0].strip() or "COMMAND>" in content[0]):
             content = content[1:]
         if not content:
             raise SkipComponent("The content of rpm command is empty!")
-        if content and '"name":' in content[0]:
-            rpm_init_method = InstalledRpm.from_json
-        else:
-            rpm_init_method = InstalledRpm.from_line
+        parse_func = InstalledRpm.from_json if any(
+                '"name":' in _l for _l in content) else InstalledRpm.from_line
+        packages = defaultdict(list)
         for line in content:
             if not line.strip():
                 continue
             if line.startswith('error:') or line.startswith('warning:'):
                 self.errors.append(line)
             else:
                 try:
-                    rpm = rpm_init_method(line)
+                    rpm = parse_func(line)
                     packages[rpm.name].append(rpm)
                 except Exception:
                     self.unparsed.append(line)
         self.packages = dict(packages)
 
     @property
     def corrupt(self):
@@ -369,23 +368,32 @@
              '1410968065' '\t'
              'Red Hat, Inc.' '\t'
              'hs20-bc2-4.build.redhat.com' '\t'
              '8902150305004...b3576ff37da7e12e2285358267495ac48a437d4eefb3213' '\t'
              'RSA/8, Mon Aug 16 11:14:17 2010, Key ID 199e2f91fd431d51')
     """
     PRODUCT_SIGNING_KEYS = [
-        'F76F66C3D4082792', '199e2f91fd431d51', '5326810137017186',
+        # NOTE: All In lower cases
+        # RELEASE PACKAGE SIGNING
+        '199e2f91fd431d51', '1ac4971355a34a82', '5054e4a45a6340b3',
+        'e1a4bd708a828aad', 'f76f66c3d4082792', '5326810137017186',
         '45689c882fa658e0', '219180cddb42a60e', '7514f77d8366b0d9',
-        'fd372689897da07a', '938a80caf21541eb',
-        '08b871e6a5787476', '1AC4971355A34A82'
-        'E191DDB2C509E861'
+        '08dd962c1c711042',
+        # BETA PACKAGE SIGNING
+        'fd372689897da07a', '938a80caf21541eb'
+        # DEVELOPMENT PACKAGE SIGNING
+        '08b871e6a5787476',
+        # OTHER PRODUCTS
+        'e191ddb2c509e861',
+        # CERTIFICATES
+        '66e8f8a29c65f85c', '680b9144769a9f8f', '8ed29db42a2898c8'
     ]
     """
-    list: List of package-signing keys. Should be updated timely according to
-          https://access.redhat.com/security/team/key/
+    list: List of package-signing keys in all lower cases. Should be updated
+          timely according to https://access.redhat.com/security/team/key/
     """
     SOSREPORT_KEYS = [
         'installtime', 'buildtime', 'vendor', 'buildserver', 'pgpsig', 'pgpsig_short'
     ]
     """list: List of keys for SOS Report RPM information."""
 
     def __init__(self, data):
@@ -408,15 +416,16 @@
 
         for k, v in data.items():
             setattr(self, k, v)
         self.epoch = data['epoch'] if 'epoch' in data and data['epoch'] != '(none)' else '0'
         self.vendor = data['vendor'] if 'vendor' in data else None
         _gpg_key_pos = data.get('sigpgp', data.get('rsaheader', data.get('pgpsig_short', data.get('pgpsig', data.get('vendor', '')))))
         if _gpg_key_pos:
-            self.redhat_signed = any(key in _gpg_key_pos for key in self.PRODUCT_SIGNING_KEYS)
+            self.redhat_signed = any(key in _gpg_key_pos.lower()
+                                     for key in self.PRODUCT_SIGNING_KEYS)
 
     @classmethod
     def from_package(cls, package_string):
         """
         The object of this class is usually created from dictionary. Alternatively it can be
         created from package string.
```

### Comparing `insights-core-3.1.9/insights/parsers/interrupts.py` & `insights-core-3.2.0/insights/parsers/interrupts.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ip.py` & `insights-core-3.2.0/insights/parsers/ip.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,18 +77,20 @@
             split_content = line.split()
             current['openvswitch'] = split_content
         elif 'geneve' in line:
             split_content = line.split()
             current['geneve'] = split_content
         elif line.startswith("inet"):
             parse_inet(line, current)
-        elif line.startswith("RX"):
+        elif line.startswith("RX") and current and "rx_bytes" not in current:
             rx_next_line = True
-        elif line.startswith("TX"):
+        elif line.startswith("TX") and current and "tx_bytes" not in current:
             tx_next_line = True
+        elif line.startswith("vf "):
+            current['vf_enabled'] = True
     for k, v in r.items():
         if_details[k] = NetworkInterface(v)
     return if_details
 
 
 def parse_interface(line):
     split_content = line.split()
@@ -98,19 +100,20 @@
         name, physical_name = name.split("@")
     current = {
         "index": int(idx),
         "name": name.strip(),
         "physical_name": physical_name if virtual else None,
         "virtual": virtual,
         "flags": split_content[2].strip("<>").split(","),
-        "addr": []
+        "addr": [],
+        "vf_enabled": False
     }
     # extract properties
-    for i in range(3, len(split_content), 2):
-        key, value = (split_content[i], split_content[i + 1])
+    for i in range(4, len(split_content), 2):
+        key, value = (split_content[i - 1], split_content[i])
         current[key] = int(value) if key in ["mtu", "qlen"] else value
     return current
 
 
 def parse_link(line, d):
     split_content = line.split()
     d["type"] = split_content[0].split("/")[1]
```

### Comparing `insights-core-3.1.9/insights/parsers/ip_netns_exec_namespace_lsof.py` & `insights-core-3.2.0/insights/parsers/ip_netns_exec_namespace_lsof.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ipaupgrade_log.py` & `insights-core-3.2.0/insights/parsers/ipaupgrade_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ipcs.py` & `insights-core-3.2.0/insights/parsers/ipcs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ipsec_conf.py` & `insights-core-3.2.0/insights/parsers/ipsec_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/iptables.py` & `insights-core-3.2.0/insights/parsers/iptables.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ironic_conf.py` & `insights-core-3.2.0/insights/parsers/ironic_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ironic_inspector_log.py` & `insights-core-3.2.0/insights/parsers/ironic_inspector_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/iscsiadm_mode_session.py` & `insights-core-3.2.0/insights/parsers/iscsiadm_mode_session.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/jboss_domain_log.py` & `insights-core-3.2.0/insights/parsers/jboss_domain_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/jboss_standalone_main_conf.py` & `insights-core-3.2.0/insights/parsers/jboss_standalone_main_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/jboss_version.py` & `insights-core-3.2.0/insights/parsers/jboss_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/journal_all.py` & `insights-core-3.2.0/insights/parsers/messages.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,43 @@
 """
-JournalAll file ``/sos_commands/logs/journalctl_--no-pager``
-============================================================
+Messages file ``/var/log/messages``
+===================================
 """
 
 from .. import Syslog, parser
 from insights.specs import Specs
-from insights.util import deprecated
 
 
-@parser(Specs.journal_all)
-class JournalAll(Syslog):
+@parser(Specs.messages)
+class Messages(Syslog):
     """
+    Read the ``/var/log/messages`` file.
 
-    .. warning::
-
-        This parser is deprecated, please use
-        :py:class:`insights.parsers.journalctl.JournalAll` instead.
-
-
-    Read the ``/sos_commands/logs/journalctl_--no-pager`` file.  Uses the
-    ``Syslog`` class parser functionality - see the base class for more details.
+    .. note::
+        Please refer to its super-class :class:`insights.core.Syslog` for more
+        details.
 
     Sample log lines::
 
-        -- Logs begin at Wed 2017-02-08 15:18:00 CET, end at Tue 2017-09-19 09:25:27 CEST. --
         May 18 15:13:34 lxc-rhel68-sat56 jabberd/sm[11057]: session started: jid=rhn-dispatcher-sat@lxc-rhel6-sat56.redhat.com/superclient
         May 18 15:13:36 lxc-rhel68-sat56 wrapper[11375]: --> Wrapper Started as Daemon
         May 18 15:13:36 lxc-rhel68-sat56 wrapper[11375]: Launching a JVM...
         May 18 15:24:28 lxc-rhel68-sat56 yum[11597]: Installed: lynx-2.8.6-27.el6.x86_64
         May 18 15:36:19 lxc-rhel68-sat56 yum[11954]: Updated: sos-3.2-40.el6.noarch
 
     .. note::
-        Because journal timestamps by default have no year,
+        Because /var/log/messages timestamps by default have no year,
         the year of the logs will be inferred from the year in your timestamp.
         This will also work around December/January crossovers.
 
     Examples:
-        >>> JournalAll.filters.append('wrapper')
-        >>> JournalAll.token_scan('daemon_start', 'Wrapper Started as Daemon')
-        >>> msgs = shared[JournalAll]
+        >>> Messages.token_scan('daemon_start', 'Wrapper Started as Daemon')
+        >>> type(msgs)
+        <class 'insights.parsers.messages.Messages'>
         >>> len(msgs.lines)
+        9
         >>> wrapper_msgs = msgs.get('wrapper') # Can only rely on lines filtered being present
-        >>> wrapper_msgs[0]
-        {'timestamp': 'May 18 15:13:36', 'hostname': 'lxc-rhel68-sat56',
-         'procname': wrapper[11375]', 'message': '--> Wrapper Started as Daemon',
-         'raw_message': 'May 18 15:13:36 lxc-rhel68-sat56 wrapper[11375]: --> Wrapper Started as Daemon'
-        }
-        >>> msgs.daemon_start # Token set if matching lines present in logs
+        >>> result = {'raw_message': 'May 18 15:13:36 lxc-rhel68-sat56 wrapper[11375]: --> Wrapper Started as Daemon', 'message': '--> Wrapper Started as Daemon', 'timestamp': 'May 18 15:13:36', 'hostname': 'lxc-rhel68-sat56', 'procname': 'wrapper[11375]'}
+        >>> wrapper_msgs[0] == result
         True
     """
-
-    def __init__(self, context):
-        deprecated(
-            JournalAll,
-            "Please use the :class:`insights.parsers.journalctl.JournalAll` instead.",
-            "3.1.25"
-        )
-        super(JournalAll, self).__init__(context)
-
     pass
```

### Comparing `insights-core-3.1.9/insights/parsers/journal_since_boot.py` & `insights-core-3.2.0/insights/tests/parsers/test_messages.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,51 @@
-"""
-JournalSinceBoot file ``/sos_commands/logs/journalctl_--no-pager_--boot``
-=========================================================================
-"""
+import doctest
 
-from .. import Syslog, parser
+from insights import add_filter
+from insights.parsers import messages
 from insights.specs import Specs
-from insights.util import deprecated
+from insights.tests import context_wrap
 
-
-@parser(Specs.journal_since_boot)
-class JournalSinceBoot(Syslog):
-    """
-
-    .. warning::
-
-        This parser is deprecated, please use
-        :py:class:`insights.parsers.journalctl.JournalSinceBoot` instead.
-
-
-    Read the ``/sos_commands/logs/journalctl_--no-pager_--boot`` file.  Uses
-    the ``Syslog`` class parser functionality - see the base class for more
-    details.
-
-    Sample log lines::
-
-        -- Logs begin at Wed 2017-02-08 15:18:00 CET, end at Tue 2017-09-19 09:25:27 CEST. --
-        May 18 15:13:34 lxc-rhel68-sat56 jabberd/sm[11057]: session started: jid=rhn-dispatcher-sat@lxc-rhel6-sat56.redhat.com/superclient
-        May 18 15:13:36 lxc-rhel68-sat56 wrapper[11375]: --> Wrapper Started as Daemon
-        May 18 15:13:36 lxc-rhel68-sat56 wrapper[11375]: Launching a JVM...
-        May 18 15:24:28 lxc-rhel68-sat56 yum[11597]: Installed: lynx-2.8.6-27.el6.x86_64
-        May 18 15:36:19 lxc-rhel68-sat56 yum[11954]: Updated: sos-3.2-40.el6.noarch
-
-    Note:
-        Because journal timestamps by default have no year,
-        the year of the logs will be inferred from the year in your timestamp.
-        This will also work around December/January crossovers.
-
-    Examples:
-        >>> JournalSinceBoot.filters.append('wrapper')
-        >>> JournalSinceBoot.token_scan('daemon_start', 'Wrapper Started as Daemon')
-        >>> msgs = shared[JournalSinceBoot]
-        >>> len(msgs.lines)
-        >>> wrapper_msgs = msgs.get('wrapper') # Can only rely on lines filtered being present
-        >>> wrapper_msgs[0]
-        {'timestamp': 'May 18 15:13:36', 'hostname': 'lxc-rhel68-sat56',
-         'procname': wrapper[11375]', 'message': '--> Wrapper Started as Daemon',
-         'raw_message': 'May 18 15:13:36 lxc-rhel68-sat56 wrapper[11375]: --> Wrapper Started as Daemon'
-        }
-        >>> msgs.daemon_start # Token set if matching lines present in logs
-        True
-    """
-
-    def __init__(self, context):
-        deprecated(
-            JournalSinceBoot,
-            "Please use the :class:`insights.parsers.journalctl.JournalSinceBoot` instead.",
-            "3.1.25"
-        )
-        super(JournalSinceBoot, self).__init__(context)
-
-    pass
+MSGINFO = """
+May 18 15:13:34 lxc-rhel68-sat56 jabberd/sm[11057]: session started: jid=rhn-dispatcher-sat@lxc-rhel6-sat56.redhat.com/superclient
+May 18 15:13:36 lxc-rhel68-sat56 wrapper[11375]: --> Wrapper Started as Daemon
+May 18 15:13:36 lxc-rhel68-sat56 wrapper[11375]: Launching a JVM...
+May 18 15:24:28 lxc-rhel68-sat56 yum[11597]: Installed: lynx-2.8.6-27.el6.x86_64
+May 18 15:36:19 lxc-rhel68-sat56 yum[11954]: Updated: sos-3.2-40.el6.noarch
+Apr 22 10:35:01 boy-bona CROND[27921]: (root) CMD (/usr/lib64/sa/sa1 -S DISK 1 1)
+Apr 22 10:37:32 boy-bona crontab[28951]: (root) LIST (root)
+Apr 22 10:40:01 boy-bona CROND[30677]: (root) CMD (/usr/lib64/sa/sa1 -S DISK 1 1)
+Apr 22 10:41:13 boy-bona crontab[32515]: (root) LIST (root)
+""".strip()
+
+add_filter(Specs.messages, [
+    "LIST",
+    "CROND",
+    "jabberd",
+    "Wrapper",
+    "Launching",
+    "yum"
+])
+
+
+def test_doc_examples():
+    env = {
+        'msgs': messages.Messages(context_wrap(MSGINFO)),
+        'Messages': messages.Messages
+    }
+    failed, total = doctest.testmod(messages, globs=env)
+    assert failed == 0
+
+
+def test_messages():
+    msg_info = messages.Messages(context_wrap(MSGINFO))
+    bona_list = msg_info.get('(root) LIST (root)')
+    assert 2 == len(bona_list)
+    assert bona_list[0].get('timestamp') == "Apr 22 10:37:32"
+    assert bona_list[1].get('timestamp') == "Apr 22 10:41:13"
+    crond = msg_info.get('CROND')
+    assert 2 == len(crond)
+    assert crond[0].get('procname') == "CROND[27921]"
+    assert msg_info.get('jabberd/sm[11057]')[0].get('hostname') == "lxc-rhel68-sat56"
+    assert msg_info.get('Wrapper')[0].get('message') == "--> Wrapper Started as Daemon"
+    assert msg_info.get('Launching')[0].get('raw_message') == "May 18 15:13:36 lxc-rhel68-sat56 wrapper[11375]: Launching a JVM..."
+    assert 2 == len(msg_info.get('yum'))
```

### Comparing `insights-core-3.1.9/insights/parsers/journalctl.py` & `insights-core-3.2.0/insights/parsers/journalctl.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/journald_conf.py` & `insights-core-3.2.0/insights/parsers/journald_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/katello_service_status.py` & `insights-core-3.2.0/insights/parsers/katello_service_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/kdump.py` & `insights-core-3.2.0/insights/parsers/kdump.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/kernel_config.py` & `insights-core-3.2.0/insights/parsers/kernel_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/keystone.py` & `insights-core-3.2.0/insights/parsers/keystone.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/keystone_log.py` & `insights-core-3.2.0/insights/parsers/keystone_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/kpatch_list.py` & `insights-core-3.2.0/insights/parsers/kpatch_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/krb5.py` & `insights-core-3.2.0/insights/parsers/krb5.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,14 +69,29 @@
         if isinstance(val, str):
             val = [val]
         val.append(value)
         return val
     return value
 
 
+def _handle_krb5_bool(value):
+    """
+    Convert krb5.conf boolean
+    """
+    # see lib/krb5/krb/libdef_parse.c _krb5_conf_boolean()
+    if value in set(["y", "yes", "true", "t", "1", "on"]):
+        return True
+    elif value in set(["n", "no", "false", "nil", "0", "off"]):
+        return False
+    else:
+        # _krb5_conf_boolean() treats any other value as "False". Return
+        # "None" so caller can identify this case.
+        return None
+
+
 @parser(Specs.krb5)
 class Krb5Configuration(Parser, LegacyItemAccess):
     """
     Class for ``krb5.conf`` and ``krb5.conf.d`` configuration files.
 
     The Kerberos .ini format is like an ordinary .ini file except that values
     can include a multiple line key-value pair 'relation' that starts with a
@@ -175,7 +190,15 @@
         """
         Check for the existence of a given option in a given section.
         Return True if the given option is present, and False if not present.
         """
         if section not in self.data:
             return False
         return option in self.data[section]
+
+    def getboolean(self, section, option):
+        """Parse option as bool
+
+        Returns None is not a krb5.conf boolean string.
+        """
+        value = self.data[section][option]
+        return _handle_krb5_bool(value)
```

### Comparing `insights-core-3.1.9/insights/parsers/krb5kdc_log.py` & `insights-core-3.2.0/insights/parsers/krb5kdc_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ksmstate.py` & `insights-core-3.2.0/insights/parsers/ksmstate.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ktimer_lockless.py` & `insights-core-3.2.0/insights/parsers/ktimer_lockless.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/kubepods_cpu_quota.py` & `insights-core-3.2.0/insights/parsers/kubepods_cpu_quota.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ld_library_path.py` & `insights-core-3.2.0/insights/parsers/ld_library_path.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ldif_config.py` & `insights-core-3.2.0/insights/parsers/ldif_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/libssh_config.py` & `insights-core-3.2.0/insights/parsers/libssh_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/libvirtd_log.py` & `insights-core-3.2.0/insights/parsers/libvirtd_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/limits_conf.py` & `insights-core-3.2.0/insights/parsers/limits_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/logrotate_conf.py` & `insights-core-3.2.0/insights/parsers/logrotate_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/losetup.py` & `insights-core-3.2.0/insights/parsers/losetup.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/lpstat.py` & `insights-core-3.2.0/insights/parsers/lpstat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_boot.py` & `insights-core-3.2.0/insights/parsers/ls_boot.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_dev.py` & `insights-core-3.2.0/insights/parsers/ls_dev.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_disk.py` & `insights-core-3.2.0/insights/parsers/ls_disk.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_docker_volumes.py` & `insights-core-3.2.0/insights/parsers/ls_docker_volumes.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_edac_mc.py` & `insights-core-3.2.0/insights/parsers/ls_edac_mc.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_etc.py` & `insights-core-3.2.0/insights/parsers/ls_etc.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_ipa_idoverride_memberof.py` & `insights-core-3.2.0/insights/parsers/ls_ipa_idoverride_memberof.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_krb5_sssd.py` & `insights-core-3.2.0/insights/parsers/ls_krb5_sssd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_lib_firmware.py` & `insights-core-3.2.0/insights/parsers/ls_lib_firmware.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_ocp_cni_openshift_sdn.py` & `insights-core-3.2.0/insights/parsers/ls_ocp_cni_openshift_sdn.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_origin_local_volumes_pods.py` & `insights-core-3.2.0/insights/parsers/ls_origin_local_volumes_pods.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_osroot.py` & `insights-core-3.2.0/insights/parsers/ls_osroot.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_sys_firmware.py` & `insights-core-3.2.0/insights/parsers/ls_sys_firmware.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_systemd_units.py` & `insights-core-3.2.0/insights/parsers/ls_systemd_units.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_tmp.py` & `insights-core-3.2.0/insights/parsers/ls_tmp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_usr_bin.py` & `insights-core-3.2.0/insights/parsers/ls_usr_bin.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_usr_lib64.py` & `insights-core-3.2.0/insights/parsers/ls_usr_lib64.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_usr_sbin.py` & `insights-core-3.2.0/insights/parsers/ls_usr_sbin.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_var_cache_pulp.py` & `insights-core-3.2.0/insights/parsers/ls_var_cache_pulp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_var_lib_mongodb.py` & `insights-core-3.2.0/insights/parsers/ls_var_lib_mongodb.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_var_lib_nova_instances.py` & `insights-core-3.2.0/insights/parsers/ls_var_lib_nova_instances.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_var_lib_pcp.py` & `insights-core-3.2.0/insights/parsers/ls_var_lib_pcp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_var_lib_rsyslog.py` & `insights-core-3.2.0/insights/parsers/ls_var_lib_rsyslog.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_var_log.py` & `insights-core-3.2.0/insights/parsers/ls_var_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_var_opt_mssql.py` & `insights-core-3.2.0/insights/parsers/ls_var_opt_mssql.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_var_opt_mssql_log.py` & `insights-core-3.2.0/insights/parsers/ls_var_opt_mssql_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_var_run.py` & `insights-core-3.2.0/insights/parsers/ls_var_run.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_var_spool_clientmq.py` & `insights-core-3.2.0/insights/parsers/ls_var_spool_clientmq.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_var_spool_postfix_maildrop.py` & `insights-core-3.2.0/insights/parsers/ls_var_spool_postfix_maildrop.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_var_tmp.py` & `insights-core-3.2.0/insights/parsers/ls_var_tmp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ls_var_www_perms.py` & `insights-core-3.2.0/insights/parsers/ls_var_www_perms.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/lsblk.py` & `insights-core-3.2.0/insights/parsers/lsblk.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/lscpu.py` & `insights-core-3.2.0/insights/parsers/yum_conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,71 @@
 """
-LsCPU - command ``lscpu``
-=========================
-
-This module provides the information about the CPU architecture using the output of the command ``lscpu``.
+YumConf - file ``/etc/yum.conf``
+================================
 """
-from insights.core import CommandParser
-from insights.core.exceptions import SkipComponent
+import six
+
+from insights.core import IniConfigFile
 from insights.core.plugins import parser
+from insights.parsr.iniparser import NoOptionError
 from insights.specs import Specs
 
 
-@parser(Specs.lscpu)
-class LsCPU(CommandParser):
-    """Parse the output of ``/usr/bin/lscpu``. It uses the ``CommandParser`` as the
-    base class. The ``parse_content`` method also converts plural keys for
-    better accessibility.
-
-    Ex: "CPU(s)" is converted to "CPUs"
-
-    Typical output of ``lscpu`` command is::
-
-        Architecture:          x86_64
-        CPU op-mode(s):        32-bit, 64-bit
-        Byte Order:            Little Endian
-        CPU(s):                2
-        On-line CPU(s) list:   0,1
-        Thread(s) per core:    2
-        Core(s) per socket:    1
-        Socket(s):             1
-        NUMA node(s):          1
-        Vendor ID:             GenuineIntel
-        CPU family:            6
-        Model:                 60
-        Model name:            Intel Core Processor (Haswell, no TSX)
-        Stepping:              1
-        CPU MHz:               2793.530
-        BogoMIPS:              5587.06
-        Hypervisor vendor:     KVM
-        Virtualization type:   full
-        L1d cache:             32K
-        L1i cache:             32K
-        L2 cache:              4096K
-        NUMA node0 CPU(s):     0,1
+@parser(Specs.yum_conf)
+class YumConf(IniConfigFile):
+    """
+    This module provides parsing for the ``/etc/yum.conf`` file.
+    The ``YumConf`` class parses the information in the file
+    ``/etc/yum.conf``. See the ``IniConfigFile`` class for more
+    information on attributes and methods.
+
+    Sample input data looks like::
+
+        [main]
+        cachedir=/var/cache/yum/$basearch/$releasever
+        keepcache=0
+        debuglevel=2
+        logfile=/var/log/yum.log
+        exactarch=1
+        obsoletes=1
+        gpgcheck=1
+        plugins=1
+        installonly_limit=3
+
+        [rhel-7-server-rpms]
+        metadata_expire = 86400
+        baseurl = https://cdn.redhat.com/content/rhel/server/7/$basearch
+        name = Red Hat Enterprise Linux 7 Server (RPMs)
+        gpgkey = file:///etc/pki/rpm-gpg/RPM-GPG-KEY-redhat-release
+        enabled = 1
+        gpgcheck = 1
 
     Examples:
-
-        >>> output.info['Architecture']
-        'x86_64'
-        >>> len(output.info)
-        22
-        >>> output.info['CPUs']
-        '2'
-        >>> output.info['Threads per core']
-        '2'
-        >>> output.info['Cores per socket']
+        >>> type(yconf)
+        <class 'insights.parsers.yum_conf.YumConf'>
+        >>> 'main' in yconf
+        True
+        >>> 'rhel-7-server-rpms' in yconf
+        True
+        >>> yconf.has_option('main', 'gpgcheck')
+        True
+        >>> yconf.has_option('main', 'foo')
+        False
+        >>> yconf.get('rhel-7-server-rpms', 'enabled')
         '1'
-        >>> output.info['Sockets']
-        '1'
-
+        >>> expected = {'obsoletes': '1', 'keepcache': '0', 'logfile': '/var/log/yum.log', 'cachedir': '/var/cache/yum/$basearch/$releasever', 'exactarch': '1', 'plugins': '1', 'gpgcheck': '1', 'debuglevel': '2', 'installonly_limit': '3'}
+        >>> yconf.items('main') == expected
+        True
     """
     def parse_content(self, content):
-        if not content:
-            raise SkipComponent("No data.")
-        self.info = {}
-        split_on = ":"
-        for line in content:
-            # On R9 they added indentation and section headers,
-            # so make sure the split len is 2 otherwise skip.
-            kv = line.split(split_on, 1)
-            if len(kv) != 2:
-                continue
-
-            self.info[kv[0].replace("(s)", "s").strip()] = kv[1].strip()
+        super(YumConf, self).parse_content(content)
+        # File /etc/yum.conf may contain repos definitions.
+        # Keywords 'gpgkey' and 'baseurl' might contain multiple
+        # values separated by comma. Convert those values into a list.
+        for section in self.sections():
+            for key in ('gpgkey', 'baseurl'):
+                try:
+                    value = self.get(section, key)
+                    if value and isinstance(value, six.string_types):
+                        self.set(section, key, value.split(','))
+                except NoOptionError:
+                    pass
```

### Comparing `insights-core-3.1.9/insights/parsers/lsinitrd.py` & `insights-core-3.2.0/insights/parsers/lsinitrd.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,20 +6,24 @@
 
 Lsinitrd - command ``lsinitrd``
 -------------------------------
 
 LsinitrdKdumpImage - command ``lsinitrd initramfs-<kernel-version>kdump.img``
 -----------------------------------------------------------------------------
 
+LsinitrdLvmConf - command ``/bin/lsinitrd -f /etc/lvm/lvm.conf --kver {default_kernel_version}``
+------------------------------------------------------------------------------------------------
+
 """
 
 from insights import parser, CommandParser
 from insights.core import ls_parser
 from insights.specs import Specs
 from insights.parsers import keyword_search
+from insights.parsers.lvm import LvmConf
 
 
 @parser(Specs.lsinitrd)
 class Lsinitrd(CommandParser):
     """
     This parser parses the filtered output of command ``lsinitrd`` and provides
     the info of listed files.
@@ -132,7 +136,25 @@
         >>> lsinitrd_kdump_image.search(name__contains='urandom')
         >>> len(result_list)
         1
         >>> result_list[0].get('raw_entry')
         'crw-r--r--   1 root     root       1,   9 Aug  4  2020 dev/urandom'
     """
     pass
+
+
+@parser(Specs.lsinitrd_lvm_conf)
+class LsinitrdLvmConf(LvmConf):
+    """
+    Parses the ``/dev/lvm/lvm.conf`` file get from the default initramfs.
+
+    Sample Input::
+        # volume_list = [ "vg1", "vg2/lvol1", "@tag1", "@*" ]
+        volume_list = [ "vg2", "vg3/lvol3", "@tag2", "@*" ]
+
+    Examples:
+        >>> type(lsinitrd_lvm_conf)
+        <class 'insights.parsers.lsinitrd.LsinitrdLvmConf'>
+        >>> lsinitrd_lvm_conf.get("volume_list")
+        [ "vg2", "vg3/lvol3", "@tag2", "@*" ]
+    """
+    pass
```

### Comparing `insights-core-3.1.9/insights/parsers/lsmod.py` & `insights-core-3.2.0/insights/parsers/lsmod.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/lsof.py` & `insights-core-3.2.0/insights/parsers/lsof.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/lspci.py` & `insights-core-3.2.0/insights/parsers/lspci.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/lssap.py` & `insights-core-3.2.0/insights/parsers/lssap.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/lsscsi.py` & `insights-core-3.2.0/insights/parsers/lsscsi.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/luksmeta.py` & `insights-core-3.2.0/insights/parsers/luksmeta.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/lvdisplay.py` & `insights-core-3.2.0/insights/parsers/lvdisplay.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/lvm.py` & `insights-core-3.2.0/insights/parsers/lvm.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/manila_conf.py` & `insights-core-3.2.0/insights/parsers/manila_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/mariadb_log.py` & `insights-core-3.2.0/insights/parsers/mariadb_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/max_uid.py` & `insights-core-3.2.0/insights/parsers/max_uid.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/md5check.py` & `insights-core-3.2.0/insights/parsers/md5check.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/mdadm.py` & `insights-core-3.2.0/insights/parsers/mdadm.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/mdstat.py` & `insights-core-3.2.0/insights/parsers/mdstat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/meminfo.py` & `insights-core-3.2.0/insights/parsers/meminfo.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/mistral_log.py` & `insights-core-3.2.0/insights/parsers/mistral_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/mlx4_port.py` & `insights-core-3.2.0/insights/parsers/mlx4_port.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/modprobe.py` & `insights-core-3.2.0/insights/parsers/modprobe.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/mokutil_sbstate.py` & `insights-core-3.2.0/insights/parsers/mokutil_sbstate.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/mongod_conf.py` & `insights-core-3.2.0/insights/parsers/mongod_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/mount.py` & `insights-core-3.2.0/insights/parsers/mount.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/mpirun.py` & `insights-core-3.2.0/insights/parsers/mpirun.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/mssql_api_assessment.py` & `insights-core-3.2.0/insights/tests/parsers/test_mssql_api_assessment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,76 @@
-"""
-MssqlApiAssessment - file ``/var/opt/mssql/log/assessments/assessment-latest``
-==============================================================================
-
-Parsers contains in this module are:
-
-MssqlApiAssessment - file ``/var/opt/mssql/log/assessments/assessment-latest``
-"""
-
-from insights import JSONParser, parser
-from insights.specs import Specs
-
-
-@parser(Specs.mssql_api_assessment)
-class MssqlApiAssessment(JSONParser):
-    """
-    Parses the file: ``/var/opt/mssql/log/assessments/assessment-latest``
-
-    Sample content of the file::
-
-        [
-          {
-            "Timestamp": "2021-05-05T21:51:55.2317511-04:00",
-            "Severity": "Information",
-            "TargetType": "Server",
-            "TargetName": "ceph4-mon",
-            "TargetPath": "Server[@Name='ceph4-mon']",
-            "CheckId": "TF174",
-            "CheckName": "TF 174 increases plan cache bucket count",
-            "Message": "Enable trace flag 174 to increase plan cache bucket count",
-            "RulesetName": "Microsoft ruleset",
-            "RulesetVersion": "1.0.305",
-            "HelpLink": "https://docs.microsoft.com/sql/t-sql/database-console-commands/dbcc-traceon-trace-flags-transact-sql"
-          },
-          {
-            "Timestamp": "2021-05-05T21:51:55.2323431-04:00",
-            "Severity": "Information",
-            "TargetType": "Server",
-            "TargetName": "ceph4-mon",
-            "TargetPath": "Server[@Name='ceph4-mon']",
-            "CheckId": "TF834",
-            "CheckName": "TF 834 enables large-page allocations",
-            "Message": "Enable trace flag 834 to use large-page allocations to improve analytical and data warehousing workloads",
-            "RulesetName": "Microsoft ruleset",
-            "RulesetVersion": "1.0.305",
-            "HelpLink": "https://support.microsoft.com/kb/3210239"
-          }
-        ]
-
-    Examples:
-        >>> type(mssql_api_assessment_output)
-        <class 'insights.parsers.mssql_api_assessment.MssqlApiAssessment'>
-        >>> mssql_api_assessment_output[0]["Severity"] == 'Information'
-        True
-    """
-    pass
+import doctest
+
+from insights.parsers import mssql_api_assessment
+from insights.parsers.mssql_api_assessment import MssqlApiAssessment, ContainerMssqlApiAssessment
+from insights.tests import context_wrap
+
+API_OUTPUT = """
+[
+  {
+    "Timestamp": "2021-05-05T21:51:55.2317511-04:00",
+    "Severity": "Information",
+    "TargetType": "Server",
+    "TargetName": "ceph4-mon",
+    "TargetPath": "Server[@Name='ceph4-mon']",
+    "CheckId": "TF174",
+    "CheckName": "TF 174 increases plan cache bucket count",
+    "Message": "Enable trace flag 174 to increase plan cache bucket count",
+    "RulesetName": "Microsoft ruleset",
+    "RulesetVersion": "1.0.305",
+    "HelpLink": "https://docs.microsoft.com/sql/t-sql/database-console-commands/dbcc-traceon-trace-flags-transact-sql"
+  },
+  {
+    "Timestamp": "2021-05-05T21:51:55.2323431-04:00",
+    "Severity": "Information",
+    "TargetType": "Server",
+    "TargetName": "ceph4-mon",
+    "TargetPath": "Server[@Name='ceph4-mon']",
+    "CheckId": "TF834",
+    "CheckName": "TF 834 enables large-page allocations",
+    "Message": "Enable trace flag 834 to use large-page allocations to improve analytical and data warehousing workloads",
+    "RulesetName": "Microsoft ruleset",
+    "RulesetVersion": "1.0.305",
+    "HelpLink": "https://support.microsoft.com/kb/3210239"
+  }
+]
+""".strip()
+
+
+def test_mssql_api_assessment():
+    ret = MssqlApiAssessment(context_wrap(API_OUTPUT))
+    assert ret[0]["Severity"] == "Information"
+    assert ret[0]["TargetName"] == "ceph4-mon"
+    assert ret[0]["CheckId"] == "TF174"
+    assert ret[0]["Message"] == "Enable trace flag 174 to increase plan cache bucket count"
+
+
+def test_mssql_api_assessment_container():
+    container_ret = ContainerMssqlApiAssessment(
+        context_wrap(
+            API_OUTPUT,
+            container_id='2869b4e2541c',
+            image='registry.access.redhat.com/ubi8/nginx-120',
+            engine='podman',
+        )
+    )
+    assert container_ret.container_id == "2869b4e2541c"
+    assert container_ret[0]["Severity"] == "Information"
+    assert container_ret[0]["TargetName"] == "ceph4-mon"
+    assert container_ret[0]["CheckId"] == "TF174"
+    assert container_ret[0]["Message"] == "Enable trace flag 174 to increase plan cache bucket count"
+
+
+def test_mssql_api_assessment_doc_examples():
+    env = {
+        'mssql_api_assessment_output': MssqlApiAssessment(context_wrap(API_OUTPUT)),
+        'container_mssql_api_assessment_output': ContainerMssqlApiAssessment(
+            context_wrap(
+                API_OUTPUT,
+                container_id='2869b4e2541c',
+                image='registry.access.redhat.com/ubi8/nginx-120',
+                engine='podman',
+            )
+        )
+    }
+    failed, total = doctest.testmod(mssql_api_assessment, globs=env)
+    assert failed == 0
```

### Comparing `insights-core-3.1.9/insights/parsers/mssql_conf.py` & `insights-core-3.2.0/insights/parsers/mssql_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/multicast_querier.py` & `insights-core-3.2.0/insights/parsers/multicast_querier.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/multipath_conf.py` & `insights-core-3.2.0/insights/parsers/multipath_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/multipath_v4_ll.py` & `insights-core-3.2.0/insights/parsers/multipath_v4_ll.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/mysql_log.py` & `insights-core-3.2.0/insights/parsers/mysql_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/mysqladmin.py` & `insights-core-3.2.0/insights/parsers/mysqladmin.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/named_checkconf.py` & `insights-core-3.2.0/insights/parsers/named_checkconf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/named_conf.py` & `insights-core-3.2.0/insights/parsers/named_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ndctl_list.py` & `insights-core-3.2.0/insights/parsers/ndctl_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/net_namespace.py` & `insights-core-3.2.0/insights/parsers/net_namespace.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/netstat.py` & `insights-core-3.2.0/insights/parsers/netstat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/networkmanager_config.py` & `insights-core-3.2.0/insights/parsers/networkmanager_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/networkmanager_dhclient.py` & `insights-core-3.2.0/insights/parsers/networkmanager_dhclient.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/neutron_conf.py` & `insights-core-3.2.0/insights/parsers/neutron_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/neutron_dhcp_agent_conf.py` & `insights-core-3.2.0/insights/parsers/neutron_dhcp_agent_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/neutron_l3_agent_conf.py` & `insights-core-3.2.0/insights/parsers/neutron_l3_agent_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/neutron_l3_agent_log.py` & `insights-core-3.2.0/insights/parsers/neutron_l3_agent_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/neutron_metadata_agent_conf.py` & `insights-core-3.2.0/insights/parsers/neutron_metadata_agent_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/neutron_metadata_agent_log.py` & `insights-core-3.2.0/insights/parsers/neutron_metadata_agent_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/neutron_ml2_conf.py` & `insights-core-3.2.0/insights/parsers/neutron_ml2_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/neutron_ovs_agent_log.py` & `insights-core-3.2.0/insights/parsers/neutron_ovs_agent_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/neutron_plugin.py` & `insights-core-3.2.0/insights/parsers/neutron_plugin.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/neutron_server_log.py` & `insights-core-3.2.0/insights/parsers/neutron_server_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/neutron_sriov_agent.py` & `insights-core-3.2.0/insights/parsers/neutron_sriov_agent.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/nfnetlink_queue.py` & `insights-core-3.2.0/insights/parsers/nfnetlink_queue.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/nfs_conf.py` & `insights-core-3.2.0/insights/parsers/nfs_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/nfs_exports.py` & `insights-core-3.2.0/insights/parsers/nfs_exports.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/nginx_conf.py` & `insights-core-3.2.0/insights/parsers/nginx_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/nginx_log.py` & `insights-core-3.2.0/insights/parsers/nginx_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/nmcli.py` & `insights-core-3.2.0/insights/parsers/nmcli.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/nova_conf.py` & `insights-core-3.2.0/insights/parsers/nova_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/nova_log.py` & `insights-core-3.2.0/insights/parsers/nova_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/nova_user_ids.py` & `insights-core-3.2.0/insights/parsers/nova_user_ids.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/nscd_conf.py` & `insights-core-3.2.0/insights/parsers/nscd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/nss_rhel7.py` & `insights-core-3.2.0/insights/parsers/nss_rhel7.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/nsswitch_conf.py` & `insights-core-3.2.0/insights/parsers/nsswitch_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ntp_sources.py` & `insights-core-3.2.0/insights/parsers/ntp_sources.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/numa_cpus.py` & `insights-core-3.2.0/insights/parsers/numa_cpus.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/numeric_user_group_name.py` & `insights-core-3.2.0/insights/parsers/numeric_user_group_name.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/nvme_core_io_timeout.py` & `insights-core-3.2.0/insights/parsers/nvme_core_io_timeout.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/octavia.py` & `insights-core-3.2.0/insights/parsers/octavia.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/od_cpu_dma_latency.py` & `insights-core-3.2.0/insights/parsers/od_cpu_dma_latency.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/odbc.py` & `insights-core-3.2.0/insights/parsers/odbc.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/open_vm_tools.py` & `insights-core-3.2.0/insights/parsers/open_vm_tools.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/openshift_configuration.py` & `insights-core-3.2.0/insights/parsers/openshift_configuration.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/openshift_get.py` & `insights-core-3.2.0/insights/parsers/openshift_get.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/openshift_get_with_config.py` & `insights-core-3.2.0/insights/parsers/openshift_get_with_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/openshift_hosts.py` & `insights-core-3.2.0/insights/parsers/openshift_hosts.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/openvswitch_logs.py` & `insights-core-3.2.0/insights/parsers/openvswitch_logs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/openvswitch_other_config.py` & `insights-core-3.2.0/insights/parsers/openvswitch_other_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/oracle.py` & `insights-core-3.2.0/insights/parsers/oracle.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/os_release.py` & `insights-core-3.2.0/insights/parsers/os_release.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/osa_dispatcher_log.py` & `insights-core-3.2.0/insights/parsers/osa_dispatcher_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ovirt_engine_log.py` & `insights-core-3.2.0/insights/parsers/ovirt_engine_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ovs_appctl_fdb_show_bridge.py` & `insights-core-3.2.0/insights/parsers/ovs_appctl_fdb_show_bridge.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ovs_ofctl_dump_flows.py` & `insights-core-3.2.0/insights/parsers/ovs_ofctl_dump_flows.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ovs_vsctl.py` & `insights-core-3.2.0/insights/parsers/ovs_vsctl.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ovs_vsctl_list_bridge.py` & `insights-core-3.2.0/insights/parsers/ovs_vsctl_list_bridge.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ovs_vsctl_show.py` & `insights-core-3.2.0/insights/parsers/ovs_vsctl_show.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/pacemaker_log.py` & `insights-core-3.2.0/insights/parsers/pacemaker_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/package_provides.py` & `insights-core-3.2.0/insights/parsers/package_provides.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/pam.py` & `insights-core-3.2.0/insights/parsers/pam.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/parted.py` & `insights-core-3.2.0/insights/parsers/parted.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,16 +271,17 @@
                     this_start_idx = idx + 1
                     is_last_line_empty = False
                 else:
                     is_last_line_empty = True
             else:
                 is_last_line_empty = False
 
-        # Take left "content" as the last Device Section
-        device_tables.append(content[this_start_idx:])
+        # Take left "content" as the last Device Section, skip the empty case
+        if this_start_idx < len(content) - 1:
+            device_tables.append(content[this_start_idx:])
 
         devices_info = []
         for dev_table in device_tables:
             try:
                 this_parsed_dev_table = PartedDevice(dev_table)
                 devices_info.append(this_parsed_dev_table)
             except ParseException:
```

### Comparing `insights-core-3.1.9/insights/parsers/partitions.py` & `insights-core-3.2.0/insights/parsers/partitions.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/passenger_status.py` & `insights-core-3.2.0/insights/parsers/passenger_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/pci_rport_target_disk_paths.py` & `insights-core-3.2.0/insights/parsers/pci_rport_target_disk_paths.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/pcp_openmetrics_log.py` & `insights-core-3.2.0/insights/parsers/pcp_openmetrics_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/pcs_config.py` & `insights-core-3.2.0/insights/parsers/pcs_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/pcs_quorum_status.py` & `insights-core-3.2.0/insights/parsers/pcs_quorum_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/pcs_status.py` & `insights-core-3.2.0/insights/parsers/pcs_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/php_ini.py` & `insights-core-3.2.0/insights/parsers/php_ini.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,16 +140,16 @@
 
             res = Entry(children=Top(content), src=self)
             return apply_defaults(res)
 
         except SkipComponent:
             raise
         except:
-            raise ParseException(ParseException("Could not parse content: '{0}'".
-                                                format(content)))
+            raise ParseException("Could not parse content: '{0}'".
+                                                format(content))
 
     def parse_content(self, content):
         super(PHPConf, self).parse_content(content)
         dict_all = {}
         for section in self.doc:
             section_dict = {}
             option_names = set(o.name for o in section)
```

### Comparing `insights-core-3.1.9/insights/parsers/pluginconf_d.py` & `insights-core-3.2.0/insights/parsers/pluginconf_d.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/pmlog_summary.py` & `insights-core-3.2.0/insights/parsers/pmlog_summary.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/pmrep.py` & `insights-core-3.2.0/insights/parsers/pmrep.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/podman_inspect.py` & `insights-core-3.2.0/insights/parsers/podman_inspect.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/podman_list.py` & `insights-core-3.2.0/insights/parsers/podman_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/postconf.py` & `insights-core-3.2.0/insights/parsers/postconf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/postgresql_conf.py` & `insights-core-3.2.0/insights/parsers/postgresql_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/postgresql_log.py` & `insights-core-3.2.0/insights/parsers/postgresql_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/proc_environ.py` & `insights-core-3.2.0/insights/parsers/proc_environ.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/proc_keys.py` & `insights-core-3.2.0/insights/parsers/proc_keys.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/proc_limits.py` & `insights-core-3.2.0/insights/parsers/proc_limits.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/proc_stat.py` & `insights-core-3.2.0/insights/parsers/proc_stat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ps.py` & `insights-core-3.2.0/insights/parsers/ps.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/pulp_worker_defaults.py` & `insights-core-3.2.0/insights/parsers/pulp_worker_defaults.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/puppet_ca_cert_expire_date.py` & `insights-core-3.2.0/insights/parsers/puppet_ca_cert_expire_date.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/qemu_conf.py` & `insights-core-3.2.0/insights/parsers/qemu_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/qemu_xml.py` & `insights-core-3.2.0/insights/parsers/qemu_xml.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/qpid_stat.py` & `insights-core-3.2.0/insights/parsers/qpid_stat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/qpidd_conf.py` & `insights-core-3.2.0/insights/parsers/qpidd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rabbitmq.py` & `insights-core-3.2.0/insights/parsers/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rabbitmq_log.py` & `insights-core-3.2.0/insights/parsers/rabbitmq_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rc_local.py` & `insights-core-3.2.0/insights/parsers/rc_local.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rdma_config.py` & `insights-core-3.2.0/insights/parsers/rdma_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/readlink_e_mtab.py` & `insights-core-3.2.0/insights/parsers/readlink_e_mtab.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/readlink_openshift_certs.py` & `insights-core-3.2.0/insights/parsers/readlink_openshift_certs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/redhat_release.py` & `insights-core-3.2.0/insights/parsers/redhat_release.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/resolv_conf.py` & `insights-core-3.2.0/insights/parsers/resolv_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rhev_data_center.py` & `insights-core-3.2.0/insights/parsers/rhev_data_center.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rhn_charsets.py` & `insights-core-3.2.0/insights/parsers/rhn_charsets.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rhn_conf.py` & `insights-core-3.2.0/insights/parsers/rhn_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rhn_entitlement_cert_xml.py` & `insights-core-3.2.0/insights/parsers/rhn_entitlement_cert_xml.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rhn_hibernate_conf.py` & `insights-core-3.2.0/insights/parsers/rhn_hibernate_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rhn_logs.py` & `insights-core-3.2.0/insights/parsers/rhn_logs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rhn_schema_stats.py` & `insights-core-3.2.0/insights/parsers/rhn_schema_stats.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rhn_schema_version.py` & `insights-core-3.2.0/insights/parsers/rhn_schema_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rhosp_release.py` & `insights-core-3.2.0/insights/parsers/rhosp_release.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rhsm_conf.py` & `insights-core-3.2.0/insights/parsers/rhsm_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rhsm_log.py` & `insights-core-3.2.0/insights/parsers/rhsm_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rhsm_releasever.py` & `insights-core-3.2.0/insights/parsers/rhsm_releasever.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rhv_log_collector_analyzer.py` & `insights-core-3.2.0/insights/parsers/rhv_log_collector_analyzer.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rndc_status.py` & `insights-core-3.2.0/insights/parsers/rndc_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ros_config.py` & `insights-core-3.2.0/insights/parsers/ros_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/route.py` & `insights-core-3.2.0/insights/parsers/route.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rpm_ostree_status.py` & `insights-core-3.2.0/insights/parsers/rpm_ostree_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rpm_v_packages.py` & `insights-core-3.2.0/insights/parsers/rpm_v_packages.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rpm_vercmp.py` & `insights-core-3.2.0/insights/parsers/rpm_vercmp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/rsyslog_conf.py` & `insights-core-3.2.0/insights/parsers/rsyslog_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/samba.py` & `insights-core-3.2.0/insights/parsers/samba.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/samba_logs.py` & `insights-core-3.2.0/insights/parsers/samba_logs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sap_dev_trace_files.py` & `insights-core-3.2.0/insights/parsers/sap_dev_trace_files.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sap_hana_python_script.py` & `insights-core-3.2.0/insights/parsers/sap_hana_python_script.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sap_hdb_version.py` & `insights-core-3.2.0/insights/parsers/sap_hdb_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sap_host_profile.py` & `insights-core-3.2.0/insights/parsers/sap_host_profile.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sapcontrol.py` & `insights-core-3.2.0/insights/parsers/sapcontrol.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/saphostctrl.py` & `insights-core-3.2.0/insights/parsers/saphostctrl.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/saphostexec.py` & `insights-core-3.2.0/insights/parsers/saphostexec.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sat5_insights_properties.py` & `insights-core-3.2.0/insights/parsers/sat5_insights_properties.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/satellite_content_hosts_count.py` & `insights-core-3.2.0/insights/parsers/satellite_content_hosts_count.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/satellite_enabled_features.py` & `insights-core-3.2.0/insights/parsers/satellite_enabled_features.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/satellite_installer_configurations.py` & `insights-core-3.2.0/insights/parsers/satellite_installer_configurations.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/satellite_missed_queues.py` & `insights-core-3.2.0/insights/parsers/satellite_missed_queues.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/satellite_mongodb.py` & `insights-core-3.2.0/insights/parsers/satellite_mongodb.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/satellite_postgresql_query.py` & `insights-core-3.2.0/insights/parsers/satellite_postgresql_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,28 +16,29 @@
 ------------------------------------------------------------------------------------------------------------------
 SatelliteProvisionParamSettings - command ``psql -d foreman -c "select name, value from parameters where name='package_upgrade' and reference_id in (select id from operatingsystems where name='RedHat' and major='9')" --csv``
 --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 SatelliteQualifiedCapsules - command ``psql -d foreman -c "select name from smart_proxies where download_policy = 'background'" --csv``
 ---------------------------------------------------------------------------------------------------------------------------------------
 SatelliteQualifiedKatelloRepos - command ``psql -d foreman -c "select id, name, url, download_policy from katello_root_repositories where download_policy = 'background' or url is NULL" --csv``
 ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+SatelliteRHVHostsCount - command ``psql -d foreman -c "select count(*) from hosts where \"compute_resource_id\" in (select id from compute_resources where type='Foreman::Model::Ovirt')" --csv``
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 SatelliteSCAStatus - command ``psql -d candlepin -c "select displayname, content_access_mode from cp_owner" --csv``
 -------------------------------------------------------------------------------------------------------------------
 """
 import os
 import yaml
 
 from csv import DictReader
 
 from insights.core import CommandParser
 from insights.core.exceptions import ParseException, SkipComponent
 from insights.core.plugins import parser
 from insights.parsers import calc_offset, keyword_search
 from insights.specs import Specs
-from insights.util import deprecated
 
 
 class SatellitePostgreSQLQuery(CommandParser, list):
     """
     Parent class of satellite postgresql table queries. It can not be used
     directly, A child class with overriding columns attribute is required.
     It saves the rows data into a list. Each row is saved into a dict.
@@ -199,48 +200,14 @@
         <class 'insights.parsers.satellite_postgresql_query.SatelliteCoreTaskReservedResourceCount'>
         >>> tasks[0]['count']
         '0'
     """
     columns = ['count']
 
 
-@parser(Specs.satellite_katello_empty_url_repositories)
-class SatelliteKatelloEmptyURLRepositories(SatellitePostgreSQLQuery):
-    """
-    .. warning::
-        This parser is deprecated, please use
-        :py:class:`insights.parsers.satellite_postgresql_query.SatelliteQualifiedKatelloRepos` instead.
-
-    Parse the output of the command ``psql -d foreman -c 'select id, name from katello_root_repositories where url is NULL;' --csv``.
-
-    Sample output::
-
-        id,name
-        54,testa
-        55,testb
-
-    Examples:
-        >>> type(katello_root_repositories)
-        <class 'insights.parsers.satellite_postgresql_query.SatelliteKatelloEmptyURLRepositories'>
-        >>> len(katello_root_repositories)
-        2
-        >>> katello_root_repositories[0]['name']
-        'testa'
-    """
-    columns = ['id', 'name']
-
-    def __init__(self, *args, **kwargs):
-        deprecated(
-            SatelliteKatelloEmptyURLRepositories,
-            "Please use the SatelliteQualifiedKatelloRepos parser in the current module.",
-            "3.1.25"
-        )
-        super(SatelliteKatelloEmptyURLRepositories, self).__init__(*args, **kwargs)
-
-
 @parser(Specs.satellite_logs_table_size)
 class SatelliteLogsTableSize(SatellitePostgreSQLQuery):
     """
     Parse the output of the command ``psql -d foreman -c "select pg_total_relation_size('logs') as logs_size" --csv``.
 
     Sample output::
 
@@ -353,14 +320,33 @@
         2
         >>> capsules[0]['name']
         'capsule1.test.com'
     """
     columns = ['name']
 
 
+@parser(Specs.satellite_rhv_hosts_count)
+class SatelliteRHVHostsCount(SatellitePostgreSQLQuery):
+    """
+    Parse the output of the command ``psql -d pulpcore -c "select count(*) from hosts where \"compute_resource_id\" in (select id from compute_resources where type='Foreman::Model::Ovirt')" --csv``.
+
+    Sample output::
+
+        count
+        2
+
+    Examples:
+        >>> type(rhv_hosts)
+        <class 'insights.parsers.satellite_postgresql_query.SatelliteRHVHostsCount'>
+        >>> rhv_hosts[0]['count']
+        '2'
+    """
+    columns = ['count']
+
+
 @parser(Specs.satellite_sca_status)
 class SatelliteSCAStatus(SatellitePostgreSQLQuery):
     """
     Parse the output of the command ``psql -d candlepin -c "select displayname, content_access_mode from cp_owner" --csv``.
 
     Sample output::
```

### Comparing `insights-core-3.1.9/insights/parsers/satellite_version.py` & `insights-core-3.2.0/insights/parsers/satellite_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/satellite_yaml.py` & `insights-core-3.2.0/insights/parsers/satellite_yaml.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/scheduler.py` & `insights-core-3.2.0/insights/parsers/scheduler.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/scsi.py` & `insights-core-3.2.0/insights/parsers/scsi.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/scsi_eh_deadline.py` & `insights-core-3.2.0/insights/parsers/scsi_eh_deadline.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/scsi_fwver.py` & `insights-core-3.2.0/insights/parsers/scsi_fwver.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sctp.py` & `insights-core-3.2.0/insights/parsers/sctp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sealert.py` & `insights-core-3.2.0/insights/parsers/sealert.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/secure.py` & `insights-core-3.2.0/insights/parsers/secure.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/selinux_config.py` & `insights-core-3.2.0/insights/parsers/selinux_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/semanage.py` & `insights-core-3.2.0/insights/parsers/semanage.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sendq_recvq_socket_buffer.py` & `insights-core-3.2.0/insights/parsers/sendq_recvq_socket_buffer.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sestatus.py` & `insights-core-3.2.0/insights/parsers/sestatus.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/setup_named_chroot.py` & `insights-core-3.2.0/insights/parsers/setup_named_chroot.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/slabinfo.py` & `insights-core-3.2.0/insights/parsers/slabinfo.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/smartctl.py` & `insights-core-3.2.0/insights/parsers/smartctl.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/smartpdc_settings.py` & `insights-core-3.2.0/insights/parsers/smartpdc_settings.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/smbstatus.py` & `insights-core-3.2.0/insights/parsers/smbstatus.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/smt.py` & `insights-core-3.2.0/insights/parsers/smt.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/snmp.py` & `insights-core-3.2.0/insights/parsers/snmp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sockstat.py` & `insights-core-3.2.0/insights/parsers/sockstat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/softnet_stat.py` & `insights-core-3.2.0/insights/parsers/softnet_stat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/software_collections_list.py` & `insights-core-3.2.0/insights/parsers/software_collections_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sos_conf.py` & `insights-core-3.2.0/insights/parsers/sos_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/spamassassin_channels.py` & `insights-core-3.2.0/insights/parsers/spamassassin_channels.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ssh.py` & `insights-core-3.2.0/insights/parsers/ssh.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ssh_client_config.py` & `insights-core-3.2.0/insights/parsers/ssh_client_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/ssl_certificate.py` & `insights-core-3.2.0/insights/parsers/ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sssd_conf.py` & `insights-core-3.2.0/insights/parsers/sssd_conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         """
         Returns the list of domains defined in the 'sssd' section.  This is
         used to refer to the domain-specific sections of the configuration.
         """
         if self.has_option('sssd', 'domains'):
             domains = self.get('sssd', 'domains')
             if domains:
-                return domains.split(',')
+                return [domain.strip() for domain in domains.split(',')]
 
         # Return a blank list if no domains.
         return []
 
     def domain_config(self, domain):
         """
         Return the configuration dictionary for a specific domain, given as
```

### Comparing `insights-core-3.1.9/insights/parsers/sssd_logs.py` & `insights-core-3.2.0/insights/parsers/sssd_logs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/subscription_manager.py` & `insights-core-3.2.0/insights/parsers/subscription_manager.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/subscription_manager_list.py` & `insights-core-3.2.0/insights/parsers/subscription_manager_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/subscription_manager_release.py` & `insights-core-3.2.0/insights/parsers/subscription_manager_release.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sudoers.py` & `insights-core-3.2.0/insights/parsers/sudoers.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/swift_conf.py` & `insights-core-3.2.0/insights/parsers/swift_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/swift_log.py` & `insights-core-3.2.0/insights/parsers/swift_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sys_bus.py` & `insights-core-3.2.0/insights/parsers/sys_bus.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sys_fs_cgroup_memory.py` & `insights-core-3.2.0/insights/parsers/sys_fs_cgroup_memory.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sys_fs_cgroup_memory_tasks_number.py` & `insights-core-3.2.0/insights/parsers/sys_fs_cgroup_memory_tasks_number.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sys_kernel.py` & `insights-core-3.2.0/insights/parsers/sys_kernel.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sys_module.py` & `insights-core-3.2.0/insights/parsers/sys_module.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sys_vmbus.py` & `insights-core-3.2.0/insights/parsers/sys_vmbus.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sysconfig.py` & `insights-core-3.2.0/insights/parsers/sysconfig.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/sysctl.py` & `insights-core-3.2.0/insights/parsers/sysctl.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/system_time.py` & `insights-core-3.2.0/insights/parsers/system_time.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/systemctl_show.py` & `insights-core-3.2.0/insights/parsers/systemctl_show.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/systemctl_status_all.py` & `insights-core-3.2.0/insights/tests/parsers/test_systemctl_status_all.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-"""
-SystemctlStatusAll command ``systemctl status --all``
-=====================================================
-"""
-
-from insights.core import LogFileOutput
-from insights.core.plugins import parser
-from insights.specs import Specs
-
-
-@parser(Specs.systemctl_status_all)
-class SystemctlStatusAll(LogFileOutput):
-    """
-    Class for parsing the output from command ``systemctl status --all``.
-
-    .. note::
-        Please refer to its super-class :class:`insights.core.LogFileOutput`
-
-    Sample log lines::
-
-        * redhat.test.com
-            State: degraded
-             Jobs: 0 queued
-           Failed: 2 units
-            Since: Thu 2021-09-23 12:03:43 UTC; 3h 7min ago
-           CGroup: /
-                   |-user.slice
-                   | `-user-1000.slice
-                   |   |-user@1000.service
-
-        * proc-sys-fs-binfmt_misc.automount - Arbitrary Executable File Formats File System Automount Point
-           Loaded: loaded (/usr/lib/systemd/system/proc-sys-fs-binfmt_misc.automount; static; vendor preset: disabled)
-           Active: active (running) since Thu 2021-09-23 12:03:43 UTC; 3h 7min ago
-            Where: /proc/sys/fs/binfmt_misc
-             Docs: https://www.kernel.org/doc/html/latest/admin-guide/binfmt-misc.html
-                   https://www.freedesktop.org/wiki/Software/systemd/APIFileSystems
-
-        Sep 23 15:11:07 redhat.test.com systemd[1]: proc-sys-fs-binfmt_misc.automount: Automount point already active?
-        Sep 23 15:11:07 redhat.test.com systemd[1]: proc-sys-fs-binfmt_misc.automount: Got automount request for /proc/sys/fs/binfmt_mis
-
-    Examples:
-        >>> "Automount point already active?" in log
-        True
-    """
-    pass
+import doctest
+
+from insights.parsers import systemctl_status_all
+from insights.parsers.systemctl_status_all import SystemctlStatusAll
+from insights.tests import context_wrap
+
+SYSTEMCTLSTATUSALL = """
+* redhat.test.com
+    State: degraded
+     Jobs: 0 queued
+   Failed: 2 units
+    Since: Thu 2021-09-23 12:03:43 UTC; 3h 7min ago
+   CGroup: /
+           |-user.slice
+           | `-user-1000.slice
+           |   |-user@1000.service
+
+* proc-sys-fs-binfmt_misc.automount - Arbitrary Executable File Formats File System Automount Point
+   Loaded: loaded (/usr/lib/systemd/system/proc-sys-fs-binfmt_misc.automount; static; vendor preset: disabled)
+   Active: active (running) since Thu 2021-09-23 12:03:43 UTC; 3h 7min ago
+    Where: /proc/sys/fs/binfmt_misc
+     Docs: https://www.kernel.org/doc/html/latest/admin-guide/binfmt-misc.html
+           https://www.freedesktop.org/wiki/Software/systemd/APIFileSystems
+
+Sep 23 15:11:07 redhat.test.com systemd[1]: proc-sys-fs-binfmt_misc.automount: Automount point already active?
+Sep 23 15:11:07 redhat.test.com systemd[1]: proc-sys-fs-binfmt_misc.automount: Got automount request for /proc/sys/fs/binfmt_mis
+""".strip()
+
+
+def test_systemctl_status():
+    ret = SystemctlStatusAll(context_wrap(SYSTEMCTLSTATUSALL))
+    assert "Automount point already active?" in ret
+    assert ret.state == 'degraded'
+    assert ret.jobs == '0 queued'
+    assert ret.failed == '2 units'
+
+
+def test_doc_example():
+    failed_count, tests = doctest.testmod(
+        systemctl_status_all,
+        globs={'systemctl_status': SystemctlStatusAll(context_wrap(SYSTEMCTLSTATUSALL))}
+    )
+    assert failed_count == 0
```

### Comparing `insights-core-3.1.9/insights/parsers/systemd_analyze.py` & `insights-core-3.2.0/insights/parsers/systemd_analyze.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/systemid.py` & `insights-core-3.2.0/insights/parsers/systemid.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/systool.py` & `insights-core-3.2.0/insights/parsers/systool.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/teamdctl_config_dump.py` & `insights-core-3.2.0/insights/parsers/teamdctl_config_dump.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/teamdctl_state_dump.py` & `insights-core-3.2.0/insights/parsers/teamdctl_state_dump.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/tmpfilesd.py` & `insights-core-3.2.0/insights/parsers/tmpfilesd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/tomcat_virtual_dir_context.py` & `insights-core-3.2.0/insights/parsers/tomcat_virtual_dir_context.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/tomcat_xml.py` & `insights-core-3.2.0/insights/parsers/tomcat_xml.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/transparent_hugepage.py` & `insights-core-3.2.0/insights/parsers/transparent_hugepage.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/tuned.py` & `insights-core-3.2.0/insights/parsers/tuned.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/tuned_conf.py` & `insights-core-3.2.0/insights/parsers/tuned_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/udev_rules.py` & `insights-core-3.2.0/insights/parsers/udev_rules.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/uname.py` & `insights-core-3.2.0/insights/parsers/uname.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,16 +111,18 @@
     "4.18.0-147": "8.1",
     "4.18.0-193": "8.2",
     "4.18.0-240": "8.3",
     "4.18.0-305": "8.4",
     "4.18.0-348": "8.5",
     "4.18.0-372": "8.6",
     "4.18.0-425": "8.7",
+    "4.18.0-477": "8.8",
     "5.14.0-70": "9.0",
     "5.14.0-162": "9.1",
+    "5.14.0-284": "9.2",
 }
 
 release_to_kernel_map = dict((v, k) for k, v in rhel_release_map.items())
 RedhatRelease = namedtuple("RedhatRelease", ("major", "minor"))
 
 
 class UnameError(Exception):
@@ -247,15 +249,20 @@
         uname_parts = uname_line.split(' ')
         if len(uname_parts) < 3:
             raise UnameError("Uname string appears invalid", uname_line)
         else:
             data['kernel'] = uname_parts[2]
             data['name'] = uname_parts[0]
             data['nodename'] = uname_parts[1]
-        has_arch = "el" not in data['kernel'].split(".")[-1]
+
+        # Check if the last segment of kernel version is the architecture (e.g. x86_64)
+        last_kernel_segment = data['kernel'].split(".")[-1]
+        # If the last segment contains "el" then we assume its the product indicator (e.g. el9_2)
+        # If the last segment contains more than just digits we assume its the architecture (e.g. x86_64)
+        has_arch = "el" not in last_kernel_segment and not last_kernel_segment.isdigit()
         try:
             data = self.parse_nvr(data['kernel'], data, arch=has_arch)
         except UnameError as error:
             error.uname_line = uname_line
             raise error
 
         # Additional uname content parsing, may not be as reliable
@@ -573,31 +580,40 @@
 
 def pad_release(release_to_pad, num_sections=4):
     '''
     Pad out package and kernel release versions so that
     ``LooseVersion`` comparisons will be correct.
 
     Release versions with less than num_sections will
-    be padded in front of the last section with zeros.
+    padded with zeros where missing versions segments are.
 
     For example ::
 
         pad_release("390.el6", 4)
 
     will return ``390.0.0.el6`` and ::
 
         pad_release("390.11.el6", 4)
 
-    will return ``390.11.0.el6``.
+    will return ``390.11.0.el6``. Finally, if no "el" is specified:
+
+        pad_release("390.11", 4)
+
+    will return ``390.11.0.0``.
 
     If the number of sections of the release to be padded is
     greater than num_sections, a ``ValueError`` will be raised.
     '''
     parts = release_to_pad.split('.')
 
     if len(parts) > num_sections:
         raise ValueError("Too many sections encountered ({found} > {num} in release string {rel}".format(
             found=len(parts), num=num_sections, rel=release_to_pad
         ))
 
     pad_count = num_sections - len(parts)
-    return ".".join(parts[:-1] + ['0'] * pad_count + parts[-1:])
+    is_el_release = any(letter.isalpha() for letter in parts[-1])
+
+    if len(parts) > 1 and is_el_release:
+        return ".".join(parts[:-1] + ['0'] * pad_count + parts[-1:])
+    else:
+        return ".".join(parts + ['0'] * pad_count)
```

### Comparing `insights-core-3.1.9/insights/parsers/up2date_log.py` & `insights-core-3.2.0/insights/parsers/up2date_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/upstart.py` & `insights-core-3.2.0/insights/parsers/upstart.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/uptime.py` & `insights-core-3.2.0/insights/parsers/uptime.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/user_group.py` & `insights-core-3.2.0/insights/parsers/user_group.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/vdo_status.py` & `insights-core-3.2.0/insights/parsers/vdo_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/vdsm_conf.py` & `insights-core-3.2.0/insights/parsers/vdsm_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/vdsm_log.py` & `insights-core-3.2.0/insights/parsers/vdsm_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/version_info.py` & `insights-core-3.2.0/insights/parsers/version_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 """
 VersionInfo - file ``version_info``
 ===================================
 
-The version of the insights core and insights client that the archive used.
+.. warning::
+    This parser is deprecated, please use
+    :py:class:`insights.parsers.client_metadata.VersionInfo` instead.
+
 
+The version of the insights core and insights client that the archive used.
 """
 from insights import JSONParser, parser
 from insights.specs import Specs
+from insights.util import deprecated
 
 
 @parser(Specs.version_info)
 class VersionInfo(JSONParser):
     """
+    .. warning::
+        This parser is deprecated, please use
+        :py:class:`insights.parsers.client_metadata.VersionInfo` instead.
+
     This parser parses the ``version_info`` file generated by the
     ``insights-client`` command.
 
     Typical content of this file is::
 
         {"core_version": "3.0.203-1", "client_version": "3.1.1"}
 
@@ -28,14 +37,22 @@
 
     Examples:
         >>> ver.core_version == '3.0.203-1'
         True
         >>> ver.client_version == '3.1.1'
         True
     """
+    def __init__(self, *args, **kwargs):
+        deprecated(
+            VersionInfo,
+            "Please use insights.parsers.client_metadata.VersionInfo instead.",
+            "3.3.25"
+        )
+        super(VersionInfo, self).__init__(*args, **kwargs)
+
     @property
     def core_version(self):
         """
         Returns:
             (str): The version of the insights core.
         """
         return self.data['core_version']
```

### Comparing `insights-core-3.1.9/insights/parsers/vgdisplay.py` & `insights-core-3.2.0/insights/parsers/vgdisplay.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/virsh_list_all.py` & `insights-core-3.2.0/insights/parsers/virsh_list_all.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/virt_uuid_facts.py` & `insights-core-3.2.0/insights/parsers/virt_uuid_facts.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/virt_what.py` & `insights-core-3.2.0/insights/parsers/virt_what.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/virt_who_conf.py` & `insights-core-3.2.0/insights/parsers/virt_who_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/virtlogd_conf.py` & `insights-core-3.2.0/insights/parsers/virtlogd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/vma_ra_enabled_s390x.py` & `insights-core-3.2.0/insights/parsers/vma_ra_enabled_s390x.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/vmcore_dmesg.py` & `insights-core-3.2.0/insights/parsers/vmcore_dmesg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/vmware_tools_conf.py` & `insights-core-3.2.0/insights/parsers/vmware_tools_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/vsftpd.py` & `insights-core-3.2.0/insights/parsers/vsftpd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/wc_proc_1_mountinfo.py` & `insights-core-3.2.0/insights/parsers/wc_proc_1_mountinfo.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/x86_debug.py` & `insights-core-3.2.0/insights/parsers/x86_debug.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/xfs_info.py` & `insights-core-3.2.0/insights/parsers/xfs_info.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/xinetd_conf.py` & `insights-core-3.2.0/insights/parsers/xinetd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/yum.py` & `insights-core-3.2.0/insights/parsers/yum.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/yum_conf.py` & `insights-core-3.2.0/insights/specs/datasources/cloud_init.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,88 @@
 """
-YumConf - file ``/etc/yum.conf``
-================================
+Custom datasources for cloud initialization information
 """
-import six
+import yaml
 
-from insights.core import IniConfigFile
-from insights.core.plugins import parser
-from insights.parsr.iniparser import NoOptionError
+from insights.core.context import HostContext
+from insights.core.exceptions import SkipComponent
+from insights.core.filters import get_filters
+from insights.core.plugins import datasource
+from insights.core.spec_factory import DatasourceProvider, simple_file
 from insights.specs import Specs
 
 
-@parser(Specs.yum_conf)
-class YumConf(IniConfigFile):
+class LocalSpecs(Specs):
+    """ Local specs used only by cloud_init datasources """
+
+    cloud_cfg_input = simple_file("/etc/cloud/cloud.cfg")
+    """ Returns the contents of the file ``/etc/cloud/cloud.cfg`` """
+
+
+@datasource(LocalSpecs.cloud_cfg_input, HostContext)
+def cloud_cfg(broker):
     """
-    This module provides parsing for the ``/etc/yum.conf`` file.
-    The ``YumConf`` class parses the information in the file
-    ``/etc/yum.conf``. See the ``IniConfigFile`` class for more
-    information on attributes and methods.
-
-    Sample input data looks like::
-
-        [main]
-        cachedir=/var/cache/yum/$basearch/$releasever
-        keepcache=0
-        debuglevel=2
-        logfile=/var/log/yum.log
-        exactarch=1
-        obsoletes=1
-        gpgcheck=1
-        plugins=1
-        installonly_limit=3
-
-        [rhel-7-server-rpms]
-        metadata_expire = 86400
-        baseurl = https://cdn.redhat.com/content/rhel/server/7/$basearch
-        name = Red Hat Enterprise Linux 7 Server (RPMs)
-        gpgkey = file:///etc/pki/rpm-gpg/RPM-GPG-KEY-redhat-release
-        enabled = 1
-        gpgcheck = 1
-
-    Examples:
-        >>> type(yconf)
-        <class 'insights.parsers.yum_conf.YumConf'>
-        >>> 'main' in yconf
-        True
-        >>> 'rhel-7-server-rpms' in yconf
-        True
-        >>> yconf.has_option('main', 'gpgcheck')
-        True
-        >>> yconf.has_option('main', 'foo')
-        False
-        >>> yconf.get('rhel-7-server-rpms', 'enabled')
-        '1'
-        >>> expected = {'obsoletes': '1', 'keepcache': '0', 'logfile': '/var/log/yum.log', 'cachedir': '/var/cache/yum/$basearch/$releasever', 'exactarch': '1', 'plugins': '1', 'gpgcheck': '1', 'debuglevel': '2', 'installonly_limit': '3'}
-        >>> yconf.items('main') == expected
-        True
+    This datasource provides configuration of ``/etc/cloud/cloud.cfg`` file.
+
+    .. note::
+        Since this file may contain sensitive information, it should be
+        filtered before the Insights collecting it.  The filters will be added
+        via the :mod:`insights.specs.Specs.cloud_cfg` Spec.  If nothing is
+        added to the filter, nothing will be collected.
+
+    Typical content of ``/etc/cloud/cloud.cfg`` file is::
+
+        #cloud-config
+        users:
+          - name: demo
+            ssh-authorized-keys:
+              - key_one
+              - key_two
+            passwd: $6$j212wezy$7H/1LT4f9/N3wpgNunhsIqtMj62OKiS3nyNwuizouQc3u7
+
+        ssh_deletekeys: 1
+
+        network:
+            version: 1
+            config:
+              - type: physical
+                name: eth0
+                subnets:
+                  - type: dhcp
+                  - type: dhcp6
+
+        system_info:
+            default_user:
+            name: user2
+            plain_text_passwd: 'someP@assword'
+            home: /home/user2
+
+        debug:
+            output: /var/log/cloud-init-debug.log
+            verbose: true
+
+    Returns:
+        str: YAML string after removing the sensitive information.
+
+    Raises:
+        SkipComponent: When the path does not exist, nothing is collected,
+                       or any exception occurs.
     """
-    def parse_content(self, content):
-        super(YumConf, self).parse_content(content)
-        # File /etc/yum.conf may contain repos definitions.
-        # Keywords 'gpgkey' and 'baseurl' might contain multiple
-        # values separated by comma. Convert those values into a list.
-        for section in self.sections():
-            for key in ('gpgkey', 'baseurl'):
-                try:
-                    value = self.get(section, key)
-                    if value and isinstance(value, six.string_types):
-                        self.set(section, key, value.split(','))
-                except NoOptionError:
-                    pass
+    relative_path = '/etc/cloud/cloud.cfg'
+    try:
+        filters = get_filters(Specs.cloud_cfg)
+        content = broker[LocalSpecs.cloud_cfg_input].content
+        if content and filters:
+            result = dict()
+            content = yaml.load('\n'.join(content), Loader=yaml.SafeLoader)
+            if isinstance(content, dict):
+                # apply filters after ignoring sensitive data
+                for item in filters:
+                    if item not in ('users', 'system_info') and item in content:
+                        result[item] = content[item]
+
+                if result:
+                    return DatasourceProvider(content=yaml.dump(result), relative_path=relative_path)
+            raise SkipComponent("Invalid YAML format")
+    except Exception as e:
+        raise SkipComponent("Unexpected exception:{e}".format(e=str(e)))
+    raise SkipComponent
```

### Comparing `insights-core-3.1.9/insights/parsers/yum_list.py` & `insights-core-3.2.0/insights/parsers/yum_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/yum_repos_d.py` & `insights-core-3.2.0/insights/parsers/yum_repos_d.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/yum_updateinfo.py` & `insights-core-3.2.0/insights/parsers/yum_updateinfo.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/yum_updates.py` & `insights-core-3.2.0/insights/parsers/yum_updates.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/yumlog.py` & `insights-core-3.2.0/insights/parsers/yumlog.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/zdump_v.py` & `insights-core-3.2.0/insights/parsers/zdump_v.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsers/zipl_conf.py` & `insights-core-3.2.0/insights/parsers/zipl_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/tests/test_corosync.py` & `insights-core-3.2.0/insights/parsr/examples/tests/test_corosync.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/tests/test_httpd.py` & `insights-core-3.2.0/insights/parsr/examples/tests/test_httpd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/tests/test_json.py` & `insights-core-3.2.0/insights/parsr/examples/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/tests/test_logrotate.py` & `insights-core-3.2.0/insights/parsr/examples/tests/test_logrotate.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/tests/test_multipath.py` & `insights-core-3.2.0/insights/parsr/examples/tests/test_multipath.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/tests/test_nginx.py` & `insights-core-3.2.0/insights/parsr/examples/tests/test_nginx.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/arith.py` & `insights-core-3.2.0/insights/parsr/examples/arith.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/corosync_conf.py` & `insights-core-3.2.0/insights/parsr/examples/corosync_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/httpd_conf.py` & `insights-core-3.2.0/insights/parsr/examples/httpd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/iniparser.py` & `insights-core-3.2.0/insights/parsr/examples/iniparser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/json_parser.py` & `insights-core-3.2.0/insights/parsr/examples/json_parser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/kvpairs.py` & `insights-core-3.2.0/insights/parsr/examples/kvpairs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/logrotate_conf.py` & `insights-core-3.2.0/insights/parsr/examples/logrotate_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/multipath_conf.py` & `insights-core-3.2.0/insights/parsr/examples/multipath_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/examples/nginx_conf.py` & `insights-core-3.2.0/insights/parsr/examples/nginx_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/query/tests/test_boolean.py` & `insights-core-3.2.0/insights/parsr/query/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/query/tests/test_choose.py` & `insights-core-3.2.0/insights/parsr/query/tests/test_choose.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/query/tests/test_compile_queries.py` & `insights-core-3.2.0/insights/parsr/query/tests/test_compile_queries.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/query/tests/test_crumbs.py` & `insights-core-3.2.0/insights/parsr/query/tests/test_crumbs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/query/tests/test_find.py` & `insights-core-3.2.0/insights/parsr/query/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/query/tests/test_query.py` & `insights-core-3.2.0/insights/parsr/query/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/query/tests/test_where.py` & `insights-core-3.2.0/insights/parsr/query/tests/test_where.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/query/__init__.py` & `insights-core-3.2.0/insights/parsr/query/__init__.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/query/boolean.py` & `insights-core-3.2.0/insights/parsr/query/boolean.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/tests/test_iniparser.py` & `insights-core-3.2.0/insights/parsr/tests/test_iniparser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/tests/test_many.py` & `insights-core-3.2.0/insights/parsr/tests/test_many.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/tests/test_pos_marker.py` & `insights-core-3.2.0/insights/parsr/tests/test_pos_marker.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/tests/test_string.py` & `insights-core-3.2.0/insights/parsr/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/__init__.py` & `insights-core-3.2.0/insights/parsr/__init__.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/parsr/iniparser.py` & `insights-core-3.2.0/insights/parsr/iniparser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/plugins/ps_rule_fakes.py` & `insights-core-3.2.0/insights/plugins/ps_rule_fakes.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/plugins/rules_fixture_plugin.py` & `insights-core-3.2.0/insights/plugins/rules_fixture_plugin.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/container/__init__.py` & `insights-core-3.2.0/insights/specs/datasources/container/__init__.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/container/containers_inspect.py` & `insights-core-3.2.0/insights/specs/datasources/container/containers_inspect.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/container/nginx_conf.py` & `insights-core-3.2.0/insights/specs/datasources/container/nginx_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/__init__.py` & `insights-core-3.2.0/insights/specs/datasources/__init__.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/aws.py` & `insights-core-3.2.0/insights/specs/datasources/aws.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/awx_manage.py` & `insights-core-3.2.0/insights/specs/datasources/awx_manage.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/candlepin_broker.py` & `insights-core-3.2.0/insights/specs/datasources/candlepin_broker.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/corosync.py` & `insights-core-3.2.0/insights/specs/datasources/corosync.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/dir_list.py` & `insights-core-3.2.0/insights/specs/datasources/dir_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/ethernet.py` & `insights-core-3.2.0/insights/specs/datasources/ethernet.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/httpd.py` & `insights-core-3.2.0/insights/specs/datasources/httpd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/ipcs.py` & `insights-core-3.2.0/insights/specs/datasources/ipcs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/kernel_module_list.py` & `insights-core-3.2.0/insights/specs/datasources/kernel_module_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/lpstat.py` & `insights-core-3.2.0/insights/specs/datasources/lpstat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/luks_devices.py` & `insights-core-3.2.0/insights/specs/datasources/luks_devices.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/malware_detection.py` & `insights-core-3.2.0/insights/specs/datasources/malware_detection.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,10 +29,12 @@
             if scan_results:
                 return DatasourceProvider(content=scan_results, relative_path="malware-detection-results.json")
             else:
                 raise SkipComponent("No scan results were produced")
         except SkipComponent as msg:
             raise SkipComponent("Skipping malware-detection app: {0}".format(str(msg)))
         except Exception as err:
+            from traceback import format_exc
             err_msg = "Unexpected exception in malware-detection app: {0}".format(str(err))
-            logger.exception(err_msg)
+            logger.error(err_msg)
+            logger.debug(format_exc())
             raise SkipComponent(err_msg)
```

### Comparing `insights-core-3.1.9/insights/specs/datasources/md5chk.py` & `insights-core-3.2.0/insights/specs/datasources/md5chk.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/package_provides.py` & `insights-core-3.2.0/insights/specs/datasources/package_provides.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/pcp.py` & `insights-core-3.2.0/insights/specs/datasources/pcp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/ps.py` & `insights-core-3.2.0/insights/specs/datasources/ps.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/rpm_pkgs.py` & `insights-core-3.2.0/insights/specs/datasources/rpm_pkgs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Custom datasource for CVE-2021-35937, CVE-2021-35938, and CVE-2021-35939.
 """
 import grp
 import pwd
 import signal
 
+from collections import defaultdict
+
 from insights.core.context import HostContext
 from insights.core.exceptions import SkipComponent
 from insights.core.plugins import datasource
 from insights.core.spec_factory import DatasourceProvider, simple_command
 from insights.specs import Specs
 
 
@@ -79,50 +81,47 @@
     The output is a sorted list of all packages, which have at least one directory with files
     inside, and this directory is writable by a specific user/group or the others.
 
     Raises:
         SkipComponent: Raised if no data is available
 
     Returns:
-        List[tuple[str,str,str]]: Sorted list of tuples, where every tuple contains `name`, `nevra`
-        and `vendor` for a given package.
-        E.g. [("httpd-core", "httpd-core-2.4.53-7.el9.x86_64", "Red Hat, Inc.")]
+        List[str]: Sorted list of strings, where every string contains `name`, `nevra`
+        and `vendor` for a given package, and the pipe is used as a separator.
+        E.g. ["httpd-core|httpd-core-2.4.53-7.el9.x86_64|Red Hat, Inc."]
     """
     content = broker[LocalSpecs.rpm_args].content
 
     if not content or "command not found" in content[0]:
         raise SkipComponent
 
     users = get_users()
     groups = get_groups(users)
 
-    dir_package = {}
+    dir_package = defaultdict(set)
     dirs = set()
 
     for line in content:
         pkg_name, nevra, path_name, perms, user, group, vendor = line.split("; ")
 
         if perms[0] == "d":
             user_w = user in users and perms[2] == "w"
             group_w = group in groups and perms[5] == "w"
             others_w = perms[8] == "w"
 
             if user_w or group_w or others_w:
                 # Stores a writeable directory with its package
-                if path_name not in dir_package:
-                    dir_package[path_name] = [(pkg_name, nevra, vendor)]
-                else:
-                    dir_package[path_name].append((pkg_name, nevra, vendor))
+                dir_package[path_name].add("{0}|{1}|{2}".format(pkg_name, nevra, vendor))
         else:
             # Stores a file directory
             dirs.add(path_name.rsplit('/', 1)[0])
 
     # Stores a package if its directory has files inside
-    packages = []
+    packages = set()
     for dir_path in dir_package:
         if dir_path in dirs:
-            packages.extend(dir_package[dir_path])
+            packages.update(dir_package[dir_path])
 
     if packages:
         return DatasourceProvider(
             content=sorted(packages), relative_path="insights_commands/rpm_pkgs"
         )
```

### Comparing `insights-core-3.1.9/insights/specs/datasources/sap.py` & `insights-core-3.2.0/insights/specs/datasources/sap.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/satellite_missed_queues.py` & `insights-core-3.2.0/insights/specs/datasources/satellite_missed_queues.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/semanage.py` & `insights-core-3.2.0/insights/specs/datasources/semanage.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/ssl_certificate.py` & `insights-core-3.2.0/insights/specs/datasources/ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/sys_fs_cgroup_memory.py` & `insights-core-3.2.0/insights/specs/datasources/sys_fs_cgroup_memory.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/sys_fs_cgroup_memory_tasks_number.py` & `insights-core-3.2.0/insights/specs/datasources/sys_fs_cgroup_memory_tasks_number.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/user_group.py` & `insights-core-3.2.0/insights/specs/datasources/user_group.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/datasources/yum_updates.py` & `insights-core-3.2.0/insights/specs/datasources/yum_updates.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/__init__.py` & `insights-core-3.2.0/insights/specs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,26 +7,30 @@
     alternatives_display_python = RegistryPoint()
     amq_broker = RegistryPoint(multi_output=True)
     ansible_host = RegistryPoint()
     audit_log = RegistryPoint(filterable=True)
     auditctl_rules = RegistryPoint()
     auditctl_status = RegistryPoint()
     auditd_conf = RegistryPoint()
+    audispd_conf = RegistryPoint()
     authselect_current = RegistryPoint()
     autofs_conf = RegistryPoint()
     avc_cache_threshold = RegistryPoint()
     avc_hash_stats = RegistryPoint()
     aws_instance_id_doc = RegistryPoint()
     aws_instance_id_pkcs7 = RegistryPoint()
+    aws_public_ipv4_addresses = RegistryPoint()
+    aws_public_hostnames = RegistryPoint()
     awx_manage_check_license = RegistryPoint()
     awx_manage_check_license_data = RegistryPoint(filterable=True)
     awx_manage_print_settings = RegistryPoint()
     azure_instance_id = RegistryPoint()
     azure_instance_plan = RegistryPoint()
     azure_instance_type = RegistryPoint()
+    azure_load_balancer = RegistryPoint()
     bdi_read_ahead_kb = RegistryPoint(multi_output=True)
     bios_uuid = RegistryPoint()
     blacklisted_specs = RegistryPoint()
     blkid = RegistryPoint()
     bond = RegistryPoint(multi_output=True)
     bond_dynamic_lb = RegistryPoint(multi_output=True)
     boot_loader_entries = RegistryPoint(multi_output=True)
@@ -98,14 +102,16 @@
     cron_foreman = RegistryPoint(filterable=True)
     crt = RegistryPoint()
     crypto_policies_bind = RegistryPoint()
     crypto_policies_config = RegistryPoint()
     crypto_policies_opensshserver = RegistryPoint()
     crypto_policies_state_current = RegistryPoint()
     cryptsetup_luksDump = RegistryPoint(multi_output=True)
+    cupsd_conf = RegistryPoint()
+    cups_files_conf = RegistryPoint()
     cups_ppd = RegistryPoint(multi_output=True)
     current_clocksource = RegistryPoint()
     date = RegistryPoint()
     date_iso = RegistryPoint()
     date_utc = RegistryPoint()
     db2ls_a_c = RegistryPoint()
     dcbtool_gc_dcb = RegistryPoint(multi_output=True)
@@ -127,15 +133,15 @@
     dmesg_log = RegistryPoint(filterable=True)
     dmidecode = RegistryPoint()
     dmsetup_info = RegistryPoint()
     dmsetup_status = RegistryPoint()
     dnf_conf = RegistryPoint(filterable=True)
     dnf_module_info = RegistryPoint()
     dnf_module_list = RegistryPoint()
-    dnf_modules = RegistryPoint()
+    dnf_modules = RegistryPoint(multi_output=True)
     dnsmasq_config = RegistryPoint(multi_output=True)
     docker_container_inspect = RegistryPoint(multi_output=True)
     docker_host_machine_id = RegistryPoint()
     docker_image_inspect = RegistryPoint(multi_output=True)
     docker_info = RegistryPoint()
     docker_list_containers = RegistryPoint()
     docker_list_images = RegistryPoint()
@@ -145,14 +151,15 @@
     docker_sysconfig = RegistryPoint()
     dotnet_version = RegistryPoint()
     doveconf = RegistryPoint(filterable=True)
     dracut_kdump_capture_service = RegistryPoint()
     dse_ldif = RegistryPoint(multi_output=True, filterable=True)
     du_dirs = RegistryPoint(multi_output=True, filterable=True)
     dumpe2fs_h = RegistryPoint(multi_output=True)
+    duplicate_machine_id = RegistryPoint(filterable=True)
     engine_config_all = RegistryPoint()
     engine_db_query_vdsm_version = RegistryPoint()
     engine_log = RegistryPoint(filterable=True)
     etc_journald_conf = RegistryPoint()
     etc_journald_conf_d = RegistryPoint(multi_output=True)
     etc_machine_id = RegistryPoint()
     etc_udev_40_redhat_rules = RegistryPoint(filterable=True)
@@ -187,14 +194,15 @@
     freeipa_healthcheck_log = RegistryPoint()
     fstab = RegistryPoint()
     fw_devices = RegistryPoint()
     fw_security = RegistryPoint()
     galera_cnf = RegistryPoint()
     gcp_instance_type = RegistryPoint()
     gcp_license_codes = RegistryPoint()
+    gcp_network_interfaces = RegistryPoint()
     getcert_list = RegistryPoint()
     getconf_page_size = RegistryPoint()
     getenforce = RegistryPoint()
     getsebool = RegistryPoint()
     gfs2_file_system_block_size = RegistryPoint(multi_output=True)
     glance_api_conf = RegistryPoint()
     glance_api_log = RegistryPoint(filterable=True)
@@ -261,14 +269,15 @@
     ip6tables_permanent = RegistryPoint()
     ip_addr = RegistryPoint()
     ip_addresses = RegistryPoint()
     ip_neigh_show = RegistryPoint()
     ip_netns_exec_namespace_lsof = RegistryPoint(multi_output=True, filterable=True)
     ip_route_show_table_all = RegistryPoint()
     ip_s_link = RegistryPoint()
+    ipa_default_conf = RegistryPoint()
     ipaupgrade_log = RegistryPoint(filterable=True)
     ipcs_m = RegistryPoint()
     ipcs_m_p = RegistryPoint()
     ipcs_s = RegistryPoint()
     ipcs_s_i = RegistryPoint(multi_output=True)
     ipsec_conf = RegistryPoint(filterable=True)
     iptables = RegistryPoint()
@@ -300,14 +309,15 @@
     keystone_log = RegistryPoint(filterable=True)
     kpatch_list = RegistryPoint()
     krb5 = RegistryPoint(multi_output=True)
     ksmstate = RegistryPoint()
     ktimer_lockless = RegistryPoint()
     kubepods_cpu_quota = RegistryPoint(multi_output=True)
     lastupload = RegistryPoint(multi_output=True)
+    leapp_report = RegistryPoint()
     ld_library_path_of_user = RegistryPoint()
     ldif_config = RegistryPoint(multi_output=True)
     libssh_client_config = RegistryPoint(filterable=True)
     libssh_server_config = RegistryPoint(filterable=True)
     libvirtd_log = RegistryPoint(filterable=True)
     libvirtd_qemu_log = RegistryPoint(multi_output=True, filterable=True)
     limits_conf = RegistryPoint(multi_output=True)
@@ -328,39 +338,41 @@
     ls_etc_ssh = RegistryPoint()
     ls_ipa_idoverride_memberof = RegistryPoint()
     ls_krb5_sssd = RegistryPoint()
     ls_lib_firmware = RegistryPoint()
     ls_ocp_cni_openshift_sdn = RegistryPoint()
     ls_origin_local_volumes_pods = RegistryPoint()
     ls_osroot = RegistryPoint()
+    ls_rsyslog_errorfile = RegistryPoint()
     ls_sys_firmware = RegistryPoint()
     ls_systemd_units = RegistryPoint()
     ls_tmp = RegistryPoint(filterable=True)
     ls_usr_bin = RegistryPoint(filterable=True)
     ls_usr_lib64 = RegistryPoint(filterable=True)
     ls_usr_sbin = RegistryPoint(filterable=True)
     ls_var_cache_pulp = RegistryPoint()
     ls_var_lib_mongodb = RegistryPoint()
     ls_var_lib_nova_instances = RegistryPoint()
     ls_var_lib_pcp = RegistryPoint()
+    ls_var_lib_rpm = RegistryPoint()
     ls_var_lib_rsyslog = RegistryPoint()
     ls_var_log = RegistryPoint()
     ls_var_opt_mssql = RegistryPoint()
     ls_var_opt_mssql_log = RegistryPoint()
     ls_var_run = RegistryPoint()
     ls_var_spool_clientmq = RegistryPoint()
     ls_var_spool_postfix_maildrop = RegistryPoint()
     ls_var_tmp = RegistryPoint(filterable=True)
     ls_var_www = RegistryPoint()
     lsblk = RegistryPoint()
     lsblk_pairs = RegistryPoint()
     lscpu = RegistryPoint()
     lsinitrd = RegistryPoint(filterable=True)
     lsinitrd_kdump_image = RegistryPoint(filterable=True)
-    lsinitrd_lvm_conf = RegistryPoint()
+    lsinitrd_lvm_conf = RegistryPoint(filterable=True)
     lsmod = RegistryPoint()
     lsof = RegistryPoint(filterable=True)
     lspci = RegistryPoint()
     lspci_vmmkn = RegistryPoint()
     lssap = RegistryPoint()
     lsscsi = RegistryPoint()
     luksmeta = RegistryPoint(multi_output=True)
@@ -380,16 +392,14 @@
     mdadm_E = RegistryPoint(multi_output=True)
     mdstat = RegistryPoint()
     meminfo = RegistryPoint()
     messages = RegistryPoint(filterable=True)
     metadata_json = RegistryPoint(raw=True)
     mistral_executor_log = RegistryPoint(filterable=True)
     mlx4_port = RegistryPoint(multi_output=True)
-    modinfo = RegistryPoint(multi_output=True)
-    modinfo_all = RegistryPoint()
     modinfo_filtered_modules = RegistryPoint()
     modinfo_modules = RegistryPoint(filterable=True)
     modprobe = RegistryPoint(multi_output=True)
     mokutil_sbstate = RegistryPoint()
     mongod_conf = RegistryPoint(multi_output=True, filterable=True)
     mount = RegistryPoint()
     mountinfo = RegistryPoint()
@@ -523,14 +533,15 @@
     podman_list_images = RegistryPoint()
     postconf = RegistryPoint(filterable=True)
     postconf_builtin = RegistryPoint(filterable=True)
     postgresql_conf = RegistryPoint()
     postgresql_log = RegistryPoint(multi_output=True, filterable=True)
     prev_uploader_log = RegistryPoint()
     proc_keys = RegistryPoint()
+    proc_keyusers = RegistryPoint()
     proc_netstat = RegistryPoint()
     proc_slabinfo = RegistryPoint()
     proc_snmp_ipv4 = RegistryPoint()
     proc_snmp_ipv6 = RegistryPoint()
     proc_stat = RegistryPoint()
     ps_alxwww = RegistryPoint(filterable=True)
     ps_aux = RegistryPoint(filterable=True)
@@ -566,14 +577,15 @@
     rc_local = RegistryPoint()
     rdma_conf = RegistryPoint()
     readlink_e_etc_mtab = RegistryPoint()
     readlink_e_shift_cert_client = RegistryPoint()
     readlink_e_shift_cert_server = RegistryPoint()
     recvq_socket_buffer = RegistryPoint()
     redhat_release = RegistryPoint()
+    repquota_agnpuv = RegistryPoint()
     resolv_conf = RegistryPoint()
     rhev_data_center = RegistryPoint()
     rhn_charsets = RegistryPoint()
     rhn_conf = RegistryPoint()
     rhn_entitlement_cert_xml = RegistryPoint(multi_output=True)
     rhn_hibernate_conf = RegistryPoint()
     rhn_schema_stats = RegistryPoint()
@@ -610,23 +622,23 @@
     sat5_insights_properties = RegistryPoint()
     satellite_compute_resources = RegistryPoint()
     satellite_content_hosts_count = RegistryPoint()
     satellite_core_taskreservedresource_count = RegistryPoint()
     satellite_custom_ca_chain = RegistryPoint()
     satellite_custom_hiera = RegistryPoint()
     satellite_enabled_features = RegistryPoint()
-    satellite_katello_empty_url_repositories = RegistryPoint()
     satellite_katello_repos_with_muliple_ref = RegistryPoint()
     satellite_logs_table_size = RegistryPoint()
     satellite_missed_pulp_agent_queues = RegistryPoint()
     satellite_mongodb_storage_engine = RegistryPoint()
     satellite_non_yum_type_repos = RegistryPoint()
     satellite_provision_param_settings = RegistryPoint()
     satellite_qualified_capsules = RegistryPoint()
     satellite_qualified_katello_repos = RegistryPoint()
+    satellite_rhv_hosts_count = RegistryPoint()
     satellite_sca_status = RegistryPoint()
     satellite_settings = RegistryPoint()
     satellite_version_rb = RegistryPoint()
     satellite_yaml = RegistryPoint()
     sched_rt_runtime_us = RegistryPoint()
     scheduler = RegistryPoint(multi_output=True)
     scsi = RegistryPoint()
@@ -659,14 +671,15 @@
     ssh_config_d = RegistryPoint(multi_output=True, filterable=True)
     ssh_foreman_config = RegistryPoint(filterable=True)
     ssh_foreman_proxy_config = RegistryPoint(filterable=True)
     sshd_config = RegistryPoint(filterable=True)
     sshd_config_perms = RegistryPoint()
     sssd_config = RegistryPoint()
     sssd_logs = RegistryPoint(multi_output=True, filterable=True)
+    sys_block_queue_stable_writes = RegistryPoint(multi_output=True)
     subscription_manager_facts = RegistryPoint(filterable=True)
     subscription_manager_id = RegistryPoint()
     subscription_manager_installed_product_ids = RegistryPoint(filterable=True)
     subscription_manager_list_consumed = RegistryPoint()
     subscription_manager_list_installed = RegistryPoint()
     subscription_manager_release_show = RegistryPoint()
     sudoers = RegistryPoint(multi_output=True, filterable=True)
@@ -782,13 +795,14 @@
 
     # container_specs
     container_cpu_online = RegistryPoint(multi_output=True)
     container_cpuset_cpus = RegistryPoint(multi_output=True)
     container_dotnet_version = RegistryPoint(multi_output=True)
     container_installed_rpms = RegistryPoint(multi_output=True)
     container_inspect_keys = RegistryPoint(filterable=True)
+    container_mssql_api_assessment = RegistryPoint(multi_output=True)
     container_nginx_conf = RegistryPoint(multi_output=True)
     container_nginx_error_log = RegistryPoint(multi_output=True, filterable=True)
     container_ps_aux = RegistryPoint(multi_output=True, filterable=True)
     container_redhat_release = RegistryPoint(multi_output=True)
     container_vsftpd_conf = RegistryPoint(multi_output=True, filterable=True)
     containers_inspect = RegistryPoint()
```

### Comparing `insights-core-3.1.9/insights/specs/core3_archive.py` & `insights-core-3.2.0/insights/specs/core3_archive.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/default.py` & `insights-core-3.2.0/insights/specs/default.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 data sources that standard Insights `Parsers` resolve against.
 """
 
 import logging
 import signal
 
 from insights.core.context import HostContext
-from insights.core.spec_factory import RawFileProvider
+from insights.core.spec_factory import MetadataProvider
 from insights.core.spec_factory import simple_file, simple_command, glob_file, head
 from insights.core.spec_factory import first_of, command_with_args
 from insights.core.spec_factory import foreach_collect, foreach_execute
 from insights.core.spec_factory import container_collect, container_execute
 from insights.core.spec_factory import first_file, listdir
 from insights.components.cloud_provider import IsAzure, IsGCP
 from insights.components.ceph import IsCephMonitor
 from insights.components.virtualization import IsBareMetal
-from insights.components.satellite import IsCapsule, IsSatellite611, IsSatellite
+from insights.components.satellite import IsSatellite611, IsSatellite
 from insights.specs import Specs
 from insights.specs.datasources import (
     aws, awx_manage, cloud_init, candlepin_broker, corosync as corosync_ds,
-    dir_list, ethernet, httpd, ipcs, kernel_module_list, lpstat, md5chk,
-    package_provides, ps as ps_datasource, sap, satellite_missed_queues,
-    semanage, ssl_certificate, sys_fs_cgroup_memory, sys_fs_cgroup_memory_tasks_number,
-    rpm_pkgs, user_group, yum_updates, luks_devices)
+    dir_list, ethernet, httpd, ipcs, kernel_module_list, leapp, lpstat,
+    machine_ids, md5chk, package_provides, ps as ps_datasource, sap,
+    satellite_missed_queues, semanage, ssl_certificate, sys_fs_cgroup_memory,
+    sys_fs_cgroup_memory_tasks_number, rpm_pkgs, user_group, yum_updates,
+    luks_devices)
 from insights.specs.datasources.sap import sap_hana_sid, sap_hana_sid_SID_nr
 from insights.specs.datasources.pcp import pcp_enabled, pmlog_summary_args
 from insights.specs.datasources.container import running_rhel_containers, containers_inspect
 from insights.specs.datasources.container.nginx_conf import nginx_conf as container_nginx_conf_ds
 
 
 logger = logging.getLogger(__name__)
@@ -52,53 +53,68 @@
             '"vendor":"%{VENDOR}"',
             '"buildhost":"%{BUILDHOST}"',
             '"sigpgp":"%{SIGPGP:pgpsig}"'
         ]
     return "\{" + ",".join(fmt) + "\}\n"
 
 
-_etc_and_sub_dirs = sorted(["/etc", "/etc/pki/tls/private", "/etc/pki/tls/certs",
-                           "/etc/pki/ovirt-vmconsole", "/etc/nova/migration", "/etc/sysconfig",
-                           "/etc/cloud/cloud.cfg.d", "/etc/rc.d/init.d"])
+_etc_and_sub_dirs = sorted(
+    [
+        "/etc", "/etc/pki/tls/private", "/etc/pki/tls/certs",
+        "/etc/pki/ovirt-vmconsole", "/etc/nova/migration", "/etc/sysconfig",
+        "/etc/cloud/cloud.cfg.d", "/etc/rc.d/init.d", "/etc/selinux/targeted/policy",
+        "/etc/watchdog.d/"
+    ])
 """ List of directories for spec `ls_etc` """
 _rpm_format = _make_rpm_formatter()
 """ Query format for specs `installed_rpms` and `container_installed_rpms` """
 
 
 class DefaultSpecs(Specs):
     # Dep specs that aren't in the registry
     block_devices_by_uuid = listdir("/dev/disk/by-uuid/", context=HostContext)
     httpd_pid = simple_command("/usr/bin/pgrep -o httpd")
     openshift_router_pid = simple_command("/usr/bin/pgrep -n openshift-route")
     ovs_vsctl_list_br = simple_command("/usr/bin/ovs-vsctl list-br")
 
+    # Archive metadata specs/files
+    ansible_host = simple_file("/ansible_host", kind=MetadataProvider)
+    blacklisted_specs = first_file(["/blacklisted_specs", "/blacklisted_specs.txt"], kind=MetadataProvider)
+    branch_info = simple_file("/branch_info", kind=MetadataProvider)
+    display_name = simple_file("/display_name", kind=MetadataProvider)
+    tags = simple_file("/tags.json", kind=MetadataProvider)
+    version_info = simple_file("/version_info", kind=MetadataProvider)
+
     # Regular collection specs
     abrt_ccpp_conf = simple_file("/etc/abrt/plugins/CCpp.conf")
     abrt_status_bare = simple_command("/usr/bin/abrt status --bare=True")
     alternatives_display_python = simple_command("/usr/sbin/alternatives --display python")
     amq_broker = glob_file("/var/opt/amq-broker/*/etc/broker.xml")
     audit_log = simple_file("/var/log/audit/audit.log")
     auditctl_rules = simple_command("/sbin/auditctl -l")
     auditctl_status = simple_command("/sbin/auditctl -s")
     auditd_conf = simple_file("/etc/audit/auditd.conf")
+    audispd_conf = simple_file("/etc/audisp/audispd.conf")
     aws_instance_id_doc = command_with_args('/usr/bin/curl -s -H "X-aws-ec2-metadata-token: %s" http://169.254.169.254/latest/dynamic/instance-identity/document --connect-timeout 5', aws.aws_imdsv2_token, deps=[aws.aws_imdsv2_token])
     aws_instance_id_pkcs7 = command_with_args('/usr/bin/curl -s -H "X-aws-ec2-metadata-token: %s" http://169.254.169.254/latest/dynamic/instance-identity/pkcs7 --connect-timeout 5', aws.aws_imdsv2_token, deps=[aws.aws_imdsv2_token])
+    aws_public_ipv4_addresses = command_with_args('/usr/bin/curl -s -H "X-aws-ec2-metadata-token: %s" http://169.254.169.254/latest/meta-data/public-ipv4 --connect-timeout 5', aws.aws_imdsv2_token, deps=[aws.aws_imdsv2_token])
+    aws_public_hostnames = command_with_args('/usr/bin/curl -s -H "X-aws-ec2-metadata-token: %s" http://169.254.169.254/latest/meta-data/public-hostname --connect-timeout 5', aws.aws_imdsv2_token, deps=[aws.aws_imdsv2_token])
     awx_manage_check_license = simple_command("/usr/bin/awx-manage check_license")
     awx_manage_check_license_data = awx_manage.awx_manage_check_license_data_datasource
     awx_manage_print_settings = simple_command("/usr/bin/awx-manage print_settings INSIGHTS_TRACKING_STATE SYSTEM_UUID INSTALL_UUID TOWER_URL_BASE AWX_CLEANUP_PATHS AWX_PROOT_BASE_PATH LOG_AGGREGATOR_ENABLED LOG_AGGREGATOR_LEVEL --format json")
     azure_instance_id = simple_command("/usr/bin/curl -s -H Metadata:true http://169.254.169.254/metadata/instance/compute/vmId?api-version=2021-12-13&format=text --connect-timeout 5", deps=[IsAzure])
     azure_instance_plan = simple_command("/usr/bin/curl -s -H Metadata:true http://169.254.169.254/metadata/instance/compute/plan?api-version=2021-12-13&format=json --connect-timeout 5", deps=[IsAzure])
     azure_instance_type = simple_command("/usr/bin/curl -s -H Metadata:true http://169.254.169.254/metadata/instance/compute/vmSize?api-version=2021-12-13&format=text --connect-timeout 5", deps=[IsAzure])
+    azure_load_balancer = simple_command("/usr/bin/curl -s -H Metadata:true http://169.254.169.254/metadata/loadbalancer?api-version=2021-12-13&format=json --connect-timeout 5", deps=[IsAzure])
     bdi_read_ahead_kb = glob_file("/sys/class/bdi/*/read_ahead_kb")
     bios_uuid = simple_command("/usr/sbin/dmidecode -s system-uuid")
     blkid = simple_command("/sbin/blkid -c /dev/null")
     bond = glob_file("/proc/net/bonding/*")
     bond_dynamic_lb = glob_file("/sys/class/net/*/bonding/tlb_dynamic_lb")
     boot_loader_entries = glob_file("/boot/loader/entries/*.conf")
-    branch_info = simple_file("/branch_info", kind=RawFileProvider)
     brctl_show = simple_command("/usr/sbin/brctl show")
     candlepin_broker = candlepin_broker.candlepin_broker
     cciss = glob_file("/proc/driver/cciss/cciss*")
     cdc_wdm = simple_file("/sys/bus/usb/drivers/cdc_wdm/module/refcnt")
     ceilometer_compute_log = first_file(["/var/log/containers/ceilometer/compute.log", "/var/log/ceilometer/compute.log"])
     ceph_conf = first_file(["/var/lib/config-data/puppet-generated/ceph/etc/ceph/ceph.conf", "/etc/ceph/ceph.conf"])
     ceph_df_detail = simple_command("/usr/bin/ceph df detail -f json")
@@ -138,14 +154,16 @@
     cron_daily_rhsmd = simple_file("/etc/cron.daily/rhsmd")
     cron_foreman = simple_file("/etc/cron.d/foreman")
     crypto_policies_bind = simple_file("/etc/crypto-policies/back-ends/bind.config")
     crypto_policies_config = simple_file("/etc/crypto-policies/config")
     crypto_policies_opensshserver = simple_file("/etc/crypto-policies/back-ends/opensshserver.config")
     crypto_policies_state_current = simple_file("/etc/crypto-policies/state/current")
     cryptsetup_luksDump = luks_devices.luks_data_sources
+    cupsd_conf = simple_file("/etc/cups/cupsd.conf")
+    cups_files_conf = simple_file("/etc/cups/cups-files.conf")
     cups_ppd = glob_file("etc/cups/ppd/*")
     current_clocksource = simple_file("/sys/devices/system/clocksource/clocksource0/current_clocksource")
     date = simple_command("/bin/date")
     date_utc = simple_command("/bin/date --utc")
     db2ls_a_c = simple_command("/usr/local/bin/db2ls -a -c")
     designate_conf = first_file(["/var/lib/config-data/puppet-generated/designate/etc/designate/designate.conf",
                                  "/etc/designate/designate.conf"])
@@ -160,24 +178,26 @@
     dmesg = simple_command("/bin/dmesg")
     dmesg_log = simple_file("/var/log/dmesg")
     dmidecode = simple_command("/usr/sbin/dmidecode")
     dmsetup_info = simple_command("/usr/sbin/dmsetup info -C")
     dmsetup_status = simple_command("/usr/sbin/dmsetup status")
     dnf_conf = simple_file("/etc/dnf/dnf.conf")
     dnf_modules = glob_file("/etc/dnf/modules.d/*.module")
+    dnf_module_list = simple_command("/usr/bin/dnf -C --noplugins module list")
     docker_info = simple_command("/usr/bin/docker info")
     docker_list_containers = simple_command("/usr/bin/docker ps --all --no-trunc")
     docker_list_images = simple_command("/usr/bin/docker images --all --no-trunc --digests")
     docker_storage_setup = simple_file("/etc/sysconfig/docker-storage-setup")
     docker_sysconfig = simple_file("/etc/sysconfig/docker")
     dotnet_version = simple_command("/usr/bin/dotnet --version")
     doveconf = simple_command("/usr/bin/doveconf")
     dracut_kdump_capture_service = simple_file("/usr/lib/dracut/modules.d/99kdumpbase/kdump-capture.service")
     dse_ldif = glob_file("/etc/dirsrv/*/dse.ldif")
     du_dirs = foreach_execute(dir_list.du_dir_list, "/bin/du -s -k %s")
+    duplicate_machine_id = machine_ids.dup_machine_id_info
     engine_log = simple_file("/var/log/ovirt-engine/engine.log")
     etc_journald_conf = simple_file(r"etc/systemd/journald.conf")
     etc_journald_conf_d = glob_file(r"etc/systemd/journald.conf.d/*.conf")
     etc_machine_id = simple_file("/etc/machine-id")
     etc_udev_40_redhat_rules = first_file(["/etc/udev/rules.d/40-redhat.rules", "/run/udev/rules.d/40-redhat.rules",
                                        "/usr/lib/udev/rules.d/40-redhat.rules", "/usr/local/lib/udev/rules.d/40-redhat.rules"])
     etc_udev_oracle_asm_rules = glob_file(r"/etc/udev/rules.d/*asm*.rules")
@@ -195,16 +215,17 @@
     firewall_cmd_list_all_zones = simple_command("/usr/bin/firewall-cmd --list-all-zones")
     firewalld_conf = simple_file("/etc/firewalld/firewalld.conf")
     foreman_production_log = simple_file("/var/log/foreman/production.log")
     fstab = simple_file("/etc/fstab")
     fw_devices = simple_command("/bin/fwupdagent get-devices", deps=[IsBareMetal])
     fw_security = simple_command("/bin/fwupdagent security --force", deps=[IsBareMetal])
     galera_cnf = first_file(["/var/lib/config-data/puppet-generated/mysql/etc/my.cnf.d/galera.cnf", "/etc/my.cnf.d/galera.cnf"])
-    gcp_instance_type = simple_command("/usr/bin/curl -s -H 'Metadata-Flavor: Google' http://metadata.google.internal/computeMetadata/v1/instance/machine-type --connect-timeout 5", deps=[IsGCP])
-    gcp_license_codes = simple_command("/usr/bin/curl -s -H 'Metadata-Flavor: Google' http://metadata.google.internal/computeMetadata/v1/instance/licenses/?recursive=True --connect-timeout 5", deps=[IsGCP])
+    gcp_instance_type = simple_command("/usr/bin/curl -s -H 'Metadata-Flavor: Google' 'http://metadata.google.internal/computeMetadata/v1/instance/machine-type' --connect-timeout 5", deps=[IsGCP])
+    gcp_license_codes = simple_command("/usr/bin/curl -s -H 'Metadata-Flavor: Google' 'http://metadata.google.internal/computeMetadata/v1/instance/licenses/?recursive=True' --connect-timeout 5", deps=[IsGCP])
+    gcp_network_interfaces = simple_command("/usr/bin/curl -s -H 'Metadata-Flavor: Google' 'http://metadata/computeMetadata/v1/instance/network-interfaces/?recursive=true' --connect-timeout 5", deps=[IsGCP])
     getcert_list = simple_command("/usr/bin/getcert list")
     getconf_page_size = simple_command("/usr/bin/getconf PAGE_SIZE")
     getenforce = simple_command("/usr/sbin/getenforce")
     getsebool = simple_command("/usr/sbin/getsebool -a")
     gluster_v_info = simple_command("/usr/sbin/gluster volume info")
     gnocchi_conf = first_file(["/var/lib/config-data/puppet-generated/gnocchi/etc/gnocchi/gnocchi.conf", "/etc/gnocchi/gnocchi.conf"])
     gnocchi_metricd_log = first_file(["/var/log/containers/gnocchi/gnocchi-metricd.log", "/var/log/gnocchi/metricd.log"])
@@ -269,14 +290,15 @@
     installed_rpms = simple_command("/bin/rpm -qa --qf '%s'" % _rpm_format, context=HostContext, signum=signal.SIGTERM)
     interrupts = simple_file("/proc/interrupts")
     ip6tables = simple_command("/sbin/ip6tables-save")
     ip_addr = simple_command("/sbin/ip addr")
     ip_addresses = simple_command("/bin/hostname -I")
     ip_route_show_table_all = simple_command("/sbin/ip route show table all")
     ip_s_link = simple_command("/sbin/ip -s -d link")
+    ipa_default_conf = simple_file("/etc/ipa/default.conf")
     ipaupgrade_log = simple_file("/var/log/ipaupgrade.log")
     ipcs_m = simple_command("/usr/bin/ipcs -m")
     ipcs_m_p = simple_command("/usr/bin/ipcs -m -p")
     ipcs_s = simple_command("/usr/bin/ipcs -s")
     ipcs_s_i = foreach_execute(ipcs.semid, "/usr/bin/ipcs -s -i %s")
     ipsec_conf = simple_file("/etc/ipsec.conf")
     iptables = simple_command("/sbin/iptables-save")
@@ -293,14 +315,15 @@
     kernel_crash_kexec_post_notifiers = simple_file("/sys/module/kernel/parameters/crash_kexec_post_notifiers")
     kexec_crash_size = simple_file("/sys/kernel/kexec_crash_size")
     keystone_crontab = simple_file("/var/spool/cron/keystone")
     kpatch_list = simple_command("/usr/sbin/kpatch list")
     krb5 = glob_file([r"etc/krb5.conf", r"etc/krb5.conf.d/*"])
     ksmstate = simple_file("/sys/kernel/mm/ksm/run")
     lastupload = glob_file(["/etc/redhat-access-insights/.lastupload", "/etc/insights-client/.lastupload"])
+    leapp_report = leapp.leapp_report
     ld_library_path_of_user = sap.ld_library_path_of_user
     ldif_config = glob_file("/etc/dirsrv/slapd-*/dse.ldif")
     libssh_client_config = simple_file("/etc/libssh/libssh_client.config")
     libssh_server_config = simple_file("/etc/libssh/libssh_server.config")
     libvirtd_log = simple_file("/var/log/libvirt/libvirtd.log")
     limits_conf = glob_file(["/etc/security/limits.conf", "/etc/security/limits.d/*.conf"])
     localtime = simple_command("/usr/bin/file -L /etc/localtime")
@@ -328,14 +351,15 @@
     ls_tmp = simple_command("/bin/ls -la /tmp")
     ls_usr_bin = simple_command("/bin/ls -lan /usr/bin")
     ls_usr_lib64 = simple_command("/bin/ls -lan /usr/lib64")
     ls_var_cache_pulp = simple_command("/bin/ls -lan /var/cache/pulp")
     ls_var_lib_mongodb = simple_command("/bin/ls -la /var/lib/mongodb")
     ls_var_lib_nova_instances = simple_command("/bin/ls -laRZ /var/lib/nova/instances")
     ls_var_lib_pcp = simple_command("/bin/ls -la /var/lib/pcp")
+    ls_var_lib_rpm = simple_command("/bin/ls -lan /var/lib/rpm")
     ls_var_lib_rsyslog = simple_command("/bin/ls -lZ /var/lib/rsyslog")
     ls_var_log = simple_command("/bin/ls -la /var/log /var/log/audit")
     ls_var_opt_mssql = simple_command("/bin/ls -ld /var/opt/mssql")
     ls_var_opt_mssql_log = simple_command("/bin/ls -la /var/opt/mssql/log")
     ls_var_run = simple_command("/bin/ls -lnL /var/run")
     ls_var_spool_clientmq = simple_command("/bin/ls -ln /var/spool/clientmqueue")
     ls_var_spool_postfix_maildrop = simple_command("/bin/ls -ln /var/spool/postfix/maildrop")
@@ -477,14 +501,15 @@
     postgresql_log = first_of(
         [
             glob_file("/var/opt/rh/rh-postgresql12/lib/pgsql/data/log/postgresql-*.log"),
             glob_file("/var/lib/pgsql/data/pg_log/postgresql-*.log"),
         ]
     )
     proc_keys = simple_file("/proc/keys")
+    proc_keyusers = simple_file("/proc/key-users")
     proc_netstat = simple_file("proc/net/netstat")
     proc_slabinfo = simple_file("proc/slabinfo")
     proc_snmp_ipv4 = simple_file("proc/net/snmp")
     proc_snmp_ipv6 = simple_file("proc/net/snmp6")
     proc_stat = simple_file("proc/stat")
     ps_alxwww = simple_command("/bin/ps alxwww")
     ps_aux = simple_command("/bin/ps aux")
@@ -503,20 +528,21 @@
     rabbitmq_env = simple_file("/etc/rabbitmq/rabbitmq-env.conf")
     rabbitmq_report = simple_command("/usr/sbin/rabbitmqctl report")
     rc_local = simple_file("/etc/rc.d/rc.local")
     readlink_e_etc_mtab = simple_command("/usr/bin/readlink -e /etc/mtab")
     readlink_e_shift_cert_client = simple_command("/usr/bin/readlink -e /etc/origin/node/certificates/kubelet-client-current.pem")
     readlink_e_shift_cert_server = simple_command("/usr/bin/readlink -e /etc/origin/node/certificates/kubelet-server-current.pem")
     redhat_release = simple_file("/etc/redhat-release")
+    repquota_agnpuv = simple_command("/usr/sbin/repquota -agnpuv")
     resolv_conf = simple_file("/etc/resolv.conf")
     rhsm_conf = simple_file("/etc/rhsm/rhsm.conf")
     rhsm_releasever = simple_file('/var/lib/rhsm/cache/releasever.json')
     rndc_status = simple_command("/usr/sbin/rndc status")
     ros_config = simple_file("/var/lib/pcp/config/pmlogger/config.ros")
-    rpm_V_packages = simple_command("/bin/rpm -V coreutils procps procps-ng shadow-utils passwd sudo chrony", keep_rc=True, signum=signal.SIGTERM)
+    rpm_V_packages = simple_command("/bin/rpm -V coreutils procps procps-ng shadow-utils passwd sudo chrony findutils", keep_rc=True, signum=signal.SIGTERM)
     rpm_ostree_status = simple_command("/usr/bin/rpm-ostree status --json", signum=signal.SIGTERM)
     rpm_pkgs = rpm_pkgs.pkgs_with_writable_dirs
     rsyslog_conf = glob_file(["/etc/rsyslog.conf", "/etc/rsyslog.d/*.conf"])
     samba = simple_file("/etc/samba/smb.conf")
     sap_hana_landscape = foreach_execute(sap_hana_sid_SID_nr, "/bin/su -l %sadm -c 'python /usr/sap/%s/HDB%s/exe/python_support/landscapeHostConfiguration.py'", keep_rc=True)
     sap_hdb_version = foreach_execute(sap_hana_sid, "/bin/su -l %sadm -c 'HDB version'", keep_rc=True)
     saphostctl_getcimobject_sapinstance = simple_command("/usr/sap/hostctrl/exe/saphostctrl -function GetCIMObject -enuminstances SAPInstance")
@@ -526,51 +552,38 @@
         "/usr/bin/sudo -iu postgres /usr/bin/psql -d foreman -c 'select name, type from compute_resources' --csv",
         deps=[IsSatellite]
     )
     satellite_content_hosts_count = simple_command(
         "/usr/bin/sudo -iu postgres /usr/bin/psql -d foreman -c 'select count(*) from hosts'",
         deps=[IsSatellite]
     )
-    satellite_core_taskreservedresource_count = simple_command(
-        "/usr/bin/sudo -iu postgres /usr/bin/psql -d pulpcore -c 'select count(*) from core_taskreservedresource' --csv",
-        deps=[IsSatellite]
-    )
     satellite_custom_ca_chain = simple_command(
         '/usr/bin/awk \'BEGIN { pipe="openssl x509 -noout -subject -enddate"} /^-+BEGIN CERT/,/^-+END CERT/ { print | pipe } /^-+END CERT/ { close(pipe); printf("\\n")}\' /etc/pki/katello/certs/katello-server-ca.crt',
     )
     satellite_custom_hiera = simple_file("/etc/foreman-installer/custom-hiera.yaml")
     satellite_enabled_features = simple_command("/usr/bin/curl -sk https://localhost:9090/features --connect-timeout 5", deps=[IsSatellite])
-    satellite_katello_repos_with_muliple_ref = simple_command(
-        '/usr/bin/sudo -iu postgres /usr/bin/psql -d foreman -c "select repository_href, count(*) from katello_repository_references group by repository_href having count(*) > 1;" --csv',
-        deps=[IsSatellite]
-    )
     satellite_logs_table_size = simple_command(
         "/usr/bin/sudo -iu postgres /usr/bin/psql -d foreman -c \"select pg_total_relation_size('logs') as logs_size\" --csv",
         deps=[IsSatellite]
     )
     satellite_missed_pulp_agent_queues = satellite_missed_queues.satellite_missed_pulp_agent_queues
-    satellite_mongodb_storage_engine = simple_command("/usr/bin/mongo pulp_database --eval 'db.serverStatus().storageEngine'")
-    satellite_non_yum_type_repos = simple_command(
-        "/usr/bin/mongo pulp_database --eval 'db.repo_importers.find({\"importer_type_id\": { $ne: \"yum_importer\"}}).count()'",
-        deps=[[IsSatellite, IsCapsule]]
-    )
     satellite_provision_param_settings = simple_command(
         "/usr/bin/sudo -iu postgres /usr/bin/psql -d foreman -c \"select name, value from parameters where name='package_upgrade' and reference_id in (select id from operatingsystems where name='RedHat' and major='9')\" --csv",
         deps=[IsSatellite611]
     )
     satellite_qualified_capsules = simple_command(
         "/usr/bin/sudo -iu postgres /usr/bin/psql -d foreman -c \"select name from smart_proxies where download_policy = 'background'\" --csv",
         deps=[IsSatellite]
     )
     satellite_qualified_katello_repos = simple_command(
         "/usr/bin/sudo -iu postgres /usr/bin/psql -d foreman -c \"select id, name, url, download_policy from katello_root_repositories where download_policy = 'background' or url is NULL\" --csv",
         deps=[IsSatellite]
     )
-    satellite_sca_status = simple_command(
-        "/usr/bin/sudo -iu postgres /usr/bin/psql -d candlepin -c \"select displayname,content_access_mode from cp_owner\" --csv",
+    satellite_rhv_hosts_count = simple_command(
+        "/usr/bin/sudo -iu postgres /usr/bin/psql -d foreman -c \"select count(*) from hosts where \"compute_resource_id\" in (select id from compute_resources where type='Foreman::Model::Ovirt')\" --csv",
         deps=[IsSatellite]
     )
     satellite_settings = simple_command(
         "/usr/bin/sudo -iu postgres /usr/bin/psql -d foreman -c \"select name, value, \\\"default\\\" from settings where name in ('destroy_vm_on_host_delete', 'unregister_delete_host')\" --csv",
         deps=[IsSatellite]
     )
     satellite_version_rb = simple_file("/usr/share/foreman/lib/satellite/version.rb")
@@ -605,14 +618,15 @@
                                                 override_env={"LC_ALL": "C.UTF-8"})
     subscription_manager_id = simple_command("/usr/sbin/subscription-manager identity",  # use "/usr/sbin" here, BZ#1690529
                                              override_env={"LC_ALL": "C.UTF-8"})
     subscription_manager_installed_product_ids = simple_command("/usr/bin/find /etc/pki/product-default/ /etc/pki/product/ -name '*pem' -exec rct cat-cert --no-content '{}' \;")
     sudoers = glob_file(["/etc/sudoers", "/etc/sudoers.d/*"])
     swift_object_expirer_conf = first_file(["/var/lib/config-data/puppet-generated/swift/etc/swift/object-expirer.conf", "/etc/swift/object-expirer.conf"])
     swift_proxy_server_conf = first_file(["/var/lib/config-data/puppet-generated/swift/etc/swift/proxy-server.conf", "/etc/swift/proxy-server.conf"])
+    sys_block_queue_stable_writes = glob_file("/sys/block/*/queue/stable_writes")
     sys_fs_cgroup_memory_tasks_number = sys_fs_cgroup_memory_tasks_number.sys_fs_cgroup_memory_tasks_number_data_datasource
     sys_fs_cgroup_uniq_memory_swappiness = sys_fs_cgroup_memory.sys_fs_cgroup_uniq_memory_swappiness
     sys_vmbus_class_id = glob_file('/sys/bus/vmbus/devices/*/class_id')
     sys_vmbus_device_id = glob_file('/sys/bus/vmbus/devices/*/device_id')
     sysconfig_grub = simple_file("/etc/default/grub")  # This is the file where the "/etc/sysconfig/grub" point to
     sysconfig_kdump = simple_file("etc/sysconfig/kdump")
     sysconfig_libvirt_guests = simple_file("etc/sysconfig/libvirt-guests")
@@ -627,24 +641,24 @@
     sysctl_d_conf_etc = glob_file("/etc/sysctl.d/*.conf")
     sysctl_d_conf_usr = glob_file("/usr/lib/sysctl.d/*.conf")
     systemctl_cat_rpcbind_socket = simple_command("/bin/systemctl cat rpcbind.socket")
     systemctl_list_unit_files = simple_command("/bin/systemctl list-unit-files")
     systemctl_list_units = simple_command("/bin/systemctl list-units")
     systemctl_show_all_services = simple_command("/bin/systemctl show *.service")
     systemctl_show_target = simple_command("/bin/systemctl show *.target")
+    systemctl_status_all = simple_command("/bin/systemctl status --all")
     systemd_analyze_blame = simple_command("/bin/systemd-analyze blame")
     systemd_docker = simple_command("/usr/bin/systemctl cat docker.service")
     systemd_logind_conf = simple_file("/etc/systemd/logind.conf")
     systemd_openshift_node = simple_command("/usr/bin/systemctl cat atomic-openshift-node.service")
     systemd_system_conf = simple_file("/etc/systemd/system.conf")
     systemid = first_of([
         simple_file("/etc/sysconfig/rhn/systemid"),
         simple_file("/conf/rhn/sysconfig/rhn/systemid")
     ])
-    tags = simple_file("/tags.json", kind=RawFileProvider)
     teamdctl_config_dump = foreach_execute(ethernet.team_interfaces, "/usr/bin/teamdctl %s config dump")
     teamdctl_state_dump = foreach_execute(ethernet.team_interfaces, "/usr/bin/teamdctl %s state dump")
     testparm_s = simple_command("/usr/bin/testparm -s")
     testparm_v_s = simple_command("/usr/bin/testparm -v -s")
     thp_enabled = simple_file("/sys/kernel/mm/transparent_hugepage/enabled")
     thp_use_zero_page = simple_file("/sys/kernel/mm/transparent_hugepage/use_zero_page")
     timedatectl_status = simple_command('/usr/bin/timedatectl status')
@@ -656,15 +670,14 @@
     up2date = simple_file("/etc/sysconfig/rhn/up2date")
     up2date_log = simple_file("/var/log/up2date")
     uptime = simple_command("/usr/bin/uptime")
     users_count_map_selinux_user = semanage.users_count_map_selinux_user
     usr_journald_conf_d = glob_file(r"usr/lib/systemd/journald.conf.d/*.conf")  # note that etc_journald.conf.d also exists
     vdo_status = simple_command("/usr/bin/vdo status")
     vdsm_log = simple_file("var/log/vdsm/vdsm.log")
-    version_info = simple_file("/version_info")
     vgdisplay = simple_command("/sbin/vgdisplay")
     vgs_noheadings = simple_command("/sbin/vgs --nameprefixes --noheadings --separator='|' -a -o vg_all --config=\"global{locking_type=0}\"")
     virsh_list_all = simple_command("/usr/bin/virsh --readonly list --all")
     virt_what = simple_command("/usr/sbin/virt-what")
     virtlogd_conf = simple_file("/etc/libvirt/virtlogd.conf")
     vma_ra_enabled = simple_file("/sys/kernel/mm/swap/vma_ra_enabled")
     vsftpd = simple_file("/etc/pam.d/vsftpd")
@@ -685,13 +698,14 @@
     zipl_conf = simple_file("/etc/zipl.conf")
 
     # Container collection specs
     container_cpu_online = container_collect(running_rhel_containers, "/sys/devices/system/cpu/online")
     container_cpuset_cpus = container_collect(running_rhel_containers, "/sys/fs/cgroup/cpuset/cpuset.cpus")
     container_dotnet_version = container_execute(running_rhel_containers, "/usr/bin/dotnet --version")
     container_installed_rpms = container_execute(running_rhel_containers, "/usr/bin/rpm -qa --qf '%s'" % _rpm_format, context=HostContext, signum=signal.SIGTERM)
+    container_mssql_api_assessment = container_collect(running_rhel_containers, "/var/opt/mssql/log/assessments/assessment-latest")
     container_nginx_conf = container_collect(container_nginx_conf_ds)
     container_nginx_error_log = container_collect(running_rhel_containers, "/var/log/nginx/error.log")
     container_ps_aux = container_execute(running_rhel_containers, "/bin/ps aux")
     container_redhat_release = container_collect(running_rhel_containers, "/etc/redhat-release")
     container_vsftpd_conf = container_collect(running_rhel_containers, "/etc/vsftpd/vsftpd.conf")
     containers_inspect = containers_inspect.containers_inspect_data_datasource
```

### Comparing `insights-core-3.1.9/insights/specs/insights_archive.py` & `insights-core-3.2.0/insights/specs/insights_archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,24 @@
 
 
 class InsightsArchiveSpecs(Specs):
 
     abrt_status_bare = simple_file("insights_commands/abrt_status_--bare_True")
     all_installed_rpms = glob_file("insights_commands/rpm_-qa*")
     alternatives_display_python = simple_file("insights_commands/alternatives_--display_python")
-    ansible_host = simple_file("ansible_host")
     auditctl_rules = simple_file("insights_commands/auditctl_-l")
     auditctl_status = simple_file("insights_commands/auditctl_-s")
     aws_instance_id_doc = simple_file("insights_commands/python_-m_insights.tools.cat_--no-header_aws_instance_id_doc")
     aws_instance_id_pkcs7 = simple_file("insights_commands/python_-m_insights.tools.cat_--no-header_aws_instance_id_pkcs7")
     awx_manage_check_license = simple_file("insights_commands/awx-manage_check_license")
     awx_manage_print_settings = simple_file("insights_commands/awx-manage_print_settings_INSIGHTS_TRACKING_STATE_SYSTEM_UUID_INSTALL_UUID_TOWER_URL_BASE_AWX_CLEANUP_PATHS_AWX_PROOT_BASE_PATH_LOG_AGGREGATOR_ENABLED_LOG_AGGREGATOR_LEVEL_--format_json")
     azure_instance_id = simple_file("insights_commands/python_-m_insights.tools.cat_--no-header_azure_instance_id")
     azure_instance_type = simple_file("insights_commands/python_-m_insights.tools.cat_--no-header_azure_instance_type")
     azure_instance_plan = simple_file("insights_commands/python_-m_insights.tools.cat_--no-header_azure_instance_plan")
     bios_uuid = simple_file("insights_commands/dmidecode_-s_system-uuid")
-    blacklisted_specs = simple_file("blacklisted_specs.txt")
     blkid = simple_file("insights_commands/blkid_-c_.dev.null")
     brctl_show = simple_file("insights_commands/brctl_show")
     ceph_df_detail = first_file(["insights_commands/ceph_df_detail_-f_json-pretty", "insights_commands/ceph_df_detail_-f_json"])
     ceph_health_detail = first_file(["insights_commands/ceph_health_detail_-f_json-pretty", "insights_commands/ceph_health_detail_-f_json"])
     ceph_insights = simple_file("insights_commands/python_-m_insights.tools.cat_--no-header_ceph_insights")
     ceph_osd_dump = first_file(["insights_commands/ceph_osd_dump_-f_json-pretty", "insights_commands/ceph_osd_dump_-f_json"])
     ceph_osd_tree = first_file(["insights_commands/ceph_osd_tree_-f_json-pretty", "insights_commands/ceph_osd_tree_-f_json"])
@@ -49,14 +47,15 @@
     df__al = first_file(["insights_commands/df_-al_-x_autofs", "insights_commands/df_-al"])
     df__alP = first_file(["insights_commands/df_-alP_-x_autofs", "insights_commands/df_-alP"])
     df__li = first_file(["insights_commands/df_-li_-x_autofs", "insights_commands/df_-li"])
     dig_dnssec = simple_file("insights_commands/dig_dnssec_._SOA")
     dig_edns = simple_file("insights_commands/dig_edns_0_._SOA")
     dig_noedns = simple_file("insights_commands/dig_noedns_._SOA")
     display_name = simple_file("display_name")
+    dnf_module_list = simple_file("insights_commands/dnf_-C_--noplugins_module_list")
     dmesg = simple_file("insights_commands/dmesg")
     dmidecode = simple_file("insights_commands/dmidecode")
     dmsetup_info = simple_file("insights_commands/dmsetup_info_-C")
     dmsetup_status = simple_file("insights_commands/dmsetup_status")
     docker_info = simple_file("insights_commands/docker_info")
     docker_list_containers = simple_file("insights_commands/docker_ps_--all_--no-trunc")
     docker_list_images = simple_file("insights_commands/docker_images_--all_--no-trunc_--digests")
@@ -117,15 +116,15 @@
     localtime = simple_file("insights_commands/file_-L_.etc.localtime")
     losetup = simple_file("insights_commands/losetup_-l")
     lpstat_p = simple_file("insights_commands/lpstat_-p")
     ls_boot = simple_file("insights_commands/ls_-lanR_.boot")
     ls_dev = simple_file("insights_commands/ls_-lanR_.dev")
     ls_disk = simple_file("insights_commands/ls_-lanR_.dev.disk")
     ls_edac_mc = simple_file("insights_commands/ls_-lan_.sys.devices.system.edac.mc")
-    ls_etc = simple_file("insights_commands/ls_-lan_.etc_.etc.cloud.cloud.cfg.d_.etc.nova.migration_.etc.pki.ovirt-vmconsole_.etc.pki.tls.certs_.etc.pki.tls.private_.etc.rc.d.init.d_.etc.sysconfig")
+    ls_etc = first_file(["insights_commands/ls_-lan_.etc_.etc.cloud.cloud.cfg.d_.etc.nova.migration_.etc.pki.ovirt-vmconsole_.etc.pki.tls.certs_.etc.pki.tls.private_.etc.rc.d.init.d_.etc.selinux.targeted.policy_.etc.sysconfig_.etc.watchdog.d", "insights_commands/ls_-lan_.etc_.etc.cloud.cloud.cfg.d_.etc.nova.migration_.etc.pki.ovirt-vmconsole_.etc.pki.tls.certs_.etc.pki.tls.private_.etc.rc.d.init.d_.etc.selinux.targeted.policy_.etc.sysconfig", "insights_commands/ls_-lan_.etc_.etc.cloud.cloud.cfg.d_.etc.nova.migration_.etc.pki.ovirt-vmconsole_.etc.pki.tls.certs_.etc.pki.tls.private_.etc.rc.d.init.d_.etc.sysconfig"])
     ls_etc_ssh = simple_file("insights_commands/ls_-lanL_.etc.ssh")
     ls_ipa_idoverride_memberof = simple_file("insights_commands/ls_-lan_.usr.share.ipa.ui.js.plugins.idoverride-memberof")
     ls_krb5_sssd = simple_file("insights_commands/ls_-lan_.var.lib.sss.pubconf.krb5.include.d")
     ls_lib_firmware = simple_file("insights_commands/ls_-lanR_.lib.firmware")
     ls_ocp_cni_openshift_sdn = simple_file("insights_commands/ls_-l_.var.lib.cni.networks.openshift-sdn")
     ls_origin_local_volumes_pods = simple_file("insights_commands/ls_-l_.var.lib.origin.openshift.local.volumes.pods")
     ls_osroot = simple_file("insights_commands/ls_-lan")
@@ -135,14 +134,15 @@
     ls_tmp = simple_file("insights_commands/ls_-la_.tmp")
     ls_usr_bin = simple_file("insights_commands/ls_-lan_.usr.bin")
     ls_usr_lib64 = simple_file("insights_commands/ls_-lan_.usr.lib64")
     ls_var_cache_pulp = simple_file("insights_commands/ls_-lan_.var.cache.pulp")
     ls_var_lib_mongodb = simple_file("insights_commands/ls_-la_.var.lib.mongodb")
     ls_var_lib_nova_instances = simple_file("insights_commands/ls_-laRZ_.var.lib.nova.instances")
     ls_var_lib_pcp = simple_file("insights_commands/ls_-la_.var.lib.pcp")
+    ls_var_lib_rpm = simple_file("insights_commands/ls_-lan_.var.lib.rpm")
     ls_var_lib_rsyslog = simple_file("insights_commands/ls_-lZ_.var.lib.rsyslog")
     ls_var_log = simple_file("insights_commands/ls_-la_.var.log_.var.log.audit")
     ls_var_opt_mssql = simple_file("insights_commands/ls_-ld_.var.opt.mssql")
     ls_var_opt_mssql_log = simple_file("insights_commands/ls_-la_.var.opt.mssql.log")
     ls_var_spool_clientmq = simple_file("insights_commands/ls_-ln_.var.spool.clientmqueue")
     ls_var_spool_postfix_maildrop = simple_file("insights_commands/ls_-ln_.var.spool.postfix.maildrop")
     ls_var_tmp = simple_file("insights_commands/ls_-ln_.var.tmp")
@@ -219,33 +219,31 @@
     puppet_ca_cert_expire_date = simple_file("insights_commands/openssl_x509_-in_.etc.puppetlabs.puppet.ssl.ca.ca_crt.pem_-enddate_-noout")
     pvs_noheadings = simple_file("insights_commands/pvs_--nameprefixes_--noheadings_--separator_-a_-o_pv_all_vg_name_--config_global_locking_type_0")
     rabbitmq_report = simple_file("insights_commands/rabbitmqctl_report")
     rabbitmq_users = simple_file("insights_commands/rabbitmqctl_list_users")
     readlink_e_etc_mtab = simple_file("insights_commands/readlink_-e_.etc.mtab")
     readlink_e_shift_cert_client = simple_file("insights_commands/readlink_-e_.etc.origin.node.certificates.kubelet-client-current.pem")
     readlink_e_shift_cert_server = simple_file("insights_commands/readlink_-e_.etc.origin.node.certificates.kubelet-server-current.pem")
+    repquota_agnpuv = simple_file("insights_commands/repquota_-agnpuv")
     rhev_data_center = simple_file("insights_commands/python_-m_insights.tools.cat_--no-header_rhev_data_center")
     rhsm_katello_default_ca_cert = simple_file("insights_commands/openssl_x509_-in_.etc.rhsm.ca.katello-default-ca.pem_-noout_-issuer")
     rndc_status = simple_file("insights_commands/rndc_status")
     rpm_ostree_status = simple_file("insights_commands/rpm-ostree_status_--json")
-    rpm_V_packages = first_file(["insights_commands/rpm_-V_coreutils_procps_procps-ng_shadow-utils_passwd_sudo_chrony", "insights_commands/rpm_-V_coreutils_procps_procps-ng_shadow-utils_passwd_sudo"])
+    rpm_V_packages = first_file(["insights_commands/rpm_-V_coreutils_procps_procps-ng_shadow-utils_passwd_sudo_chrony_findutils", "insights_commands/rpm_-V_coreutils_procps_procps-ng_shadow-utils_passwd_sudo_chrony", "insights_commands/rpm_-V_coreutils_procps_procps-ng_shadow-utils_passwd_sudo"])
     saphostctl_getcimobject_sapinstance = simple_file("insights_commands/usr.sap.hostctrl.exe.saphostctrl_-function_GetCIMObject_-enuminstances_SAPInstance")
     saphostexec_status = simple_file("insights_commands/usr.sap.hostctrl.exe.saphostexec_-status")
     saphostexec_version = simple_file("insights_commands/usr.sap.hostctrl.exe.saphostexec_-version")
     satellite_content_hosts_count = first_file([
         "insights_commands/sudo_-iu_postgres_.usr.bin.psql_-d_foreman_-c_select_count_from_hosts",
         "insights_commands/sudo_-iu_postgres_psql_-d_foreman_-c_select_count_from_hosts"
     ])
     satellite_custom_ca_chain = simple_file("insights_commands/awk_BEGIN_pipe_openssl_x509_-noout_-subject_-enddate_._-_BEGIN_CERT._._-_END_CERT._print_pipe_._-_END_CERT._close_pipe_printf_n_.etc.pki.katello.certs.katello-server-ca.crt")
-    satellite_mongodb_storage_engine = simple_file("insights_commands/mongo_pulp_database_--eval_db.serverStatus_.storageEngine")
-    satellite_katello_repos_with_muliple_ref = simple_file('insights_commands/sudo_-iu_postgres_.usr.bin.psql_-d_foreman_-c_select_repository_href_count_from_katello_repository_references_group_by_repository_href_having_count_1_--csv')
     satellite_provision_param_settings = simple_file('insights_commands/sudo_-iu_postgres_.usr.bin.psql_-d_foreman_-c_select_name_value_from_parameters_where_name_package_upgrade_and_reference_id_in_select_id_from_operatingsystems_where_name_RedHat_and_major_9_--csv')
     satellite_qualified_capsules = simple_file("insights_commands/sudo_-iu_postgres_.usr.bin.psql_-d_foreman_-c_select_name_from_smart_proxies_where_download_policy_background_--csv")
     satellite_qualified_katello_repos = simple_file("insights_commands/sudo_-iu_postgres_.usr.bin.psql_-d_foreman_-c_select_id_name_url_download_policy_from_katello_root_repositories_where_download_policy_background_or_url_is_NULL_--csv")
-    satellite_sca_status = simple_file("insights_commands/sudo_-iu_postgres_.usr.bin.psql_-d_candlepin_-c_select_displayname_content_access_mode_from_cp_owner_--csv")
     sealert = simple_file('insights_commands/sealert_-l')
     sestatus = simple_file("insights_commands/sestatus_-b")
     smbstatus_p = simple_file("insights_commands/smbstatus_-p")
     software_collections_list = simple_file('insights_commands/scl_--list')
     spamassassin_channels = simple_file('insights_commands/grep_-r_s_CHANNELURL_.etc.mail.spamassassin.channel.d')
     ss = simple_file("insights_commands/ss_-tupna")
     sshd_config_perms = first_file(["insights_commands/ls_-lH_.etc.ssh.sshd_config", "insights_commands/ls_-l_.etc.ssh.sshd_config"])
@@ -268,15 +266,14 @@
     testparm_s = simple_file("insights_commands/testparm_-s")
     testparm_v_s = simple_file("insights_commands/testparm_-v_-s")
     timedatectl_status = simple_file("insights_commands/timedatectl_status")
     tomcat_vdc_fallback = simple_file("insights_commands/find_.usr.share_-maxdepth_1_-name_tomcat_-exec_.bin.grep_-R_-s_VirtualDirContext_--include_.xml")
     tuned_adm = simple_file("insights_commands/tuned-adm_list")
     uname = simple_file("insights_commands/uname_-a")
     uptime = simple_file("insights_commands/uptime")
-    version_info = simple_file("version_info")
     vdo_status = simple_file("insights_commands/vdo_status")
     vgdisplay = simple_file("insights_commands/vgdisplay")
     vgs_noheadings = simple_file("insights_commands/vgs_--nameprefixes_--noheadings_--separator_-a_-o_vg_all_--config_global_locking_type_0")
     virsh_list_all = simple_file("insights_commands/virsh_--readonly_list_--all")
     virt_what = simple_file("insights_commands/virt-what")
     wc_proc_1_mountinfo = simple_file("insights_commands/wc_-l_.proc.1.mountinfo")
     yum_list_available = simple_file("insights_commands/yum_-C_--noplugins_list_available")
```

### Comparing `insights-core-3.1.9/insights/specs/jdr_archive.py` & `insights-core-3.2.0/insights/specs/jdr_archive.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/specs/sos_archive.py` & `insights-core-3.2.0/insights/specs/sos_archive.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 class SosSpecs(Specs):
     alternatives_display_python = simple_file("sos_commands/alternatives/alternatives_--display_python")
     auditctl_rules = simple_file("sos_commands/auditd/auditctl_-l")
     auditctl_status = simple_file("sos_commands/auditd/auditctl_-s")
     auditd_conf = simple_file("/etc/audit/auditd.conf")
+    audispd_conf = simple_file("/etc/audisp/audispd.conf")
     autofs_conf = simple_file("/etc/autofs.conf")
 
     blkid = first_file(["sos_commands/block/blkid_-c_.dev.null", "sos_commands/filesys/blkid_-c_.dev.null"])
     candlepin_error_log = first_of([
         simple_file("var/log/candlepin/error.log"),
         simple_file(r"sos_commands/foreman/foreman-debug/var/log/candlepin/error.log")
     ])
@@ -141,26 +142,27 @@
     ])
     lspci = first_of([
         simple_file("sos_commands/pci/lspci_-nnvv"),
         simple_file("sos_commands/pci/lspci_-nvv"),
         simple_file("sos_commands/pci/lspci")
     ])
     lsscsi = simple_file("sos_commands/scsi/lsscsi")
+    lvm_conf = simple_file("/etc/lvm/lvm.conf")
     lvs_headings = first_file([
         "sos_commands/lvm2/lvs_-a_-o_lv_tags_devices_lv_kernel_read_ahead_lv_read_ahead_stripes_stripesize_--config_global_metadata_read_only_1_--nolocking_--foreign",
         "sos_commands/lvm2/lvs_-a_-o_lv_tags_devices_lv_kernel_read_ahead_lv_read_ahead_stripes_stripesize_--config_global_locking_type_0_metadata_read_only_1",
         "sos_commands/lvm2/lvs_-a_-o_lv_tags_devices_--config_global_locking_type_0",
         "sos_commands/lvm2/lvs_-a_-o_devices",
         "sos_commands/devicemapper/lvs_-a_-o__devices"
     ])
     manila_conf = first_file(["/var/lib/config-data/puppet-generated/manila/etc/manila/manila.conf", "/etc/manila/manila.conf"])
     mdadm_E = glob_file("sos_commands/md/mdadm_-E_*")
     mistral_executor_log = simple_file("/var/log/mistral/executor.log")
     mlx4_port = glob_file("/sys/bus/pci/devices/*/mlx4_port[0-9]")
-    modinfo_all = glob_file("sos_commands/kernel/modinfo_*")
+    modinfo_filtered_modules = simple_file("sos_commands/kernel/modinfo_ALL_MODULES")
     mokutil_sbstate = simple_file("sos_commands/boot/mokutil_--sb-state")
     mount = simple_file("sos_commands/filesys/mount_-l")
     mountinfo = simple_file("proc/self/mountinfo")
     mounts = simple_file("/proc/mounts")
     multipath__v4__ll = first_file(["sos_commands/multipath/multipath_-v4_-ll", "sos_commands/devicemapper/multipath_-v4_-ll"])
     netstat = first_file(["sos_commands/networking/netstat_-neopa", "sos_commands/networking/netstat_-W_-neopa", "sos_commands/networking/netstat_-T_-neopa"])
     netstat_agn = first_of([simple_file("sos_commands/networking/netstat_-agn"), simple_file("sos_commands/networking/netstat_-W_-agn"), simple_file("sos_commands/networking/netstat_-T_-agn")])
```

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_ansible_info.py` & `insights-core-3.2.0/insights/tests/combiners/test_ansible_info.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_ceph_osd_tree.py` & `insights-core-3.2.0/insights/tests/combiners/test_ceph_osd_tree.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_ceph_version.py` & `insights-core-3.2.0/insights/tests/combiners/test_ceph_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_cloud_instance.py` & `insights-core-3.2.0/insights/tests/combiners/test_cloud_instance.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_cloud_provider.py` & `insights-core-3.2.0/insights/tests/combiners/test_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_cpu_vulns_all.py` & `insights-core-3.2.0/insights/tests/combiners/test_cpu_vulns_all.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_crio_conf.py` & `insights-core-3.2.0/insights/tests/combiners/test_crio_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_cryptsetup.py` & `insights-core-3.2.0/insights/tests/combiners/test_cryptsetup.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_dmesg.py` & `insights-core-3.2.0/insights/tests/combiners/test_dmesg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_dnsmasq_conf_all.py` & `insights-core-3.2.0/insights/tests/combiners/test_dnsmasq_conf_all.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_du.py` & `insights-core-3.2.0/insights/tests/combiners/test_du.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_grub_conf.py` & `insights-core-3.2.0/insights/tests/combiners/test_grub_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_hostname.py` & `insights-core-3.2.0/insights/tests/combiners/test_hostname.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_httpd_conf_tree.py` & `insights-core-3.2.0/insights/tests/combiners/test_httpd_conf_tree.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_ipcs_semaphores.py` & `insights-core-3.2.0/insights/tests/combiners/test_ipcs_semaphores.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_ipcs_shared_memory.py` & `insights-core-3.2.0/insights/tests/combiners/test_ipcs_shared_memory.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_ipv6.py` & `insights-core-3.2.0/insights/tests/combiners/test_ipv6.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_journald_conf.py` & `insights-core-3.2.0/insights/tests/combiners/test_journald_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_krb5.py` & `insights-core-3.2.0/insights/tests/combiners/test_krb5.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,33 +47,35 @@
 # default_ccache_name = KEYRING:persistent:%{uid}
  EXAMPLE.COM = {
   kdc = kerberos.example.com
   kdc = test2.example.com
   kdc = test3.example.com
   admin_server = kerberos.example.com
  }
+ EXAMPLE2.COM = {
+  kdc = kerberos.example2.com
+  admin_server = kerberos.example2.com
+ }
+ EXAMPLE3.COM = {
+  kdc = kerberos.example3.com
+  admin_server = kerberos.example3.com
+ } *
 
 [logging]
  default = FILE:/var/log/krb5libs2.log
  kdc = FILE:/var/log/krb5kdc2.log
  admin_server = FILE:/var/log/kadmind2.log
 
 [libdefaults]
+ default_realm = EXAMPLE2.COM
+ dns_canonicalize_hostname = false
  donotoverwrite2 = true
  dnsdsd = false
  tilnvs = 24h
  default_ccache_name = KEYRING:%{uid}:persistent
- EXAMPLE2.COM = {
-  kdc = kerberos.example2.com
-  admin_server = kerberos.example2.com
- }
- EXAMPLE3.COM = {
-  kdc = kerberos.example3.com
-  admin_server = kerberos.example3.com *
- }
 """.strip()
 
 
 KRB5CONFIG3 = """
 
 [libdefaults]
  donotoverwrite3 = true
@@ -85,22 +87,28 @@
     krb51 = Krb5Configuration(context_wrap(KRB5CONFIG, path='/etc/krb5.conf'))
     krb52 = Krb5Configuration(context_wrap(KRB5CONFIG2, path='/etc/krb5.conf.d/test.conf'))
     krb53 = Krb5Configuration(context_wrap(KRB5CONFIG3, path='/etc/krb5.conf.d/test2.conf'))
     result = AllKrb5Conf([krb51, krb52, krb53])
     assert result.has_option("libdefaults", "donotoverwrite1")
     assert result.has_option("libdefaults", "donotoverwrite2")
     assert result.has_option("libdefaults", "donotoverwrite3")
+    assert result.getboolean("libdefaults", "donotoverwrite3") is True
+    assert result.getboolean("libdefaults", "dnsdsd") is False
     assert result["logging"]["kdc"] == "FILE:/var/log/krb5kdc.log"
     assert result.has_option("logging", "admin_server")
-    assert result["libdefaults"]["EXAMPLE2.COM"]["kdc"] == "kerberos.example2.com"
+    assert result["realms"]["EXAMPLE2.COM"]["kdc"] == "kerberos.example2.com"
     assert result["libdefaults"]["default_ccache_name"] == "KEYRING:%{uid}:persistent"
     assert "realms" in result.sections()
     assert "realmstest" not in result.sections()
     assert result.has_section("realms")
     assert not result.has_option("realms", "nosuchoption")
     assert not result.has_option("nosucsection", "nosuchoption")
     assert not result.options("realmsno")
     assert sorted(result.options("logging")) == sorted(['default', 'admin_server', 'kdc'])
     assert result.include == ["/etc/krb5test.conf"]
     assert result.includedir == ["/etc/krb5.conf.d/"]
     assert result.module == ["/etc/krb5test.conf:residual"]
     assert result.files == ['krb5.conf', 'test.conf', 'test2.conf']
+    assert result.dns_lookup_realm is True
+    assert result.dns_lookup_kdc is True
+    assert result.default_realm == "EXAMPLE2.COM"
+    assert result.realms == set(["EXAMPLE.COM", "EXAMPLE2.COM", "EXAMPLE3.COM", "EXAMPLE4.COM"])
```

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_limits_conf.py` & `insights-core-3.2.0/insights/tests/combiners/test_limits_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_logrotate_conf.py` & `insights-core-3.2.0/insights/tests/combiners/test_logrotate_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_logrotate_conf_tree.py` & `insights-core-3.2.0/insights/tests/combiners/test_logrotate_conf_tree.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_lspci.py` & `insights-core-3.2.0/insights/tests/combiners/test_lspci.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_lvm.py` & `insights-core-3.2.0/insights/tests/combiners/test_lvm.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_md5check.py` & `insights-core-3.2.0/insights/tests/combiners/test_md5check.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_mlx4_port.py` & `insights-core-3.2.0/insights/tests/combiners/test_mlx4_port.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_modinfo.py` & `insights-core-3.2.0/insights/tests/combiners/test_modinfo.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,27 @@
 import doctest
-from insights.parsers.modinfo import (ModInfoEach, KernelModulesInfo)
+
+from insights.parsers.modinfo import KernelModulesInfo
 from insights.combiners.modinfo import ModulesInfo
 from insights.tests.parsers.test_modinfo import (
         MODINFO_I40E, MODINFO_INTEL, MODINFO_BNX2X
 )
 from insights.tests import context_wrap
-from insights.combiners.modinfo import ModInfo
 from insights.combiners import modinfo
 
 
 def test_modinfo_doc_examples():
-    modinfo_i40e = ModInfoEach(context_wrap(MODINFO_I40E))
-    modinfo_intel = ModInfoEach(context_wrap(MODINFO_INTEL))
-    modinfo_bnx2x = ModInfoEach(context_wrap(MODINFO_BNX2X))
-    comb = ModInfo(
-        None, [
-            modinfo_i40e,
-            modinfo_intel,
-            modinfo_bnx2x]
-    )
     filter_modules = KernelModulesInfo(context_wrap(
         '{0}\n{1}\n{2}'.format(
             MODINFO_I40E,
             MODINFO_INTEL,
             MODINFO_BNX2X)
     ))
-    combiner_obj = ModulesInfo(
-        filter_modules
-    )
-    env = {
-        'modinfo_obj': comb,
-        'modules_obj': combiner_obj
-    }
+    combiner_obj = ModulesInfo(filter_modules)
+    env = {'modules_obj': combiner_obj}
     failed, total = doctest.testmod(modinfo, globs=env)
     assert failed == 0
 
 
 def test_modules_info():
     filter_modules = KernelModulesInfo(context_wrap(
         '{0}\n{1}\n{2}'.format(
```

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_modprobe.py` & `insights-core-3.2.0/insights/tests/combiners/test_modprobe.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_netstat.py` & `insights-core-3.2.0/insights/tests/combiners/test_netstat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_nfs_exports.py` & `insights-core-3.2.0/insights/tests/combiners/test_nfs_exports.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_nginx_conf.py` & `insights-core-3.2.0/insights/tests/combiners/test_nginx_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_nmcli_dev_show.py` & `insights-core-3.2.0/insights/tests/combiners/test_nmcli_dev_show.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_ps.py` & `insights-core-3.2.0/insights/tests/combiners/test_ps.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_redhat_release.py` & `insights-core-3.2.0/insights/tests/combiners/test_redhat_release.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_rhel_for_edge.py` & `insights-core-3.2.0/insights/tests/combiners/test_rhel_for_edge.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_rhsm_release.py` & `insights-core-3.2.0/insights/tests/combiners/test_rhsm_release.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_rsyslog_confs.py` & `insights-core-3.2.0/insights/tests/combiners/test_rsyslog_confs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_sap.py` & `insights-core-3.2.0/insights/tests/combiners/test_sap.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_satellite_version.py` & `insights-core-3.2.0/insights/tests/combiners/test_satellite_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_selinux.py` & `insights-core-3.2.0/insights/tests/combiners/test_selinux.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_services.py` & `insights-core-3.2.0/insights/tests/combiners/test_services.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_smt.py` & `insights-core-3.2.0/insights/tests/combiners/test_smt.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_ssl_certificate.py` & `insights-core-3.2.0/insights/tests/combiners/test_ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_sudoers.py` & `insights-core-3.2.0/insights/tests/combiners/test_sudoers.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_sys_vmbus_devices.py` & `insights-core-3.2.0/insights/tests/combiners/test_sys_vmbus_devices.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_sysctl_conf.py` & `insights-core-3.2.0/insights/tests/combiners/test_sysctl_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_tmpfilesd.py` & `insights-core-3.2.0/insights/tests/combiners/test_tmpfilesd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_tomcat_virtual_dir_context.py` & `insights-core-3.2.0/insights/tests/combiners/test_tomcat_virtual_dir_context.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_user_namespaces.py` & `insights-core-3.2.0/insights/tests/combiners/test_user_namespaces.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_virt_what.py` & `insights-core-3.2.0/insights/tests/combiners/test_virt_what.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_virt_who_conf.py` & `insights-core-3.2.0/insights/tests/combiners/test_virt_who_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/combiners/test_x86_page_branch.py` & `insights-core-3.2.0/insights/tests/combiners/test_x86_page_branch.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/components/test_ceph.py` & `insights-core-3.2.0/insights/tests/components/test_ceph.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/components/test_cloud_provider.py` & `insights-core-3.2.0/insights/tests/components/test_cloud_provider.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/components/test_cryptsetup.py` & `insights-core-3.2.0/insights/tests/components/test_cryptsetup.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/components/test_openstack.py` & `insights-core-3.2.0/insights/tests/components/test_openstack.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/components/test_rhel_version.py` & `insights-core-3.2.0/insights/tests/components/test_rhel_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/components/test_satellite.py` & `insights-core-3.2.0/insights/tests/components/test_satellite.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/components/test_virtualization.py` & `insights-core-3.2.0/insights/tests/components/test_virtualization.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/container/test_containers_inspect.py` & `insights-core-3.2.0/insights/tests/datasources/container/test_containers_inspect.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/container/test_nginx_conf.py` & `insights-core-3.2.0/insights/tests/datasources/container/test_nginx_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/container/test_running_rhel_containers.py` & `insights-core-3.2.0/insights/tests/datasources/container/test_running_rhel_containers.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_aws.py` & `insights-core-3.2.0/insights/tests/datasources/test_aws.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_awx_manage.py` & `insights-core-3.2.0/insights/tests/datasources/test_awx_manage.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_candlepin_broker.py` & `insights-core-3.2.0/insights/tests/datasources/test_candlepin_broker.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_cloud_init.py` & `insights-core-3.2.0/insights/tests/datasources/test_cloud_init.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_corosync.py` & `insights-core-3.2.0/insights/tests/datasources/test_corosync.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_datasource_timeout.py` & `insights-core-3.2.0/insights/tests/datasources/test_datasource_timeout.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_dir_list.py` & `insights-core-3.2.0/insights/tests/datasources/test_dir_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_ethernet.py` & `insights-core-3.2.0/insights/tests/datasources/test_ethernet.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_get_running_commands.py` & `insights-core-3.2.0/insights/tests/datasources/test_get_running_commands.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_httpd.py` & `insights-core-3.2.0/insights/tests/datasources/test_httpd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_ipcs.py` & `insights-core-3.2.0/insights/tests/datasources/test_ipcs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_kernel_module_list.py` & `insights-core-3.2.0/insights/tests/datasources/test_kernel_module_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_lpstat.py` & `insights-core-3.2.0/insights/tests/datasources/test_lpstat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_luks_devices.py` & `insights-core-3.2.0/insights/tests/datasources/test_luks_devices.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_package_provides.py` & `insights-core-3.2.0/insights/tests/datasources/test_package_provides.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_pcp.py` & `insights-core-3.2.0/insights/tests/datasources/test_pcp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_ps.py` & `insights-core-3.2.0/insights/tests/datasources/test_ps.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_rpm_pkgs.py` & `insights-core-3.2.0/insights/tests/datasources/test_rpm_pkgs.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 httpd-core; httpd-core-2.4.53-7.el9.x86_64; /usr/share/doc/httpd-core; drwxr-xr-x; apache; root; Red Hat, Inc.
 httpd-core; httpd-core-2.4.53-7.el9.x86_64; /usr/share/doc/httpd-core/CHANGES; -rw-r--r--; root; root; Red Hat, Inc.
 postgresql-server; postgresql-server-13.7-1.el9_0.x86_64; /var/lib/pgsql; drwx------; postgres; postgres; Red Hat, Inc.
 polkit; polkit-0.117-10.el9_0.x86_64; /usr/lib/polkit-1; drwxrwxr-x; polkitd; polkitd; Red Hat, Inc.
 polkit; polkit-0.117-10.el9_0.x86_64; /usr/lib/polkit-1/polkitd; -rwxr-xr-x; root; root; Red Hat, Inc.
 """.strip()
 
-RPM_EXPECTED = [("httpd-core", "httpd-core-2.4.53-7.el9.x86_64", "Red Hat, Inc.")]
+RPM_EXPECTED = ["httpd-core|httpd-core-2.4.53-7.el9.x86_64|Red Hat, Inc."]
 
 RPM_BAD_CMD = "bash: rpm: command not found..."
 
 RPM_EMPTY_CMD = ""
 
 RELATIVE_PATH = "insights_commands/rpm_pkgs"
```

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_sap.py` & `insights-core-3.2.0/insights/tests/datasources/test_sap.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_satellite_missed_queues.py` & `insights-core-3.2.0/insights/tests/datasources/test_satellite_missed_queues.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_semanage.py` & `insights-core-3.2.0/insights/tests/datasources/test_semanage.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_ssl_certificate.py` & `insights-core-3.2.0/insights/tests/datasources/test_ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_sys_fs_cgroup_memory.py` & `insights-core-3.2.0/insights/tests/datasources/test_sys_fs_cgroup_memory.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_sys_fs_cgroup_memory_tasks_number.py` & `insights-core-3.2.0/insights/tests/datasources/test_sys_fs_cgroup_memory_tasks_number.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_user_group.py` & `insights-core-3.2.0/insights/tests/datasources/test_user_group.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/datasources/test_yum_updates.py` & `insights-core-3.2.0/insights/tests/datasources/test_yum_updates.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/__init__.py` & `insights-core-3.2.0/insights/tests/parsers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,18 +49,18 @@
     """
     deprecated(
         skip_component_check,
         "Please use the :method:`skip_component_check` instead.",
         "3.2.25"
     )
 
-    from insights.core.exceptions import SkipException
+    from insights.core.exceptions import SkipComponent
     from insights.tests import context_wrap
 
-    with pytest.raises(SkipException) as ex:
+    with pytest.raises(SkipComponent) as ex:
         parser_obj(context_wrap(output_str))
     return str(ex)
 
 
 def skip_component_check(parser_obj, output_str=""):
     from insights.core.exceptions import SkipComponent
     from insights.tests import context_wrap
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/lvm_test_data.py` & `insights-core-3.2.0/insights/tests/parsers/lvm_test_data.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_abrt_ccpp.py` & `insights-core-3.2.0/insights/tests/parsers/test_abrt_ccpp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_abrt_status_bare.py` & `insights-core-3.2.0/insights/tests/parsers/test_abrt_status_bare.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_alternatives.py` & `insights-core-3.2.0/insights/tests/parsers/test_alternatives.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_amq_broker.py` & `insights-core-3.2.0/insights/tests/parsers/test_amq_broker.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_audit_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_audit_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_auditctl.py` & `insights-core-3.2.0/insights/tests/parsers/test_auditctl.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_auditd_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_auditd_conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from insights.parsers.auditd_conf import AuditdConf
+from insights.parsers.auditd_conf import AuditdConf, AudispdConf
 from insights.tests import context_wrap
 
 # from RHEL 6.8, 7.2
 AUDITD_CONF_1 = """
 #
 # This file controls the configuration of the audit daemon
 #
@@ -54,14 +54,29 @@
 broken_option_g
 option_h = value_h # some comment
 option_i = value_i # this must be accessible, even after all these errors
 """.strip()
 
 AUDITD_CONF_PATH = "etc/audit/auditd.conf"
 
+AUDISPD_CONF_1 = """
+#
+# This file controls the configuration of the audit event
+# dispatcher daemon, audispd.
+#
+
+q_depth = 150
+overflow_action = SYSLOG
+priority_boost = 4
+max_restarts = 10
+name_format = HOSTNAME
+#name = mydomain
+""".strip()
+AUDISPD_CONF_PATH = "etc/audisp/audispd.conf"
+
 
 def test_constructor():
     context = context_wrap(AUDITD_CONF_1, AUDITD_CONF_PATH)
     result = AuditdConf(context)
 
     assert "tcp_listen_queue = 5" in result.active_lines_unparsed
     assert "SUSPEND" == result.active_settings["disk_error_action"]
@@ -112,7 +127,26 @@
 
 def test_get_active_setting_value():
     context = context_wrap(AUDITD_CONF_1, AUDITD_CONF_PATH)
     result = AuditdConf(context)
     active_settings = build_active_settings_expected()
     for key, value in active_settings.items():
         assert result.get_active_setting_value(key) == value
+
+
+def test_audispd_conf():
+    context = context_wrap(AUDISPD_CONF_1, AUDISPD_CONF_PATH)
+    result = AudispdConf(context)
+
+    assert "q_depth = 150" in result.active_lines_unparsed
+    assert "150" == result.active_settings["q_depth"]
+    assert "name" not in result.active_settings
+    assert "#name" not in result.active_settings
+    assert "SYSLOG" == result.get_active_setting_value("overflow_action")
+    assert "10" == result.get_active_setting_value("max_restarts")
+
+    context = context_wrap(AUDITD_CONF_2, AUDISPD_CONF_PATH)
+    result = AudispdConf(context)
+
+    assert "comment" not in result.active_settings
+    assert "broken_option_g" not in result.active_settings
+    assert "value_i" == result.get_active_setting_value("option_i")
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_authselect.py` & `insights-core-3.2.0/insights/tests/parsers/test_authselect.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_autofs_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_autofs_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_avc_cache_threshold.py` & `insights-core-3.2.0/insights/tests/parsers/test_avc_cache_threshold.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_avc_hash_stats.py` & `insights-core-3.2.0/insights/tests/parsers/test_avc_hash_stats.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_aws_instance_id.py` & `insights-core-3.2.0/insights/tests/parsers/test_aws_instance_id.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import doctest
 import pytest
 
 from insights.core.exceptions import ParseException, SkipComponent
 from insights.parsers import aws_instance_id
-from insights.parsers.aws_instance_id import AWSInstanceIdDoc, AWSInstanceIdPkcs7
+from insights.parsers.aws_instance_id import AWSInstanceIdDoc, AWSInstanceIdPkcs7,\
+        AWSPublicIpv4Addresses, AWSPublicHostnames
 from insights.tests import context_wrap
 
 AWS_CURL_ERROR = """
 curl: (7) couldn't connect to host
 """
 
 AWS_ID_DOC = """
@@ -202,7 +203,31 @@
 def test_doc_examples():
     env = {
         'aws_id_doc': AWSInstanceIdDoc(context_wrap(AWS_ID_DOC)),
         'aws_id_sig': AWSInstanceIdPkcs7(context_wrap(AWS_ID_PKCS7)),
     }
     failed, total = doctest.testmod(aws_instance_id, globs=env)
     assert failed == 0
+
+
+def test_aws_public_ipv4_addresses():
+    with pytest.raises(SkipComponent):
+        AWSPublicIpv4Addresses(context_wrap(AWS_CURL_ERROR))
+
+    with pytest.raises(SkipComponent):
+        AWSPublicIpv4Addresses(context_wrap(""))
+
+    doc = AWSPublicIpv4Addresses(context_wrap("1.2.3.4"))
+    assert doc is not None
+    assert doc == ["1.2.3.4"]
+
+
+def test_aws_public_hostnames():
+    with pytest.raises(SkipComponent):
+        AWSPublicHostnames(context_wrap(AWS_CURL_ERROR))
+
+    with pytest.raises(SkipComponent):
+        AWSPublicHostnames(context_wrap(""))
+
+    doc = AWSPublicHostnames(context_wrap("1.2.3.4"))
+    assert doc is not None
+    assert doc == ["1.2.3.4"]
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_awx_manage.py` & `insights-core-3.2.0/insights/tests/parsers/test_awx_manage.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_azure_instance.py` & `insights-core-3.2.0/insights/tests/parsers/test_azure_instance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import doctest
 import pytest
 
 from insights.core.exceptions import ContentException, ParseException, SkipComponent
 from insights.parsers import azure_instance
-from insights.parsers.azure_instance import AzureInstanceID, AzureInstancePlan, AzureInstanceType
+from insights.parsers.azure_instance import AzureInstanceID, AzureInstancePlan, AzureInstanceType, AzurePublicIpv4Addresses
 from insights.tests import context_wrap
 
 # For AzureInstanceID
 AZURE_ID = "f904ece8-c6c1-4b5c-881f-309b50f25e50"
 
 # For AzureInstanceType
 AZURE_TYPE_1 = "Standard_L32s"
@@ -57,14 +57,41 @@
 AZURE_PLAN_AB_2 = """
 curl: (7) couldn't connect to host
 """.strip()
 AZURE_PLAN_AB_3 = """
 curl: (28) connect() timed out!
 """.strip()
 
+# For AzurePublicIpv4Addresses and AzurePublicHostname
+AZURE_LB_1 = """
+{
+  "loadbalancer": {
+    "publicIpAddresses": [
+      {
+        "frontendIpAddress": "137.116.118.209",
+        "privateIpAddress": "10.0.0.4"
+      }
+    ],
+    "inboundRules": [],
+    "outboundRules": []
+  }
+}
+""".strip()
+
+AZURE_LB_ERR1 = """
+curl: (7) Failed to connect to 169.254.169.254 port 80: Connection timed out
+""".strip()
+AZURE_LB_ERR2 = """
+curl: (7) couldn't connect to host
+""".strip()
+AZURE_LB_ERR3 = """
+curl: (28) connect() timed out!
+""".strip()
+AZURE_LB_ERR4 = "}}}"
+
 
 # Test AzureInstanceID
 def test_azure_instance_id_ab_empty():
     with pytest.raises(SkipComponent):
         AzureInstanceID(context_wrap(''))
 
 
@@ -167,7 +194,24 @@
     env = {
         'azure_id': AzureInstanceID(context_wrap(AZURE_ID)),
         'azure_plan': AzureInstancePlan(context_wrap(AZURE_PLAN_DOC)),
         'azure_type': AzureInstanceType(context_wrap(AZURE_TYPE_DOC)),
     }
     failed, total = doctest.testmod(azure_instance, globs=env)
     assert failed == 0
+
+
+def test_azure_public_ipv4():
+    with pytest.raises(SkipComponent):
+        AzurePublicIpv4Addresses(context_wrap(AZURE_LB_ERR1))
+
+    with pytest.raises(SkipComponent):
+        AzurePublicIpv4Addresses(context_wrap(AZURE_LB_ERR2))
+
+    with pytest.raises(SkipComponent):
+        AzurePublicIpv4Addresses(context_wrap(AZURE_LB_ERR3))
+
+    with pytest.raises(ParseException):
+        AzurePublicIpv4Addresses(context_wrap(AZURE_LB_ERR4))
+
+    azure = AzurePublicIpv4Addresses(context_wrap(AZURE_LB_1))
+    assert azure[0] == "137.116.118.209"
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_azure_instance_plan.py` & `insights-core-3.2.0/insights/tests/parsers/test_azure_instance_plan.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_azure_instance_type.py` & `insights-core-3.2.0/insights/tests/parsers/test_azure_instance_type.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_bdi_read_ahead_kb.py` & `insights-core-3.2.0/insights/tests/parsers/test_bdi_read_ahead_kb.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_blacklisted.py` & `insights-core-3.2.0/insights/tests/parsers/test_blacklisted.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_blkid.py` & `insights-core-3.2.0/insights/tests/parsers/test_blkid.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_bond.py` & `insights-core-3.2.0/insights/tests/parsers/test_bond.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_bond_dynamic_lb.py` & `insights-core-3.2.0/insights/tests/parsers/test_bond_dynamic_lb.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_brctl_show.py` & `insights-core-3.2.0/insights/tests/parsers/test_brctl_show.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_candlepin_broker.py` & `insights-core-3.2.0/insights/tests/parsers/test_candlepin_broker.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_catalina_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_catalina_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cciss.py` & `insights-core-3.2.0/insights/tests/parsers/test_cciss.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ceilometer_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_ceilometer_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ceilometer_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_ceilometer_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ceph_cmd_json_parsing.py` & `insights-core-3.2.0/insights/tests/parsers/test_ceph_cmd_json_parsing.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ceph_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_ceph_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ceph_insights.py` & `insights-core-3.2.0/insights/tests/parsers/test_ceph_insights.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ceph_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_ceph_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ceph_osd_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_ceph_osd_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ceph_osd_tree_text.py` & `insights-core-3.2.0/insights/tests/parsers/test_ceph_osd_tree_text.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ceph_version.py` & `insights-core-3.2.0/insights/tests/parsers/test_ceph_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_certificates_enddate.py` & `insights-core-3.2.0/insights/tests/parsers/test_certificates_enddate.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cgroups.py` & `insights-core-3.2.0/insights/tests/parsers/test_cgroups.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_checkin_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_checkin_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_chkconfig.py` & `insights-core-3.2.0/insights/tests/parsers/test_chkconfig.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cib.py` & `insights-core-3.2.0/insights/tests/parsers/test_cib.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cinder_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_cinder_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cinder_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_cinder_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cloud_cfg.py` & `insights-core-3.2.0/insights/tests/parsers/test_cloud_cfg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cloud_init_custom_network.py` & `insights-core-3.2.0/insights/tests/parsers/test_cloud_init_custom_network.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cloud_init_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_cloud_init_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cluster_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_cluster_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cmdline.py` & `insights-core-3.2.0/insights/tests/parsers/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cni_podman_bridge_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_cni_podman_bridge_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cobbler_modules_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_cobbler_modules_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cobbler_settings.py` & `insights-core-3.2.0/insights/tests/parsers/test_cobbler_settings.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_config_file_perms.py` & `insights-core-3.2.0/insights/tests/parsers/test_config_file_perms.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_containers_inspect.py` & `insights-core-3.2.0/insights/tests/parsers/test_containers_inspect.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_containers_policy.py` & `insights-core-3.2.0/insights/tests/parsers/test_containers_policy.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_corosync.py` & `insights-core-3.2.0/insights/tests/parsers/test_corosync.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_corosync_cmapctl.py` & `insights-core-3.2.0/insights/tests/parsers/test_corosync_cmapctl.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cpu_online.py` & `insights-core-3.2.0/insights/tests/parsers/test_cpu_online.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cpu_vulns.py` & `insights-core-3.2.0/insights/tests/parsers/test_cpu_vulns.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cpuinfo.py` & `insights-core-3.2.0/insights/tests/parsers/test_cpuinfo.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cpupower_frequency_info.py` & `insights-core-3.2.0/insights/tests/parsers/test_cpupower_frequency_info.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cpuset_cpus.py` & `insights-core-3.2.0/insights/tests/parsers/test_cpuset_cpus.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_crictl_logs.py` & `insights-core-3.2.0/insights/tests/parsers/test_crictl_logs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_crio_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_crio_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cron_daily_rhsmd.py` & `insights-core-3.2.0/insights/tests/parsers/test_cron_daily_rhsmd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cron_jobs.py` & `insights-core-3.2.0/insights/tests/parsers/test_cron_jobs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_crontab.py` & `insights-core-3.2.0/insights/tests/parsers/test_crontab.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_crypto_policies_bind.py` & `insights-core-3.2.0/insights/tests/parsers/test_crypto_policies_bind.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_crypto_policies_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_crypto_policies_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_crypto_policies_doc_examples.py` & `insights-core-3.2.0/insights/tests/parsers/test_crypto_policies_doc_examples.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_crypto_policies_opensshserver.py` & `insights-core-3.2.0/insights/tests/parsers/test_crypto_policies_opensshserver.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cryptsetup_luksDump.py` & `insights-core-3.2.0/insights/tests/parsers/test_cryptsetup_luksDump.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_cups_ppd.py` & `insights-core-3.2.0/insights/tests/parsers/test_cups_ppd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_date.py` & `insights-core-3.2.0/insights/tests/parsers/test_date.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_db2.py` & `insights-core-3.2.0/insights/tests/parsers/test_db2.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dcbtool_gc_dcb.py` & `insights-core-3.2.0/insights/tests/parsers/test_dcbtool_gc_dcb.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_designate_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_designate_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_df.py` & `insights-core-3.2.0/insights/tests/parsers/test_df.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dig.py` & `insights-core-3.2.0/insights/tests/parsers/test_dig.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dirsrv_logs.py` & `insights-core-3.2.0/insights/tests/parsers/test_dirsrv_logs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dmesg.py` & `insights-core-3.2.0/insights/tests/parsers/test_dmesg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dmesg_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_dmesg_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dmidecode.py` & `insights-core-3.2.0/insights/tests/parsers/test_dmidecode.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dmsetup.py` & `insights-core-3.2.0/insights/tests/parsers/test_dmsetup.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dnf_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_dnf_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dnf_module.py` & `insights-core-3.2.0/insights/tests/parsers/test_dnf_module.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,31 +27,35 @@
 postgresql          10 [d]      client, server [d]                        PostgreSQL server and client module
 postgresql          9.6         client, server [d]                        PostgreSQL server and client module
 python27            2.7 [d]     common [d]                                Python programming language, version 2.7
 python36            3.6 [d][e]  common [d], build                         Python programming language, version 3.6
 redis               5 [d]       common [d]                                Redis persistent key-value database
 rhn-tools           1.0 [d]     common [d]                                Red Hat Satellite 5 tools for RHEL
 ruby                2.5 [d]     common [d]                                An interpreter of object-oriented scripting language
+ruby                2.6 [e]     common [d]                                An interpreter of object-oriented scripting language
+ruby                2.7         common [d]                                An interpreter of object-oriented scripting language
 rust-toolset        rhel8 [d]   common [d]                                Rust
 satellite-5-client  1.0 [d]     common [d], gui                           Red Hat Satellite 5 client packages
 scala               2.10 [d]    common [d]                                A hybrid functional/object-oriented language for the JVM
 squid               4 [d]       common [d]                                Squid - Optimising Web Delivery
 subversion          1.10 [d]    common [d], server                        Apache Subversion
 swig                3.0 [d]     common [d], complete                      Connects C/C++/Objective C to some high-level programming languages
 varnish             6 [d]       common [d]                                Varnish HTTP cache
 virt                rhel [d]    common [d]                                Virtualization module
+default_disabled    1.0 [d][x]                                            Default module which is disabled
 
 Hint: [d]efault, [e]nabled, [x]disabled, [i]nstalled
 """.strip()
 
 DNF_MODULE_LIST_DOC = """
 Updating Subscription Management repositories.
 Name                Stream      Profiles                                  Summary
 389-ds              1.4                                                   389 Directory Server (base)
 ant                 1.10 [d]    common [d]                                Java build tool
+ant                 1.20        common [d]                                Java build tool
 
 Hint: [d]efault, [e]nabled, [x]disabled, [i]nstalled
 """.strip()
 
 DNF_MODULE_LIST_EXP1 = """
 Updating Subscription Management repositories.
 Cache-only enabled but no cache for 'rhel-8-for-x86_64-appstream-rpms', ignoring this repo.
@@ -180,15 +184,43 @@
 """.strip()
 
 
 def test_dnf_module_list():
     module_list = DnfModuleList(context_wrap(DNF_MODULE_LIST))
     assert 'ant' in module_list
     assert module_list['httpd'].name == 'httpd'
-    assert module_list['httpd'].stream == '2.4 [d][e]'
+    assert module_list['httpd'].streams[0].stream == '2.4'
+    assert module_list['httpd'].streams[0].default
+    assert module_list['httpd'].streams[0].enabled
+    assert module_list['httpd'].streams[0].active
+    assert module_list['postgresql'].streams[0].stream == '10'
+    assert not module_list['postgresql'].streams[0].enabled
+    assert module_list['postgresql'].streams[0].active
+    assert module_list['postgresql'].streams[0].default
+    assert module_list['postgresql'].streams[1].stream == '9.6'
+    assert not module_list['postgresql'].streams[1].enabled
+    assert not module_list['postgresql'].streams[1].active
+    assert not module_list['postgresql'].streams[1].default
+    assert module_list['ruby'].streams[0].stream == '2.5'
+    assert module_list['ruby'].streams[0].default
+    assert not module_list['ruby'].streams[0].enabled
+    assert not module_list['ruby'].streams[0].active
+    assert module_list['ruby'].streams[1].stream == '2.6'
+    assert module_list['ruby'].streams[1].enabled
+    assert module_list['ruby'].streams[1].active
+    assert not module_list['ruby'].streams[1].default
+    assert module_list['ruby'].streams[2].stream == '2.7'
+    assert not module_list['ruby'].streams[2].enabled
+    assert not module_list['ruby'].streams[2].active
+    assert not module_list['ruby'].streams[2].default
+    assert module_list['default_disabled'].streams[0].stream == '1.0'
+    assert module_list['default_disabled'].streams[0].default
+    assert module_list['default_disabled'].streams[0].disabled
+    assert not module_list['default_disabled'].streams[0].enabled
+    assert not module_list['default_disabled'].streams[0].active
 
 
 def test_dnf_module_list_exp():
     with pytest.raises(ValueError):
         DnfModuleList(context_wrap(DNF_MODULE_LIST_EXP1))
 
     with pytest.raises(SkipComponent):
@@ -198,17 +230,17 @@
 def test_dnf_module_info():
     module_infos = DnfModuleInfo(context_wrap(DNF_MODULE_INFO))
     assert len(module_infos) == 3
     assert module_infos.modules == ['389-ds', 'ant', 'httpd']
     assert len(module_infos['httpd']) == 2
     assert module_infos['httpd'][0].name == 'httpd'
     assert module_infos['httpd'][0].version == '8000020190405071959'
-    assert len(module_infos['httpd'][0].profiles) == 3
+    assert len(module_infos['httpd'][0].streams[0].profiles) == 3
     assert module_infos['httpd'][0].default_profiles == 'common'
-    assert module_infos['httpd'][1].summary == 'Apache HTTP Server'
+    assert module_infos['httpd'][1].streams[0].summary == 'Apache HTTP Server'
     assert module_infos['httpd'][1].context == '9edba152'
     assert 'mod_http2-0:1.11.3-1.module+el8+2443+605475b7.x86_64' in module_infos['httpd'][1].artifacts
 
 
 def test_dnf_module_info_exp():
     with pytest.raises(SkipComponent):
         DnfModuleInfo(context_wrap(DNF_MODULE_INFO_EXP))
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dnf_modules.py` & `insights-core-3.2.0/insights/tests/parsers/test_dnf_modules.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dnsmasq_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_dnsmasq_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_docker_info.py` & `insights-core-3.2.0/insights/tests/parsers/test_docker_info.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_docker_inspect.py` & `insights-core-3.2.0/insights/tests/parsers/test_docker_inspect.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_docker_list.py` & `insights-core-3.2.0/insights/tests/parsers/test_docker_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dotnet.py` & `insights-core-3.2.0/insights/tests/parsers/test_dotnet.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_doveconf.py` & `insights-core-3.2.0/insights/tests/parsers/test_doveconf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dracut_modules.py` & `insights-core-3.2.0/insights/tests/parsers/test_dracut_modules.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dse_ldif_simple.py` & `insights-core-3.2.0/insights/tests/parsers/test_dse_ldif_simple.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_du.py` & `insights-core-3.2.0/insights/tests/parsers/test_du.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_dumpe2fs_h.py` & `insights-core-3.2.0/insights/tests/parsers/test_dumpe2fs_h.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_engine_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_engine_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_engine_db_query.py` & `insights-core-3.2.0/insights/tests/parsers/test_engine_db_query.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_engine_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_engine_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_etcd_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_etcd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ethtool.py` & `insights-core-3.2.0/insights/tests/parsers/test_ethtool.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_facter.py` & `insights-core-3.2.0/insights/tests/parsers/test_facter.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_fapolicyd_rules.py` & `insights-core-3.2.0/insights/tests/parsers/test_fapolicyd_rules.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_fc_match.py` & `insights-core-3.2.0/insights/tests/parsers/test_fc_match.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_fcoeadm_i.py` & `insights-core-3.2.0/insights/tests/parsers/test_fcoeadm_i.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_findmnt.py` & `insights-core-3.2.0/insights/tests/parsers/test_findmnt.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_firewall_cmd.py` & `insights-core-3.2.0/insights/tests/parsers/test_firewall_cmd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_foreman_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_foreman_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_firewall_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_firewall_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_foreman_proxy_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_foreman_proxy_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_foreman_rake_db_migrate_status.py` & `insights-core-3.2.0/insights/tests/parsers/test_foreman_rake_db_migrate_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_freeipa_healthcheck_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_freeipa_healthcheck_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_fstab.py` & `insights-core-3.2.0/insights/tests/parsers/test_fstab.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,14 +38,20 @@
 ## default mount options##
 /dev/foo /foo somefs
 ###SIMBOX MOUNT###
 192.168.48.65:/cellSiteData /ceSiteData nfs
     /dev/vg_data/lv_pg /var/opt/rh/rh-postgresql95/lib/pgsql  xfs rw,noatime        0        0
 """
 
+FSTAB_DUPLICATE_MOUNT = """
+UUID=94ea609a-7ed9-4b3d-a33c-59db91b945df   /       xfs     defaults        0 0
+UUID=05ce4fc3-04c3-4111-xxxx                /boot   ext4    defaults        1 2
+UUID=94ea609a-7ed9-4b3d-a33c-59db91b945df   /lvm2   xfs     defaults,noexec        0 0
+""".strip()
+
 
 def test_fstab():
     context = context_wrap(FS_TAB_DATA)
     results = fstab.FSTab(context)
     assert results is not None
     assert len(results) == 10
     sdb1 = None
@@ -146,7 +152,19 @@
                        '/tmp/vm tools': '/dev/sda2',
                        '/l ok/at/you': '/dev/sdb5',
                        '/l ok': '/dev/sda2',  # dict treat '/l\040ok' same as '/l ok'
                        r'/l\040ok': '/dev/sda2',
                        }
     for path, dev in path_device_map.items():
         assert dev == fstab_info.fsspec_of_path(path)
+
+
+def test_fstab_with_duplicated_mount():
+    fstab_info = fstab.FSTab(context_wrap(FSTAB_DUPLICATE_MOUNT))
+    for entry in fstab_info:
+        mount_target = entry.fs_file
+        fs_spec = entry.fs_spec
+        if fs_spec == 'UUID=94ea609a-7ed9-4b3d-a33c-59db91b945df':
+            if mount_target == '/':
+                assert 'noexec' not in entry.raw
+            if mount_target == 'lvm2':
+                assert 'noexec' in entry.raw
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_fwupdagent.py` & `insights-core-3.2.0/insights/tests/parsers/test_fwupdagent.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_galera_cnf.py` & `insights-core-3.2.0/insights/tests/parsers/test_galera_cnf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_gcp_instance_type.py` & `insights-core-3.2.0/insights/tests/parsers/test_gcp_instance_type.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_gcp_license_codes.py` & `insights-core-3.2.0/insights/tests/parsers/test_gcp_license_codes.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_getcert_list.py` & `insights-core-3.2.0/insights/tests/parsers/test_getcert_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_getconf_pagesize.py` & `insights-core-3.2.0/insights/tests/parsers/test_getconf_pagesize.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_getenforce.py` & `insights-core-3.2.0/insights/tests/parsers/test_getenforce.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_getsebool.py` & `insights-core-3.2.0/insights/tests/parsers/test_getsebool.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_gfs2_file_system_block_size.py` & `insights-core-3.2.0/insights/tests/parsers/test_gfs2_file_system_block_size.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_glance_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_glance_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_gluster_peer_status.py` & `insights-core-3.2.0/insights/tests/parsers/test_gluster_peer_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 State: Peer in Cluster (Connected)
 
 Hostname: 10.30.32.20
 Uuid: 4673e3-5e95-4c02-b9bb-2823483e067bb3
 State: Peer in Cluster (Disconnected)
 """.strip()
 
+OUTPUT_NG = """
+Connection failed. Please check if gluster daemon is operational.
+""".strip()
+
 
 def test_output():
     output = gluster_peer_status.GlusterPeerStatus(context_wrap(OUTPUT_1))
     assert output.status['peers'] == len(output.status.get('hosts', []))
     assert output.status.get('hosts', []) == [
         {'Hostname': 'versegluster1.verse.loc', 'State': 'Peer in Cluster (Connected)', 'Uuid': '86c0266b-c78c-4d0c-afe7-953dec143530'},
         {'Hostname': '10.30.32.16', 'State': 'Peer in Cluster (Connected)', 'Uuid': '3b4673e3-5e95-4c02-b9bb-2823483e067b'},
@@ -42,13 +46,19 @@
 
 def test_blank_output():
     with pytest.raises(SkipComponent) as e:
         gluster_peer_status.GlusterPeerStatus(context_wrap(""))
     assert "No data." in str(e)
 
 
+def test_failed_output():
+    with pytest.raises(SkipComponent) as e:
+        gluster_peer_status.GlusterPeerStatus(context_wrap(OUTPUT_NG))
+    assert "No data." in str(e)
+
+
 def test_documentation():
     failed_count, tests = doctest.testmod(
         gluster_peer_status,
         globs={'output': gluster_peer_status.GlusterPeerStatus(context_wrap(OUTPUT))}
     )
     assert failed_count == 0
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_gluster_vol.py` & `insights-core-3.2.0/insights/tests/parsers/test_gluster_vol.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_gnocchi.py` & `insights-core-3.2.0/insights/tests/parsers/test_gnocchi.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_greenboot_status.py` & `insights-core-3.2.0/insights/tests/parsers/test_greenboot_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_grub_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_grub_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_grub_conf_efi.py` & `insights-core-3.2.0/insights/tests/parsers/test_grub_conf_efi.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_grub_conf_kdump.py` & `insights-core-3.2.0/insights/tests/parsers/test_grub_conf_kdump.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_grub_conf_missing_boot_files.py` & `insights-core-3.2.0/insights/tests/parsers/test_grub_conf_missing_boot_files.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_grubby.py` & `insights-core-3.2.0/insights/tests/parsers/test_rndc_status.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 import doctest
 import pytest
 
 from insights.core.exceptions import ParseException, SkipComponent
-from insights.parsers import grubby
-from insights.parsers.grubby import GrubbyDefaultIndex, GrubbyDefaultKernel
+from insights.parsers import rndc_status
+from insights.parsers.rndc_status import RndcStatus
 from insights.tests import context_wrap
 
-DEFAULT_INDEX_1 = '0'
-DEFAULT_INDEX_2 = '1'
-ABDEFAULT_INDEX_EMPTY = ''
-DEFAULT_INDEX_AB = '-2'
-
-DEFAULT_KERNEL = "/boot/vmlinuz-2.6.32-573.el6.x86_64"
-DEFAULT_KERNEL_EMPTY = ""
-DEFAULT_KERNEL_AB = """
-/boot/vmlinuz-2.6.32-573.el6.x86_64"
-/boot/vmlinuz-2.6.32-573.el6.x86_64"
+RNDC_STATUS = """
+version: BIND 9.11.4-P2-RedHat-9.11.4-9.P2.el7 (Extended Support Version) <id:7107deb>
+running on rhel7: Linux x86_64 3.10.0-957.10.1.el7.x86_64 #1 SMP Thu Feb 7 07:12:53 UTC 2019
+boot time: Mon, 26 Aug 2019 02:17:03 GMT
+last configured: Mon, 26 Aug 2019 02:17:03 GMT
+configuration file: /etc/named.conf
+CPUs found: 4
+worker threads: 4
+UDP listeners per interface: 3
+number of zones: 103 (97 automatic)
+debug level: 0
+xfers running: 0
+xfers deferred: 0
+soa queries in progress: 0
+query logging is OFF
+recursive clients: 0/900/1000
+tcp clients: 1/150
+server is up and running
 """.strip()
-DEFAULT_KERNEL_INVALID = 'rpm-sort: Invalid input'
 
+RNDC_STATUS_INVALID = """
+invalid
+invalid
+invalid
+""".strip()
 
-def test_grubby_default_index():
-    res = GrubbyDefaultIndex(context_wrap(DEFAULT_INDEX_1))
-    assert res.default_index == 0
-
-    res = GrubbyDefaultIndex(context_wrap(DEFAULT_INDEX_2))
-    assert res.default_index == 1
-
-
-def test_grubby_default_index_ab():
-    with pytest.raises(SkipComponent) as excinfo:
-        GrubbyDefaultIndex(context_wrap(ABDEFAULT_INDEX_EMPTY))
-    assert 'Empty output' in str(excinfo.value)
-
-    with pytest.raises(ParseException) as excinfo:
-        GrubbyDefaultIndex(context_wrap(DEFAULT_INDEX_AB))
-    assert 'Invalid output:' in str(excinfo.value)
+RNDC_STATUS_EMPTY = """
+""".strip()
 
 
-def test_grubby_default_kernel_ab():
-    with pytest.raises(SkipComponent) as excinfo:
-        GrubbyDefaultKernel(context_wrap(DEFAULT_KERNEL_EMPTY))
-    assert 'Empty output' in str(excinfo.value)
+def test_rndc_status():
+    rndc_status = RndcStatus(context_wrap(RNDC_STATUS))
+    assert rndc_status['boot time'] == 'Mon, 26 Aug 2019 02:17:03 GMT'
+    assert rndc_status['server'] == 'up and running'
 
-    with pytest.raises(ParseException) as excinfo:
-        GrubbyDefaultKernel(context_wrap(DEFAULT_KERNEL_AB))
-    assert 'Invalid output:' in str(excinfo.value)
 
-    with pytest.raises(ParseException) as excinfo:
-        GrubbyDefaultKernel(context_wrap(DEFAULT_KERNEL_INVALID))
-    assert 'Invalid output:' in str(excinfo.value)
+def test_invalid():
+    with pytest.raises(ParseException) as e:
+        RndcStatus(context_wrap(RNDC_STATUS_INVALID))
+    assert "invalid" in str(e)
 
 
-def test_grubby_default_kernel():
-    res = GrubbyDefaultKernel(context_wrap(DEFAULT_KERNEL))
-    assert res.default_kernel == DEFAULT_KERNEL
+def test_empty():
+    with pytest.raises(SkipComponent) as e:
+        RndcStatus(context_wrap(RNDC_STATUS_EMPTY))
+    assert "Empty content" in str(e)
 
 
-def test_doc_examples():
+def test_rndc_status_doc_examples():
     env = {
-            'grubby_default_index': GrubbyDefaultIndex(context_wrap(DEFAULT_INDEX_1)),
-            'grubby_default_kernel': GrubbyDefaultKernel(context_wrap(DEFAULT_KERNEL)),
-          }
-    failed, total = doctest.testmod(grubby, globs=env)
+        'rndc_status': RndcStatus(
+            context_wrap(RNDC_STATUS)),
+    }
+    failed, total = doctest.testmod(rndc_status, globs=env)
     assert failed == 0
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_grubenv.py` & `insights-core-3.2.0/insights/tests/parsers/test_grubenv.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_hammer_ping.py` & `insights-core-3.2.0/insights/tests/parsers/test_hammer_ping.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_hammer_task_list.py` & `insights-core-3.2.0/insights/tests/parsers/test_hammer_task_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_haproxy_cfg.py` & `insights-core-3.2.0/insights/tests/parsers/test_haproxy_cfg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_heat_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_heat_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_heat_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_heat_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_hostname.py` & `insights-core-3.2.0/insights/tests/parsers/test_hostname.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_hosts.py` & `insights-core-3.2.0/insights/tests/parsers/test_hosts.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_hponcfg.py` & `insights-core-3.2.0/insights/tests/parsers/test_hponcfg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_httpd_M.py` & `insights-core-3.2.0/insights/tests/parsers/test_httpd_M.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_httpd_V.py` & `insights-core-3.2.0/insights/tests/parsers/test_httpd_V.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_httpd_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_httpd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_httpd_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_httpd_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_httpd_open_nfs.py` & `insights-core-3.2.0/insights/tests/parsers/test_httpd_open_nfs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ibm_proc.py` & `insights-core-3.2.0/insights/tests/parsers/test_ibm_proc.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ifcfg.py` & `insights-core-3.2.0/insights/tests/parsers/test_ifcfg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_imagemagick_policy.py` & `insights-core-3.2.0/insights/tests/parsers/test_imagemagick_policy.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_init_process_cgroup.py` & `insights-core-3.2.0/insights/tests/parsers/test_init_process_cgroup.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_initscript.py` & `insights-core-3.2.0/insights/tests/parsers/test_initscript.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_insights_client_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_insights_client_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_installed_product_ids.py` & `insights-core-3.2.0/insights/tests/parsers/test_installed_product_ids.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_installed_rpms.py` & `insights-core-3.2.0/insights/tests/parsers/test_installed_rpms.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,14 +64,34 @@
 {"name": "jline","version": "1.0","epoch": "(none)","release": "8.el7","arch": "noarch","installtime": "Thu 02 Jun 2016 05:10:32 PM EDT","buildtime": "1388212830","rsaheader": "RSA/SHA256, Tue 01 Apr 2014 02:54:16 PM EDT, Key ID 199e2f91fd431d51","dsaheader": "(none)","srpm": "jline-1.0-8.el7.src.rpm"}
 {"name": "libteam","version": "1.17","epoch": "(none)","release": "6.el7_2","arch": "x86_64","installtime": "Fri 24 Jun 2016 04:18:17 PM EDT","buildtime": "1454604485","rsaheader": "RSA/SHA256, Wed 17 Feb 2016 02:25:16 AM EST, Key ID 199e2f91fd431d51","dsaheader": "(none)","srpm": "libteam-1.17-6.el7_2.src.rpm"}
 {"name": "crash","epoch":"(none)","version":"7.1.0","release":"8.el6","arch":"x86_64","installtime":"Fri Jul 13 06:53:28 2018","buildtime":"1524061059","vendor":"Red Hat, Inc.","buildhost":"x86-032.build.eng.bos.redhat.com","sigpgp":"RSA/8, Wed Apr 18 10:40:59 2018, Key ID 199e2f91fd431d51"}
 {"name": "xorg-x11-drv-vmmouse","epoch":"(none)","version":"13.1.0","release":"1.el6","arch":"x86_64","installtime":"Thu Aug  4 12:23:32 2016","buildtime":"1447274489","vendor":"Red Hat, Inc.","buildhost":"x86-028.build.eng.bos.redhat.com","sigpgp":"RSA/8, Mon Apr 4 11:35:36 2016, Key ID 199e2f91fd431d51"}
 {"name": "libnl","epoch":"(none)","version":"1.1.4","release":"2.el6","arch":"x86_64","installtime":"Mon Jun 16 13:21:21 2014","buildtime":"1378459378","vendor":"(none)","buildhost":"x86-007.build.bos.redhat.com","sigpgp":"RSA/8, Mon Sep 23 07:25:47 2013, Key ID 199e2f91fd431d51"}
 '''.strip()
 
+RPMS_JSON_W_WARNING = '''
+warning: Signature not supported. Hash algorithm SHA1 not available.
+{"name": "util-linux","version": "2.23.2","epoch": "(none)","release": "26.el7_2.2","arch": "x86_64","installtime": "Fri 24 Jun 2016 04:17:58 PM EDT","buildtime": "1458159298","rsaheader": "RSA/SHA256, Sun 20 Mar 2016 10:00:45 PM EDT, Key ID 199e2f91fd431d51","dsaheader": "(none)","srpm": "util-linux-2.23.2-26.el7_2.2.src.rpm"}
+{"name": "libestr","version": "0.1.9","epoch": "(none)","release": "2.el7","arch": "x86_64","installtime": "Fri 06 May 2016 03:53:26 PM EDT","buildtime": "1390734694","rsaheader": "RSA/SHA256, Tue 01 Apr 2014 04:49:20 PM EDT, Key ID 199e2f91fd431d51","dsaheader": "(none)","srpm": "libestr-0.1.9-2.el7.src.rpm"}
+{"name": "log4j","version": "1.2.17","epoch": "0","release": "15.el7","arch": "noarch","installtime": "Thu 02 Jun 2016 05:10:29 PM EDT","buildtime": "1388247429","rsaheader": "RSA/SHA256, Wed 02 Apr 2014 11:25:59 AM EDT, Key ID 199e2f91fd431d51","dsaheader": "(none)","srpm": "log4j-1.2.17-15.el7.src.rpm"}
+{"name": "kbd-misc","version": "1.15.5","epoch": "(none)","release": "11.el7","arch": "noarch","installtime": "Fri 06 May 2016 03:52:06 PM EDT","buildtime": "1412004323","rsaheader": "RSA/SHA256, Tue 16 Dec 2014 10:02:15 AM EST, Key ID 199e2f91fd431d51","dsaheader": "(none)","srpm": "kbd-1.15.5-11.el7.src.rpm"}
+{"name": "grub2-tools","version": "2.02","epoch": "1","release": "0.34.el7_2","arch": "x86_64","installtime": "Fri 24 Jun 2016 04:18:01 PM EDT","buildtime": "1450199819","rsaheader": "RSA/SHA256, Wed 23 Dec 2015 04:22:27 AM EST, Key ID 199e2f91fd431d51","dsaheader": "(none)","srpm": "grub2-2.02-0.34.el7_2.src.rpm"}
+{"name": "kbd-legacy","version": "1.15.5","epoch": "(none)","release": "11.el7","arch": "noarch","installtime": "Fri 06 May 2016 03:53:32 PM EDT","buildtime": "1412004323","rsaheader": "RSA/SHA256, Tue 16 Dec 2014 10:02:14 AM EST, Key ID 199e2f91fd431d51","dsaheader": "(none)","srpm": "kbd-1.15.5-11.el7.src.rpm"}
+{"name": "jboss-servlet-3.0-api","version": "1.0.1","epoch": "(none)","release": "9.el7","arch": "noarch","installtime": "Thu 02 Jun 2016 05:10:30 PM EDT","buildtime": "1388211302","rsaheader": "RSA/SHA256, Tue 01 Apr 2014 02:51:30 PM EDT, Key ID 199e2f91fd431d51","dsaheader": "(none)","srpm": "jboss-servlet-3.0-api-1.0.1-9.el7.src.rpm"}
+{"name": "bash","version": "4.2.46","epoch": "(none)","release": "19.el7","arch": "x86_64","installtime": "Fri 06 May 2016 03:52:13 PM EDT","buildtime": "1436354006","rsaheader": "RSA/SHA256, Wed 07 Oct 2015 01:14:10 PM EDT, Key ID 199e2f91fd431d51","dsaheader": "(none)","srpm": "bash-4.2.46-19.el7.src.rpm"}
+{"name": "ca-certificates","version": "2015.2.6","epoch": "(none)","release": "70.1.el7_2","arch": "noarch","installtime": "Fri 24 Jun 2016 04:18:04 PM EDT","buildtime": "1453976868","rsaheader": "RSA/SHA256, Tue 02 Feb 2016 09:45:04 AM EST, Key ID 199e2f91fd431d51","dsaheader": "(none)","srpm": "ca-certificates-2015.2.6-70.1.el7_2.src.rpm"}
+{"name": "jline","version": "1.0","epoch": "(none)","release": "8.el7","arch": "noarch","installtime": "Thu 02 Jun 2016 05:10:32 PM EDT","buildtime": "1388212830","rsaheader": "RSA/SHA256, Tue 01 Apr 2014 02:54:16 PM EDT, Key ID 199e2f91fd431d51","dsaheader": "(none)","srpm": "jline-1.0-8.el7.src.rpm"}
+{"name": "libteam","version": "1.17","epoch": "(none)","release": "6.el7_2","arch": "x86_64","installtime": "Fri 24 Jun 2016 04:18:17 PM EDT","buildtime": "1454604485","rsaheader": "RSA/SHA256, Wed 17 Feb 2016 02:25:16 AM EST, Key ID 199e2f91fd431d51","dsaheader": "(none)","srpm": "libteam-1.17-6.el7_2.src.rpm"}
+{"name": "crash","epoch":"(none)","version":"7.1.0","release":"8.el6","arch":"x86_64","installtime":"Fri Jul 13 06:53:28 2018","buildtime":"1524061059","vendor":"Red Hat, Inc.","buildhost":"x86-032.build.eng.bos.redhat.com","sigpgp":"RSA/8, Wed Apr 18 10:40:59 2018, Key ID 199e2f91fd431d51"}
+{"name": "xorg-x11-drv-vmmouse","epoch":"(none)","version":"13.1.0","release":"1.el6","arch":"x86_64","installtime":"Thu Aug  4 12:23:32 2016","buildtime":"1447274489","vendor":"Red Hat, Inc.","buildhost":"x86-028.build.eng.bos.redhat.com","sigpgp":"RSA/8, Mon Apr 4 11:35:36 2016, Key ID 199e2f91fd431d51"}
+warning: Signature not supported. Hash algorithm SHA1 not available.
+{"name": "libnl","epoch":"(none)","version":"1.1.4","release":"2.el6","arch":"x86_64","installtime":"Mon Jun 16 13:21:21 2014","buildtime":"1378459378","vendor":"(none)","buildhost":"x86-007.build.bos.redhat.com","sigpgp":"RSA/8, Mon Sep 23 07:25:47 2013, Key ID 199e2f91fd431d51"}
+warning: Signature not supported. Hash algorithm SHA1 not available.
+'''.strip()
+
 RPMS_MULTIPLE = '''
 yum-3.4.3-132.el7.noarch
 yum-3.4.2-132.el7.noarch
 '''
 
 RPMS_MULTIPLE_KERNEL = '''
 kernel-3.10.0-327.el7.x86_64
@@ -220,14 +240,28 @@
     assert rpms.get_max("util-linux").epoch == '0'
     assert rpms.get_max("jboss-servlet-3.0-api").redhat_signed
 
     assert rpms.newest('libnl').vendor == '(none)'
     assert rpms.newest('crash').vendor == 'Red Hat, Inc.'
     assert rpms.newest('log4j').vendor is None
 
+    rpms = InstalledRpms(context_wrap(RPMS_JSON_W_WARNING))
+    assert isinstance(rpms.get_max("log4j").source, InstalledRpm)
+    assert len(rpms.packages) == len(RPMS_JSON.splitlines())
+    assert rpms.get_max("log4j").source.name == "log4j"
+    assert rpms.get_max("util-linux").epoch == '0'
+    assert rpms.get_max("jboss-servlet-3.0-api").redhat_signed
+
+    assert rpms.newest('libnl').vendor == '(none)'
+    assert rpms.newest('crash').vendor == 'Red Hat, Inc.'
+    assert rpms.newest('log4j').vendor is None
+
+    assert len(rpms.errors) == 3
+    assert "warning: Signature not supported." in rpms.errors[0]
+
 
 def test_garbage():
     rpms = InstalledRpms(context_wrap(RPMS_PACKAGE_WITH_GARBAGE))
     assert 'openssh-server' not in rpms
 
 
 def test_corrupt_db():
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_interrupts.py` & `insights-core-3.2.0/insights/tests/parsers/test_interrupts.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ip.py` & `insights-core-3.2.0/insights/tests/parsers/test_ip.py`

 * *Files 4% similar despite different names*

```diff
@@ -315,20 +315,87 @@
     geneve id 11 remote 192.168.43.173 dstport 6081 noudpcsum udp6zerocsumrx addrgenmode eui64
     RX: bytes  packets  errors  dropped overrun mcast
     0          0        8       0       0       0
     TX: bytes  packets  errors  dropped carrier collsns
     536        8        0       0       0       0
 """.strip()
 
+IP_S_LINK_ALL_4 = """
+1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN mode DEFAULT group default qlen 1000
+    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00 promiscuity 0 minmtu 0 maxmtu 0 addrgenmode eui64 numtxqueues 1 numrxqueues 1 gso_max_size 65536 gso_max_segs 65535
+    RX: bytes  packets  errors  dropped missed  mcast
+    10409771   7627     0       0       0       0
+    TX: bytes  packets  errors  dropped carrier collsns
+    10409771   7627     0       0       0       0
+3: ens1f0: <BROADCAST,MULTICAST,SLAVE,UP,LOWER_UP> mtu 1500 qdisc mq master bond1 state UP mode DEFAULT group default qlen 1000
+    link/ether b4:96:91:e5:c8:a8 brd ff:ff:ff:ff:ff:ff promiscuity 1 minmtu 68 maxmtu 9702
+    bond_slave state ACTIVE mii_status UP link_failure_count 0 perm_hwaddr b4:96:91:e5:c8:a8 queue_id 0 addrgenmode none numtxqueues 112 numrxqueues 112 gso_max_size 65536 gso_max_segs 65535
+    RX: bytes  packets  errors  dropped missed  mcast
+    3486063351 2629875  0       0       0       3064
+    TX: bytes  packets  errors  dropped carrier collsns
+    259638429  543551   0       0       0       0
+7: ens1f1: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc mq state UP mode DEFAULT group default qlen 1000
+    link/ether b4:96:91:e5:c8:a9 brd ff:ff:ff:ff:ff:ff promiscuity 0 minmtu 68 maxmtu 9702 addrgenmode none numtxqueues 112 n
+umrxqueues 112 gso_max_size 65536 gso_max_segs 65535
+    RX: bytes  packets  errors  dropped missed  mcast
+    17496609   257835   0       67      0       792
+    TX: bytes  packets  errors  dropped carrier collsns
+    33991      231      0       0       0       0
+    vf 0     link/ether 6e:cc:c3:fe:ad:7f brd ff:ff:ff:ff:ff:ff, spoof checking on, link-state auto, trust off
+    RX: bytes  packets  mcast   bcast   dropped
+    14069717   192865   0       192865  192865
+    TX: bytes  packets   dropped
+    0          0        0
+    vf 1     link/ether c6:5b:b6:3c:db:f1 brd ff:ff:ff:ff:ff:ff, spoof checking on, link-state auto, trust off
+    RX: bytes  packets  mcast   bcast   dropped
+    14069717   192865   0       192865  192865
+    TX: bytes  packets   dropped
+    0          0        0
+    vf 2     link/ether f6:a4:d0:2d:a5:a1 brd ff:ff:ff:ff:ff:ff, spoof checking on, link-state auto, trust off
+    RX: bytes  packets  mcast   bcast   dropped
+    14069717   192865   0       192865  192865
+    TX: bytes  packets   dropped
+    0          0        0
+    vf 3     link/ether 92:50:97:c4:9d:f0 brd ff:ff:ff:ff:ff:ff, spoof checking on, link-state auto, trust off
+    RX: bytes  packets  mcast   bcast   dropped
+    14069717   192865   0       192865  192865
+    TX: bytes  packets   dropped
+    0          0        0
+91: ens1f1v64: <BROADCAST,MULTICAST> mtu 1500 qdisc noop state DOWN mode DEFAULT group default qlen 1000
+    link/ether 76:47:d1:15:9f:59 brd ff:ff:ff:ff:ff:ff promiscuity 0 minmtu 68 maxmtu 9702 addrgenmode eui64 numtxqueues 16 numrxqueues 16 gso_max_size 65536 gso_max_segs 65535
+    RX: bytes  packets  errors  dropped missed  mcast
+    0          0        0       0       0       0
+    TX: bytes  packets  errors  dropped carrier collsns
+    0          0        0       0       0       0
+""".strip()
+
+IP_S_LINK_ALL_5 = """
+1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN mode DEFAULT group default qlen 1000
+    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00 promiscuity 0 minmtu 0 maxmtu 0 addrgenmode eui64 numtxqueues 1 numrxqueues 1 gso_max_size 65536 gso_max_segs 65535
+    RX: bytes  packets  errors  dropped missed  mcast
+    10409771   7627     0       0       0       0
+    TX: bytes  packets  errors  dropped carrier collsns
+    10409771   7627     0       0       0       0
+2: ens1: <BROADCAST,MULTICAST,SLAVE,UP,LOWER_UP> mtu 1500 qdisc mq master bond1 state UP mode DEFAULT group default qlen 1000 unpaired_attr
+    link/ether b4:96:91:e5:c8:a8 brd ff:ff:ff:ff:ff:ff promiscuity 1 minmtu 68 maxmtu 9702
+    bond_slave state ACTIVE mii_status UP link_failure_count 0 perm_hwaddr b4:96:91:e5:c8:a8 queue_id 0 addrgenmode none numtxqueues 112 numrxqueues 112 gso_max_size 65536 gso_max_segs 65535
+    RX: bytes  packets  errors  dropped missed  mcast
+    3486063351 2629875  0       0       0       3064
+    TX: bytes  packets  errors  dropped carrier collsns
+    259638429  543551   0       0       0       0
+""".strip()
+
 
 def test_ip_data_Link():
     link_info = ip.IpLinkInfo(context_wrap(IP_S_LINK))
     link_info_all = ip.IpLinkInfo(context_wrap(IP_S_LINK_ALL))
     link_info_all_2 = ip.IpLinkInfo(context_wrap(IP_S_LINK_ALL_2))
     link_info_all_3 = ip.IpLinkInfo(context_wrap(IP_S_LINK_ALL_3))
+    link_info_all_4 = ip.IpLinkInfo(context_wrap(IP_S_LINK_ALL_4))
+    link_info_all_5 = ip.IpLinkInfo(context_wrap(IP_S_LINK_ALL_5))
     if_list_all_3 = link_info_all_3.active
     assert sorted(if_list_all_3) == sorted(['lo', 'eth0_1', 'eth0_2', 'vxlan_sys_4789', 'gre1', 'geneve0', 'geneve1'])
     eth0_1 = link_info_all_3["eth0_1"]
     assert eth0_1["mac"] == "00:90:fa:8d:36:1e"
     assert eth0_1["rx_packets"] == 15139642734
     assert eth0_1["rx_bytes"] == 16809815066893
     if_list_all_2 = link_info_all_2.active
@@ -382,14 +449,22 @@
     assert tm0["mac"] == "d4:f5:ef:01:1a:3c"
     assert tm0["flags"] == ['BROADCAST', 'MULTICAST', 'UP', 'LOWER_UP']
     assert tm0["type"] == "ether"
     assert tm0["mtu"] == 1500
     assert tm0['promiscuity'] == '1'
     assert tm0["rx_packets"] == 11784
 
+    ens1f0 = link_info_all_4["ens1f0"]
+    assert ens1f0["vf_enabled"] is False
+    ens1f1 = link_info_all_4["ens1f1"]
+    assert ens1f1["vf_enabled"] is True
+
+    ens1 = link_info_all_5["ens1"]
+    assert ens1["qlen"] == 1000
+
 
 IP_ROUTE_SHOW_TABLE_ALL_TEST = """
 throw 30.142.64.0/26  table red_mgmt
 default via 30.142.64.1 dev bond0.400  table red_mgmt
 throw 30.142.34.0/26  table red_storage
 default via 30.142.34.1 dev bond0.300  table red_storage
 30.0.0.0/8 dev notExist proto kernel scope link src 30.0.0.1
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ip_netns_exec_namespace_lsof.py` & `insights-core-3.2.0/insights/tests/parsers/test_ip_netns_exec_namespace_lsof.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ipaupgrade_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_ipaupgrade_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ipcs.py` & `insights-core-3.2.0/insights/tests/parsers/test_ipcs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ipsec_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_ipsec_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_iptables.py` & `insights-core-3.2.0/insights/tests/parsers/test_iptables.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ironic_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_ironic_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ironic_inspector_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_ironic_inspector_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_iscsiadm_mode_session.py` & `insights-core-3.2.0/insights/tests/parsers/test_iscsiadm_mode_session.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_jboss_domain_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_jboss_domain_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_jboss_standalone_main_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_jboss_standalone_main_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_jboss_version.py` & `insights-core-3.2.0/insights/tests/parsers/test_jboss_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_journal_all.py` & `insights-core-3.2.0/insights/tests/test_syslog.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,38 @@
-from insights.parsers.journal_all import JournalAll
+from insights.core import Syslog
 from insights.tests import context_wrap
 
 MSGINFO = """
--- Logs begin at Wed 2017-02-08 15:18:00 CET, end at Tue 2017-09-19 09:12:59 CEST. --
-May 18 15:13:34 lxc-rhel68-sat56 jabberd/sm[11057]: session started: jid=rhn-dispatcher-sat@lxc-rhel6-sat56.redhat.com/superclient
-May 18 15:13:36 lxc-rhel68-sat56 wrapper[11375]: --> Wrapper Started as Daemon
-May 18 15:13:36 lxc-rhel68-sat56 wrapper[11375]: Launching a JVM...
-May 18 15:24:28 lxc-rhel68-sat56 yum[11597]: Installed: lynx-2.8.6-27.el6.x86_64
-May 18 15:36:19 lxc-rhel68-sat56 yum[11954]: Updated: sos-3.2-40.el6.noarch
 Apr 22 10:35:01 boy-bona CROND[27921]: (root) CMD (/usr/lib64/sa/sa1 -S DISK 1 1)
 Apr 22 10:37:32 boy-bona crontab[28951]: (root) LIST (root)
 Apr 22 10:40:01 boy-bona CROND[30677]: (root) CMD (/usr/lib64/sa/sa1 -S DISK 1 1)
 Apr 22 10:41:13 boy-bona crontab[32515]: (root) LIST (root)
+Apr 29 11:33:36 kvmr7u5 ehtest: crontab[12345]: {
+April 29 11:33:36 kvmr7u5 ehtest: crontab[12345]: { # this line will be skipped by `_parse_line`
+May  5 03:50:01 kvmr7u5 systemd: Removed slice user-0.slice.
+May  9 15:13:34 lxc-rhel68-sat56 jabberd/sm[11057]: session started: jid=rhn-dispatcher-sat@lxc-rhel6-sat56.redhat.com/superclient
+May  9 15:13:36 lxc-rhel68-sat56 wrapper[11375]: --> Wrapper Started as Daemon
+May  9 15:13:36 lxc-rhel68-sat56 wrapper[11375]: Launching a JVM...
+May 10 15:24:28 lxc-rhel68-sat56 yum[11597]: Installed: lynx-2.8.6-27.el6.x86_64
+May 10 15:36:19 lxc-rhel68-sat56 yum[11954]: Updated: sos-3.2-40.el6.noarch
 """.strip()
 
 
-def test_messages():
-    msg_info = JournalAll(context_wrap(MSGINFO))
+def test_syslog():
+    msg_info = Syslog(context_wrap(MSGINFO))
     bona_list = msg_info.get('(root) LIST (root)')
     assert 2 == len(bona_list)
     assert bona_list[0].get('timestamp') == "Apr 22 10:37:32"
     assert bona_list[1].get('timestamp') == "Apr 22 10:41:13"
     crond = msg_info.get('CROND')
     assert 2 == len(crond)
     assert crond[0].get('procname') == "CROND[27921]"
     assert msg_info.get('jabberd/sm[11057]')[0].get('hostname') == "lxc-rhel68-sat56"
     assert msg_info.get('Wrapper')[0].get('message') == "--> Wrapper Started as Daemon"
-    assert msg_info.get('Launching')[0].get('raw_message') == "May 18 15:13:36 lxc-rhel68-sat56 wrapper[11375]: Launching a JVM..."
+    assert msg_info.get('Launching')[0].get('raw_message') == "May  9 15:13:36 lxc-rhel68-sat56 wrapper[11375]: Launching a JVM..."
     assert 2 == len(msg_info.get('yum'))
+    crontab_logs = list(msg_info.get_logs_by_procname('crontab'))
+    assert len(crontab_logs) == 2
+    assert crontab_logs[1]['raw_message'] == "Apr 22 10:41:13 boy-bona crontab[32515]: (root) LIST (root)"
+    systemd_logs = list(msg_info.get_logs_by_procname('systemd'))
+    assert len(systemd_logs) == 1
+    assert systemd_logs[0]['timestamp'] == 'May  5 03:50:01'
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_journalctl.py` & `insights-core-3.2.0/insights/tests/parsers/test_journalctl.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_journald_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_journald_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_katello_service_status.py` & `insights-core-3.2.0/insights/tests/parsers/test_katello_service_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_kdump.py` & `insights-core-3.2.0/insights/tests/parsers/test_kdump.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_kernel_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_kernel_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_keystone.py` & `insights-core-3.2.0/insights/tests/parsers/test_keystone.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_keystone_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_keystone_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_kpatch_list.py` & `insights-core-3.2.0/insights/tests/parsers/test_kpatch_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_krb5.py` & `insights-core-3.2.0/insights/tests/parsers/test_krb5.py`

 * *Files 26% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 KRB5_CONF_PATH = "etc/krb5.conf"
 KRB5_DCONF_PATH = "etc/krb5.conf.d/test.conf"
 
 
 def test_krb5configuration():
     common_conf_info = krb5.Krb5Configuration(context_wrap(KRB5CONFIG, path=KRB5_CONF_PATH))
     assert common_conf_info["libdefaults"]["dnsdsd"] == "false"
+    assert common_conf_info.getboolean("libdefaults", "dnsdsd") is False
     assert "renew_lifetime" not in common_conf_info.data.keys()
     assert common_conf_info["realms"]["EXAMPLE.COM"]["kdc"] == "kerberos.example.com"
     assert common_conf_info["realms"]["default_ccache_name"] == "KEYRING:persistent:%{uid}"
     assert common_conf_info["libdefaults"]["default_ccache_name"] == "KEYRING:%{uid}:persistent"
     assert common_conf_info["realms"]["kdc_default_options"] == ["default.example.com", "default2.example.com"]
     assert "realms" in common_conf_info.sections()
     assert "realmstest" not in common_conf_info.sections()
@@ -123,14 +124,16 @@
     assert common_conf_info.include == ["/etc/krb5test.conf"]
     assert common_conf_info.includedir == ["/etc/krb5.conf.d/"]
     assert common_conf_info.module == ["/etc/krb5test.conf:residual"]
 
     common_conf_info = krb5.Krb5Configuration(context_wrap(KRB5CONFIG3, path=KRB5_CONF_PATH))
     assert len(common_conf_info.sections()) == 4
     assert common_conf_info.has_section('domain_realm') is True
+    assert common_conf_info.getboolean("libdefaults", "forwardable") is True
+    assert common_conf_info.getboolean("libdefaults", "renew_lifetime") is None
     assert sorted(common_conf_info.options('logging')) == sorted(['default', 'kdc', 'admin_server'])
     assert common_conf_info.has_option('libdefaults', 'dns_lookup_realm') is True
     assert common_conf_info.has_option('domain_realm', 'example.com') is False
 
 
 def test2_krb5configuration():
     common_conf_info = krb5.Krb5Configuration(context_wrap(KRB5CONFIG2, path=KRB5_CONF_PATH))
@@ -140,7 +143,18 @@
 def test_krb5Dconfiguration():
     common_conf_info = krb5.Krb5Configuration(context_wrap(KRB5DCONFIG, path=KRB5_DCONF_PATH))
     assert common_conf_info["realms"]["ticket_lifetime"] == "24h"
     assert "default_ccache_name" not in common_conf_info.data.keys()
     assert common_conf_info["realms"]["EXAMPLE.COM"]["kdc"] == ['kerberos.example.com', 'test2.example.com', 'test3.example.com']
     assert common_conf_info.has_option("logging", "admin_server")
     assert common_conf_info["logging"]["kdc"] == "FILE:/var/log/krb5kdc.log"
+
+
+def test_handle_krb5_bool():
+    assert krb5._handle_krb5_bool("yes") is True
+    assert krb5._handle_krb5_bool("1") is True
+    assert krb5._handle_krb5_bool("on") is True
+    assert krb5._handle_krb5_bool("no") is False
+    assert krb5._handle_krb5_bool("false") is False
+    assert krb5._handle_krb5_bool("0") is False
+    assert krb5._handle_krb5_bool("unknown") is None
+    assert krb5._handle_krb5_bool("") is None
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_krb5kdc_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_krb5kdc_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ksmstate.py` & `insights-core-3.2.0/insights/tests/parsers/test_ksmstate.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ktimer_lockless.py` & `insights-core-3.2.0/insights/tests/parsers/test_ktimer_lockless.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_kubepods_cpu_quota.py` & `insights-core-3.2.0/insights/tests/parsers/test_kubepods_cpu_quota.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ld_library_path.py` & `insights-core-3.2.0/insights/tests/parsers/test_ld_library_path.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ldif_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_ldif_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_libssh_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_libssh_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_libvirtd_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_libvirtd_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_limits_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_limits_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_logrotate_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_logrotate_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_losetup.py` & `insights-core-3.2.0/insights/tests/parsers/test_losetup.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_lpstat.py` & `insights-core-3.2.0/insights/tests/parsers/test_lpstat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_boot.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_boot.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_dev.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_dev.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_disk.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_disk.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_docker_volumes.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_docker_volumes.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_edac_mc.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_edac_mc.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_etc.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_etc.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_ipa_idoverride_memberof.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_ipa_idoverride_memberof.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_krb5_sssd.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_krb5_sssd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_lib_firmware.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_lib_firmware.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_ocp_nci_openshift_sdn.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_ocp_nci_openshift_sdn.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_origin_local_volumes_pods.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_origin_local_volumes_pods.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_osroot.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_osroot.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_sys_firmware.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_sys_firmware.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_systemd_units.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_systemd_units.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_tmp.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_tmp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_usr_bin.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_usr_bin.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_usr_lib64.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_usr_lib64.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_usr_sbin.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_usr_sbin.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_var_cache_pulp.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_var_cache_pulp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_var_lib_mongodb.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_var_lib_mongodb.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_var_lib_nova_instances.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_var_lib_nova_instances.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_var_lib_pcp.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_var_lib_pcp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_var_lib_rsyslog.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_var_lib_rsyslog.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_var_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_var_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_var_opt_mssql.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_var_opt_mssql.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_var_opt_mssql_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_var_opt_mssql_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_var_run.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_var_run.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_lsof.py` & `insights-core-3.2.0/insights/tests/parsers/test_lsof.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_var_spool_clientmq.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_var_spool_clientmq.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_var_spool_postfix_maildrop.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_var_spool_postfix_maildrop.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_var_tmp.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_var_tmp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ls_var_www_perms.py` & `insights-core-3.2.0/insights/tests/parsers/test_ls_var_www_perms.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_lsblk.py` & `insights-core-3.2.0/insights/tests/parsers/test_lsblk.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_lscpu.py` & `insights-core-3.2.0/insights/tests/parsers/test_lscpu.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_lsinitrd.py` & `insights-core-3.2.0/insights/tests/parsers/test_lsinitrd.py`

 * *Files 6% similar despite different names*

```diff
@@ -172,14 +172,19 @@
 crw-r--r--   1 root     root       1,   9 Aug  4  2020 dev/urandom
 drwxr-xr-x  14 root     root            0 Aug  4  2020 .
 lrwxrwxrwx   1 root     root            7 Aug  4  2020 bin -> usr/bin
 drwxr-xr-x   2 root     root            0 Aug  4  2020 dev
 ========================================================================
 """.strip()
 
+LSINITRD_LVM_CONF = """
+# volume_list = [ "vg1", "vg2/lvol1", "@tag1", "@*" ]
+volume_list = [ "vg2", "vg3/lvol3", "@tag2", "@*" ]
+""".strip()
+
 
 def test_lsinitrd_empty():
     d = lsinitrd.Lsinitrd(context_wrap(LSINITRD_EMPTY))
     assert len(d.data) == 0
     assert d.search(name__contains='kernel') == []
     assert d.unparsed_lines == []
 
@@ -222,13 +227,19 @@
     parser_result = LsinitrdKdumpImage(context_wrap(LSINITRD_KDUMP_IMAGE_VALID))
     assert parser_result is not None
     result_list = parser_result.search(name__contains='devname')
     assert len(result_list) == 1
     assert result_list[0].get('raw_entry') == '-rw-r--r--   1 root     root          126 Aug  4  2020 usr/lib/modules/4.18.0-240.el8.x86_64/modules.devname'
 
 
+def test_lsinitrd_lvm_conf():
+    lvm_conf = lsinitrd.LsinitrdLvmConf(context_wrap(LSINITRD_LVM_CONF))
+    assert lvm_conf["volume_list"] == ["vg2", "vg3/lvol3", "@tag2", "@*"]
+
+
 def test_lsinitrd_docs():
     failed_count, tests = doctest.testmod(
         globs={'ls': lsinitrd.Lsinitrd(context_wrap(LSINITRD_FILTERED)),
-               'lsinitrd_kdump_image': LsinitrdKdumpImage(context_wrap(LSINITRD_KDUMP_IMAGE_VALID_EXAMPLE))}
+               'lsinitrd_kdump_image': LsinitrdKdumpImage(context_wrap(LSINITRD_KDUMP_IMAGE_VALID_EXAMPLE)),
+               'lsinitrd_lvm_conf': lsinitrd.LsinitrdLvmConf(context_wrap(LSINITRD_LVM_CONF))}
     )
     assert failed_count == 0
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_lsmod.py` & `insights-core-3.2.0/insights/tests/parsers/test_lsmod.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_lspci.py` & `insights-core-3.2.0/insights/tests/parsers/test_lspci.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_lssap.py` & `insights-core-3.2.0/insights/tests/parsers/test_lssap.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_lsscsi.py` & `insights-core-3.2.0/insights/tests/parsers/test_lsscsi.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_luksmeta.py` & `insights-core-3.2.0/insights/tests/parsers/test_luksmeta.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_lvdisplay.py` & `insights-core-3.2.0/insights/tests/parsers/test_lvdisplay.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_lvm.py` & `insights-core-3.2.0/insights/tests/parsers/test_lvm.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_lvm_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_lvm_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_lvs.py` & `insights-core-3.2.0/insights/tests/parsers/test_lvs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_manila_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_manila_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_mariadb_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_mariadb_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_max_uid.py` & `insights-core-3.2.0/insights/tests/parsers/test_max_uid.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_md5check.py` & `insights-core-3.2.0/insights/tests/parsers/test_md5check.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_mdadm.py` & `insights-core-3.2.0/insights/tests/parsers/test_mdadm.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_mdstat.py` & `insights-core-3.2.0/insights/tests/parsers/test_mdstat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_meminfo.py` & `insights-core-3.2.0/insights/tests/parsers/test_meminfo.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_mistral_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_mistral_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_mlx4_port.py` & `insights-core-3.2.0/insights/tests/parsers/test_mlx4_port.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_modinfo.py` & `insights-core-3.2.0/insights/tests/parsers/test_modinfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import doctest
 import pytest
 
 from insights.core.exceptions import SkipComponent
 from insights.parsers import modinfo
-from insights.parsers.modinfo import ModInfoEach, ModInfoAll, KernelModulesInfo
+from insights.parsers.modinfo import KernelModulesInfo
 from insights.tests import context_wrap
 
 MODINFO_I40E = """
 filename:       /lib/modules/3.10.0-993.el7.x86_64/kernel/drivers/net/ethernet/intel/i40e/i40e.ko.xz
 firmware:       i40e/i40e-e2-7.13.1.0.fw
 firmware:       i40e/i40e-e1h-7.13.1.0.fw
 version:        2.3.2-k
@@ -152,17 +152,14 @@
 signer:         Red Hat Enterprise Linux kernel signing key
 sig_key:        69:10:6E:D5:83:0D:2C:66:97:41:91:7B:0F:57:D4:1D:95:A2:8A:EB
 sig_hashalgo:   sha256
 parm:           max_vfs:Maximum number of virtual functions to allocate per physical function (uint)
 parm:           debug:Debug level (0=none,...,16=all) (int)
 """.strip()
 
-MODINFO_NO = """
-""".strip()
-
 MODINFO_NO_1 = """
 modinfo ERROR Module i40e not found.
 """.strip()
 
 MODINFO_VETH = """
 filename:       /lib/modules/3.10.0-327.el7.x86_64/kernel/drivers/net/veth.ko
 alias:          rtnl-link-veth
@@ -213,13 +210,11 @@
     with pytest.raises(SkipComponent) as exc:
         KernelModulesInfo(context_wrap(''))
     assert 'No Contents' in str(exc)
 
 
 def test_modinfo_doc_examples():
     env = {
-            'modinfo_obj': ModInfoEach(context_wrap(MODINFO_I40E)),
-            'modinfo_all': ModInfoAll(context_wrap("{0}\n{1}".format(MODINFO_VMXNET3, MODINFO_I40E))),
-            'mods_info': KernelModulesInfo(context_wrap("{0}\n{1}".format(MODINFO_VMXNET3, MODINFO_I40E)))
+        'mods_info': KernelModulesInfo(context_wrap("{0}\n{1}".format(MODINFO_VMXNET3, MODINFO_I40E)))
     }
     failed, total = doctest.testmod(modinfo, globs=env)
     assert failed == 0
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_modprobe.py` & `insights-core-3.2.0/insights/tests/parsers/test_modprobe.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_mokutil_sbstate.py` & `insights-core-3.2.0/insights/tests/parsers/test_mokutil_sbstate.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_mongod_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_mongod_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_mount.py` & `insights-core-3.2.0/insights/tests/parsers/test_mount.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_mpirun.py` & `insights-core-3.2.0/insights/tests/parsers/test_mpirun.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_mssql_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_mssql_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_multicast_querier.py` & `insights-core-3.2.0/insights/tests/parsers/test_multicast_querier.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_multipath_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_multipath_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_multipath_v4_ll.py` & `insights-core-3.2.0/insights/tests/parsers/test_multipath_v4_ll.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_mysql_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_mysql_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_mysqladmin.py` & `insights-core-3.2.0/insights/tests/parsers/test_mysqladmin.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_named_checkconf.py` & `insights-core-3.2.0/insights/tests/parsers/test_named_checkconf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_named_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_named_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ndctl_list.py` & `insights-core-3.2.0/insights/tests/parsers/test_ndctl_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_net_namespace.py` & `insights-core-3.2.0/insights/tests/parsers/test_net_namespace.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_netstat.py` & `insights-core-3.2.0/insights/tests/parsers/test_netstat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_networkmanager_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_networkmanager_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_networkmanager_dhclient.py` & `insights-core-3.2.0/insights/tests/parsers/test_networkmanager_dhclient.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_neutron_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_neutron_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_neutron_dhcp_agent_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_neutron_dhcp_agent_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_neutron_l3_agent_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_neutron_l3_agent_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_neutron_l3_agent_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_neutron_l3_agent_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_neutron_metadata_agent_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_neutron_metadata_agent_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_neutron_metadata_agent_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_neutron_metadata_agent_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_neutron_ml2_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_neutron_ml2_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_neutron_ovs_agent_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_neutron_ovs_agent_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_neutron_plugin.py` & `insights-core-3.2.0/insights/tests/parsers/test_neutron_plugin.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_neutron_server_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_neutron_server_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_neutron_sriov_agent.py` & `insights-core-3.2.0/insights/tests/parsers/test_neutron_sriov_agent.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_nfnetlink_queue.py` & `insights-core-3.2.0/insights/tests/parsers/test_nfnetlink_queue.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_nfs_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_nfs_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_nfs_exports.py` & `insights-core-3.2.0/insights/tests/parsers/test_nfs_exports.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_nginx_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_nginx_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_nginx_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_nginx_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_nmcli.py` & `insights-core-3.2.0/insights/tests/parsers/test_nmcli.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_nova_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_nova_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_nova_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_nova_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_nova_user_ids.py` & `insights-core-3.2.0/insights/tests/parsers/test_nova_user_ids.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_nscd_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_nscd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_nss_rhel7.py` & `insights-core-3.2.0/insights/tests/parsers/test_nss_rhel7.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_nsswitch_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_nsswitch_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ntp_sources.py` & `insights-core-3.2.0/insights/tests/parsers/test_ntp_sources.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_numa_cpus.py` & `insights-core-3.2.0/insights/tests/parsers/test_numa_cpus.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_numeric_user_group_name.py` & `insights-core-3.2.0/insights/tests/parsers/test_numeric_user_group_name.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_nvme_core_io_timeout.py` & `insights-core-3.2.0/insights/tests/parsers/test_nvme_core_io_timeout.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_octavia.py` & `insights-core-3.2.0/insights/tests/parsers/test_octavia.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_od_cpu_dma_latency.py` & `insights-core-3.2.0/insights/tests/parsers/test_od_cpu_dma_latency.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_odbc.py` & `insights-core-3.2.0/insights/tests/parsers/test_odbc.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_open_vm_tools.py` & `insights-core-3.2.0/insights/tests/parsers/test_open_vm_tools.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_openshift_configuration.py` & `insights-core-3.2.0/insights/tests/parsers/test_openshift_configuration.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_openshift_get.py` & `insights-core-3.2.0/insights/tests/parsers/test_openshift_get.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_openshift_get_with_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_openshift_get_with_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_openshift_hosts.py` & `insights-core-3.2.0/insights/tests/parsers/test_openshift_hosts.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_openvswitch_logs.py` & `insights-core-3.2.0/insights/tests/parsers/test_openvswitch_logs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_openvswitch_other_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_openvswitch_other_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_oracle.py` & `insights-core-3.2.0/insights/tests/parsers/test_oracle.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_os_release.py` & `insights-core-3.2.0/insights/tests/parsers/test_os_release.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_osa_dispatcher_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_osa_dispatcher_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ovirt_engine_confd.py` & `insights-core-3.2.0/insights/tests/parsers/test_ovirt_engine_confd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ovirt_engine_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_ovirt_engine_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ovs_appctl_fdb_show_bridge.py` & `insights-core-3.2.0/insights/tests/parsers/test_ovs_appctl_fdb_show_bridge.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ovs_ofctl_dump_flows.py` & `insights-core-3.2.0/insights/tests/parsers/test_ovs_ofctl_dump_flows.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ovs_vsctl.py` & `insights-core-3.2.0/insights/tests/parsers/test_ovs_vsctl.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ovs_vsctl_list_bridge.py` & `insights-core-3.2.0/insights/tests/parsers/test_ovs_vsctl_list_bridge.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ovs_vsctl_show.py` & `insights-core-3.2.0/insights/tests/parsers/test_ovs_vsctl_show.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_pacemaker_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_pacemaker_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_package_provides.py` & `insights-core-3.2.0/insights/tests/parsers/test_package_provides.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_pam.py` & `insights-core-3.2.0/insights/tests/parsers/test_pam.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_parsers_module.py` & `insights-core-3.2.0/insights/tests/parsers/test_parsers_module.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_parted.py` & `insights-core-3.2.0/insights/tests/parsers/test_parted.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,28 @@
 
 Number  Start     End        Size       File system  Name                  Flags
  1      2048s     2099199s   2097152s   fat32        EFI System Partition  boot, esp
  2      2099200s  4196351s   2097152s   xfs
  3      4196352s  83904511s  79708160s                                     lvm
 """.strip()
 
+PARTED_DATA_7 = """
+Model: Virtio Block Device (virtblk)
+Disk /dev/vda: 32.2GB
+Sector size (logical/physical): 512B/512B
+Partition Table: msdos
+Disk Flags:
+
+Number  Start   End     Size    Type     File system  Flags
+ 1      1049kB  525MB   524MB   primary  xfs          boot
+ 2      525MB   26.5GB  25.9GB  primary
+
+
+"""
+
 
 def test_parted_partedl():
     context = context_wrap(PARTED_DATA)
     res = PartedL(context)
     results = res.devices_info[0]
     assert results is not None
     assert results.get('model') == 'Virtio Block Device (virtblk)'
@@ -276,14 +290,22 @@
     results = res.get('/dev/sdc')
     assert results.get('size') == '15032385536s'
     assert results.get('model') == 'VMware Virtual disk (scsi)'
     assert results.get('sector_size') == '512B/512B'
     assert results.get('partition_table') == 'msdos'
     assert results.get('disk_flags') is None
 
+    context = context_wrap(PARTED_DATA_6)
+    res = PartedL(context)
+    assert len([dev_info.disk for dev_info in res]) == 1
+
+    context = context_wrap(PARTED_DATA_7)
+    res = PartedL(context)
+    assert len([dev_info.disk for dev_info in res]) == 1
+
 
 PARTED_ERR_DATA = """
 Error: /dev/dm-1: unrecognised disk label
 """
 
 PARTED_ERR_DATA_2 = """
 Model: IBM 2107900 (scsi)
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_partitions.py` & `insights-core-3.2.0/insights/tests/parsers/test_partitions.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_passenger_status.py` & `insights-core-3.2.0/insights/tests/parsers/test_passenger_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_password.py` & `insights-core-3.2.0/insights/tests/parsers/test_password.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_pci_rport_target_disk_paths.py` & `insights-core-3.2.0/insights/tests/parsers/test_pci_rport_target_disk_paths.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_pcp_openmetrics_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_pcp_openmetrics_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_pcs_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_pcs_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_pcs_quorum_status.py` & `insights-core-3.2.0/insights/tests/parsers/test_pcs_quorum_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_pcs_status.py` & `insights-core-3.2.0/insights/tests/parsers/test_pcs_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_php_ini.py` & `insights-core-3.2.0/insights/tests/parsers/test_php_ini.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_pluginconf_d.py` & `insights-core-3.2.0/insights/tests/parsers/test_pluginconf_d.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_pmlog_summary.py` & `insights-core-3.2.0/insights/tests/parsers/test_pmlog_summary.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_pmrep.py` & `insights-core-3.2.0/insights/tests/parsers/test_pmrep.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_podman_inspect.py` & `insights-core-3.2.0/insights/tests/parsers/test_podman_inspect.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_podman_list.py` & `insights-core-3.2.0/insights/tests/parsers/test_podman_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_postconf.py` & `insights-core-3.2.0/insights/tests/parsers/test_postconf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_postgresql_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_postgresql_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_postgresql_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_postgresql_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_proc_environ.py` & `insights-core-3.2.0/insights/tests/parsers/test_proc_environ.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_proc_keys.py` & `insights-core-3.2.0/insights/tests/parsers/test_proc_keys.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_proc_limits.py` & `insights-core-3.2.0/insights/tests/parsers/test_proc_limits.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_proc_stat.py` & `insights-core-3.2.0/insights/tests/parsers/test_proc_stat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ps.py` & `insights-core-3.2.0/insights/tests/parsers/test_ps.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_pulp_worker_defaults.py` & `insights-core-3.2.0/insights/tests/parsers/test_pulp_worker_defaults.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_puppet_ca_cert_expire_date.py` & `insights-core-3.2.0/insights/tests/parsers/test_puppet_ca_cert_expire_date.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_pvs.py` & `insights-core-3.2.0/insights/tests/parsers/test_pvs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_qemu_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_qemu_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_qemu_xml.py` & `insights-core-3.2.0/insights/tests/parsers/test_qemu_xml.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_qpid_stat.py` & `insights-core-3.2.0/insights/tests/parsers/test_qpid_stat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_qpidd_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_qpidd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rabbit_users.py` & `insights-core-3.2.0/insights/tests/parsers/test_rabbit_users.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rabbitmq_env.py` & `insights-core-3.2.0/insights/tests/parsers/test_rabbitmq_env.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rabbitmq_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_rabbitmq_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rabbitmq_queues.py` & `insights-core-3.2.0/insights/tests/parsers/test_rabbitmq_queues.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rabbitmq_report.py` & `insights-core-3.2.0/insights/tests/parsers/test_rabbitmq_report.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rc_local.py` & `insights-core-3.2.0/insights/tests/parsers/test_rc_local.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rdma_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_rdma_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_readlink_mtab.py` & `insights-core-3.2.0/insights/tests/parsers/test_readlink_mtab.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_readlink_openshift_certs.py` & `insights-core-3.2.0/insights/tests/parsers/test_readlink_openshift_certs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_redhat_release.py` & `insights-core-3.2.0/insights/tests/parsers/test_redhat_release.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_resolv_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_resolv_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rhev_data_center.py` & `insights-core-3.2.0/insights/tests/parsers/test_rhev_data_center.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rhn_charsets.py` & `insights-core-3.2.0/insights/tests/parsers/test_rhn_charsets.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rhn_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_rhn_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rhn_entitlement_cert_xml.py` & `insights-core-3.2.0/insights/tests/parsers/test_rhn_entitlement_cert_xml.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rhn_hibernate_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_rhn_hibernate_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rhn_logs.py` & `insights-core-3.2.0/insights/tests/parsers/test_rhn_logs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rhn_schema_stats.py` & `insights-core-3.2.0/insights/tests/parsers/test_rhn_schema_stats.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rhosp_release.py` & `insights-core-3.2.0/insights/tests/parsers/test_rhosp_release.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rhsm_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_rhsm_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rhsm_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_rhsm_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rhsm_releasever.py` & `insights-core-3.2.0/insights/tests/parsers/test_rhsm_releasever.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rhv_log_collector_analyzer.py` & `insights-core-3.2.0/insights/tests/parsers/test_rhv_log_collector_analyzer.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ros_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_ros_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_route.py` & `insights-core-3.2.0/insights/tests/parsers/test_route.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rpm_ostree_status.py` & `insights-core-3.2.0/insights/tests/parsers/test_rpm_ostree_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rpm_pkgs.py` & `insights-core-3.2.0/insights/tests/parsers/test_rpm_pkgs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pytest
 
 from insights.parsers import rpm_pkgs
 from insights.parsers.rpm_pkgs import RpmPkgs, RpmPkgsWritable
 from insights.tests import context_wrap
 
 
-DATASOURCE_OUTPUT = [("httpd-core", "httpd-core-2.4.53-7.el9.x86_64", "Red Hat, Inc.")]
+DATASOURCE_OUTPUT = ["httpd-core|httpd-core-2.4.53-7.el9.x86_64|Red Hat, Inc."]
 
 RPM_PKGS_OUTPUT = ["httpd-core"]
 RPM_PKGS_WRITABLE_OUTPUT = [("httpd-core", "httpd-core-2.4.53-7.el9.x86_64", "Red Hat, Inc.")]
 
 
 @pytest.mark.parametrize("parser, output", [
     (RpmPkgs, RPM_PKGS_OUTPUT),
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rpm_v_packages.py` & `insights-core-3.2.0/insights/tests/parsers/test_rpm_v_packages.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rpm_vercmp.py` & `insights-core-3.2.0/insights/tests/parsers/test_rpm_vercmp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_rsyslog_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_rsyslog_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_samba.py` & `insights-core-3.2.0/insights/tests/parsers/test_samba.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_samba_logs.py` & `insights-core-3.2.0/insights/tests/parsers/test_samba_logs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sap_dev_trace_files.py` & `insights-core-3.2.0/insights/tests/parsers/test_sap_dev_trace_files.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sap_hana_python_script.py` & `insights-core-3.2.0/insights/tests/parsers/test_sap_hana_python_script.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sap_hdb_version.py` & `insights-core-3.2.0/insights/tests/parsers/test_sap_hdb_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sap_host_profile.py` & `insights-core-3.2.0/insights/tests/parsers/test_sap_host_profile.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sapcontrol.py` & `insights-core-3.2.0/insights/tests/parsers/test_sapcontrol.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_saphostctrl.py` & `insights-core-3.2.0/insights/tests/parsers/test_saphostctrl.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_saphostexec.py` & `insights-core-3.2.0/insights/tests/parsers/test_saphostexec.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sat5_insights_properties.py` & `insights-core-3.2.0/insights/tests/parsers/test_sat5_insights_properties.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_satellite_content_hosts_count.py` & `insights-core-3.2.0/insights/tests/parsers/test_satellite_content_hosts_count.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_satellite_enabled_features.py` & `insights-core-3.2.0/insights/tests/parsers/test_satellite_enabled_features.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_satellite_installer_configurations.py` & `insights-core-3.2.0/insights/tests/parsers/test_satellite_installer_configurations.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_satellite_missed_queues.py` & `insights-core-3.2.0/insights/tests/parsers/test_satellite_missed_queues.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_satellite_mongodb.py` & `insights-core-3.2.0/insights/tests/parsers/test_satellite_mongodb.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_satellite_postgresql_query.py` & `insights-core-3.2.0/insights/tests/parsers/test_satellite_postgresql_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -198,37 +198,42 @@
 """.strip()
 
 SATELLITE_LOGS_TABLE_SIZE3 = """
 logs_size
 abc
 """.strip()
 
+SATELLITE_RHV_HOSTS_COUNT = """
+count
+2
+""".strip()
+
 
 def test_HTL_doc_examples():
     settings = satellite_postgresql_query.SatelliteAdminSettings(context_wrap(SATELLITE_SETTINGS_1))
     resources_table = satellite_postgresql_query.SatelliteComputeResources(context_wrap(SATELLITE_COMPUTE_RESOURCE_1))
     sat_sca_info = satellite_postgresql_query.SatelliteSCAStatus(context_wrap(SATELLITE_SCA_INFO_1))
-    repositories = satellite_postgresql_query.SatelliteKatelloEmptyURLRepositories(context_wrap(SATELLITE_KATELLO_ROOT_REPOSITORIES))
     tasks = satellite_postgresql_query.SatelliteCoreTaskReservedResourceCount(context_wrap(SATELLITE_TASK_RESERVERDRESOURCE_CONTENT))
     capsules = satellite_postgresql_query.SatelliteQualifiedCapsules(context_wrap(SATELLITE_CAPSULES_WITH_BACKGROUND_DOWNLOADPOLICY))
     repos = satellite_postgresql_query.SatelliteQualifiedKatelloRepos(context_wrap(SATELLITE_REPOS_INFO))
     multi_ref_katello_repos = satellite_postgresql_query.SatelliteKatellloReposWithMultipleRef(context_wrap(SATELLITE_KATELLO_REPOS_WITH_MULTI_REF))
     param_settings = satellite_postgresql_query.SatelliteProvisionParamSettings(context_wrap(SATELLITE_PROVISION_PARAMETERS_HIT_1))
     logs_table = satellite_postgresql_query.SatelliteLogsTableSize(context_wrap(SATELLITE_LOGS_TABLE_SIZE1))
+    rhv_hosts = satellite_postgresql_query.SatelliteRHVHostsCount(context_wrap(SATELLITE_RHV_HOSTS_COUNT))
     globs = {
         'table': settings,
         'resources_table': resources_table,
         'sat_sca_info': sat_sca_info,
-        'katello_root_repositories': repositories,
         'tasks': tasks,
         'capsules': capsules,
         'repos': repos,
         'multi_ref_katello_repos': multi_ref_katello_repos,
         'param_settings': param_settings,
-        'logs_table': logs_table
+        'logs_table': logs_table,
+        'rhv_hosts': rhv_hosts
     }
     failed, _ = doctest.testmod(satellite_postgresql_query, globs=globs)
     assert failed == 0
 
 
 def test_no_headers():
     with pytest.raises(NotImplementedError):
@@ -291,30 +296,14 @@
 
 
 def test_satellite_sca():
     sat_sca_info = satellite_postgresql_query.SatelliteSCAStatus(context_wrap(SATELLITE_SCA_INFO_2))
     assert not sat_sca_info.sca_enabled
 
 
-def test_satellite_katello_empty_url_repositories():
-    repositories = satellite_postgresql_query.SatelliteKatelloEmptyURLRepositories(context_wrap(SATELLITE_KATELLO_ROOT_REPOSITORIES))
-    assert repositories[1]['name'] == 'testb'
-
-    table = satellite_postgresql_query.SatelliteKatelloEmptyURLRepositories(context_wrap(SATELLITE_QUERY_DATA1))
-    assert len(table) == 1
-    assert table[0]['id'] == '1'
-    assert table[0]['name'] == 'Puppet_Base'
-
-    with pytest.raises(SkipComponent):
-        satellite_postgresql_query.SatelliteKatelloEmptyURLRepositories(context_wrap(SATELLITE_QUERY_DATA2))
-
-    with pytest.raises(ValueError):
-        satellite_postgresql_query.SatelliteKatelloEmptyURLRepositories(context_wrap(SATELLITE_QUERY_DATA3))
-
-
 def test_satellite_taskreservedresource():
     tasks = satellite_postgresql_query.SatelliteCoreTaskReservedResourceCount(context_wrap(SATELLITE_TASK_RESERVERDRESOURCE_CONTENT))
     assert tasks[0]['count'] == '0'
 
 
 def test_satellite_qulified_capsules():
     capsules = satellite_postgresql_query.SatelliteQualifiedCapsules(context_wrap(SATELLITE_CAPSULES_WITH_BACKGROUND_DOWNLOADPOLICY))
@@ -353,10 +342,16 @@
 
 def test_satellite_logs_table_size():
     logs_table = satellite_postgresql_query.SatelliteLogsTableSize(context_wrap(SATELLITE_LOGS_TABLE_SIZE2))
     assert len(logs_table) == 1
     assert logs_table[0]['logs_size'] == 552 * 1024 * 1024
 
 
+def test_satelite_rhv_hosts():
+    rhv_hosts = satellite_postgresql_query.SatelliteRHVHostsCount(context_wrap(SATELLITE_RHV_HOSTS_COUNT))
+    assert len(rhv_hosts) == 1
+    assert int(rhv_hosts[0]['count']) == 2
+
+
 def test_satellite_logs_table_size_except():
     with pytest.raises(ParseException):
         satellite_postgresql_query.SatelliteLogsTableSize(context_wrap(SATELLITE_LOGS_TABLE_SIZE3))
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_satellite_version.py` & `insights-core-3.2.0/insights/tests/parsers/test_satellite_version.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_satellite_yaml.py` & `insights-core-3.2.0/insights/tests/parsers/test_satellite_yaml.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_scheduler.py` & `insights-core-3.2.0/insights/tests/parsers/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_scsi.py` & `insights-core-3.2.0/insights/tests/parsers/test_scsi.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_scsi_eh_deadline.py` & `insights-core-3.2.0/insights/tests/parsers/test_scsi_eh_deadline.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_scsi_fwver.py` & `insights-core-3.2.0/insights/tests/parsers/test_scsi_fwver.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sctp.py` & `insights-core-3.2.0/insights/tests/parsers/test_sctp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sealert.py` & `insights-core-3.2.0/insights/tests/parsers/test_sealert.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_secure.py` & `insights-core-3.2.0/insights/tests/parsers/test_secure.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_selinux_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_selinux_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_semanage.py` & `insights-core-3.2.0/insights/tests/parsers/test_semanage.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sendq_recvq_socket_buffer.py` & `insights-core-3.2.0/insights/tests/parsers/test_sendq_recvq_socket_buffer.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sestatus.py` & `insights-core-3.2.0/insights/tests/parsers/test_sestatus.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_setup_named_chroot.py` & `insights-core-3.2.0/insights/tests/parsers/test_setup_named_chroot.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_slabinfo.py` & `insights-core-3.2.0/insights/tests/parsers/test_slabinfo.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_smartctl.py` & `insights-core-3.2.0/insights/tests/parsers/test_smartctl.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_smartpdc_settings.py` & `insights-core-3.2.0/insights/tests/parsers/test_smartpdc_settings.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_smbstatus.py` & `insights-core-3.2.0/insights/tests/parsers/test_smbstatus.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_smt.py` & `insights-core-3.2.0/insights/tests/parsers/test_smt.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_snmp.py` & `insights-core-3.2.0/insights/tests/parsers/test_snmp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sockstat.py` & `insights-core-3.2.0/insights/tests/parsers/test_sockstat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_softnet_stat.py` & `insights-core-3.2.0/insights/tests/parsers/test_softnet_stat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_software_collections_list.py` & `insights-core-3.2.0/insights/tests/parsers/test_software_collections_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sos_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_sos_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_spamassassin_channels.py` & `insights-core-3.2.0/insights/tests/parsers/test_spamassassin_channels.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ssh.py` & `insights-core-3.2.0/insights/tests/parsers/test_ssh.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ssh_client_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_ssh_client_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_ssl_certificate.py` & `insights-core-3.2.0/insights/tests/parsers/test_ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sssd_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_sssd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sssd_logs.py` & `insights-core-3.2.0/insights/tests/parsers/test_sssd_logs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_subscription_manager.py` & `insights-core-3.2.0/insights/tests/parsers/test_subscription_manager.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_subscription_manager_list.py` & `insights-core-3.2.0/insights/tests/parsers/test_subscription_manager_list.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_subscription_manager_release.py` & `insights-core-3.2.0/insights/tests/parsers/test_subscription_manager_release.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sudoers.py` & `insights-core-3.2.0/insights/tests/parsers/test_sudoers.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_swift_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_swift_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_swift_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_swift_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sys_bus.py` & `insights-core-3.2.0/insights/tests/parsers/test_sys_bus.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sys_fs_cgroup_memory.py` & `insights-core-3.2.0/insights/tests/parsers/test_sys_fs_cgroup_memory.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sys_kernel.py` & `insights-core-3.2.0/insights/tests/parsers/test_sys_kernel.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sys_module.py` & `insights-core-3.2.0/insights/tests/parsers/test_sys_module.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sys_vmbus.py` & `insights-core-3.2.0/insights/tests/parsers/test_sys_vmbus.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_corosync.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_corosync.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_dirsrv.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_dirsrv.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_doc_examples.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_doc_examples.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_docker.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_docker.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_docker_storage.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_docker_storage.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_docker_storage_setup.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_docker_storage_setup.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_grub.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_grub.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_httpd.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_httpd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_ifcfg_static_route.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_ifcfg_static_route.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_irqbalance.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_irqbalance.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_kdump.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_kdump.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_libvirt_guests.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_libvirt_guests.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_memcached.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_memcached.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_netconsole.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_netconsole.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_nfs.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_nfs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_oracleasm.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_oracleasm.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_prelink.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_prelink.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_puppetserver.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_puppetserver.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_sshd.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_sshd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_up2date.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_up2date.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysconfig_virt_who.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysconfig_virt_who.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_sysctl.py` & `insights-core-3.2.0/insights/tests/parsers/test_sysctl.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_system_time.py` & `insights-core-3.2.0/insights/tests/parsers/test_system_time.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_systemctl_show.py` & `insights-core-3.2.0/insights/tests/parsers/test_systemctl_show.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_systemd_analyze.py` & `insights-core-3.2.0/insights/tests/parsers/test_systemd_analyze.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_systemd_config.py` & `insights-core-3.2.0/insights/tests/parsers/test_systemd_config.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_systemid.py` & `insights-core-3.2.0/insights/tests/parsers/test_systemid.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_systool.py` & `insights-core-3.2.0/insights/tests/parsers/test_systool.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_tags.py` & `insights-core-3.2.0/insights/tests/parsers/test_tags.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_teamdctl_config_dump.py` & `insights-core-3.2.0/insights/tests/parsers/test_teamdctl_config_dump.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_teamdctl_state_dump.py` & `insights-core-3.2.0/insights/tests/parsers/test_teamdctl_state_dump.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_tmpfilesd.py` & `insights-core-3.2.0/insights/tests/parsers/test_tmpfilesd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_tomcat_virtual_dir_context.py` & `insights-core-3.2.0/insights/tests/parsers/test_tomcat_virtual_dir_context.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_tomcat_xml.py` & `insights-core-3.2.0/insights/tests/parsers/test_tomcat_xml.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_transparent_hugepage.py` & `insights-core-3.2.0/insights/tests/parsers/test_transparent_hugepage.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_tuned.py` & `insights-core-3.2.0/insights/tests/parsers/test_tuned.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_tuned_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_tuned_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_udev_rules.py` & `insights-core-3.2.0/insights/tests/parsers/test_udev_rules.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_uname.py` & `insights-core-3.2.0/insights/tests/parsers/test_uname.py`

 * *Files 3% similar despite different names*

```diff
@@ -216,14 +216,17 @@
     assert cve_2016_0728.kernel == '3.10.0-229.1.2.rt56.141.2.el7_1.x86_64'
 
 
 def test_pad_release():
     assert "390.0.0.el6" == uname.pad_release("390.el6")
     assert "390.12.0.el6" == uname.pad_release("390.12.el6")
     assert "390.12.0.0.el6" == uname.pad_release("390.12.el6", 5)
+    assert "390.0.0.0" == uname.pad_release("390")
+    assert "390.12.0.0" == uname.pad_release("390.12")
+    assert "1160.71.1.0" == uname.pad_release("1160.71.1")
     with pytest.raises(ValueError):
         uname.pad_release('390.11.12.13.el6')
 
 
 def test_fixed_by():
     u = uname.Uname.from_uname_str("Linux qqhrycsq2 2.6.32-504.el6.x86_64 #1 SMP Wed Jun 13 18:24:36 EDT 2012 x86_64 x86_64 x86_64 GNU/Linux")
     assert [] == u.fixed_by('2.6.32-220.1.el6', '2.6.32-504.el6')
@@ -253,14 +256,33 @@
 
     ]
     for u, expected in test_kernels:
         fixed_by = u.fixed_by("2.6.18-128.39.1.el5", "2.6.18-238.40.1.el5", "2.6.18-308.13.1.el5", "2.6.18-348.el5")
         assert expected == fixed_by
 
 
+def test_from_kernel_partial():
+    u = uname.Uname.from_kernel("5.14.0-284.13.1")
+    assert "284.13.1.0.0" == u._lv_release
+
+    u = uname.Uname.from_kernel("5.14.0-284")
+    assert "284.0.0.0.0" == u._lv_release
+
+    early_rhel9 = uname.Uname.from_uname_str("Linux example 5.14.0-70.22.1.el9_0.x86_64 #1 SMP Wed May 24 08:55:08 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux")
+    later_rhel9_1 = uname.Uname.from_kernel("5.14.0-162.18.1")
+    later_rhel9_2 = uname.Uname.from_kernel("5.14.0-284")
+
+    # Test comparison of full uname with partial kernel version
+    assert early_rhel9 < later_rhel9_1
+
+    # Test comparison of partial kernel versions
+    assert early_rhel9 < later_rhel9_2
+    assert later_rhel9_1 < later_rhel9_2
+
+
 def test_from_release():
     release = ("6", "4")
     from_release = uname.Uname.from_release(release)
     from_nvr = uname.Uname.from_kernel("2.6.32-358")
     assert str(from_release) == str(from_nvr)
 
     # Test the regular 7.4 version.
```

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_unitfiles.py` & `insights-core-3.2.0/insights/tests/parsers/test_unitfiles.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_up2date_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_up2date_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_upstart.py` & `insights-core-3.2.0/insights/tests/parsers/test_upstart.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_uptime.py` & `insights-core-3.2.0/insights/tests/parsers/test_uptime.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_user_group.py` & `insights-core-3.2.0/insights/tests/parsers/test_user_group.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_vdo_status.py` & `insights-core-3.2.0/insights/tests/parsers/test_vdo_status.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_vdsm_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_vdsm_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_vdsm_log.py` & `insights-core-3.2.0/insights/tests/parsers/test_vdsm_log.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_version_info.py` & `insights-core-3.2.0/insights/tests/parsers/test_version_info.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_vgdisplay.py` & `insights-core-3.2.0/insights/tests/parsers/test_vgdisplay.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_vgs.py` & `insights-core-3.2.0/insights/tests/parsers/test_vgs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_virsh_list_all.py` & `insights-core-3.2.0/insights/tests/parsers/test_virsh_list_all.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_virt_uuid_facts.py` & `insights-core-3.2.0/insights/tests/parsers/test_virt_uuid_facts.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_virt_what.py` & `insights-core-3.2.0/insights/tests/parsers/test_virt_what.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_virt_who_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_virt_who_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_virtlogd_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_virtlogd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_vma_ra_enabled_s390x.py` & `insights-core-3.2.0/insights/tests/parsers/test_vma_ra_enabled_s390x.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_vmcore_dmesg.py` & `insights-core-3.2.0/insights/tests/parsers/test_vmcore_dmesg.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_vmware_tools_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_vmware_tools_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_vsftpd.py` & `insights-core-3.2.0/insights/tests/parsers/test_vsftpd.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_wc_proc_1_mountinfo.py` & `insights-core-3.2.0/insights/tests/parsers/test_wc_proc_1_mountinfo.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_x86_debug.py` & `insights-core-3.2.0/insights/tests/parsers/test_x86_debug.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_xfs_info.py` & `insights-core-3.2.0/insights/tests/parsers/test_xfs_info.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_xinetd_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_xinetd_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_yum_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_yum_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_yum_list_available.py` & `insights-core-3.2.0/insights/tests/parsers/test_yum_list_available.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_yum_repolist.py` & `insights-core-3.2.0/insights/tests/parsers/test_yum_repolist.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_yum_repos_d.py` & `insights-core-3.2.0/insights/tests/parsers/test_yum_repos_d.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_yum_updateinfo.py` & `insights-core-3.2.0/insights/tests/parsers/test_yum_updateinfo.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_yum_updates.py` & `insights-core-3.2.0/insights/tests/parsers/test_yum_updates.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_yumlog.py` & `insights-core-3.2.0/insights/tests/parsers/test_yumlog.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_zdump_v.py` & `insights-core-3.2.0/insights/tests/parsers/test_zdump_v.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/parsers/test_zipl_conf.py` & `insights-core-3.2.0/insights/tests/parsers/test_zipl_conf.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_plugins/test_returns_none.py` & `insights-core-3.2.0/insights/tests/test_plugins/test_returns_none.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/__init__.py` & `insights-core-3.2.0/insights/tests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,42 +82,83 @@
 
 DEFAULT_RELEASE = "Red Hat Enterprise Linux Server release 7.2 (Maipo)"
 DEFAULT_HOSTNAME = "hostname.example.com"
 
 MAKE_NONE_RESULT = make_none()
 
 
+def _beautify_deep_compare_diff(result, expected):
+    if not (isinstance(result, dict) and isinstance(expected, dict)):
+        return result
+
+    if result.get('type') == 'skip':
+        return result
+
+    expected_keys = set(expected.keys())
+    result_keys = set(result.keys())
+    common_keys = set.intersection(result_keys, expected_keys)
+
+    diff = []
+    for k in result_keys - common_keys:
+        diff.append('\tkey "{0}" not in Expected;'.format(k))
+    for k in expected_keys - common_keys:
+        diff.append('\tkey "{0}" not in Result;'.format(k))
+    for k in common_keys:
+        if not eq(result[k], expected[k]):
+            diff.append('\tkey "{0}" unequal values:\n\t\tExpected: {1}\n\t\tResult  : {2}'.format(
+                            k, expected[k], result[k]))
+    if not diff:
+        diff.append('\tUnrecognized unequal values in result layer one;')
+
+    diff.append('Result: "{0}"'.format(result))
+    return '\n' + '\n'.join(diff)
+
+
 def deep_compare(result, expected):
     """
     Deep compare rule reducer results when testing.
+
+    .. note::
+        "[None, XX]" is a special format of the `expected` for this methoed to
+        check the missing dependencies.
     """
     logger.debug("--Comparing-- (%s) %s to (%s) %s", type(result), result, type(expected), expected)
 
+    missing = None
+    if isinstance(expected, (tuple, list, set)) and len(expected) == 2 and expected[0] is None:
+        expected, missing = expected
+
     # This case ensures that when rules return a make_none() response, all of the older
     # CI tests that are looking for None instead of make_none() will still pass
     if result is None or (isinstance(result, dict) and result.get("type") == "none"):
         assert (expected is None or expected == MAKE_NONE_RESULT), result
         return
 
     if isinstance(result, dict) and expected is None:
+        # checking the missing component (RHINRULE-283)
+        if missing:
+            assert "MISSING_REQUIREMENTS" == result['reason'], result['reason']
+            for mis in [missing] if isinstance(missing, str) else missing:
+                assert mis in result['details'], '"{0}" not in "{1}"'.format(mis, result['details'])
         assert result["type"] == "skip", result
         return
 
-    assert eq(result, expected), result
+    assert eq(result, expected), _beautify_deep_compare_diff(result, expected)
 
 
-def run_input_data(component, input_data):
+def run_input_data(component, input_data, store_skips=False):
     broker = dr.Broker()
     for k, v in input_data.data.items():
         broker[k] = v
 
     graph = dr.get_dependency_graph(component)
     broker = dr.run(graph, broker=broker)
+    broker.store_skips = store_skips
     for v in broker.tracebacks.values():
-        print(v)
+        logger.warning(v)
     return broker
 
 
 def run_test(component, input_data, expected=None, return_make_none=False):
     if filters.ENABLED:
         mod = component.__module__
         sup_mod = '.'.join(mod.split('.')[:-1])
```

### Comparing `insights-core-3.1.9/insights/tests/helpers.py` & `insights-core-3.2.0/insights/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/integration.py` & `insights-core-3.2.0/insights/tests/integration.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/mock_web_server.py` & `insights-core-3.2.0/insights/tests/mock_web_server.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/spec_tests.py` & `insights-core-3.2.0/insights/tests/spec_tests.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_canonical_facts.py` & `insights-core-3.2.0/insights/tests/test_canonical_facts.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_collect.py` & `insights-core-3.2.0/insights/tests/test_collect.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_command_parser.py` & `insights-core-3.2.0/insights/tests/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_commandparser.py` & `insights-core-3.2.0/insights/tests/test_commandparser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_component_metadata.py` & `insights-core-3.2.0/insights/tests/test_component_metadata.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_config_parser.py` & `insights-core-3.2.0/insights/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_context.py` & `insights-core-3.2.0/insights/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_context_wrap.py` & `insights-core-3.2.0/insights/tests/test_context_wrap.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_determine_components.py` & `insights-core-3.2.0/insights/tests/test_determine_components.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_dr_enabled.py` & `insights-core-3.2.0/insights/tests/test_dr_enabled.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_dr_run.py` & `insights-core-3.2.0/insights/tests/test_dr_run.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_evaluators.py` & `insights-core-3.2.0/insights/tests/test_evaluators.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_extractors.py` & `insights-core-3.2.0/insights/tests/test_extractors.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_file_listing.py` & `insights-core-3.2.0/insights/tests/test_file_listing.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_file_permissions.py` & `insights-core-3.2.0/insights/tests/test_file_permissions.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_find.py` & `insights-core-3.2.0/insights/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_formats.py` & `insights-core-3.2.0/insights/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_fs.py` & `insights-core-3.2.0/insights/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_get_dependency_specs.py` & `insights-core-3.2.0/insights/tests/test_get_dependency_specs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_insights_heartbeat.py` & `insights-core-3.2.0/insights/tests/test_insights_heartbeat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_integration_support.py` & `insights-core-3.2.0/insights/tests/test_integration_support.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_json_parser.py` & `insights-core-3.2.0/insights/tests/test_json_parser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_logfileoutput.py` & `insights-core-3.2.0/insights/tests/test_logfileoutput.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_ls_parser.py` & `insights-core-3.2.0/insights/tests/test_ls_parser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_parser_class.py` & `insights-core-3.2.0/insights/tests/test_parser_class.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_parser_continue_on_error.py` & `insights-core-3.2.0/insights/tests/test_parser_continue_on_error.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_query.py` & `insights-core-3.2.0/insights/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_remote_resource.py` & `insights-core-3.2.0/insights/tests/test_remote_resource.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_rules_fixture.py` & `insights-core-3.2.0/insights/tests/test_rules_fixture.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_scannable.py` & `insights-core-3.2.0/insights/tests/test_scannable.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_serde.py` & `insights-core-3.2.0/insights/tests/test_serde.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_soscleaner.py` & `insights-core-3.2.0/insights/tests/test_soscleaner.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_spec_serialization.py` & `insights-core-3.2.0/insights/tests/test_spec_serialization.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_specs.py` & `insights-core-3.2.0/insights/tests/test_specs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_subproc.py` & `insights-core-3.2.0/insights/tests/test_subproc.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_sysconfig_options.py` & `insights-core-3.2.0/insights/tests/test_sysconfig_options.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_taglang.py` & `insights-core-3.2.0/insights/tests/test_taglang.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_test.py` & `insights-core-3.2.0/insights/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_util.py` & `insights-core-3.2.0/insights/tests/test_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,14 +98,36 @@
     with pytest.raises(AssertionError):
         deep_compare({"foo": 1}, {"foo": 2})
 
     with pytest.raises(AssertionError):
         deep_compare({"foo": 1, "bar": [1, 2, 3]}, {"foo": 1, "bar": [0, 1, 2]})
 
 
+def test_beautify_deep_compare_diff():
+    with pytest.raises(AssertionError) as err:
+        deep_compare({"foo": "some foo"}, {"bar": "some bar"})
+    einfo = None
+    if hasattr(err, "value"):       # py3
+        einfo = err.value
+    elif hasattr(err, "message"):   # py2
+        einfo = err.message
+    assert 'key "foo" not in Expected;' in str(einfo)
+    assert 'key "bar" not in Result;' in str(einfo)
+
+    with pytest.raises(AssertionError) as err:
+        deep_compare({"e": "k", "common": "left"}, {"e": "k", "common": "right"})
+    einfo = None
+    if hasattr(err, "value"):       # py3
+        einfo = err.value
+    elif hasattr(err, "message"):   # py2
+        einfo = err.message
+    assert 'key "common" unequal values:' in str(einfo)
+    assert 'Result: ' in str(einfo)
+
+
 def test_deep_nest():
     a = {"error_key": "test1", "stuff": {"abba": [{"foo": 2}]}}
     b = {"error_key": "test1", "stuff": {"abba": [{"foo": 2}]}}
 
     deep_compare(a, b)
 
     with pytest.raises(AssertionError):
@@ -190,14 +212,33 @@
     a = {3: [33, [set([4, 3]), '33', 333]], 2: (22, 222)}
     b = {2: (22, 222), 3: [33, [set([4, 3]), '33', 333]]}
     with pytest.raises(AssertionError):
         b[3][1] = set([3, 4])
         deep_compare(a, b)
 
 
+def test_deep_compare_special():
+    """
+    Test the special format of the `expected`
+    """
+    a = {'type': 'skip', 'reason': 'MISSING_REQUIREMENTS', 'details': 'test1'}
+    b1 = (None, 'test1')
+    b2 = [None, ['test1']]
+    deep_compare(a, b1)
+    deep_compare(a, b2)
+
+    with pytest.raises(AssertionError):
+        a = {'type': 'skip', 'reason': 'NO_MISSING', 'details': 'test1'}
+        deep_compare(a, b1)
+
+    with pytest.raises(AssertionError):
+        a = {'type': 'skip', 'reason': 'MISSING_REQUIREMENTS', 'details': 'test0'}
+        deep_compare(a, b1)
+
+
 def test_case_variants():
     filter_list = ['Ciphers', 'MACs', 'UsePAM', 'MaxAuthTries', 'nt pipe support',
                    'A-Dash-SEPARATED-tESt-tEST-tesT-test-ExAMPle']
     expanded_list = ['Ciphers', 'ciphers', 'CIPHERS',
                      'MACs', 'Macs', 'macs', 'MACS',
                      'UsePAM', 'UsePam', 'usepam', 'USEPAM', 'Usepam',
                      'MaxAuthTries', 'maxauthtries', 'MAXAUTHTRIES', 'Maxauthtries',
```

### Comparing `insights-core-3.1.9/insights/tests/test_vulnerable_kernel.py` & `insights-core-3.2.0/insights/tests/test_vulnerable_kernel.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_xmlparser.py` & `insights-core-3.2.0/insights/tests/test_xmlparser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tests/test_yaml_parser.py` & `insights-core-3.2.0/insights/tests/test_yaml_parser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tools/apply_spec_filters.py` & `insights-core-3.2.0/insights/tools/apply_spec_filters.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tools/cat.py` & `insights-core-3.2.0/insights/tools/cat.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tools/dupkeycheck.py` & `insights-core-3.2.0/insights/tools/dupkeycheck.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tools/insights_inspect.py` & `insights-core-3.2.0/insights/tools/insights_inspect.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/tools/query.py` & `insights-core-3.2.0/insights/tools/query.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/util/autology/datasources.py` & `insights-core-3.2.0/insights/util/autology/datasources.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/util/__init__.py` & `insights-core-3.2.0/insights/util/__init__.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/util/canonical_facts.py` & `insights-core-3.2.0/insights/util/canonical_facts.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/util/command.py` & `insights-core-3.2.0/insights/util/command.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/util/component_graph.py` & `insights-core-3.2.0/insights/util/component_graph.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/util/content_type.py` & `insights-core-3.2.0/insights/util/content_type.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/util/file_permissions.py` & `insights-core-3.2.0/insights/util/file_permissions.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/util/fs.py` & `insights-core-3.2.0/insights/util/fs.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/util/mangle.py` & `insights-core-3.2.0/insights/util/mangle.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/util/specs_catalog.py` & `insights-core-3.2.0/insights/util/specs_catalog.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/util/streams.py` & `insights-core-3.2.0/insights/util/streams.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/util/subproc.py` & `insights-core-3.2.0/insights/util/subproc.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/__init__.py` & `insights-core-3.2.0/insights/__init__.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/collect.py` & `insights-core-3.2.0/insights/collect.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 and what to serialize. If a manifest isn't provided, a default one is used that
 runs all datasources in ``insights.specs.Specs`` and
 ``insights.specs.default.DefaultSpecs`` and saves all datasources in
 ``insights.specs.Specs``.
 """
 from __future__ import print_function
 import argparse
-import json
 import logging
 import os
 import sys
 import tempfile
 import yaml
 
 from datetime import datetime
@@ -437,19 +436,14 @@
     parallel = run_strategy.get("name") == "parallel"
     pool_args = run_strategy.get("args", {})
     with get_pool(parallel, "insights-collector-pool", pool_args) as pool:
         h = Hydration(output_path, pool=pool)
         broker.add_observer(h.make_persister(to_persist))
         dr.run_all(broker=broker, pool=pool)
 
-    if BLACKLISTED_SPECS:
-        _write_out_blacklisted_specs(output_path)
-        # Delete the list so the specs aren't written again by the client.
-        del BLACKLISTED_SPECS[:]
-
     collect_errors = _parse_broker_exceptions(broker, EXCEPTIONS_TO_REPORT)
 
     if compress:
         return create_archive(output_path), collect_errors
     return output_path, collect_errors
 
 
@@ -477,49 +471,14 @@
                         else:
                             errors[ex_type] = [(ex, component)]
     except Exception as e:
         log.warning("Could not parse exceptions from the broker.: %s", str(e))
     return errors
 
 
-def _write_out_blacklisted_specs(output_path):
-    """
-    Write out the blacklisted specs to blacklisted_specs.txt, and create
-    a meta-data file for this file. That way it can be loaded when the
-    archive is processed.
-
-    Args:
-        output_path (str): Path of the output directory.
-    """
-    if os.path.exists(os.path.join(output_path, "meta_data")):
-        output_path_root = os.path.join(output_path, "data")
-    else:
-        output_path_root = output_path
-
-    with open(os.path.join(output_path_root, "blacklisted_specs.txt"), "w") as of:
-        json.dump({"specs": BLACKLISTED_SPECS}, of)
-
-    doc = {
-        "name": "insights.specs.Specs.blacklisted_specs",
-        "exec_time": 0.0,
-        "errors": [],
-        "results": {
-            "type": "insights.core.spec_factory.DatasourceProvider",
-            "object": {
-                "relative_path": "blacklisted_specs.txt"
-            }
-        },
-        "ser_time": 0.0
-    }
-
-    meta_path = os.path.join(os.path.join(output_path, "meta_data"), "insights.specs.Specs.blacklisted_specs")
-    with open(meta_path, "w") as of:
-        json.dump(doc, of)
-
-
 def main():
     # Remove command line args so that they are not parsed by any called modules
     # The main fxn is only invoked as a cli, if calling from another cli then
     # use the collect function instead
     collect_args = [arg for arg in sys.argv[1:]] if len(sys.argv) > 1 else []
     sys.argv = [sys.argv[0], ] if sys.argv else sys.argv
```

### Comparing `insights-core-3.1.9/insights/command_parser.py` & `insights-core-3.2.0/insights/command_parser.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/defaults.yaml` & `insights-core-3.2.0/insights/defaults.yaml`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/ocp.py` & `insights-core-3.2.0/insights/ocp.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/ocpshell.py` & `insights-core-3.2.0/insights/ocpshell.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/settings.py` & `insights-core-3.2.0/insights/settings.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights/shell.py` & `insights-core-3.2.0/insights/shell.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/insights_core.egg-info/PKG-INFO` & `insights-core-3.2.0/insights_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insights-core
-Version: 3.1.9
+Version: 3.2.0
 Summary: Insights Core is a data collection and analysis framework
 Home-page: https://github.com/redhatinsights/insights-core
 Author: Red Hat, Inc.
 Author-email: insights@redhat.com
 License: Apache 2.0
 Description: =============
         Insights Core
@@ -156,17 +156,17 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: develop
+Provides-Extra: develop26
 Provides-Extra: client-develop
-Provides-Extra: linting
-Provides-Extra: cluster
 Provides-Extra: openshift
-Provides-Extra: develop26
-Provides-Extra: testing
-Provides-Extra: optional
-Provides-Extra: develop
 Provides-Extra: client
+Provides-Extra: optional
+Provides-Extra: testing
 Provides-Extra: docs
+Provides-Extra: cluster
+Provides-Extra: linting
```

### Comparing `insights-core-3.1.9/insights_core.egg-info/SOURCES.txt` & `insights-core-3.2.0/insights_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -98,28 +98,29 @@
 insights/combiners/cryptsetup.py
 insights/combiners/dmesg.py
 insights/combiners/dnsmasq_conf_all.py
 insights/combiners/du.py
 insights/combiners/grub_conf.py
 insights/combiners/hostname.py
 insights/combiners/httpd_conf.py
+insights/combiners/identity_domain.py
+insights/combiners/ipa.py
 insights/combiners/ipcs_semaphores.py
 insights/combiners/ipcs_shared_memory.py
 insights/combiners/ipv6.py
 insights/combiners/journald_conf.py
 insights/combiners/krb5.py
 insights/combiners/limits_conf.py
 insights/combiners/logrotate_conf.py
 insights/combiners/lspci.py
 insights/combiners/lvm.py
 insights/combiners/md5check.py
 insights/combiners/mlx4_port.py
 insights/combiners/modinfo.py
 insights/combiners/modprobe.py
-insights/combiners/mounts.py
 insights/combiners/multinode.py
 insights/combiners/netstat.py
 insights/combiners/nfs_exports.py
 insights/combiners/nginx_conf.py
 insights/combiners/nmcli_dev_show.py
 insights/combiners/os_release.py
 insights/combiners/ps.py
@@ -190,15 +191,14 @@
 insights/parsers/__init__.py
 insights/parsers/abrt_ccpp.py
 insights/parsers/abrt_status_bare.py
 insights/parsers/alternatives.py
 insights/parsers/amq_broker.py
 insights/parsers/audit_log.py
 insights/parsers/auditctl.py
-insights/parsers/auditctl_status.py
 insights/parsers/auditd_conf.py
 insights/parsers/authselect.py
 insights/parsers/autofs_conf.py
 insights/parsers/avc_cache_threshold.py
 insights/parsers/avc_hash_stats.py
 insights/parsers/aws_instance_id.py
 insights/parsers/awx_manage.py
@@ -227,14 +227,15 @@
 insights/parsers/certificates_enddate.py
 insights/parsers/cgroups.py
 insights/parsers/checkin_conf.py
 insights/parsers/chkconfig.py
 insights/parsers/cib.py
 insights/parsers/cinder_conf.py
 insights/parsers/cinder_log.py
+insights/parsers/client_metadata.py
 insights/parsers/cloud_cfg.py
 insights/parsers/cloud_init_custom_network.py
 insights/parsers/cloud_init_log.py
 insights/parsers/cluster_conf.py
 insights/parsers/cmdline.py
 insights/parsers/cni_podman_bridge_conf.py
 insights/parsers/cobbler_modules_conf.py
@@ -252,14 +253,15 @@
 insights/parsers/crictl_logs.py
 insights/parsers/crio_conf.py
 insights/parsers/cron_daily_rhsmd.py
 insights/parsers/cron_jobs.py
 insights/parsers/crontab.py
 insights/parsers/crypto_policies.py
 insights/parsers/cryptsetup_luksDump.py
+insights/parsers/cups_confs.py
 insights/parsers/cups_ppd.py
 insights/parsers/current_clocksource.py
 insights/parsers/date.py
 insights/parsers/db2.py
 insights/parsers/dcbtool_gc_dcb.py
 insights/parsers/designate_conf.py
 insights/parsers/df.py
@@ -282,14 +284,15 @@
 insights/parsers/dracut_modules.py
 insights/parsers/dse_ldif_simple.py
 insights/parsers/du.py
 insights/parsers/dumpe2fs_h.py
 insights/parsers/engine_config.py
 insights/parsers/engine_db_query.py
 insights/parsers/engine_log.py
+insights/parsers/etc_machine_id.py
 insights/parsers/etcd_conf.py
 insights/parsers/ethtool.py
 insights/parsers/facter.py
 insights/parsers/fapolicyd_rules.py
 insights/parsers/fc_match.py
 insights/parsers/fcoeadm_i.py
 insights/parsers/findmnt.py
@@ -300,14 +303,15 @@
 insights/parsers/foreman_rake_db_migrate_status.py
 insights/parsers/freeipa_healthcheck_log.py
 insights/parsers/fstab.py
 insights/parsers/fwupdagent.py
 insights/parsers/galera_cnf.py
 insights/parsers/gcp_instance_type.py
 insights/parsers/gcp_license_codes.py
+insights/parsers/gcp_network_interfaces.py
 insights/parsers/getcert_list.py
 insights/parsers/getconf_pagesize.py
 insights/parsers/getenforce.py
 insights/parsers/getsebool.py
 insights/parsers/gfs2_file_system_block_size.py
 insights/parsers/glance_log.py
 insights/parsers/gluster_peer_status.py
@@ -338,26 +342,25 @@
 insights/parsers/initscript.py
 insights/parsers/insights_client_conf.py
 insights/parsers/installed_product_ids.py
 insights/parsers/installed_rpms.py
 insights/parsers/interrupts.py
 insights/parsers/ip.py
 insights/parsers/ip_netns_exec_namespace_lsof.py
+insights/parsers/ipa_conf.py
 insights/parsers/ipaupgrade_log.py
 insights/parsers/ipcs.py
 insights/parsers/ipsec_conf.py
 insights/parsers/iptables.py
 insights/parsers/ironic_conf.py
 insights/parsers/ironic_inspector_log.py
 insights/parsers/iscsiadm_mode_session.py
 insights/parsers/jboss_domain_log.py
 insights/parsers/jboss_standalone_main_conf.py
 insights/parsers/jboss_version.py
-insights/parsers/journal_all.py
-insights/parsers/journal_since_boot.py
 insights/parsers/journalctl.py
 insights/parsers/journald_conf.py
 insights/parsers/katello_service_status.py
 insights/parsers/kdump.py
 insights/parsers/kernel_config.py
 insights/parsers/keystone.py
 insights/parsers/keystone_log.py
@@ -365,14 +368,15 @@
 insights/parsers/krb5.py
 insights/parsers/krb5kdc_log.py
 insights/parsers/ksmstate.py
 insights/parsers/ktimer_lockless.py
 insights/parsers/kubepods_cpu_quota.py
 insights/parsers/ld_library_path.py
 insights/parsers/ldif_config.py
+insights/parsers/leapp.py
 insights/parsers/libssh_config.py
 insights/parsers/libvirtd_log.py
 insights/parsers/limits_conf.py
 insights/parsers/logrotate_conf.py
 insights/parsers/losetup.py
 insights/parsers/lpstat.py
 insights/parsers/ls_boot.py
@@ -383,24 +387,26 @@
 insights/parsers/ls_etc.py
 insights/parsers/ls_ipa_idoverride_memberof.py
 insights/parsers/ls_krb5_sssd.py
 insights/parsers/ls_lib_firmware.py
 insights/parsers/ls_ocp_cni_openshift_sdn.py
 insights/parsers/ls_origin_local_volumes_pods.py
 insights/parsers/ls_osroot.py
+insights/parsers/ls_rsyslog_errorfile.py
 insights/parsers/ls_sys_firmware.py
 insights/parsers/ls_systemd_units.py
 insights/parsers/ls_tmp.py
 insights/parsers/ls_usr_bin.py
 insights/parsers/ls_usr_lib64.py
 insights/parsers/ls_usr_sbin.py
 insights/parsers/ls_var_cache_pulp.py
 insights/parsers/ls_var_lib_mongodb.py
 insights/parsers/ls_var_lib_nova_instances.py
 insights/parsers/ls_var_lib_pcp.py
+insights/parsers/ls_var_lib_rpm.py
 insights/parsers/ls_var_lib_rsyslog.py
 insights/parsers/ls_var_log.py
 insights/parsers/ls_var_opt_mssql.py
 insights/parsers/ls_var_opt_mssql_log.py
 insights/parsers/ls_var_run.py
 insights/parsers/ls_var_spool_clientmq.py
 insights/parsers/ls_var_spool_postfix_maildrop.py
@@ -413,14 +419,15 @@
 insights/parsers/lsof.py
 insights/parsers/lspci.py
 insights/parsers/lssap.py
 insights/parsers/lsscsi.py
 insights/parsers/luksmeta.py
 insights/parsers/lvdisplay.py
 insights/parsers/lvm.py
+insights/parsers/machine_id.py
 insights/parsers/manila_conf.py
 insights/parsers/mariadb_log.py
 insights/parsers/max_uid.py
 insights/parsers/md5check.py
 insights/parsers/mdadm.py
 insights/parsers/mdstat.py
 insights/parsers/meminfo.py
@@ -514,14 +521,15 @@
 insights/parsers/podman_inspect.py
 insights/parsers/podman_list.py
 insights/parsers/postconf.py
 insights/parsers/postgresql_conf.py
 insights/parsers/postgresql_log.py
 insights/parsers/proc_environ.py
 insights/parsers/proc_keys.py
+insights/parsers/proc_keyusers.py
 insights/parsers/proc_limits.py
 insights/parsers/proc_stat.py
 insights/parsers/ps.py
 insights/parsers/pulp_worker_defaults.py
 insights/parsers/puppet_ca_cert_expire_date.py
 insights/parsers/qemu_conf.py
 insights/parsers/qemu_xml.py
@@ -530,14 +538,15 @@
 insights/parsers/rabbitmq.py
 insights/parsers/rabbitmq_log.py
 insights/parsers/rc_local.py
 insights/parsers/rdma_config.py
 insights/parsers/readlink_e_mtab.py
 insights/parsers/readlink_openshift_certs.py
 insights/parsers/redhat_release.py
+insights/parsers/repquota.py
 insights/parsers/resolv_conf.py
 insights/parsers/rhev_data_center.py
 insights/parsers/rhn_charsets.py
 insights/parsers/rhn_conf.py
 insights/parsers/rhn_entitlement_cert_xml.py
 insights/parsers/rhn_hibernate_conf.py
 insights/parsers/rhn_logs.py
@@ -604,14 +613,15 @@
 insights/parsers/sssd_logs.py
 insights/parsers/subscription_manager.py
 insights/parsers/subscription_manager_list.py
 insights/parsers/subscription_manager_release.py
 insights/parsers/sudoers.py
 insights/parsers/swift_conf.py
 insights/parsers/swift_log.py
+insights/parsers/sys_block.py
 insights/parsers/sys_bus.py
 insights/parsers/sys_fs_cgroup_memory.py
 insights/parsers/sys_fs_cgroup_memory_tasks_number.py
 insights/parsers/sys_kernel.py
 insights/parsers/sys_module.py
 insights/parsers/sys_vmbus.py
 insights/parsers/sysconfig.py
@@ -735,22 +745,25 @@
 insights/specs/datasources/corosync.py
 insights/specs/datasources/dir_list.py
 insights/specs/datasources/ethernet.py
 insights/specs/datasources/httpd.py
 insights/specs/datasources/ipcs.py
 insights/specs/datasources/kernel.py
 insights/specs/datasources/kernel_module_list.py
+insights/specs/datasources/leapp.py
 insights/specs/datasources/lpstat.py
 insights/specs/datasources/luks_devices.py
+insights/specs/datasources/machine_ids.py
 insights/specs/datasources/malware_detection.py
 insights/specs/datasources/md5chk.py
 insights/specs/datasources/package_provides.py
 insights/specs/datasources/pcp.py
 insights/specs/datasources/ps.py
 insights/specs/datasources/rpm_pkgs.py
+insights/specs/datasources/rsyslog_confs.py
 insights/specs/datasources/sap.py
 insights/specs/datasources/satellite_missed_queues.py
 insights/specs/datasources/semanage.py
 insights/specs/datasources/ssl_certificate.py
 insights/specs/datasources/sys_fs_cgroup_memory.py
 insights/specs/datasources/sys_fs_cgroup_memory_tasks_number.py
 insights/specs/datasources/user_group.py
@@ -760,16 +773,16 @@
 insights/specs/datasources/container/nginx_conf.py
 insights/tests/__init__.py
 insights/tests/helpers.py
 insights/tests/integration.py
 insights/tests/mock_web_server.py
 insights/tests/spec_tests.py
 insights/tests/test_add_component.py
-insights/tests/test_add_exception.py
 insights/tests/test_always_fires.py
+insights/tests/test_broker_exceptions.py
 insights/tests/test_canonical_facts.py
 insights/tests/test_collect.py
 insights/tests/test_command_parser.py
 insights/tests/test_commandparser.py
 insights/tests/test_component_metadata.py
 insights/tests/test_config_parser.py
 insights/tests/test_context.py
@@ -822,29 +835,30 @@
 insights/tests/combiners/test_cryptsetup.py
 insights/tests/combiners/test_dmesg.py
 insights/tests/combiners/test_dnsmasq_conf_all.py
 insights/tests/combiners/test_du.py
 insights/tests/combiners/test_grub_conf.py
 insights/tests/combiners/test_hostname.py
 insights/tests/combiners/test_httpd_conf_tree.py
+insights/tests/combiners/test_identity_domain.py
+insights/tests/combiners/test_ipa.py
 insights/tests/combiners/test_ipcs_semaphores.py
 insights/tests/combiners/test_ipcs_shared_memory.py
 insights/tests/combiners/test_ipv6.py
 insights/tests/combiners/test_journald_conf.py
 insights/tests/combiners/test_krb5.py
 insights/tests/combiners/test_limits_conf.py
 insights/tests/combiners/test_logrotate_conf.py
 insights/tests/combiners/test_logrotate_conf_tree.py
 insights/tests/combiners/test_lspci.py
 insights/tests/combiners/test_lvm.py
 insights/tests/combiners/test_md5check.py
 insights/tests/combiners/test_mlx4_port.py
 insights/tests/combiners/test_modinfo.py
 insights/tests/combiners/test_modprobe.py
-insights/tests/combiners/test_mounts.py
 insights/tests/combiners/test_netstat.py
 insights/tests/combiners/test_nfs_exports.py
 insights/tests/combiners/test_nginx_conf.py
 insights/tests/combiners/test_nmcli_dev_show.py
 insights/tests/combiners/test_os_release.py
 insights/tests/combiners/test_ps.py
 insights/tests/combiners/test_redhat_release.py
@@ -884,20 +898,23 @@
 insights/tests/datasources/test_dir_list.py
 insights/tests/datasources/test_ethernet.py
 insights/tests/datasources/test_get_running_commands.py
 insights/tests/datasources/test_httpd.py
 insights/tests/datasources/test_ipcs.py
 insights/tests/datasources/test_kernel.py
 insights/tests/datasources/test_kernel_module_list.py
+insights/tests/datasources/test_leapp.py
 insights/tests/datasources/test_lpstat.py
 insights/tests/datasources/test_luks_devices.py
+insights/tests/datasources/test_machine_ids.py
 insights/tests/datasources/test_package_provides.py
 insights/tests/datasources/test_pcp.py
 insights/tests/datasources/test_ps.py
 insights/tests/datasources/test_rpm_pkgs.py
+insights/tests/datasources/test_rsyslog_confs.py
 insights/tests/datasources/test_sap.py
 insights/tests/datasources/test_satellite_missed_queues.py
 insights/tests/datasources/test_semanage.py
 insights/tests/datasources/test_ssl_certificate.py
 insights/tests/datasources/test_sys_fs_cgroup_memory.py
 insights/tests/datasources/test_sys_fs_cgroup_memory_tasks_number.py
 insights/tests/datasources/test_user_group.py
@@ -910,15 +927,14 @@
 insights/tests/parsers/lvm_test_data.py
 insights/tests/parsers/test_abrt_ccpp.py
 insights/tests/parsers/test_abrt_status_bare.py
 insights/tests/parsers/test_alternatives.py
 insights/tests/parsers/test_amq_broker.py
 insights/tests/parsers/test_audit_log.py
 insights/tests/parsers/test_auditctl.py
-insights/tests/parsers/test_auditctl_status.py
 insights/tests/parsers/test_auditd_conf.py
 insights/tests/parsers/test_authselect.py
 insights/tests/parsers/test_autofs_conf.py
 insights/tests/parsers/test_avc_cache_threshold.py
 insights/tests/parsers/test_avc_hash_stats.py
 insights/tests/parsers/test_aws_instance_id.py
 insights/tests/parsers/test_awx_manage.py
@@ -947,14 +963,15 @@
 insights/tests/parsers/test_certificates_enddate.py
 insights/tests/parsers/test_cgroups.py
 insights/tests/parsers/test_checkin_conf.py
 insights/tests/parsers/test_chkconfig.py
 insights/tests/parsers/test_cib.py
 insights/tests/parsers/test_cinder_conf.py
 insights/tests/parsers/test_cinder_log.py
+insights/tests/parsers/test_client_metadata.py
 insights/tests/parsers/test_cloud_cfg.py
 insights/tests/parsers/test_cloud_init_custom_network.py
 insights/tests/parsers/test_cloud_init_log.py
 insights/tests/parsers/test_cluster_conf.py
 insights/tests/parsers/test_cmdline.py
 insights/tests/parsers/test_cni_podman_bridge_conf.py
 insights/tests/parsers/test_cobbler_modules_conf.py
@@ -976,14 +993,15 @@
 insights/tests/parsers/test_crontab.py
 insights/tests/parsers/test_crypto_policies_bind.py
 insights/tests/parsers/test_crypto_policies_config.py
 insights/tests/parsers/test_crypto_policies_doc_examples.py
 insights/tests/parsers/test_crypto_policies_opensshserver.py
 insights/tests/parsers/test_crypto_policies_state_current.py
 insights/tests/parsers/test_cryptsetup_luksDump.py
+insights/tests/parsers/test_cups_confs.py
 insights/tests/parsers/test_cups_ppd.py
 insights/tests/parsers/test_current_clocksource.py
 insights/tests/parsers/test_date.py
 insights/tests/parsers/test_db2.py
 insights/tests/parsers/test_dcbtool_gc_dcb.py
 insights/tests/parsers/test_designate_conf.py
 insights/tests/parsers/test_df.py
@@ -1006,14 +1024,15 @@
 insights/tests/parsers/test_dracut_modules.py
 insights/tests/parsers/test_dse_ldif_simple.py
 insights/tests/parsers/test_du.py
 insights/tests/parsers/test_dumpe2fs_h.py
 insights/tests/parsers/test_engine_config.py
 insights/tests/parsers/test_engine_db_query.py
 insights/tests/parsers/test_engine_log.py
+insights/tests/parsers/test_etc_machine_id.py
 insights/tests/parsers/test_etcd_conf.py
 insights/tests/parsers/test_ethtool.py
 insights/tests/parsers/test_facter.py
 insights/tests/parsers/test_fapolicyd_rules.py
 insights/tests/parsers/test_fc_match.py
 insights/tests/parsers/test_fcoeadm_i.py
 insights/tests/parsers/test_findmnt.py
@@ -1024,14 +1043,15 @@
 insights/tests/parsers/test_foreman_rake_db_migrate_status.py
 insights/tests/parsers/test_freeipa_healthcheck_log.py
 insights/tests/parsers/test_fstab.py
 insights/tests/parsers/test_fwupdagent.py
 insights/tests/parsers/test_galera_cnf.py
 insights/tests/parsers/test_gcp_instance_type.py
 insights/tests/parsers/test_gcp_license_codes.py
+insights/tests/parsers/test_gcp_network_interfaces.py
 insights/tests/parsers/test_getcert_list.py
 insights/tests/parsers/test_getconf_pagesize.py
 insights/tests/parsers/test_getenforce.py
 insights/tests/parsers/test_getsebool.py
 insights/tests/parsers/test_gfs2_file_system_block_size.py
 insights/tests/parsers/test_glance_log.py
 insights/tests/parsers/test_gluster_peer_status.py
@@ -1065,26 +1085,25 @@
 insights/tests/parsers/test_initscript.py
 insights/tests/parsers/test_insights_client_conf.py
 insights/tests/parsers/test_installed_product_ids.py
 insights/tests/parsers/test_installed_rpms.py
 insights/tests/parsers/test_interrupts.py
 insights/tests/parsers/test_ip.py
 insights/tests/parsers/test_ip_netns_exec_namespace_lsof.py
+insights/tests/parsers/test_ipa_conf.py
 insights/tests/parsers/test_ipaupgrade_log.py
 insights/tests/parsers/test_ipcs.py
 insights/tests/parsers/test_ipsec_conf.py
 insights/tests/parsers/test_iptables.py
 insights/tests/parsers/test_ironic_conf.py
 insights/tests/parsers/test_ironic_inspector_log.py
 insights/tests/parsers/test_iscsiadm_mode_session.py
 insights/tests/parsers/test_jboss_domain_log.py
 insights/tests/parsers/test_jboss_standalone_main_conf.py
 insights/tests/parsers/test_jboss_version.py
-insights/tests/parsers/test_journal_all.py
-insights/tests/parsers/test_journal_since_boot.py
 insights/tests/parsers/test_journalctl.py
 insights/tests/parsers/test_journald_conf.py
 insights/tests/parsers/test_katello_service_status.py
 insights/tests/parsers/test_kdump.py
 insights/tests/parsers/test_kernel_config.py
 insights/tests/parsers/test_keystone.py
 insights/tests/parsers/test_keystone_log.py
@@ -1092,14 +1111,15 @@
 insights/tests/parsers/test_krb5.py
 insights/tests/parsers/test_krb5kdc_log.py
 insights/tests/parsers/test_ksmstate.py
 insights/tests/parsers/test_ktimer_lockless.py
 insights/tests/parsers/test_kubepods_cpu_quota.py
 insights/tests/parsers/test_ld_library_path.py
 insights/tests/parsers/test_ldif_config.py
+insights/tests/parsers/test_leapp.py
 insights/tests/parsers/test_libssh_config.py
 insights/tests/parsers/test_libvirtd_log.py
 insights/tests/parsers/test_limits_conf.py
 insights/tests/parsers/test_logrotate_conf.py
 insights/tests/parsers/test_losetup.py
 insights/tests/parsers/test_lpstat.py
 insights/tests/parsers/test_ls_boot.py
@@ -1110,24 +1130,26 @@
 insights/tests/parsers/test_ls_etc.py
 insights/tests/parsers/test_ls_ipa_idoverride_memberof.py
 insights/tests/parsers/test_ls_krb5_sssd.py
 insights/tests/parsers/test_ls_lib_firmware.py
 insights/tests/parsers/test_ls_ocp_nci_openshift_sdn.py
 insights/tests/parsers/test_ls_origin_local_volumes_pods.py
 insights/tests/parsers/test_ls_osroot.py
+insights/tests/parsers/test_ls_rsyslog_errorfile.py
 insights/tests/parsers/test_ls_sys_firmware.py
 insights/tests/parsers/test_ls_systemd_units.py
 insights/tests/parsers/test_ls_tmp.py
 insights/tests/parsers/test_ls_usr_bin.py
 insights/tests/parsers/test_ls_usr_lib64.py
 insights/tests/parsers/test_ls_usr_sbin.py
 insights/tests/parsers/test_ls_var_cache_pulp.py
 insights/tests/parsers/test_ls_var_lib_mongodb.py
 insights/tests/parsers/test_ls_var_lib_nova_instances.py
 insights/tests/parsers/test_ls_var_lib_pcp.py
+insights/tests/parsers/test_ls_var_lib_rpm.py
 insights/tests/parsers/test_ls_var_lib_rsyslog.py
 insights/tests/parsers/test_ls_var_log.py
 insights/tests/parsers/test_ls_var_opt_mssql.py
 insights/tests/parsers/test_ls_var_opt_mssql_log.py
 insights/tests/parsers/test_ls_var_run.py
 insights/tests/parsers/test_ls_var_spool_clientmq.py
 insights/tests/parsers/test_ls_var_spool_postfix_maildrop.py
@@ -1142,14 +1164,15 @@
 insights/tests/parsers/test_lssap.py
 insights/tests/parsers/test_lsscsi.py
 insights/tests/parsers/test_luksmeta.py
 insights/tests/parsers/test_lvdisplay.py
 insights/tests/parsers/test_lvm.py
 insights/tests/parsers/test_lvm_conf.py
 insights/tests/parsers/test_lvs.py
+insights/tests/parsers/test_machine_id.py
 insights/tests/parsers/test_manila_conf.py
 insights/tests/parsers/test_mariadb_log.py
 insights/tests/parsers/test_max_uid.py
 insights/tests/parsers/test_md5check.py
 insights/tests/parsers/test_mdadm.py
 insights/tests/parsers/test_mdstat.py
 insights/tests/parsers/test_meminfo.py
@@ -1243,14 +1266,15 @@
 insights/tests/parsers/test_podman_inspect.py
 insights/tests/parsers/test_podman_list.py
 insights/tests/parsers/test_postconf.py
 insights/tests/parsers/test_postgresql_conf.py
 insights/tests/parsers/test_postgresql_log.py
 insights/tests/parsers/test_proc_environ.py
 insights/tests/parsers/test_proc_keys.py
+insights/tests/parsers/test_proc_keyusers.py
 insights/tests/parsers/test_proc_limits.py
 insights/tests/parsers/test_proc_stat.py
 insights/tests/parsers/test_ps.py
 insights/tests/parsers/test_pulp_worker_defaults.py
 insights/tests/parsers/test_puppet_ca_cert_expire_date.py
 insights/tests/parsers/test_pvs.py
 insights/tests/parsers/test_qemu_conf.py
@@ -1263,14 +1287,15 @@
 insights/tests/parsers/test_rabbitmq_queues.py
 insights/tests/parsers/test_rabbitmq_report.py
 insights/tests/parsers/test_rc_local.py
 insights/tests/parsers/test_rdma_config.py
 insights/tests/parsers/test_readlink_mtab.py
 insights/tests/parsers/test_readlink_openshift_certs.py
 insights/tests/parsers/test_redhat_release.py
+insights/tests/parsers/test_repquota.py
 insights/tests/parsers/test_resolv_conf.py
 insights/tests/parsers/test_rhev_data_center.py
 insights/tests/parsers/test_rhn_charsets.py
 insights/tests/parsers/test_rhn_conf.py
 insights/tests/parsers/test_rhn_entitlement_cert_xml.py
 insights/tests/parsers/test_rhn_hibernate_conf.py
 insights/tests/parsers/test_rhn_logs.py
@@ -1337,14 +1362,15 @@
 insights/tests/parsers/test_sssd_logs.py
 insights/tests/parsers/test_subscription_manager.py
 insights/tests/parsers/test_subscription_manager_list.py
 insights/tests/parsers/test_subscription_manager_release.py
 insights/tests/parsers/test_sudoers.py
 insights/tests/parsers/test_swift_conf.py
 insights/tests/parsers/test_swift_log.py
+insights/tests/parsers/test_sys_block.py
 insights/tests/parsers/test_sys_bus.py
 insights/tests/parsers/test_sys_fs_cgroup_memory.py
 insights/tests/parsers/test_sys_fs_cgroup_memory_tasks_number.py
 insights/tests/parsers/test_sys_kernel.py
 insights/tests/parsers/test_sys_module.py
 insights/tests/parsers/test_sys_vmbus.py
 insights/tests/parsers/test_sysconfig_chronyd.py
```

### Comparing `insights-core-3.1.9/insights_core.egg-info/requires.txt` & `insights-core-3.2.0/insights_core.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-defusedxml
 redis
-six
-cachecontrol
+cachecontrol[filecache]
 requests
-cachecontrol[redis]
 lockfile
-cachecontrol[filecache]
+defusedxml
+six
+cachecontrol[redis]
+cachecontrol
 
 [:python_version < "2.7"]
 pyyaml<=3.13,>=3.10
 
 [:python_version <= "2.7"]
 jinja2<=2.11.3
 
 [:python_version > "2.7"]
 jinja2
 
 [:python_version >= "2.7"]
 pyyaml
 
 [client]
-oyaml
-defusedxml
 redis
-six
-cachecontrol
-requests
-cachecontrol[redis]
 python-gnupg==0.4.6
-lockfile
 cachecontrol[filecache]
+requests
+lockfile
+defusedxml
+six
+cachecontrol[redis]
+cachecontrol
+oyaml
 
 [client-develop]
-oyaml
 redis
-six
-mock==2.0.0
-cachecontrol[redis]
-lockfile
 python-gnupg==0.4.6
-defusedxml
+cachecontrol[filecache]
+wheel
+cachecontrol[redis]
 cachecontrol
 requests
-wheel
-cachecontrol[filecache]
+lockfile
+defusedxml
+six
+mock==2.0.0
+oyaml
 
 [client-develop:python_version < "2.7"]
-flake8==2.6.2
-pytest-cov==2.4.0
+pytest==3.0.6
 coverage==4.3.4
+pytest-cov==2.4.0
 pyyaml<=3.13,>=3.10
-pytest==3.0.6
+flake8==2.6.2
 
 [client-develop:python_version <= "2.7"]
 jinja2<=2.11.3
 
 [client-develop:python_version == "2.7"]
 pytest~=4.6.0
 
 [client-develop:python_version > "2.7"]
 jinja2
 
 [client-develop:python_version >= "2.7"]
 pyyaml
-flake8
-coverage
 pytest-cov
+coverage
+flake8
 
 [client-develop:python_version >= "3"]
 pytest
 
 [client:python_version < "2.7"]
 pyyaml<=3.13,>=3.10
 
@@ -79,194 +79,194 @@
 [client:python_version > "2.7"]
 jinja2
 
 [client:python_version >= "2.7"]
 pyyaml
 
 [cluster]
-colorama
-defusedxml
 redis
-six
-cachecontrol
-pandas
+cachecontrol[filecache]
 requests
-cachecontrol[redis]
+pandas
 ansible
 lockfile
-cachecontrol[filecache]
+defusedxml
+six
+cachecontrol[redis]
+cachecontrol
+colorama
 
 [cluster:python_version < "2.7"]
 pyyaml<=3.13,>=3.10
 
 [cluster:python_version <= "2.7"]
 jinja2<=2.11.3
 
 [cluster:python_version > "2.7"]
 jinja2
 
 [cluster:python_version >= "2.7"]
 pyyaml
 
 [develop]
-oyaml
-nbsphinx
-six
-sphinx_rtd_theme
-ipython<8.7.0
+redis
+cachecontrol[filecache]
 Pygments
-jedi
+oyaml
+lockfile
 defusedxml
+six
 docutils
-colorama
-pandas
-redis
 mock==2.0.0
-cachecontrol[redis]
-ansible
-lockfile
 MarkupSafe==2.0.1
+colorama
 python-gnupg==0.4.6
-Sphinx
+pandas
+nbsphinx
+wheel
+cachecontrol[redis]
 cachecontrol
+sphinx_rtd_theme
 requests
-wheel
-cachecontrol[filecache]
+ansible
+jedi
+Sphinx
+ipython<8.7.0
 
 [develop26]
-oyaml
-colorama
-pandas
 redis
-six
-mock==2.0.0
+python-gnupg==0.4.6
+cachecontrol[filecache]
+pandas
+wheel
 cachecontrol[redis]
+cachecontrol
+requests
 ansible
 lockfile
-python-gnupg==0.4.6
 defusedxml
-cachecontrol
-requests
-wheel
-cachecontrol[filecache]
+six
+colorama
+mock==2.0.0
+oyaml
 
 [develop26:python_version < "2.7"]
-flake8==2.6.2
-pytest-cov==2.4.0
+pytest==3.0.6
 coverage==4.3.4
+pytest-cov==2.4.0
 pyyaml<=3.13,>=3.10
-pytest==3.0.6
+flake8==2.6.2
 
 [develop26:python_version <= "2.7"]
 jinja2<=2.11.3
 
 [develop26:python_version == "2.7"]
 pytest~=4.6.0
 
 [develop26:python_version > "2.7"]
 jinja2
 
 [develop26:python_version >= "2.7"]
 pyyaml
-flake8
-coverage
 pytest-cov
+coverage
+flake8
 
 [develop26:python_version >= "3"]
 pytest
 
 [develop:python_version < "2.7"]
-flake8==2.6.2
 pytest-cov==2.4.0
+pytest==3.0.6
 coverage==4.3.4
 pyyaml<=3.13,>=3.10
-pytest==3.0.6
+flake8==2.6.2
 
 [develop:python_version <= "2.7"]
 jinja2<=2.11.3
 
 [develop:python_version == "2.7"]
 pytest~=4.6.0
 
 [develop:python_version > "2.7"]
 jinja2
 
 [develop:python_version >= "2.7"]
 pyyaml
+pytest-cov
 flake8
 coverage
-pytest-cov
 
 [develop:python_version >= "3"]
 pytest
 
 [docs]
-Sphinx
-nbsphinx
-colorama
 Pygments
-docutils
 jedi
+nbsphinx
+Sphinx
+docutils
+ipython<8.7.0
 MarkupSafe==2.0.1
 sphinx_rtd_theme
-ipython<8.7.0
+colorama
 
 [linting]
+python-gnupg==0.4.6
 requests
 oyaml
-python-gnupg==0.4.6
 
 [linting:python_version < "2.7"]
 flake8==2.6.2
 
 [linting:python_version >= "2.7"]
 flake8
 
 [openshift]
+redis
+cachecontrol[filecache]
+requests
 openshift
+lockfile
 defusedxml
-redis
 six
-cachecontrol
-requests
 cachecontrol[redis]
-lockfile
-cachecontrol[filecache]
+cachecontrol
 
 [openshift:python_version < "2.7"]
 pyyaml<=3.13,>=3.10
 
 [openshift:python_version <= "2.7"]
 jinja2<=2.11.3
 
 [openshift:python_version > "2.7"]
 jinja2
 
 [openshift:python_version >= "2.7"]
 pyyaml
 
 [optional]
-watchdog
-python-cjson
-python-logstash
 python-statsd
+python-logstash
+python-cjson
+watchdog
 
 [testing]
-oyaml
-mock==2.0.0
-requests
 python-gnupg==0.4.6
+requests
+mock==2.0.0
+oyaml
 
 [testing:python_version < "2.7"]
-pytest-cov==2.4.0
-coverage==4.3.4
 pytest==3.0.6
+coverage==4.3.4
+pytest-cov==2.4.0
 
 [testing:python_version == "2.7"]
 pytest~=4.6.0
 
 [testing:python_version >= "2.7"]
-coverage
 pytest-cov
+coverage
 
 [testing:python_version >= "3"]
 pytest
```

### Comparing `insights-core-3.1.9/LICENSE` & `insights-core-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/README.rst` & `insights-core-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/setup.py` & `insights-core-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `insights-core-3.1.9/PKG-INFO` & `insights-core-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insights-core
-Version: 3.1.9
+Version: 3.2.0
 Summary: Insights Core is a data collection and analysis framework
 Home-page: https://github.com/redhatinsights/insights-core
 Author: Red Hat, Inc.
 Author-email: insights@redhat.com
 License: Apache 2.0
 Description: =============
         Insights Core
@@ -156,17 +156,17 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: develop
+Provides-Extra: develop26
 Provides-Extra: client-develop
-Provides-Extra: linting
-Provides-Extra: cluster
 Provides-Extra: openshift
-Provides-Extra: develop26
-Provides-Extra: testing
-Provides-Extra: optional
-Provides-Extra: develop
 Provides-Extra: client
+Provides-Extra: optional
+Provides-Extra: testing
 Provides-Extra: docs
+Provides-Extra: cluster
+Provides-Extra: linting
```

