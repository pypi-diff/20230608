# Comparing `tmp/ladok3-3.6.tar.gz` & `tmp/ladok3-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ladok3-3.6.tar", max compression
+gzip compressed data, was "ladok3-3.7.tar", max compression
```

## Comparing `ladok3-3.6.tar` & `ladok3-3.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1155 2023-02-09 10:24:29.151703 ladok3-3.6/LICENSE
--rw-r--r--   0        0        0     6677 2022-10-25 12:52:56.416560 ladok3-3.6/README.md
--rw-r--r--   0        0        0      980 2023-02-09 10:25:13.624003 ladok3-3.6/doc/Makefile
--rw-r--r--   0        0        0      173 2022-10-25 09:48:40.909030 ladok3-3.6/doc/abstract.tex
--rw-r--r--   0        0        0     3723 2023-02-09 10:24:29.155703 ladok3-3.6/doc/ladok3.tex
--rw-r--r--   0        0        0     1160 2022-10-25 09:48:40.917030 ladok3-3.6/doc/preamble.tex
--rw-r--r--   0        0        0     3276 2022-10-25 09:54:49.529819 ladok3-3.6/makefiles/doc.mk
--rw-r--r--   0        0        0     1326 2022-10-20 12:02:01.907186 ladok3-3.6/makefiles/exam.mk
--rw-r--r--   0        0        0       66 2022-10-20 12:02:01.903186 ladok3-3.6/makefiles/haskell.mk
--rw-r--r--   0        0        0      820 2022-10-20 12:02:01.907186 ladok3-3.6/makefiles/miun.course.mk
--rw-r--r--   0        0        0     6206 2022-10-20 12:02:01.903186 ladok3-3.6/makefiles/miun.depend.mk
--rw-r--r--   0        0        0      664 2022-10-20 12:02:01.903186 ladok3-3.6/makefiles/miun.docs.mk
--rw-r--r--   0        0        0      611 2022-10-20 12:02:01.903186 ladok3-3.6/makefiles/miun.port.mk
--rw-r--r--   0        0        0      709 2022-10-20 12:02:01.903186 ladok3-3.6/makefiles/miun.pub.mk
--rw-r--r--   0        0        0     2880 2022-10-20 12:02:01.907186 ladok3-3.6/makefiles/noweb.mk
--rw-r--r--   0        0        0     2363 2022-10-20 12:02:01.907186 ladok3-3.6/makefiles/pkg.mk
--rw-r--r--   0        0        0     1225 2022-10-20 12:02:01.907186 ladok3-3.6/makefiles/portability.mk
--rw-r--r--   0        0        0     4827 2022-10-25 09:54:49.533819 ladok3-3.6/makefiles/pub.mk
--rw-r--r--   0        0        0     2321 2022-10-20 12:02:01.903186 ladok3-3.6/makefiles/results.mk
--rw-r--r--   0        0        0      421 2022-10-20 12:02:01.903186 ladok3-3.6/makefiles/subdir.mk
--rw-r--r--   0        0        0     6376 2022-10-25 09:54:49.533819 ladok3-3.6/makefiles/tex.mk
--rw-r--r--   0        0        0     2536 2022-10-20 12:02:01.903186 ladok3-3.6/makefiles/transform.mk
--rw-r--r--   0        0        0     1766 2023-03-30 09:45:48.759494 ladok3-3.6/pyproject.toml
--rw-r--r--   0        0        0       81 2022-10-25 12:52:56.440560 ladok3-3.6/src/ladok3/.gitignore
--rw-r--r--   0        0        0      557 2023-02-09 10:24:29.155703 ladok3-3.6/src/ladok3/Makefile
--rw-r--r--   0        0        0    43238 2023-02-09 19:44:21.886639 ladok3-3.6/src/ladok3/api.nw
--rw-r--r--   0        0        0    20472 2023-03-24 09:13:29.004895 ladok3-3.6/src/ladok3/cli.nw
--rw-r--r--   0        0        0    11785 2023-03-24 10:51:01.801680 ladok3-3.6/src/ladok3/data.nw
--rw-r--r--   0        0        0    48653 2023-02-09 13:29:07.825891 ladok3-3.6/src/ladok3/ladok3.nw
--rw-r--r--   0        0        0     7303 2023-02-08 20:51:23.897946 ladok3-3.6/src/ladok3/report.nw
--rw-r--r--   0        0        0     3194 2023-03-30 09:45:10.519410 ladok3-3.6/src/ladok3/student.nw
--rw-r--r--   0        0        0   180333 2023-02-09 19:28:11.895452 ladok3-3.6/src/ladok3/undoc.nw
--rw-r--r--   0        0        0     8098 1970-01-01 00:00:00.000000 ladok3-3.6/PKG-INFO
+-rw-r--r--   0        0        0     1155 2023-02-09 10:24:29.151703 ladok3-3.7/LICENSE
+-rw-r--r--   0        0        0     6677 2022-10-25 12:52:56.416560 ladok3-3.7/README.md
+-rw-r--r--   0        0        0      980 2023-02-09 10:25:13.624003 ladok3-3.7/doc/Makefile
+-rw-r--r--   0        0        0      173 2022-10-25 09:48:40.909030 ladok3-3.7/doc/abstract.tex
+-rw-r--r--   0        0        0     3723 2023-02-09 10:24:29.155703 ladok3-3.7/doc/ladok3.tex
+-rw-r--r--   0        0        0     1160 2022-10-25 09:48:40.917030 ladok3-3.7/doc/preamble.tex
+-rw-r--r--   0        0        0     3276 2022-10-25 09:54:49.529819 ladok3-3.7/makefiles/doc.mk
+-rw-r--r--   0        0        0     1326 2022-10-20 12:02:01.907186 ladok3-3.7/makefiles/exam.mk
+-rw-r--r--   0        0        0       66 2022-10-20 12:02:01.903186 ladok3-3.7/makefiles/haskell.mk
+-rw-r--r--   0        0        0      820 2022-10-20 12:02:01.907186 ladok3-3.7/makefiles/miun.course.mk
+-rw-r--r--   0        0        0     6206 2022-10-20 12:02:01.903186 ladok3-3.7/makefiles/miun.depend.mk
+-rw-r--r--   0        0        0      664 2022-10-20 12:02:01.903186 ladok3-3.7/makefiles/miun.docs.mk
+-rw-r--r--   0        0        0      611 2022-10-20 12:02:01.903186 ladok3-3.7/makefiles/miun.port.mk
+-rw-r--r--   0        0        0      709 2022-10-20 12:02:01.903186 ladok3-3.7/makefiles/miun.pub.mk
+-rw-r--r--   0        0        0     2880 2022-10-20 12:02:01.907186 ladok3-3.7/makefiles/noweb.mk
+-rw-r--r--   0        0        0     2363 2022-10-20 12:02:01.907186 ladok3-3.7/makefiles/pkg.mk
+-rw-r--r--   0        0        0     1225 2022-10-20 12:02:01.907186 ladok3-3.7/makefiles/portability.mk
+-rw-r--r--   0        0        0     4827 2022-10-25 09:54:49.533819 ladok3-3.7/makefiles/pub.mk
+-rw-r--r--   0        0        0     2321 2022-10-20 12:02:01.903186 ladok3-3.7/makefiles/results.mk
+-rw-r--r--   0        0        0      421 2022-10-20 12:02:01.903186 ladok3-3.7/makefiles/subdir.mk
+-rw-r--r--   0        0        0     6376 2022-10-25 09:54:49.533819 ladok3-3.7/makefiles/tex.mk
+-rw-r--r--   0        0        0     2536 2022-10-20 12:02:01.903186 ladok3-3.7/makefiles/transform.mk
+-rw-r--r--   0        0        0     1766 2023-06-08 19:45:29.110813 ladok3-3.7/pyproject.toml
+-rw-r--r--   0        0        0       81 2022-10-25 12:52:56.440560 ladok3-3.7/src/ladok3/.gitignore
+-rw-r--r--   0        0        0      557 2023-02-09 10:24:29.155703 ladok3-3.7/src/ladok3/Makefile
+-rw-r--r--   0        0        0    43238 2023-02-09 19:44:21.886639 ladok3-3.7/src/ladok3/api.nw
+-rw-r--r--   0        0        0    20472 2023-03-24 09:13:29.004895 ladok3-3.7/src/ladok3/cli.nw
+-rw-r--r--   0        0        0    11785 2023-03-24 10:51:01.801680 ladok3-3.7/src/ladok3/data.nw
+-rw-r--r--   0        0        0    50144 2023-06-08 19:44:13.018284 ladok3-3.7/src/ladok3/ladok3.nw
+-rw-r--r--   0        0        0     7303 2023-02-08 20:51:23.897946 ladok3-3.7/src/ladok3/report.nw
+-rw-r--r--   0        0        0     3356 2023-05-10 13:55:07.360271 ladok3-3.7/src/ladok3/student.nw
+-rw-r--r--   0        0        0   180333 2023-02-09 19:28:11.895452 ladok3-3.7/src/ladok3/undoc.nw
+-rw-r--r--   0        0        0     8098 1970-01-01 00:00:00.000000 ladok3-3.7/PKG-INFO
```

### Comparing `ladok3-3.6/LICENSE` & `ladok3-3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/README.md` & `ladok3-3.7/README.md`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/doc/Makefile` & `ladok3-3.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/doc/ladok3.tex` & `ladok3-3.7/doc/ladok3.tex`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/doc/preamble.tex` & `ladok3-3.7/doc/preamble.tex`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/makefiles/doc.mk` & `ladok3-3.7/makefiles/doc.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/makefiles/exam.mk` & `ladok3-3.7/makefiles/exam.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/makefiles/miun.course.mk` & `ladok3-3.7/makefiles/miun.course.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/makefiles/miun.depend.mk` & `ladok3-3.7/makefiles/miun.depend.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/makefiles/miun.docs.mk` & `ladok3-3.7/makefiles/miun.docs.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/makefiles/miun.port.mk` & `ladok3-3.7/makefiles/miun.port.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/makefiles/miun.pub.mk` & `ladok3-3.7/makefiles/miun.pub.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/makefiles/noweb.mk` & `ladok3-3.7/makefiles/noweb.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/makefiles/pkg.mk` & `ladok3-3.7/makefiles/pkg.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/makefiles/portability.mk` & `ladok3-3.7/makefiles/portability.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/makefiles/pub.mk` & `ladok3-3.7/makefiles/pub.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/makefiles/results.mk` & `ladok3-3.7/makefiles/results.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/makefiles/tex.mk` & `ladok3-3.7/makefiles/tex.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/makefiles/transform.mk` & `ladok3-3.7/makefiles/transform.mk`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/pyproject.toml` & `ladok3-3.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ladok3"
-version = "3.6"
+version = "3.7"
 description = "Python wrapper and CLI for the LADOK3 REST API."
 authors = [
   "Daniel Bosk <dbosk@kth.se>",
   "Alexander Baltatzis",
   "Gerald Q. Maguire Jr"
 ]
 license = "MIT"
```

### Comparing `ladok3-3.6/src/ladok3/Makefile` & `ladok3-3.7/src/ladok3/Makefile`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/src/ladok3/api.nw` & `ladok3-3.7/src/ladok3/api.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/src/ladok3/cli.nw` & `ladok3-3.7/src/ladok3/cli.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/src/ladok3/data.nw` & `ladok3-3.7/src/ladok3/data.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/src/ladok3/ladok3.nw` & `ladok3-3.7/src/ladok3/ladok3.nw`

 * *Files 3% similar despite different names*

```diff
@@ -904,14 +904,32 @@
   self.__courses.append(CourseRegistration(
     ladok=self.ladok,
     student=self,
     **course["Utbildningsinformation"]))
 @
 
 
+\section{Is the student suspended?}
+
+We also want to know if a student is suspended or not.
+We can get a list of suspensions for a student.
+However, since suspended students are rare, we haven't found a specimen to 
+study; so we simply don't know what the list contains.
+But we can return it nonetheless.
+We never cache this result since we always want the most up-to-date version.
+<<student attribute methods>>=
+@property
+def suspensions(self):
+  """
+  The list of the students' suspensions.
+  """
+  return self.ladok.get_student_suspensions_JSON(self.ladok_id)["Avstangning"]
+@
+
+
 \chapter{Courses}\label{CourseClasses}
 
 We can use the course-related classes as follows.
 \inputminted{python}{../examples/example_Course.py}
 
 \section{Course rounds}
 
@@ -1095,23 +1113,28 @@
 ladok3.clean_data(data)
 print(json.dumps(data, indent=2))
 print(r"\end{minted}")
 \end{pycode}
 
 Now that we have the [[data]] object, we can assign its values to the private 
 attributes.
+We note, however, that some course instances lack both [[Versionsnummer]] and 
+[[Omfattning]].
+It seems like faux courses are created to document when students go on 
+Exchanges.
+These faux courses have a name and code, but no credits or version of syllabus.
 <<assign CourseInstance data to private attributes>>=
 self.__education_id = data.pop("UtbildningUID")
 
 self.__code = data.pop("Utbildningskod")
 self.__name = data.pop("Benamning")
-self.__version = data.pop("Versionsnummer")
+self.__version = data.pop("Versionsnummer", None) 
 
-self.__credits = data.pop("Omfattning")
-self.__unit = data.pop("Enhet")
+self.__credits = data.pop("Omfattning", None)
+self.__unit = data.pop("Enhet", None)
 
 self.__grade_scale = self.ladok.get_grade_scales(
   id=data.pop("BetygsskalaID"))
 
 if "IngaendeMoment" in data:
   self.__components = [CourseComponent(
       ladok=self.ladok, course=self,
@@ -1122,14 +1145,18 @@
 
 
 \section{Course components}
 
 The [[CourseComponent]] class will make the attributes available.
 We specify the most interesting ones and let the [[LadokData]] constructor turn 
 the rest into properties as well, so that they are available for the curious.
+
+Turns out that some course components don't have any credits.
+This is probably a consequence of being a component in a course with no 
+credits, \eg one of those faux courses to register exchange studies.
 <<classes>>=
 class CourseComponent(LadokData):
   """Represents a course component of a course registration"""
   def __init__(self, /, **kwargs):
     super().__init__(**kwargs)
 
     self.__course = kwargs.pop("course")
@@ -1144,16 +1171,16 @@
     self.__code = kwargs.pop("Utbildningskod")
     description = kwargs.pop("Benamning")
     if isinstance(description, dict):
       self.__description = description["sv"]
     else:
       self.__description = description
 
-    self.__credits = kwargs.pop("Omfattning")
-    self.__unit = kwargs.pop("Enhet")
+    self.__credits = kwargs.pop("Omfattning", None)
+    self.__unit = kwargs.pop("Enhet", None)
 
     ladok = kwargs.pop("ladok")
     grade_scale_id = kwargs.pop("BetygsskalaID")
     self.__grade_scale = ladok.get_grade_scales(id=grade_scale_id)[0]
 
   @property
   def course(self):
@@ -1256,23 +1283,29 @@
 \chapter{Course objects related to students}
 
 \section{Course registrations and a student's results}
 
 Students register for a course.
 The [[CourseRegistration]] class represents this data from LADOK.
 This is the object that must be used to get results for a student.
+This object keeps more info than the course instance.
+
+We note that some registrations lack the \enquote{Utbildningstillfalleskod} 
+attribute.
+This happens on \enquote{custom courses} like Erasmus exchanges.
+If that's the case, we use the value [[None]] in its place.
 <<classes>>=
 class CourseRegistration(CourseInstance):
   """Represents a student's participation in a course instance"""
   def __init__(self, /, **kwargs):
     self.__student = kwargs.pop("student")
 
     # ett Ladok-ID för kursomgången
     self.__round_id = kwargs.pop("UtbildningstillfalleUID")
-    self.__round_code = kwargs.pop("Utbildningstillfalleskod")
+    self.__round_code = kwargs.pop("Utbildningstillfalleskod", None)
 
     dates = kwargs.pop("Studieperiod")
     self.__start = datetime.date.fromisoformat(dates["Startdatum"])
     self.__end = datetime.date.fromisoformat(dates["Slutdatum"])
 
     super().__init__(**kwargs)
 
@@ -1291,18 +1324,18 @@
     return self.__start
 
   @property
   def end(self):
     return self.__end
 
   def __str__(self):
-    return f"{self.code} {self.round_code} ({self.start}--{self.end})"
+    return f"{self.code} {self.round_code or ''} ({self.start}--{self.end})"
 
   def __repr__(self):
-    return f"{self.code}:{self.round_code}:{self.start}--{self.end}"
+    return f"{self.code}:{self.round_code or ''}:{self.start}--{self.end}"
 
   def results(self, /, **kwargs):
     """Returns the student's results on the course, filtered on keywords"""
     try:
       return filter_on_keys(self.__results, **kwargs)
     except:
       self.__fill_results()
@@ -1440,14 +1473,18 @@
     return self.__date
 
   @property
   def attested(self):
     """Returns True if the grade has been attested in LADOK"""
     return self.__attested
 
+  def __str__(self):
+    return f"{self.component} {self.grade} " \
+           f"{self.date}{'*' if not self.attested else ''}"
+
   def push(self):
     if self.__uid:
       <<push the existing CourseResult grade data to LADOK>>
     else:
       <<push the new CourseResult grade data to LADOK>>
     self.__modified = False
 @
```

### Comparing `ladok3-3.6/src/ladok3/report.nw` & `ladok3-3.7/src/ladok3/report.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/src/ladok3/student.nw` & `ladok3-3.7/src/ladok3/student.nw`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,15 @@
   student.alive
 except Exception as err:
   ladok3.cli.err(-1, f"can't fetch student data for {args.id}: {err}")
 
 print_student_data(student)
 
 if args.course:
+  print()
   print_course_data(student, args.course)
 @
 
 \subsection{Printing personal student data}
 
 To print the student's personal data, we simply print the most interesting 
 attributes.
@@ -90,20 +91,24 @@
 def print_student_data(student):
   """Prints the student data, all attributes, to stdout."""
   print(f"First name:   {student.first_name}")
   print(f"Last name:    {student.last_name}")
   print(f"Personnummer: {student.personnummer}")
   print(f"LADOK ID:     {student.ladok_id}")
   print(f"Alive:        {student.alive}")
+  print(f"Suspended:    {student.suspensions}")
 @
 
 \subsection{Printing student's course data}
 
 To print the student's course data, we simply filter the courses on the option 
 that the user supplies.
+We then print all results for each course.
 <<functions>>=
 def print_course_data(student, course):
   """Prints the courses"""
   print("Courses:")
   for course in student.courses(code=course):
-    print(f"- {course}")
+    print(f"{course}")
+    for result in course.results():
+      print(f"  {result}")
 @
```

### Comparing `ladok3-3.6/src/ladok3/undoc.nw` & `ladok3-3.7/src/ladok3/undoc.nw`

 * *Files identical despite different names*

### Comparing `ladok3-3.6/PKG-INFO` & `ladok3-3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladok3
-Version: 3.6
+Version: 3.7
 Summary: Python wrapper and CLI for the LADOK3 REST API.
 Home-page: https://github.com/dbosk/ladok3
 License: MIT
 Keywords: ladok3,ladok
 Author: Daniel Bosk
 Author-email: dbosk@kth.se
 Requires-Python: >=3.8,<4.0
```

