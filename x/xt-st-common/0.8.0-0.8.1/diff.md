# Comparing `tmp/xt_st_common-0.8.0.tar.gz` & `tmp/xt_st_common-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-0.8.0.tar", max compression
+gzip compressed data, was "xt_st_common-0.8.1.tar", max compression
```

## Comparing `xt_st_common-0.8.0.tar` & `xt_st_common-0.8.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      720 2023-06-07 15:01:42.693166 xt_st_common-0.8.0/README.md
--rw-r--r--   0        0        0     2603 2023-06-07 15:01:42.689166 xt_st_common-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6128 2023-06-07 15:01:03.676754 xt_st_common-0.8.0/src/streamlit_plotly_events/__init__.py
--rw-r--r--   0        0        0      180 2023-06-07 15:01:03.676754 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/.env
--rw-r--r--   0        0        0       67 2023-06-07 15:01:03.676754 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/.prettierrc
--rw-r--r--   0        0        0      859 2023-06-07 15:01:03.676754 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     2052 2023-06-07 15:01:03.676754 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/index.html
--rw-r--r--   0        0        0      564 2023-06-07 15:01:03.676754 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
--rw-r--r--   0        0        0     1183 2023-06-07 15:01:03.676754 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/service-worker.js
--rw-r--r--   0        0        0  4138182 2023-06-07 15:01:03.696755 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
--rw-r--r--   0        0        0     3326 2023-06-07 15:01:03.696755 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0 16152785 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
--rw-r--r--   0        0        0     1442 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
--rw-r--r--   0        0        0     3848 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
--rw-r--r--   0        0        0     1598 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0        0        0     8317 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
--rw-r--r--   0        0        0     1141 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/package.json
--rw-r--r--   0        0        0      839 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/public/index.html
--rw-r--r--   0        0        0     1922 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
--rw-r--r--   0        0        0      274 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      459 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/tsconfig.json
--rw-r--r--   0        0        0       22 2023-06-07 15:01:42.689166 xt_st_common-0.8.0/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     5010 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/components.py
--rw-r--r--   0        0        0     2371 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/config.py
--rw-r--r--   0        0        0     3177 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/database.py
--rw-r--r--   0        0        0     6303 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/fs_upload_page.py
--rw-r--r--   0        0        0    35117 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/project_components.py
--rw-r--r--   0        0        0     6518 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/project_models.py
--rw-r--r--   0        0        0     5976 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/session.py
--rw-r--r--   0        0        0     6450 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     1957 2023-06-07 15:01:03.776756 xt_st_common-0.8.0/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-06-08 07:45:04.296526 xt_st_common-0.8.1/README.md
+-rw-r--r--   0        0        0     2603 2023-06-08 07:45:04.296526 xt_st_common-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6128 2023-06-08 07:44:30.075797 xt_st_common-0.8.1/src/streamlit_plotly_events/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-08 07:44:30.075797 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/.env
+-rw-r--r--   0        0        0       67 2023-06-08 07:44:30.075797 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/.prettierrc
+-rw-r--r--   0        0        0      859 2023-06-08 07:44:30.075797 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2052 2023-06-08 07:44:30.075797 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/index.html
+-rw-r--r--   0        0        0      564 2023-06-08 07:44:30.075797 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
+-rw-r--r--   0        0        0     1183 2023-06-08 07:44:30.075797 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/service-worker.js
+-rw-r--r--   0        0        0  4138182 2023-06-08 07:44:30.099798 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
+-rw-r--r--   0        0        0     3326 2023-06-08 07:44:30.099798 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0 16152785 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
+-rw-r--r--   0        0        0     1442 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
+-rw-r--r--   0        0        0     3848 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
+-rw-r--r--   0        0        0     1598 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0        0        0     8317 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
+-rw-r--r--   0        0        0     1141 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/package.json
+-rw-r--r--   0        0        0      839 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/public/index.html
+-rw-r--r--   0        0        0     1922 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
+-rw-r--r--   0        0        0      274 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/tsconfig.json
+-rw-r--r--   0        0        0       22 2023-06-08 07:45:04.296526 xt_st_common-0.8.1/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     5010 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     2750 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     3177 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/database.py
+-rw-r--r--   0        0        0     6303 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/fs_upload_page.py
+-rw-r--r--   0        0        0    37146 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/project_components.py
+-rw-r--r--   0        0        0     6518 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/project_models.py
+-rw-r--r--   0        0        0     5976 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     6450 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     1957 2023-06-08 07:44:30.175799 xt_st_common-0.8.1/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.8.1/PKG-INFO
```

### Comparing `xt_st_common-0.8.0/README.md` & `xt_st_common-0.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XT-STREAMLIT - 0.8.0
+# XT-STREAMLIT - 0.8.1
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

### Comparing `xt_st_common-0.8.0/pyproject.toml` & `xt_st_common-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xt-st-common"
-version = "0.8.0"
+version = "0.8.1"
 description = "Common Streamlit framework used by Exploration Toolkit"
 authors = ["Alex Hunt <alex.hunt@csiro.au>", "Sam Bradley <sam.bradley@csiro.au>", "John Hille <john.hille@csiro.au>"]
 readme = "README.md"
 packages = [{include = "xt_st_common", from= "src"}, {include = "streamlit_plotly_events", from= "src"}]
 
 [tool.poe.tasks]
 test = { cmd="pytest --cov=src/xt_st_common", help="Run unit tests"}
```

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/__init__.py` & `xt_st_common-0.8.1/src/streamlit_plotly_events/__init__.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/asset-manifest.json` & `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/index.html` & `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js` & `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/service-worker.js` & `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js` & `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt` & `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map` & `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js` & `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map` & `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js` & `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/package.json` & `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/package.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/public/index.html` & `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx` & `xt_st_common-0.8.1/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/xt_st_common/components.py` & `xt_st_common-0.8.1/src/xt_st_common/components.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/xt_st_common/config.py` & `xt_st_common-0.8.1/src/xt_st_common/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,20 @@
 
     APP_NAME: str = "my_app"
     """Name of the app that be tagged in the DB"""
     APP_TAG_TEXT: str = "Development"
     """text that will appear next the application logo"""
     APP_TAG_BACKGROUND: Color = Color("#00a9ce")
     """background colour of the APP_TAG_TEXT"""
+    APP_GET_HELP: str = None
+    """Link to "Get Help" in streamlit hamburger menu (menu item is hidden if set to None)"""
+    APP_REPORT_BUG: str = None
+    """Link to "Report a Bug" in streamlit hamburger menu (menu item is hidden if set to None)"""
+    APP_ABOUT: str = None
+    """Markdown Text to show in streamlit hamburger menu (shows streamlit default if set to None)"""
     DEBUG: bool = False
     """Enable debug information in the app"""
     DEBUG_MOCK_SESSION: bool = False
     """Mock the session headers returned when deployed to AWS"""
     USE_COGNITO: bool = False
     """Use AWS Cognito for Auth"""
     COGNITO_COOKIE: str = "AWSELBAuthSessionCookie"
```

### Comparing `xt_st_common-0.8.0/src/xt_st_common/database.py` & `xt_st_common-0.8.1/src/xt_st_common/database.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/xt_st_common/fs_upload_page.py` & `xt_st_common-0.8.1/src/xt_st_common/fs_upload_page.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/xt_st_common/project_components.py` & `xt_st_common-0.8.1/src/xt_st_common/project_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,24 +32,30 @@
 # mapping for language options for streamlit code formatter. For other available options
 # see: https://github.com/react-syntax-highlighter/react-syntax-highlighter/blob/master/AVAILABLE_LANGUAGES_PRISM.MD
 CODE_FORMAT_MAPPING = {
     "json": "json",
     "yaml": "yaml",
     "yml": "yaml",
     "toml": "toml",
-    "md": "markfown",
+    "md": "markdown",
 }
 
 REPLACE_FILE_HELP_TXT = (
     "The new file can have a different name but must have the same extension."
     "Warning: Uploading a new file that is significantly different to the original "
     "can have catastrophic results."
 )
 
 
+def has_project_write_access(project: Project):
+    return project.owner.lower() == get_user_email().lower() or get_user_email().lower() in (
+        user.lower() for user in project.users
+    )
+
+
 def state_reset():
     for s in ProjectState:
         if s in [ProjectState.PROJECT_TO_DELETE, ProjectState.FILE_TO_DELETE]:
             set_state(s, None)
         else:
             set_state(s, "")
 
@@ -67,50 +73,63 @@
     project = get_selected_project()
     if project is None:
         raise ValueError("No project was selected")
     return project
 
 
 def set_selected_project(project: Optional[Project]):
+    if project is not None and not isinstance(project, Project):
+        raise ValueError("Setting selected project to a type other than project")
     st.session_state.selected_project = project
 
 
 def submit_delete_project(project: Project):
     """Callback function to set state in order to enable a delete on the next run."""
     # display a warning if the user entered an existing name
 
     if project is None:
         set_state(ProjectState.PROJECT_WARNING_MESSAGE, "No project is selected")
+    elif project.owner.lower() != get_user_email().lower():
+        set_state(
+            ProjectState.PROJECT_WARNING_MESSAGE,
+            f"Delete of project **{project.name}** failed: You are not the owner.",
+        )
     else:
         set_state(
             ProjectState.PROJECT_DELETE_CONFIRM,
             (
                 "Deleting will remove all files that are part of project: "
                 + f"**'{project.name}'**. Are you sure you want to continue?"
             ),
         )
         set_state(ProjectState.PROJECT_TO_DELETE, project)
 
 
 def action_delete(project: Project):
-    if project.id is not None:
+    if project.id is not None and project.owner.lower() == get_user_email().lower():
         delete_project(project.id)
     set_state(
         ProjectState.PROJECT_SUCCESS_MESSAGE,
         f"Project **'{project.name}'** deleted successfully",
     )
 
 
 def submit_delete_folder(folder: str):
     """Callback function to set state in order to enable a delete on the next run."""
     # display a warning if the user entered an existing name
     project = st.session_state.selected_project
     if project is None:
         set_state(ProjectState.UPLOAD_WARNING_MESSAGE, "No project is selected")
-    if folder is None:
+    elif not has_project_write_access(project):
+        set_state(
+            ProjectState.UPLOAD_WARNING_MESSAGE,
+            f"You don't have write access to project: {project.name}",
+        )
+        return
+    elif folder is None:
         set_state(ProjectState.UPLOAD_WARNING_MESSAGE, "No folder is selected")
     else:
         set_state(
             ProjectState.UPLOAD_DELETE_CONFIRM,
             (
                 "Deleting will remove all files that are part of this folder: "
                 + f"**'{folder}'**. Are you sure you want to continue?"
@@ -133,16 +152,22 @@
 
 def submit_delete_file(file: FileRef):
     """Callback function to set state in order to enable a delete on the next run."""
     # display a warning if the user entered an existing name
     project = st.session_state.selected_project
     if project is None:
         set_state(ProjectState.FILE_WARNING_MESSAGE, "No project is selected")
-    if file is None:
+    elif file is None:
         set_state(ProjectState.FILE_WARNING_MESSAGE, "No file is selected")
+    elif not has_project_write_access(project):
+        set_state(
+            ProjectState.FILE_WARNING_MESSAGE,
+            f"You don't have write access to project: {project.name}",
+        )
+        return
     else:
         set_state(
             ProjectState.FILE_DELETE_CONFIRM,
             f"Are you sure you want to delete file **'{file.name}'**?",
         )
         set_state(ProjectState.FILE_TO_DELETE, file)
 
@@ -253,14 +278,21 @@
     if not folders_string:
         set_state(
             ProjectState.UPLOAD_WARNING_MESSAGE,
             "Cannot add new folders: Folder name was empty",
         )
         return
 
+    if not has_project_write_access(project):
+        set_state(
+            ProjectState.UPLOAD_WARNING_MESSAGE,
+            f"You don't have write access to project: {project.name}",
+        )
+        return
+
     count = project.add_folders(folders_string)
     save_project(project)
     set_state(
         ProjectState.UPLOAD_SUCCESS_MESSAGE,
         f"{count} folders were added to **'{project.name}'**",
     )
 
@@ -273,14 +305,17 @@
     if ext == ".csv":
         file = storage_client().get_file(path)
         encoding, dialect = get_encoding_and_dialect(file)
         return pd.read_csv(file, nrows=num_rows, sep=dialect.delimiter, encoding=encoding)
     if ext == ".feather":
         file = storage_client().get_file(path)
         return pd.read_feather(file)
+    if ext == ".xlsx":
+        file = storage_client().get_file(path)
+        return pd.read_excel(file, sheet_name=0, nrows=num_rows)
 
     return None
 
 
 def get_string_preview(fileref: FileRef):
     file = storage_client().get_file(fileref.path)
     return file.getvalue().decode("utf-8")
@@ -325,15 +360,15 @@
     Args:
         root_path (Path): The root Path to where the project folders live
     """
     selected_project = None
 
     if header_text is not None:
         st_context.subheader(header_text)
-    include_public = st_context.checkbox("Include Public", value=False, key="include_public_projects")
+    include_public = st_context.checkbox("Public projects", value=False, key="include_public_projects")
     options, projects, sel_idx = get_proj_options(include_public, get_project_cache())
     proj_options = {}
 
     # accomodate the null option if one is provided
     if null_option is not None:
         proj_options = {-1: null_option}
         sel_idx = sel_idx + 1
@@ -504,17 +539,17 @@
     if path is not None and folder is not None:
         row = container1.expander("Folder Actions", expanded=expand_folder_actions)
 
         state = _state_name(str(project.id), folder)
         if state not in st.session_state:
             st.session_state[state] = 0
 
-        if allow_upload:
+        if allow_upload and has_project_write_access(project):
             if auto_parse_csv:
-                try_parse_csv = st.checkbox(
+                try_parse_csv = row.checkbox(
                     "Parse CSV/TXT as Dataset",
                     value=True,
                     help=(
                         "If a CSV or TXT file is uploaded you will be given options to help "
                         + "calibrate it for use as a dataset."
                     ),
                 )
@@ -647,15 +682,15 @@
                 if allow_delete:
                     row.button(
                         "Delete",
                         key=f"{key_prefix}file_delete_btn",
                         on_click=submit_delete_file,
                         args=(selected_file,),
                     )
-                if selected_key.lower().endswith((".zip", ".csv", ".geojson", ".gpkg", ".feather")):
+                if selected_key.lower().endswith((".zip", ".csv", ".geojson", ".gpkg", ".feather", ".xlsx")):
                     preview_frame = row.button(
                         "Preview Frame",
                         key=f"{key_prefix}file_manager_preview_frame",
                     )
                     if preview_frame:
                         with st.expander(f"**Frame Viewer:** {selected_file.name}", expanded=True):
                             st.dataframe(get_df_preview(selected_file.path, selected_file.get_ext()))
@@ -695,35 +730,38 @@
                         accept_multiple_files=False,
                     )
                 ):
                     project.add_replace_file_by_path(uploaded_replace_file, selected_file.path)
                     save_project(project)
                     uploaded_replace_file.close()
                     _update_key(key_prefix, True)
+                    set_state(
+                        ProjectState.FILE_SUCCESS_MESSAGE,
+                        f"Contents of file: **'{selected_file.path}'** was succesfully replaced",
+                    )
                     st.experimental_rerun()
         else:
             container2.markdown("##")
             container2.info("No files in selected folder")
 
         state_reset()
     return path, folder
 
 
 def get_projects_data(projects):
     selected_project = get_selected_project()
     proj_data = []
-
     for proj in projects:
-        proj_dict = proj.dict(exclude={"files"})
+        proj_dict = proj.dict(exclude={"files", "folders"})
         # proj_dict = proj.dict(exclude={"files", "folders", "id"})
 
-        # proj_dict["folders"] = "\n".join(proj.folders)
-        proj_dict["files"] = [file.name for file in proj.files]
+        proj_dict["folders"] = f"{len(proj.folders) if proj.folders else 0} Folders"
+        proj_dict["files"] = f"{len(proj.files) if proj.files else 0} Files"
         proj_dict["users"] = ", ".join(proj.users)
-        proj_dict["select"] = selected_project is not None and proj.name == selected_project.name
+        proj_dict["select"] = proj.name == (selected_project.name if selected_project is not None else None)
 
         proj_data.append(proj_dict)
     return proj_data
 
 
 def add_new_project(number=1):
     user_email = get_user_email()
@@ -919,14 +957,19 @@
                     )
                     if db_project is None:
                         set_state(
                             ProjectState.PROJECT_WARNING_MESSAGE,
                             f"Cannot update project: **'{edited_project_data['name'][changed_id]}'** "
                             + " not found in database",
                         )
+                    elif db_project.owner.lower() != get_user_email().lower():
+                        set_state(
+                            ProjectState.PROJECT_WARNING_MESSAGE,
+                            f"Save changes on project **{db_project.name}** failed: You are not the owner.",
+                        )
                     else:
                         db_project.__dict__.update(
                             {
                                 "name": edited_project_data["name"][changed_id],
                                 "description": edited_project_data["description"][changed_id],
                                 "users": seperate_users(edited_project_data["users"][changed_id]),
                                 "public": bool(edited_project_data["public"][changed_id]),
```

### Comparing `xt_st_common-0.8.0/src/xt_st_common/project_models.py` & `xt_st_common-0.8.1/src/xt_st_common/project_models.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/xt_st_common/session.py` & `xt_st_common-0.8.1/src/xt_st_common/session.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/xt_st_common/storage.py` & `xt_st_common-0.8.1/src/xt_st_common/storage.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/src/xt_st_common/utils.py` & `xt_st_common-0.8.1/src/xt_st_common/utils.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.0/PKG-INFO` & `xt_st_common-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 0.8.0
+Version: 0.8.1
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
 
-# XT-STREAMLIT - 0.8.0
+# XT-STREAMLIT - 0.8.1
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

