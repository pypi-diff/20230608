# Comparing `tmp/kodexa_cli-6.2.25163504424.tar.gz` & `tmp/kodexa_cli-6.2.25203804340.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa_cli-6.2.25163504424.tar", max compression
+gzip compressed data, was "kodexa_cli-6.2.25203804340.tar", max compression
```

## Comparing `kodexa_cli-6.2.25163504424.tar` & `kodexa_cli-6.2.25203804340.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/LICENSE
--rw-r--r--   0        0        0     2707 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/README.md
--rw-r--r--   0        0        0       64 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/__init__.py
--rw-r--r--   0        0        0    26764 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/cli.py
--rw-r--r--   0        0        0     7641 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/documentation.py
--rw-r--r--   0        0        0      134 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/action.jinja2
--rw-r--r--   0        0        0     1356 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/assistant.jinja2
--rw-r--r--   0        0        0     1021 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/content-taxon.jinja2
--rw-r--r--   0        0        0      328 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/data-store.jinja2
--rw-r--r--   0        0        0      707 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/document-store.jinja2
--rw-r--r--   0        0        0       30 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/extension-pack.jinja2
--rw-r--r--   0        0        0      818 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/header.jinja2
--rw-r--r--   0        0        0      343 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/index.jinja2
--rw-r--r--   0        0        0       30 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/model-runtime.jinja2
--rw-r--r--   0        0        0     2999 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/model.jinja2
--rw-r--r--   0        0        0     1137 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/options.jinja2
--rw-r--r--   0        0        0        0 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/overview.jinja2
--rw-r--r--   0        0        0      922 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/processing-taxon.jinja2
--rw-r--r--   0        0        0       30 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/project-template.jinja2
--rw-r--r--   0        0        0       30 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/store.jinja2
--rw-r--r--   0        0        0      492 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/taxon.jinja2
--rw-r--r--   0        0        0      273 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/taxonomy-labels.jinja2
--rw-r--r--   0        0        0      534 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/taxonomy-structure.jinja2
--rw-r--r--   0        0        0      269 2023-06-03 11:55:22.936837 kodexa_cli-6.2.25163504424/kodexa_cli/templates/taxonomy.jinja2
--rw-r--r--   0        0        0      780 2023-06-03 11:55:38.944747 kodexa_cli-6.2.25163504424/pyproject.toml
--rw-r--r--   0        0        0     3665 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25163504424/setup.py
--rw-r--r--   0        0        0     3389 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25163504424/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/LICENSE
+-rw-r--r--   0        0        0     2707 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/README.md
+-rw-r--r--   0        0        0       64 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/__init__.py
+-rw-r--r--   0        0        0    26567 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/cli.py
+-rw-r--r--   0        0        0     7641 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/documentation.py
+-rw-r--r--   0        0        0      134 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/action.jinja2
+-rw-r--r--   0        0        0     1356 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/assistant.jinja2
+-rw-r--r--   0        0        0     1021 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/content-taxon.jinja2
+-rw-r--r--   0        0        0      328 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/data-store.jinja2
+-rw-r--r--   0        0        0      707 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/document-store.jinja2
+-rw-r--r--   0        0        0       30 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/extension-pack.jinja2
+-rw-r--r--   0        0        0      818 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/header.jinja2
+-rw-r--r--   0        0        0      343 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/index.jinja2
+-rw-r--r--   0        0        0       30 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/model-runtime.jinja2
+-rw-r--r--   0        0        0     2999 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/model.jinja2
+-rw-r--r--   0        0        0     1137 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/options.jinja2
+-rw-r--r--   0        0        0        0 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/overview.jinja2
+-rw-r--r--   0        0        0      922 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/processing-taxon.jinja2
+-rw-r--r--   0        0        0       30 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/project-template.jinja2
+-rw-r--r--   0        0        0       30 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/store.jinja2
+-rw-r--r--   0        0        0      492 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/taxon.jinja2
+-rw-r--r--   0        0        0      273 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/taxonomy-labels.jinja2
+-rw-r--r--   0        0        0      534 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/taxonomy-structure.jinja2
+-rw-r--r--   0        0        0      269 2023-06-07 19:09:00.590309 kodexa_cli-6.2.25203804340/kodexa_cli/templates/taxonomy.jinja2
+-rw-r--r--   0        0        0      780 2023-06-07 19:09:15.362355 kodexa_cli-6.2.25203804340/pyproject.toml
+-rw-r--r--   0        0        0     3665 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25203804340/setup.py
+-rw-r--r--   0        0        0     3389 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25203804340/PKG-INFO
```

### Comparing `kodexa_cli-6.2.25163504424/LICENSE` & `kodexa_cli-6.2.25203804340/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25163504424/README.md` & `kodexa_cli-6.2.25203804340/README.md`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25163504424/kodexa_cli/cli.py` & `kodexa_cli-6.2.25203804340/kodexa_cli/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from shutil import copyfile
 
 import click
 import wrapt
 import yaml
 from functional import seq
 from kodexa.model import ModelContentMetadata
-from kodexa.platform.client import DEFAULT_COLUMNS, ModelStoreEndpoint
+from kodexa.platform.client import ModelStoreEndpoint
 from rich import print
 
 logging.root.addHandler(logging.StreamHandler(sys.stdout))
 
 from kodexa import KodexaClient
 from kodexa.platform.kodexa import KodexaPlatform
 
@@ -34,14 +34,64 @@
     0: logging.NOTSET,
     1: logging.ERROR,
     2: logging.WARN,
     3: logging.INFO,
     4: logging.DEBUG,
 }  #: a mapping of `verbose` option counts to logging levels
 
+DEFAULT_COLUMNS = {
+    'extensionPacks': [
+        'ref',
+        'name',
+        'description',
+        'type',
+        'status'
+    ],
+    'projects': [
+        'id',
+        'organization.name',
+        'name',
+        'description'
+    ],
+    'assistants': [
+        'ref',
+        'name',
+        'description',
+        'template'
+    ],
+    'executions': [
+        'id',
+        'startDate',
+        'endDate',
+        'status',
+        'assistant.name',
+        'documentFamily.path'
+    ],
+    'memberships': [
+        'organization.slug',
+        'organization.name'
+    ],
+
+    'stores': [
+        'ref',
+        'name',
+        'description',
+        'store_type',
+        'store_purpose',
+        'template'
+    ],
+    'default': [
+        'ref',
+        'name',
+        'description',
+        'type',
+        'template'
+    ]
+}
+
 
 class Info(object):
     """An information object to pass data between CLI functions."""
 
     def __init__(self):  # Note: This object must have an empty constructor.
         """Create a new instance."""
         self.verbose: int = 0
@@ -120,42 +170,14 @@
                 f"(LEVEL={logging.root.getEffectiveLevel()})",
                 fg="yellow",
             )
         )
     info.verbose = verbose
 
 
-@cli.command
-@click.argument('project_id', required=True)
-@click.option('--url', default=KodexaPlatform.get_url(), help='The URL to the Kodexa server')
-@click.option('--token', default=KodexaPlatform.get_access_token(), help='Access token')
-@pass_info
-def project(_: Info, project_id: str, token: str, url: str):
-    """
-    Get details for a specific project.
-
-    project_id is the ID of the project to get details for.
-
-    """
-
-    client = KodexaClient(url=url, access_token=token)
-    project_instance = client.get_project(project_id)
-    print(f"Name: [bold]{project_instance.name}[/bold]")
-    print(f"Description: [bold]{project_instance.description}[/bold]\n")
-
-    print("[bold]Document Stores[/bold]")
-    project_instance.document_stores.print_table()
-    print("[bold]Data Stores[/bold]")
-    project_instance.data_stores.print_table()
-    print("[bold]Data Structures[/bold]")
-    project_instance.taxonomies.print_table()
-    print("[bold]Assistants[/bold]")
-    project_instance.assistants.print_table()
-
-
 @cli.command()
 @click.argument('ref', required=True)
 @click.argument('paths', required=True, nargs=-1)
 @click.option('--url', default=KodexaPlatform.get_url(), help='The URL to the Kodexa server')
 @click.option('--token', default=KodexaPlatform.get_access_token(), help='Access token')
 @pass_info
 def upload(_: Info, ref: str, paths: list[str], token: str, url: str):
```

### Comparing `kodexa_cli-6.2.25163504424/kodexa_cli/documentation.py` & `kodexa_cli-6.2.25203804340/kodexa_cli/documentation.py`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25163504424/kodexa_cli/templates/assistant.jinja2` & `kodexa_cli-6.2.25203804340/kodexa_cli/templates/assistant.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25163504424/kodexa_cli/templates/content-taxon.jinja2` & `kodexa_cli-6.2.25203804340/kodexa_cli/templates/content-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25163504424/kodexa_cli/templates/document-store.jinja2` & `kodexa_cli-6.2.25203804340/kodexa_cli/templates/document-store.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25163504424/kodexa_cli/templates/header.jinja2` & `kodexa_cli-6.2.25203804340/kodexa_cli/templates/header.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25163504424/kodexa_cli/templates/model.jinja2` & `kodexa_cli-6.2.25203804340/kodexa_cli/templates/model.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25163504424/kodexa_cli/templates/options.jinja2` & `kodexa_cli-6.2.25203804340/kodexa_cli/templates/options.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25163504424/kodexa_cli/templates/processing-taxon.jinja2` & `kodexa_cli-6.2.25203804340/kodexa_cli/templates/processing-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25163504424/kodexa_cli/templates/taxonomy-structure.jinja2` & `kodexa_cli-6.2.25203804340/kodexa_cli/templates/taxonomy-structure.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25163504424/pyproject.toml` & `kodexa_cli-6.2.25203804340/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa-cli"
-version = "6.2.25163504424"
+version = "6.2.25203804340"
 description = "Command Line Tools for Kodexa"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>", "John Patrick Sese <jp@kodexa.com>"]
 readme = "README.md"
 packages = [{include = "kodexa_cli"}]
 
 [tool.poetry.scripts]
 kodexa = 'kodexa_cli:cli'
```

### Comparing `kodexa_cli-6.2.25163504424/setup.py` & `kodexa_cli-6.2.25203804340/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'rich==13.3.5']
 
 entry_points = \
 {'console_scripts': ['kodexa = kodexa_cli:cli']}
 
 setup_kwargs = {
     'name': 'kodexa-cli',
-    'version': '6.2.25163504424',
+    'version': '6.2.25203804340',
     'description': 'Command Line Tools for Kodexa',
     'long_description': '# Kodexa Command Line Tools\n\n[![Kodexa CLI Python Package](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml/badge.svg)](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml)\n\n![img.png](https://docs.kodexa.com/img.png)\n\nKodexa is a platform for building intelligent document processing pipelines. It is a set of tools and services that\nallow you to build a pipeline that can take a document, extract the content, and then process it to extract the\ninformation you need.\n\nIt is built on a set of core principles:\n\n* **Document Centric** - Kodexa is built around the idea of a document. A document is a collection of content\n  nodes that are connected together. This is a powerful model that allows you to build pipelines that can\n  extract content from a wide range of sources.\n\n* **Pipeline Oriented** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that\n  can be executed on a document. This allows you to build a pipeline that can extract content from a wide range\n  of sources.\n\n* **Extensible** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that can be executed\n  on a document. This allows you to build a pipeline that can extract content from a wide range of sources.\n\n* **Label Driven** - Kodexa focuses on the idea of labels. Labels are a way to identify content within a document\n  and then use that content to drive the processing of the document.\n\n# Command Line Tools\n\nThis repository contains the command line tools for Kodexa. The tools are the primary way to interact with Kodexa. It\nallows you to configure components and manage aspects of your Kodexa Platform installation.\n\n## Documentation & Examples\n\nDocumentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)\n\n## Current Development\n\n**BUILD VERSION FLOW**\n![build-version-flow.png](docs%2Fbuild-version-flow.png)\nBuild version will differ based on the branches that are published to pypi.\n\n**GITHUB PROCESS**\n![github-process.png](docs%2Fgithub-process.png)\nChanges that contain bugs, features, and fixes should first be pushed to the test branch.\nOnce these changes are thoroughly tested, they can be submitted as a pull request to the main branch. The pull request should be reviewed and approved by an appropriate person before the changes can be merged.\n\n## Set-up\n\nWe use poetry to manage our dependencies, so you can install them with:\n\n    poetry install\n\nYou can then run the tests with:\n\n    poetry run pytest\n\n# Contributing\n\nWe welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.\n\n# License\n\nApache 2.0\n',
     'author': 'Austin Redenbaugh',
     'author_email': 'austin@kodexa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kodexa_cli-6.2.25163504424/PKG-INFO` & `kodexa_cli-6.2.25203804340/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa-cli
-Version: 6.2.25163504424
+Version: 6.2.25203804340
 Summary: Command Line Tools for Kodexa
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

