# Comparing `tmp/async-cb-rate-1.0.0.tar.gz` & `tmp/async-cb-rate-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-cb-rate-1.0.0.tar", last modified: Wed Oct  5 20:13:02 2022, max compression
+gzip compressed data, was "async-cb-rate-1.0.1.tar", last modified: Thu Jun  8 21:48:20 2023, max compression
```

## Comparing `async-cb-rate-1.0.0.tar` & `async-cb-rate-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-10-05 20:13:02.793531 async-cb-rate-1.0.0/
--rw-rw-rw-   0        0        0     3225 2022-10-05 20:13:02.793531 async-cb-rate-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2924 2022-10-05 19:44:46.000000 async-cb-rate-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-10-05 20:13:02.787554 async-cb-rate-1.0.0/async_cb_rate/
--rw-rw-rw-   0        0        0        0 2022-10-01 16:15:27.000000 async-cb-rate-1.0.0/async_cb_rate/__init__.py
--rw-rw-rw-   0        0        0      105 2022-10-05 19:44:46.000000 async-cb-rate-1.0.0/async_cb_rate/errors.py
--rw-rw-rw-   0        0        0      167 2022-10-02 18:27:38.000000 async-cb-rate-1.0.0/async_cb_rate/models.py
--rw-rw-rw-   0        0        0     3397 2022-10-05 19:51:42.000000 async-cb-rate-1.0.0/async_cb_rate/parser.py
-drwxrwxrwx   0        0        0        0 2022-10-05 20:13:02.792532 async-cb-rate-1.0.0/async_cb_rate.egg-info/
--rw-rw-rw-   0        0        0     3225 2022-10-05 20:13:02.000000 async-cb-rate-1.0.0/async_cb_rate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2022-10-05 20:13:02.000000 async-cb-rate-1.0.0/async_cb_rate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-05 20:13:02.000000 async-cb-rate-1.0.0/async_cb_rate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2022-10-05 20:13:02.000000 async-cb-rate-1.0.0/async_cb_rate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-10-05 20:13:02.000000 async-cb-rate-1.0.0/async_cb_rate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-05 20:13:02.794531 async-cb-rate-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      699 2022-10-05 20:12:36.000000 async-cb-rate-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:48:20.402649 async-cb-rate-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-08 21:48:20.402649 async-cb-rate-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-08 21:48:01.000000 async-cb-rate-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:48:20.402649 async-cb-rate-1.0.1/async_cb_rate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 21:48:01.000000 async-cb-rate-1.0.1/async_cb_rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 21:48:01.000000 async-cb-rate-1.0.1/async_cb_rate/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-08 21:48:01.000000 async-cb-rate-1.0.1/async_cb_rate/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-08 21:48:01.000000 async-cb-rate-1.0.1/async_cb_rate/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:48:20.402649 async-cb-rate-1.0.1/async_cb_rate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-08 21:48:20.000000 async-cb-rate-1.0.1/async_cb_rate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-08 21:48:20.000000 async-cb-rate-1.0.1/async_cb_rate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 21:48:20.000000 async-cb-rate-1.0.1/async_cb_rate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 21:48:20.000000 async-cb-rate-1.0.1/async_cb_rate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 21:48:20.000000 async-cb-rate-1.0.1/async_cb_rate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 21:48:20.402649 async-cb-rate-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-08 21:48:01.000000 async-cb-rate-1.0.1/setup.py
```

### Comparing `async-cb-rate-1.0.0/PKG-INFO` & `async-cb-rate-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,53 @@
-Metadata-Version: 2.1
-Name: async-cb-rate
-Version: 1.0.0
-Summary: Package for async parsing CB rates
-Home-page: https://github.com/alenapoliakova/async-cb-rate
-Author: Alena Polyakova
-Author-email: alenapoliakova2003@gmail.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# async-cb-rate
-Асинхронная библиотека для парсинга курса валют с сайта ЦБ РФ.
-
-### Библиотеку можно использовать для:
-- мониторинга за курсом валют
-- построения графиков изменения курса
-
-### Установка c pip
-```shell
-pip install async-cb-rate
-```
-
-### Краткий обзор функциональности
-- Библиотека позволяет получить курс валюты на любой день. По умолчанию курс ищется на сегодняшний день.
-- Функции возвращают объекты `Currency`, с которыми удобно далее работать.
-```python
-import asyncio
-
-from async_cb_rate.parser import get_rate, get_codes, get_all_rates
-
-
-async def main():
-    usd_rate = await get_rate("USD")
-    print(f"USD rate for today={usd_rate.price}₽")  # USD rate for today=55.2987₽
-
-    euro_rate = await get_rate("EUR")  # EUR rate for today=52.7379₽
-    print(f"EUR rate for today={euro_rate.price}₽")
-
-    codes = await get_codes()
-    print(f"Available codes: {codes}") # ['AUD', 'AZN', 'GBP', 'AMD', 'BYN', 'BGN', 'BRL', 'HUF', 'HKD', 'DKK', 'USD', 
-    # 'EUR', 'INR', 'KZT', 'CAD', 'KGS', 'CNY', 'MDL', 'NOK', 'PLN', 'RON', 'XDR', 'SGD', 'TJS', 'TRY', 'TMT', 'UZS', 
-    # 'UAH', 'CZK', 'SEK', 'CHF', 'ZAR', 'KRW', 'JPY']
-
-    all_rates = await get_all_rates()
-    print(f"All rates for today: {all_rates}")  # [Currency(name='Австралийский доллар', code='AUD', price=35.9552, 
-    # date=datetime.datetime(2022, 10, 3, 23, 45, 29, 145779)), ...]
-
-
-asyncio.run(main())
-```
-
-### Доступные асинхронные функции библиотеки:
-- **get_codes(date)** - получить все доступные коды валют на определённую дату:  
-`codes = await get_codes()  # Коды валют`
-- **get_rate(code, date)** - получить курс определённой валюты по её коду на определённую дату:  
-`usd_rate = await get_rate("USD")  # Курс доллара на сегодня`
-- **get_all_rates(date)** - получить курс всех доступных валют от ЦБ на определённую дату:  
-`all_rates = await get_all_rates()  # Все курсы валют на сегодня`  
-! По умолчанию поле date - это сегодня.
-
-### Ошибки, которые можно получить при работе с библиотекой:
-- `NoValidDateError` - функция была вызвана с датой, которая ещё не наступила.
-- `CurrencyRateNotFoundError` - курс для данного кода валюты не найден.
+# async-cb-rate
+Асинхронная библиотека для парсинга курса валют с сайта ЦБ РФ.
+
+### Библиотеку можно использовать для:
+- мониторинга за курсом валют
+- построения графиков изменения курса
+
+### Установка c pip
+```shell
+pip install async-cb-rate
+```
+
+### Краткий обзор функциональности
+- Библиотека позволяет получить курс валюты на любой день. По умолчанию курс ищется на сегодняшний день.
+- Функции возвращают объекты `Currency`, с которыми удобно далее работать.
+```python
+import asyncio
+
+from async_cb_rate.parser import get_rate, get_codes, get_all_rates
+
+
+async def main():
+    usd_rate = await get_rate("USD")
+    print(f"USD rate for today={usd_rate.price}₽")  # USD rate for today=55.2987₽
+
+    euro_rate = await get_rate("EUR")  # EUR rate for today=52.7379₽
+    print(f"EUR rate for today={euro_rate.price}₽")
+
+    codes = await get_codes()
+    print(f"Available codes: {codes}") # ['AUD', 'AZN', 'GBP', 'AMD', 'BYN', 'BGN', 'BRL', 'HUF', 'HKD', 'DKK', 'USD', 
+    # 'EUR', 'INR', 'KZT', 'CAD', 'KGS', 'CNY', 'MDL', 'NOK', 'PLN', 'RON', 'XDR', 'SGD', 'TJS', 'TRY', 'TMT', 'UZS', 
+    # 'UAH', 'CZK', 'SEK', 'CHF', 'ZAR', 'KRW', 'JPY']
+
+    all_rates = await get_all_rates()
+    print(f"All rates for today: {all_rates}")  # [Currency(name='Австралийский доллар', code='AUD', price=35.9552, 
+    # date=datetime.datetime(2022, 10, 3, 23, 45, 29, 145779)), ...]
+
+
+asyncio.run(main())
+```
+
+### Доступные асинхронные функции библиотеки:
+- **get_codes(date)** - получить все доступные коды валют на определённую дату:  
+`codes = await get_codes()  # Коды валют`
+- **get_rate(code, date)** - получить курс определённой валюты по её коду на определённую дату:  
+`usd_rate = await get_rate("USD")  # Курс доллара на сегодня`
+- **get_all_rates(date)** - получить курс всех доступных валют от ЦБ на определённую дату:  
+`all_rates = await get_all_rates()  # Все курсы валют на сегодня`  
+! По умолчанию поле date - это сегодня.
+
+### Ошибки, которые можно получить при работе с библиотекой:
+- `NoValidDateError` - функция была вызвана с датой, которая ещё не наступила.
+- `CurrencyRateNotFoundError` - курс для данного кода валюты не найден.
```

### Comparing `async-cb-rate-1.0.0/README.md` & `async-cb-rate-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,63 @@
-# async-cb-rate
-Асинхронная библиотека для парсинга курса валют с сайта ЦБ РФ.
-
-### Библиотеку можно использовать для:
-- мониторинга за курсом валют
-- построения графиков изменения курса
-
-### Установка c pip
-```shell
-pip install async-cb-rate
-```
-
-### Краткий обзор функциональности
-- Библиотека позволяет получить курс валюты на любой день. По умолчанию курс ищется на сегодняшний день.
-- Функции возвращают объекты `Currency`, с которыми удобно далее работать.
-```python
-import asyncio
-
-from async_cb_rate.parser import get_rate, get_codes, get_all_rates
-
-
-async def main():
-    usd_rate = await get_rate("USD")
-    print(f"USD rate for today={usd_rate.price}₽")  # USD rate for today=55.2987₽
-
-    euro_rate = await get_rate("EUR")  # EUR rate for today=52.7379₽
-    print(f"EUR rate for today={euro_rate.price}₽")
-
-    codes = await get_codes()
-    print(f"Available codes: {codes}") # ['AUD', 'AZN', 'GBP', 'AMD', 'BYN', 'BGN', 'BRL', 'HUF', 'HKD', 'DKK', 'USD', 
-    # 'EUR', 'INR', 'KZT', 'CAD', 'KGS', 'CNY', 'MDL', 'NOK', 'PLN', 'RON', 'XDR', 'SGD', 'TJS', 'TRY', 'TMT', 'UZS', 
-    # 'UAH', 'CZK', 'SEK', 'CHF', 'ZAR', 'KRW', 'JPY']
-
-    all_rates = await get_all_rates()
-    print(f"All rates for today: {all_rates}")  # [Currency(name='Австралийский доллар', code='AUD', price=35.9552, 
-    # date=datetime.datetime(2022, 10, 3, 23, 45, 29, 145779)), ...]
-
-
-asyncio.run(main())
-```
-
-### Доступные асинхронные функции библиотеки:
-- **get_codes(date)** - получить все доступные коды валют на определённую дату:  
-`codes = await get_codes()  # Коды валют`
-- **get_rate(code, date)** - получить курс определённой валюты по её коду на определённую дату:  
-`usd_rate = await get_rate("USD")  # Курс доллара на сегодня`
-- **get_all_rates(date)** - получить курс всех доступных валют от ЦБ на определённую дату:  
-`all_rates = await get_all_rates()  # Все курсы валют на сегодня`  
-! По умолчанию поле date - это сегодня.
-
-### Ошибки, которые можно получить при работе с библиотекой:
-- `NoValidDateError` - функция была вызвана с датой, которая ещё не наступила.
-- `CurrencyRateNotFoundError` - курс для данного кода валюты не найден.
+Metadata-Version: 2.1
+Name: async-cb-rate
+Version: 1.0.1
+Summary: Package for async parsing CB rates
+Home-page: https://github.com/alenapoliakova/async-cb-rate
+Author: Alena Polyakova
+Author-email: alenapoliakova2003@gmail.com
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# async-cb-rate
+Асинхронная библиотека для парсинга курса валют с сайта ЦБ РФ.
+
+### Библиотеку можно использовать для:
+- мониторинга за курсом валют
+- построения графиков изменения курса
+
+### Установка c pip
+```shell
+pip install async-cb-rate
+```
+
+### Краткий обзор функциональности
+- Библиотека позволяет получить курс валюты на любой день. По умолчанию курс ищется на сегодняшний день.
+- Функции возвращают объекты `Currency`, с которыми удобно далее работать.
+```python
+import asyncio
+
+from async_cb_rate.parser import get_rate, get_codes, get_all_rates
+
+
+async def main():
+    usd_rate = await get_rate("USD")
+    print(f"USD rate for today={usd_rate.price}₽")  # USD rate for today=55.2987₽
+
+    euro_rate = await get_rate("EUR")  # EUR rate for today=52.7379₽
+    print(f"EUR rate for today={euro_rate.price}₽")
+
+    codes = await get_codes()
+    print(f"Available codes: {codes}") # ['AUD', 'AZN', 'GBP', 'AMD', 'BYN', 'BGN', 'BRL', 'HUF', 'HKD', 'DKK', 'USD', 
+    # 'EUR', 'INR', 'KZT', 'CAD', 'KGS', 'CNY', 'MDL', 'NOK', 'PLN', 'RON', 'XDR', 'SGD', 'TJS', 'TRY', 'TMT', 'UZS', 
+    # 'UAH', 'CZK', 'SEK', 'CHF', 'ZAR', 'KRW', 'JPY']
+
+    all_rates = await get_all_rates()
+    print(f"All rates for today: {all_rates}")  # [Currency(name='Австралийский доллар', code='AUD', price=35.9552, 
+    # date=datetime.datetime(2022, 10, 3, 23, 45, 29, 145779)), ...]
+
+
+asyncio.run(main())
+```
+
+### Доступные асинхронные функции библиотеки:
+- **get_codes(date)** - получить все доступные коды валют на определённую дату:  
+`codes = await get_codes()  # Коды валют`
+- **get_rate(code, date)** - получить курс определённой валюты по её коду на определённую дату:  
+`usd_rate = await get_rate("USD")  # Курс доллара на сегодня`
+- **get_all_rates(date)** - получить курс всех доступных валют от ЦБ на определённую дату:  
+`all_rates = await get_all_rates()  # Все курсы валют на сегодня`  
+! По умолчанию поле date - это сегодня.
+
+### Ошибки, которые можно получить при работе с библиотекой:
+- `NoValidDateError` - функция была вызвана с датой, которая ещё не наступила.
+- `CurrencyRateNotFoundError` - курс для данного кода валюты не найден.
```

### Comparing `async-cb-rate-1.0.0/async_cb_rate.egg-info/PKG-INFO` & `async-cb-rate-1.0.1/async_cb_rate.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-Metadata-Version: 2.1
-Name: async-cb-rate
-Version: 1.0.0
-Summary: Package for async parsing CB rates
-Home-page: https://github.com/alenapoliakova/async-cb-rate
-Author: Alena Polyakova
-Author-email: alenapoliakova2003@gmail.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# async-cb-rate
-Асинхронная библиотека для парсинга курса валют с сайта ЦБ РФ.
-
-### Библиотеку можно использовать для:
-- мониторинга за курсом валют
-- построения графиков изменения курса
-
-### Установка c pip
-```shell
-pip install async-cb-rate
-```
-
-### Краткий обзор функциональности
-- Библиотека позволяет получить курс валюты на любой день. По умолчанию курс ищется на сегодняшний день.
-- Функции возвращают объекты `Currency`, с которыми удобно далее работать.
-```python
-import asyncio
-
-from async_cb_rate.parser import get_rate, get_codes, get_all_rates
-
-
-async def main():
-    usd_rate = await get_rate("USD")
-    print(f"USD rate for today={usd_rate.price}₽")  # USD rate for today=55.2987₽
-
-    euro_rate = await get_rate("EUR")  # EUR rate for today=52.7379₽
-    print(f"EUR rate for today={euro_rate.price}₽")
-
-    codes = await get_codes()
-    print(f"Available codes: {codes}") # ['AUD', 'AZN', 'GBP', 'AMD', 'BYN', 'BGN', 'BRL', 'HUF', 'HKD', 'DKK', 'USD', 
-    # 'EUR', 'INR', 'KZT', 'CAD', 'KGS', 'CNY', 'MDL', 'NOK', 'PLN', 'RON', 'XDR', 'SGD', 'TJS', 'TRY', 'TMT', 'UZS', 
-    # 'UAH', 'CZK', 'SEK', 'CHF', 'ZAR', 'KRW', 'JPY']
-
-    all_rates = await get_all_rates()
-    print(f"All rates for today: {all_rates}")  # [Currency(name='Австралийский доллар', code='AUD', price=35.9552, 
-    # date=datetime.datetime(2022, 10, 3, 23, 45, 29, 145779)), ...]
-
-
-asyncio.run(main())
-```
-
-### Доступные асинхронные функции библиотеки:
-- **get_codes(date)** - получить все доступные коды валют на определённую дату:  
-`codes = await get_codes()  # Коды валют`
-- **get_rate(code, date)** - получить курс определённой валюты по её коду на определённую дату:  
-`usd_rate = await get_rate("USD")  # Курс доллара на сегодня`
-- **get_all_rates(date)** - получить курс всех доступных валют от ЦБ на определённую дату:  
-`all_rates = await get_all_rates()  # Все курсы валют на сегодня`  
-! По умолчанию поле date - это сегодня.
-
-### Ошибки, которые можно получить при работе с библиотекой:
-- `NoValidDateError` - функция была вызвана с датой, которая ещё не наступила.
-- `CurrencyRateNotFoundError` - курс для данного кода валюты не найден.
+Metadata-Version: 2.1
+Name: async-cb-rate
+Version: 1.0.1
+Summary: Package for async parsing CB rates
+Home-page: https://github.com/alenapoliakova/async-cb-rate
+Author: Alena Polyakova
+Author-email: alenapoliakova2003@gmail.com
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# async-cb-rate
+Асинхронная библиотека для парсинга курса валют с сайта ЦБ РФ.
+
+### Библиотеку можно использовать для:
+- мониторинга за курсом валют
+- построения графиков изменения курса
+
+### Установка c pip
+```shell
+pip install async-cb-rate
+```
+
+### Краткий обзор функциональности
+- Библиотека позволяет получить курс валюты на любой день. По умолчанию курс ищется на сегодняшний день.
+- Функции возвращают объекты `Currency`, с которыми удобно далее работать.
+```python
+import asyncio
+
+from async_cb_rate.parser import get_rate, get_codes, get_all_rates
+
+
+async def main():
+    usd_rate = await get_rate("USD")
+    print(f"USD rate for today={usd_rate.price}₽")  # USD rate for today=55.2987₽
+
+    euro_rate = await get_rate("EUR")  # EUR rate for today=52.7379₽
+    print(f"EUR rate for today={euro_rate.price}₽")
+
+    codes = await get_codes()
+    print(f"Available codes: {codes}") # ['AUD', 'AZN', 'GBP', 'AMD', 'BYN', 'BGN', 'BRL', 'HUF', 'HKD', 'DKK', 'USD', 
+    # 'EUR', 'INR', 'KZT', 'CAD', 'KGS', 'CNY', 'MDL', 'NOK', 'PLN', 'RON', 'XDR', 'SGD', 'TJS', 'TRY', 'TMT', 'UZS', 
+    # 'UAH', 'CZK', 'SEK', 'CHF', 'ZAR', 'KRW', 'JPY']
+
+    all_rates = await get_all_rates()
+    print(f"All rates for today: {all_rates}")  # [Currency(name='Австралийский доллар', code='AUD', price=35.9552, 
+    # date=datetime.datetime(2022, 10, 3, 23, 45, 29, 145779)), ...]
+
+
+asyncio.run(main())
+```
+
+### Доступные асинхронные функции библиотеки:
+- **get_codes(date)** - получить все доступные коды валют на определённую дату:  
+`codes = await get_codes()  # Коды валют`
+- **get_rate(code, date)** - получить курс определённой валюты по её коду на определённую дату:  
+`usd_rate = await get_rate("USD")  # Курс доллара на сегодня`
+- **get_all_rates(date)** - получить курс всех доступных валют от ЦБ на определённую дату:  
+`all_rates = await get_all_rates()  # Все курсы валют на сегодня`  
+! По умолчанию поле date - это сегодня.
+
+### Ошибки, которые можно получить при работе с библиотекой:
+- `NoValidDateError` - функция была вызвана с датой, которая ещё не наступила.
+- `CurrencyRateNotFoundError` - курс для данного кода валюты не найден.
```

