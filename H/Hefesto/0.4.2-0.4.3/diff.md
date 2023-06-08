# Comparing `tmp/Hefesto-0.4.2.tar.gz` & `tmp/Hefesto-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hefesto-0.4.2.tar", last modified: Mon May 29 11:02:09 2023, max compression
+gzip compressed data, was "Hefesto-0.4.3.tar", last modified: Thu Jun  8 12:02:56 2023, max compression
```

## Comparing `Hefesto-0.4.2.tar` & `Hefesto-0.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-05-29 11:02:09.147207 Hefesto-0.4.2/
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-05-29 11:02:09.143207 Hefesto-0.4.2/Hefesto/
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.2/Hefesto/__init__.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    10220 2023-05-29 11:01:36.000000 Hefesto-0.4.2/Hefesto/main.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     7518 2023-05-29 09:20:38.000000 Hefesto-0.4.2/Hefesto/template.py
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-05-29 11:02:09.147207 Hefesto-0.4.2/Hefesto.egg-info/
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-05-29 11:02:09.000000 Hefesto-0.4.2/Hefesto.egg-info/PKG-INFO
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-05-29 11:02:09.000000 Hefesto-0.4.2/Hefesto.egg-info/SOURCES.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-05-29 11:02:09.000000 Hefesto-0.4.2/Hefesto.egg-info/dependency_links.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-05-29 11:02:09.000000 Hefesto-0.4.2/Hefesto.egg-info/top_level.txt
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.2/MANIFEST.in
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-05-29 11:02:09.147207 Hefesto-0.4.2/PKG-INFO
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      719 2023-02-08 11:49:59.000000 Hefesto-0.4.2/README.md
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       31 2023-02-10 09:50:43.000000 Hefesto-0.4.2/requirements.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-05-29 11:02:09.147207 Hefesto-0.4.2/setup.cfg
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-05-29 11:01:40.000000 Hefesto-0.4.2/setup.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-08 12:02:56.097395 Hefesto-0.4.3/
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-08 12:02:56.097395 Hefesto-0.4.3/Hefesto/
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.3/Hefesto/__init__.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    11315 2023-06-08 12:02:08.000000 Hefesto-0.4.3/Hefesto/main.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     6796 2023-06-07 10:58:15.000000 Hefesto-0.4.3/Hefesto/template.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-08 12:02:56.097395 Hefesto-0.4.3/Hefesto.egg-info/
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-06-08 12:02:55.000000 Hefesto-0.4.3/Hefesto.egg-info/PKG-INFO
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-06-08 12:02:56.000000 Hefesto-0.4.3/Hefesto.egg-info/SOURCES.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-06-08 12:02:55.000000 Hefesto-0.4.3/Hefesto.egg-info/dependency_links.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-06-08 12:02:55.000000 Hefesto-0.4.3/Hefesto.egg-info/top_level.txt
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.3/MANIFEST.in
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-06-08 12:02:56.097395 Hefesto-0.4.3/PKG-INFO
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      719 2023-02-08 11:49:59.000000 Hefesto-0.4.3/README.md
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       22 2023-05-29 17:45:16.000000 Hefesto-0.4.3/requirements.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-06-08 12:02:56.097395 Hefesto-0.4.3/setup.cfg
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-06-08 12:02:36.000000 Hefesto-0.4.3/setup.py
```

### Comparing `Hefesto-0.4.2/Hefesto/main.py` & `Hefesto-0.4.3/Hefesto/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,47 +137,70 @@
             resulting_df.at[i, "uniqid"] = milisec()
 
         
         print("Structural transformation: Done")
         new = Hefesto.__init__(self, datainput= resulting_df, reset = True)
         return new
 
-    def cleanBlanks(self, resulting_df):
+    def cleanBlanks(self, resulting_df): # TODO solve the attribute_type value problem
 
         for row_final in resulting_df.iterrows():
-            if row_final[1]["value"] == None and row_final[1]["attribute_id"] == None and row_final[1]["comments"] == None and row_final[1]["agent_id"] == None:
+            if row_final[1]["value"] == None and row_final[1]["valueIRI"] == None and row_final[1]["comments"] == None and row_final[1]["agent_id"] == None:
                 resulting_df = resulting_df.drop(row_final[0])
         del resulting_df["value"]
+        del resulting_df["valueIRI"]
 
         return resulting_df
 
     def valueEdition(self, resulting_df):
 
+        # valueIRI 
+        valueRelation = {
+            "Sex":"attribute_type",
+            "Status":"attribute_type",
+            "Diagnosis":"attribute_type",
+            "Genetic":"attribute_id",
+            "Symptoms":"attribute_type",
+            "Imaging":"attribute_id",
+            "Clinical_trial":"attribute_type"
+        }
         # Datatype:
-        datatype_relationship = {
+        datatypeRelation = {
             "xsd:string":"value_string",
             "xsd:date" : "value_date",
             "xsd:float": "value_float",
             "xsd:integer":"value_integer"
         }
         
         # Value edition:
         for index, row in resulting_df.iterrows():
-            for k,v in datatype_relationship.items():
+            for k,v in datatypeRelation.items():
                 
                 # value ---> value_DATATYPE:
                 if row["value_datatype"] == k:
                     resulting_df.at[index, v] = resulting_df["value"][index]
                     resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
                 # enddate correction:
                 if row["startdate"] != None and row["enddate"] == None:
                     resulting_df.at[index,"enddate"] = resulting_df["startdate"][index]
                     resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
+            for k,v in valueRelation.items():
+                # valueIRI ---> attribute_id/value:
+                if row["model"] == k:
+                    resulting_df.at[index, v] = resulting_df["valueIRI"][index]
+                    resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
+
+            # attribute_id_value
+            if row["model"] == "Genetic":
+                resulting_df.at[index, "attribute_id_value"] = resulting_df["value"][index]
+                resulting_df.at[index, "value_string"] = None # Deleting the value_string in case it moves from value to value_string
+                resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
+
         return resulting_df
 
     def get_uri(self, col, ont):
 
         
         if not col in list(self.df_data.columns):
             sys.exit("ERROR: selected column doesnt exist")
@@ -249,21 +272,21 @@
         print("Replacement from " + key + "to "+ value + " at column " + col +": Done")
         new = Hefesto.__init__(self, datainput= self.df_data, reset = True)
         return new
         
 
 # # Test 1:
 
-# test = Hefesto(datainput = "../data/INPUT_DATA.csv")
-# transform = test.transform_Fiab()
+# test = Hefesto(datainput = "../data/INPUT_DATA_test.csv")
+# transform = test.transformFiab()
 # transform.to_csv ("../data/OUTPUT_DATA.csv", index = False, header=True)
 
 # # # Test 2
 # with open("../data/CDEconfig.yaml") as file:
 #     configuration = yaml.load(file, Loader=yaml.FullLoader)
 
 # test = Hefesto(datainput = "../data/INPUT_DATA2.csv")
-# transform = test.transform_shape(configuration=configuration, clean_blanks = True) #, clean_blanks=False
+# transform = test.transformShape(configuration=configuration, clean_blanks = True) #, clean_blanks=False
 # # label = test.get_label("output_type")
 # # url_from_label= test.get_uri("output_type_label","ncit")
 # # repl= test.replacement("output_type_label", "Date","DateXXX", duplicate=False)
 # transform.to_csv ("../data/OUTPUT_DATA2.csv", index = False, header=True)
```

### Comparing `Hefesto-0.4.2/Hefesto/template.py` & `Hefesto-0.4.3/Hefesto/template.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,172 +2,149 @@
 class Template:
 
   template_model = dict(
 
     Birthyear = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_id = "http://purl.obolibrary.org/obo/NCIT_C83164",
+      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C83164",
       value_datatype = "xsd:integer",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Birthdate = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_id = "http://purl.obolibrary.org/obo/NCIT_C68615",
+      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C68615",
       value_datatype = "xsd:date",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Deathdate = dict( 
       process_type= "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type= "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_id = "http://purl.obolibrary.org/obo/NCIT_C70810",
+      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C70810",
       value_datatype = "xsd:date",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     First_visit = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_id = "http://purl.obolibrary.org/obo/NCIT_C164021",
+      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C164021",
       value_datatype = "xsd:date",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Sex = dict( 
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C28421",
+      attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C28421",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
 
     Status = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C166244",
+      attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C166244",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Diagnosis = dict(
       process_type= "http://purl.obolibrary.org/obo/NCIT_C15220",
       output_type= "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C2991",
+      attribute_type2= "http://purl.obolibrary.org/obo/NCIT_C2991",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
-    # Onset_diagnosis = dict(
-    #   process_type= "http://purl.obolibrary.org/obo/NCIT_C142470",
-    #   output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-    #   attribute_type= "http://purl.obolibrary.org/obo/NCIT_C164339",
-    #   value_datatype = "xsd:date",
-    #   startdate = None,
-    #   enddate = None,
-    #   pid = None,
-    #   context_id = None
-    # ),
-
-    Symptoms_onset_date = dict(
-      process_type= "http://purl.obolibrary.org/obo/NCIT_C142470",
-      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C124353",
-      attribute_id= "http://purl.obolibrary.org/obo/NCIT_C119242",
-      value_datatype = "xsd:date",
-      startdate = None,
-      enddate = None,
-      pid = None,
-      context_id = None
-    ),
-
-    Symptoms_onset_age = dict(
-      process_type= "http://purl.obolibrary.org/obo/NCIT_C142470",
+    Symptoms = dict(
+      process_type= "http://purl.obolibrary.org/obo/NCIT_C15220",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C124353",
-      attribute_id= "http://purl.obolibrary.org/obo/NCIT_C174273",
-      value_datatype = "xsd:float",
+      attribute_type2= "http://purl.obolibrary.org/obo/NCIT_C100104",
+      value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Genetic = dict(
       process_type= "http://purl.obolibrary.org/obo/NCIT_C15709",
       output_type= "http://purl.obolibrary.org/obo/NCIT_C70856",
       attribute_type= "http://purl.obolibrary.org/obo/NCIT_C103223",
+      attribute_id_type = "http://purl.obolibrary.org/obo/NCIT_C45766",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Consent_contacted = dict(
       process_type= "http://purl.obolibrary.org/obo/OBI_0000810",
       output_type = "http://purl.obolibrary.org/obo/OBIB_0000488",
-      attribute_id= "http://purl.obolibrary.org/obo/NCIT_C25460",
+      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25460",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Consent_used = dict(
       process_type= "http://purl.obolibrary.org/obo/OBI_0000810",
       output_type = "http://purl.obolibrary.org/obo/DUO_0000001",
-      attribute_id= "http://purl.obolibrary.org/obo/NCIT_C25460",
+      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25460",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Biobank = dict(
       process_type= "http://purl.obolibrary.org/obo/OMIABIS_0000061",
       output_type= "http://purl.obolibrary.org/obo/NCIT_C115570",
-      attribute_id= "http://purl.obolibrary.org/obo/NCIT_C25429",
+      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25429",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Disability = dict(
       process_type = None,
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_id = "http://purl.obolibrary.org/obo/NCIT_C21007",
+      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C21007",
       value_datatype = "xsd:float",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
@@ -194,15 +171,16 @@
       context_id= None 
     ),
 
 
     Imaging = dict(
       process_type = None ,
       output_type =  "http://purl.obolibrary.org/obo/NCIT_C70856" ,
-      attribute_id = "http://purl.obolibrary.org/obo/NCIT_C176708",
+      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C176708",
+      attribute_id_type = "http://purl.obolibrary.org/obo/NCIT_C81289",
       value_datatype = "xsd:string" ,
       startdate= None ,
       enddate= None ,
       comments= None ,
       pid = None ,
       context_id= None 
     ),
@@ -217,15 +195,15 @@
       context_id= None 
     ),
 
 
     Clinical_trial = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C71104" ,
       output_type=  "http://purl.obolibrary.org/obo/NCIT_C115575" ,
-      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C2991" ,
+      attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C2991" ,
       agent_type = "http://purl.obolibrary.org/obo/NCIT_C16696" ,
       value_datatype= "xsd:string",
       startdate= None ,
       enddate= None ,
       comments= None ,
       pid= None ,
       context_id= None
```

### Comparing `Hefesto-0.4.2/README.md` & `Hefesto-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `Hefesto-0.4.2/setup.py` & `Hefesto-0.4.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #     readme = readme_file.read()
 
 # with open('requirements.txt') as f:
 #     requirements = f.read().splitlines()
 
 setup(
     name="Hefesto",
-    version="0.4.2",
+    version="0.4.3",
     packages=["Hefesto"],
     author="Pablo Alarcón Moreno",
     author_email="pabloalarconmoreno@gmail.com",
     url="https://github.com/pabloalarconm/hefesto",
     description="Preprocessing datatable toolkit",
     license="MIT",
     keywords=["EJP","CDE"]
```

