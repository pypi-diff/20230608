# Comparing `tmp/swoop.db-0.1.1.tar.gz` & `tmp/swoop.db-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swoop.db-0.1.1.tar", last modified: Thu Jun  1 19:55:43 2023, max compression
+gzip compressed data, was "swoop.db-0.1.2.tar", last modified: Thu Jun  8 21:08:26 2023, max compression
```

## Comparing `swoop.db-0.1.1.tar` & `swoop.db-0.1.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.205333 swoop.db-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.197333 swoop.db-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.201333 swoop.db-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.github/workflows/publish-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.github/workflows/snyk-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.snyk
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.sqlfluff
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-01 19:55:28.000000 swoop.db-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-01 19:55:28.000000 swoop.db-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-01 19:55:28.000000 swoop.db-0.1.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-01 19:55:28.000000 swoop.db-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-01 19:55:43.205333 swoop.db-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-01 19:55:28.000000 swoop.db-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-01 19:55:28.000000 swoop.db-0.1.1/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-01 19:55:28.000000 swoop.db-0.1.1/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-01 19:55:28.000000 swoop.db-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-01 19:55:28.000000 swoop.db-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:55:43.205333 swoop.db-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.201333 swoop.db-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.201333 swoop.db-0.1.1/src/swoop/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.205333 swoop.db-0.1.1/src/swoop/db/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-01 19:55:28.000000 swoop.db-0.1.1/src/swoop/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-01 19:55:28.000000 swoop.db-0.1.1/src/swoop/db/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-01 19:55:28.000000 swoop.db-0.1.1/src/swoop/db/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.205333 swoop.db-0.1.1/src/swoop/db/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-01 19:55:28.000000 swoop.db-0.1.1/src/swoop/db/fixtures/base_01.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.205333 swoop.db-0.1.1/src/swoop/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-06-01 19:55:28.000000 swoop.db-0.1.1/src/swoop/db/migrations/00000_base_schema.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:28.000000 swoop.db-0.1.1/src/swoop/db/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-06-01 19:55:28.000000 swoop.db-0.1.1/src/swoop/db/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.201333 swoop.db-0.1.1/src/swoop.db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-01 19:55:43.000000 swoop.db-0.1.1/src/swoop.db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-01 19:55:43.000000 swoop.db-0.1.1/src/swoop.db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:55:43.000000 swoop.db-0.1.1/src/swoop.db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 19:55:43.000000 swoop.db-0.1.1/src/swoop.db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-01 19:55:43.000000 swoop.db-0.1.1/src/swoop.db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 19:55:43.000000 swoop.db-0.1.1/src/swoop.db.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.205333 swoop.db-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-01 19:55:28.000000 swoop.db-0.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.205333 swoop.db-0.1.1/tests/pgtap/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-01 19:55:28.000000 swoop.db-0.1.1/tests/pgtap/test_action.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-01 19:55:28.000000 swoop.db-0.1.1/tests/pgtap/test_item_inserts.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-01 19:55:28.000000 swoop.db-0.1.1/tests/pgtap/test_limit-locking.sql
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-01 19:55:28.000000 swoop.db-0.1.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-01 19:55:28.000000 swoop.db-0.1.1/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.644108 swoop.db-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.636107 swoop.db-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.640107 swoop.db-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.github/workflows/publish-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.github/workflows/snyk-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.snyk
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-08 21:08:04.000000 swoop.db-0.1.2/.sqlfluff
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-08 21:08:04.000000 swoop.db-0.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-08 21:08:04.000000 swoop.db-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-08 21:08:04.000000 swoop.db-0.1.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-08 21:08:04.000000 swoop.db-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-08 21:08:26.640107 swoop.db-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-08 21:08:04.000000 swoop.db-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-08 21:08:04.000000 swoop.db-0.1.2/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-08 21:08:04.000000 swoop.db-0.1.2/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-08 21:08:04.000000 swoop.db-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-08 21:08:04.000000 swoop.db-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 21:08:26.644108 swoop.db-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.636107 swoop.db-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.636107 swoop.db-0.1.2/src/swoop/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.640107 swoop.db-0.1.2/src/swoop/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 21:08:04.000000 swoop.db-0.1.2/src/swoop/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-08 21:08:04.000000 swoop.db-0.1.2/src/swoop/db/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-08 21:08:04.000000 swoop.db-0.1.2/src/swoop/db/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.640107 swoop.db-0.1.2/src/swoop/db/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-08 21:08:04.000000 swoop.db-0.1.2/src/swoop/db/fixtures/base_01.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.640107 swoop.db-0.1.2/src/swoop/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    15652 2023-06-08 21:08:04.000000 swoop.db-0.1.2/src/swoop/db/migrations/00000_base_schema.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:04.000000 swoop.db-0.1.2/src/swoop/db/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15807 2023-06-08 21:08:04.000000 swoop.db-0.1.2/src/swoop/db/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.640107 swoop.db-0.1.2/src/swoop.db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-08 21:08:26.000000 swoop.db-0.1.2/src/swoop.db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-08 21:08:26.000000 swoop.db-0.1.2/src/swoop.db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 21:08:26.000000 swoop.db-0.1.2/src/swoop.db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 21:08:26.000000 swoop.db-0.1.2/src/swoop.db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-08 21:08:26.000000 swoop.db-0.1.2/src/swoop.db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 21:08:26.000000 swoop.db-0.1.2/src/swoop.db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.640107 swoop.db-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-08 21:08:04.000000 swoop.db-0.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:08:26.640107 swoop.db-0.1.2/tests/pgtap/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-08 21:08:04.000000 swoop.db-0.1.2/tests/pgtap/test_action.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-08 21:08:04.000000 swoop.db-0.1.2/tests/pgtap/test_item_inserts.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-08 21:08:04.000000 swoop.db-0.1.2/tests/pgtap/test_limit-locking.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-08 21:08:04.000000 swoop.db-0.1.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-08 21:08:04.000000 swoop.db-0.1.2/tests/test_database.py
```

### Comparing `swoop.db-0.1.1/.github/workflows/publish-image.yml` & `swoop.db-0.1.2/.github/workflows/publish-image.yml`

 * *Files 18% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 on:
   release:
     types:
       - published
   push:
     branches:
       - main
-    tags:
-      - '*'
   pull_request:
     branches:
       - '*'
 
 jobs:
   build:
     env:
       context: .
       image_name: swoop-db
+      image_registry: "${{ secrets.REGISTRY_URI }}"
+      image_repository: "${{ secrets.REGISTRY_REPOSITORY }}"
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@main
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
@@ -28,47 +28,50 @@
 
       - name: Install dependencies
         run: pip install setuptools-scm
 
       - name: Get image tags
         id: image_tags
         run: |
-          echo -n ::set-output name=IMAGE_TAGS::
           VERSION="$(python -m setuptools_scm | tr + -)"
           TAGS=("${VERSION}")
 
           if [ -n "${{ github.event.release.tag_name }}" ]; then
             MAJOR="$(<<<"${VERSION}" cut -d '.' -f 1)"
             MINOR="${MAJOR}.$(<<<"${VERSION}" cut -d '.' -f 2)"
             TAGS+=('latest' "${MAJOR}" "${MINOR}")
           fi
 
           if [[ "${GITHUB_REF}" =~ refs/tags/(.*) ]]; then
               TAGS+=("git-${BASH_REMATCH[1]}")
           fi
 
+          PREFIX="${{ env.image_registry }}/${{ env.image_repository }}/${{ env.image_name }}"
+          EOF=$(dd if=/dev/urandom bs=15 count=1 status=none | base64)
+          echo "IMAGE_TAGS<<$EOF" >> "$GITHUB_ENV"
           for tag in "${TAGS[@]}"; do
-              echo ${{ secrets.REGISTRY_REPOSITORY }}/${{ env.image_name }}/${tag}
+              echo "${PREFIX}:${tag}" >> "$GITHUB_ENV"
           done
+          echo "$EOF" >> "$GITHUB_ENV"
 
       - name: Set up QEMU
         uses: docker/setup-qemu-action@v2
 
       - name: Set up Docker Buildx
         uses: docker/setup-buildx-action@v2
         with:
           buildkitd-flags: --debug
 
       - name: Login to Quay.io
         uses: docker/login-action@v2
         with:
-          registry: ${{ secrets.REGISTRY_URI }}
+          registry: ${{ env.image_registry }}
           username: ${{ secrets.REGISTRY_USERNAME }}
           password: ${{ secrets.REGISTRY_PASSWORD }}
 
       - name: Build and publish image to Quay
         uses: docker/build-push-action@v4
         with:
           context: ${{ env.context }}
           platforms: linux/amd64,linux/arm64
           push: ${{ github.event_name == 'release' }}
-          tags: ${{ steps.image_tags.outputs.IMAGE_TAGS }}
+          tags: ${{ env.IMAGE_TAGS }}
```

### Comparing `swoop.db-0.1.1/.github/workflows/python-publish.yml` & `swoop.db-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/.github/workflows/python-test.yml` & `swoop.db-0.1.2/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/.github/workflows/snyk-scan.yml` & `swoop.db-0.1.2/.github/workflows/snyk-scan.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/.gitignore` & `swoop.db-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/.pre-commit-config.yaml` & `swoop.db-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/.snyk` & `swoop.db-0.1.2/.snyk`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/CONTRIBUTING.md` & `swoop.db-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/Dockerfile` & `swoop.db-0.1.2/Dockerfile`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 # build python venv for inclusion into image
 FROM postgres:15-bullseye as APP
 RUN apt-get update && apt-get install -y git python3-venv
 WORKDIR /opt/swoop/db
 RUN python3 -m venv --copies swoop-db-venv
 COPY requirements.txt .
-RUN ls ./swoop-db-venv/bin/
 RUN ./swoop-db-venv/bin/pip install -r requirements.txt
-COPY ./src ./src
-COPY README.md pyproject.toml LICENSE ./
-RUN --mount=source=.git,target=.git,type=bind ./swoop-db-venv/bin/pip install .
-
+RUN --mount=source=.git,target=.git,type=bind git clone . clone
+RUN ./swoop-db-venv/bin/pip install ./clone
 
 FROM postgres:15-bullseye
 # install build deps and pg_partman
 RUN set -x && \
     apt-get update && \
     apt-get install -y postgresql-15-partman curl make patch && \
     apt-get clean -y && \
```

### Comparing `swoop.db-0.1.1/LICENSE` & `swoop.db-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/PKG-INFO` & `swoop.db-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 0.1.1
+Version: 0.1.2
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-0.1.1/README.md` & `swoop.db-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/RELEASE.md` & `swoop.db-0.1.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/pyproject.toml` & `swoop.db-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/src/swoop/db/cli.py` & `swoop.db-0.1.2/src/swoop/db/cli.py`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/src/swoop/db/fixtures/base_01.sql` & `swoop.db-0.1.2/src/swoop/db/fixtures/base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/src/swoop/db/migrations/00000_base_schema.up.sql` & `swoop.db-0.1.2/src/swoop/db/schema.sql`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 CREATE SCHEMA swoop;
 CREATE SCHEMA partman;
 CREATE EXTENSION pg_partman SCHEMA partman;
 
 
+CREATE TABLE swoop.schema_version (
+  version integer,
+  applied_at timestamptz DEFAULT now()
+);
+
+INSERT INTO swoop.schema_version (version) VALUES (0);
+
+
 CREATE TABLE swoop.event_state (
   name text PRIMARY KEY,
   description text NOT NULL
 );
 
 INSERT INTO swoop.event_state (name, description) VALUES
 ('PENDING', 'Action created and waiting to be executed'),
@@ -431,7 +439,74 @@
 DECLARE
 BEGIN
   RETURN (
     SELECT pg_advisory_unlock(to_regclass('swoop.thread')::oid::integer, _lock_id)
   );
 END;
 $$;
+
+CREATE FUNCTION swoop.check_cache(plhash bytea, wf_version smallint, wf_name text, invalid timestamptz)
+RETURNS RECORD
+AS $$
+DECLARE
+  rec RECORD;
+BEGIN
+    IF EXISTS (SELECT * FROM swoop.payload_cache WHERE payload_hash = plhash) THEN
+    -- cache already exists
+        DECLARE
+            _status text;
+            _jobid uuid;
+            _payloadid uuid;
+        BEGIN
+            SELECT t.status, t.action_uuid, p.payload_uuid
+            INTO _status,_jobid, _payloadid
+            FROM swoop.payload_cache p
+            INNER JOIN swoop.action a
+            ON p.payload_uuid = a.payload_uuid
+            INNER JOIN swoop.thread t
+            ON a.action_uuid = t.action_uuid
+            WHERE p.payload_hash = plhash
+            ORDER BY t.created_at DESC
+			LIMIT 1;
+
+            IF _status IN ('RUNNING', 'PENDING', 'QUEUED', 'BACKOFF', 'SUCCESSFUL', 'INVALID') THEN
+            -- redirect to job details for that workflow, do not process
+                SELECT FALSE, _jobid INTO rec;
+            ELSE
+            --     -- this means there is already a record in both payload_cache and action tables for this
+            --     -- need to reprocess
+                DECLARE
+                    _ver smallint;
+                    _invalid timestamptz;
+                BEGIN
+                    SELECT workflow_version, invalid_after
+                    INTO _ver, _invalid
+                    FROM   swoop.payload_cache
+                    WHERE  payload_hash = plhash;
+
+                    IF wf_version > _ver OR _invalid < NOW() THEN
+                        IF wf_version > _ver AND _invalid < NOW() THEN
+                            UPDATE swoop.payload_cache SET workflow_version = wf_version, invalid_after = NULL WHERE payload_hash = plhash;
+                        ELSIF wf_version > _ver THEN
+                            UPDATE swoop.payload_cache SET workflow_version = wf_version WHERE payload_hash = plhash;
+                        ELSE
+                            UPDATE swoop.payload_cache SET invalid_after = NULL WHERE payload_hash = plhash;
+                        END IF;
+
+                        -- reprocess the payload
+                        SELECT TRUE, _payloadid, gen_random_uuid() INTO rec;
+                    ELSE
+                        SELECT FALSE, _jobid INTO rec;
+                    END IF;
+                END;
+            END IF;
+        END;
+	ELSE
+        INSERT INTO swoop.payload_cache(payload_hash, workflow_version, workflow_name, invalid_after)
+        VALUES (plhash, wf_version, wf_name, invalid)
+        RETURNING TRUE, payload_uuid, gen_random_uuid() INTO rec;
+    -- process the payload
+	END IF;
+    RETURN rec;
+END;
+$$
+LANGUAGE plpgsql;
```

### Comparing `swoop.db-0.1.1/src/swoop/db/schema.sql` & `swoop.db-0.1.2/src/swoop/db/migrations/00000_base_schema.up.sql`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 CREATE SCHEMA swoop;
 CREATE SCHEMA partman;
 CREATE EXTENSION pg_partman SCHEMA partman;
 
 
-CREATE TABLE swoop.schema_version (
-  version integer,
-  applied_at timestamptz DEFAULT now()
-);
-
-INSERT INTO swoop.schema_version (version) VALUES (0);
-
-
 CREATE TABLE swoop.event_state (
   name text PRIMARY KEY,
   description text NOT NULL
 );
 
 INSERT INTO swoop.event_state (name, description) VALUES
 ('PENDING', 'Action created and waiting to be executed'),
@@ -439,7 +431,74 @@
 DECLARE
 BEGIN
   RETURN (
     SELECT pg_advisory_unlock(to_regclass('swoop.thread')::oid::integer, _lock_id)
   );
 END;
 $$;
+
+CREATE FUNCTION swoop.check_cache(plhash bytea, wf_version smallint, wf_name text, invalid timestamptz)
+RETURNS RECORD
+AS $$
+DECLARE
+  rec RECORD;
+BEGIN
+    IF EXISTS (SELECT * FROM swoop.payload_cache WHERE payload_hash = plhash) THEN
+    -- cache already exists
+        DECLARE
+            _status text;
+            _jobid uuid;
+            _payloadid uuid;
+        BEGIN
+            SELECT t.status, t.action_uuid, p.payload_uuid
+            INTO _status,_jobid, _payloadid
+            FROM swoop.payload_cache p
+            INNER JOIN swoop.action a
+            ON p.payload_uuid = a.payload_uuid
+            INNER JOIN swoop.thread t
+            ON a.action_uuid = t.action_uuid
+            WHERE p.payload_hash = plhash
+            ORDER BY t.created_at DESC
+			LIMIT 1;
+
+            IF _status IN ('RUNNING', 'PENDING', 'QUEUED', 'BACKOFF', 'SUCCESSFUL', 'INVALID') THEN
+            -- redirect to job details for that workflow, do not process
+                SELECT FALSE, _jobid INTO rec;
+            ELSE
+            --     -- this means there is already a record in both payload_cache and action tables for this
+            --     -- need to reprocess
+                DECLARE
+                    _ver smallint;
+                    _invalid timestamptz;
+                BEGIN
+                    SELECT workflow_version, invalid_after
+                    INTO _ver, _invalid
+                    FROM   swoop.payload_cache
+                    WHERE  payload_hash = plhash;
+
+                    IF wf_version > _ver OR _invalid < NOW() THEN
+                        IF wf_version > _ver AND _invalid < NOW() THEN
+                            UPDATE swoop.payload_cache SET workflow_version = wf_version, invalid_after = NULL WHERE payload_hash = plhash;
+                        ELSIF wf_version > _ver THEN
+                            UPDATE swoop.payload_cache SET workflow_version = wf_version WHERE payload_hash = plhash;
+                        ELSE
+                            UPDATE swoop.payload_cache SET invalid_after = NULL WHERE payload_hash = plhash;
+                        END IF;
+
+                        -- reprocess the payload
+                        SELECT TRUE, _payloadid, gen_random_uuid() INTO rec;
+                    ELSE
+                        SELECT FALSE, _jobid INTO rec;
+                    END IF;
+                END;
+            END IF;
+        END;
+	ELSE
+        INSERT INTO swoop.payload_cache(payload_hash, workflow_version, workflow_name, invalid_after)
+        VALUES (plhash, wf_version, wf_name, invalid)
+        RETURNING TRUE, payload_uuid, gen_random_uuid() INTO rec;
+    -- process the payload
+	END IF;
+    RETURN rec;
+END;
+$$
+LANGUAGE plpgsql;
```

### Comparing `swoop.db-0.1.1/src/swoop.db.egg-info/PKG-INFO` & `swoop.db-0.1.2/src/swoop.db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 0.1.1
+Version: 0.1.2
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-0.1.1/src/swoop.db.egg-info/SOURCES.txt` & `swoop.db-0.1.2/src/swoop.db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/tests/conftest.py` & `swoop.db-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/tests/pgtap/test_action.sql` & `swoop.db-0.1.2/tests/pgtap/test_action.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/tests/pgtap/test_item_inserts.sql` & `swoop.db-0.1.2/tests/pgtap/test_item_inserts.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.1/tests/pgtap/test_limit-locking.sql` & `swoop.db-0.1.2/tests/pgtap/test_limit-locking.sql`

 * *Files identical despite different names*

