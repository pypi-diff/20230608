# Comparing `tmp/kingspan_connect_sensor-2.1.1.tar.gz` & `tmp/kingspan_connect_sensor-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingspan_connect_sensor-2.1.1.tar", max compression
+gzip compressed data, was "kingspan_connect_sensor-3.0.0.tar", max compression
```

## Comparing `kingspan_connect_sensor-2.1.1.tar` & `kingspan_connect_sensor-3.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1078 2022-11-19 09:25:30.276140 kingspan_connect_sensor-2.1.1/LICENSE
--rw-r--r--   0        0        0     3604 2022-11-26 11:07:29.414711 kingspan_connect_sensor-2.1.1/README.md
--rw-r--r--   0        0        0     2285 2023-05-05 08:22:02.083484 kingspan_connect_sensor-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      190 2022-11-24 19:10:40.355078 kingspan_connect_sensor-2.1.1/src/connectsensor/__init__.py
--rw-r--r--   0        0        0     3542 2022-11-26 08:54:31.150331 kingspan_connect_sensor-2.1.1/src/connectsensor/_kingspan_export.py
--rw-r--r--   0        0        0     5722 2022-11-26 10:59:27.697337 kingspan_connect_sensor-2.1.1/src/connectsensor/_kingspan_notifier.py
--rw-r--r--   0        0        0     1816 2023-02-26 17:41:22.129396 kingspan_connect_sensor-2.1.1/src/connectsensor/_kingspan_status.py
--rw-r--r--   0        0        0     4488 2022-11-24 19:48:32.745484 kingspan_connect_sensor-2.1.1/src/connectsensor/client.py
--rw-r--r--   0        0        0      545 2021-01-30 15:44:34.000000 kingspan_connect_sensor-2.1.1/src/connectsensor/debug.py
--rw-r--r--   0        0        0      200 2022-11-24 13:07:58.577473 kingspan_connect_sensor-2.1.1/src/connectsensor/exceptions.py
--rw-r--r--   0        0        0     3551 2022-12-11 15:27:42.709954 kingspan_connect_sensor-2.1.1/src/connectsensor/tank.py
--rw-r--r--   0        0        0     4885 1970-01-01 00:00:00.000000 kingspan_connect_sensor-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-11-19 09:25:30.276140 kingspan_connect_sensor-3.0.0/LICENSE
+-rw-r--r--   0        0        0     4033 2023-06-08 09:19:57.908283 kingspan_connect_sensor-3.0.0/README.md
+-rw-r--r--   0        0        0     2187 2023-06-08 09:05:24.106065 kingspan_connect_sensor-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      190 2022-11-24 19:10:40.355078 kingspan_connect_sensor-3.0.0/src/connectsensor/__init__.py
+-rw-r--r--   0        0        0     3570 2023-06-08 09:08:11.851107 kingspan_connect_sensor-3.0.0/src/connectsensor/_kingspan_export.py
+-rw-r--r--   0        0        0     5736 2023-06-08 09:17:59.368334 kingspan_connect_sensor-3.0.0/src/connectsensor/_kingspan_notifier.py
+-rw-r--r--   0        0        0     1825 2023-06-08 09:21:14.131699 kingspan_connect_sensor-3.0.0/src/connectsensor/_kingspan_status.py
+-rw-r--r--   0        0        0     4488 2022-11-24 19:48:32.745484 kingspan_connect_sensor-3.0.0/src/connectsensor/client.py
+-rw-r--r--   0        0        0      545 2021-01-30 15:44:34.000000 kingspan_connect_sensor-3.0.0/src/connectsensor/debug.py
+-rw-r--r--   0        0        0      200 2022-11-24 13:07:58.577473 kingspan_connect_sensor-3.0.0/src/connectsensor/exceptions.py
+-rw-r--r--   0        0        0     3592 2023-06-08 08:37:38.261232 kingspan_connect_sensor-3.0.0/src/connectsensor/tank.py
+-rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 kingspan_connect_sensor-3.0.0/PKG-INFO
```

### Comparing `kingspan_connect_sensor-2.1.1/LICENSE` & `kingspan_connect_sensor-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-2.1.1/README.md` & `kingspan_connect_sensor-3.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,20 +43,28 @@
     tank_capcity = await tanks[0].capacity
     tank_percent = 100 * (tank_level / tank_percent)
     print(f"Tank is {tank_percent:.1f}% full")
 ```
 
 ## Tanks object
 
-`history` returns a Pandas dataframe with all entries available from the web API, sorted by logging time. There should be one record per day. The dataframe has the following entries:
+As of version 3.0, `history` no longer returns a Pandas dataframe to simplify packge dependencies. Instead, an list of dicts is returned, where each list element is a sample from the web API, sorted by logging time. There should be one record per day. Each dict has the following keys:
 
 * `reading_date`: a datetime object indicating the time a measurement was made
 * `level_percent`: integer percentage full
 * `level_litres`: number of lites in the tank
 
+You can construct a Pandas dataframe simply using:
+
+``` python
+tanks = await client.tanks
+history = await tanks[0].history
+df = pd.DataFrame(history)
+```
+
 ## Scripts
 
 Reporting on the current status of the tank using `kingspan-status`:
 
 ``` bash
 % kingspan-status --username=test@example.com --password=s3cret
 
@@ -71,15 +79,15 @@
  Reading date           %Full  Litres
  30-Jan-2021 00:29      94     1224 
  31-Jan-2021 00:59      80     1040 
  01-Feb-2021 00:29      78     1008 
  02-Feb-2021 00:59      76     986  
 ```
 
-`kingspan-notifier` can be used to check the status of a tabk and report via email when the tank is likely to run out of oil.
+`kingspan-notifier` can be used to check the status of a tabk and report via email when the tank is likely to run out of oil. As of version 3.0, [pandas](https://pypi.org/project/pandas/) is no longer installed as a dependency so you must `pip install pandas` manually to use `kingspan-notifier`.
 
 ``` bash
 % kingspan-notifier --config kingspan.ini
 Current level 1148 litres
 No notification; 196 days oil remain
 ```
```

### Comparing `kingspan_connect_sensor-2.1.1/pyproject.toml` & `kingspan_connect_sensor-3.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -11,32 +11,30 @@
 description = "API to get oil tank from Kingspan SENSiT sensors"
 documentation = "https://github.com/masaccio/kingspan-connect-sensor/blob/main/README.md"
 license = "MIT"
 name = "kingspan-connect-sensor"
 packages = [{include = "connectsensor", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/masaccio/kingspan-connect-sensor"
-version = "2.1.1"
+version = "3.0.0"
 
 [tool.poetry.dependencies]
 async-property = "^0.2.1"
 asyncio = "^3.4.3"
 datetime = "^4.7"
-# homeassistant has a constraint on httpx==0.24
 httpx = "^0.24"
-# homeassistant has a constraint on pandas==1.4.3
-pandas = "^1.4.3"
 python = "^3.9"
 requests = "^2.28.1"
 zeep = "^4.2.0"
 
 [tool.poetry.group.dev.dependencies]
 aiofiles = "^22.1.0"
 black = {version = "^22.10.0", allow-prereleases = true}
 openpyxl = "^3.0.10"
+pandas = "^1.4.3"
 pytest = "^7.1.0"
 pytest-asyncio = "^0.20.2"
 pytest-console-scripts = "^1.3.1"
 pytest-cov = "^3.0.0"
 xlsxwriter = "^3.0.3"
 
 [build-system]
```

### Comparing `kingspan_connect_sensor-2.1.1/src/connectsensor/_kingspan_export.py` & `kingspan_connect_sensor-3.0.0/src/connectsensor/_kingspan_export.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,18 +46,18 @@
         cursor = db.cursor()
     except sqlite3.Error as e:
         raise DBError(f"{cache_db}: connection failed") from e
 
     if table_exists(cursor):
         query = "SELECT * FROM history;"
         old_history = pd.read_sql_query(query, db, parse_dates=["reading_date"])
-        new_history = tank.history
+        new_history = pd.DataFrame(tank.history)
         history = pd.concat([old_history, new_history]).drop_duplicates()
     else:
-        history = tank.history
+        history = pd.DataFrame(tank.history)
 
     if update:
         history.to_sql("history", db, if_exists="replace", index=False)
 
     cursor.close()
     db.close()
```

### Comparing `kingspan_connect_sensor-2.1.1/src/connectsensor/_kingspan_notifier.py` & `kingspan_connect_sensor-3.0.0/src/connectsensor/_kingspan_notifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 "Authentication Failed: invalid username or password", file=sys.stderr
             )
         else:  # pragma: no cover
             print("Unknown API error:", e.value, file=sys.stderr)
         sys.exit(1)
 
     tanks = client.tanks
-    return tanks[0].history
+    return pd.DataFrame(tanks[0].history)
 
 
 def update_tank_cache(config, history, update=False):
     cache_db = config.get("sensit", "cache", fallback=None)
     cache_db = os.path.expanduser(cache_db)
     if cache_db is None:
         return
```

### Comparing `kingspan_connect_sensor-2.1.1/src/connectsensor/_kingspan_status.py` & `kingspan_connect_sensor-3.0.0/src/connectsensor/_kingspan_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,20 +38,20 @@
         print(f"\tSerial Number = {tank.serial_number}")
         print(f"\tModel = {tank.model}")
         print(f"\tLevel = {tank_level_percent}% ({tank.level} litres)")
         print(f"\tLast Read = {tank.last_read}")
 
         print("\nHistory:")
         print("\t{0:<22} {1:<6} {2:<5}".format("Reading date", "%Full", "Litres"))
-        for index, measurement in tank.history.iterrows():
+        for index, measurement in enumerate(tank.history):
             print(
                 "\t{0:<22} {1:<6} {2:<5}".format(
-                    measurement.reading_date.strftime("%d-%b-%Y %H:%M"),
-                    measurement.level_percent,
-                    measurement.level_litres,
+                    measurement["reading_date"].strftime("%d-%b-%Y %H:%M"),
+                    measurement["level_percent"],
+                    measurement["level_litres"],
                 )
             )
 
 
 if __name__ == "__main__":
     # execute only if run as a script
     main()
```

### Comparing `kingspan_connect_sensor-2.1.1/src/connectsensor/client.py` & `kingspan_connect_sensor-3.0.0/src/connectsensor/client.py`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-2.1.1/src/connectsensor/debug.py` & `kingspan_connect_sensor-3.0.0/src/connectsensor/debug.py`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-2.1.1/src/connectsensor/tank.py` & `kingspan_connect_sensor-3.0.0/src/connectsensor/tank.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         """Return the last read date of the tank as a datetime object"""
         self._cache_tank_data()
         return self._level_data["ReadingDate"]
 
     @property
     def history(self):
         history_data = self._soap_client._get_history(self._signalman_no)
-        return history_to_df(history_data)
+        return transform_history_data(history_data)
 
     def _cache_tank_data(self):
         if self._level_data is None:
             response = self._soap_client._get_latest_level(self._signalman_no)
             unpack_tank_data(self, response)
 
 
@@ -90,26 +90,31 @@
         """Return the last read date of the tank as a datetime object"""
         await self._cache_tank_data()
         return self._level_data["ReadingDate"]
 
     @async_property
     async def history(self):
         history_data = await self._soap_client._get_history(self._signalman_no)
-        return history_to_df(history_data)
+        return transform_history_data(history_data)
 
     async def _cache_tank_data(self):
         if self._level_data is None:
             response = await self._soap_client._get_latest_level(self._signalman_no)
             unpack_tank_data(self, response)
 
 
 def unpack_tank_data(cls, response):
     cls._level_data = serialize_object(response["Level"])
     tank_info = serialize_object(response["TankInfo"])
     cls._tank_info = {x["Name"]: x["Value"] for x in tank_info["APITankInfoItem"]}
 
 
-def history_to_df(history_data):
-    df = pd.DataFrame(serialize_object(history_data))
-    df = df[["ReadingDate", "LevelPercentage", "LevelLitres"]]
-    df.columns = ["reading_date", "level_percent", "level_litres"]
-    return df
+def transform_history_data(data):
+    data = [
+        {
+            "reading_date": x["ReadingDate"],
+            "level_percent": x["LevelPercentage"],
+            "level_litres": x["LevelLitres"],
+        }
+        for x in data
+    ]
+    return data
```

### Comparing `kingspan_connect_sensor-2.1.1/PKG-INFO` & `kingspan_connect_sensor-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingspan-connect-sensor
-Version: 2.1.1
+Version: 3.0.0
 Summary: API to get oil tank from Kingspan SENSiT sensors
 Home-page: https://github.com/masaccio/kingspan-connect-sensor
 License: MIT
 Author: Jon Connell
 Author-email: python@figsandfudge.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: async-property (>=0.2.1,<0.3.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: datetime (>=4.7,<5.0)
 Requires-Dist: httpx (>=0.24,<0.25)
-Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: zeep (>=4.2.0,<5.0.0)
 Project-URL: Documentation, https://github.com/masaccio/kingspan-connect-sensor/blob/main/README.md
 Project-URL: Repository, https://github.com/masaccio/kingspan-connect-sensor
 Description-Content-Type: text/markdown
 
 # kingspan-connect-sensor
@@ -73,20 +72,28 @@
     tank_capcity = await tanks[0].capacity
     tank_percent = 100 * (tank_level / tank_percent)
     print(f"Tank is {tank_percent:.1f}% full")
 ```
 
 ## Tanks object
 
-`history` returns a Pandas dataframe with all entries available from the web API, sorted by logging time. There should be one record per day. The dataframe has the following entries:
+As of version 3.0, `history` no longer returns a Pandas dataframe to simplify packge dependencies. Instead, an list of dicts is returned, where each list element is a sample from the web API, sorted by logging time. There should be one record per day. Each dict has the following keys:
 
 * `reading_date`: a datetime object indicating the time a measurement was made
 * `level_percent`: integer percentage full
 * `level_litres`: number of lites in the tank
 
+You can construct a Pandas dataframe simply using:
+
+``` python
+tanks = await client.tanks
+history = await tanks[0].history
+df = pd.DataFrame(history)
+```
+
 ## Scripts
 
 Reporting on the current status of the tank using `kingspan-status`:
 
 ``` bash
 % kingspan-status --username=test@example.com --password=s3cret
 
@@ -101,15 +108,15 @@
  Reading date           %Full  Litres
  30-Jan-2021 00:29      94     1224 
  31-Jan-2021 00:59      80     1040 
  01-Feb-2021 00:29      78     1008 
  02-Feb-2021 00:59      76     986  
 ```
 
-`kingspan-notifier` can be used to check the status of a tabk and report via email when the tank is likely to run out of oil.
+`kingspan-notifier` can be used to check the status of a tabk and report via email when the tank is likely to run out of oil. As of version 3.0, [pandas](https://pypi.org/project/pandas/) is no longer installed as a dependency so you must `pip install pandas` manually to use `kingspan-notifier`.
 
 ``` bash
 % kingspan-notifier --config kingspan.ini
 Current level 1148 litres
 No notification; 196 days oil remain
 ```
```

