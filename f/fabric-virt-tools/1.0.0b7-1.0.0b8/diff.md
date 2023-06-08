# Comparing `tmp/fabric-virt-tools-1.0.0b7.tar.gz` & `tmp/fabric-virt-tools-1.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-virt-tools-1.0.0b7.tar", last modified: Wed May 31 21:05:27 2023, max compression
+gzip compressed data, was "fabric-virt-tools-1.0.0b8.tar", last modified: Thu Jun  1 14:27:49 2023, max compression
```

## Comparing `fabric-virt-tools-1.0.0b7.tar` & `fabric-virt-tools-1.0.0b8.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-05-31 18:44:31.383234 fabric-virt-tools-1.0.0b7/LICENSE
--rw-r--r--   0        0        0      279 2023-05-31 18:44:17.271476 fabric-virt-tools-1.0.0b7/README.md
--rw-r--r--   0        0        0       24 2023-05-31 21:05:00.042394 fabric-virt-tools-1.0.0b7/fabric_virt_tools/__init__.py
--rw-r--r--   0        0        0     8485 2023-05-31 17:54:08.507450 fabric-virt-tools-1.0.0b7/fabric_virt_tools/cpu_tune.py
--rw-r--r--   0        0        0    12229 2023-05-31 18:39:32.027641 fabric-virt-tools-1.0.0b7/fabric_virt_tools/numa_tune.py
--rw-r--r--   0        0        0     1559 2023-05-31 17:39:04.855580 fabric-virt-tools-1.0.0b7/fabric_virt_tools/utils.py
--rw-r--r--   0        0        0     3838 2023-05-31 19:48:41.435763 fabric-virt-tools-1.0.0b7/fabric_virt_tools/virt_tools_cli.py
--rw-r--r--   0        0        0      955 2023-05-31 21:04:53.032899 fabric-virt-tools-1.0.0b7/pyproject.toml
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 fabric-virt-tools-1.0.0b7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-31 18:44:31.383234 fabric-virt-tools-1.0.0b8/LICENSE
+-rw-r--r--   0        0        0      279 2023-05-31 18:44:17.271476 fabric-virt-tools-1.0.0b8/README.md
+-rw-r--r--   0        0        0       24 2023-06-01 14:26:36.764308 fabric-virt-tools-1.0.0b8/fabric_virt_tools/__init__.py
+-rw-r--r--   0        0        0     8127 2023-06-01 14:16:18.671031 fabric-virt-tools-1.0.0b8/fabric_virt_tools/cpu_tune.py
+-rw-r--r--   0        0        0     8485 2023-06-01 14:14:36.062000 fabric-virt-tools-1.0.0b8/fabric_virt_tools/cpu_tune_bkp.py
+-rw-r--r--   0        0        0    12229 2023-05-31 18:39:32.027641 fabric-virt-tools-1.0.0b8/fabric_virt_tools/numa_tune.py
+-rw-r--r--   0        0        0     1559 2023-05-31 17:39:04.855580 fabric-virt-tools-1.0.0b8/fabric_virt_tools/utils.py
+-rw-r--r--   0        0        0     3972 2023-06-01 14:21:14.282339 fabric-virt-tools-1.0.0b8/fabric_virt_tools/virt_tools_cli.py
+-rw-r--r--   0        0        0      955 2023-05-31 21:04:53.032899 fabric-virt-tools-1.0.0b8/pyproject.toml
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 fabric-virt-tools-1.0.0b8/PKG-INFO
```

### Comparing `fabric-virt-tools-1.0.0b7/LICENSE` & `fabric-virt-tools-1.0.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b7/fabric_virt_tools/cpu_tune.py` & `fabric-virt-tools-1.0.0b8/fabric_virt_tools/cpu_tune_bkp.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b7/fabric_virt_tools/numa_tune.py` & `fabric-virt-tools-1.0.0b8/fabric_virt_tools/numa_tune.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b7/fabric_virt_tools/utils.py` & `fabric-virt-tools-1.0.0b8/fabric_virt_tools/utils.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b7/fabric_virt_tools/virt_tools_cli.py` & `fabric-virt-tools-1.0.0b8/fabric_virt_tools/virt_tools_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,22 +62,24 @@
     except Exception as e:
         traceback.print_exc()
         raise click.ClickException(f"virt_tools_cli: {e}")
 
 
 @cpu.command()
 @click.option('--domain_name', help='Virtual Guest Domain Name', required=True)
-@click.option('--vcpu_cpu_map', help='Virtual CPU to Host Cpu Map', required=True)
+@click.option('--vcpu', help='Virtual CPU', required=True)
+@click.option('--cpu', help='Physical CPU', required=True)
 @click.pass_context
-def tune(ctx, domain_name: str, vcpu_cpu_map: List[Dict[str, str]]):
-    """ Query CPU Info for VM Guest and relevant host information as well
+def pin(ctx, domain_name: str, vcpu: str, cpu: str):
+    """ Pin vCPU to Host CPU
     """
     try:
         cpu_tune = CpuTune()
-        cpu_tune.vcpu_pin(domain_name=domain_name, vcpu_cpu_map=vcpu_cpu_map)
+        cpu_tune.vcpu_pin(domain_name=domain_name, vcpu=vcpu, cpu=cpu)
+        print(f"CPU pinning for {domain_name} for VCPU: {vcpu} to CPU {cpu} done!")
     except Exception as e:
         traceback.print_exc()
         raise click.ClickException(f"virt_tools_cli: {e}")
 
 
 @click.group()
 @click.pass_context
@@ -99,22 +101,23 @@
     except Exception as e:
         traceback.print_exc()
         raise click.ClickException(f"virt_tools_cli: {e}")
 
 
 @numa.command()
 @click.option('--domain_name', help='Virtual Guest Domain Name', required=True)
-@click.option('--node_set', help='List of the nodes to be assigned', required=True)
+@click.option('--node_set', help='List of the nodes to be assigned', required=True, multiple=True)
 @click.pass_context
 def tune(ctx, domain_name: str, node_set: List[str]):
     """ Pin Numa Node to the VM Guest
     """
     try:
         numa_tune = NumaTune()
         numa_tune.numa_tune(domain_name=domain_name, node_set=node_set)
+        print(f"Numa tuning for {domain_name} to {node_set} done!")
     except Exception as e:
         traceback.print_exc()
         raise click.ClickException(f"virt_tools_cli: {e}")
 
 
 virt_tools_cli.add_command(cpu)
 virt_tools_cli.add_command(numa)
```

### Comparing `fabric-virt-tools-1.0.0b7/pyproject.toml` & `fabric-virt-tools-1.0.0b8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b7/PKG-INFO` & `fabric-virt-tools-1.0.0b8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-virt-tools
-Version: 1.0.0b7
+Version: 1.0.0b8
 Summary: Fabric Virtual Machine Tools
 Keywords: Fabric Virtual Machine Tools
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

