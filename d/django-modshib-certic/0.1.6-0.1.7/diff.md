# Comparing `tmp/django_modshib_certic-0.1.6.tar.gz` & `tmp/django_modshib_certic-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_modshib_certic-0.1.6.tar", max compression
+gzip compressed data, was "django_modshib_certic-0.1.7.tar", max compression
```

## Comparing `django_modshib_certic-0.1.6.tar` & `django_modshib_certic-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.6/modshib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.6/modshib/admin.py
--rw-r--r--   0        0        0      146 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.6/modshib/apps.py
--rw-r--r--   0        0        0      400 2023-06-01 08:51:10.568109 django_modshib_certic-0.1.6/modshib/context_processors.py
--rw-r--r--   0        0        0        0 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.6/modshib/migrations/__init__.py
--rw-r--r--   0        0        0       57 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.6/modshib/models.py
--rw-r--r--   0        0        0      896 2023-06-02 14:33:23.664664 django_modshib_certic-0.1.6/modshib/templates/registration/logged_out.html
--rw-r--r--   0        0        0     3065 2023-06-02 15:32:51.152782 django_modshib_certic-0.1.6/modshib/templates/registration/login.html
--rw-r--r--   0        0        0     1032 2023-06-05 14:35:51.956852 django_modshib_certic-0.1.6/modshib/templates/registration/reg_base.html
--rw-r--r--   0        0        0      811 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.6/modshib/templates/registration/sso_fail.html
--rw-r--r--   0        0        0      830 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.6/modshib/templates/registration/sso_no_account.html
--rw-r--r--   0        0        0       60 2023-05-24 14:07:03.824594 django_modshib_certic-0.1.6/modshib/tests.py
--rw-r--r--   0        0        0      117 2023-05-24 14:07:03.824594 django_modshib_certic-0.1.6/modshib/urls.py
--rw-r--r--   0        0        0     2746 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.6/modshib/views.py
--rw-r--r--   0        0        0      550 2023-06-05 14:36:13.932852 django_modshib_certic-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 django_modshib_certic-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-19 06:10:59.653227 django_modshib_certic-0.1.7/modshib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-19 06:10:59.654166 django_modshib_certic-0.1.7/modshib/admin.py
+-rw-r--r--   0        0        0      146 2023-05-24 09:58:37.360521 django_modshib_certic-0.1.7/modshib/apps.py
+-rw-r--r--   0        0        0      592 2023-06-08 09:24:21.472633 django_modshib_certic-0.1.7/modshib/context_processors.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:10:59.656283 django_modshib_certic-0.1.7/modshib/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2023-05-19 06:10:59.655746 django_modshib_certic-0.1.7/modshib/models.py
+-rw-r--r--   0        0        0      896 2023-06-01 14:40:15.254122 django_modshib_certic-0.1.7/modshib/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     3319 2023-06-08 09:24:21.468403 django_modshib_certic-0.1.7/modshib/templates/registration/login.html
+-rw-r--r--   0        0        0     1032 2023-06-08 09:14:42.230762 django_modshib_certic-0.1.7/modshib/templates/registration/reg_base.html
+-rw-r--r--   0        0        0      811 2023-06-01 08:20:11.704836 django_modshib_certic-0.1.7/modshib/templates/registration/sso_fail.html
+-rw-r--r--   0        0        0      830 2023-06-01 08:20:11.705098 django_modshib_certic-0.1.7/modshib/templates/registration/sso_no_account.html
+-rw-r--r--   0        0        0       60 2023-05-19 06:10:59.655994 django_modshib_certic-0.1.7/modshib/tests.py
+-rw-r--r--   0        0        0      117 2023-05-22 09:06:53.828987 django_modshib_certic-0.1.7/modshib/urls.py
+-rw-r--r--   0        0        0     2746 2023-06-01 08:20:11.705496 django_modshib_certic-0.1.7/modshib/views.py
+-rw-r--r--   0        0        0      550 2023-06-08 09:27:48.381699 django_modshib_certic-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 django_modshib_certic-0.1.7/PKG-INFO
```

### Comparing `django_modshib_certic-0.1.6/modshib/templates/registration/logged_out.html` & `django_modshib_certic-0.1.7/modshib/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.6/modshib/templates/registration/login.html` & `django_modshib_certic-0.1.7/modshib/templates/registration/login.html`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,25 @@
 {% block head_title %}{% translate "Connexion" %}{% endblock head_title %}
 {% block content %}
     <div class="d-flex flex-column min-vh-100 justify-content-center align-items-center">
         <div class="card" style="margin: 2em">
             <div class="card-body">
                 <h5 class="card-title">{% translate MODSHIB_FORMS_TITLE %}</h5>
                 <h6 class="card-subtitle mb-2 text-muted">{% translate "Connexion" %}</h6>
+                {% if MODSHIB_SHOW_SSO_LOGIN %}
                 <div class="card-text d-grid gap-2">
-                    <a href="{% url "modshib_sso" %}" class="btn btn-primary">{% translate "Connexion via SSO" %}</a>
-                </div>
-                <div class="card-text" style="margin-top: 1em;margin-bottom: 1em;">
-                    ou:
+                    <a href="{% url "modshib_sso" %}" class="btn btn-primary">{% translate MODSHIB_SSO_SUBMIT_LABEL %}</a>
                 </div>
+                    {% if MODSHIB_SHOW_LOCAL_LOGIN %}
+                    <div class="card-text" style="margin-top: 1em;margin-bottom: 1em;">
+                        ou:
+                    </div>
+                    {% endif %}
+                {% endif %}
+                {% if MODSHIB_SHOW_LOCAL_LOGIN %}
                 <div class="card-text" id="localForm">
                     <form method="post" class="d-grid gap-2">
                         {% csrf_token %}
                         {% if form.errors %}
                             <div class="alert alert-danger" role="alert">
                                 {% translate "Échec de la connexion" %}
                             </div>
@@ -42,14 +47,15 @@
                                            name="password"
                                            autocomplete="current-password"
                                            required=""
                                            id="id_password"
                                            value="{% if form.password.value %}{{ form.password.value}}{% endif %}"></td>
                             </tr>
                         </table>
-                        <button class="btn btn-secondary" type="submit">{% translate "Connexion avec mot de passe" %}</button>
+                        <button class="btn btn-secondary" type="submit">{% translate MODSHIB_LOCAL_SUBMIT_LABEL %}</button>
                     </form>
                 </div>
+                {% endif %}
             </div>
         </div>
     </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,14 +1,18 @@
 {% extends "registration/reg_base.html" %} {% load i18n %} {% block head_title
 %}{% translate "Connexion" %}{% endblock head_title %} {% block content %}
 ** {% translate MODSHIB_FORMS_TITLE %} **
 * {% translate "Connexion" %} *
- %}" class="btn btn-primary">{% translate "Connexion via SSO" %}
+{% if MODSHIB_SHOW_SSO_LOGIN %}
+ %}" class="btn btn-primary">{% translate MODSHIB_SSO_SUBMIT_LABEL %}
+{% if MODSHIB_SHOW_LOCAL_LOGIN %}
 ou:
+{% endif %} {% endif %} {% if MODSHIB_SHOW_LOCAL_LOGIN %}
 {% csrf_token %} {% if form.errors %}
 {% translate "Ãchec de la connexion" %}
 {% endif %}
 {% translate "Utilisateur" %}  [{% if form.username.value %}{
                                { form.username.value}}{% endif %}]
 {% translate "Mot de passe" %} [********************]
-{% translate "Connexion avec mot de passe" %}
+{% translate MODSHIB_LOCAL_SUBMIT_LABEL %}
+{% endif %}
 {% endblock content %}
```

### Comparing `django_modshib_certic-0.1.6/modshib/templates/registration/reg_base.html` & `django_modshib_certic-0.1.7/modshib/templates/registration/reg_base.html`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.6/modshib/templates/registration/sso_fail.html` & `django_modshib_certic-0.1.7/modshib/templates/registration/sso_fail.html`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.6/modshib/templates/registration/sso_no_account.html` & `django_modshib_certic-0.1.7/modshib/templates/registration/sso_no_account.html`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.6/modshib/views.py` & `django_modshib_certic-0.1.7/modshib/views.py`

 * *Files identical despite different names*

### Comparing `django_modshib_certic-0.1.6/pyproject.toml` & `django_modshib_certic-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-modshib-CERTIC"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Mickaël Desfrênes <mickael.desfrenes@unicaen.fr>"]
 license = "Cecill-B"
 packages = [
     { include = "modshib"},
 ]
 homepage = "https://www.certic.unicaen.fr"
```

### Comparing `django_modshib_certic-0.1.6/PKG-INFO` & `django_modshib_certic-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-modshib-certic
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Home-page: https://www.certic.unicaen.fr
 License: CECILL-B
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
```

