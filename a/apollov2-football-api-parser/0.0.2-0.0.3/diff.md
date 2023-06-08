# Comparing `tmp/apollov2_football_api_parser-0.0.2.tar.gz` & `tmp/apollov2_football_api_parser-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollov2_football_api_parser-0.0.2.tar", last modified: Thu Jun  8 16:49:23 2023, max compression
+gzip compressed data, was "apollov2_football_api_parser-0.0.3.tar", last modified: Thu Jun  8 17:11:41 2023, max compression
```

## Comparing `apollov2_football_api_parser-0.0.2.tar` & `apollov2_football_api_parser-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:49:23.425166 apollov2_football_api_parser-0.0.2/
--rw-r--r--   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:25:55.000000 apollov2_football_api_parser-0.0.2/LICENSE
--rw-r--r--   0 jerrywang   (501) staff       (20)      912 2023-06-08 16:49:23.425255 apollov2_football_api_parser-0.0.2/PKG-INFO
--rw-r--r--   0 jerrywang   (501) staff       (20)      528 2023-06-08 16:30:33.000000 apollov2_football_api_parser-0.0.2/README.md
--rw-r--r--   0 jerrywang   (501) staff       (20)      103 2023-06-08 16:27:29.000000 apollov2_football_api_parser-0.0.2/pyproject.toml
--rw-r--r--   0 jerrywang   (501) staff       (20)      508 2023-06-08 16:49:23.425615 apollov2_football_api_parser-0.0.2/setup.cfg
-drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:49:23.422825 apollov2_football_api_parser-0.0.2/src/
-drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:49:23.423714 apollov2_football_api_parser-0.0.2/src/apollov2/
--rw-r--r--   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:48:32.000000 apollov2_football_api_parser-0.0.2/src/apollov2/__init__.py
--rw-r--r--   0 jerrywang   (501) staff       (20)    15911 2023-06-08 16:30:31.000000 apollov2_football_api_parser-0.0.2/src/apollov2/api_parser.py
-drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:49:23.425010 apollov2_football_api_parser-0.0.2/src/apollov2_football_api_parser.egg-info/
--rw-r--r--   0 jerrywang   (501) staff       (20)      912 2023-06-08 16:49:23.000000 apollov2_football_api_parser-0.0.2/src/apollov2_football_api_parser.egg-info/PKG-INFO
--rw-r--r--   0 jerrywang   (501) staff       (20)      318 2023-06-08 16:49:23.000000 apollov2_football_api_parser-0.0.2/src/apollov2_football_api_parser.egg-info/SOURCES.txt
--rw-r--r--   0 jerrywang   (501) staff       (20)        1 2023-06-08 16:49:23.000000 apollov2_football_api_parser-0.0.2/src/apollov2_football_api_parser.egg-info/dependency_links.txt
--rw-r--r--   0 jerrywang   (501) staff       (20)        9 2023-06-08 16:49:23.000000 apollov2_football_api_parser-0.0.2/src/apollov2_football_api_parser.egg-info/top_level.txt
+drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 17:11:41.645495 apollov2_football_api_parser-0.0.3/
+-rw-r--r--   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:25:55.000000 apollov2_football_api_parser-0.0.3/LICENSE
+-rw-r--r--   0 jerrywang   (501) staff       (20)      912 2023-06-08 17:11:41.645599 apollov2_football_api_parser-0.0.3/PKG-INFO
+-rw-r--r--   0 jerrywang   (501) staff       (20)      528 2023-06-08 16:30:33.000000 apollov2_football_api_parser-0.0.3/README.md
+-rw-r--r--   0 jerrywang   (501) staff       (20)      103 2023-06-08 16:27:29.000000 apollov2_football_api_parser-0.0.3/pyproject.toml
+-rw-r--r--   0 jerrywang   (501) staff       (20)      508 2023-06-08 17:11:41.646559 apollov2_football_api_parser-0.0.3/setup.cfg
+drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 17:11:41.642745 apollov2_football_api_parser-0.0.3/src/
+drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 17:11:41.643659 apollov2_football_api_parser-0.0.3/src/apollov2/
+-rw-r--r--   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:48:32.000000 apollov2_football_api_parser-0.0.3/src/apollov2/__init__.py
+-rw-r--r--   0 jerrywang   (501) staff       (20)    16043 2023-06-08 17:10:56.000000 apollov2_football_api_parser-0.0.3/src/apollov2/api_parser.py
+drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 17:11:41.645059 apollov2_football_api_parser-0.0.3/src/apollov2_football_api_parser.egg-info/
+-rw-r--r--   0 jerrywang   (501) staff       (20)      912 2023-06-08 17:11:41.000000 apollov2_football_api_parser-0.0.3/src/apollov2_football_api_parser.egg-info/PKG-INFO
+-rw-r--r--   0 jerrywang   (501) staff       (20)      318 2023-06-08 17:11:41.000000 apollov2_football_api_parser-0.0.3/src/apollov2_football_api_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 jerrywang   (501) staff       (20)        1 2023-06-08 17:11:41.000000 apollov2_football_api_parser-0.0.3/src/apollov2_football_api_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 jerrywang   (501) staff       (20)        9 2023-06-08 17:11:41.000000 apollov2_football_api_parser-0.0.3/src/apollov2_football_api_parser.egg-info/top_level.txt
```

### Comparing `apollov2_football_api_parser-0.0.2/PKG-INFO` & `apollov2_football_api_parser-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollov2_football_api_parser
-Version: 0.0.2
+Version: 0.0.3
 Summary: extract data from api and transform it into dataframe
 Author: zhe wang
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `apollov2_football_api_parser-0.0.2/README.md` & `apollov2_football_api_parser-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `apollov2_football_api_parser-0.0.2/src/apollov2/api_parser.py` & `apollov2_football_api_parser-0.0.3/src/apollov2/api_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,16 +243,17 @@
         progress_bar.close()
 
         df_injuries = pd.concat(frames).reset_index(drop=True)
 
         return df_injuries
 
     def get_all_transfers(self, players_list):
+        ''' df_all_players = parser.get_all_players()
+            players_list = df_all_players['id'].unique().tolist()'''
         frames = []
-
         # Create a progress bar
         progress_bar = tqdm(players_list, desc="Processing players")
 
         for player_id in progress_bar:
             url = "https://api-football-v1.p.rapidapi.com/v3/transfers"
             querystring = {"player": str(player_id)}
 
@@ -282,15 +283,15 @@
                       "season": season, "page": str(page_number)}
             response = self.session.get(
                 'https://api-football-v1.p.rapidapi.com/v3/players', params=params)
             return pd.DataFrame(response.json()['response']) if response.status_code == 200 else None
 
         self.session = requests.Session()
         self.session.headers.update({
-            "X-RapidAPI-Key": api_key,
+            "X-RapidAPI-Key": self.api_key,
             "X-RapidAPI-Host": "api-football-v1.p.rapidapi.com"
         })
         player_frames = []
         for season in self.season_list:
             params = {"league": self.league_id, "season": season, "page": "1"}
             total_pages = self.session.get(
                 'https://api-football-v1.p.rapidapi.com/v3/players', params=params).json()['paging']['total']
@@ -320,15 +321,15 @@
 
         return final_df
 
     def get_all_sidelined(self, players_list):
         frames = []
         session = requests.Session()
         session.headers.update({
-            "X-RapidAPI-Key": api_key,
+            "X-RapidAPI-Key": self.api_key,
             "X-RapidAPI-Host": "api-football-v1.p.rapidapi.com"
         })
 
         for i in tqdm(players_list, desc="Processing players"):
             try:
                 response = session.get(
                     "https://api-football-v1.p.rapidapi.com/v3/sidelined", params={"player": str(i)})
```

### Comparing `apollov2_football_api_parser-0.0.2/src/apollov2_football_api_parser.egg-info/PKG-INFO` & `apollov2_football_api_parser-0.0.3/src/apollov2_football_api_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollov2-football-api-parser
-Version: 0.0.2
+Version: 0.0.3
 Summary: extract data from api and transform it into dataframe
 Author: zhe wang
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

