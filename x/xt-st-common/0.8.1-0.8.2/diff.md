# Comparing `tmp/xt_st_common-0.8.1.tar.gz` & `tmp/xt_st_common-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-0.8.1.tar", max compression
+gzip compressed data, was "xt_st_common-0.8.2.tar", max compression
```

## Comparing `xt_st_common-0.8.1.tar` & `xt_st_common-0.8.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      720 2023-06-08 07:45:04.296526 xt_st_common-0.8.1/README.md
--rw-r--r--   0        0        0     2603 2023-06-08 07:45:04.296526 xt_st_common-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     6128 2023-06-08 07:44:30.075797 xt_st_common-0.8.1/src/streamlit_plotly_events/__init__.py
--rw-r--r--   0        0        0      180 2023-06-08 07:44:30.075797 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/.env
--rw-r--r--   0        0        0       67 2023-06-08 07:44:30.075797 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/.prettierrc
--rw-r--r--   0        0        0      859 2023-06-08 07:44:30.075797 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     2052 2023-06-08 07:44:30.075797 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/index.html
--rw-r--r--   0        0        0      564 2023-06-08 07:44:30.075797 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
--rw-r--r--   0        0        0     1183 2023-06-08 07:44:30.075797 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/service-worker.js
--rw-r--r--   0        0        0  4138182 2023-06-08 07:44:30.099798 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
--rw-r--r--   0        0        0     3326 2023-06-08 07:44:30.099798 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0 16152785 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
--rw-r--r--   0        0        0     1442 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
--rw-r--r--   0        0        0     3848 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
--rw-r--r--   0        0        0     1598 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0        0        0     8317 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
--rw-r--r--   0        0        0     1141 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/package.json
--rw-r--r--   0        0        0      839 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/public/index.html
--rw-r--r--   0        0        0     1922 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
--rw-r--r--   0        0        0      274 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      459 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/tsconfig.json
--rw-r--r--   0        0        0       22 2023-06-08 07:45:04.296526 xt_st_common-0.8.1/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     5010 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/components.py
--rw-r--r--   0        0        0     2750 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/config.py
--rw-r--r--   0        0        0     3177 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/database.py
--rw-r--r--   0        0        0     6303 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/fs_upload_page.py
--rw-r--r--   0        0        0    37146 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/project_components.py
--rw-r--r--   0        0        0     6518 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/project_models.py
--rw-r--r--   0        0        0     5976 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/session.py
--rw-r--r--   0        0        0     6450 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     1957 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-06-08 10:07:59.069908 xt_st_common-0.8.2/README.md
+-rw-r--r--   0        0        0     2603 2023-06-08 10:07:59.069908 xt_st_common-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     6128 2023-06-08 10:07:22.057981 xt_st_common-0.8.2/src/streamlit_plotly_events/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-08 10:07:22.057981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/.env
+-rw-r--r--   0        0        0       67 2023-06-08 10:07:22.057981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/.prettierrc
+-rw-r--r--   0        0        0      859 2023-06-08 10:07:22.057981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2052 2023-06-08 10:07:22.057981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/index.html
+-rw-r--r--   0        0        0      564 2023-06-08 10:07:22.057981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
+-rw-r--r--   0        0        0     1183 2023-06-08 10:07:22.057981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/service-worker.js
+-rw-r--r--   0        0        0  4138182 2023-06-08 10:07:22.081981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
+-rw-r--r--   0        0        0     3326 2023-06-08 10:07:22.081981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0 16152785 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
+-rw-r--r--   0        0        0     1442 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
+-rw-r--r--   0        0        0     3848 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
+-rw-r--r--   0        0        0     1598 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0        0        0     8317 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
+-rw-r--r--   0        0        0     1141 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/package.json
+-rw-r--r--   0        0        0      839 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/public/index.html
+-rw-r--r--   0        0        0     1922 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
+-rw-r--r--   0        0        0      274 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/tsconfig.json
+-rw-r--r--   0        0        0       22 2023-06-08 10:07:59.065908 xt_st_common-0.8.2/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     5010 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     2750 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     3177 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/xt_st_common/database.py
+-rw-r--r--   0        0        0     6303 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/xt_st_common/fs_upload_page.py
+-rw-r--r--   0        0        0    39344 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/xt_st_common/project_components.py
+-rw-r--r--   0        0        0     6518 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/xt_st_common/project_models.py
+-rw-r--r--   0        0        0     5976 2023-06-08 10:07:22.157981 xt_st_common-0.8.2/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     6854 2023-06-08 10:07:22.161980 xt_st_common-0.8.2/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     1957 2023-06-08 10:07:22.161980 xt_st_common-0.8.2/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.8.2/PKG-INFO
```

### Comparing `xt_st_common-0.8.1/README.md` & `xt_st_common-0.8.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XT-STREAMLIT - 0.8.1
+# XT-STREAMLIT - 0.8.2
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

### Comparing `xt_st_common-0.8.1/pyproject.toml` & `xt_st_common-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xt-st-common"
-version = "0.8.1"
+version = "0.8.2"
 description = "Common Streamlit framework used by Exploration Toolkit"
 authors = ["Alex Hunt <alex.hunt@csiro.au>", "Sam Bradley <sam.bradley@csiro.au>", "John Hille <john.hille@csiro.au>"]
 readme = "README.md"
 packages = [{include = "xt_st_common", from= "src"}, {include = "streamlit_plotly_events", from= "src"}]
 
 [tool.poe.tasks]
 test = { cmd="pytest --cov=src/xt_st_common", help="Run unit tests"}
```

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/__init__.py` & `xt_st_common-0.8.2/src/streamlit_plotly_events/__init__.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/asset-manifest.json` & `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/index.html` & `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js` & `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/service-worker.js` & `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js` & `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt` & `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map` & `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js` & `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map` & `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js` & `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/package.json` & `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/package.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/public/index.html` & `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx` & `xt_st_common-0.8.2/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/xt_st_common/components.py` & `xt_st_common-0.8.2/src/xt_st_common/components.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/xt_st_common/config.py` & `xt_st_common-0.8.2/src/xt_st_common/config.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/xt_st_common/database.py` & `xt_st_common-0.8.2/src/xt_st_common/database.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/xt_st_common/fs_upload_page.py` & `xt_st_common-0.8.2/src/xt_st_common/fs_upload_page.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/xt_st_common/project_components.py` & `xt_st_common-0.8.2/src/xt_st_common/project_components.py`

 * *Files 4% similar despite different names*

```diff
@@ -293,14 +293,43 @@
     save_project(project)
     set_state(
         ProjectState.UPLOAD_SUCCESS_MESSAGE,
         f"{count} folders were added to **'{project.name}'**",
     )
 
 
+def rename_file(selected_file):
+    project = st.session_state["selected_project"]
+    rename_string = st.session_state["rename_project_file_name"]
+
+    if not rename_string:
+        set_state(
+            ProjectState.FILE_WARNING_MESSAGE,
+            "Cannot rename file. New name was empty",
+        )
+        return
+
+    if not has_project_write_access(project):
+        set_state(
+            ProjectState.FILE_WARNING_MESSAGE,
+            f"You don't have write access to project: {project.name}",
+        )
+        return
+
+    new_path = f"{selected_file.get_prefix()}/{rename_string}"
+
+    storage_client.move_file(selected_file.path, new_path)
+
+    # save_project(project)
+    set_state(
+        ProjectState.FILE_SUCCESS_MESSAGE,
+        f"File **'{selected_file}'** was renamed to **'{rename_string}'**",
+    )
+
+
 @st.cache_data(ttl=300)
 def get_df_preview(path: str, ext: Optional[str], num_rows=10):
     # if filepath.suffix == ".zip":
     #     frame = get_gdf_from_file(filepath)
     #     return frame.iloc[:num_rows, :-1]
     if ext == ".csv":
         file = storage_client().get_file(path)
@@ -482,14 +511,15 @@
     st_context=st.sidebar,
     upload_label: str = "Upload file(s) to selected folder",
     help_text: Optional[str] = None,
     allow_upload=True,
     allow_multiple_uploads=False,
     allow_delete=True,
     allow_replace=True,
+    allow_file_rename=False,
     allow_folder_add=False,
     key_prefix: str = "",
     expand_file_actions=False,
     expand_folder_actions=True,
     folder_select_text="Select Borehole/Run",
     auto_parse_csv=True,
     render_layout: Literal["vertical", "horizontal", "compact"] = "vertical",
@@ -674,52 +704,66 @@
                 key=f"{key_prefix}file_manager_file_select",
             )
             selected_file = files[selected_key] if selected_key in files else None
             if selected_file is not None and selected_key is not None:
                 row = container2.expander("File Actions", expanded=expand_file_actions)
                 if len(selected_key) > 30:
                     row.caption(selected_key)
+
+                if render_layout == "compact":
+                    file_container0 = row.container()
+                    file_container1, file_container2 = row.columns([1, 1])
+                    file_container3 = row.container()
+                    file_container4 = row.container()
+                    file_container5 = row.container()
+
+                else:
+                    file_container0, file_container1, file_container2 = row.columns([1, 1, 1])
+                    file_container3, file_container4, file_container5 = row.columns([2, 1, 1])
+                    file_container4.markdown("#")
+                    file_container5.markdown("#")
+
                 # options = []
                 if allow_delete:
-                    row.button(
-                        "Delete",
+                    file_container5.button(
+                        "Delete Selected",
                         key=f"{key_prefix}file_delete_btn",
                         on_click=submit_delete_file,
                         args=(selected_file,),
                     )
                 if selected_key.lower().endswith((".zip", ".csv", ".geojson", ".gpkg", ".feather", ".xlsx")):
-                    preview_frame = row.button(
+                    preview_frame = file_container0.button(
                         "Preview Frame",
                         key=f"{key_prefix}file_manager_preview_frame",
                     )
                     if preview_frame:
                         with st.expander(f"**Frame Viewer:** {selected_file.name}", expanded=True):
                             st.dataframe(get_df_preview(selected_file.path, selected_file.get_ext()))
                 if selected_key.lower().endswith((".json", ".yml", ".yaml", ".toml", ".md", ".txt")) and (
-                    preview_frame := row.button(
+                    preview_frame := file_container0.button(
                         "Preview File",
                         key=f"{key_prefix}file_manager_preview_file",
                     )
                 ):
                     with st.expander(f"**File Viewer:** {selected_file.name}", expanded=True):
                         code_format = CODE_FORMAT_MAPPING.get(selected_key.lower().split(".")[-1])
                         if code_format is None:
                             st.write(get_string_preview(selected_file))
                         else:
                             st.code(
                                 get_string_preview(selected_file),
                                 language=code_format,
                             )
-                if row.checkbox(
+                if file_container1.checkbox(
                     "Prepare Download",
                     key=f"{key_prefix}file_manager_download_chbx",
                 ):
                     file_data = storage_client().get_file(selected_file.path)
 
-                    row.download_button(
+                    file_container2.download_button(
                         "Download",
                         file_data,
                         selected_file.name,
                         key=f"{key_prefix}file_manager_download_button",
                     )
                 if allow_replace and (
                     uploaded_replace_file := row.file_uploader(
@@ -735,14 +779,28 @@
                     uploaded_replace_file.close()
                     _update_key(key_prefix, True)
                     set_state(
                         ProjectState.FILE_SUCCESS_MESSAGE,
                         f"Contents of file: **'{selected_file.path}'** was succesfully replaced",
                     )
                     st.experimental_rerun()
+                if allow_file_rename:
+                    file_container3.text_input(
+                        "Rename file as:",
+                        key="rename_project_file_name",
+                        help="Selected file will be renamed to this value when 'Rename Selected' is clicked",
+                        placeholder="New file name",
+                    )
+                    file_container4.button(
+                        label="Rename Selected",
+                        help="Rename File",
+                        on_click=rename_file,
+                        args=(selected_file,),
+                    )
+
         else:
             container2.markdown("##")
             container2.info("No files in selected folder")
 
         state_reset()
     return path, folder
```

### Comparing `xt_st_common-0.8.1/src/xt_st_common/project_models.py` & `xt_st_common-0.8.2/src/xt_st_common/project_models.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/xt_st_common/session.py` & `xt_st_common-0.8.2/src/xt_st_common/session.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/src/xt_st_common/storage.py` & `xt_st_common-0.8.2/src/xt_st_common/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 from abc import ABC, abstractmethod
 from io import BytesIO
 from typing import Optional, Union
 
 import streamlit as st
 from minio import Minio
+from minio.commonconfig import CopySource
 from minio.credentials import IamAwsProvider, Provider
 from minio.credentials.providers import StaticProvider
 from minio.error import MinioException
 from minio.helpers import ObjectWriteResult
 from pydantic import BaseModel
 
 from xt_st_common.config import StorageType, StreamlitBaseSettings
@@ -62,14 +63,18 @@
     def list_files(self, path_prefix=""):
         pass
 
     @abstractmethod
     def file_exists(self, file_path: str):
         pass
 
+    @abstractmethod
+    def move_file(self, file_path: str, new_file_path: str):
+        pass
+
 
 class MinioStorageClient(StorageClient):
     def __init__(
         self,
         bucket: str,
         endpoint="s3.amazonaws.com",
         credentials: Provider = IamAwsProvider(),
@@ -133,14 +138,19 @@
         # set MIME_TYPE for MSCL/GeoTek files
         if content_type is None and file_path.lower().endswith((".cal", ".out", ".raw", ".sbd", ".xrf")):
             content_type = "text/plain"
 
         obj = self.__client.put_object(self.__bucket, file_path, file_bytes, file_len, content_type=content_type)
         return self.object_to_file(obj, file_len, content_type)
 
+    def move_file(self, file_path: str, new_file_path: str) -> Optional[FileRef]:
+        obj = self.__client.copy_object(self.__bucket, new_file_path, CopySource(self.__bucket, file_path))
+        self.delete_file(file_path)
+        return self.object_to_file(obj)
+
     def get_file(self, file_path: str):
         response_data = None
         try:
             response = self.__client.get_object(self.__bucket, file_path)
             # Read data from response.
             response_data = BytesIO(response.read())
             response_data.name = file_path
```

### Comparing `xt_st_common-0.8.1/src/xt_st_common/utils.py` & `xt_st_common-0.8.2/src/xt_st_common/utils.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.1/PKG-INFO` & `xt_st_common-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 0.8.1
+Version: 0.8.2
 Summary: Common Streamlit framework used by Exploration Toolkit
 Author: Alex Hunt
 Author-email: alex.hunt@csiro.au
 Requires-Python: >3.9.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,15 +19,15 @@
 Requires-Dist: pymongo (>=4.3.3) ; extra == "databases"
 Requires-Dist: pymongo-auth-aws (>=1.1.0) ; extra == "databases"
 Requires-Dist: streamlit (>=1.23.1)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
 Description-Content-Type: text/markdown
 
-# XT-STREAMLIT - 0.8.1
+# XT-STREAMLIT - 0.8.2
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

