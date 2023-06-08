# Comparing `tmp/econdata-1.0.3.tar.gz` & `tmp/econdata-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econdata-1.0.3.tar", last modified: Wed May 31 03:26:51 2023, max compression
+gzip compressed data, was "econdata-1.0.4.tar", last modified: Thu Jun  8 06:51:51 2023, max compression
```

## Comparing `econdata-1.0.3.tar` & `econdata-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 03:26:51.472361 econdata-1.0.3/
--rw-rw-rw-   0        0        0     2251 2023-05-31 03:26:51.471364 econdata-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1779 2023-05-31 03:25:02.000000 econdata-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-31 03:26:51.472361 econdata-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      908 2023-05-31 03:25:34.000000 econdata-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 03:26:51.248604 econdata-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 03:26:51.437085 econdata-1.0.3/src/econdata/
--rw-rw-rw-   0        0        0     6259 2023-05-31 03:24:33.000000 econdata-1.0.3/src/econdata/BCRP.py
--rw-rw-rw-   0        0        0     2820 2023-05-31 03:24:33.000000 econdata-1.0.3/src/econdata/BM.py
--rw-rw-rw-   0        0        0     4008 2023-05-31 03:24:33.000000 econdata-1.0.3/src/econdata/FRED.py
--rw-rw-rw-   0        0        0     2112 2023-05-31 03:24:33.000000 econdata-1.0.3/src/econdata/OECD.py
--rw-rw-rw-   0        0        0     3592 2023-05-31 03:24:33.000000 econdata-1.0.3/src/econdata/YFinance.py
--rw-rw-rw-   0        0        0        0 2023-05-31 03:24:33.000000 econdata-1.0.3/src/econdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 03:26:51.470366 econdata-1.0.3/src/econdata.egg-info/
--rw-rw-rw-   0        0        0     2251 2023-05-31 03:26:51.000000 econdata-1.0.3/src/econdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-05-31 03:26:51.000000 econdata-1.0.3/src/econdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 03:26:51.000000 econdata-1.0.3/src/econdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-31 03:26:51.000000 econdata-1.0.3/src/econdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 03:26:51.000000 econdata-1.0.3/src/econdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 06:51:51.660580 econdata-1.0.4/
+-rw-rw-rw-   0        0        0     2251 2023-06-08 06:51:51.660580 econdata-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1779 2023-06-08 06:49:59.000000 econdata-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 06:51:51.661593 econdata-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-06-08 06:49:43.000000 econdata-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:51:51.641646 econdata-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 06:51:51.651313 econdata-1.0.4/src/econdata/
+-rw-rw-rw-   0        0        0     6314 2023-06-08 06:47:58.000000 econdata-1.0.4/src/econdata/BCRP.py
+-rw-rw-rw-   0        0        0     2820 2023-06-08 06:47:12.000000 econdata-1.0.4/src/econdata/BM.py
+-rw-rw-rw-   0        0        0     4008 2023-06-08 06:47:12.000000 econdata-1.0.4/src/econdata/FRED.py
+-rw-rw-rw-   0        0        0     2112 2023-06-08 06:47:12.000000 econdata-1.0.4/src/econdata/OECD.py
+-rw-rw-rw-   0        0        0     3592 2023-06-08 06:47:12.000000 econdata-1.0.4/src/econdata/YFinance.py
+-rw-rw-rw-   0        0        0        0 2023-06-08 06:47:12.000000 econdata-1.0.4/src/econdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:51:51.659580 econdata-1.0.4/src/econdata.egg-info/
+-rw-rw-rw-   0        0        0     2251 2023-06-08 06:51:51.000000 econdata-1.0.4/src/econdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-06-08 06:51:51.000000 econdata-1.0.4/src/econdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 06:51:51.000000 econdata-1.0.4/src/econdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-08 06:51:51.000000 econdata-1.0.4/src/econdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 06:51:51.000000 econdata-1.0.4/src/econdata.egg-info/top_level.txt
```

### Comparing `econdata-1.0.3/PKG-INFO` & `econdata-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econdata
-Version: 1.0.3
+Version: 1.0.4
 Summary: Extracción de series de tiempo de las principales instituciones económicas para el Perú
 Home-page: https://github.com/mauricioalvaradoo/econdata
 Author: Mauricio Alvarado, Andrei Romero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -16,26 +16,26 @@
 2. Yahoo Finance
 3. Federal Reserve Economic Data (FRED)
 4. World Bank
 5. Organización para la Cooperación y el Desarrollo Económicos (OCDE)
 
 ```
 # Instalación mediante PyPI
-!pip install econdata==1.0.3
+!pip install econdata==1.0.4
 
 # o simplemente:
 !pip install econdata
 ```
 El anuncio fue realizado en Linkedin, y está disponible [aquí](https://www.linkedin.com/posts/mauricioalvaradoo_github-mauricioalvaradooecondata-extracci%C3%B3n-activity-7053798889950179328-wl5w?utm_source=share&utm_medium=member_desktop). 
 
 
-## Versión 1.0.3
+## Versión 1.0.4
 * Para el `BCRP`, `Yahoo Finance`, `FRED` y el `World Bank`, se cuenta con ambos métodos: `get_data()` y `search()`.
 * Para la `OCDE`, se cuenta únicamente con el método `get_data()`.
-* En la versión 1.0.3, (i) se corrigió el formato de las fechas para `BCRP` y `FRED`, y (ii) se añadió el filtro de frecuencia en `search()` para `FRED`.
+* En la versión 1.0.4, (i) se corrigió el formato de las fechas para `BCRP` y `FRED`, y (ii) se añadió el filtro de frecuencia en `search()` para `FRED`.
 
 
 ## Métodos
 Para cada institución se tiene dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
 get_data()
 ```
```

### Comparing `econdata-1.0.3/README.md` & `econdata-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 2. Yahoo Finance
 3. Federal Reserve Economic Data (FRED)
 4. World Bank
 5. Organización para la Cooperación y el Desarrollo Económicos (OCDE)
 
 ```
 # Instalación mediante PyPI
-!pip install econdata==1.0.3
+!pip install econdata==1.0.4
 
 # o simplemente:
 !pip install econdata
 ```
 El anuncio fue realizado en Linkedin, y está disponible [aquí](https://www.linkedin.com/posts/mauricioalvaradoo_github-mauricioalvaradooecondata-extracci%C3%B3n-activity-7053798889950179328-wl5w?utm_source=share&utm_medium=member_desktop). 
 
 
-## Versión 1.0.3
+## Versión 1.0.4
 * Para el `BCRP`, `Yahoo Finance`, `FRED` y el `World Bank`, se cuenta con ambos métodos: `get_data()` y `search()`.
 * Para la `OCDE`, se cuenta únicamente con el método `get_data()`.
-* En la versión 1.0.3, (i) se corrigió el formato de las fechas para `BCRP` y `FRED`, y (ii) se añadió el filtro de frecuencia en `search()` para `FRED`.
+* En la versión 1.0.4, (i) se corrigió el formato de las fechas para `BCRP` y `FRED`, y (ii) se añadió el filtro de frecuencia en `search()` para `FRED`.
 
 
 ## Métodos
 Para cada institución se tiene dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
 get_data()
 ```
```

### Comparing `econdata-1.0.3/setup.py` & `econdata-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='econdata',
-    version = '1.0.3',
+    version = '1.0.4',
     author = 'Mauricio Alvarado, Andrei Romero',
     description = 'Extracción de series de tiempo de las principales instituciones económicas para el Perú',
     long_description = long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mauricioalvaradoo/econdata',
     classifiers = [
         'Programming Language :: Python :: 3',
```

### Comparing `econdata-1.0.3/src/econdata/BCRP.py` & `econdata-1.0.4/src/econdata/BCRP.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         
     df.set_index("time", inplace=True)
     df.rename(series, axis=1, inplace=True)
 
 
     # Formatos de fechas
     if keys[0][-1] == 'D':
+        df.index = df.index.str.replace('Set', 'Sep')
         df.index = pd.to_datetime(df.index, format="%d.%b.%y")
     if keys[0][-1] == 'M':
         df.index = df.index.str.replace('Set', 'Sep')
         df.index = pd.to_datetime(df.index, format="%b.%Y")
     if keys[0][-1] == 'Q':
         try:
             df.index = pd.period_range(fechaini, fechafin, freq="Q")
```

### Comparing `econdata-1.0.3/src/econdata/BM.py` & `econdata-1.0.4/src/econdata/BM.py`

 * *Files identical despite different names*

### Comparing `econdata-1.0.3/src/econdata/FRED.py` & `econdata-1.0.4/src/econdata/FRED.py`

 * *Files identical despite different names*

### Comparing `econdata-1.0.3/src/econdata/OECD.py` & `econdata-1.0.4/src/econdata/OECD.py`

 * *Files identical despite different names*

### Comparing `econdata-1.0.3/src/econdata/YFinance.py` & `econdata-1.0.4/src/econdata/YFinance.py`

 * *Files identical despite different names*

### Comparing `econdata-1.0.3/src/econdata.egg-info/PKG-INFO` & `econdata-1.0.4/src/econdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econdata
-Version: 1.0.3
+Version: 1.0.4
 Summary: Extracción de series de tiempo de las principales instituciones económicas para el Perú
 Home-page: https://github.com/mauricioalvaradoo/econdata
 Author: Mauricio Alvarado, Andrei Romero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -16,26 +16,26 @@
 2. Yahoo Finance
 3. Federal Reserve Economic Data (FRED)
 4. World Bank
 5. Organización para la Cooperación y el Desarrollo Económicos (OCDE)
 
 ```
 # Instalación mediante PyPI
-!pip install econdata==1.0.3
+!pip install econdata==1.0.4
 
 # o simplemente:
 !pip install econdata
 ```
 El anuncio fue realizado en Linkedin, y está disponible [aquí](https://www.linkedin.com/posts/mauricioalvaradoo_github-mauricioalvaradooecondata-extracci%C3%B3n-activity-7053798889950179328-wl5w?utm_source=share&utm_medium=member_desktop). 
 
 
-## Versión 1.0.3
+## Versión 1.0.4
 * Para el `BCRP`, `Yahoo Finance`, `FRED` y el `World Bank`, se cuenta con ambos métodos: `get_data()` y `search()`.
 * Para la `OCDE`, se cuenta únicamente con el método `get_data()`.
-* En la versión 1.0.3, (i) se corrigió el formato de las fechas para `BCRP` y `FRED`, y (ii) se añadió el filtro de frecuencia en `search()` para `FRED`.
+* En la versión 1.0.4, (i) se corrigió el formato de las fechas para `BCRP` y `FRED`, y (ii) se añadió el filtro de frecuencia en `search()` para `FRED`.
 
 
 ## Métodos
 Para cada institución se tiene dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
 get_data()
 ```
```

