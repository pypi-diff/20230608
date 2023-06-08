# Comparing `tmp/whatsapp-chatbot-python-0.2.1.tar.gz` & `tmp/whatsapp-chatbot-python-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-chatbot-python-0.2.1.tar", last modified: Sun Jun  4 07:05:21 2023, max compression
+gzip compressed data, was "whatsapp-chatbot-python-0.2.2.tar", last modified: Thu Jun  8 08:55:13 2023, max compression
```

## Comparing `whatsapp-chatbot-python-0.2.1.tar` & `whatsapp-chatbot-python-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 07:05:21.641748 whatsapp-chatbot-python-0.2.1/
--rw-rw-rw-   0        0        0    18829 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     8648 2023-06-04 07:05:21.641748 whatsapp-chatbot-python-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     7623 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-04 07:05:21.641748 whatsapp-chatbot-python-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1405 2023-06-04 07:00:41.000000 whatsapp-chatbot-python-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:05:21.630719 whatsapp-chatbot-python-0.2.1/tests/
--rw-rw-rw-   0        0        0     1224 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/tests/test_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:05:21.633727 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/
--rw-rw-rw-   0        0        0      184 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/__init__.py
--rw-rw-rw-   0        0        0     1020 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/bot.py
--rw-rw-rw-   0        0        0     3569 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/filters.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:05:21.640745 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/
--rw-rw-rw-   0        0        0        0 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/__init__.py
--rw-rw-rw-   0        0        0     3277 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/handler.py
--rw-rw-rw-   0        0        0     1821 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/observer.py
--rw-rw-rw-   0        0        0     1144 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/router.py
-drwxrwxrwx   0        0        0        0 2023-06-04 07:05:21.637737 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/
--rw-rw-rw-   0        0        0     8648 2023-06-04 07:05:21.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-06-04 07:05:21.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 07:05:21.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-04 07:05:21.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-04 07:05:21.000000 whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 08:55:13.025522 whatsapp-chatbot-python-0.2.2/
+-rw-rw-rw-   0        0        0    18829 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     9060 2023-06-08 08:55:13.025522 whatsapp-chatbot-python-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8035 2023-06-08 08:50:01.000000 whatsapp-chatbot-python-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 08:55:13.025522 whatsapp-chatbot-python-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1405 2023-06-08 08:51:43.000000 whatsapp-chatbot-python-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:55:13.012488 whatsapp-chatbot-python-0.2.2/tests/
+-rw-rw-rw-   0        0        0     1224 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/tests/test_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:55:13.016498 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/
+-rw-rw-rw-   0        0        0      184 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/__init__.py
+-rw-rw-rw-   0        0        0     1020 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/bot.py
+-rw-rw-rw-   0        0        0     3569 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/filters.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:55:13.023517 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/
+-rw-rw-rw-   0        0        0        0 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/__init__.py
+-rw-rw-rw-   0        0        0     3277 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/handler.py
+-rw-rw-rw-   0        0        0     1821 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/observer.py
+-rw-rw-rw-   0        0        0     1144 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/router.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:55:13.020509 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/
+-rw-rw-rw-   0        0        0     9060 2023-06-08 08:55:12.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-06-08 08:55:13.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 08:55:12.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-08 08:55:12.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-08 08:55:12.000000 whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/top_level.txt
```

### Comparing `whatsapp-chatbot-python-0.2.1/LICENSE` & `whatsapp-chatbot-python-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.1/PKG-INFO` & `whatsapp-chatbot-python-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.2.1
+Version: 0.2.2
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-chatbot-python)
 ![](https://img.shields.io/pypi/pyversions/whatsapp-chatbot-python)
 ![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-chatbot-python/python-package.yml)
 ![](https://img.shields.io/pypi/dm/whatsapp-chatbot-python)
 
-- [Документация на русском языке](docs/README.md).
+- [Документация на русском языке](https://github.com/green-api/whatsapp-chatbot-python/blob/master/docs/README.md).
 
 whatsapp-chatbot-python is a library for integration with WhatsApp messenger using the API
 service [green-api.com](https://green-api.com/en/). You should get a registration token and an account ID in
 your [personal cabinet](https://console.green-api.com/) to use the library. There is a free developer account tariff.
 
 ## API
 
@@ -79,18 +79,18 @@
 
 Next, you need to add the handler function to the list of handlers. This can be done with the `bot.router.message`
 decorator as in the example or with the `bot.router.message.add_handler` function. The decorator must be called with
 brackets.
 
 To start the bot, call the `bot.run_forever` function. You can stop the bot with the key combination Ctrl + C.
 
-Link to example: [base.py](examples/base.py).
+Link to example: [base.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/base.py).
 
 ```
-@bot.router.message()
+@bot.router.message(text_message="message")
 def message_handler(notification: Notification) -> None:
     notification.answer("Hello")
 
 
 bot.run_forever()
 ```
 
@@ -101,15 +101,15 @@
 - To receive outgoing messages, you need to use the `bot.router.outgoing_message` object;
 - To receive outgoing API messages, you need to use the `bot.router.outgoing_api_message` object;
 - To receive the status of sent messages, you need to use the `bot.router.outgoing_message_status` object.
 
 The body of the notification is in `notification.event`. In this example, we get the message type from the notification
 body.
 
-Link to example: [event.py](examples/event.py).
+Link to example: [event.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/event.py).
 
 ```
 @bot.router.message()
 def message_handler(notification: Notification) -> None:
     print(notification.event)
 
 
@@ -182,30 +182,30 @@
 
 ```
 command = ("help", "!/")
 ```
 
 #### Example
 
-Link to example: [filters.py](examples/filters.py).
+Link to example: [filters.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/filters.py).
 
 ```
 @bot.router.message(command="help")
 def message_handler(notification: Notification) -> None:
     notification.answer_with_file(file="help.png")
 
 
 bot.run_forever()
 ```
 
 ### How to handle buttons
 
 To be notified when a button is pressed, you must use the `bot.router.buttons` object.
 
-Link to example: [buttons.py](examples/buttons.py).
+Link to example: [buttons.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/buttons.py).
 
 ```
 @bot.router.buttons()
 def buttons_handler(notification: Notification) -> None:
     notification.answer_buttons("Choose a color", [
         {
             "buttonId": 1,
@@ -230,8 +230,8 @@
 [Service methods documentation](https://green-api.com/en/docs/api/)
 
 ## License
 
 Licensed under [
 Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 ](https://creativecommons.org/licenses/by-nd/4.0/) terms.
-Please see file [LICENSE](LICENSE).
+Please see file [LICENSE](https://github.com/green-api/whatsapp-chatbot-python/blob/master/LICENSE).
```

### Comparing `whatsapp-chatbot-python-0.2.1/README.md` & `whatsapp-chatbot-python-0.2.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-chatbot-python)
 ![](https://img.shields.io/pypi/pyversions/whatsapp-chatbot-python)
 ![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-chatbot-python/python-package.yml)
 ![](https://img.shields.io/pypi/dm/whatsapp-chatbot-python)
 
-- [Документация на русском языке](docs/README.md).
+- [Документация на русском языке](https://github.com/green-api/whatsapp-chatbot-python/blob/master/docs/README.md).
 
 whatsapp-chatbot-python is a library for integration with WhatsApp messenger using the API
 service [green-api.com](https://green-api.com/en/). You should get a registration token and an account ID in
 your [personal cabinet](https://console.green-api.com/) to use the library. There is a free developer account tariff.
 
 ## API
 
@@ -56,18 +56,18 @@
 
 Next, you need to add the handler function to the list of handlers. This can be done with the `bot.router.message`
 decorator as in the example or with the `bot.router.message.add_handler` function. The decorator must be called with
 brackets.
 
 To start the bot, call the `bot.run_forever` function. You can stop the bot with the key combination Ctrl + C.
 
-Link to example: [base.py](examples/base.py).
+Link to example: [base.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/base.py).
 
 ```
-@bot.router.message()
+@bot.router.message(text_message="message")
 def message_handler(notification: Notification) -> None:
     notification.answer("Hello")
 
 
 bot.run_forever()
 ```
 
@@ -78,15 +78,15 @@
 - To receive outgoing messages, you need to use the `bot.router.outgoing_message` object;
 - To receive outgoing API messages, you need to use the `bot.router.outgoing_api_message` object;
 - To receive the status of sent messages, you need to use the `bot.router.outgoing_message_status` object.
 
 The body of the notification is in `notification.event`. In this example, we get the message type from the notification
 body.
 
-Link to example: [event.py](examples/event.py).
+Link to example: [event.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/event.py).
 
 ```
 @bot.router.message()
 def message_handler(notification: Notification) -> None:
     print(notification.event)
 
 
@@ -159,30 +159,30 @@
 
 ```
 command = ("help", "!/")
 ```
 
 #### Example
 
-Link to example: [filters.py](examples/filters.py).
+Link to example: [filters.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/filters.py).
 
 ```
 @bot.router.message(command="help")
 def message_handler(notification: Notification) -> None:
     notification.answer_with_file(file="help.png")
 
 
 bot.run_forever()
 ```
 
 ### How to handle buttons
 
 To be notified when a button is pressed, you must use the `bot.router.buttons` object.
 
-Link to example: [buttons.py](examples/buttons.py).
+Link to example: [buttons.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/buttons.py).
 
 ```
 @bot.router.buttons()
 def buttons_handler(notification: Notification) -> None:
     notification.answer_buttons("Choose a color", [
         {
             "buttonId": 1,
@@ -207,8 +207,8 @@
 [Service methods documentation](https://green-api.com/en/docs/api/)
 
 ## License
 
 Licensed under [
 Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 ](https://creativecommons.org/licenses/by-nd/4.0/) terms.
-Please see file [LICENSE](LICENSE).
+Please see file [LICENSE](https://github.com/green-api/whatsapp-chatbot-python/blob/master/LICENSE).
```

### Comparing `whatsapp-chatbot-python-0.2.1/setup.py` & `whatsapp-chatbot-python-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-chatbot-python",
-    version="0.2.1",
+    version="0.2.2",
     description=(
         "This library helps you easily create"
         " a Python chatbot with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
```

### Comparing `whatsapp-chatbot-python-0.2.1/tests/test_manager.py` & `whatsapp-chatbot-python-0.2.2/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/bot.py` & `whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/bot.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/filters.py` & `whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/filters.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/handler.py` & `whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/handler.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/observer.py` & `whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/observer.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python/manager/router.py` & `whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python/manager/router.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/PKG-INFO` & `whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.2.1
+Version: 0.2.2
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-chatbot-python)
 ![](https://img.shields.io/pypi/pyversions/whatsapp-chatbot-python)
 ![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-chatbot-python/python-package.yml)
 ![](https://img.shields.io/pypi/dm/whatsapp-chatbot-python)
 
-- [Документация на русском языке](docs/README.md).
+- [Документация на русском языке](https://github.com/green-api/whatsapp-chatbot-python/blob/master/docs/README.md).
 
 whatsapp-chatbot-python is a library for integration with WhatsApp messenger using the API
 service [green-api.com](https://green-api.com/en/). You should get a registration token and an account ID in
 your [personal cabinet](https://console.green-api.com/) to use the library. There is a free developer account tariff.
 
 ## API
 
@@ -79,18 +79,18 @@
 
 Next, you need to add the handler function to the list of handlers. This can be done with the `bot.router.message`
 decorator as in the example or with the `bot.router.message.add_handler` function. The decorator must be called with
 brackets.
 
 To start the bot, call the `bot.run_forever` function. You can stop the bot with the key combination Ctrl + C.
 
-Link to example: [base.py](examples/base.py).
+Link to example: [base.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/base.py).
 
 ```
-@bot.router.message()
+@bot.router.message(text_message="message")
 def message_handler(notification: Notification) -> None:
     notification.answer("Hello")
 
 
 bot.run_forever()
 ```
 
@@ -101,15 +101,15 @@
 - To receive outgoing messages, you need to use the `bot.router.outgoing_message` object;
 - To receive outgoing API messages, you need to use the `bot.router.outgoing_api_message` object;
 - To receive the status of sent messages, you need to use the `bot.router.outgoing_message_status` object.
 
 The body of the notification is in `notification.event`. In this example, we get the message type from the notification
 body.
 
-Link to example: [event.py](examples/event.py).
+Link to example: [event.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/event.py).
 
 ```
 @bot.router.message()
 def message_handler(notification: Notification) -> None:
     print(notification.event)
 
 
@@ -182,30 +182,30 @@
 
 ```
 command = ("help", "!/")
 ```
 
 #### Example
 
-Link to example: [filters.py](examples/filters.py).
+Link to example: [filters.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/filters.py).
 
 ```
 @bot.router.message(command="help")
 def message_handler(notification: Notification) -> None:
     notification.answer_with_file(file="help.png")
 
 
 bot.run_forever()
 ```
 
 ### How to handle buttons
 
 To be notified when a button is pressed, you must use the `bot.router.buttons` object.
 
-Link to example: [buttons.py](examples/buttons.py).
+Link to example: [buttons.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/buttons.py).
 
 ```
 @bot.router.buttons()
 def buttons_handler(notification: Notification) -> None:
     notification.answer_buttons("Choose a color", [
         {
             "buttonId": 1,
@@ -230,8 +230,8 @@
 [Service methods documentation](https://green-api.com/en/docs/api/)
 
 ## License
 
 Licensed under [
 Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 ](https://creativecommons.org/licenses/by-nd/4.0/) terms.
-Please see file [LICENSE](LICENSE).
+Please see file [LICENSE](https://github.com/green-api/whatsapp-chatbot-python/blob/master/LICENSE).
```

### Comparing `whatsapp-chatbot-python-0.2.1/whatsapp_chatbot_python.egg-info/SOURCES.txt` & `whatsapp-chatbot-python-0.2.2/whatsapp_chatbot_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

