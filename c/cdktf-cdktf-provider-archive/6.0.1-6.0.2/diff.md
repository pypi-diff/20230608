# Comparing `tmp/cdktf-cdktf-provider-archive-6.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-archive-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-archive-6.0.1.tar", last modified: Thu Jun  1 14:09:48 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-archive-6.0.2.tar", last modified: Thu Jun  8 03:15:29 2023, max compression
```

## Comparing `cdktf-cdktf-provider-archive-6.0.1.tar` & `cdktf-cdktf-provider-archive-6.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:48.007406 cdktf-cdktf-provider-archive-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:09:33.000000 cdktf-cdktf-provider-archive-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:09:33.000000 cdktf-cdktf-provider-archive-6.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-01 14:09:48.007406 cdktf-cdktf-provider-archive-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-01 14:09:33.000000 cdktf-cdktf-provider-archive-6.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:09:33.000000 cdktf-cdktf-provider-archive-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:09:48.007406 cdktf-cdktf-provider-archive-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-01 14:09:33.000000 cdktf-cdktf-provider-archive-6.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:48.003406 cdktf-cdktf-provider-archive-6.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:48.003406 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-01 14:09:33.000000 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:48.003406 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-01 14:09:33.000000 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40572 2023-06-01 14:09:33.000000 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/_jsii/provider-archive@6.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:48.007406 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/data_archive_file/
--rw-r--r--   0 runner    (1001) docker     (123)    53743 2023-06-01 14:09:33.000000 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/data_archive_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:48.007406 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/file/
--rw-r--r--   0 runner    (1001) docker     (123)    52790 2023-06-01 14:09:33.000000 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:48.007406 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-01 14:09:33.000000 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:09:33.000000 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:48.003406 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-01 14:09:47.000000 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-01 14:09:47.000000 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:09:47.000000 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:09:47.000000 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 14:09:47.000000 cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:15:29.022463 cdktf-cdktf-provider-archive-6.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-08 03:15:14.000000 cdktf-cdktf-provider-archive-6.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 03:15:14.000000 cdktf-cdktf-provider-archive-6.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-08 03:15:29.022463 cdktf-cdktf-provider-archive-6.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-08 03:15:14.000000 cdktf-cdktf-provider-archive-6.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-08 03:15:14.000000 cdktf-cdktf-provider-archive-6.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 03:15:29.022463 cdktf-cdktf-provider-archive-6.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-08 03:15:14.000000 cdktf-cdktf-provider-archive-6.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:15:29.018463 cdktf-cdktf-provider-archive-6.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:15:29.022463 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-08 03:15:14.000000 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:15:29.022463 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-08 03:15:14.000000 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44057 2023-06-08 03:15:14.000000 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/_jsii/provider-archive@6.0.2.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:15:29.022463 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/data_archive_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    58290 2023-06-08 03:15:14.000000 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/data_archive_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:15:29.022463 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/file/
+-rw-r--r--   0 runner    (1001) docker     (123)    57295 2023-06-08 03:15:14.000000 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:15:29.022463 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-08 03:15:14.000000 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 03:15:14.000000 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:15:29.022463 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-08 03:15:28.000000 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-08 03:15:28.000000 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 03:15:28.000000 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 03:15:28.000000 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 03:15:28.000000 cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-archive-6.0.1/LICENSE` & `cdktf-cdktf-provider-archive-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-archive-6.0.1/PKG-INFO` & `cdktf-cdktf-provider-archive-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-archive
-Version: 6.0.1
+Version: 6.0.2
 Summary: Prebuilt archive Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-archive.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-archive.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-archive-6.0.1/README.md` & `cdktf-cdktf-provider-archive-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-archive-6.0.1/setup.py` & `cdktf-cdktf-provider-archive-6.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-archive",
-    "version": "6.0.1",
+    "version": "6.0.2",
     "description": "Prebuilt archive Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-archive.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -25,25 +25,25 @@
         "cdktf_cdktf_provider_archive._jsii",
         "cdktf_cdktf_provider_archive.data_archive_file",
         "cdktf_cdktf_provider_archive.file",
         "cdktf_cdktf_provider_archive.provider"
     ],
     "package_data": {
         "cdktf_cdktf_provider_archive._jsii": [
-            "provider-archive@6.0.1.jsii.tgz"
+            "provider-archive@6.0.2.jsii.tgz"
         ],
         "cdktf_cdktf_provider_archive": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdktf>=0.16.3, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.81.0, <2.0.0",
+        "jsii>=1.83.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/__init__.py` & `cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/data_archive_file/__init__.py` & `cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/data_archive_file/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_archive_file`
 
-Refer to the Terraform Registory for docs: [`data_archive_file`](https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file).
+Refer to the Terraform Registory for docs: [`data_archive_file`](https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,51 +22,53 @@
 
 
 class DataArchiveFile(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-archive.dataArchiveFile.DataArchiveFile",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file archive_file}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file archive_file}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         output_path: builtins.str,
         type: builtins.str,
         excludes: typing.Optional[typing.Sequence[builtins.str]] = None,
+        exclude_symlink_directories: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         output_file_mode: typing.Optional[builtins.str] = None,
         source: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataArchiveFileSource", typing.Dict[builtins.str, typing.Any]]]]] = None,
         source_content: typing.Optional[builtins.str] = None,
         source_content_filename: typing.Optional[builtins.str] = None,
         source_dir: typing.Optional[builtins.str] = None,
         source_file: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file archive_file} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file archive_file} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#output_path DataArchiveFile#output_path}
-        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#type DataArchiveFile#type}
-        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#excludes DataArchiveFile#excludes}
-        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#output_file_mode DataArchiveFile#output_file_mode}
-        :param source: source block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source DataArchiveFile#source}
-        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_content DataArchiveFile#source_content}
-        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_content_filename DataArchiveFile#source_content_filename}
-        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_dir DataArchiveFile#source_dir}
-        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_file DataArchiveFile#source_file}
+        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#output_path DataArchiveFile#output_path}
+        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#type DataArchiveFile#type}
+        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#excludes DataArchiveFile#excludes}
+        :param exclude_symlink_directories: Boolean flag indicating whether symbolically linked directories should be excluded during the creation of the archive. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#exclude_symlink_directories DataArchiveFile#exclude_symlink_directories}
+        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#output_file_mode DataArchiveFile#output_file_mode}
+        :param source: source block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source DataArchiveFile#source}
+        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source_content DataArchiveFile#source_content}
+        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source_content_filename DataArchiveFile#source_content_filename}
+        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source_dir DataArchiveFile#source_dir}
+        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source_file DataArchiveFile#source_file}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -75,14 +77,15 @@
             type_hints = typing.get_type_hints(_typecheckingstub__3f8174f229f3604133f5c77a80cd25d2977aef1687fff32139249b73dce43cf7)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = DataArchiveFileConfig(
             output_path=output_path,
             type=type,
             excludes=excludes,
+            exclude_symlink_directories=exclude_symlink_directories,
             output_file_mode=output_file_mode,
             source=source,
             source_content=source_content,
             source_content_filename=source_content_filename,
             source_dir=source_dir,
             source_file=source_file,
             connection=connection,
@@ -109,14 +112,18 @@
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "putSource", [value]))
 
     @jsii.member(jsii_name="resetExcludes")
     def reset_excludes(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetExcludes", []))
 
+    @jsii.member(jsii_name="resetExcludeSymlinkDirectories")
+    def reset_exclude_symlink_directories(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetExcludeSymlinkDirectories", []))
+
     @jsii.member(jsii_name="resetOutputFileMode")
     def reset_output_file_mode(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetOutputFileMode", []))
 
     @jsii.member(jsii_name="resetSource")
     def reset_source(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetSource", []))
@@ -153,24 +160,39 @@
 
     @builtins.property
     @jsii.member(jsii_name="outputBase64Sha256")
     def output_base64_sha256(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "outputBase64Sha256"))
 
     @builtins.property
+    @jsii.member(jsii_name="outputBase64Sha512")
+    def output_base64_sha512(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "outputBase64Sha512"))
+
+    @builtins.property
     @jsii.member(jsii_name="outputMd5")
     def output_md5(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "outputMd5"))
 
     @builtins.property
     @jsii.member(jsii_name="outputSha")
     def output_sha(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "outputSha"))
 
     @builtins.property
+    @jsii.member(jsii_name="outputSha256")
+    def output_sha256(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "outputSha256"))
+
+    @builtins.property
+    @jsii.member(jsii_name="outputSha512")
+    def output_sha512(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "outputSha512"))
+
+    @builtins.property
     @jsii.member(jsii_name="outputSize")
     def output_size(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "outputSize"))
 
     @builtins.property
     @jsii.member(jsii_name="source")
     def source(self) -> "DataArchiveFileSourceList":
@@ -178,14 +200,21 @@
 
     @builtins.property
     @jsii.member(jsii_name="excludesInput")
     def excludes_input(self) -> typing.Optional[typing.List[builtins.str]]:
         return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "excludesInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="excludeSymlinkDirectoriesInput")
+    def exclude_symlink_directories_input(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "excludeSymlinkDirectoriesInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="outputFileModeInput")
     def output_file_mode_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "outputFileModeInput"))
 
     @builtins.property
     @jsii.member(jsii_name="outputPathInput")
     def output_path_input(self) -> typing.Optional[builtins.str]:
@@ -232,14 +261,31 @@
     def excludes(self, value: typing.List[builtins.str]) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__20c4285397b574ace2586d5b7d9c0efed97c37db7016848d04cb03aa64878453)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "excludes", value)
 
     @builtins.property
+    @jsii.member(jsii_name="excludeSymlinkDirectories")
+    def exclude_symlink_directories(
+        self,
+    ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
+        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "excludeSymlinkDirectories"))
+
+    @exclude_symlink_directories.setter
+    def exclude_symlink_directories(
+        self,
+        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__63461d561599bf3138af7b713358f4ca8a37731df554faa092adba7988d201e6)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "excludeSymlinkDirectories", value)
+
+    @builtins.property
     @jsii.member(jsii_name="outputFileMode")
     def output_file_mode(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "outputFileMode"))
 
     @output_file_mode.setter
     def output_file_mode(self, value: builtins.str) -> None:
         if __debug__:
@@ -330,14 +376,15 @@
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "output_path": "outputPath",
         "type": "type",
         "excludes": "excludes",
+        "exclude_symlink_directories": "excludeSymlinkDirectories",
         "output_file_mode": "outputFileMode",
         "source": "source",
         "source_content": "sourceContent",
         "source_content_filename": "sourceContentFilename",
         "source_dir": "sourceDir",
         "source_file": "sourceFile",
     },
@@ -352,14 +399,15 @@
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         output_path: builtins.str,
         type: builtins.str,
         excludes: typing.Optional[typing.Sequence[builtins.str]] = None,
+        exclude_symlink_directories: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         output_file_mode: typing.Optional[builtins.str] = None,
         source: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataArchiveFileSource", typing.Dict[builtins.str, typing.Any]]]]] = None,
         source_content: typing.Optional[builtins.str] = None,
         source_content_filename: typing.Optional[builtins.str] = None,
         source_dir: typing.Optional[builtins.str] = None,
         source_file: typing.Optional[builtins.str] = None,
     ) -> None:
@@ -367,23 +415,24 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#output_path DataArchiveFile#output_path}
-        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#type DataArchiveFile#type}
-        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#excludes DataArchiveFile#excludes}
-        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#output_file_mode DataArchiveFile#output_file_mode}
-        :param source: source block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source DataArchiveFile#source}
-        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_content DataArchiveFile#source_content}
-        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_content_filename DataArchiveFile#source_content_filename}
-        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_dir DataArchiveFile#source_dir}
-        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_file DataArchiveFile#source_file}
+        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#output_path DataArchiveFile#output_path}
+        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#type DataArchiveFile#type}
+        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#excludes DataArchiveFile#excludes}
+        :param exclude_symlink_directories: Boolean flag indicating whether symbolically linked directories should be excluded during the creation of the archive. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#exclude_symlink_directories DataArchiveFile#exclude_symlink_directories}
+        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#output_file_mode DataArchiveFile#output_file_mode}
+        :param source: source block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source DataArchiveFile#source}
+        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source_content DataArchiveFile#source_content}
+        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source_content_filename DataArchiveFile#source_content_filename}
+        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source_dir DataArchiveFile#source_dir}
+        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source_file DataArchiveFile#source_file}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__395d6c956a8f6a157e1bf9db0b880a72f8d80755220480442d2acbff968ca74f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -391,14 +440,15 @@
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument output_path", value=output_path, expected_type=type_hints["output_path"])
             check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             check_type(argname="argument excludes", value=excludes, expected_type=type_hints["excludes"])
+            check_type(argname="argument exclude_symlink_directories", value=exclude_symlink_directories, expected_type=type_hints["exclude_symlink_directories"])
             check_type(argname="argument output_file_mode", value=output_file_mode, expected_type=type_hints["output_file_mode"])
             check_type(argname="argument source", value=source, expected_type=type_hints["source"])
             check_type(argname="argument source_content", value=source_content, expected_type=type_hints["source_content"])
             check_type(argname="argument source_content_filename", value=source_content_filename, expected_type=type_hints["source_content_filename"])
             check_type(argname="argument source_dir", value=source_dir, expected_type=type_hints["source_dir"])
             check_type(argname="argument source_file", value=source_file, expected_type=type_hints["source_file"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -417,14 +467,16 @@
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
         if excludes is not None:
             self._values["excludes"] = excludes
+        if exclude_symlink_directories is not None:
+            self._values["exclude_symlink_directories"] = exclude_symlink_directories
         if output_file_mode is not None:
             self._values["output_file_mode"] = output_file_mode
         if source is not None:
             self._values["source"] = source
         if source_content is not None:
             self._values["source_content"] = source_content
         if source_content_filename is not None:
@@ -498,101 +550,112 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def output_path(self) -> builtins.str:
         '''The output of the archive file.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#output_path DataArchiveFile#output_path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#output_path DataArchiveFile#output_path}
         '''
         result = self._values.get("output_path")
         assert result is not None, "Required property 'output_path' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The type of archive to generate. NOTE: ``zip`` is supported.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#type DataArchiveFile#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#type DataArchiveFile#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def excludes(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Specify files to ignore when reading the ``source_dir``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#excludes DataArchiveFile#excludes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#excludes DataArchiveFile#excludes}
         '''
         result = self._values.get("excludes")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
+    def exclude_symlink_directories(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        '''Boolean flag indicating whether symbolically linked directories should be excluded during the creation of the archive. Defaults to false.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#exclude_symlink_directories DataArchiveFile#exclude_symlink_directories}
+        '''
+        result = self._values.get("exclude_symlink_directories")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
+
+    @builtins.property
     def output_file_mode(self) -> typing.Optional[builtins.str]:
         '''String that specifies the octal file mode for all archived files.
 
         For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#output_file_mode DataArchiveFile#output_file_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#output_file_mode DataArchiveFile#output_file_mode}
         '''
         result = self._values.get("output_file_mode")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataArchiveFileSource"]]]:
         '''source block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source DataArchiveFile#source}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source DataArchiveFile#source}
         '''
         result = self._values.get("source")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataArchiveFileSource"]]], result)
 
     @builtins.property
     def source_content(self) -> typing.Optional[builtins.str]:
         '''Add only this content to the archive with ``source_content_filename`` as the filename.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_content DataArchiveFile#source_content}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source_content DataArchiveFile#source_content}
         '''
         result = self._values.get("source_content")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_content_filename(self) -> typing.Optional[builtins.str]:
         '''Set this as the filename when using ``source_content``.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_content_filename DataArchiveFile#source_content_filename}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source_content_filename DataArchiveFile#source_content_filename}
         '''
         result = self._values.get("source_content_filename")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_dir(self) -> typing.Optional[builtins.str]:
         '''Package entire contents of this directory into the archive.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_dir DataArchiveFile#source_dir}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source_dir DataArchiveFile#source_dir}
         '''
         result = self._values.get("source_dir")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_file(self) -> typing.Optional[builtins.str]:
         '''Package this file into the archive.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#source_file DataArchiveFile#source_file}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#source_file DataArchiveFile#source_file}
         '''
         result = self._values.get("source_file")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -609,41 +672,41 @@
     jsii_type="@cdktf/provider-archive.dataArchiveFile.DataArchiveFileSource",
     jsii_struct_bases=[],
     name_mapping={"content": "content", "filename": "filename"},
 )
 class DataArchiveFileSource:
     def __init__(self, *, content: builtins.str, filename: builtins.str) -> None:
         '''
-        :param content: Add this content to the archive with ``filename`` as the filename. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#content DataArchiveFile#content}
-        :param filename: Set this as the filename when declaring a ``source``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#filename DataArchiveFile#filename}
+        :param content: Add this content to the archive with ``filename`` as the filename. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#content DataArchiveFile#content}
+        :param filename: Set this as the filename when declaring a ``source``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#filename DataArchiveFile#filename}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5904c5461679cf6f1f619fb8bf2ab9cf44afa5adb738fa7a85022f5f3df3fa5b)
             check_type(argname="argument content", value=content, expected_type=type_hints["content"])
             check_type(argname="argument filename", value=filename, expected_type=type_hints["filename"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "content": content,
             "filename": filename,
         }
 
     @builtins.property
     def content(self) -> builtins.str:
         '''Add this content to the archive with ``filename`` as the filename.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#content DataArchiveFile#content}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#content DataArchiveFile#content}
         '''
         result = self._values.get("content")
         assert result is not None, "Required property 'content' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def filename(self) -> builtins.str:
         '''Set this as the filename when declaring a ``source``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/data-sources/file#filename DataArchiveFile#filename}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/data-sources/file#filename DataArchiveFile#filename}
         '''
         result = self._values.get("filename")
         assert result is not None, "Required property 'filename' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -838,14 +901,15 @@
 def _typecheckingstub__3f8174f229f3604133f5c77a80cd25d2977aef1687fff32139249b73dce43cf7(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     output_path: builtins.str,
     type: builtins.str,
     excludes: typing.Optional[typing.Sequence[builtins.str]] = None,
+    exclude_symlink_directories: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     output_file_mode: typing.Optional[builtins.str] = None,
     source: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataArchiveFileSource, typing.Dict[builtins.str, typing.Any]]]]] = None,
     source_content: typing.Optional[builtins.str] = None,
     source_content_filename: typing.Optional[builtins.str] = None,
     source_dir: typing.Optional[builtins.str] = None,
     source_file: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
@@ -867,14 +931,20 @@
 
 def _typecheckingstub__20c4285397b574ace2586d5b7d9c0efed97c37db7016848d04cb03aa64878453(
     value: typing.List[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__63461d561599bf3138af7b713358f4ca8a37731df554faa092adba7988d201e6(
+    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__5cf0d3fbf6707bec587f4a960cd54edd8e60f917d78b8b942cc183e29c7291d2(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__3592643f4a565fac9e7ff8c5189ac2f818943f620f705989325f0070d0f74749(
@@ -921,14 +991,15 @@
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     output_path: builtins.str,
     type: builtins.str,
     excludes: typing.Optional[typing.Sequence[builtins.str]] = None,
+    exclude_symlink_directories: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     output_file_mode: typing.Optional[builtins.str] = None,
     source: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataArchiveFileSource, typing.Dict[builtins.str, typing.Any]]]]] = None,
     source_content: typing.Optional[builtins.str] = None,
     source_content_filename: typing.Optional[builtins.str] = None,
     source_dir: typing.Optional[builtins.str] = None,
     source_file: typing.Optional[builtins.str] = None,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/file/__init__.py` & `cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/file/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `archive_file`
 
-Refer to the Terraform Registory for docs: [`archive_file`](https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file).
+Refer to the Terraform Registory for docs: [`archive_file`](https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,51 +22,53 @@
 
 
 class File(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-archive.file.File",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file archive_file}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file archive_file}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         output_path: builtins.str,
         type: builtins.str,
         excludes: typing.Optional[typing.Sequence[builtins.str]] = None,
+        exclude_symlink_directories: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         output_file_mode: typing.Optional[builtins.str] = None,
-        source: typing.Optional[typing.Union[typing.Sequence[typing.Union["FileSource", typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable]] = None,
+        source: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["FileSource", typing.Dict[builtins.str, typing.Any]]]]] = None,
         source_content: typing.Optional[builtins.str] = None,
         source_content_filename: typing.Optional[builtins.str] = None,
         source_dir: typing.Optional[builtins.str] = None,
         source_file: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file archive_file} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file archive_file} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#output_path File#output_path}
-        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#type File#type}
-        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#excludes File#excludes}
-        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#output_file_mode File#output_file_mode}
-        :param source: source block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source File#source}
-        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_content File#source_content}
-        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_content_filename File#source_content_filename}
-        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_dir File#source_dir}
-        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_file File#source_file}
+        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#output_path File#output_path}
+        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#type File#type}
+        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#excludes File#excludes}
+        :param exclude_symlink_directories: Boolean flag indicating whether symbolically linked directories should be excluded during the creation of the archive. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#exclude_symlink_directories File#exclude_symlink_directories}
+        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#output_file_mode File#output_file_mode}
+        :param source: source block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source File#source}
+        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source_content File#source_content}
+        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source_content_filename File#source_content_filename}
+        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source_dir File#source_dir}
+        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source_file File#source_file}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -75,14 +77,15 @@
             type_hints = typing.get_type_hints(_typecheckingstub__ffa9a1e310e0fed84f9ce7cadd39e4c006e02fc1451a79fc6f283c6e1f9bd7c1)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = FileConfig(
             output_path=output_path,
             type=type,
             excludes=excludes,
+            exclude_symlink_directories=exclude_symlink_directories,
             output_file_mode=output_file_mode,
             source=source,
             source_content=source_content,
             source_content_filename=source_content_filename,
             source_dir=source_dir,
             source_file=source_file,
             connection=connection,
@@ -95,28 +98,32 @@
         )
 
         jsii.create(self.__class__, self, [scope, id, config])
 
     @jsii.member(jsii_name="putSource")
     def put_source(
         self,
-        value: typing.Union[typing.Sequence[typing.Union["FileSource", typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
+        value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["FileSource", typing.Dict[builtins.str, typing.Any]]]],
     ) -> None:
         '''
         :param value: -
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a50c420f409a76db13cab937bd8f16a960a6716abc4dbd523bbb8b76ec1df579)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "putSource", [value]))
 
     @jsii.member(jsii_name="resetExcludes")
     def reset_excludes(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetExcludes", []))
 
+    @jsii.member(jsii_name="resetExcludeSymlinkDirectories")
+    def reset_exclude_symlink_directories(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetExcludeSymlinkDirectories", []))
+
     @jsii.member(jsii_name="resetOutputFileMode")
     def reset_output_file_mode(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetOutputFileMode", []))
 
     @jsii.member(jsii_name="resetSource")
     def reset_source(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetSource", []))
@@ -153,24 +160,39 @@
 
     @builtins.property
     @jsii.member(jsii_name="outputBase64Sha256")
     def output_base64_sha256(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "outputBase64Sha256"))
 
     @builtins.property
+    @jsii.member(jsii_name="outputBase64Sha512")
+    def output_base64_sha512(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "outputBase64Sha512"))
+
+    @builtins.property
     @jsii.member(jsii_name="outputMd5")
     def output_md5(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "outputMd5"))
 
     @builtins.property
     @jsii.member(jsii_name="outputSha")
     def output_sha(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "outputSha"))
 
     @builtins.property
+    @jsii.member(jsii_name="outputSha256")
+    def output_sha256(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "outputSha256"))
+
+    @builtins.property
+    @jsii.member(jsii_name="outputSha512")
+    def output_sha512(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "outputSha512"))
+
+    @builtins.property
     @jsii.member(jsii_name="outputSize")
     def output_size(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "outputSize"))
 
     @builtins.property
     @jsii.member(jsii_name="source")
     def source(self) -> "FileSourceList":
@@ -178,14 +200,21 @@
 
     @builtins.property
     @jsii.member(jsii_name="excludesInput")
     def excludes_input(self) -> typing.Optional[typing.List[builtins.str]]:
         return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "excludesInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="excludeSymlinkDirectoriesInput")
+    def exclude_symlink_directories_input(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "excludeSymlinkDirectoriesInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="outputFileModeInput")
     def output_file_mode_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "outputFileModeInput"))
 
     @builtins.property
     @jsii.member(jsii_name="outputPathInput")
     def output_path_input(self) -> typing.Optional[builtins.str]:
@@ -211,16 +240,16 @@
     def source_file_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "sourceFileInput"))
 
     @builtins.property
     @jsii.member(jsii_name="sourceInput")
     def source_input(
         self,
-    ) -> typing.Optional[typing.Union[typing.List["FileSource"], _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[typing.List["FileSource"], _cdktf_9a9027ec.IResolvable]], jsii.get(self, "sourceInput"))
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FileSource"]]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FileSource"]]], jsii.get(self, "sourceInput"))
 
     @builtins.property
     @jsii.member(jsii_name="typeInput")
     def type_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "typeInput"))
 
     @builtins.property
@@ -232,14 +261,31 @@
     def excludes(self, value: typing.List[builtins.str]) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7797e5908778c373a4181c51cf5bc07966c3d6d42e2c81354904354c289b140d)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "excludes", value)
 
     @builtins.property
+    @jsii.member(jsii_name="excludeSymlinkDirectories")
+    def exclude_symlink_directories(
+        self,
+    ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
+        return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], jsii.get(self, "excludeSymlinkDirectories"))
+
+    @exclude_symlink_directories.setter
+    def exclude_symlink_directories(
+        self,
+        value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ec6358dfba6df53628e9b10b8e43331763b8b0e69bf1de2903c39cc6f40fa1de)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "excludeSymlinkDirectories", value)
+
+    @builtins.property
     @jsii.member(jsii_name="outputFileMode")
     def output_file_mode(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "outputFileMode"))
 
     @output_file_mode.setter
     def output_file_mode(self, value: builtins.str) -> None:
         if __debug__:
@@ -330,14 +376,15 @@
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "output_path": "outputPath",
         "type": "type",
         "excludes": "excludes",
+        "exclude_symlink_directories": "excludeSymlinkDirectories",
         "output_file_mode": "outputFileMode",
         "source": "source",
         "source_content": "sourceContent",
         "source_content_filename": "sourceContentFilename",
         "source_dir": "sourceDir",
         "source_file": "sourceFile",
     },
@@ -352,38 +399,40 @@
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         output_path: builtins.str,
         type: builtins.str,
         excludes: typing.Optional[typing.Sequence[builtins.str]] = None,
+        exclude_symlink_directories: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         output_file_mode: typing.Optional[builtins.str] = None,
-        source: typing.Optional[typing.Union[typing.Sequence[typing.Union["FileSource", typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable]] = None,
+        source: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["FileSource", typing.Dict[builtins.str, typing.Any]]]]] = None,
         source_content: typing.Optional[builtins.str] = None,
         source_content_filename: typing.Optional[builtins.str] = None,
         source_dir: typing.Optional[builtins.str] = None,
         source_file: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#output_path File#output_path}
-        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#type File#type}
-        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#excludes File#excludes}
-        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#output_file_mode File#output_file_mode}
-        :param source: source block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source File#source}
-        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_content File#source_content}
-        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_content_filename File#source_content_filename}
-        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_dir File#source_dir}
-        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_file File#source_file}
+        :param output_path: The output of the archive file. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#output_path File#output_path}
+        :param type: The type of archive to generate. NOTE: ``zip`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#type File#type}
+        :param excludes: Specify files to ignore when reading the ``source_dir``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#excludes File#excludes}
+        :param exclude_symlink_directories: Boolean flag indicating whether symbolically linked directories should be excluded during the creation of the archive. Defaults to false. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#exclude_symlink_directories File#exclude_symlink_directories}
+        :param output_file_mode: String that specifies the octal file mode for all archived files. For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#output_file_mode File#output_file_mode}
+        :param source: source block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source File#source}
+        :param source_content: Add only this content to the archive with ``source_content_filename`` as the filename. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source_content File#source_content}
+        :param source_content_filename: Set this as the filename when using ``source_content``. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source_content_filename File#source_content_filename}
+        :param source_dir: Package entire contents of this directory into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source_dir File#source_dir}
+        :param source_file: Package this file into the archive. One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source_file File#source_file}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4cf416deaa089a02b7fc630d948296d45144383aef1cde25d0742ca6c4454dd4)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -391,14 +440,15 @@
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument output_path", value=output_path, expected_type=type_hints["output_path"])
             check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             check_type(argname="argument excludes", value=excludes, expected_type=type_hints["excludes"])
+            check_type(argname="argument exclude_symlink_directories", value=exclude_symlink_directories, expected_type=type_hints["exclude_symlink_directories"])
             check_type(argname="argument output_file_mode", value=output_file_mode, expected_type=type_hints["output_file_mode"])
             check_type(argname="argument source", value=source, expected_type=type_hints["source"])
             check_type(argname="argument source_content", value=source_content, expected_type=type_hints["source_content"])
             check_type(argname="argument source_content_filename", value=source_content_filename, expected_type=type_hints["source_content_filename"])
             check_type(argname="argument source_dir", value=source_dir, expected_type=type_hints["source_dir"])
             check_type(argname="argument source_file", value=source_file, expected_type=type_hints["source_file"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -417,14 +467,16 @@
             self._values["lifecycle"] = lifecycle
         if provider is not None:
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
         if excludes is not None:
             self._values["excludes"] = excludes
+        if exclude_symlink_directories is not None:
+            self._values["exclude_symlink_directories"] = exclude_symlink_directories
         if output_file_mode is not None:
             self._values["output_file_mode"] = output_file_mode
         if source is not None:
             self._values["source"] = source
         if source_content is not None:
             self._values["source_content"] = source_content
         if source_content_filename is not None:
@@ -498,101 +550,112 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def output_path(self) -> builtins.str:
         '''The output of the archive file.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#output_path File#output_path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#output_path File#output_path}
         '''
         result = self._values.get("output_path")
         assert result is not None, "Required property 'output_path' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The type of archive to generate. NOTE: ``zip`` is supported.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#type File#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#type File#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def excludes(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Specify files to ignore when reading the ``source_dir``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#excludes File#excludes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#excludes File#excludes}
         '''
         result = self._values.get("excludes")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
+    def exclude_symlink_directories(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
+        '''Boolean flag indicating whether symbolically linked directories should be excluded during the creation of the archive. Defaults to false.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#exclude_symlink_directories File#exclude_symlink_directories}
+        '''
+        result = self._values.get("exclude_symlink_directories")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
+
+    @builtins.property
     def output_file_mode(self) -> typing.Optional[builtins.str]:
         '''String that specifies the octal file mode for all archived files.
 
         For example: ``"0666"``. Setting this will ensure that cross platform usage of this module will not vary the modes of archived files (and ultimately checksums) resulting in more deterministic behavior.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#output_file_mode File#output_file_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#output_file_mode File#output_file_mode}
         '''
         result = self._values.get("output_file_mode")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source(
         self,
-    ) -> typing.Optional[typing.Union[typing.List["FileSource"], _cdktf_9a9027ec.IResolvable]]:
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FileSource"]]]:
         '''source block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source File#source}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source File#source}
         '''
         result = self._values.get("source")
-        return typing.cast(typing.Optional[typing.Union[typing.List["FileSource"], _cdktf_9a9027ec.IResolvable]], result)
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FileSource"]]], result)
 
     @builtins.property
     def source_content(self) -> typing.Optional[builtins.str]:
         '''Add only this content to the archive with ``source_content_filename`` as the filename.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_content File#source_content}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source_content File#source_content}
         '''
         result = self._values.get("source_content")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_content_filename(self) -> typing.Optional[builtins.str]:
         '''Set this as the filename when using ``source_content``.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_content_filename File#source_content_filename}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source_content_filename File#source_content_filename}
         '''
         result = self._values.get("source_content_filename")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_dir(self) -> typing.Optional[builtins.str]:
         '''Package entire contents of this directory into the archive.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_dir File#source_dir}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source_dir File#source_dir}
         '''
         result = self._values.get("source_dir")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_file(self) -> typing.Optional[builtins.str]:
         '''Package this file into the archive.
 
         One and only one of ``source``, ``source_content_filename`` (with ``source_content``), ``source_file``, or ``source_dir`` must be specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#source_file File#source_file}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#source_file File#source_file}
         '''
         result = self._values.get("source_file")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -609,41 +672,41 @@
     jsii_type="@cdktf/provider-archive.file.FileSource",
     jsii_struct_bases=[],
     name_mapping={"content": "content", "filename": "filename"},
 )
 class FileSource:
     def __init__(self, *, content: builtins.str, filename: builtins.str) -> None:
         '''
-        :param content: Add this content to the archive with ``filename`` as the filename. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#content File#content}
-        :param filename: Set this as the filename when declaring a ``source``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#filename File#filename}
+        :param content: Add this content to the archive with ``filename`` as the filename. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#content File#content}
+        :param filename: Set this as the filename when declaring a ``source``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#filename File#filename}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b11194e55a06bbf9bdba900600d77ae8dc999b8147683c454f2452321f3945f3)
             check_type(argname="argument content", value=content, expected_type=type_hints["content"])
             check_type(argname="argument filename", value=filename, expected_type=type_hints["filename"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "content": content,
             "filename": filename,
         }
 
     @builtins.property
     def content(self) -> builtins.str:
         '''Add this content to the archive with ``filename`` as the filename.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#content File#content}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#content File#content}
         '''
         result = self._values.get("content")
         assert result is not None, "Required property 'content' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def filename(self) -> builtins.str:
         '''Set this as the filename when declaring a ``source``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs/resources/file#filename File#filename}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs/resources/file#filename File#filename}
         '''
         result = self._values.get("filename")
         assert result is not None, "Required property 'filename' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -729,21 +792,21 @@
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wrapsSet", value)
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[typing.Union[typing.List[FileSource], _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[typing.List[FileSource], _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[FileSource]]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[FileSource]]], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[typing.Union[typing.List[FileSource], _cdktf_9a9027ec.IResolvable]],
+        value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[FileSource]]],
     ) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__63dc9e7bd3b8e8b0a0c8634914d15010d2e2cfaab364a3bc4de880d005ea84c2)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
@@ -838,16 +901,17 @@
 def _typecheckingstub__ffa9a1e310e0fed84f9ce7cadd39e4c006e02fc1451a79fc6f283c6e1f9bd7c1(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     output_path: builtins.str,
     type: builtins.str,
     excludes: typing.Optional[typing.Sequence[builtins.str]] = None,
+    exclude_symlink_directories: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     output_file_mode: typing.Optional[builtins.str] = None,
-    source: typing.Optional[typing.Union[typing.Sequence[typing.Union[FileSource, typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable]] = None,
+    source: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[FileSource, typing.Dict[builtins.str, typing.Any]]]]] = None,
     source_content: typing.Optional[builtins.str] = None,
     source_content_filename: typing.Optional[builtins.str] = None,
     source_dir: typing.Optional[builtins.str] = None,
     source_file: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
@@ -856,25 +920,31 @@
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__a50c420f409a76db13cab937bd8f16a960a6716abc4dbd523bbb8b76ec1df579(
-    value: typing.Union[typing.Sequence[typing.Union[FileSource, typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable],
+    value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[FileSource, typing.Dict[builtins.str, typing.Any]]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__7797e5908778c373a4181c51cf5bc07966c3d6d42e2c81354904354c289b140d(
     value: typing.List[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__ec6358dfba6df53628e9b10b8e43331763b8b0e69bf1de2903c39cc6f40fa1de(
+    value: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__79807569b50d474ed25e61d3183471ceccafe0ac9a335d23e8029877e20d5b8e(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__8b96d34815e85a1bca3a705cde1b0b5ebf49ddc55fd930c516553cd449b41c00(
@@ -921,16 +991,17 @@
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     output_path: builtins.str,
     type: builtins.str,
     excludes: typing.Optional[typing.Sequence[builtins.str]] = None,
+    exclude_symlink_directories: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     output_file_mode: typing.Optional[builtins.str] = None,
-    source: typing.Optional[typing.Union[typing.Sequence[typing.Union[FileSource, typing.Dict[builtins.str, typing.Any]]], _cdktf_9a9027ec.IResolvable]] = None,
+    source: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[FileSource, typing.Dict[builtins.str, typing.Any]]]]] = None,
     source_content: typing.Optional[builtins.str] = None,
     source_content_filename: typing.Optional[builtins.str] = None,
     source_dir: typing.Optional[builtins.str] = None,
     source_file: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
@@ -972,15 +1043,15 @@
 def _typecheckingstub__054ee919fefa8e8d55d5535984746684f261fde847ee427f26d3284cfc14f309(
     value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__63dc9e7bd3b8e8b0a0c8634914d15010d2e2cfaab364a3bc4de880d005ea84c2(
-    value: typing.Optional[typing.Union[typing.List[FileSource], _cdktf_9a9027ec.IResolvable]],
+    value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[FileSource]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__53122ab2bbcfabc5e5e696a74bf00cc9c8ec91e86193cf0c6c3f5bcf03cd99af(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
```

### Comparing `cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive/provider/__init__.py` & `cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive/provider/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`archive`](https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs).
+Refer to the Terraform Registory for docs: [`archive`](https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,28 +22,28 @@
 
 
 class ArchiveProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-archive.provider.ArchiveProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs archive}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs archive}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs archive} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs archive} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs#alias ArchiveProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs#alias ArchiveProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9334d8ee2bfd48a0b6bd3d2efceb54053666d2fefddaec92ffc4d091954d4b64)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = ArchiveProviderConfig(alias=alias)
 
@@ -84,28 +84,28 @@
     jsii_type="@cdktf/provider-archive.provider.ArchiveProviderConfig",
     jsii_struct_bases=[],
     name_mapping={"alias": "alias"},
 )
 class ArchiveProviderConfig:
     def __init__(self, *, alias: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs#alias ArchiveProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs#alias ArchiveProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3c55b33d0d45082b5aaf9d9b53d8c0dbe974d4f669c09696067c98d7276df49b)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if alias is not None:
             self._values["alias"] = alias
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.3.0/docs#alias ArchiveProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/archive/2.4.0/docs#alias ArchiveProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive.egg-info/PKG-INFO` & `cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-archive
-Version: 6.0.1
+Version: 6.0.2
 Summary: Prebuilt archive Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-archive.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-archive.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-archive-6.0.1/src/cdktf_cdktf_provider_archive.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-archive-6.0.2/src/cdktf_cdktf_provider_archive.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 src/cdktf_cdktf_provider_archive/py.typed
 src/cdktf_cdktf_provider_archive.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_archive.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_archive.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_archive.egg-info/requires.txt
 src/cdktf_cdktf_provider_archive.egg-info/top_level.txt
 src/cdktf_cdktf_provider_archive/_jsii/__init__.py
-src/cdktf_cdktf_provider_archive/_jsii/provider-archive@6.0.1.jsii.tgz
+src/cdktf_cdktf_provider_archive/_jsii/provider-archive@6.0.2.jsii.tgz
 src/cdktf_cdktf_provider_archive/data_archive_file/__init__.py
 src/cdktf_cdktf_provider_archive/file/__init__.py
 src/cdktf_cdktf_provider_archive/provider/__init__.py
```

