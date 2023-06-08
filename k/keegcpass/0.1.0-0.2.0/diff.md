# Comparing `tmp/keegcpass-0.1.0.tar.gz` & `tmp/keegcpass-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keegcpass-0.1.0.tar", max compression
+gzip compressed data, was "keegcpass-0.2.0.tar", max compression
```

## Comparing `keegcpass-0.1.0.tar` & `keegcpass-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-06-07 14:16:28.244922 keegcpass-0.1.0/LICENSE.md
--rw-r--r--   0        0        0        0 2023-06-07 11:37:50.075552 keegcpass-0.1.0/README.md
--rw-r--r--   0        0        0      624 2023-06-07 14:59:26.432364 keegcpass-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 11:33:25.399637 keegcpass-0.1.0/src/__init__.py
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 keegcpass-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1180 2023-06-08 08:09:32.686333 keegcpass-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     9881 2023-06-08 08:09:32.686333 keegcpass-0.2.0/LICENSES_3RD_PARTY.md
+-rw-r--r--   0        0        0        0 2023-06-07 11:37:50.075552 keegcpass-0.2.0/README.md
+-rw-r--r--   0        0        0      636 2023-06-08 08:09:32.690333 keegcpass-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-07 11:33:25.399637 keegcpass-0.2.0/src/__init__.py
+-rw-r--r--   0        0        0     2503 2023-06-08 08:09:32.690333 keegcpass-0.2.0/src/secrets_readers.py
+-rw-r--r--   0        0        0     2382 2023-06-08 08:09:32.690333 keegcpass-0.2.0/src/secrets_writers.py
+-rw-r--r--   0        0        0      700 2023-06-08 08:09:32.690333 keegcpass-0.2.0/src/validation_models.py
+-rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 keegcpass-0.2.0/PKG-INFO
```

### Comparing `keegcpass-0.1.0/LICENSE.md` & `keegcpass-0.2.0/LICENSE.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,7 +15,11 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
+
+
+
+This app uses [third-party dependencies](LICENSES_3RD_PARTY.md) that are subject to their respective licenses.
```

### Comparing `keegcpass-0.1.0/pyproject.toml` & `keegcpass-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "keegcpass"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     "Andy Koch <andyvk85@gmail.com>",
 ]
 description = ""
 classifiers = ["Programming Language :: Python :: 3"]
 readme = "README.md"
 packages = [{ include = "src" }]
 license = "MIT"
 repository = "https://github.com/andyvk85/KeeGCPass"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-google-cloud-secret-manager = "^2.16"
-pydantic = "^1.10"
-pykeepass = "^4.0"
+google-cloud-secret-manager = "^2"
+pydantic = "^1"
+pykeepass = "^4"
+pip-licenses = "^4"
 
 [[tool.poetry.source]]
 name = "testpypi"
-url = "https://test.pypi.org/simple/"
+url = "https://test.pypi.org/legacy/"
 default = false
 secondary = false
 
 [build-system]
 requires = ["poetry-core>=1.6.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `keegcpass-0.1.0/PKG-INFO` & `keegcpass-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: keegcpass
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/andyvk85/KeeGCPass
 License: MIT
 Author: Andy Koch
 Author-email: andyvk85@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: google-cloud-secret-manager (>=2.16,<3.0)
-Requires-Dist: pydantic (>=1.10,<2.0)
-Requires-Dist: pykeepass (>=4.0,<5.0)
+Requires-Dist: google-cloud-secret-manager (>=2,<3)
+Requires-Dist: pip-licenses (>=4,<5)
+Requires-Dist: pydantic (>=1,<2)
+Requires-Dist: pykeepass (>=4,<5)
 Project-URL: Repository, https://github.com/andyvk85/KeeGCPass
 Description-Content-Type: text/markdown
```

