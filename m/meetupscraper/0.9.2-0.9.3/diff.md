# Comparing `tmp/meetupscraper-0.9.2.tar.gz` & `tmp/meetupscraper-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meetupscraper-0.9.2.tar", last modified: Tue Dec 13 07:10:06 2022, max compression
+gzip compressed data, was "meetupscraper-0.9.3.tar", last modified: Thu Jun  8 02:22:26 2023, max compression
```

## Comparing `meetupscraper-0.9.2.tar` & `meetupscraper-0.9.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pmysl      (501) staff       (20)        0 2022-12-13 07:10:06.271474 meetupscraper-0.9.2/
--rw-r--r--   0 pmysl      (501) staff       (20)      476 2022-12-13 06:58:34.000000 meetupscraper-0.9.2/LICENSE
--rw-r--r--   0 pmysl      (501) staff       (20)      246 2022-12-13 07:10:06.271355 meetupscraper-0.9.2/PKG-INFO
-drwxr-xr-x   0 pmysl      (501) staff       (20)        0 2022-12-13 07:10:06.270422 meetupscraper-0.9.2/meetupscraper/
--rw-r--r--   0 pmysl      (501) staff       (20)      900 2022-12-13 07:01:15.000000 meetupscraper-0.9.2/meetupscraper/__init__.py
-drwxr-xr-x   0 pmysl      (501) staff       (20)        0 2022-12-13 07:10:06.271194 meetupscraper-0.9.2/meetupscraper.egg-info/
--rw-r--r--   0 pmysl      (501) staff       (20)      246 2022-12-13 07:10:06.000000 meetupscraper-0.9.2/meetupscraper.egg-info/PKG-INFO
--rw-r--r--   0 pmysl      (501) staff       (20)      226 2022-12-13 07:10:06.000000 meetupscraper-0.9.2/meetupscraper.egg-info/SOURCES.txt
--rw-r--r--   0 pmysl      (501) staff       (20)        1 2022-12-13 07:10:06.000000 meetupscraper-0.9.2/meetupscraper.egg-info/dependency_links.txt
--rw-r--r--   0 pmysl      (501) staff       (20)       30 2022-12-13 07:10:06.000000 meetupscraper-0.9.2/meetupscraper.egg-info/requires.txt
--rw-r--r--   0 pmysl      (501) staff       (20)       14 2022-12-13 07:10:06.000000 meetupscraper-0.9.2/meetupscraper.egg-info/top_level.txt
--rw-r--r--   0 pmysl      (501) staff       (20)       38 2022-12-13 07:10:06.271507 meetupscraper-0.9.2/setup.cfg
--rw-r--r--   0 pmysl      (501) staff       (20)      500 2022-12-13 07:06:59.000000 meetupscraper-0.9.2/setup.py
+drwxr-xr-x   0 pmysl      (501) staff       (20)        0 2023-06-08 02:22:26.685133 meetupscraper-0.9.3/
+-rw-r--r--   0 pmysl      (501) staff       (20)      476 2022-12-13 06:58:34.000000 meetupscraper-0.9.3/LICENSE
+-rw-r--r--   0 pmysl      (501) staff       (20)      326 2023-06-08 02:22:26.684967 meetupscraper-0.9.3/PKG-INFO
+drwxr-xr-x   0 pmysl      (501) staff       (20)        0 2023-06-08 02:22:26.683629 meetupscraper-0.9.3/meetupscraper/
+-rw-r--r--   0 pmysl      (501) staff       (20)      921 2023-06-08 01:57:45.000000 meetupscraper-0.9.3/meetupscraper/__init__.py
+drwxr-xr-x   0 pmysl      (501) staff       (20)        0 2023-06-08 02:22:26.684696 meetupscraper-0.9.3/meetupscraper.egg-info/
+-rw-r--r--   0 pmysl      (501) staff       (20)      326 2023-06-08 02:22:26.000000 meetupscraper-0.9.3/meetupscraper.egg-info/PKG-INFO
+-rw-r--r--   0 pmysl      (501) staff       (20)      226 2023-06-08 02:22:26.000000 meetupscraper-0.9.3/meetupscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 pmysl      (501) staff       (20)        1 2023-06-08 02:22:26.000000 meetupscraper-0.9.3/meetupscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 pmysl      (501) staff       (20)       30 2023-06-08 02:22:26.000000 meetupscraper-0.9.3/meetupscraper.egg-info/requires.txt
+-rw-r--r--   0 pmysl      (501) staff       (20)       14 2023-06-08 02:22:26.000000 meetupscraper-0.9.3/meetupscraper.egg-info/top_level.txt
+-rw-r--r--   0 pmysl      (501) staff       (20)       38 2023-06-08 02:22:26.685191 meetupscraper-0.9.3/setup.cfg
+-rw-r--r--   0 pmysl      (501) staff       (20)      627 2023-06-08 02:20:36.000000 meetupscraper-0.9.3/setup.py
```

### Comparing `meetupscraper-0.9.2/meetupscraper/__init__.py` & `meetupscraper-0.9.3/meetupscraper/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     LOGGER.info("Looking up %r", url)
     r = requests.get(url)
 
     events = r.json()
 
     for event in events:
         date = datetime.datetime.fromtimestamp(event["time"] / 1000)
-        venue = event["venue"]
+        venue = event.get("venue", {"name": "N/A"})
 
         yield Event(
             title=event["name"],
             date=date,
             url=event["link"],
             venue=Venue(name=venue["name"], street=venue.get("address_1")),
         )
```

