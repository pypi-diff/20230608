# Comparing `tmp/kagi-0.3.0.tar.gz` & `tmp/kagi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kagi-0.3.0.tar", max compression
+gzip compressed data, was "kagi-0.4.0.tar", max compression
```

## Comparing `kagi-0.3.0.tar` & `kagi-0.4.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1391 2022-09-18 04:53:57.135006 kagi-0.3.0/LICENSE
--rw-r--r--   0        0        0     4023 2022-09-18 04:53:57.135006 kagi-0.3.0/README.rst
--rw-r--r--   0        0        0        0 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/__init__.py
--rw-r--r--   0        0        0     2099 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/admin.py
--rw-r--r--   0        0        0      256 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/apps.py
--rw-r--r--   0        0        0     1603 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/forms.py
--rw-r--r--   0        0        0        0 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/management/__init__.py
--rw-r--r--   0        0        0        0 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/management/commands/__init__.py
--rw-r--r--   0        0        0     2266 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/management/commands/addbackupcode.py
--rw-r--r--   0        0        0     3270 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/migrations/__init__.py
--rw-r--r--   0        0        0     2723 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/models.py
--rw-r--r--   0        0        0     1315 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/oath.py
--rw-r--r--   0        0        0      835 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/settings.py
--rw-r--r--   0        0        0     2372 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/static/kagi/base64js.min.js
--rw-r--r--   0        0        0    10851 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/static/kagi/webauthn.js
--rw-r--r--   0        0        0      495 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/templates/kagi/add_key.html
--rw-r--r--   0        0        0      491 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/templates/kagi/backup_codes.html
--rw-r--r--   0        0        0      836 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/templates/kagi/base.html
--rw-r--r--   0        0        0     1032 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/templates/kagi/key_list.html
--rw-r--r--   0        0        0      216 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/templates/kagi/login.html
--rw-r--r--   0        0        0      626 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/templates/kagi/totp_device.html
--rw-r--r--   0        0        0      907 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/templates/kagi/totpdevice_list.html
--rw-r--r--   0        0        0      869 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/templates/kagi/two_factor_settings.html
--rw-r--r--   0        0        0     1105 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/templates/kagi/verify_second_factor.html
--rw-r--r--   0        0        0        0 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/tests/__init__.py
--rw-r--r--   0        0        0      464 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/tests/test_admin.py
--rw-r--r--   0        0        0     4760 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/tests/test_backups_code.py
--rw-r--r--   0        0        0     8364 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/tests/test_totp.py
--rw-r--r--   0        0        0     1605 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/tests/test_two_factor_settings.py
--rw-r--r--   0        0        0      200 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/tests/test_util.py
--rw-r--r--   0        0        0    13359 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/tests/test_webauthn_keys.py
--rw-r--r--   0        0        0     1137 2022-09-18 04:53:57.135006 kagi-0.3.0/kagi/urls.py
--rw-r--r--   0        0        0     1494 2022-09-18 04:53:57.139006 kagi-0.3.0/kagi/util.py
--rw-r--r--   0        0        0     1224 2022-09-18 04:53:57.139006 kagi-0.3.0/kagi/views/__init__.py
--rw-r--r--   0        0        0     6705 2022-09-18 04:53:57.139006 kagi-0.3.0/kagi/views/api.py
--rw-r--r--   0        0        0      441 2022-09-18 04:53:57.139006 kagi-0.3.0/kagi/views/backup_codes.py
--rw-r--r--   0        0        0     5490 2022-09-18 04:53:57.139006 kagi-0.3.0/kagi/views/login.py
--rw-r--r--   0        0        0      167 2022-09-18 04:53:57.139006 kagi-0.3.0/kagi/views/mixin.py
--rw-r--r--   0        0        0     3741 2022-09-18 04:53:57.139006 kagi-0.3.0/kagi/views/totp_devices.py
--rw-r--r--   0        0        0     1058 2022-09-18 04:53:57.139006 kagi-0.3.0/kagi/views/webauthn_keys.py
--rw-r--r--   0        0        0     2217 2022-09-18 04:54:08.715173 kagi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4988 1970-01-01 00:00:00.000000 kagi-0.3.0/setup.py
--rw-r--r--   0        0        0     5410 1970-01-01 00:00:00.000000 kagi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1391 2022-06-08 13:25:27.000000 kagi-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4001 2023-06-07 10:37:42.375000 kagi-0.4.0/README.rst
+-rw-r--r--   0        0        0        0 2022-09-18 04:46:06.000000 kagi-0.4.0/kagi/__init__.py
+-rw-r--r--   0        0        0     2099 2022-09-18 04:46:06.000000 kagi-0.4.0/kagi/admin.py
+-rw-r--r--   0        0        0      310 2023-06-07 10:37:42.375198 kagi-0.4.0/kagi/apps.py
+-rw-r--r--   0        0        0       45 2023-06-07 10:37:42.375306 kagi-0.4.0/kagi/constants.py
+-rw-r--r--   0        0        0     1603 2022-09-18 04:46:06.000000 kagi-0.4.0/kagi/forms.py
+-rw-r--r--   0        0        0        0 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/management/commands/__init__.py
+-rw-r--r--   0        0        0     2265 2023-06-02 08:12:31.597053 kagi-0.4.0/kagi/management/commands/addbackupcode.py
+-rw-r--r--   0        0        0     3269 2023-06-07 10:37:42.375489 kagi-0.4.0/kagi/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/migrations/__init__.py
+-rw-r--r--   0        0        0     2723 2023-06-07 10:37:32.681911 kagi-0.4.0/kagi/models.py
+-rw-r--r--   0        0        0     1315 2022-06-08 15:15:18.000000 kagi-0.4.0/kagi/oath.py
+-rw-r--r--   0        0        0      835 2023-06-07 10:37:32.681999 kagi-0.4.0/kagi/settings.py
+-rw-r--r--   0        0        0     2372 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/static/kagi/base64js.min.js
+-rw-r--r--   0        0        0    10851 2023-06-07 10:37:32.682505 kagi-0.4.0/kagi/static/kagi/webauthn.js
+-rw-r--r--   0        0        0      495 2023-06-07 10:37:32.682669 kagi-0.4.0/kagi/templates/kagi/add_key.html
+-rw-r--r--   0        0        0      491 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/templates/kagi/backup_codes.html
+-rw-r--r--   0        0        0      836 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/templates/kagi/base.html
+-rw-r--r--   0        0        0     1032 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/templates/kagi/key_list.html
+-rw-r--r--   0        0        0      216 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/templates/kagi/login.html
+-rw-r--r--   0        0        0      559 2023-06-07 10:37:42.375933 kagi-0.4.0/kagi/templates/kagi/totp_device.html
+-rw-r--r--   0        0        0      907 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/templates/kagi/totpdevice_list.html
+-rw-r--r--   0        0        0      869 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/templates/kagi/two_factor_settings.html
+-rw-r--r--   0        0        0     1105 2023-06-07 10:37:32.682780 kagi-0.4.0/kagi/templates/kagi/verify_second_factor.html
+-rw-r--r--   0        0        0        0 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/tests/__init__.py
+-rw-r--r--   0        0        0      464 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/tests/test_admin.py
+-rw-r--r--   0        0        0     4760 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/tests/test_backups_code.py
+-rw-r--r--   0        0        0     9590 2023-06-07 10:37:42.376098 kagi-0.4.0/kagi/tests/test_totp.py
+-rw-r--r--   0        0        0     1605 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/tests/test_two_factor_settings.py
+-rw-r--r--   0        0        0      200 2023-06-07 10:37:32.682963 kagi-0.4.0/kagi/tests/test_util.py
+-rw-r--r--   0        0        0    13359 2023-06-07 10:37:32.683100 kagi-0.4.0/kagi/tests/test_webauthn_keys.py
+-rw-r--r--   0        0        0     1137 2022-09-18 04:46:06.000000 kagi-0.4.0/kagi/urls.py
+-rw-r--r--   0        0        0     1494 2023-06-07 10:37:32.683413 kagi-0.4.0/kagi/util.py
+-rw-r--r--   0        0        0     1224 2022-09-18 04:46:06.000000 kagi-0.4.0/kagi/views/__init__.py
+-rw-r--r--   0        0        0     6708 2023-06-07 10:37:42.376314 kagi-0.4.0/kagi/views/api.py
+-rw-r--r--   0        0        0      441 2022-06-08 13:25:27.000000 kagi-0.4.0/kagi/views/backup_codes.py
+-rw-r--r--   0        0        0     5490 2022-09-18 04:46:06.000000 kagi-0.4.0/kagi/views/login.py
+-rw-r--r--   0        0        0      167 2022-09-18 04:46:06.000000 kagi-0.4.0/kagi/views/mixin.py
+-rw-r--r--   0        0        0     4833 2023-06-07 10:37:42.376860 kagi-0.4.0/kagi/views/totp_devices.py
+-rw-r--r--   0        0        0     1058 2022-09-18 04:46:06.000000 kagi-0.4.0/kagi/views/webauthn_keys.py
+-rw-r--r--   0        0        0     2516 2023-06-08 09:06:15.269598 kagi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5478 1970-01-01 00:00:00.000000 kagi-0.4.0/PKG-INFO
```

### Comparing `kagi-0.3.0/LICENSE` & `kagi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/README.rst` & `kagi-0.4.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 |coc| |build-status| |coverage| |readthedocs| |pypi|
 
 
 .. |coc| image:: https://img.shields.io/badge/%E2%9D%A4-code%20of%20conduct-blue.svg
     :target: https://github.com/justinmayer/kagi/blob/master/CODE_OF_CONDUCT.rst
     :alt: Code of Conduct
 
-.. |build-status| image:: https://img.shields.io/github/workflow/status/justinmayer/kagi/build
+.. |build-status| image:: https://img.shields.io/github/actions/workflow/status/justinmayer/kagi/main.yml?branch=main
     :target: https://github.com/justinmayer/kagi/actions
     :alt: Build Status
 
 .. |coverage| image:: https://img.shields.io/badge/coverage-100%25-brightgreen
     :target: https://github.com/justinmayer/kagi
     :alt: Code Coverage
 
@@ -49,15 +49,15 @@
 ----
 
 To see a demo, use the test project included in this repository and perform the
 following steps (creating and activating a virtual environment first is optional).
 
 First, install Poetry_::
 
-    curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/install-poetry.py | python -
+    curl -sSL https://install.python-poetry.org/ | python -
 
 Clone the Kagi source code and switch to its directory::
 
     git clone https://github.com/justinmayer/kagi.git && cd kagi
 
 Install dependencies, run database migrations, create a user, and serve the demo::
```

### Comparing `kagi-0.3.0/kagi/admin.py` & `kagi-0.4.0/kagi/admin.py`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/forms.py` & `kagi-0.4.0/kagi/forms.py`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/management/commands/addbackupcode.py` & `kagi-0.4.0/kagi/management/commands/addbackupcode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from django.contrib.auth import get_user_model
-from django.core.management.base import BaseCommand, CommandError
-
 """
 This is inspired by addstatictoken in django-otp, which is licensed as follows:
 
     Copyright (c) 2012, Peter Sagerson
     All rights reserved.
 
     Redistribution and use in source and binary forms, with or without
@@ -24,14 +21,16 @@
     FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
     DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
     SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
     CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
     OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
     OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
+from django.contrib.auth import get_user_model
+from django.core.management.base import BaseCommand, CommandError
 
 
 class Command(BaseCommand):
     help = "Adds a single backup code to the given user."
 
     def add_arguments(self, parser):
         parser.add_argument("username")
```

### Comparing `kagi-0.3.0/kagi/migrations/0001_initial.py` & `kagi-0.4.0/kagi/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [migrations.swappable_dependency(settings.AUTH_USER_MODEL)]
 
     operations = [
         migrations.CreateModel(
             name="TOTPDevice",
```

### Comparing `kagi-0.3.0/kagi/models.py` & `kagi-0.4.0/kagi/models.py`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/oath.py` & `kagi-0.4.0/kagi/oath.py`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/settings.py` & `kagi-0.4.0/kagi/settings.py`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/static/kagi/base64js.min.js` & `kagi-0.4.0/kagi/static/kagi/base64js.min.js`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/static/kagi/webauthn.js` & `kagi-0.4.0/kagi/static/kagi/webauthn.js`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/templates/kagi/base.html` & `kagi-0.4.0/kagi/templates/kagi/base.html`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/templates/kagi/key_list.html` & `kagi-0.4.0/kagi/templates/kagi/key_list.html`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/templates/kagi/totp_device.html` & `kagi-0.4.0/kagi/templates/kagi/totp_device.html`

 * *Files 11% similar despite different names*

```diff
@@ -17,12 +17,11 @@
 <p>
   {% trans 'Then, enter the token it gives you.' %}
 </p>
 
 <form method="POST">
   {% csrf_token %}
   {{ form.as_p }}
-  <input type="hidden" name="base32_key" value="{{ base32_key }}">
   <button value="backup" name="type">{% trans 'Submit' %}</button>
 </form>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% extends "kagi/base.html" %} {% load i18n %} {% block content %} {
 { block.super }}
 {% trans 'Scan this in your authenticator app:' %}
 {{_qr_svg|safe_}}
 {% trans "Or, if you can't scan a QR Code, enter this key as a time-based
 account:" %} {{_base32_key_}}
 {% trans 'Then, enter the token it gives you.' %}
-{% csrf_token %} {{ form.as_p }}  {% trans 'Submit' %}
+{% csrf_token %} {{ form.as_p }} {% trans 'Submit' %}
 {% endblock %}
```

### Comparing `kagi-0.3.0/kagi/templates/kagi/totpdevice_list.html` & `kagi-0.4.0/kagi/templates/kagi/totpdevice_list.html`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/templates/kagi/two_factor_settings.html` & `kagi-0.4.0/kagi/templates/kagi/two_factor_settings.html`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/templates/kagi/verify_second_factor.html` & `kagi-0.4.0/kagi/templates/kagi/verify_second_factor.html`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/tests/test_backups_code.py` & `kagi-0.4.0/kagi/tests/test_backups_code.py`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/tests/test_totp.py` & `kagi-0.4.0/kagi/tests/test_totp.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     response = client.get(reverse("kagi:add-totp"))
     assert response.status_code == 200
 
     base32_key = response.context_data["base32_key"]
     key = base64.b32decode(base32_key.encode("utf-8"))
     token = totp(key, now)
-    response = client.post(url, {"base32_key": base32_key, "token": token})
+    response = client.post(url, {"token": token})
     response.token = token
     return response
 
 
 def test_list_totp_devices(admin_client):
     response = admin_client.get(reverse("kagi:totp-devices"))
     assert list(response.context_data["totpdevice_list"]) == []
@@ -57,35 +57,63 @@
     assert re.match(base32_regexp, response.context_data["base32_key"])
     assert response.context_data["otpauth"] == (
         f"otpauth://totp/testserver:admin?secret={response.context_data['base32_key']}"
         f"&digits=6&issuer=testserver"
     )
 
 
-def test_add_a_new_totp_device_validates_the_otpauth_code_and_change_key_in_case_of_mismatch(
+def test_add_a_new_totp_device_validates_the_otpauth_code_but_keeps_secret_in_case_of_mismatch(
     admin_client,
 ):
     response = admin_client.get(reverse("kagi:add-totp"))
     assert response.status_code == 200
     base32_key = response.context_data["base32_key"]
-    response = admin_client.post(
-        reverse("kagi:add-totp"), {"base32_key": base32_key, "token": "123456"}
-    )
+
+    # Submit the form once, but with an invalid token. The secret should remain
+    # the same.
+    response = admin_client.post(reverse("kagi:add-totp"), {"token": "123456"})
     assert response.status_code == 200
     assert base32_key == response.context_data["base32_key"]
     form = response.context_data["form"]
     assert form.errors == {"token": ["That token is invalid."]}
 
+    # Submit the form a second time with the correct token. This should work.
+    key = base64.b32decode(base32_key.encode("utf-8"))
+    token = totp(key, timezone.now())
+    response = admin_client.post(reverse("kagi:add-totp"), {"token": token})
+    assert response.status_code == 302
+    assert response.url == reverse("kagi:totp-devices")
+    # Ensure the secret is removed from the user session after adding a device.
+    assert "kagi_totp_secret" not in admin_client.session
+
+    response = admin_client.get(reverse("kagi:totp-devices"))
+    assert len(response.context_data["totpdevice_list"]) == 1
+
+
+def test_add_a_new_totp_device_fails_when_secret_is_missing_in_session(admin_client):
+    response = admin_client.get(reverse("kagi:add-totp"))
+    assert response.status_code == 200
+
+    session = admin_client.session
+    del session["kagi_totp_secret"]
+    session.save()
+
+    response = admin_client.post(reverse("kagi:add-totp"), {"token": "123456"})
+    assert response.status_code == 302
+    assert response.url == reverse("kagi:add-totp")
+
 
 def test_add_a_new_totp_device_validates_the_otpauth_code_and_create_the_device_if_valid(
     admin_client,
 ):
     response = add_new_totp_device(admin_client)
     assert response.status_code == 302
     assert response.url == reverse("kagi:totp-devices")
+    # Ensure the secret is removed from the user session after adding a device.
+    assert "kagi_totp_secret" not in admin_client.session
 
     response = admin_client.get(reverse("kagi:totp-devices"))
     assert len(response.context_data["totpdevice_list"]) == 1
 
 
 def test_prevent_reuse_of_totp_device_code(admin_client):
     response = add_new_totp_device(admin_client)
```

### Comparing `kagi-0.3.0/kagi/tests/test_two_factor_settings.py` & `kagi-0.4.0/kagi/tests/test_two_factor_settings.py`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/tests/test_webauthn_keys.py` & `kagi-0.4.0/kagi/tests/test_webauthn_keys.py`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/urls.py` & `kagi-0.4.0/kagi/urls.py`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/util.py` & `kagi-0.4.0/kagi/util.py`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/views/__init__.py` & `kagi-0.4.0/kagi/views/__init__.py`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/views/api.py` & `kagi-0.4.0/kagi/views/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     try:
         sign_count = webauthn_assertion_response.verify()
     except Exception as e:
         return JsonResponse({"fail": f"Assertion failed. Error: {e}"}, status=400)
 
     # Update counter.
     key.sign_count = sign_count
-    key.last_used = now()
+    key.last_used_at = now()
     key.save()
 
     try:
         del request.session["kagi_pre_verify_user_pk"]
         del request.session["kagi_pre_verify_user_backend"]
         del request.session["challenge"]
     except KeyError:  # pragma: no cover
```

### Comparing `kagi-0.3.0/kagi/views/login.py` & `kagi-0.4.0/kagi/views/login.py`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/kagi/views/webauthn_keys.py` & `kagi-0.4.0/kagi/views/webauthn_keys.py`

 * *Files identical despite different names*

### Comparing `kagi-0.3.0/pyproject.toml` & `kagi-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "kagi"
-version = "0.3.0"
+version = "0.4.0"
 description = "Django app for WebAuthn and TOTP-based multi-factor authentication"
 authors = ["Justin Mayer <entroP@gmail.com>", "Rémy Hubscher <hubscher.remy@gmail.com>"]
 license = "BSD-2-Clause"
 readme = "README.rst"
 keywords = ["Django", "WebAuthn", "authentication", "MFA", "2FA"]
 
 repository = "https://github.com/justinmayer/kagi"
 documentation = "https://kagi.readthedocs.io"
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Framework :: Django",
-    "Framework :: Django :: 2.2",
     "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
+    "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
+    # "Programming Language :: Python :: ..." is auto-generated by poetry!
     "Topic :: Security",
     "Topic :: Security :: Cryptography",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/justinmayer/kagi/issues"
@@ -29,45 +32,40 @@
 [tool.poetry.dependencies]
 Django = ">= 2.2"
 python = ">= 3.7, < 4.0"
 qrcode = ">= 6.1, < 8.0"
 webauthn = "^0.4"
 
 [tool.poetry.dev-dependencies]
-black = "^22.8"
-flake8 = "^4.0"
-flake8-black = "^0.3"
+black = "^23.3"
+flake8 = "^5.0"
+Flake8-pyproject = "^1.2.3"
 furo = "2022.04.07"
-invoke = "^1.3"
-isort = "^5.2"
+invoke = "^2.0"
+isort = "^5.11"
 livereload = "^2.6"
 psutil = {version = "^5.7", optional = true}
-pyOpenSSL = "^21.0"
-pytest = "^6.0"
+pyOpenSSL = "^22.0"
+pytest = "^7.1"
 pytest-cov = "^3.0"
 pytest-django = "^4.0"
-pytest-pythonpath = "^0.7"
 pytest-sugar = "^0.9"
 pytest-xdist = "^2.1"
 sphinx = "^4.0"
 Werkzeug = "^2.0"
 
 [tool.autopub]
 project-name = "Kagi"
 git-username = "botpub"
 git-email = "botpub@autopub.rocks"
 append-github-contributor = true
 
 [tool.isort]
-# Maintain compatibility with Black
+profile = "black"
 combine_as_imports = true
-force_grid_wrap = 0
-include_trailing_comma = true
-line_length = 88
-multi_line_output = 3
 
 # Sort imports within their section independent of the import type
 force_sort_within_sections = true
 
 # Designate `django` and `kagi` as separate sections
 known_django = "django"
 known_kagi = "kagi"
@@ -76,7 +74,16 @@
 
 # Skip isort checks on these directories and files
 skip_glob = "**/migrations/**,**/node_modules/**,kagi/static/**,static,*.json,*.json"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+filterwarnings = ['ignore::DeprecationWarning:invoke.loader', 'ignore::DeprecationWarning:invoke.tasks']
+pythonpath = 'testproj'
+DJANGO_SETTINGS_MODULE = 'testproj.settings'
+
+[tool.flake8]
+ignore = ['E203', 'E501', 'W503']
+max-line-length = 88
```

### Comparing `kagi-0.3.0/setup.py` & `kagi-0.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,148 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: kagi
+Version: 0.4.0
+Summary: Django app for WebAuthn and TOTP-based multi-factor authentication
+Home-page: https://github.com/justinmayer/kagi
+License: BSD-2-Clause
+Keywords: Django,WebAuthn,authentication,MFA,2FA
+Author: Justin Mayer
+Author-email: entroP@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Security
+Classifier: Topic :: Security :: Cryptography
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: Django (>=2.2)
+Requires-Dist: qrcode (>=6.1,<8.0)
+Requires-Dist: webauthn (>=0.4,<0.5)
+Project-URL: Documentation, https://kagi.readthedocs.io
+Project-URL: Issue Tracker, https://github.com/justinmayer/kagi/issues
+Project-URL: Repository, https://github.com/justinmayer/kagi
+Description-Content-Type: text/x-rst
 
-packages = \
-['kagi',
- 'kagi.management',
- 'kagi.management.commands',
- 'kagi.migrations',
- 'kagi.tests',
- 'kagi.views']
-
-package_data = \
-{'': ['*'], 'kagi': ['static/kagi/*', 'templates/kagi/*']}
-
-install_requires = \
-['Django>=2.2', 'qrcode>=6.1,<8.0', 'webauthn>=0.4,<0.5']
-
-setup_kwargs = {
-    'name': 'kagi',
-    'version': '0.3.0',
-    'description': 'Django app for WebAuthn and TOTP-based multi-factor authentication',
-    'long_description': 'Kagi\n====\n\n|coc| |build-status| |coverage| |readthedocs| |pypi|\n\n\n.. |coc| image:: https://img.shields.io/badge/%E2%9D%A4-code%20of%20conduct-blue.svg\n    :target: https://github.com/justinmayer/kagi/blob/master/CODE_OF_CONDUCT.rst\n    :alt: Code of Conduct\n\n.. |build-status| image:: https://img.shields.io/github/workflow/status/justinmayer/kagi/build\n    :target: https://github.com/justinmayer/kagi/actions\n    :alt: Build Status\n\n.. |coverage| image:: https://img.shields.io/badge/coverage-100%25-brightgreen\n    :target: https://github.com/justinmayer/kagi\n    :alt: Code Coverage\n\n.. |readthedocs| image:: https://readthedocs.org/projects/kagi/badge/?version=latest\n    :target: https://kagi.readthedocs.io/en/latest/\n    :alt: Documentation Status\n\n.. |pypi| image:: https://img.shields.io/pypi/v/kagi.svg\n    :target: https://pypi.org/project/kagi/\n    :alt: PyPI Version\n\n\nKagi provides support for FIDO WebAuthn security keys and TOTP tokens in Django.\n\nKagi is a relatively young project and has not yet been fully battle-tested.\nIts use in a high-impact environment should be accompanied by a thorough\nunderstanding of how it works before relying on it.\n\nInstallation\n------------\n\n::\n\n    python -m pip install kagi\n\nAdd ``kagi`` to ``INSTALLED_APPS`` and include ``kagi.urls`` somewhere in your\nURL patterns. Set: ``LOGIN_URL = "kagi:login"``\n\nMake sure that Django’s built-in login view does not have a\n``urlpattern``, because it will authenticate users without their second\nfactor. Kagi provides its own login view to handle that.\n\nDemo\n----\n\nTo see a demo, use the test project included in this repository and perform the\nfollowing steps (creating and activating a virtual environment first is optional).\n\nFirst, install Poetry_::\n\n    curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/install-poetry.py | python -\n\nClone the Kagi source code and switch to its directory::\n\n    git clone https://github.com/justinmayer/kagi.git && cd kagi\n\nInstall dependencies, run database migrations, create a user, and serve the demo::\n\n    poetry install\n    poetry shell\n    invoke migrate\n    python testproj/manage.py createsuperuser\n    invoke serve\n\nYou should now be able to see the demo project login page in your browser at:\nhttp://localhost:8000/kagi/login\n\nSupported browsers and versions can be found here: https://caniuse.com/webauthn\nFor domains other than ``localhost``, WebAuthn requires that the site is served\nover a secure (HTTPS) connection.\n\nSince you haven’t added any security keys yet, you will be logged in with just a\nusername and password. Once logged in and on the multi-factor settings page,\nchoose “Manage WebAuthn keys” and then “Add another key” and follow the provided\ninstructions. Once WebAuthn and/or TOTP has been successfully configured, your\naccount will be protected by multi-factor authentication, and when you log in\nthe next time, your WebAuthn key or TOTP token will be required.\n\nYou can manage the keys attached to your account on the key management page at:\nhttp://localhost:8000/kagi/keys\n\n\nUsing WebAuthn Keys on Linux\n============================\n\nSome distros don’t come with udev rules to make USB HID /dev/\nnodes accessible to normal users. If your key doesn’t light up\nand start flashing when you expect it to, this might be what is\nhappening. See https://github.com/Yubico/libu2f-host/issues/2 and\nhttps://github.com/Yubico/libu2f-host/blob/master/70-u2f.rules for some\ndiscussion of the rule to make it accessible. If you just want a quick\ntemporary fix, you can run ``sudo chmod 666 /dev/hidraw*`` every time\nafter you plug in your key (the files disappear after unplugging).\n\n\nGratitude\n=========\n\nThis project would not exist without the significant contributions made by\n`Rémy HUBSCHER <https://github.com/natim>`_.\n\nThanks to Gavin Wahl for `django-u2f <https://github.com/gavinwahl/django-u2f>`_,\nwhich served as useful initial scaffolding for this project.\n\n\n.. _Poetry: https://python-poetry.org/docs/#installation\n',
-    'author': 'Justin Mayer',
-    'author_email': 'entroP@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/justinmayer/kagi',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+Kagi
+====
 
+|coc| |build-status| |coverage| |readthedocs| |pypi|
+
+
+.. |coc| image:: https://img.shields.io/badge/%E2%9D%A4-code%20of%20conduct-blue.svg
+    :target: https://github.com/justinmayer/kagi/blob/master/CODE_OF_CONDUCT.rst
+    :alt: Code of Conduct
+
+.. |build-status| image:: https://img.shields.io/github/actions/workflow/status/justinmayer/kagi/main.yml?branch=main
+    :target: https://github.com/justinmayer/kagi/actions
+    :alt: Build Status
+
+.. |coverage| image:: https://img.shields.io/badge/coverage-100%25-brightgreen
+    :target: https://github.com/justinmayer/kagi
+    :alt: Code Coverage
+
+.. |readthedocs| image:: https://readthedocs.org/projects/kagi/badge/?version=latest
+    :target: https://kagi.readthedocs.io/en/latest/
+    :alt: Documentation Status
+
+.. |pypi| image:: https://img.shields.io/pypi/v/kagi.svg
+    :target: https://pypi.org/project/kagi/
+    :alt: PyPI Version
+
+
+Kagi provides support for FIDO WebAuthn security keys and TOTP tokens in Django.
+
+Kagi is a relatively young project and has not yet been fully battle-tested.
+Its use in a high-impact environment should be accompanied by a thorough
+understanding of how it works before relying on it.
+
+Installation
+------------
+
+::
+
+    python -m pip install kagi
+
+Add ``kagi`` to ``INSTALLED_APPS`` and include ``kagi.urls`` somewhere in your
+URL patterns. Set: ``LOGIN_URL = "kagi:login"``
+
+Make sure that Django’s built-in login view does not have a
+``urlpattern``, because it will authenticate users without their second
+factor. Kagi provides its own login view to handle that.
+
+Demo
+----
+
+To see a demo, use the test project included in this repository and perform the
+following steps (creating and activating a virtual environment first is optional).
+
+First, install Poetry_::
+
+    curl -sSL https://install.python-poetry.org/ | python -
+
+Clone the Kagi source code and switch to its directory::
+
+    git clone https://github.com/justinmayer/kagi.git && cd kagi
+
+Install dependencies, run database migrations, create a user, and serve the demo::
+
+    poetry install
+    poetry shell
+    invoke migrate
+    python testproj/manage.py createsuperuser
+    invoke serve
+
+You should now be able to see the demo project login page in your browser at:
+http://localhost:8000/kagi/login
+
+Supported browsers and versions can be found here: https://caniuse.com/webauthn
+For domains other than ``localhost``, WebAuthn requires that the site is served
+over a secure (HTTPS) connection.
+
+Since you haven’t added any security keys yet, you will be logged in with just a
+username and password. Once logged in and on the multi-factor settings page,
+choose “Manage WebAuthn keys” and then “Add another key” and follow the provided
+instructions. Once WebAuthn and/or TOTP has been successfully configured, your
+account will be protected by multi-factor authentication, and when you log in
+the next time, your WebAuthn key or TOTP token will be required.
+
+You can manage the keys attached to your account on the key management page at:
+http://localhost:8000/kagi/keys
+
+
+Using WebAuthn Keys on Linux
+============================
+
+Some distros don’t come with udev rules to make USB HID /dev/
+nodes accessible to normal users. If your key doesn’t light up
+and start flashing when you expect it to, this might be what is
+happening. See https://github.com/Yubico/libu2f-host/issues/2 and
+https://github.com/Yubico/libu2f-host/blob/master/70-u2f.rules for some
+discussion of the rule to make it accessible. If you just want a quick
+temporary fix, you can run ``sudo chmod 666 /dev/hidraw*`` every time
+after you plug in your key (the files disappear after unplugging).
+
+
+Gratitude
+=========
+
+This project would not exist without the significant contributions made by
+`Rémy HUBSCHER <https://github.com/natim>`_.
+
+Thanks to Gavin Wahl for `django-u2f <https://github.com/gavinwahl/django-u2f>`_,
+which served as useful initial scaffolding for this project.
+
+
+.. _Poetry: https://python-poetry.org/docs/#installation
 
-setup(**setup_kwargs)
```

