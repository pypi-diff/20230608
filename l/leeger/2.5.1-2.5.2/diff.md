# Comparing `tmp/leeger-2.5.1.tar.gz` & `tmp/leeger-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leeger-2.5.1.tar", last modified: Thu Jun  8 00:32:25 2023, max compression
+gzip compressed data, was "leeger-2.5.2.tar", last modified: Thu Jun  8 00:59:58 2023, max compression
```

## Comparing `leeger-2.5.1.tar` & `leeger-2.5.2.tar`

### file list

```diff
@@ -1,221 +1,220 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:25.087222 leeger-2.5.1/
--rw-rw-rw-   0        0        0     1088 2022-06-10 22:18:01.000000 leeger-2.5.1/LICENSE
--rw-rw-rw-   0        0        0       63 2023-06-08 00:32:18.000000 leeger-2.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     9890 2023-06-08 00:32:25.086220 leeger-2.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     9480 2023-06-04 21:27:09.000000 leeger-2.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.564222 leeger-2.5.1/leeger/
--rw-rw-rw-   0        0        0       43 2022-08-13 05:53:15.000000 leeger-2.5.1/leeger/__init__.py
--rw-rw-rw-   0        0        0       98 2023-06-08 00:27:39.000000 leeger-2.5.1/leeger/_version.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.619224 leeger-2.5.1/leeger/calculator/
--rw-rw-rw-   0        0        0        0 2022-08-13 05:53:37.000000 leeger-2.5.1/leeger/calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.649222 leeger-2.5.1/leeger/calculator/all_time_calculator/
--rw-rw-rw-   0        0        0     5029 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py
--rw-rw-rw-   0        0        0     9107 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py
--rw-rw-rw-   0        0        0     1318 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py
--rw-rw-rw-   0        0        0     4490 2023-05-11 04:22:19.000000 leeger-2.5.1/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py
--rw-rw-rw-   0        0        0     9320 2023-05-11 04:31:22.000000 leeger-2.5.1/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py
--rw-rw-rw-   0        0        0     8996 2023-05-11 04:31:22.000000 leeger-2.5.1/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py
--rw-rw-rw-   0        0        0     2644 2023-05-11 04:22:19.000000 leeger-2.5.1/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py
--rw-rw-rw-   0        0        0     3351 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py
--rw-rw-rw-   0        0        0     8906 2023-05-11 04:22:19.000000 leeger-2.5.1/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py
--rw-rw-rw-   0        0        0     1519 2023-05-11 04:22:19.000000 leeger-2.5.1/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py
--rw-rw-rw-   0        0        0      712 2023-05-14 08:22:22.000000 leeger-2.5.1/leeger/calculator/all_time_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.657222 leeger-2.5.1/leeger/calculator/parent/
--rw-rw-rw-   0        0        0    15345 2023-05-11 04:22:19.000000 leeger-2.5.1/leeger/calculator/parent/AllTimeCalculator.py
--rw-rw-rw-   0        0        0     1671 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/calculator/parent/YearCalculator.py
--rw-rw-rw-   0        0        0       94 2023-05-14 08:22:22.000000 leeger-2.5.1/leeger/calculator/parent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.685224 leeger-2.5.1/leeger/calculator/year_calculator/
--rw-rw-rw-   0        0        0     9896 2023-05-11 04:22:19.000000 leeger-2.5.1/leeger/calculator/year_calculator/AWALYearCalculator.py
--rw-rw-rw-   0        0        0    18719 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py
--rw-rw-rw-   0        0        0     2018 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/calculator/year_calculator/PlusMinusYearCalculator.py
--rw-rw-rw-   0        0        0     5843 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/calculator/year_calculator/PointsScoredYearCalculator.py
--rw-rw-rw-   0        0        0     6208 2023-05-11 04:22:19.000000 leeger-2.5.1/leeger/calculator/year_calculator/SSLYearCalculator.py
--rw-rw-rw-   0        0        0     8945 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/calculator/year_calculator/ScoringShareYearCalculator.py
--rw-rw-rw-   0        0        0     2396 2023-05-11 04:22:19.000000 leeger-2.5.1/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py
--rw-rw-rw-   0        0        0     2973 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/calculator/year_calculator/SingleScoreYearCalculator.py
--rw-rw-rw-   0        0        0     8392 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/calculator/year_calculator/SmartWinsYearCalculator.py
--rw-rw-rw-   0        0        0     1699 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py
--rw-rw-rw-   0        0        0      652 2023-05-14 08:22:22.000000 leeger-2.5.1/leeger/calculator/year_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.690220 leeger-2.5.1/leeger/decorator/
--rw-rw-rw-   0        0        0       85 2023-05-14 08:22:22.000000 leeger-2.5.1/leeger/decorator/__init__.py
--rw-rw-rw-   0        0        0     4853 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/decorator/validators.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.694224 leeger-2.5.1/leeger/enum/
--rw-rw-rw-   0        0        0      784 2023-04-29 23:36:04.000000 leeger-2.5.1/leeger/enum/MatchupType.py
--rw-rw-rw-   0        0        0       38 2023-05-14 08:22:22.000000 leeger-2.5.1/leeger/enum/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.730225 leeger-2.5.1/leeger/exception/
--rw-rw-rw-   0        0        0      145 2023-05-28 03:17:48.000000 leeger-2.5.1/leeger/exception/DoesNotExistException.py
--rw-rw-rw-   0        0        0      131 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/exception/InvalidDivisionFormatException.py
--rw-rw-rw-   0        0        0      105 2023-05-28 03:17:48.000000 leeger-2.5.1/leeger/exception/InvalidFilterException.py
--rw-rw-rw-   0        0        0      126 2023-05-28 03:17:48.000000 leeger-2.5.1/leeger/exception/InvalidLeagueFormatException.py
--rw-rw-rw-   0        0        0      128 2023-05-28 03:17:48.000000 leeger-2.5.1/leeger/exception/InvalidMatchupFormatException.py
--rw-rw-rw-   0        0        0      125 2023-05-28 03:17:48.000000 leeger-2.5.1/leeger/exception/InvalidOwnerFormatException.py
--rw-rw-rw-   0        0        0      122 2023-05-28 03:17:48.000000 leeger-2.5.1/leeger/exception/InvalidTeamFormatException.py
--rw-rw-rw-   0        0        0      122 2023-05-28 03:17:48.000000 leeger-2.5.1/leeger/exception/InvalidWeekFormatException.py
--rw-rw-rw-   0        0        0      122 2023-05-28 03:17:48.000000 leeger-2.5.1/leeger/exception/InvalidYearFormatException.py
--rw-rw-rw-   0        0        0      138 2023-05-28 03:17:48.000000 leeger-2.5.1/leeger/exception/InvalidYearSettingsFormatException.py
--rw-rw-rw-   0        0        0      126 2023-04-29 23:36:04.000000 leeger-2.5.1/leeger/exception/LeagueLoaderException.py
--rw-rw-rw-   0        0        0      136 2023-04-29 23:36:04.000000 leeger-2.5.1/leeger/exception/UnsupportedLeegerFeatureException.py
--rw-rw-rw-   0        0        0      838 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.750221 leeger-2.5.1/leeger/league_loader/
--rw-rw-rw-   0        0        0    10201 2023-06-06 05:00:31.000000 leeger-2.5.1/leeger/league_loader/ESPNLeagueLoader.py
--rw-rw-rw-   0        0        0     9035 2023-06-06 05:00:40.000000 leeger-2.5.1/leeger/league_loader/FleaflickerLeagueLoader.py
--rw-rw-rw-   0        0        0     5393 2023-06-06 05:19:37.000000 leeger-2.5.1/leeger/league_loader/LeagueLoader.py
--rw-rw-rw-   0        0        0    11796 2023-06-06 05:00:47.000000 leeger-2.5.1/leeger/league_loader/MyFantasyLeagueLeagueLoader.py
--rw-rw-rw-   0        0        0    21640 2023-06-06 05:00:55.000000 leeger-2.5.1/leeger/league_loader/SleeperLeagueLoader.py
--rw-rw-rw-   0        0        0    11705 2023-06-06 05:01:02.000000 leeger-2.5.1/leeger/league_loader/YahooLeagueLoader.py
--rw-rw-rw-   0        0        0      222 2023-05-14 08:22:22.000000 leeger-2.5.1/leeger/league_loader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.753224 leeger-2.5.1/leeger/model/
--rw-rw-rw-   0        0        0        0 2022-08-13 05:54:09.000000 leeger-2.5.1/leeger/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.761225 leeger-2.5.1/leeger/model/abstract/
--rw-rw-rw-   0        0        0      469 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/model/abstract/EqualityCheck.py
--rw-rw-rw-   0        0        0      550 2023-02-17 18:45:58.000000 leeger-2.5.1/leeger/model/abstract/UniqueId.py
--rw-rw-rw-   0        0        0       32 2023-05-14 08:22:22.000000 leeger-2.5.1/leeger/model/abstract/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.774222 leeger-2.5.1/leeger/model/filter/
--rw-rw-rw-   0        0        0     5463 2023-05-27 03:21:06.000000 leeger-2.5.1/leeger/model/filter/AllTimeFilters.py
--rw-rw-rw-   0        0        0      321 2023-05-27 03:21:04.000000 leeger-2.5.1/leeger/model/filter/WeekFilters.py
--rw-rw-rw-   0        0        0     5141 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/model/filter/YearFilters.py
--rw-rw-rw-   0        0        0      120 2023-05-27 03:21:08.000000 leeger-2.5.1/leeger/model/filter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.797220 leeger-2.5.1/leeger/model/league/
--rw-rw-rw-   0        0        0     1644 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/model/league/Division.py
--rw-rw-rw-   0        0        0     7069 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/model/league/League.py
--rw-rw-rw-   0        0        0     4776 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/model/league/Matchup.py
--rw-rw-rw-   0        0        0     1593 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/model/league/Owner.py
--rw-rw-rw-   0        0        0     1884 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/model/league/Team.py
--rw-rw-rw-   0        0        0     4255 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/model/league/Week.py
--rw-rw-rw-   0        0        0     5383 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/model/league/Year.py
--rw-rw-rw-   0        0        0     1812 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/model/league/YearSettings.py
--rw-rw-rw-   0        0        0      228 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/model/league/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.803222 leeger-2.5.1/leeger/model/league_helper/
--rw-rw-rw-   0        0        0     3867 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/model/league_helper/Performance.py
--rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.5.1/leeger/model/league_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.811220 leeger-2.5.1/leeger/model/stat/
--rw-rw-rw-   0        0        0     3880 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/model/stat/AllTimeStatSheet.py
--rw-rw-rw-   0        0        0     4126 2023-05-28 03:02:41.000000 leeger-2.5.1/leeger/model/stat/YearStatSheet.py
--rw-rw-rw-   0        0        0       90 2023-05-14 08:22:22.000000 leeger-2.5.1/leeger/model/stat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.813224 leeger-2.5.1/leeger/properties/
--rw-rw-rw-   0        0        0       93 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/properties/app.properties
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.847224 leeger-2.5.1/leeger/util/
--rw-rw-rw-   0        0        0     1007 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/util/ConfigReader.py
--rw-rw-rw-   0        0        0     1114 2023-04-29 23:36:04.000000 leeger-2.5.1/leeger/util/CustomFormatter.py
--rw-rw-rw-   0        0        0      889 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/util/CustomLogger.py
--rw-rw-rw-   0        0        0      513 2022-06-11 23:09:37.000000 leeger-2.5.1/leeger/util/Deci.py
--rw-rw-rw-   0        0        0     4421 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/util/GeneralUtil.py
--rw-rw-rw-   0        0        0      237 2022-06-10 22:18:01.000000 leeger-2.5.1/leeger/util/IdGenerator.py
--rw-rw-rw-   0        0        0      296 2023-05-14 17:09:42.000000 leeger-2.5.1/leeger/util/JSONDeserializable.py
--rw-rw-rw-   0        0        0      262 2023-05-14 17:09:42.000000 leeger-2.5.1/leeger/util/JSONSerializable.py
--rw-rw-rw-   0        0        0        0 2022-08-13 05:54:20.000000 leeger-2.5.1/leeger/util/__init__.py
--rw-rw-rw-   0        0        0     3667 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/util/equality.py
--rw-rw-rw-   0        0        0    15086 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/util/excel.py
--rw-rw-rw-   0        0        0     9373 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/util/excel_helper.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.862225 leeger-2.5.1/leeger/util/navigator/
--rw-rw-rw-   0        0        0     5682 2023-05-11 04:22:19.000000 leeger-2.5.1/leeger/util/navigator/LeagueNavigator.py
--rw-rw-rw-   0        0        0     2071 2023-04-29 23:41:28.000000 leeger-2.5.1/leeger/util/navigator/MatchupNavigator.py
--rw-rw-rw-   0        0        0     2207 2023-04-29 23:41:27.000000 leeger-2.5.1/leeger/util/navigator/WeekNavigator.py
--rw-rw-rw-   0        0        0     7048 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/util/navigator/YearNavigator.py
--rw-rw-rw-   0        0        0      178 2023-05-14 08:22:22.000000 leeger-2.5.1/leeger/util/navigator/__init__.py
--rw-rw-rw-   0        0        0    11436 2023-04-29 23:41:28.000000 leeger-2.5.1/leeger/util/stat_sheet.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.885224 leeger-2.5.1/leeger/validate/
--rw-rw-rw-   0        0        0      258 2023-05-14 08:22:22.000000 leeger-2.5.1/leeger/validate/__init__.py
--rw-rw-rw-   0        0        0      529 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/validate/divisionValidation.py
--rw-rw-rw-   0        0        0     4583 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/validate/leagueValidation.py
--rw-rw-rw-   0        0        0     2481 2023-04-29 23:41:28.000000 leeger-2.5.1/leeger/validate/matchupValidation.py
--rw-rw-rw-   0        0        0      493 2023-04-29 23:41:28.000000 leeger-2.5.1/leeger/validate/ownerValidation.py
--rw-rw-rw-   0        0        0      744 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/validate/teamValidation.py
--rw-rw-rw-   0        0        0     4830 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/validate/weekValidation.py
--rw-rw-rw-   0        0        0      221 2023-05-14 17:09:42.000000 leeger-2.5.1/leeger/validate/yearSettingsValidation.py
--rw-rw-rw-   0        0        0    18614 2023-06-04 21:27:09.000000 leeger-2.5.1/leeger/validate/yearValidation.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.616220 leeger-2.5.1/leeger.egg-info/
--rw-rw-rw-   0        0        0     9890 2023-06-08 00:32:24.000000 leeger-2.5.1/leeger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8216 2023-06-08 00:32:24.000000 leeger-2.5.1/leeger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 00:32:24.000000 leeger-2.5.1/leeger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2023-06-08 00:32:24.000000 leeger-2.5.1/leeger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-08 00:32:24.000000 leeger-2.5.1/leeger.egg-info/top_level.txt
--rwxrwxrwx   0        0        0      231 2023-06-04 21:27:09.000000 leeger-2.5.1/main.bat
--rw-rw-rw-   0        0        0      217 2023-06-04 21:27:09.000000 leeger-2.5.1/pyproject.toml
--rw-rw-rw-   0        0        0      168 2023-06-04 21:27:09.000000 leeger-2.5.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 00:32:25.087222 leeger-2.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1048 2023-06-04 21:27:09.000000 leeger-2.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.542222 leeger-2.5.1/test/
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.888221 leeger-2.5.1/test/test_calculator/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.1/test/test_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.930224 leeger-2.5.1/test/test_calculator/test_all_time_calculator/
--rw-rw-rw-   0        0        0        0 2022-06-27 00:56:09.000000 leeger-2.5.1/test/test_calculator/test_all_time_calculator/__init__.py
--rw-rw-rw-   0        0        0    86146 2023-04-29 23:41:33.000000 leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py
--rw-rw-rw-   0        0        0   220423 2023-04-29 23:41:38.000000 leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py
--rw-rw-rw-   0        0        0    24301 2023-04-29 23:41:29.000000 leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py
--rw-rw-rw-   0        0        0    96680 2023-04-29 23:41:34.000000 leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py
--rw-rw-rw-   0        0        0    42298 2023-05-11 04:22:19.000000 leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py
--rw-rw-rw-   0        0        0   107979 2023-04-29 23:41:35.000000 leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py
--rw-rw-rw-   0        0        0    27851 2023-04-29 23:41:29.000000 leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py
--rw-rw-rw-   0        0        0    47446 2023-04-29 23:41:31.000000 leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py
--rw-rw-rw-   0        0        0   103504 2023-04-29 23:41:34.000000 leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py
--rw-rw-rw-   0        0        0    54546 2023-05-11 04:22:19.000000 leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.965223 leeger-2.5.1/test/test_calculator/test_year_calculator/
--rw-rw-rw-   0        0        0        0 2022-06-27 00:54:55.000000 leeger-2.5.1/test/test_calculator/test_year_calculator/__init__.py
--rw-rw-rw-   0        0        0   104455 2023-04-29 23:41:35.000000 leeger-2.5.1/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py
--rw-rw-rw-   0        0        0    84963 2023-04-29 23:41:33.000000 leeger-2.5.1/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py
--rw-rw-rw-   0        0        0     9711 2023-05-11 04:22:19.000000 leeger-2.5.1/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py
--rw-rw-rw-   0        0        0    39044 2023-05-11 04:22:19.000000 leeger-2.5.1/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py
--rw-rw-rw-   0        0        0    29836 2023-05-11 04:22:19.000000 leeger-2.5.1/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py
--rw-rw-rw-   0        0        0    44383 2023-05-11 04:22:19.000000 leeger-2.5.1/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py
--rw-rw-rw-   0        0        0    12194 2023-05-11 04:22:19.000000 leeger-2.5.1/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py
--rw-rw-rw-   0        0        0    35141 2023-05-11 04:22:19.000000 leeger-2.5.1/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py
--rw-rw-rw-   0        0        0    82020 2023-04-29 23:41:36.000000 leeger-2.5.1/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py
--rw-rw-rw-   0        0        0    21748 2023-05-11 04:22:19.000000 leeger-2.5.1/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.971223 leeger-2.5.1/test/test_decorator/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.1/test/test_decorator/__init__.py
--rw-rw-rw-   0        0        0     4803 2023-04-29 23:41:33.000000 leeger-2.5.1/test/test_decorator/test_validators.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.989222 leeger-2.5.1/test/test_league_loader/
--rw-rw-rw-   0        0        0        0 2022-06-25 00:07:47.000000 leeger-2.5.1/test/test_league_loader/__init__.py
--rw-rw-rw-   0        0        0    49779 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_league_loader/test_ESPNLeagueLoader.py
--rw-rw-rw-   0        0        0    50085 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_league_loader/test_FleaflickerLeagueLoader.py
--rw-rw-rw-   0        0        0     8165 2023-06-06 05:19:43.000000 leeger-2.5.1/test/test_league_loader/test_LeagueLoader.py
--rw-rw-rw-   0        0        0    94605 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py
--rw-rw-rw-   0        0        0   131293 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_league_loader/test_SleeperLeagueLoader.py
--rw-rw-rw-   0        0        0    63226 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_league_loader/test_YahooLeagueLoader.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.991222 leeger-2.5.1/test/test_model/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.1/test/test_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:24.995223 leeger-2.5.1/test/test_model/test_abstract/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.1/test/test_model/test_abstract/__init__.py
--rw-rw-rw-   0        0        0      932 2022-09-19 23:01:23.000000 leeger-2.5.1/test/test_model/test_abstract/test_UniqueId.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:25.000222 leeger-2.5.1/test/test_model/test_filter/
--rw-rw-rw-   0        0        0        0 2022-07-01 18:59:46.000000 leeger-2.5.1/test/test_model/test_filter/__init__.py
--rw-rw-rw-   0        0        0     2098 2023-04-29 23:41:33.000000 leeger-2.5.1/test/test_model/test_filter/test_AllTimeFilters.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:25.022221 leeger-2.5.1/test/test_model/test_league/
--rw-rw-rw-   0        0        0        0 2022-06-23 01:09:11.000000 leeger-2.5.1/test/test_model/test_league/__init__.py
--rw-rw-rw-   0        0        0     1333 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_model/test_league/test_Division.py
--rw-rw-rw-   0        0        0    23031 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_model/test_league/test_League.py
--rw-rw-rw-   0        0        0     9164 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_model/test_league/test_Matchup.py
--rw-rw-rw-   0        0        0     1477 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_model/test_league/test_Owner.py
--rw-rw-rw-   0        0        0     1434 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_model/test_league/test_Team.py
--rw-rw-rw-   0        0        0    10522 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_model/test_league/test_Week.py
--rw-rw-rw-   0        0        0     9195 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_model/test_league/test_Year.py
--rw-rw-rw-   0        0        0     1809 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_model/test_league/test_YearSettings.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:25.026220 leeger-2.5.1/test/test_model/test_league_helper/
--rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.5.1/test/test_model/test_league_helper/__init__.py
--rw-rw-rw-   0        0        0     6726 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_model/test_league_helper/test_Performance.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:25.046223 leeger-2.5.1/test/test_util/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.1/test/test_util/__init__.py
--rw-rw-rw-   0        0        0      471 2022-07-13 01:00:46.000000 leeger-2.5.1/test/test_util/test_Deci.py
--rw-rw-rw-   0        0        0     9143 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_util/test_GeneralUtil.py
--rw-rw-rw-   0        0        0      486 2022-07-13 01:00:45.000000 leeger-2.5.1/test/test_util/test_IdGenerator.py
--rw-rw-rw-   0        0        0     7379 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_util/test_equality.py
--rw-rw-rw-   0        0        0    65300 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_util/test_excel.py
--rw-rw-rw-   0        0        0     7246 2023-04-29 23:41:34.000000 leeger-2.5.1/test/test_util/test_excel_helper.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:25.058220 leeger-2.5.1/test/test_util/test_navigator/
--rw-rw-rw-   0        0        0        0 2022-08-12 22:44:07.000000 leeger-2.5.1/test/test_util/test_navigator/__init__.py
--rw-rw-rw-   0        0        0    52517 2023-04-29 23:41:36.000000 leeger-2.5.1/test/test_util/test_navigator/test_LeagueNavigator.py
--rw-rw-rw-   0        0        0     3970 2023-04-29 23:41:34.000000 leeger-2.5.1/test/test_util/test_navigator/test_MatchupNavigator.py
--rw-rw-rw-   0        0        0     6154 2023-04-29 23:41:34.000000 leeger-2.5.1/test/test_util/test_navigator/test_WeekNavigator.py
--rw-rw-rw-   0        0        0    29212 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_util/test_navigator/test_YearNavigator.py
--rw-rw-rw-   0        0        0    10570 2023-04-29 23:41:34.000000 leeger-2.5.1/test/test_util/test_stat_sheet.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:32:25.081225 leeger-2.5.1/test/test_validate/
--rw-rw-rw-   0        0        0        0 2022-08-12 22:13:02.000000 leeger-2.5.1/test/test_validate/__init__.py
--rw-rw-rw-   0        0        0      560 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_validate/test_divisionValidation.py
--rw-rw-rw-   0        0        0     9561 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_validate/test_leagueValidation.py
--rw-rw-rw-   0        0        0     4772 2023-05-11 04:22:19.000000 leeger-2.5.1/test/test_validate/test_matchupValidation.py
--rw-rw-rw-   0        0        0      530 2023-04-29 23:41:34.000000 leeger-2.5.1/test/test_validate/test_ownerValidation.py
--rw-rw-rw-   0        0        0     1174 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_validate/test_teamValidation.py
--rw-rw-rw-   0        0        0     6416 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_validate/test_weekValidation.py
--rw-rw-rw-   0        0        0      612 2023-02-17 19:20:44.000000 leeger-2.5.1/test/test_validate/test_yearSettingsValidation.py
--rw-rw-rw-   0        0        0    36250 2023-06-04 21:27:09.000000 leeger-2.5.1/test/test_validate/test_yearValidation.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.427210 leeger-2.5.2/
+-rw-rw-rw-   0        0        0     1088 2022-06-10 22:18:01.000000 leeger-2.5.2/LICENSE
+-rw-rw-rw-   0        0        0       87 2023-06-08 00:59:42.000000 leeger-2.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9890 2023-06-08 00:59:58.425211 leeger-2.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9480 2023-06-04 21:27:09.000000 leeger-2.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:57.954209 leeger-2.5.2/leeger/
+-rw-rw-rw-   0        0        0       43 2022-08-13 05:53:15.000000 leeger-2.5.2/leeger/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-06-08 00:44:26.000000 leeger-2.5.2/leeger/_version.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:57.993208 leeger-2.5.2/leeger/calculator/
+-rw-rw-rw-   0        0        0        0 2022-08-13 05:53:37.000000 leeger-2.5.2/leeger/calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.021210 leeger-2.5.2/leeger/calculator/all_time_calculator/
+-rw-rw-rw-   0        0        0     5029 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     9107 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     1318 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     4490 2023-05-11 04:22:19.000000 leeger-2.5.2/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     9320 2023-05-11 04:31:22.000000 leeger-2.5.2/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     8996 2023-05-11 04:31:22.000000 leeger-2.5.2/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     2644 2023-05-11 04:22:19.000000 leeger-2.5.2/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     3351 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     8906 2023-05-11 04:22:19.000000 leeger-2.5.2/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     1519 2023-05-11 04:22:19.000000 leeger-2.5.2/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py
+-rw-rw-rw-   0        0        0      712 2023-05-14 08:22:22.000000 leeger-2.5.2/leeger/calculator/all_time_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.027210 leeger-2.5.2/leeger/calculator/parent/
+-rw-rw-rw-   0        0        0    15345 2023-05-11 04:22:19.000000 leeger-2.5.2/leeger/calculator/parent/AllTimeCalculator.py
+-rw-rw-rw-   0        0        0     1671 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/calculator/parent/YearCalculator.py
+-rw-rw-rw-   0        0        0       94 2023-05-14 08:22:22.000000 leeger-2.5.2/leeger/calculator/parent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.054209 leeger-2.5.2/leeger/calculator/year_calculator/
+-rw-rw-rw-   0        0        0     9896 2023-05-11 04:22:19.000000 leeger-2.5.2/leeger/calculator/year_calculator/AWALYearCalculator.py
+-rw-rw-rw-   0        0        0    18719 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py
+-rw-rw-rw-   0        0        0     2018 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/calculator/year_calculator/PlusMinusYearCalculator.py
+-rw-rw-rw-   0        0        0     5843 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/calculator/year_calculator/PointsScoredYearCalculator.py
+-rw-rw-rw-   0        0        0     6208 2023-05-11 04:22:19.000000 leeger-2.5.2/leeger/calculator/year_calculator/SSLYearCalculator.py
+-rw-rw-rw-   0        0        0     8945 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/calculator/year_calculator/ScoringShareYearCalculator.py
+-rw-rw-rw-   0        0        0     2396 2023-05-11 04:22:19.000000 leeger-2.5.2/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py
+-rw-rw-rw-   0        0        0     2973 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/calculator/year_calculator/SingleScoreYearCalculator.py
+-rw-rw-rw-   0        0        0     8392 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/calculator/year_calculator/SmartWinsYearCalculator.py
+-rw-rw-rw-   0        0        0     1699 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py
+-rw-rw-rw-   0        0        0      652 2023-05-14 08:22:22.000000 leeger-2.5.2/leeger/calculator/year_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.059212 leeger-2.5.2/leeger/decorator/
+-rw-rw-rw-   0        0        0       85 2023-05-14 08:22:22.000000 leeger-2.5.2/leeger/decorator/__init__.py
+-rw-rw-rw-   0        0        0     4853 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/decorator/validators.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.064211 leeger-2.5.2/leeger/enum/
+-rw-rw-rw-   0        0        0      784 2023-04-29 23:36:04.000000 leeger-2.5.2/leeger/enum/MatchupType.py
+-rw-rw-rw-   0        0        0       38 2023-05-14 08:22:22.000000 leeger-2.5.2/leeger/enum/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.095209 leeger-2.5.2/leeger/exception/
+-rw-rw-rw-   0        0        0      145 2023-05-28 03:17:48.000000 leeger-2.5.2/leeger/exception/DoesNotExistException.py
+-rw-rw-rw-   0        0        0      131 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/exception/InvalidDivisionFormatException.py
+-rw-rw-rw-   0        0        0      105 2023-05-28 03:17:48.000000 leeger-2.5.2/leeger/exception/InvalidFilterException.py
+-rw-rw-rw-   0        0        0      126 2023-05-28 03:17:48.000000 leeger-2.5.2/leeger/exception/InvalidLeagueFormatException.py
+-rw-rw-rw-   0        0        0      128 2023-05-28 03:17:48.000000 leeger-2.5.2/leeger/exception/InvalidMatchupFormatException.py
+-rw-rw-rw-   0        0        0      125 2023-05-28 03:17:48.000000 leeger-2.5.2/leeger/exception/InvalidOwnerFormatException.py
+-rw-rw-rw-   0        0        0      122 2023-05-28 03:17:48.000000 leeger-2.5.2/leeger/exception/InvalidTeamFormatException.py
+-rw-rw-rw-   0        0        0      122 2023-05-28 03:17:48.000000 leeger-2.5.2/leeger/exception/InvalidWeekFormatException.py
+-rw-rw-rw-   0        0        0      122 2023-05-28 03:17:48.000000 leeger-2.5.2/leeger/exception/InvalidYearFormatException.py
+-rw-rw-rw-   0        0        0      138 2023-05-28 03:17:48.000000 leeger-2.5.2/leeger/exception/InvalidYearSettingsFormatException.py
+-rw-rw-rw-   0        0        0      126 2023-04-29 23:36:04.000000 leeger-2.5.2/leeger/exception/LeagueLoaderException.py
+-rw-rw-rw-   0        0        0      136 2023-04-29 23:36:04.000000 leeger-2.5.2/leeger/exception/UnsupportedLeegerFeatureException.py
+-rw-rw-rw-   0        0        0      838 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/exception/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.112215 leeger-2.5.2/leeger/league_loader/
+-rw-rw-rw-   0        0        0    10201 2023-06-06 05:00:31.000000 leeger-2.5.2/leeger/league_loader/ESPNLeagueLoader.py
+-rw-rw-rw-   0        0        0     9035 2023-06-06 05:00:40.000000 leeger-2.5.2/leeger/league_loader/FleaflickerLeagueLoader.py
+-rw-rw-rw-   0        0        0     5393 2023-06-06 05:19:37.000000 leeger-2.5.2/leeger/league_loader/LeagueLoader.py
+-rw-rw-rw-   0        0        0    11796 2023-06-06 05:00:47.000000 leeger-2.5.2/leeger/league_loader/MyFantasyLeagueLeagueLoader.py
+-rw-rw-rw-   0        0        0    21640 2023-06-06 05:00:55.000000 leeger-2.5.2/leeger/league_loader/SleeperLeagueLoader.py
+-rw-rw-rw-   0        0        0    11705 2023-06-06 05:01:02.000000 leeger-2.5.2/leeger/league_loader/YahooLeagueLoader.py
+-rw-rw-rw-   0        0        0      222 2023-05-14 08:22:22.000000 leeger-2.5.2/leeger/league_loader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.115211 leeger-2.5.2/leeger/model/
+-rw-rw-rw-   0        0        0        0 2022-08-13 05:54:09.000000 leeger-2.5.2/leeger/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.122210 leeger-2.5.2/leeger/model/abstract/
+-rw-rw-rw-   0        0        0      469 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/model/abstract/EqualityCheck.py
+-rw-rw-rw-   0        0        0      550 2023-02-17 18:45:58.000000 leeger-2.5.2/leeger/model/abstract/UniqueId.py
+-rw-rw-rw-   0        0        0       32 2023-05-14 08:22:22.000000 leeger-2.5.2/leeger/model/abstract/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.132212 leeger-2.5.2/leeger/model/filter/
+-rw-rw-rw-   0        0        0     5463 2023-05-27 03:21:06.000000 leeger-2.5.2/leeger/model/filter/AllTimeFilters.py
+-rw-rw-rw-   0        0        0      321 2023-05-27 03:21:04.000000 leeger-2.5.2/leeger/model/filter/WeekFilters.py
+-rw-rw-rw-   0        0        0     5141 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/model/filter/YearFilters.py
+-rw-rw-rw-   0        0        0      120 2023-05-27 03:21:08.000000 leeger-2.5.2/leeger/model/filter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.154212 leeger-2.5.2/leeger/model/league/
+-rw-rw-rw-   0        0        0     1644 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/model/league/Division.py
+-rw-rw-rw-   0        0        0     7069 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/model/league/League.py
+-rw-rw-rw-   0        0        0     4776 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/model/league/Matchup.py
+-rw-rw-rw-   0        0        0     1593 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/model/league/Owner.py
+-rw-rw-rw-   0        0        0     1884 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/model/league/Team.py
+-rw-rw-rw-   0        0        0     4255 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/model/league/Week.py
+-rw-rw-rw-   0        0        0     5383 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/model/league/Year.py
+-rw-rw-rw-   0        0        0     1812 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/model/league/YearSettings.py
+-rw-rw-rw-   0        0        0      228 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/model/league/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.159210 leeger-2.5.2/leeger/model/league_helper/
+-rw-rw-rw-   0        0        0     3867 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/model/league_helper/Performance.py
+-rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.5.2/leeger/model/league_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.166208 leeger-2.5.2/leeger/model/stat/
+-rw-rw-rw-   0        0        0     3880 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/model/stat/AllTimeStatSheet.py
+-rw-rw-rw-   0        0        0     4126 2023-05-28 03:02:41.000000 leeger-2.5.2/leeger/model/stat/YearStatSheet.py
+-rw-rw-rw-   0        0        0       90 2023-05-14 08:22:22.000000 leeger-2.5.2/leeger/model/stat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.168214 leeger-2.5.2/leeger/properties/
+-rw-rw-rw-   0        0        0       93 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/properties/app.properties
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.200208 leeger-2.5.2/leeger/util/
+-rw-rw-rw-   0        0        0     1007 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/util/ConfigReader.py
+-rw-rw-rw-   0        0        0     1114 2023-04-29 23:36:04.000000 leeger-2.5.2/leeger/util/CustomFormatter.py
+-rw-rw-rw-   0        0        0      889 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/util/CustomLogger.py
+-rw-rw-rw-   0        0        0      513 2022-06-11 23:09:37.000000 leeger-2.5.2/leeger/util/Deci.py
+-rw-rw-rw-   0        0        0     4421 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/util/GeneralUtil.py
+-rw-rw-rw-   0        0        0      237 2022-06-10 22:18:01.000000 leeger-2.5.2/leeger/util/IdGenerator.py
+-rw-rw-rw-   0        0        0      296 2023-05-14 17:09:42.000000 leeger-2.5.2/leeger/util/JSONDeserializable.py
+-rw-rw-rw-   0        0        0      262 2023-05-14 17:09:42.000000 leeger-2.5.2/leeger/util/JSONSerializable.py
+-rw-rw-rw-   0        0        0        0 2022-08-13 05:54:20.000000 leeger-2.5.2/leeger/util/__init__.py
+-rw-rw-rw-   0        0        0     3667 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/util/equality.py
+-rw-rw-rw-   0        0        0    15086 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/util/excel.py
+-rw-rw-rw-   0        0        0     9373 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/util/excel_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.217211 leeger-2.5.2/leeger/util/navigator/
+-rw-rw-rw-   0        0        0     5682 2023-05-11 04:22:19.000000 leeger-2.5.2/leeger/util/navigator/LeagueNavigator.py
+-rw-rw-rw-   0        0        0     2071 2023-04-29 23:41:28.000000 leeger-2.5.2/leeger/util/navigator/MatchupNavigator.py
+-rw-rw-rw-   0        0        0     2207 2023-04-29 23:41:27.000000 leeger-2.5.2/leeger/util/navigator/WeekNavigator.py
+-rw-rw-rw-   0        0        0     7048 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/util/navigator/YearNavigator.py
+-rw-rw-rw-   0        0        0      178 2023-05-14 08:22:22.000000 leeger-2.5.2/leeger/util/navigator/__init__.py
+-rw-rw-rw-   0        0        0    11436 2023-04-29 23:41:28.000000 leeger-2.5.2/leeger/util/stat_sheet.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.241208 leeger-2.5.2/leeger/validate/
+-rw-rw-rw-   0        0        0      258 2023-05-14 08:22:22.000000 leeger-2.5.2/leeger/validate/__init__.py
+-rw-rw-rw-   0        0        0      529 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/validate/divisionValidation.py
+-rw-rw-rw-   0        0        0     4583 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/validate/leagueValidation.py
+-rw-rw-rw-   0        0        0     2481 2023-04-29 23:41:28.000000 leeger-2.5.2/leeger/validate/matchupValidation.py
+-rw-rw-rw-   0        0        0      493 2023-04-29 23:41:28.000000 leeger-2.5.2/leeger/validate/ownerValidation.py
+-rw-rw-rw-   0        0        0      744 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/validate/teamValidation.py
+-rw-rw-rw-   0        0        0     4830 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/validate/weekValidation.py
+-rw-rw-rw-   0        0        0      221 2023-05-14 17:09:42.000000 leeger-2.5.2/leeger/validate/yearSettingsValidation.py
+-rw-rw-rw-   0        0        0    18614 2023-06-04 21:27:09.000000 leeger-2.5.2/leeger/validate/yearValidation.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:57.991211 leeger-2.5.2/leeger.egg-info/
+-rw-rw-rw-   0        0        0     9890 2023-06-08 00:59:57.000000 leeger-2.5.2/leeger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8207 2023-06-08 00:59:57.000000 leeger-2.5.2/leeger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 00:59:57.000000 leeger-2.5.2/leeger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2023-06-08 00:59:57.000000 leeger-2.5.2/leeger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-08 00:59:57.000000 leeger-2.5.2/leeger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      217 2023-06-04 21:27:09.000000 leeger-2.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0      168 2023-06-04 21:27:09.000000 leeger-2.5.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 00:59:58.427210 leeger-2.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1048 2023-06-04 21:27:09.000000 leeger-2.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:57.933213 leeger-2.5.2/test/
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.244210 leeger-2.5.2/test/test_calculator/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.2/test/test_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.274211 leeger-2.5.2/test/test_calculator/test_all_time_calculator/
+-rw-rw-rw-   0        0        0        0 2022-06-27 00:56:09.000000 leeger-2.5.2/test/test_calculator/test_all_time_calculator/__init__.py
+-rw-rw-rw-   0        0        0    86146 2023-04-29 23:41:33.000000 leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py
+-rw-rw-rw-   0        0        0   220423 2023-04-29 23:41:38.000000 leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    24301 2023-04-29 23:41:29.000000 leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    96680 2023-04-29 23:41:34.000000 leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    42298 2023-05-11 04:22:19.000000 leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py
+-rw-rw-rw-   0        0        0   107979 2023-04-29 23:41:35.000000 leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    27851 2023-04-29 23:41:29.000000 leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    47446 2023-04-29 23:41:31.000000 leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py
+-rw-rw-rw-   0        0        0   103504 2023-04-29 23:41:34.000000 leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    54546 2023-05-11 04:22:19.000000 leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.305210 leeger-2.5.2/test/test_calculator/test_year_calculator/
+-rw-rw-rw-   0        0        0        0 2022-06-27 00:54:55.000000 leeger-2.5.2/test/test_calculator/test_year_calculator/__init__.py
+-rw-rw-rw-   0        0        0   104455 2023-04-29 23:41:35.000000 leeger-2.5.2/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py
+-rw-rw-rw-   0        0        0    84963 2023-04-29 23:41:33.000000 leeger-2.5.2/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py
+-rw-rw-rw-   0        0        0     9711 2023-05-11 04:22:19.000000 leeger-2.5.2/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py
+-rw-rw-rw-   0        0        0    39044 2023-05-11 04:22:19.000000 leeger-2.5.2/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py
+-rw-rw-rw-   0        0        0    29836 2023-05-11 04:22:19.000000 leeger-2.5.2/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py
+-rw-rw-rw-   0        0        0    44383 2023-05-11 04:22:19.000000 leeger-2.5.2/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py
+-rw-rw-rw-   0        0        0    12194 2023-05-11 04:22:19.000000 leeger-2.5.2/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py
+-rw-rw-rw-   0        0        0    35141 2023-05-11 04:22:19.000000 leeger-2.5.2/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py
+-rw-rw-rw-   0        0        0    82020 2023-04-29 23:41:36.000000 leeger-2.5.2/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py
+-rw-rw-rw-   0        0        0    21748 2023-05-11 04:22:19.000000 leeger-2.5.2/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.310208 leeger-2.5.2/test/test_decorator/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.2/test/test_decorator/__init__.py
+-rw-rw-rw-   0        0        0     4803 2023-04-29 23:41:33.000000 leeger-2.5.2/test/test_decorator/test_validators.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.330211 leeger-2.5.2/test/test_league_loader/
+-rw-rw-rw-   0        0        0        0 2022-06-25 00:07:47.000000 leeger-2.5.2/test/test_league_loader/__init__.py
+-rw-rw-rw-   0        0        0    49779 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_league_loader/test_ESPNLeagueLoader.py
+-rw-rw-rw-   0        0        0    50085 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_league_loader/test_FleaflickerLeagueLoader.py
+-rw-rw-rw-   0        0        0     8165 2023-06-06 05:19:43.000000 leeger-2.5.2/test/test_league_loader/test_LeagueLoader.py
+-rw-rw-rw-   0        0        0    94605 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py
+-rw-rw-rw-   0        0        0   131293 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_league_loader/test_SleeperLeagueLoader.py
+-rw-rw-rw-   0        0        0    63226 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_league_loader/test_YahooLeagueLoader.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.333211 leeger-2.5.2/test/test_model/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.2/test/test_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.337210 leeger-2.5.2/test/test_model/test_abstract/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.2/test/test_model/test_abstract/__init__.py
+-rw-rw-rw-   0        0        0      932 2022-09-19 23:01:23.000000 leeger-2.5.2/test/test_model/test_abstract/test_UniqueId.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.341215 leeger-2.5.2/test/test_model/test_filter/
+-rw-rw-rw-   0        0        0        0 2022-07-01 18:59:46.000000 leeger-2.5.2/test/test_model/test_filter/__init__.py
+-rw-rw-rw-   0        0        0     2098 2023-04-29 23:41:33.000000 leeger-2.5.2/test/test_model/test_filter/test_AllTimeFilters.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.363210 leeger-2.5.2/test/test_model/test_league/
+-rw-rw-rw-   0        0        0        0 2022-06-23 01:09:11.000000 leeger-2.5.2/test/test_model/test_league/__init__.py
+-rw-rw-rw-   0        0        0     1333 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_model/test_league/test_Division.py
+-rw-rw-rw-   0        0        0    23031 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_model/test_league/test_League.py
+-rw-rw-rw-   0        0        0     9164 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_model/test_league/test_Matchup.py
+-rw-rw-rw-   0        0        0     1477 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_model/test_league/test_Owner.py
+-rw-rw-rw-   0        0        0     1434 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_model/test_league/test_Team.py
+-rw-rw-rw-   0        0        0    10522 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_model/test_league/test_Week.py
+-rw-rw-rw-   0        0        0     9195 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_model/test_league/test_Year.py
+-rw-rw-rw-   0        0        0     1809 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_model/test_league/test_YearSettings.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.368211 leeger-2.5.2/test/test_model/test_league_helper/
+-rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.5.2/test/test_model/test_league_helper/__init__.py
+-rw-rw-rw-   0        0        0     6726 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_model/test_league_helper/test_Performance.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.388210 leeger-2.5.2/test/test_util/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.2/test/test_util/__init__.py
+-rw-rw-rw-   0        0        0      471 2022-07-13 01:00:46.000000 leeger-2.5.2/test/test_util/test_Deci.py
+-rw-rw-rw-   0        0        0     9143 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_util/test_GeneralUtil.py
+-rw-rw-rw-   0        0        0      486 2022-07-13 01:00:45.000000 leeger-2.5.2/test/test_util/test_IdGenerator.py
+-rw-rw-rw-   0        0        0     7379 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_util/test_equality.py
+-rw-rw-rw-   0        0        0    65300 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_util/test_excel.py
+-rw-rw-rw-   0        0        0     7246 2023-04-29 23:41:34.000000 leeger-2.5.2/test/test_util/test_excel_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.400210 leeger-2.5.2/test/test_util/test_navigator/
+-rw-rw-rw-   0        0        0        0 2022-08-12 22:44:07.000000 leeger-2.5.2/test/test_util/test_navigator/__init__.py
+-rw-rw-rw-   0        0        0    52517 2023-04-29 23:41:36.000000 leeger-2.5.2/test/test_util/test_navigator/test_LeagueNavigator.py
+-rw-rw-rw-   0        0        0     3970 2023-04-29 23:41:34.000000 leeger-2.5.2/test/test_util/test_navigator/test_MatchupNavigator.py
+-rw-rw-rw-   0        0        0     6154 2023-04-29 23:41:34.000000 leeger-2.5.2/test/test_util/test_navigator/test_WeekNavigator.py
+-rw-rw-rw-   0        0        0    29212 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_util/test_navigator/test_YearNavigator.py
+-rw-rw-rw-   0        0        0    10570 2023-04-29 23:41:34.000000 leeger-2.5.2/test/test_util/test_stat_sheet.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:59:58.422209 leeger-2.5.2/test/test_validate/
+-rw-rw-rw-   0        0        0        0 2022-08-12 22:13:02.000000 leeger-2.5.2/test/test_validate/__init__.py
+-rw-rw-rw-   0        0        0      560 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_validate/test_divisionValidation.py
+-rw-rw-rw-   0        0        0     9561 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_validate/test_leagueValidation.py
+-rw-rw-rw-   0        0        0     4772 2023-05-11 04:22:19.000000 leeger-2.5.2/test/test_validate/test_matchupValidation.py
+-rw-rw-rw-   0        0        0      530 2023-04-29 23:41:34.000000 leeger-2.5.2/test/test_validate/test_ownerValidation.py
+-rw-rw-rw-   0        0        0     1174 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_validate/test_teamValidation.py
+-rw-rw-rw-   0        0        0     6416 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_validate/test_weekValidation.py
+-rw-rw-rw-   0        0        0      612 2023-02-17 19:20:44.000000 leeger-2.5.2/test/test_validate/test_yearSettingsValidation.py
+-rw-rw-rw-   0        0        0    36250 2023-06-04 21:27:09.000000 leeger-2.5.2/test/test_validate/test_yearValidation.py
```

### Comparing `leeger-2.5.1/LICENSE` & `leeger-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/PKG-INFO` & `leeger-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leeger
-Version: 2.5.1
+Version: 2.5.2
 Summary: Instant stats for any fantasy football league.
 Home-page: https://github.com/joeyagreco/leeger
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: nfl statistics stats football espn yahoo sleeper myfantasyleague,fleaflicker
 Requires-Python: >=3.10
```

### Comparing `leeger-2.5.1/README.md` & `leeger-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py` & `leeger-2.5.2/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py` & `leeger-2.5.2/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py` & `leeger-2.5.2/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py` & `leeger-2.5.2/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py` & `leeger-2.5.2/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py` & `leeger-2.5.2/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py` & `leeger-2.5.2/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py` & `leeger-2.5.2/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py` & `leeger-2.5.2/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py` & `leeger-2.5.2/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/all_time_calculator/__init__.py` & `leeger-2.5.2/leeger/calculator/all_time_calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/parent/AllTimeCalculator.py` & `leeger-2.5.2/leeger/calculator/parent/AllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/parent/YearCalculator.py` & `leeger-2.5.2/leeger/calculator/parent/YearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/year_calculator/AWALYearCalculator.py` & `leeger-2.5.2/leeger/calculator/year_calculator/AWALYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py` & `leeger-2.5.2/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/year_calculator/PlusMinusYearCalculator.py` & `leeger-2.5.2/leeger/calculator/year_calculator/PlusMinusYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/year_calculator/PointsScoredYearCalculator.py` & `leeger-2.5.2/leeger/calculator/year_calculator/PointsScoredYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/year_calculator/SSLYearCalculator.py` & `leeger-2.5.2/leeger/calculator/year_calculator/SSLYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/year_calculator/ScoringShareYearCalculator.py` & `leeger-2.5.2/leeger/calculator/year_calculator/ScoringShareYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py` & `leeger-2.5.2/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/year_calculator/SingleScoreYearCalculator.py` & `leeger-2.5.2/leeger/calculator/year_calculator/SingleScoreYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/year_calculator/SmartWinsYearCalculator.py` & `leeger-2.5.2/leeger/calculator/year_calculator/SmartWinsYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py` & `leeger-2.5.2/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/calculator/year_calculator/__init__.py` & `leeger-2.5.2/leeger/calculator/year_calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/decorator/validators.py` & `leeger-2.5.2/leeger/decorator/validators.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/enum/MatchupType.py` & `leeger-2.5.2/leeger/enum/MatchupType.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/exception/__init__.py` & `leeger-2.5.2/leeger/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/league_loader/ESPNLeagueLoader.py` & `leeger-2.5.2/leeger/league_loader/ESPNLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/league_loader/FleaflickerLeagueLoader.py` & `leeger-2.5.2/leeger/league_loader/FleaflickerLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/league_loader/LeagueLoader.py` & `leeger-2.5.2/leeger/league_loader/LeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/league_loader/MyFantasyLeagueLeagueLoader.py` & `leeger-2.5.2/leeger/league_loader/MyFantasyLeagueLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/league_loader/SleeperLeagueLoader.py` & `leeger-2.5.2/leeger/league_loader/SleeperLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/league_loader/YahooLeagueLoader.py` & `leeger-2.5.2/leeger/league_loader/YahooLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/model/abstract/UniqueId.py` & `leeger-2.5.2/leeger/model/abstract/UniqueId.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/model/filter/AllTimeFilters.py` & `leeger-2.5.2/leeger/model/filter/AllTimeFilters.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/model/filter/YearFilters.py` & `leeger-2.5.2/leeger/model/filter/YearFilters.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/model/league/Division.py` & `leeger-2.5.2/leeger/model/league/Division.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/model/league/League.py` & `leeger-2.5.2/leeger/model/league/League.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/model/league/Matchup.py` & `leeger-2.5.2/leeger/model/league/Matchup.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/model/league/Owner.py` & `leeger-2.5.2/leeger/model/league/Owner.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/model/league/Team.py` & `leeger-2.5.2/leeger/model/league/Team.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/model/league/Week.py` & `leeger-2.5.2/leeger/model/league/Week.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/model/league/Year.py` & `leeger-2.5.2/leeger/model/league/Year.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/model/league/YearSettings.py` & `leeger-2.5.2/leeger/model/league/YearSettings.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/model/league_helper/Performance.py` & `leeger-2.5.2/leeger/model/league_helper/Performance.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/model/stat/AllTimeStatSheet.py` & `leeger-2.5.2/leeger/model/stat/AllTimeStatSheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/model/stat/YearStatSheet.py` & `leeger-2.5.2/leeger/model/stat/YearStatSheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/util/ConfigReader.py` & `leeger-2.5.2/leeger/util/ConfigReader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/util/CustomFormatter.py` & `leeger-2.5.2/leeger/util/CustomFormatter.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/util/CustomLogger.py` & `leeger-2.5.2/leeger/util/CustomLogger.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/util/Deci.py` & `leeger-2.5.2/leeger/util/Deci.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/util/GeneralUtil.py` & `leeger-2.5.2/leeger/util/GeneralUtil.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/util/equality.py` & `leeger-2.5.2/leeger/util/equality.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/util/excel.py` & `leeger-2.5.2/leeger/util/excel.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/util/excel_helper.py` & `leeger-2.5.2/leeger/util/excel_helper.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/util/navigator/LeagueNavigator.py` & `leeger-2.5.2/leeger/util/navigator/LeagueNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/util/navigator/MatchupNavigator.py` & `leeger-2.5.2/leeger/util/navigator/MatchupNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/util/navigator/WeekNavigator.py` & `leeger-2.5.2/leeger/util/navigator/WeekNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/util/navigator/YearNavigator.py` & `leeger-2.5.2/leeger/util/navigator/YearNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/util/stat_sheet.py` & `leeger-2.5.2/leeger/util/stat_sheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/validate/divisionValidation.py` & `leeger-2.5.2/leeger/validate/divisionValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/validate/leagueValidation.py` & `leeger-2.5.2/leeger/validate/leagueValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/validate/matchupValidation.py` & `leeger-2.5.2/leeger/validate/matchupValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/validate/teamValidation.py` & `leeger-2.5.2/leeger/validate/teamValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/validate/weekValidation.py` & `leeger-2.5.2/leeger/validate/weekValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger/validate/yearValidation.py` & `leeger-2.5.2/leeger/validate/yearValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/leeger.egg-info/PKG-INFO` & `leeger-2.5.2/leeger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leeger
-Version: 2.5.1
+Version: 2.5.2
 Summary: Instant stats for any fantasy football league.
 Home-page: https://github.com/joeyagreco/leeger
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: nfl statistics stats football espn yahoo sleeper myfantasyleague,fleaflicker
 Requires-Python: >=3.10
```

### Comparing `leeger-2.5.1/leeger.egg-info/SOURCES.txt` & `leeger-2.5.2/leeger.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-main.bat
 pyproject.toml
 requirements.txt
 setup.py
 leeger/__init__.py
 leeger/_version.py
 leeger.egg-info/PKG-INFO
 leeger.egg-info/SOURCES.txt
```

### Comparing `leeger-2.5.1/setup.py` & `leeger-2.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py` & `leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py` & `leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py` & `leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py` & `leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py` & `leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py` & `leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py` & `leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py` & `leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py` & `leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py` & `leeger-2.5.2/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py` & `leeger-2.5.2/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py` & `leeger-2.5.2/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py` & `leeger-2.5.2/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py` & `leeger-2.5.2/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py` & `leeger-2.5.2/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py` & `leeger-2.5.2/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py` & `leeger-2.5.2/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py` & `leeger-2.5.2/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py` & `leeger-2.5.2/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py` & `leeger-2.5.2/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_decorator/test_validators.py` & `leeger-2.5.2/test/test_decorator/test_validators.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_league_loader/test_ESPNLeagueLoader.py` & `leeger-2.5.2/test/test_league_loader/test_ESPNLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_league_loader/test_FleaflickerLeagueLoader.py` & `leeger-2.5.2/test/test_league_loader/test_FleaflickerLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_league_loader/test_LeagueLoader.py` & `leeger-2.5.2/test/test_league_loader/test_LeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py` & `leeger-2.5.2/test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_league_loader/test_SleeperLeagueLoader.py` & `leeger-2.5.2/test/test_league_loader/test_SleeperLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_league_loader/test_YahooLeagueLoader.py` & `leeger-2.5.2/test/test_league_loader/test_YahooLeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_model/test_abstract/test_UniqueId.py` & `leeger-2.5.2/test/test_model/test_abstract/test_UniqueId.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_model/test_filter/test_AllTimeFilters.py` & `leeger-2.5.2/test/test_model/test_filter/test_AllTimeFilters.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_model/test_league/test_Division.py` & `leeger-2.5.2/test/test_model/test_league/test_Division.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_model/test_league/test_League.py` & `leeger-2.5.2/test/test_model/test_league/test_League.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_model/test_league/test_Matchup.py` & `leeger-2.5.2/test/test_model/test_league/test_Matchup.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_model/test_league/test_Owner.py` & `leeger-2.5.2/test/test_model/test_league/test_Owner.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_model/test_league/test_Team.py` & `leeger-2.5.2/test/test_model/test_league/test_Team.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_model/test_league/test_Week.py` & `leeger-2.5.2/test/test_model/test_league/test_Week.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_model/test_league/test_Year.py` & `leeger-2.5.2/test/test_model/test_league/test_Year.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_model/test_league/test_YearSettings.py` & `leeger-2.5.2/test/test_model/test_league/test_YearSettings.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_model/test_league_helper/test_Performance.py` & `leeger-2.5.2/test/test_model/test_league_helper/test_Performance.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_util/test_GeneralUtil.py` & `leeger-2.5.2/test/test_util/test_GeneralUtil.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_util/test_equality.py` & `leeger-2.5.2/test/test_util/test_equality.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_util/test_excel.py` & `leeger-2.5.2/test/test_util/test_excel.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_util/test_excel_helper.py` & `leeger-2.5.2/test/test_util/test_excel_helper.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_util/test_navigator/test_LeagueNavigator.py` & `leeger-2.5.2/test/test_util/test_navigator/test_LeagueNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_util/test_navigator/test_MatchupNavigator.py` & `leeger-2.5.2/test/test_util/test_navigator/test_MatchupNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_util/test_navigator/test_WeekNavigator.py` & `leeger-2.5.2/test/test_util/test_navigator/test_WeekNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_util/test_navigator/test_YearNavigator.py` & `leeger-2.5.2/test/test_util/test_navigator/test_YearNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_util/test_stat_sheet.py` & `leeger-2.5.2/test/test_util/test_stat_sheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_validate/test_divisionValidation.py` & `leeger-2.5.2/test/test_validate/test_divisionValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_validate/test_leagueValidation.py` & `leeger-2.5.2/test/test_validate/test_leagueValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_validate/test_matchupValidation.py` & `leeger-2.5.2/test/test_validate/test_matchupValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_validate/test_ownerValidation.py` & `leeger-2.5.2/test/test_validate/test_ownerValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_validate/test_teamValidation.py` & `leeger-2.5.2/test/test_validate/test_teamValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_validate/test_weekValidation.py` & `leeger-2.5.2/test/test_validate/test_weekValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_validate/test_yearSettingsValidation.py` & `leeger-2.5.2/test/test_validate/test_yearSettingsValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.5.1/test/test_validate/test_yearValidation.py` & `leeger-2.5.2/test/test_validate/test_yearValidation.py`

 * *Files identical despite different names*

