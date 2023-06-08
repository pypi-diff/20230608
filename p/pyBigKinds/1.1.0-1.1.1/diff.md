# Comparing `tmp/pyBigKinds-1.1.0-py3-none-any.whl.zip` & `tmp/pyBigKinds-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7585 bytes, number of entries: 11
--rw-r--r--  2.0 unx      783 b- defN 23-Jun-08 16:52 pyBigKinds/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-08 16:52 pyBigKinds/_version.py
--rw-r--r--  2.0 unx     2475 b- defN 23-Jun-08 16:52 pyBigKinds/base.py
--rw-r--r--  2.0 unx     2552 b- defN 23-Jun-08 16:52 pyBigKinds/preprocessing.py
--rw-r--r--  2.0 unx     4080 b- defN 23-Jun-08 16:52 pyBigKinds/representation.py
--rw-r--r--  2.0 unx     2374 b- defN 23-Jun-08 16:52 pyBigKinds/visualization.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Jun-08 16:53 pyBigKinds-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1601 b- defN 23-Jun-08 16:53 pyBigKinds-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 16:53 pyBigKinds-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-08 16:53 pyBigKinds-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      884 b- defN 23-Jun-08 16:53 pyBigKinds-1.1.0.dist-info/RECORD
-11 files, 15944 bytes uncompressed, 6091 bytes compressed:  61.8%
+Zip file size: 7552 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      783 b- defN 23-Jun-08 17:25 pyBigKinds/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-08 17:25 pyBigKinds/_version.py
+-rw-r--r--  2.0 unx     2475 b- defN 23-Jun-08 17:25 pyBigKinds/base.py
+-rw-r--r--  2.0 unx     2552 b- defN 23-Jun-08 17:25 pyBigKinds/preprocessing.py
+-rw-r--r--  2.0 unx     4080 b- defN 23-Jun-08 17:25 pyBigKinds/representation.py
+-rw-r--r--  2.0 unx     2386 b- defN 23-Jun-08 17:25 pyBigKinds/visualization.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Jun-08 17:27 pyBigKinds-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1521 b- defN 23-Jun-08 17:27 pyBigKinds-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 17:27 pyBigKinds-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-08 17:27 pyBigKinds-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      884 b- defN 23-Jun-08 17:27 pyBigKinds-1.1.1.dist-info/RECORD
+11 files, 15876 bytes uncompressed, 6058 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: pyBigKinds/representation.py
 Comment: 
 
 Filename: pyBigKinds/visualization.py
 Comment: 
 
-Filename: pyBigKinds-1.1.0.dist-info/LICENSE
+Filename: pyBigKinds-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pyBigKinds-1.1.0.dist-info/METADATA
+Filename: pyBigKinds-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pyBigKinds-1.1.0.dist-info/WHEEL
+Filename: pyBigKinds-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyBigKinds-1.1.0.dist-info/top_level.txt
+Filename: pyBigKinds-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyBigKinds-1.1.0.dist-info/RECORD
+Filename: pyBigKinds-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyBigKinds/_version.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.0"
+__version__ = "1.1.1"
```

## pyBigKinds/visualization.py

```diff
@@ -26,15 +26,15 @@
 
 plt.rcParams["axes.unicode_minus"] = False
 
 
 def keywords_wordcloud(df, press):
     """언론사 별 키워드 워드클라우드 생성"""
     if isinstance(df, pd.DataFrame):
-        df_keywords = df[df[press] == press]
+        df_keywords = df[df["언론사"] == press]
         keywords = keyword_list(df_keywords)
         news_key = keyword_parser(keywords)
         news_key = duplication_remover(news_key)
         key = word_counter(news_key)
         news_key = counter_to_dataframe(key)
         wc = wordcloud.WordCloud(
             font_path=font_path,
@@ -49,15 +49,15 @@
     else:
         raise TypeError("input type is to be have to DataFrame")
 
 
 def top_words(df, press, top_n=25):
     """언론사 별 사용 단어 빈도 상위 n개"""
     if isinstance(df, pd.DataFrame):
-        df_keywords = df[df[press].str.contains(press)]
+        df_keywords = df[df["언론사"].str.contains(press)]
         keywords = keyword_list(df_keywords)
         news_key = keyword_parser(keywords)
         news_key = duplication_remover(news_key)
         key = word_counter(news_key)
         news_key = counter_to_dataframe(key)
 
         data = news_key.head(top_n)
```

## Comparing `pyBigKinds-1.1.0.dist-info/LICENSE` & `pyBigKinds-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyBigKinds-1.1.0.dist-info/METADATA` & `pyBigKinds-1.1.1.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBigKinds
-Version: 1.1.0
+Version: 1.1.1
 Summary: BigKinds Data Analysis Toolkit for python
 Home-page: https://github.com/sorrychoe/pyBigKinds
 Author: Sorrychoe
 License: MIT
 Project-URL: Source Code, https://github.com/sorrychoe/pyBigKinds
 Project-URL: Bug Tracker, https://github.com/sorrychoe/pyBigKinds/issues
 Keywords: Journalism,preprocessing-data,BigKinds
@@ -43,28 +43,20 @@
 
 - Windows, linux
 
   ```bash
   python -m pip install pyBigKinds
   ```
 
-## Example
+## Usage
 
-```python
-import pyBigKinds as bk
-
-bk.press_counter(df)
-
-```
-
-## Authors
-
-- [sorrychoe](https://www.github.com/sorrychoe)
+![](docs/example1.png)
+![](docs/example2.png)
 
 
 ## License
 
-- [MIT](https://choosealicense.com/licenses/mit/)
+[MIT](https://choosealicense.com/licenses/mit/)
 
 ## you have some issue?
 
 사용 중 문제 발생 시, 해당 Repo issue에 등록해주세요.
```

## Comparing `pyBigKinds-1.1.0.dist-info/RECORD` & `pyBigKinds-1.1.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pyBigKinds/__init__.py,sha256=3Trd45Kpi8CK1BvxsOR1d2Kf9v_wN3qdZLuVADyUwU4,783
-pyBigKinds/_version.py,sha256=LGVQyDsWifdACo7qztwb8RWWHds1E7uQ-ZqD8SAjyw4,22
+pyBigKinds/_version.py,sha256=q8_5C0f-8mHWNb6mMw02zlYPnEGXBqvOmP3z0CEwZKM,22
 pyBigKinds/base.py,sha256=KrKO3O1wpXvWr8TVq-3hl2JwwWu4l3lLBtpuXUyv1mg,2475
 pyBigKinds/preprocessing.py,sha256=4blorjI5OFdg99mgioKLnybbD_xlyjLctCIAx1Ut15U,2552
 pyBigKinds/representation.py,sha256=uFqybooPWrrHvKTy6rcjrKbuvb3ay3_pTv9ajZvdH1g,4080
-pyBigKinds/visualization.py,sha256=5HuguRxYlzLms6xDAp8SMwAl_-upCESrtz6_aDh5KIY,2374
-pyBigKinds-1.1.0.dist-info/LICENSE,sha256=4qpntoObC47xSDR5kl1lMvxC4Hz6PuFVKIthT3E3j8Y,1070
-pyBigKinds-1.1.0.dist-info/METADATA,sha256=JCBoJmF4CL1djPKWF-yh26x54UQrwwFSK_sy7Jxf18U,1601
-pyBigKinds-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyBigKinds-1.1.0.dist-info/top_level.txt,sha256=LDFcWpfU5Sf0n08ITRMJP20n-2u9ckNkEErPtU8iYbg,11
-pyBigKinds-1.1.0.dist-info/RECORD,,
+pyBigKinds/visualization.py,sha256=oSuvR2x64tSm6I11C-FG9z6WmAhUtz0KR4qTuvxXNWU,2386
+pyBigKinds-1.1.1.dist-info/LICENSE,sha256=4qpntoObC47xSDR5kl1lMvxC4Hz6PuFVKIthT3E3j8Y,1070
+pyBigKinds-1.1.1.dist-info/METADATA,sha256=jokaHRzrXRaW3T_2FEpSLAoGdCoLp1oXBg-KnpzPjPA,1521
+pyBigKinds-1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyBigKinds-1.1.1.dist-info/top_level.txt,sha256=LDFcWpfU5Sf0n08ITRMJP20n-2u9ckNkEErPtU8iYbg,11
+pyBigKinds-1.1.1.dist-info/RECORD,,
```

