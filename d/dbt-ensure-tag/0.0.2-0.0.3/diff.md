# Comparing `tmp/dbt_ensure_tag-0.0.2.tar.gz` & `tmp/dbt_ensure_tag-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_ensure_tag-0.0.2.tar", last modified: Sat Apr  8 03:29:04 2023, max compression
+gzip compressed data, was "dbt_ensure_tag-0.0.3.tar", last modified: Thu Jun  8 03:39:28 2023, max compression
```

## Comparing `dbt_ensure_tag-0.0.2.tar` & `dbt_ensure_tag-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 jclemons  (1000) jclemons  (1000)        0 2023-04-08 03:29:04.528979 dbt_ensure_tag-0.0.2/
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)     1073 2023-04-08 02:06:30.000000 dbt_ensure_tag-0.0.2/LICENSE
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)      606 2023-04-08 03:29:04.528979 dbt_ensure_tag-0.0.2/PKG-INFO
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)      146 2023-04-08 02:05:24.000000 dbt_ensure_tag-0.0.2/README.md
-drwxrwxr-x   0 jclemons  (1000) jclemons  (1000)        0 2023-04-08 03:29:04.528979 dbt_ensure_tag-0.0.2/dbt_ensure_tag.egg-info/
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)      606 2023-04-08 03:29:04.000000 dbt_ensure_tag-0.0.2/dbt_ensure_tag.egg-info/PKG-INFO
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)      247 2023-04-08 03:29:04.000000 dbt_ensure_tag-0.0.2/dbt_ensure_tag.egg-info/SOURCES.txt
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)        1 2023-04-08 03:29:04.000000 dbt_ensure_tag-0.0.2/dbt_ensure_tag.egg-info/dependency_links.txt
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)       55 2023-04-08 03:29:04.000000 dbt_ensure_tag-0.0.2/dbt_ensure_tag.egg-info/entry_points.txt
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)       15 2023-04-08 03:29:04.000000 dbt_ensure_tag-0.0.2/dbt_ensure_tag.egg-info/top_level.txt
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)      995 2023-04-08 03:28:37.000000 dbt_ensure_tag-0.0.2/dbt_ensure_tag.py
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)      637 2023-04-08 03:29:04.532979 dbt_ensure_tag-0.0.2/setup.cfg
--rw-rw-r--   0 jclemons  (1000) jclemons  (1000)       74 2023-04-08 01:56:06.000000 dbt_ensure_tag-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 03:39:28.650896 dbt_ensure_tag-0.0.3/
+-rw-rw-rw-   0        0        0     1094 2023-06-08 02:44:15.000000 dbt_ensure_tag-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      785 2023-06-08 03:39:28.650896 dbt_ensure_tag-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-06-08 03:30:07.000000 dbt_ensure_tag-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 03:39:28.649896 dbt_ensure_tag-0.0.3/dbt_ensure_tag.egg-info/
+-rw-rw-rw-   0        0        0      785 2023-06-08 03:39:28.000000 dbt_ensure_tag-0.0.3/dbt_ensure_tag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-06-08 03:39:28.000000 dbt_ensure_tag-0.0.3/dbt_ensure_tag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 03:39:28.000000 dbt_ensure_tag-0.0.3/dbt_ensure_tag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-08 03:39:28.000000 dbt_ensure_tag-0.0.3/dbt_ensure_tag.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-06-08 03:39:28.000000 dbt_ensure_tag-0.0.3/dbt_ensure_tag.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-08 03:39:28.000000 dbt_ensure_tag-0.0.3/dbt_ensure_tag.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1391 2023-06-08 03:30:19.000000 dbt_ensure_tag-0.0.3/dbt_ensure_tag.py
+-rw-rw-rw-   0        0        0      705 2023-06-08 03:39:28.652895 dbt_ensure_tag-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       79 2023-06-08 02:44:15.000000 dbt_ensure_tag-0.0.3/setup.py
```

### Comparing `dbt_ensure_tag-0.0.2/LICENSE` & `dbt_ensure_tag-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Jonathan Clemons
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Jonathan Clemons
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `dbt_ensure_tag-0.0.2/PKG-INFO` & `dbt_ensure_tag-0.0.3/dbt_ensure_tag.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,34 @@
-Metadata-Version: 2.1
-Name: dbt_ensure_tag
-Version: 0.0.2
-Summary: checks dbt models for tags
-Home-page: https://github.com/j-clemons/dbt-ensure-tag
-Author: Jonathan Clemons
-Author-email: j-clemons@tuta.io
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# dbt-ensure-tag
-Checks dbt models for existence of a tag(s)
-
-# Installation
-
-`pip install dbt-ensure-tag`
-
-# Usage
-
-`dbt-ensure-tag [filenames]`
+Metadata-Version: 2.1
+Name: dbt-ensure-tag
+Version: 0.0.3
+Summary: checks dbt models for tags
+Home-page: https://github.com/j-clemons/dbt-ensure-tag
+Author: Jonathan Clemons
+Author-email: j-clemons@tuta.io
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dbt-ensure-tag
+Checks dbt models for existence of a tag(s)
+
+# Installation
+
+`pip install dbt-ensure-tag`
+
+# Usage
+
+`dbt-ensure-tag [filenames]`
+
+## pre-commit config
+```
+repos:
+-   repo: https://github.com/j-clemons/dbt-ensure-tag
+    rev: v0.0.3
+    hooks:
+    -   id: dbt-ensure-tag
+```
```

### Comparing `dbt_ensure_tag-0.0.2/dbt_ensure_tag.py` & `dbt_ensure_tag-0.0.3/dbt_ensure_tag.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,54 @@
-from __future__ import annotations
-
-import argparse
-import json
-from subprocess import run
-from typing import Sequence
-
-
-def main(argv: Sequence[str] | None = None) -> int:
-    parser = argparse.ArgumentParser()
-    parser.add_argument('filenames', nargs='*')
-
-    args = parser.parse_args(argv)
-
-    result = run(
-        f'dbt ls --resource-type model --output json '
-        f'--output-keys alias,original_file_path,tags '
-        f'-s {" ".join(args.filenames)}',
-        capture_output=True,
-        shell=True,
-        text=True,
-    )
-
-    return_code = 0
-    for res in result.stdout.split('\n'):
-        try:
-            j = json.loads(res)
-        except json.decoder.JSONDecodeError:
-            continue
-
-        tags = j.get('tags')
-        if tags is None:
-            continue
-        elif len(tags) == 0:
-            print(f'{j.get("original_file_path")} not tagged.')
-            return_code = 1
-
-    return return_code
-
-
-if __name__ == '__main__':
-    raise SystemExit(main())
+from __future__ import annotations
+
+import argparse
+import json
+import sys
+from typing import Sequence
+from io import StringIO
+from dbt.cli.main import dbtRunner, dbtRunnerResult
+
+
+class NullIO(StringIO):
+    def write(self, txt: str) -> int:
+        pass
+
+
+def main(argv: Sequence[str] | None = None) -> int:
+    parser = argparse.ArgumentParser()
+    parser.add_argument('filenames', nargs='*')
+
+    args = parser.parse_args(argv)
+
+    cli_args = ['ls', '--resource-type', 'model', '--output', 'json',
+                '--output-keys', 'alias', 'original_file_path', 'tags', '-s',
+                ' '.join(args.filenames)]
+
+    dbt = dbtRunner()
+
+    # Suppress stdout from dbt invocation
+    sys.stdout = NullIO()
+    res: dbtRunnerResult = dbt.invoke(cli_args)
+    sys.stdout = sys.__stdout__
+
+    return_code = 0
+    if res.success:
+        for res in res.result:
+            try:
+                j = json.loads(res)
+            except json.decoder.JSONDecodeError:
+                continue
+
+            tags = j.get('tags')
+            if tags is None:
+                continue
+            elif len(tags) == 0:
+                print(f'{j.get("original_file_path")} not tagged.')
+                return_code = 1
+    else:
+        print(res.exception)
+
+    return return_code
+
+
+if __name__ == '__main__':
+    raise SystemExit(main())
```

