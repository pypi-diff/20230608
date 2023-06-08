# Comparing `tmp/hun-date-parser-0.1.1.tar.gz` & `tmp/hun-date-parser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hun-date-parser-0.1.1.tar", last modified: Sun Apr 10 16:58:46 2022, max compression
+gzip compressed data, was "hun-date-parser-0.2.0.tar", last modified: Wed Jun  7 18:04:36 2023, max compression
```

## Comparing `hun-date-parser-0.1.1.tar` & `hun-date-parser-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 somanagy  (1000) somanagy  (1000)        0 2022-04-10 16:58:46.000000 hun-date-parser-0.1.1/
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     1035 2021-10-11 14:03:23.000000 hun-date-parser-0.1.1/LICENSE
--rw-r--r--   0 somanagy  (1000) somanagy  (1000)     3528 2022-04-10 16:58:46.000000 hun-date-parser-0.1.1/PKG-INFO
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     3372 2021-10-11 14:03:23.000000 hun-date-parser-0.1.1/README.md
-drwxr-xr-x   0 somanagy  (1000) somanagy  (1000)        0 2022-04-10 16:58:46.000000 hun-date-parser-0.1.1/hun_date_parser/
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)      354 2022-04-10 16:53:47.000000 hun-date-parser-0.1.1/hun_date_parser/__init__.py
-drwxr-xr-x   0 somanagy  (1000) somanagy  (1000)        0 2022-04-10 16:58:46.000000 hun-date-parser-0.1.1/hun_date_parser/date_parser/
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)        0 2021-10-11 14:03:23.000000 hun-date-parser-0.1.1/hun_date_parser/date_parser/__init__.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)    11113 2022-04-10 16:46:47.000000 hun-date-parser-0.1.1/hun_date_parser/date_parser/date_parsers.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)    11961 2022-01-12 19:15:06.000000 hun-date-parser-0.1.1/hun_date_parser/date_parser/datetime_extractor.py
-drwxr-xr-x   0 somanagy  (1000) somanagy  (1000)        0 2022-04-10 16:58:46.000000 hun-date-parser-0.1.1/hun_date_parser/date_parser/interval_restriction/
--rw-r--r--   0 somanagy  (1000) somanagy  (1000)      222 2021-11-13 18:02:03.000000 hun-date-parser-0.1.1/hun_date_parser/date_parser/interval_restriction/__init__.py
--rw-r--r--   0 somanagy  (1000) somanagy  (1000)     5793 2022-01-15 13:15:49.000000 hun-date-parser-0.1.1/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     2859 2022-04-10 16:44:31.000000 hun-date-parser-0.1.1/hun_date_parser/date_parser/patterns.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     1212 2022-01-12 19:11:19.000000 hun-date-parser-0.1.1/hun_date_parser/date_parser/structure_parsers.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     8007 2021-12-17 10:46:26.000000 hun-date-parser-0.1.1/hun_date_parser/date_parser/time_parsers.py
-drwxr-xr-x   0 somanagy  (1000) somanagy  (1000)        0 2022-04-10 16:58:46.000000 hun-date-parser-0.1.1/hun_date_parser/date_textualizer/
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)        0 2021-10-11 14:03:23.000000 hun-date-parser-0.1.1/hun_date_parser/date_textualizer/__init__.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     1439 2021-10-11 14:03:23.000000 hun-date-parser-0.1.1/hun_date_parser/date_textualizer/date2text.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     2161 2021-11-13 18:02:03.000000 hun-date-parser-0.1.1/hun_date_parser/date_textualizer/datetime_textualizer.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     4182 2021-11-13 18:02:03.000000 hun-date-parser-0.1.1/hun_date_parser/date_textualizer/time2text.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     3064 2021-10-11 14:03:23.000000 hun-date-parser-0.1.1/hun_date_parser/utils.py
-drwxr-xr-x   0 somanagy  (1000) somanagy  (1000)        0 2022-04-10 16:58:46.000000 hun-date-parser-0.1.1/hun_date_parser.egg-info/
--rw-r--r--   0 somanagy  (1000) somanagy  (1000)     3528 2022-04-10 16:58:46.000000 hun-date-parser-0.1.1/hun_date_parser.egg-info/PKG-INFO
--rw-r--r--   0 somanagy  (1000) somanagy  (1000)     1059 2022-04-10 16:58:46.000000 hun-date-parser-0.1.1/hun_date_parser.egg-info/SOURCES.txt
--rw-r--r--   0 somanagy  (1000) somanagy  (1000)        1 2022-04-10 16:58:46.000000 hun-date-parser-0.1.1/hun_date_parser.egg-info/dependency_links.txt
--rw-r--r--   0 somanagy  (1000) somanagy  (1000)       21 2022-04-10 16:58:46.000000 hun-date-parser-0.1.1/hun_date_parser.egg-info/top_level.txt
--rw-r--r--   0 somanagy  (1000) somanagy  (1000)       38 2022-04-10 16:58:46.000000 hun-date-parser-0.1.1/setup.cfg
--rw-r--r--   0 somanagy  (1000) somanagy  (1000)      900 2021-11-13 18:02:03.000000 hun-date-parser-0.1.1/setup.py
-drwxr-xr-x   0 somanagy  (1000) somanagy  (1000)        0 2022-04-10 16:58:46.000000 hun-date-parser-0.1.1/test/
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)        0 2021-10-11 14:03:23.000000 hun-date-parser-0.1.1/test/__init__.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     5972 2022-04-10 16:45:09.000000 hun-date-parser-0.1.1/test/test_date_parsers.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     2869 2021-11-13 18:02:03.000000 hun-date-parser-0.1.1/test/test_datetime2text.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     4623 2022-01-26 18:27:57.000000 hun-date-parser-0.1.1/test/test_datetime_extractor.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     1490 2022-01-11 16:16:23.000000 hun-date-parser-0.1.1/test/test_exposed.py
--rw-r--r--   0 somanagy  (1000) somanagy  (1000)     4168 2022-01-15 13:11:36.000000 hun-date-parser-0.1.1/test/test_restricted_parsing.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     1471 2022-01-26 18:28:30.000000 hun-date-parser-0.1.1/test/test_structure_parsers.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     4315 2022-01-12 18:53:54.000000 hun-date-parser-0.1.1/test/test_time_parsers.py
--rw-rw-r--   0 somanagy  (1000) somanagy  (1000)     1074 2021-10-11 14:03:23.000000 hun-date-parser-0.1.1/test/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:04:36.059893 hun-date-parser-0.2.0/
+-rw-rw-rw-   0        0        0     1035 2021-10-11 13:03:22.000000 hun-date-parser-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     6246 2023-06-07 18:04:36.059893 hun-date-parser-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5213 2023-06-07 17:34:49.000000 hun-date-parser-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 18:04:35.989882 hun-date-parser-0.2.0/hun_date_parser/
+-rw-rw-rw-   0        0        0      354 2023-06-07 17:05:15.000000 hun-date-parser-0.2.0/hun_date_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:04:36.021130 hun-date-parser-0.2.0/hun_date_parser/date_parser/
+-rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/__init__.py
+-rw-rw-rw-   0        0        0    17255 2023-06-07 16:48:16.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/date_parsers.py
+-rw-rw-rw-   0        0        0    13654 2023-06-07 17:57:27.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/datetime_extractor.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:04:36.036754 hun-date-parser-0.2.0/hun_date_parser/date_parser/interval_restriction/
+-rw-rw-rw-   0        0        0      222 2021-11-13 17:02:02.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/interval_restriction/__init__.py
+-rw-rw-rw-   0        0        0     5789 2023-06-07 17:51:56.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py
+-rw-rw-rw-   0        0        0     4089 2023-05-31 06:07:00.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/patterns.py
+-rw-rw-rw-   0        0        0     1212 2022-01-12 18:11:18.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/structure_parsers.py
+-rw-rw-rw-   0        0        0     8862 2023-05-24 09:42:41.000000 hun-date-parser-0.2.0/hun_date_parser/date_parser/time_parsers.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:04:36.036754 hun-date-parser-0.2.0/hun_date_parser/date_textualizer/
+-rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.0/hun_date_parser/date_textualizer/__init__.py
+-rw-rw-rw-   0        0        0     1439 2021-10-11 13:03:22.000000 hun-date-parser-0.2.0/hun_date_parser/date_textualizer/date2text.py
+-rw-rw-rw-   0        0        0     2161 2021-11-13 17:02:02.000000 hun-date-parser-0.2.0/hun_date_parser/date_textualizer/datetime_textualizer.py
+-rw-rw-rw-   0        0        0     4182 2021-11-13 17:02:02.000000 hun-date-parser-0.2.0/hun_date_parser/date_textualizer/time2text.py
+-rw-rw-rw-   0        0        0     3965 2023-06-06 04:24:10.000000 hun-date-parser-0.2.0/hun_date_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:04:36.021130 hun-date-parser-0.2.0/hun_date_parser.egg-info/
+-rw-rw-rw-   0        0        0     6246 2023-06-07 18:04:35.000000 hun-date-parser-0.2.0/hun_date_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1097 2023-06-07 18:04:35.000000 hun-date-parser-0.2.0/hun_date_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 18:04:35.000000 hun-date-parser-0.2.0/hun_date_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-07 18:04:35.000000 hun-date-parser-0.2.0/hun_date_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-07 18:04:35.000000 hun-date-parser-0.2.0/hun_date_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 18:04:36.059893 hun-date-parser-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2023-06-07 17:16:42.000000 hun-date-parser-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 18:04:36.059893 hun-date-parser-0.2.0/test/
+-rw-rw-rw-   0        0        0        0 2021-10-11 13:03:22.000000 hun-date-parser-0.2.0/test/__init__.py
+-rw-rw-rw-   0        0        0    13631 2023-06-07 17:51:56.000000 hun-date-parser-0.2.0/test/test_date_parsers.py
+-rw-rw-rw-   0        0        0     2869 2021-11-13 17:02:02.000000 hun-date-parser-0.2.0/test/test_datetime2text.py
+-rw-rw-rw-   0        0        0    11544 2023-06-07 17:56:26.000000 hun-date-parser-0.2.0/test/test_datetime_extractor.py
+-rw-rw-rw-   0        0        0     1490 2022-01-11 15:16:22.000000 hun-date-parser-0.2.0/test/test_exposed.py
+-rw-rw-rw-   0        0        0     4168 2022-01-15 12:11:36.000000 hun-date-parser-0.2.0/test/test_restricted_parsing.py
+-rw-rw-rw-   0        0        0     1471 2022-01-26 17:28:30.000000 hun-date-parser-0.2.0/test/test_structure_parsers.py
+-rw-rw-rw-   0        0        0     4315 2022-01-12 17:53:54.000000 hun-date-parser-0.2.0/test/test_time_parsers.py
+-rw-rw-rw-   0        0        0     1074 2021-10-11 13:03:22.000000 hun-date-parser-0.2.0/test/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hun-date-parser-0.1.1/LICENSE` & `hun-date-parser-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.1.1/hun_date_parser/date_parser/datetime_extractor.py` & `hun-date-parser-0.2.0/hun_date_parser/date_parser/datetime_extractor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,99 @@
 """This module handles combined date and time parsing."""
 
 from datetime import datetime, timedelta, date, time
 from calendar import monthrange
 from itertools import chain
 
-from typing import Dict, List, Union, Tuple
+from typing import Dict, List, Union
 from copy import copy
 
 from hun_date_parser.date_parser.structure_parsers import match_multi_match, match_interval
 from hun_date_parser.date_parser.date_parsers import (match_named_month, match_iso_date, match_weekday,
                                                       match_relative_day,
-                                                      match_week, match_named_year, match_n_periods_compared_to_now)
+                                                      match_week, match_named_year, match_n_periods_compared_to_now,
+                                                      match_relative_month, match_in_past_n_periods)
 from hun_date_parser.date_parser.time_parsers import match_digi_clock, match_time_words, match_now, match_hwords
-from hun_date_parser.utils import Year, Month, Week, Day, Daypart, Hour, Minute, monday_of_calenderweek
+from hun_date_parser.utils import (Year, Month, Week, Day, Daypart, Hour, Minute, OverrideTopWithNow, SearchScopes,
+                                   OverrideBottomWithNow, monday_of_calenderweek, DateTimePartConatiner,
+                                   return_on_value_error)
 
 datelike = Union[datetime, date, time, None]
 
 daypart_mapping = [
     (3, 5),     # hajnal
     (6, 10),    # reggel
     (8, 11),    # délelőtt
     (12, 18),   # délután
     (18, 21),   # este
     (22, 2)     # éjjel
 ]
 
 
 def text2datetime(input_sentence: str, now: datetime = datetime.now(),
-                  expect_future_day: bool = False) -> List[Dict[str, datelike]]:
+                  search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List[Dict[str, datelike]]:
     """
     Returns the list of datetime intervals found in the input sentence.
     :param input_sentence: Input sentence string.
     :param now: Current timestamp to calculate relative dates.
-    :param expect_future_day: Shows if the extracted date will be offset.
+    :param search_scope: Defines whether the timeframe should be restricted to past or future.
     :return: list of datetime interval dictionaries
     """
-    datetime_extractor = DatetimeExtractor(now=now, output_container='datetime', expect_future_day=expect_future_day)
+    datetime_extractor = DatetimeExtractor(now=now, output_container='datetime', search_scope=search_scope)
     return datetime_extractor.parse_datetime(sentence=input_sentence)
 
 
 def text2date(input_sentence: str, now: datetime = datetime.now(),
-              expect_future_day: bool = False) -> List[Dict[str, datelike]]:
+              search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List[Dict[str, datelike]]:
     """
     Returns the list of date intervals found in the input sentence.
     :param input_sentence: Input sentence string.
     :param now: Current timestamp to calculate relative dates.
-    :param expect_future_day: Shows if the extracted date will be offset.
+    :param search_scope: Defines whether the timeframe should be restricted to past or future.
     :return: list of date interval dictionaries
     """
-    datetime_extractor = DatetimeExtractor(now=now, output_container='date', expect_future_day=expect_future_day)
+    datetime_extractor = DatetimeExtractor(now=now, output_container='date', search_scope=search_scope)
     return datetime_extractor.parse_datetime(sentence=input_sentence)
 
 
 def text2time(input_sentence: str, now: datetime = datetime.now(),
-              expect_future_day: bool = False) -> List[Dict[str, datelike]]:
+              search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List[Dict[str, datelike]]:
     """
     Returns the list of time intervals found in the input sentence.
     :param input_sentence: Input sentence string.
     :param now: Current timestamp to calculate relative dates.
-    :param expect_future_day: Shows if the extracted date will be offset.
+    :param search_scope: Defines whether the timeframe should be restricted to past or future.
     :return: list of time interval dictionaries
     """
-    datetime_extractor = DatetimeExtractor(now=now, output_container='time', expect_future_day=expect_future_day)
+    datetime_extractor = DatetimeExtractor(now=now, output_container='time', search_scope=search_scope)
     return datetime_extractor.parse_datetime(sentence=input_sentence)
 
 
-def match_rules(now: datetime, sentence: str, expect_future_day: bool = False) -> List:
+def match_rules(now: datetime, sentence: str,
+                search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> List:
     """
     Matches all rules against input text.
     :param now: Current timestamp to calculate relative dates.
     :param sentence: Input sentence.
-    :param expect_future_day: Shows if the extracted date will be offset.
+    :param search_scope: Defines whether the timeframe should be restricted to past or future.
     :return: Parsed date and time classes.
     """
-    matches = [*match_named_month(sentence, now),
+    matches = [*match_named_month(sentence, now, search_scope),
                *match_iso_date(sentence),
                *match_relative_day(sentence, now),
-               *match_weekday(sentence, now, expect_future_day),
+               *match_weekday(sentence, now, search_scope),
                *match_week(sentence, now),
                *match_named_year(sentence, now),
                *match_digi_clock(sentence),
                *match_hwords(sentence),
                *match_time_words(sentence),
                *match_now(sentence, now),
-               *match_n_periods_compared_to_now(sentence, now)]
+               *match_n_periods_compared_to_now(sentence, now),
+               *match_relative_month(sentence, now),
+               *match_in_past_n_periods(sentence, now)]
 
     matches = list(chain(*[m['date_parts'] for m in matches]))
 
     return matches
 
 
 def extend_start_end(interval: Dict) -> Dict:
@@ -118,29 +124,30 @@
 
 class DatetimeExtractor:
     """
     This class handles combined date and time parsing.
     """
 
     def __init__(self, now: datetime = datetime.now(), output_container: str = 'datetime',
-                 expect_future_day: bool = False) -> None:
+                 search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED) -> None:
         """
         :param now: Current timestamp to calculate relative dates.
         :param output_container: datetime object to populate with datetime parts
-        :param expect_future_day: Shows if the extracted date will be offset.
+        :param search_scope: Defines whether the timeframe should be restricted to past or future.
         """
         self.now = now
         self.output_container = output_container
-        self.expect_future_day = expect_future_day
+        self.search_scope = search_scope
 
     def _get_implicit_intervall(self, sentence_part: str):
-        matches = match_rules(self.now, sentence_part, self.expect_future_day)
+        matches = match_rules(self.now, sentence_part, self.search_scope)
         return [{'start_date': matches, 'end_date': matches}]
 
-    def assamble_datetime(self, now: datetime,
+    @return_on_value_error(None)
+    def assemble_datetime(self, now: datetime,
                           dateparts: Union[List[Union[Year, Month, Week, Day, Daypart, Hour, Minute]], str],
                           bottom: bool = True) -> datelike:
         """
         Assambles parsed date and time classes into datetime instance.
         :param now: Current timestamp to calculate relative dates.
         :param dateparts: List of date and time classes.
         :param bottom: True if the bottom of the interval should be returned, False otherwise
@@ -152,96 +159,101 @@
         if dateparts == 'OPEN':
             return None
         if not dateparts:
             return None
 
         has_date, has_time = False, False
 
+        # this functionality is used to override the bottom or the top of the interval with the current date
+        # rules indicate the necessity for this with returning either OverrideBottomWithNow or OverrideTopWithNow
+        override_bottom, override_top = type_isin_list(OverrideBottomWithNow, dateparts),\
+            type_isin_list(OverrideTopWithNow, dateparts)
+
         pre_first = True
         for date_type in [Year, Month, Week, Day, Daypart, Hour, Minute]:
             dp_match = [pot_dp for pot_dp in dateparts if isinstance(pot_dp, date_type)]
 
-            _dp_match: Union[Tuple[int, str], None]
+            _dp_match: Union[DateTimePartConatiner, None]
             if dp_match:
                 _dp_match = dp_match[0]
             else:
                 _dp_match = None
 
             if date_type == Year:
-                if _dp_match:
+                if _dp_match and _dp_match.value is not None:
                     has_date = True
                     pre_first = False
-                    res_dt.append(_dp_match[0])
+                    res_dt.append(_dp_match.value)
                 else:
-                    # TODO: this should take into account the expect_future_day parameter...
+                    # TODO: this should take into account the search_scope parameter...
                     res_dt.append(now.year)
 
             if date_type == Month:
-                if _dp_match:
+                if _dp_match and _dp_match.value is not None:
                     has_date = True
                     pre_first = False
-                    res_dt.append(_dp_match[0])
+                    res_dt.append(_dp_match.value)
                 elif pre_first:
                     res_dt.append(now.month)
                 elif bottom:
                     res_dt.append(1)
                 else:
                     res_dt.append(12)
 
             if date_type == Week and not type_isin_list(Day, dateparts):
-                if _dp_match:
+                if _dp_match and _dp_match.value is not None:
                     has_date = True
                     pre_first = False
-                    week2dt = monday_of_calenderweek(res_dt[0], _dp_match[0]) + timedelta(days=(0 if bottom else 6))
+                    week2dt = monday_of_calenderweek(res_dt[0], _dp_match.value) + timedelta(days=(0 if bottom else 6))
                     res_dt = [week2dt.year, week2dt.month, week2dt.day]
 
             if date_type == Day and len(res_dt) == 2:
-                if _dp_match:
+                if _dp_match and _dp_match.value is not None:
                     has_date = True
                     pre_first = False
-                    res_dt.append(_dp_match[0])
+                    res_dt.append(_dp_match.value)
                 elif pre_first:
                     res_dt.append(now.day)
                 elif bottom:
                     res_dt.append(1)
                 else:
                     mr = monthrange(res_dt[0], res_dt[1])
                     res_dt.append(mr[1])
 
             if date_type == Daypart:
-                if _dp_match:
+                if _dp_match and _dp_match.value is not None:
                     has_time = True
                     pre_first = False
-                    dp = _dp_match[0]
+                    dp = _dp_match.value
                     if bottom:
                         res_dt.append(daypart_mapping[dp][0])
                     elif dp == 5:
                         y, m, d = res_dt
                         next_day = datetime(y, m, d) + timedelta(days=1)
                         res_dt = [next_day.year, next_day.month, next_day.day, daypart_mapping[dp][1]]
                     else:
                         res_dt.append(daypart_mapping[dp][1])
 
             if date_type == Hour and len(res_dt) == 3:
-                if _dp_match:
+                if _dp_match and _dp_match.value is not None:
                     has_time = True
                     pre_first = False
-                    res_dt.append(_dp_match[0])
+                    res_dt.append(_dp_match.value)
                 elif pre_first:
                     res_dt.append(now.hour)
                 elif bottom:
                     res_dt.append(0)
                 elif not bottom:
                     res_dt.append(23)
 
             if date_type == Minute:
-                if _dp_match:
+                if _dp_match and _dp_match.value is not None:
                     has_time = True
                     pre_first = False
-                    res_dt.append(_dp_match[0])
+                    res_dt.append(_dp_match.value)
                 elif pre_first:
                     res_dt.append(now.minute)
                 elif bottom:
                     res_dt.append(0)
                 elif not bottom:
                     res_dt.append(59)
 
@@ -249,25 +261,37 @@
             res_dt.append(0)
         else:
             res_dt.append(59)
 
         y, m, d, h, mi, s = res_dt
 
         if self.output_container == 'datetime':
-            if has_date or has_time:
+            if bottom and override_bottom:
+                return now
+            elif not bottom and override_top:
+                return now
+            elif has_date or has_time:
                 return datetime(y, m, d, h, mi, s)
             else:
                 return None
         elif self.output_container == 'date':
-            if has_date:
+            if bottom and override_bottom:
+                return now.date()
+            elif not bottom and override_top:
+                return now.date()
+            elif has_date:
                 return date(y, m, d)
             else:
                 return None
         elif self.output_container == 'time':
-            if has_time:
+            if bottom and override_bottom:
+                return now.time()
+            elif not bottom and override_top:
+                return now.time()
+            elif has_time:
                 return time(h, mi, s)
             else:
                 return None
         else:
             return None
 
     def parse_datetime(self, sentence: str) -> List[Dict[str, datelike]]:
@@ -281,23 +305,23 @@
         parsed_dates = []
 
         for sentence_part in sentence_parts:
             interval = match_interval(sentence_part)
 
             if interval:
                 interval['start_date'] = 'OPEN' if interval['start_date'] == 'OPEN' else match_rules(self.now, interval[
-                    'start_date'], self.expect_future_day)
+                    'start_date'], self.search_scope)
                 interval['end_date'] = 'OPEN' if interval['end_date'] == 'OPEN' else match_rules(self.now, interval[
-                    'end_date'], self.expect_future_day)
+                    'end_date'], self.search_scope)
                 parsed_dates.append(interval)
             else:
                 parsed_dates += self._get_implicit_intervall(sentence_part)
 
         parsed_dates = [extend_start_end(intv) for intv in parsed_dates]
 
-        parsed_dates = [{'start_date': self.assamble_datetime(self.now, parsed_date['start_date'], bottom=True),
-                         'end_date': self.assamble_datetime(self.now, parsed_date['end_date'], bottom=False)}
+        parsed_dates = [{'start_date': self.assemble_datetime(self.now, parsed_date['start_date'], bottom=True),
+                         'end_date': self.assemble_datetime(self.now, parsed_date['end_date'], bottom=False)}
                         for parsed_date in parsed_dates]
 
         parsed_dates = [intv for intv in parsed_dates if intv['start_date'] or intv['end_date']]
 
         return parsed_dates
```

### Comparing `hun-date-parser-0.1.1/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py` & `hun-date-parser-0.2.0/hun_date_parser/date_parser/interval_restriction/restricted_parsing.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from datetime import datetime, date, time, timedelta
 from enum import Enum
 from typing import Dict, List, Union, Tuple
 from copy import deepcopy
 
 from hun_date_parser import text2datetime
-from hun_date_parser.utils import remove_accent
+from hun_date_parser.utils import remove_accent, SearchScopes
 from hun_date_parser.date_parser.time_parsers import _raw_match_time_words
 
 datelike = Union[datetime, date, time, None]
 
 
 def get_reversed_am_pm(dt: datetime):
     dt_ = deepcopy(dt)
@@ -49,30 +49,30 @@
 
     return False
 
 
 def extract_datetime_within_interval(interval_start: datetime,
                                      interval_end: datetime,
                                      query_text: str,
-                                     expect_future_day: bool = False,
+                                     search_scope: SearchScopes = SearchScopes.NOT_RESTRICTED,
                                      fallback_now=datetime.now()) -> Tuple[ExtractWithinRangeSuccess,
                                                                            List[Dict[str, datelike]]]:
     """
     Extracts datetime intervals from pre-determined datetime intervals.
     :param interval_start: Bounding interval start
     :param interval_end: Bounding interval end
     :param query_text: Text to extract datetime interval from
-    :param expect_future_day: Shows if the extracted date will be offset.
+    :param search_scope: Sets the desired time horizont of the search.
     :param fallback_now: When interval restriction is unsuccessful (RELATIVE_TIME_WORD_FALLBACK, OUT_OF_RANGE_FALLBACK)
     the text2datetime function's result is returned, which can be supplied with a pseudo-now datetime
     :return: success flag, restricted time interval
     """
 
     res = text2datetime(query_text,
-                        expect_future_day=expect_future_day,
+                        search_scope=search_scope,
                         now=interval_start)
 
     possible_am_pm_missmatch = False
     parts = _raw_match_time_words(query_text)
     if parts:
         group, daypart, hour_modifier, hour, minute = parts
         if not daypart and hour:
@@ -91,37 +91,37 @@
 
     restricted_date: List[Dict[str, datelike]] = []
     response_candidates = [(5, ExtractWithinRangeSuccess.NO_MATCH_FALLBACK, restricted_date)]
     for r in res:
         if not (isinstance(r['start_date'], datetime) and isinstance(r['end_date'], datetime)):
             response_type = ExtractWithinRangeSuccess.OPEN_RANGE_FALLBACK
             restricted_date = text2datetime(query_text,
-                                            expect_future_day=expect_future_day,
+                                            search_scope=search_scope,
                                             now=fallback_now)
 
             response_candidates.append((4, response_type, restricted_date))
             continue
 
         assert type(interval_start) == datetime and type(r['start_date']) == datetime
         assert type(interval_end) == datetime and type(r['end_date']) == datetime
         if not (interval_start <= r['start_date'] and r['end_date'] <= interval_end):
             # Extracted datetime is out of expected interval...
             response_type = ExtractWithinRangeSuccess.OUT_OF_RANGE_FALLBACK
             restricted_date = text2datetime(query_text,
-                                            expect_future_day=expect_future_day,
+                                            search_scope=search_scope,
                                             now=fallback_now)
 
             response_candidates.append((2, response_type, restricted_date))
             continue
 
         if is_relative_datetime(query_text):
             # Datetime ranges relative to the current timestamp doesn't really make sense in this scenario...
             response_type = ExtractWithinRangeSuccess.RELATIVE_TIME_WORD_FALLBACK
             restricted_date = text2datetime(query_text,
-                                            expect_future_day=expect_future_day,
+                                            search_scope=search_scope,
                                             now=fallback_now)
 
             response_candidates.append((3, response_type, restricted_date))
         else:
             response_type = ExtractWithinRangeSuccess.VALID_IN_RANGE
             restricted_date = [r]
```

### Comparing `hun-date-parser-0.1.1/hun_date_parser/date_parser/patterns.py` & `hun-date-parser-0.2.0/hun_date_parser/date_parser/patterns.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 R_TOLIG = r'(.*-?t[oóöő]l\b)(.*-?ig\b)'
 R_TOL = r'([:\w ]*-?t[oóöő]l\b).*'
 R_IG = r'([:\w ]*-?ig\b)'
 
 # hyper day level patterns
 R_ISO_DATE = r'(\b\d{4,4})(?:[-\\/\.](1[0-2]|0?[1-9]))?(?:[-\\/\.](1[0-9]|2[0-9]|3[01]|0?[1-9]))?'
 R_NAMED_MONTH = r'(j[oöő]v[oöő].*?|tavaly.*?)?(\bjan(?:\b|\.|u[aá]r){1}|\bfeb(?:\b|r\.|\.|ru[aá]r){1}|\bm[aá]r(?:\b|c\b|c\.|\.|cius){1}|\b[aá]pr(?:\b|\.|ilis){1}\b|m[aá]j(?:\b|\.|us){1}|\bj[uú]n(?:\b|\.|ius){1}|\bj[uú]l(?:\b|\.|ius){1}|\baug(?:\b|\.|usztus){1}|\bszep(?:t\b|t\.|\b|\.|tember){1}|\bokt(?:\b|\.|[oó]ber){1}|\bnov(?:\b|\.|ember){1}|\bdec(?:\b|\.|ember){1})(?: ([1-3][0-9]|[1-9]))?'
+R_RELATIVE_MONTH = r'(?:(\blegut[oó]bbi|\butols[oó]|\bmúlt|\but[oó]bbi|\bezen|\bebben|\baktu[aá]lis|\bj[oöő]v[oöő]|\bk[oö]vetkez[oőö]|\bk[oö]vetkezend[oőö]).*)? a?h[oó]nap'
 
 R_WEEKDAY = r'(?:(el[oő]z[oő]|m[uú]lt|ezen|j[oöő]v[oöő]).*)?(h[eé]tf[oő]|kedd|szerd[aá]|cs[uü]t[oö]rt[oö]k|p[eé]ntek|szombat|vas[aá]rnap)'
 R_WEEK = r'(el[oő]z[oő] h[eé]t|m[uú]lt h[eé]t|m[uú]lth[eé]t|ezen a? h[eé]t|j[oöő]v[oöő]h[eé]t|j[oöő]v[oöő] h[eé]t)'
 
 R_TODAY = r'\b(má(?:tól|ra))\b|\b(ma)\b|\b(mai nap)\b'
 R_TOMORROW = r'\b(holnap)(?!ut[aá]n)'
 R_NTOMORROW = r'\b(holnaput[aá]n)'
@@ -20,21 +21,33 @@
 R_NYESTERDAY = r'\b(tegnapel[oő]tt)'
 
 R_NMINS_FROM_NOW = r'(([\w]*) perc m[úu]lva)'
 R_NHOURS_FROM_NOW = r'(([\w]*) [oó]ra m[úu]lva)'
 R_NDAYS_FROM_NOW = r'(([\w]*) nap m[úu]lva)'
 R_NWEEKS_FROM_NOW = r'(([\w]*) h[eé]t m[úu]lva)'
 
+R_NMINS_PRIOR_NOW = r'(([\w]*) percc?el (ezel[oöő]tt|kor[aá]bban|kor[aá]bbi))'
+R_NHOURS_PRIOR_NOW = r'(([\w]*) [oó]r[aá]val (ezel[oöő]tt|kor[aá]bban|kor[aá]bbi))'
+R_NDAYS_PRIOR_NOW = r'(([\w]*) napp?al (ezel[oöő]tt|kor[aá]bban|kor[aá]bbi))'
+R_NWEEKS_PRIOR_NOW = r'(([\w]*) h[eé]tt?el (ezel[oöő]tt|kor[aá]bban|kor[aá]bbi))'
+
+R_IN_PAST_PERIOD_MINS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b(percben|perc)'
+R_IN_PAST_PERIOD_HOURS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b([oó]r[aá]ban|[oó]rai|[oó]ra)'
+R_IN_PAST_PERIOD_DAYS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b(napban|napi|nap)'
+R_IN_PAST_PERIOD_WEEKS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b(h[eé]tben|heti|h[eé]t)'
+R_IN_PAST_PERIOD_MONTHS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b(h[oó]napban|havi|h[oó]nap)'
+R_IN_PAST_PERIOD_YEARS = r'(elm[úu]lt|megel[oőö]z[oőö]|el[oőö]z[oőö])\b([ \w]*)\b([eé]v|[eé]vben|[eé]vi)'
+
 R_YEAR = r'(tavalyel[oöő]tt|id[eé]n|j[oöő]v[oöő]re|tavaly|.*[eé]v m[uú]lva|.*[eé]vvel ezel[oő]tt|.*[eé]vvel kor[aá]bban)'
 
 # hour level
 R_AT = r'([:\w ]*-?kor)'
 
 # hour+minute parsers
 R_DIGI = r'\b([0-2]?[0-9]):([0-9][0-9])'
 R_HWORDS = r'([0-2][0-9])(?: ?óra|-?kor| ?h) ?(?:([0-9][0-9])(?:(?: ?perc| ?p)[\w]*))? ?(?:([0-9][0-9])(?:(?: ?m[áa]sodperc| ?mp)[\w]*))?'
-R_HWORDS_ = r'([1-2]?[0-9])?h'
+R_HWORDS_ = r'([1-2]?[0-9])?h\b'
 R_HOUR_MIN = r'(?:(.*hajnal[i]?|.*reggel|.*d[eé]lel[oőö]tt|.*d[eé]lut[aá]n|.*este|.*[eé]jjel))? ?(?:(.*negyed|.*f[eé]l|.*h[aá]romnegyed))? ?(?:(?:\b([0-9]{1,2}|nulla|egy|kett[oöő]|h[aá]rom|n[eé]gy|[öo]t|hat|h[eé]t|nyolc|kilenc|t[ií]z|tizenegy|tizenkett[oő]|tizenh[aá]rom|tizenn[eé]gy|tizen[oö]t|tizenhat|tizenh[eé]t|tizennyolc|tizenkilenc|h[uú]sz|huszonegy|huszonkett[oöő]|huszonh[aá]rom)(?! [eé]v|perc)-?(?:kor|ra|\b)(?: [oó]ra)?)?((?:el[oő]tt|ut[aá]n)?.*perc)?)?'
 R_HOUR_MIN_REV = r'(?:(.*)(?:perc.{0,4}))?? (?:(hajnal[i]?|reggel|d[eé]lel[oőö]tt|d[eé]lut[aá]n|este|[eé]jjel))? ?(negyed|f[eé]l|h[aá]romnegyed)? ?(?:([0-9]{1,2}|nulla|egy|kett[oöő]|h[aá]rom|n[eé]gy|[öo]t|hat|h[eé]t|nyolc|kilenc|t[ií]z|tizenegy|tizenkett[oő]|tizenh[aá]rom|tizenn[eé]gy|tizen[oö]t|tizenhat|tizenh[eé]t|tizennyolc|tizenkilenc|h[uú]sz|huszonegy|huszonkett[oöő]|huszonh[aá]rom)(?! [eé]v|perc)-?(?:kor|ra|\b)(?: [oó]ra)?)? ?(ut[aá]n|el[oöő]tt)?'
 
 # R_MIN = r'(.*)(?:perc)'
 # R_SEC = r'(.*)(?: ?m[áa]sodperc| ?mp)'
```

### Comparing `hun-date-parser-0.1.1/hun_date_parser/date_parser/structure_parsers.py` & `hun-date-parser-0.2.0/hun_date_parser/date_parser/structure_parsers.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.1.1/hun_date_parser/date_parser/time_parsers.py` & `hun-date-parser-0.2.0/hun_date_parser/date_parser/time_parsers.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,14 +39,41 @@
     for match in group:
         match = int(match)
         res.append({'match': match, 'date_parts': [Hour(match, 'hwords')]})
 
     return res
 
 
+def is_indeed_hour(s: str):
+    s_uac = remove_accent(s)
+
+    words_indicating_hour = [
+        "ora",
+        "-kor",
+        "egykor",
+        "kettokor",
+        "haromkor",
+        "negykor",
+        "otkor",
+        "hatkor",
+        "hetkor",
+        "nyolckor",
+        "kilenckor",
+        "tizkor",
+        "tizenegykor",
+        "tizenkettokor"
+    ]
+
+    for w in words_indicating_hour:
+        if w in s_uac:
+            return True
+
+    return False
+
+
 def _raw_match_time_words(s: str) -> Optional[Tuple[Any, Any, Any, Any, Any]]:
     """
     Extracts date and time particles from text
     :param s: input text
     :return:
     """
     group = re.findall(R_HOUR_MIN, s)
@@ -64,14 +91,20 @@
         minute += (' ' + is_before)
     elif group_rev[0].count('') < group[0].count(''):
         minute, daypart, hour_modifier, hour, is_before = group_rev[0]
         minute += (' ' + is_before)
     else:
         daypart, hour_modifier, hour, minute = group[0]
 
+    # when a single number is matched, the pattern currently interprets it as an hour value
+    # i.e.: "1" --> 1 hour or "egy" --> 1 hour
+    # this check is designed to address this issue (R_HOUR_MIN pattern needs to be rewritten for a proper solution)
+    if not (daypart or minute or hour_modifier) and hour and not is_indeed_hour(s):
+        return [('', '', '', '')], '', '', '', ''
+
     return group, daypart, hour_modifier, hour, minute
 
 
 def match_time_words(s: str) -> List[Dict[str, Any]]:
     """
     :param s: textual input
     :return: tuple of date parts
```

### Comparing `hun-date-parser-0.1.1/hun_date_parser/date_textualizer/date2text.py` & `hun-date-parser-0.2.0/hun_date_parser/date_textualizer/date2text.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.1.1/hun_date_parser/date_textualizer/datetime_textualizer.py` & `hun-date-parser-0.2.0/hun_date_parser/date_textualizer/datetime_textualizer.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.1.1/hun_date_parser/date_textualizer/time2text.py` & `hun-date-parser-0.2.0/hun_date_parser/date_textualizer/time2text.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.1.1/hun_date_parser.egg-info/SOURCES.txt` & `hun-date-parser-0.2.0/hun_date_parser.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 hun_date_parser/__init__.py
 hun_date_parser/utils.py
 hun_date_parser.egg-info/PKG-INFO
 hun_date_parser.egg-info/SOURCES.txt
 hun_date_parser.egg-info/dependency_links.txt
+hun_date_parser.egg-info/requires.txt
 hun_date_parser.egg-info/top_level.txt
 hun_date_parser/date_parser/__init__.py
 hun_date_parser/date_parser/date_parsers.py
 hun_date_parser/date_parser/datetime_extractor.py
 hun_date_parser/date_parser/patterns.py
 hun_date_parser/date_parser/structure_parsers.py
 hun_date_parser/date_parser/time_parsers.py
```

### Comparing `hun-date-parser-0.1.1/test/test_datetime2text.py` & `hun-date-parser-0.2.0/test/test_datetime2text.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.1.1/test/test_exposed.py` & `hun-date-parser-0.2.0/test/test_exposed.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.1.1/test/test_restricted_parsing.py` & `hun-date-parser-0.2.0/test/test_restricted_parsing.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.1.1/test/test_structure_parsers.py` & `hun-date-parser-0.2.0/test/test_structure_parsers.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.1.1/test/test_time_parsers.py` & `hun-date-parser-0.2.0/test/test_time_parsers.py`

 * *Files identical despite different names*

### Comparing `hun-date-parser-0.1.1/test/test_utils.py` & `hun-date-parser-0.2.0/test/test_utils.py`

 * *Files identical despite different names*

