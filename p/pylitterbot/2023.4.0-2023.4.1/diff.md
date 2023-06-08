# Comparing `tmp/pylitterbot-2023.4.0.tar.gz` & `tmp/pylitterbot-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylitterbot-2023.4.0.tar", max compression
+gzip compressed data, was "pylitterbot-2023.4.1.tar", max compression
```

## Comparing `pylitterbot-2023.4.0.tar` & `pylitterbot-2023.4.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1076 2022-12-07 17:50:03.192551 pylitterbot-2023.4.0/LICENSE
--rw-r--r--   0        0        0     3168 2023-04-20 15:27:40.760888 pylitterbot-2023.4.0/README.md
--rw-r--r--   0        0        0      403 2023-04-20 15:28:39.998601 pylitterbot-2023.4.0/pylitterbot/__init__.py
--rw-r--r--   0        0        0     7546 2023-01-19 22:33:35.031260 pylitterbot-2023.4.0/pylitterbot/account.py
--rw-r--r--   0        0        0     1118 2022-12-07 18:02:31.737246 pylitterbot-2023.4.0/pylitterbot/activity.py
--rw-r--r--   0        0        0     4597 2023-01-19 22:33:35.031445 pylitterbot-2023.4.0/pylitterbot/enums.py
--rw-r--r--   0        0        0      348 2023-01-20 18:04:12.653826 pylitterbot-2023.4.0/pylitterbot/exceptions.py
--rw-r--r--   0        0        0        0 2022-12-07 17:50:03.196040 pylitterbot-2023.4.0/pylitterbot/py.typed
--rw-r--r--   0        0        0     6838 2023-01-09 02:35:41.467367 pylitterbot-2023.4.0/pylitterbot/robot/__init__.py
--rw-r--r--   0        0        0    10446 2023-04-20 15:27:40.762530 pylitterbot-2023.4.0/pylitterbot/robot/feederrobot.py
--rw-r--r--   0        0        0     7187 2023-01-19 22:33:35.031678 pylitterbot-2023.4.0/pylitterbot/robot/litterrobot.py
--rw-r--r--   0        0        0    11704 2023-01-19 22:33:35.031877 pylitterbot-2023.4.0/pylitterbot/robot/litterrobot3.py
--rw-r--r--   0        0        0    25329 2023-04-20 15:27:40.762808 pylitterbot-2023.4.0/pylitterbot/robot/litterrobot4.py
--rw-r--r--   0        0        0     2364 2023-01-19 22:33:35.032287 pylitterbot-2023.4.0/pylitterbot/robot/models.py
--rw-r--r--   0        0        0     7738 2022-12-07 18:02:31.739910 pylitterbot-2023.4.0/pylitterbot/session.py
--rw-r--r--   0        0        0     2545 2023-01-19 22:33:35.032462 pylitterbot-2023.4.0/pylitterbot/utils.py
--rw-r--r--   0        0        0     5148 2023-01-09 02:35:41.468325 pylitterbot-2023.4.0/pylitterbot/ws_monitor.py
--rw-r--r--   0        0        0     1027 2023-04-20 15:28:39.998966 pylitterbot-2023.4.0/pyproject.toml
--rw-r--r--   0        0        0     4189 1970-01-01 00:00:00.000000 pylitterbot-2023.4.0/setup.py
--rw-r--r--   0        0        0     4138 1970-01-01 00:00:00.000000 pylitterbot-2023.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-08 19:24:00.692748 pylitterbot-2023.4.1/LICENSE
+-rw-r--r--   0        0        0     3168 2023-06-08 19:24:00.692748 pylitterbot-2023.4.1/README.md
+-rw-r--r--   0        0        0      403 2023-06-08 19:24:18.749018 pylitterbot-2023.4.1/pylitterbot/__init__.py
+-rw-r--r--   0        0        0     7546 2023-06-08 19:24:00.696748 pylitterbot-2023.4.1/pylitterbot/account.py
+-rw-r--r--   0        0        0     1118 2023-06-08 19:24:00.696748 pylitterbot-2023.4.1/pylitterbot/activity.py
+-rw-r--r--   0        0        0     4597 2023-06-08 19:24:00.696748 pylitterbot-2023.4.1/pylitterbot/enums.py
+-rw-r--r--   0        0        0      348 2023-06-08 19:24:00.696748 pylitterbot-2023.4.1/pylitterbot/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:24:00.696748 pylitterbot-2023.4.1/pylitterbot/py.typed
+-rw-r--r--   0        0        0     6838 2023-06-08 19:24:00.696748 pylitterbot-2023.4.1/pylitterbot/robot/__init__.py
+-rw-r--r--   0        0        0    10446 2023-06-08 19:24:00.696748 pylitterbot-2023.4.1/pylitterbot/robot/feederrobot.py
+-rw-r--r--   0        0        0     7187 2023-06-08 19:24:00.696748 pylitterbot-2023.4.1/pylitterbot/robot/litterrobot.py
+-rw-r--r--   0        0        0    11704 2023-06-08 19:24:00.696748 pylitterbot-2023.4.1/pylitterbot/robot/litterrobot3.py
+-rw-r--r--   0        0        0    25443 2023-06-08 19:24:00.696748 pylitterbot-2023.4.1/pylitterbot/robot/litterrobot4.py
+-rw-r--r--   0        0        0     2364 2023-06-08 19:24:00.696748 pylitterbot-2023.4.1/pylitterbot/robot/models.py
+-rw-r--r--   0        0        0     7874 2023-06-08 19:24:00.696748 pylitterbot-2023.4.1/pylitterbot/session.py
+-rw-r--r--   0        0        0     2545 2023-06-08 19:24:00.696748 pylitterbot-2023.4.1/pylitterbot/utils.py
+-rw-r--r--   0        0        0     5148 2023-06-08 19:24:00.696748 pylitterbot-2023.4.1/pylitterbot/ws_monitor.py
+-rw-r--r--   0        0        0     1154 2023-06-08 19:24:18.749018 pylitterbot-2023.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 pylitterbot-2023.4.1/PKG-INFO
```

### Comparing `pylitterbot-2023.4.0/LICENSE` & `pylitterbot-2023.4.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020-2022 Nathan Spencer
+Copyright (c) 2020-2023 Nathan Spencer
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pylitterbot-2023.4.0/README.md` & `pylitterbot-2023.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.0/pylitterbot/account.py` & `pylitterbot-2023.4.1/pylitterbot/account.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.0/pylitterbot/activity.py` & `pylitterbot-2023.4.1/pylitterbot/activity.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.0/pylitterbot/enums.py` & `pylitterbot-2023.4.1/pylitterbot/enums.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.0/pylitterbot/robot/__init__.py` & `pylitterbot-2023.4.1/pylitterbot/robot/__init__.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.0/pylitterbot/robot/feederrobot.py` & `pylitterbot-2023.4.1/pylitterbot/robot/feederrobot.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.0/pylitterbot/robot/litterrobot.py` & `pylitterbot-2023.4.1/pylitterbot/robot/litterrobot.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.0/pylitterbot/robot/litterrobot3.py` & `pylitterbot-2023.4.1/pylitterbot/robot/litterrobot3.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.0/pylitterbot/robot/litterrobot4.py` & `pylitterbot-2023.4.1/pylitterbot/robot/litterrobot4.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,14 +461,16 @@
                     "serial": self.serial,
                     "limit": limit,
                     "consumer": "app",
                 },
             }
         )
         activities = cast(dict, data).get("data", {}).get("getLitterRobot4Activity", {})
+        if activities is None:
+            raise LitterRobotException("Activity history could not be retrieved.")
         return [
             Activity(timestamp, self._parse_activity(activity))
             for activity in activities
             if (timestamp := to_timestamp(activity["timestamp"])) is not None
         ]
 
     async def get_insight(
```

### Comparing `pylitterbot-2023.4.0/pylitterbot/robot/models.py` & `pylitterbot-2023.4.1/pylitterbot/robot/models.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.0/pylitterbot/session.py` & `pylitterbot-2023.4.1/pylitterbot/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
             return None
         return f"Bearer {access_token}"
 
     async def request(
         self, method: str, url: str, **kwargs: Any
     ) -> dict | list[dict] | None:
         """Make a request."""
+        _LOGGER.debug("Making %s request to %s", method, url)
+
         if "headers" not in kwargs:
             kwargs["headers"] = {}
 
         if (authorization := await self.get_bearer_authorization()) is not None:
             kwargs["headers"]["authorization"] = authorization
 
         async with self.websession.request(method, url, **kwargs) as resp:
@@ -95,14 +97,15 @@
                         ),
                         expires - now,
                     )
                 _LOGGER.error("Unauthorized")
 
             resp.raise_for_status()
             data = await resp.json()
+            _LOGGER.debug("Received %s response: %s", resp.status, data)
             return data  # type: ignore
 
     async def __aenter__(self: T) -> T:
         """Async enter."""
         return self
 
     async def __aexit__(
```

### Comparing `pylitterbot-2023.4.0/pylitterbot/utils.py` & `pylitterbot-2023.4.1/pylitterbot/utils.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.0/pylitterbot/ws_monitor.py` & `pylitterbot-2023.4.1/pylitterbot/ws_monitor.py`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.0/setup.py` & `pylitterbot-2023.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,131 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pylitterbot
+Version: 2023.4.1
+Summary: Python package for controlling Whisker automatic robots.
+Home-page: https://github.com/natekspencer/pylitterbot
+License: MIT
+Keywords: Whisker,Litter-Robot,Feeder-Robot,litter box,pet feeder,asynchronous
+Author: Nathan Spencer
+Author-email: natekspencer@gmail.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyJWT (>=2.7.0,<3.0.0)
+Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
+Requires-Dist: backports.zoneinfo (>=0.2.1,<0.3.0) ; python_version < "3.9"
+Requires-Dist: deepdiff (>=6.2.1,<7.0.0)
+Project-URL: Repository, https://github.com/natekspencer/pylitterbot
+Description-Content-Type: text/markdown
 
-packages = \
-['pylitterbot', 'pylitterbot.robot']
+[![pypi](https://img.shields.io/pypi/v/pylitterbot?style=for-the-badge)](https://pypi.org/project/pylitterbot)
+[![downloads](https://img.shields.io/pypi/dm/pylitterbot?style=for-the-badge)](https://pypi.org/project/pylitterbot)
+[![Buy Me A Coffee/Beer](https://img.shields.io/badge/Buy_Me_A_☕/🍺-F16061?style=for-the-badge&logo=ko-fi&logoColor=white&labelColor=grey)](https://ko-fi.com/natekspencer)
+[![Purchase Litter-Robot](https://img.shields.io/badge/Buy_a_Litter--Robot-Save_$25-lightgrey?style=for-the-badge&labelColor=grey)](https://www.gopjn.com/t/SENKTktMR0lDSEtJTklPQ0hKS05HTQ)
 
-package_data = \
-{'': ['*']}
+# pylitterbot
 
-install_requires = \
-['PyJWT>=2.4.0,<3.0.0', 'aiohttp>=3.8.1,<4.0.0', 'deepdiff>=6.2.1,<7.0.0']
-
-extras_require = \
-{':python_version < "3.9"': ['backports.zoneinfo>=0.2.1,<0.3.0']}
-
-setup_kwargs = {
-    'name': 'pylitterbot',
-    'version': '2023.4.0',
-    'description': 'Python package for controlling Whisker automatic robots.',
-    'long_description': '[![pypi](https://img.shields.io/pypi/v/pylitterbot?style=for-the-badge)](https://pypi.org/project/pylitterbot)\n[![downloads](https://img.shields.io/pypi/dm/pylitterbot?style=for-the-badge)](https://pypi.org/project/pylitterbot)\n[![Buy Me A Coffee/Beer](https://img.shields.io/badge/Buy_Me_A_☕/🍺-F16061?style=for-the-badge&logo=ko-fi&logoColor=white&labelColor=grey)](https://ko-fi.com/natekspencer)\n[![Purchase Litter-Robot](https://img.shields.io/badge/Buy_a_Litter--Robot-Save_$25-lightgrey?style=for-the-badge&labelColor=grey)](https://www.gopjn.com/t/SENKTktMR0lDSEtJTklPQ0hKS05HTQ)\n\n# pylitterbot\n\nPython package for controlling Whisker connected self-cleaning litter boxes and feeders.\n\nThis is an unofficial API for controlling various Whisker automated robots. It currently supports Litter-Robot 3 (with connect), Litter-Robot 4 and Feeder-Robot.\n\n## Disclaimer\n\nThis API is experimental and was reverse-engineered by monitoring network traffic and decompiling source code from the Whisker app since no public API is currently available at this time. It may cease to work at any time. Use at your own risk.\n\n## Installation\n\nInstall using pip\n\n```bash\npip install pylitterbot\n```\n\nAlternatively, clone the repository and run\n\n```bash\npoetry install\n```\n\n## Usage\n\n```python\nimport asyncio\n\nfrom pylitterbot import Account\n\n# Set email and password for initial authentication.\nusername = "Your username"\npassword = "Your password"\n\n\nasync def main():\n    # Create an account.\n    account = Account()\n\n    try:\n        # Connect to the API and load robots.\n        await account.connect(username=username, password=password, load_robots=True)\n\n        # Print robots associated with account.\n        print("Robots:")\n        for robot in account.robots:\n            print(robot)\n    finally:\n        # Disconnect from the API.\n        await account.disconnect()\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nwhich will output something like:\n\n```\nName: Litter-Robot Name, Serial: LR3C012345, id: a0123b4567cd8e\n```\n\nTo start a clean cycle\n\n```python\nawait robot.start_cleaning()\n```\n\nIf no exception occurred, your Litter-Robot should now perform a clean cycle.\n\nCurrently the following methods are available in the Robot class:\n\n- refresh()\n- start_cleaning()\n- reset_settings()\n- set_panel_lockout()\n- set_night_light()\n- set_power_status()\n- set_sleep_mode()\n- set_wait_time()\n- set_name()\n- get_activity_history()\n- get_insight()\n\n---\n\n## TODO\n\n- Improve support for Litter-Robot 4\n- Improve support for Feeder-Robot\n\n---\n\n## Support Me\n\nI\'m not employed by Whisker and provide this python package as-is.\n\nIf you don\'t already own a Litter-Robot, please consider using [my affiliate link](https://www.gopjn.com/t/SENKTktMR0lDSEtJTklPQ0hKS05HTQ) to purchase your own robot and save $25!\n\nIf you already own a Litter-Robot and/or want to donate to me directly, consider buying me a coffee (or beer) instead by using the link below:\n\n<a href=\'https://ko-fi.com/natekspencer\' target=\'_blank\'><img height=\'35\' style=\'border:0px;height:46px;\' src=\'https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0\' border=\'0\' alt=\'Buy Me a Coffee at ko-fi.com\' />\n',
-    'author': 'Nathan Spencer',
-    'author_email': 'natekspencer@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/natekspencer/pylitterbot',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7.2,<4.0.0',
-}
+Python package for controlling Whisker connected self-cleaning litter boxes and feeders.
 
+This is an unofficial API for controlling various Whisker automated robots. It currently supports Litter-Robot 3 (with connect), Litter-Robot 4 and Feeder-Robot.
+
+## Disclaimer
+
+This API is experimental and was reverse-engineered by monitoring network traffic and decompiling source code from the Whisker app since no public API is currently available at this time. It may cease to work at any time. Use at your own risk.
+
+## Installation
+
+Install using pip
+
+```bash
+pip install pylitterbot
+```
+
+Alternatively, clone the repository and run
+
+```bash
+poetry install
+```
+
+## Usage
+
+```python
+import asyncio
+
+from pylitterbot import Account
+
+# Set email and password for initial authentication.
+username = "Your username"
+password = "Your password"
+
+
+async def main():
+    # Create an account.
+    account = Account()
+
+    try:
+        # Connect to the API and load robots.
+        await account.connect(username=username, password=password, load_robots=True)
+
+        # Print robots associated with account.
+        print("Robots:")
+        for robot in account.robots:
+            print(robot)
+    finally:
+        # Disconnect from the API.
+        await account.disconnect()
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+which will output something like:
+
+```
+Name: Litter-Robot Name, Serial: LR3C012345, id: a0123b4567cd8e
+```
+
+To start a clean cycle
+
+```python
+await robot.start_cleaning()
+```
+
+If no exception occurred, your Litter-Robot should now perform a clean cycle.
+
+Currently the following methods are available in the Robot class:
+
+- refresh()
+- start_cleaning()
+- reset_settings()
+- set_panel_lockout()
+- set_night_light()
+- set_power_status()
+- set_sleep_mode()
+- set_wait_time()
+- set_name()
+- get_activity_history()
+- get_insight()
+
+---
+
+## TODO
+
+- Improve support for Litter-Robot 4
+- Improve support for Feeder-Robot
+
+---
+
+## Support Me
+
+I'm not employed by Whisker and provide this python package as-is.
+
+If you don't already own a Litter-Robot, please consider using [my affiliate link](https://www.gopjn.com/t/SENKTktMR0lDSEtJTklPQ0hKS05HTQ) to purchase your own robot and save $25!
+
+If you already own a Litter-Robot and/or want to donate to me directly, consider buying me a coffee (or beer) instead by using the link below:
+
+<a href='https://ko-fi.com/natekspencer' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com' />
 
-setup(**setup_kwargs)
```

