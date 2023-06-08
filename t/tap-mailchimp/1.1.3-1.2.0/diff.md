# Comparing `tmp/tap-mailchimp-1.1.3.tar.gz` & `tmp/tap-mailchimp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-mailchimp-1.1.3.tar", last modified: Mon Dec 20 22:30:59 2021, max compression
+gzip compressed data, was "tap-mailchimp-1.2.0.tar", last modified: Thu Jun  8 13:21:27 2023, max compression
```

## Comparing `tap-mailchimp-1.1.3.tar` & `tap-mailchimp-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-20 22:30:59.029431 tap-mailchimp-1.1.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      310 2021-12-20 22:30:59.029431 tap-mailchimp-1.1.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2710 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2021-12-20 22:30:59.029431 tap-mailchimp-1.1.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      807 2021-12-20 22:28:57.000000 tap-mailchimp-1.1.3/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-20 22:30:59.029431 tap-mailchimp-1.1.3/tap_mailchimp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1097 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/tap_mailchimp/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3777 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/tap_mailchimp/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      609 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/tap_mailchimp/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1701 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/tap_mailchimp/schema.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-20 22:30:59.029431 tap-mailchimp-1.1.3/tap_mailchimp/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6687 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/tap_mailchimp/schemas/automations.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8473 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/tap_mailchimp/schemas/campaigns.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3356 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/tap_mailchimp/schemas/list_members.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2587 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/tap_mailchimp/schemas/list_segment_members.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1807 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/tap_mailchimp/schemas/list_segments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5360 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/tap_mailchimp/schemas/lists.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      876 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/tap_mailchimp/schemas/reports_email_activity.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      800 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/tap_mailchimp/schemas/unsubscribes.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20872 2021-12-20 16:47:23.000000 tap-mailchimp-1.1.3/tap_mailchimp/sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-20 22:30:59.029431 tap-mailchimp-1.1.3/tap_mailchimp.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      310 2021-12-20 22:30:58.000000 tap-mailchimp-1.1.3/tap_mailchimp.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      700 2021-12-20 22:30:58.000000 tap-mailchimp-1.1.3/tap_mailchimp.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2021-12-20 22:30:58.000000 tap-mailchimp-1.1.3/tap_mailchimp.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2021-12-20 22:30:58.000000 tap-mailchimp-1.1.3/tap_mailchimp.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2021-12-20 22:30:58.000000 tap-mailchimp-1.1.3/tap_mailchimp.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2021-12-20 22:30:58.000000 tap-mailchimp-1.1.3/tap_mailchimp.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-08 13:21:27.969123 tap-mailchimp-1.2.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2022-12-12 10:22:04.000000 tap-mailchimp-1.2.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      299 2023-06-08 13:21:27.969123 tap-mailchimp-1.2.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2856 2023-06-08 13:03:43.000000 tap-mailchimp-1.2.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-08 13:21:27.969123 tap-mailchimp-1.2.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      807 2023-06-08 13:03:43.000000 tap-mailchimp-1.2.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-08 13:21:27.965123 tap-mailchimp-1.2.0/tap_mailchimp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1097 2023-06-08 13:03:55.000000 tap-mailchimp-1.2.0/tap_mailchimp/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4389 2023-06-08 13:03:43.000000 tap-mailchimp-1.2.0/tap_mailchimp/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      609 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1701 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schema.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-08 13:21:27.969123 tap-mailchimp-1.2.0/tap_mailchimp/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6687 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/automations.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8473 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/campaigns.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3356 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/list_members.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2587 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/list_segment_members.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1807 2023-01-04 05:38:09.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/list_segments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5360 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/lists.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      876 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/reports_email_activity.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      800 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/unsubscribes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21929 2023-06-08 13:03:43.000000 tap-mailchimp-1.2.0/tap_mailchimp/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-08 13:21:27.965123 tap-mailchimp-1.2.0/tap_mailchimp.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      299 2023-06-08 13:21:27.000000 tap-mailchimp-1.2.0/tap_mailchimp.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      700 2023-06-08 13:21:27.000000 tap-mailchimp-1.2.0/tap_mailchimp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-08 13:21:27.000000 tap-mailchimp-1.2.0/tap_mailchimp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2023-06-08 13:21:27.000000 tap-mailchimp-1.2.0/tap_mailchimp.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-06-08 13:21:27.000000 tap-mailchimp-1.2.0/tap_mailchimp.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-06-08 13:21:27.000000 tap-mailchimp-1.2.0/tap_mailchimp.egg-info/top_level.txt
```

### Comparing `tap-mailchimp-1.1.3/LICENSE` & `tap-mailchimp-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.1.3/README.md` & `tap-mailchimp-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 | -------- | -------- | ------- | ----------- |
 | `access_token` | See note. | "20208d81..." | The access token from the OAuth2 flow. |
 | `api_key` | See note. | "ac0ad1..." | The Mailchimp API key, if using API key auth instead of OAuth. |
 | `dc` | See note. | "us14" | The Mailchimp data center, only requried when using API key auth. |
 | `start_date` | Y | "2010-01-01T00:00:00Z" | The default start date to use for date modified replication, when available. |
 | `user_agent` | N | "Vandelay Industries ETL Runner" | The user agent to send on every request. |
 | `request_timeout` | N | 300 | Time for which request should wait to get response. |
+| `email_activity_date_window` | N | 30 | Used to fetch campaigns that are sent in the last `x` days to retrive `reports_email_activity` stream |
 
 ## Usage 
 
 To run `tap-mailchimp` with the configuration file, use this command:
 
 ```sh
 tap-mailchimp -c my-config.json
```

### Comparing `tap-mailchimp-1.1.3/setup.py` & `tap-mailchimp-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-mailchimp',
-      version='1.1.3',
+      version='1.2.0',
       description='Singer.io tap for extracting data from the Mailchimp API',
       author='Stitch',
       url='https://singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_mailchimp'],
       install_requires=[
           'backoff==1.8.0',
```

### Comparing `tap-mailchimp-1.1.3/tap_mailchimp/__init__.py` & `tap-mailchimp-1.2.0/tap_mailchimp/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.1.3/tap_mailchimp/discover.py` & `tap-mailchimp-1.2.0/tap_mailchimp/discover.py`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.1.3/tap_mailchimp/schema.py` & `tap-mailchimp-1.2.0/tap_mailchimp/schema.py`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.1.3/tap_mailchimp/schemas/automations.json` & `tap-mailchimp-1.2.0/tap_mailchimp/schemas/automations.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.1.3/tap_mailchimp/schemas/campaigns.json` & `tap-mailchimp-1.2.0/tap_mailchimp/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.1.3/tap_mailchimp/schemas/list_members.json` & `tap-mailchimp-1.2.0/tap_mailchimp/schemas/list_members.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.1.3/tap_mailchimp/schemas/list_segment_members.json` & `tap-mailchimp-1.2.0/tap_mailchimp/schemas/list_segment_members.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.1.3/tap_mailchimp/schemas/list_segments.json` & `tap-mailchimp-1.2.0/tap_mailchimp/schemas/list_segments.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.1.3/tap_mailchimp/schemas/lists.json` & `tap-mailchimp-1.2.0/tap_mailchimp/schemas/lists.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.1.3/tap_mailchimp/schemas/reports_email_activity.json` & `tap-mailchimp-1.2.0/tap_mailchimp/schemas/reports_email_activity.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.1.3/tap_mailchimp/schemas/unsubscribes.json` & `tap-mailchimp-1.2.0/tap_mailchimp/schemas/unsubscribes.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.1.3/tap_mailchimp/sync.py` & `tap-mailchimp-1.2.0/tap_mailchimp/sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -448,14 +448,47 @@
                         batch_id)
             return
 
         # Resume from bookmarked job_id, then if completed, issue a new batch for processing.
         campaigns = [] # Don't need a list of campaigns if resuming
         sync_email_activity(client, catalog, state, start_date, campaigns, batch_id)
 
+def fetch_recent_campaigns(client, catalog, state, campaigns_config):
+    return sync_endpoint(client, catalog, state,
+                         client.adjusted_start_date,  # adjusted start date
+                         "campaigns", False, # persist set to false (fetch campaign id's only)
+                         campaigns_config.get('path'),
+                         campaigns_config.get( 'data_path', "campaigns"),
+                         campaigns_config.get('params', {}), ["campaigns"],
+                         "since_send_time", #new bookmark_query_field
+                         None)
+
+def sync_reports_email_activity(streams_to_sync, id_bag, client, catalog, state, start_date, campaign_config):
+    should_stream, _ = should_sync_stream(
+        streams_to_sync, [], 'reports_email_activity')
+    if client.adjusted_start_date:
+        LOGGER.info("Fetching Campaigns since %s for email activty", client.adjusted_start_date)
+        campaign_ids = fetch_recent_campaigns(client, catalog, state, campaign_config)
+    else:
+        campaign_ids = id_bag.get('campaigns')
+    if should_stream and campaign_ids:
+        # Resume previous batch, if necessary
+        check_and_resume_email_activity_batch(
+            client, catalog, state, start_date)
+        # Chunk batch_ids, bookmarking the chunk number
+        sorted_campaigns = sorted(campaign_ids)
+        chunk_bookmark = int(get_bookmark(
+            state, ['reports_email_activity_next_chunk'], 0))
+        for i, campaign_chunk in enumerate(chunk_campaigns(sorted_campaigns, chunk_bookmark)):
+            write_email_activity_chunk_bookmark(
+                state, chunk_bookmark, i, sorted_campaigns)
+            sync_email_activity(client, catalog, state,
+                                start_date, campaign_chunk)
+        # Start from the beginning next time
+        write_bookmark(state, ['reports_email_activity_next_chunk'], 0)
 ## TODO: is current_stream being updated?
 
 def sync(client, catalog, state, start_date):
     streams_to_sync = {
         'selected_streams': get_selected_streams(catalog),
         'last_stream': state.get('current_stream')
     }
@@ -519,23 +552,8 @@
                     state,
                     start_date,
                     streams_to_sync,
                     id_bag,
                     stream_name,
                     endpoint_config)
 
-    should_stream, _ = should_sync_stream(streams_to_sync,
-                                          [],
-                                          'reports_email_activity')
-    campaign_ids = id_bag.get('campaigns')
-    if should_stream and campaign_ids:
-        # Resume previous batch, if necessary
-        check_and_resume_email_activity_batch(client, catalog, state, start_date)
-        # Chunk batch_ids, bookmarking the chunk number
-        sorted_campaigns = sorted(campaign_ids)
-        chunk_bookmark = int(get_bookmark(state, ['reports_email_activity_next_chunk'], 0))
-        for i, campaign_chunk in enumerate(chunk_campaigns(sorted_campaigns, chunk_bookmark)):
-            write_email_activity_chunk_bookmark(state, chunk_bookmark, i, sorted_campaigns)
-            sync_email_activity(client, catalog, state, start_date, campaign_chunk)
-
-        # Start from the beginning next time
-        write_bookmark(state, ['reports_email_activity_next_chunk'], 0)
+    sync_reports_email_activity(streams_to_sync, id_bag, client, catalog, state, start_date, endpoints["campaigns"])
```

### Comparing `tap-mailchimp-1.1.3/tap_mailchimp.egg-info/SOURCES.txt` & `tap-mailchimp-1.2.0/tap_mailchimp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

