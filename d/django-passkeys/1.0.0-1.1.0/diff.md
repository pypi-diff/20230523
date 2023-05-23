# Comparing `tmp/django-passkeys-1.0.0.tar.gz` & `tmp/django-passkeys-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-passkeys-1.0.0.tar", last modified: Sun Apr  9 09:42:26 2023, max compression
+gzip compressed data, was "django-passkeys-1.1.0.tar", last modified: Tue May 23 13:56:29 2023, max compression
```

## Comparing `django-passkeys-1.0.0.tar` & `django-passkeys-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1075 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/LICENSE
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       74 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/MANIFEST.in
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5962 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4585 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/README.md
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/django_passkeys.egg-info/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5962 2023-04-09 09:42:26.000000 django-passkeys-1.0.0/django_passkeys.egg-info/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      864 2023-04-09 09:42:26.000000 django-passkeys-1.0.0/django_passkeys.egg-info/SOURCES.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-04-09 09:42:26.000000 django-passkeys-1.0.0/django_passkeys.egg-info/dependency_links.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-04-09 09:42:26.000000 django-passkeys-1.0.0/django_passkeys.egg-info/not-zip-safe
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       47 2023-04-09 09:42:26.000000 django-passkeys-1.0.0/django_passkeys.egg-info/requires.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        9 2023-04-09 09:42:26.000000 django-passkeys-1.0.0/django_passkeys.egg-info/top_level.txt
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/passkeys/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5244 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/FIDO2.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       65 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      771 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/backend.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/passkeys/migrations/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1176 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/migrations/0001_initial.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/migrations/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      599 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/models.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.496876 django-passkeys-1.0.0/passkeys/static/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.496876 django-passkeys-1.0.0/passkeys/static/passkeys/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/passkeys/static/passkeys/css/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1590 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/static/passkeys/css/bootstrap-toggle.min.css
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/passkeys/static/passkeys/imgs/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     8981 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/passkeys/static/passkeys/js/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2684 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/static/passkeys/js/base64url.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4129 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/static/passkeys/js/bootstrap-toggle.min.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      687 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/static/passkeys/js/helpers.js
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/passkeys/templates/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5696 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/templates/PassKeys.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      128 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/templates/PassKeys_base.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      724 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/templates/check_passkeys.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      807 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/templates/modal.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1769 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/templates/passkeys.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      563 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/urls.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      911 2023-04-09 08:41:37.000000 django-passkeys-1.0.0/passkeys/views.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-04-09 09:42:26.500876 django-passkeys-1.0.0/setup.cfg
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1811 2023-04-09 09:40:02.000000 django-passkeys-1.0.0/setup.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-23 13:56:29.707177 django-passkeys-1.1.0/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1075 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/LICENSE
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       74 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/MANIFEST.in
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6394 2023-05-23 13:56:29.707177 django-passkeys-1.1.0/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5017 2023-05-23 13:55:19.000000 django-passkeys-1.1.0/README.md
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-23 13:56:29.707177 django-passkeys-1.1.0/django_passkeys.egg-info/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6394 2023-05-23 13:56:29.000000 django-passkeys-1.1.0/django_passkeys.egg-info/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      864 2023-05-23 13:56:29.000000 django-passkeys-1.1.0/django_passkeys.egg-info/SOURCES.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-23 13:56:29.000000 django-passkeys-1.1.0/django_passkeys.egg-info/dependency_links.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-04-09 09:42:26.000000 django-passkeys-1.1.0/django_passkeys.egg-info/not-zip-safe
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       47 2023-05-23 13:56:29.000000 django-passkeys-1.1.0/django_passkeys.egg-info/requires.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        9 2023-05-23 13:56:29.000000 django-passkeys-1.1.0/django_passkeys.egg-info/top_level.txt
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-23 13:56:29.707177 django-passkeys-1.1.0/passkeys/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5661 2023-05-23 13:45:55.000000 django-passkeys-1.1.0/passkeys/FIDO2.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       65 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      734 2023-05-23 13:41:18.000000 django-passkeys-1.1.0/passkeys/backend.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-23 13:56:29.707177 django-passkeys-1.1.0/passkeys/migrations/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1176 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/migrations/0001_initial.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/migrations/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      599 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/models.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-23 13:56:29.707177 django-passkeys-1.1.0/passkeys/static/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-23 13:56:29.707177 django-passkeys-1.1.0/passkeys/static/passkeys/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-23 13:56:29.707177 django-passkeys-1.1.0/passkeys/static/passkeys/css/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1590 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/static/passkeys/css/bootstrap-toggle.min.css
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-23 13:56:29.707177 django-passkeys-1.1.0/passkeys/static/passkeys/imgs/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     8981 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-23 13:56:29.707177 django-passkeys-1.1.0/passkeys/static/passkeys/js/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2684 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/static/passkeys/js/base64url.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4129 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/static/passkeys/js/bootstrap-toggle.min.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      687 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/static/passkeys/js/helpers.js
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-23 13:56:29.707177 django-passkeys-1.1.0/passkeys/templates/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5795 2023-05-23 13:40:14.000000 django-passkeys-1.1.0/passkeys/templates/PassKeys.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      128 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/templates/PassKeys_base.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      724 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/templates/check_passkeys.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      807 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/templates/modal.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1769 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/templates/passkeys.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      563 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/urls.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      911 2023-04-09 08:41:37.000000 django-passkeys-1.1.0/passkeys/views.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-05-23 13:56:29.707177 django-passkeys-1.1.0/setup.cfg
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1811 2023-05-23 13:55:47.000000 django-passkeys-1.1.0/setup.py
```

### Comparing `django-passkeys-1.0.0/LICENSE` & `django-passkeys-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.0.0/PKG-INFO` & `django-passkeys-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Django Authentication Backend for Passkeys
 Home-page: https://github.com/mkalioby/django-passkeys
 Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,15 +42,17 @@
 Passkeys is an extension to Web Authentication API that will allow the user to login to a service using another device.
 
 This app is a slim-down version of [django-mfa2](https://github.com/mkalioby/django-mfa2)
 
 Passkeys are now supported on 
 * Apple Ecosystem (iPhone 16.0+, iPadOS 16.1, Mac OS X Ventura)
 * Chromium based browsers (on PC and Laptop) allows picking up credentials from Android and iPhone/iPadOS.
-* Android Credentials creation for ResidentKeys is currently in Beta.
+* Android Credentials creation for ResidentKeys is currently in live now
+
+On May 3, 2023, Google allowed the use of Passkeys for the users to login, killing the password for enrolled users. 
 
 # Installation
 
 `pip install django-passkeys`
 
 Currently, it support Django 2.0+, Python 3.7+
 
@@ -71,25 +73,29 @@
    ```python
     AUTHENTICATION_BACKENDS = ['passkeys.backend.PasskeyModelBackend'] # Change your authentication backend
     FIDO_SERVER_ID="localhost"      # Server rp id for FIDO2, it the full domain of your project
     FIDO_SERVER_NAME="TestApp"
     import passkeys
     KEY_ATTACHMENT = NONE | passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM
    ```
+   **Note**: Starting v1.1, `FIDO_SERVER_ID` and/or `FIDO_SERVER_NAME` can be callable to support multi-tenants web applications.
 5. Add passkeys to urls.py
    ```python 
 
    urls_patterns= [
    '...',
    url(r'^passkeys/', include('passkeys.urls')),
    '....',
     ]
     ```
 6. To match the look and feel of your project, Passkeys includes `base.html` but it needs blocks named `head` & `content` to added its content to it.
-   **Note:** You can override `PassKeys_base.html` which is used by `Passkeys.html` so you can control the styling better and current `Passkeys_base.html` extends `base.html`
+   **Notes:** 
+    
+    1. You can override `PassKeys_base.html` which is used by `Passkeys.html` so you can control the styling better and current `Passkeys_base.html` extends `base.html`
+    1. Currently, `PassKeys_base.html` needs JQuery and bootstrap. 
 
 7. Somewhere in your app, add a link to 'passkeys:home'
     ```<li><a href="{% url 'passkeys:home' %}">Passkeys</a> </li>```
 8. In your login view, change the authenticate call to include the request as follows
    ```python
     user=authenticate(request, username=request.POST["username"],password=request.POST["password"])
     ```
@@ -141,11 +147,13 @@
 
 To report a security vulnerability, please use the
 [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure.
 
 # Contributors
 * [mahmoodnasr](https://github.com/mahmoodnasr)
+* [jacopsd](https://github.com/jacopsd)   
+* [gasparbrogueira](https://github.com/gasparbrogueira)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-passkeys Version: 1.0.0 Summary: A Django
+Metadata-Version: 2.1 Name: django-passkeys Version: 1.1.0 Summary: A Django
 Authentication Backend for Passkeys Home-page: https://github.com/mkalioby/
 django-passkeys Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby Author-email: mkalioby@mkalioby.com License: MIT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Framework :: Django Classifier: Framework ::
 Django :: 2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework ::
 Django :: 2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework ::
@@ -20,31 +20,36 @@
 pepy.tech/project/django-passkeys) An extension to Django *ModelBackend*
 backend to support passkeys. Passkeys is an extension to Web Authentication API
 that will allow the user to login to a service using another device. This app
 is a slim-down version of [django-mfa2](https://github.com/mkalioby/django-
 mfa2) Passkeys are now supported on * Apple Ecosystem (iPhone 16.0+, iPadOS
 16.1, Mac OS X Ventura) * Chromium based browsers (on PC and Laptop) allows
 picking up credentials from Android and iPhone/iPadOS. * Android Credentials
-creation for ResidentKeys is currently in Beta. # Installation `pip install
-django-passkeys` Currently, it support Django 2.0+, Python 3.7+ # Usage 1. in
-your settings.py add the application to your installed apps ```python
-INSTALLED_APPS=( '......', 'passkeys', '......') ``` 2. Collect Static Files
-`python manage.py collectstatic` 3. Run migrate `python manage.py migrate` 4.
-Add the following settings to your file ```python AUTHENTICATION_BACKENDS =
+creation for ResidentKeys is currently in live now On May 3, 2023, Google
+allowed the use of Passkeys for the users to login, killing the password for
+enrolled users. # Installation `pip install django-passkeys` Currently, it
+support Django 2.0+, Python 3.7+ # Usage 1. in your settings.py add the
+application to your installed apps ```python INSTALLED_APPS=( '......',
+'passkeys', '......') ``` 2. Collect Static Files `python manage.py
+collectstatic` 3. Run migrate `python manage.py migrate` 4. Add the following
+settings to your file ```python AUTHENTICATION_BACKENDS =
 ['passkeys.backend.PasskeyModelBackend'] # Change your authentication backend
 FIDO_SERVER_ID="localhost" # Server rp id for FIDO2, it the full domain of your
 project FIDO_SERVER_NAME="TestApp" import passkeys KEY_ATTACHMENT = NONE |
-passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM ``` 5. Add
-passkeys to urls.py ```python urls_patterns= [ '...', url(r'^passkeys/',
-include('passkeys.urls')), '....', ] ``` 6. To match the look and feel of your
-project, Passkeys includes `base.html` but it needs blocks named `head` &
-`content` to added its content to it. **Note:** You can override
-`PassKeys_base.html` which is used by `Passkeys.html` so you can control the
-styling better and current `Passkeys_base.html` extends `base.html` 7.
-Somewhere in your app, add a link to 'passkeys:home' ```
+passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM ``` **Note**:
+Starting v1.1, `FIDO_SERVER_ID` and/or `FIDO_SERVER_NAME` can be callable to
+support multi-tenants web applications. 5. Add passkeys to urls.py ```python
+urls_patterns= [ '...', url(r'^passkeys/', include('passkeys.urls')), '....', ]
+``` 6. To match the look and feel of your project, Passkeys includes
+`base.html` but it needs blocks named `head` & `content` to added its content
+to it. **Notes:** 1. You can override `PassKeys_base.html` which is used by
+`Passkeys.html` so you can control the styling better and current
+`Passkeys_base.html` extends `base.html` 1. Currently, `PassKeys_base.html`
+needs JQuery and bootstrap. 7. Somewhere in your app, add a link to 'passkeys:
+home' ```
 Passkeys
 ``` 8. In your login view, change the authenticate call to include the request
 as follows ```python user=authenticate(request, username=request.POST
 ["username"],password=request.POST["password"]) ``` 8. Finally, In your
 `login.html` * Give an id to your login form e.g 'loginForm', the id should be
 provided when calling `authn` function * Inside the form, add ```html  [{%
 static 'passkeys/imgs/FIDO-Passkey_Icon-White.png' %}] {%include 'passkeys.js'
@@ -65,8 +70,9 @@
 `platform_authenticator`: if the service requires only a platform authenticator
 (e.g TouchID, Windows Hello or Android SafetyNet) * `success_func`: function to
 call if a platform authenticator is found or if the user didn't login by a
 passkey * `fail_func`: function to call if no platform authenticator is found
 (optional). ## Security contact information To report a security vulnerability,
 please use the [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure. # Contributors * [mahmoodnasr]
-(https://github.com/mahmoodnasr)
+(https://github.com/mahmoodnasr) * [jacopsd](https://github.com/jacopsd) *
+[gasparbrogueira](https://github.com/gasparbrogueira)
```

### Comparing `django-passkeys-1.0.0/README.md` & `django-passkeys-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 Passkeys is an extension to Web Authentication API that will allow the user to login to a service using another device.
 
 This app is a slim-down version of [django-mfa2](https://github.com/mkalioby/django-mfa2)
 
 Passkeys are now supported on 
 * Apple Ecosystem (iPhone 16.0+, iPadOS 16.1, Mac OS X Ventura)
 * Chromium based browsers (on PC and Laptop) allows picking up credentials from Android and iPhone/iPadOS.
-* Android Credentials creation for ResidentKeys is currently in Beta.
+* Android Credentials creation for ResidentKeys is currently in live now
+
+On May 3, 2023, Google allowed the use of Passkeys for the users to login, killing the password for enrolled users. 
 
 # Installation
 
 `pip install django-passkeys`
 
 Currently, it support Django 2.0+, Python 3.7+
 
@@ -36,25 +38,29 @@
    ```python
     AUTHENTICATION_BACKENDS = ['passkeys.backend.PasskeyModelBackend'] # Change your authentication backend
     FIDO_SERVER_ID="localhost"      # Server rp id for FIDO2, it the full domain of your project
     FIDO_SERVER_NAME="TestApp"
     import passkeys
     KEY_ATTACHMENT = NONE | passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM
    ```
+   **Note**: Starting v1.1, `FIDO_SERVER_ID` and/or `FIDO_SERVER_NAME` can be callable to support multi-tenants web applications.
 5. Add passkeys to urls.py
    ```python 
 
    urls_patterns= [
    '...',
    url(r'^passkeys/', include('passkeys.urls')),
    '....',
     ]
     ```
 6. To match the look and feel of your project, Passkeys includes `base.html` but it needs blocks named `head` & `content` to added its content to it.
-   **Note:** You can override `PassKeys_base.html` which is used by `Passkeys.html` so you can control the styling better and current `Passkeys_base.html` extends `base.html`
+   **Notes:** 
+    
+    1. You can override `PassKeys_base.html` which is used by `Passkeys.html` so you can control the styling better and current `Passkeys_base.html` extends `base.html`
+    1. Currently, `PassKeys_base.html` needs JQuery and bootstrap. 
 
 7. Somewhere in your app, add a link to 'passkeys:home'
     ```<li><a href="{% url 'passkeys:home' %}">Passkeys</a> </li>```
 8. In your login view, change the authenticate call to include the request as follows
    ```python
     user=authenticate(request, username=request.POST["username"],password=request.POST["password"])
     ```
@@ -106,11 +112,13 @@
 
 To report a security vulnerability, please use the
 [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure.
 
 # Contributors
 * [mahmoodnasr](https://github.com/mahmoodnasr)
+* [jacopsd](https://github.com/jacopsd)   
+* [gasparbrogueira](https://github.com/gasparbrogueira)
```

#### html2text {}

```diff
@@ -2,31 +2,36 @@
 (https://pepy.tech/project/django-passkeys) An extension to Django
 *ModelBackend* backend to support passkeys. Passkeys is an extension to Web
 Authentication API that will allow the user to login to a service using another
 device. This app is a slim-down version of [django-mfa2](https://github.com/
 mkalioby/django-mfa2) Passkeys are now supported on * Apple Ecosystem (iPhone
 16.0+, iPadOS 16.1, Mac OS X Ventura) * Chromium based browsers (on PC and
 Laptop) allows picking up credentials from Android and iPhone/iPadOS. * Android
-Credentials creation for ResidentKeys is currently in Beta. # Installation `pip
-install django-passkeys` Currently, it support Django 2.0+, Python 3.7+ # Usage
-1. in your settings.py add the application to your installed apps ```python
-INSTALLED_APPS=( '......', 'passkeys', '......') ``` 2. Collect Static Files
-`python manage.py collectstatic` 3. Run migrate `python manage.py migrate` 4.
-Add the following settings to your file ```python AUTHENTICATION_BACKENDS =
+Credentials creation for ResidentKeys is currently in live now On May 3, 2023,
+Google allowed the use of Passkeys for the users to login, killing the password
+for enrolled users. # Installation `pip install django-passkeys` Currently, it
+support Django 2.0+, Python 3.7+ # Usage 1. in your settings.py add the
+application to your installed apps ```python INSTALLED_APPS=( '......',
+'passkeys', '......') ``` 2. Collect Static Files `python manage.py
+collectstatic` 3. Run migrate `python manage.py migrate` 4. Add the following
+settings to your file ```python AUTHENTICATION_BACKENDS =
 ['passkeys.backend.PasskeyModelBackend'] # Change your authentication backend
 FIDO_SERVER_ID="localhost" # Server rp id for FIDO2, it the full domain of your
 project FIDO_SERVER_NAME="TestApp" import passkeys KEY_ATTACHMENT = NONE |
-passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM ``` 5. Add
-passkeys to urls.py ```python urls_patterns= [ '...', url(r'^passkeys/',
-include('passkeys.urls')), '....', ] ``` 6. To match the look and feel of your
-project, Passkeys includes `base.html` but it needs blocks named `head` &
-`content` to added its content to it. **Note:** You can override
-`PassKeys_base.html` which is used by `Passkeys.html` so you can control the
-styling better and current `Passkeys_base.html` extends `base.html` 7.
-Somewhere in your app, add a link to 'passkeys:home' ```
+passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM ``` **Note**:
+Starting v1.1, `FIDO_SERVER_ID` and/or `FIDO_SERVER_NAME` can be callable to
+support multi-tenants web applications. 5. Add passkeys to urls.py ```python
+urls_patterns= [ '...', url(r'^passkeys/', include('passkeys.urls')), '....', ]
+``` 6. To match the look and feel of your project, Passkeys includes
+`base.html` but it needs blocks named `head` & `content` to added its content
+to it. **Notes:** 1. You can override `PassKeys_base.html` which is used by
+`Passkeys.html` so you can control the styling better and current
+`Passkeys_base.html` extends `base.html` 1. Currently, `PassKeys_base.html`
+needs JQuery and bootstrap. 7. Somewhere in your app, add a link to 'passkeys:
+home' ```
 Passkeys
 ``` 8. In your login view, change the authenticate call to include the request
 as follows ```python user=authenticate(request, username=request.POST
 ["username"],password=request.POST["password"]) ``` 8. Finally, In your
 `login.html` * Give an id to your login form e.g 'loginForm', the id should be
 provided when calling `authn` function * Inside the form, add ```html  [{%
 static 'passkeys/imgs/FIDO-Passkey_Icon-White.png' %}] {%include 'passkeys.js'
@@ -47,8 +52,9 @@
 `platform_authenticator`: if the service requires only a platform authenticator
 (e.g TouchID, Windows Hello or Android SafetyNet) * `success_func`: function to
 call if a platform authenticator is found or if the user didn't login by a
 passkey * `fail_func`: function to call if no platform authenticator is found
 (optional). ## Security contact information To report a security vulnerability,
 please use the [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure. # Contributors * [mahmoodnasr]
-(https://github.com/mahmoodnasr)
+(https://github.com/mahmoodnasr) * [jacopsd](https://github.com/jacopsd) *
+[gasparbrogueira](https://github.com/gasparbrogueira)
```

### Comparing `django-passkeys-1.0.0/django_passkeys.egg-info/PKG-INFO` & `django-passkeys-1.1.0/django_passkeys.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Django Authentication Backend for Passkeys
 Home-page: https://github.com/mkalioby/django-passkeys
 Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,15 +42,17 @@
 Passkeys is an extension to Web Authentication API that will allow the user to login to a service using another device.
 
 This app is a slim-down version of [django-mfa2](https://github.com/mkalioby/django-mfa2)
 
 Passkeys are now supported on 
 * Apple Ecosystem (iPhone 16.0+, iPadOS 16.1, Mac OS X Ventura)
 * Chromium based browsers (on PC and Laptop) allows picking up credentials from Android and iPhone/iPadOS.
-* Android Credentials creation for ResidentKeys is currently in Beta.
+* Android Credentials creation for ResidentKeys is currently in live now
+
+On May 3, 2023, Google allowed the use of Passkeys for the users to login, killing the password for enrolled users. 
 
 # Installation
 
 `pip install django-passkeys`
 
 Currently, it support Django 2.0+, Python 3.7+
 
@@ -71,25 +73,29 @@
    ```python
     AUTHENTICATION_BACKENDS = ['passkeys.backend.PasskeyModelBackend'] # Change your authentication backend
     FIDO_SERVER_ID="localhost"      # Server rp id for FIDO2, it the full domain of your project
     FIDO_SERVER_NAME="TestApp"
     import passkeys
     KEY_ATTACHMENT = NONE | passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM
    ```
+   **Note**: Starting v1.1, `FIDO_SERVER_ID` and/or `FIDO_SERVER_NAME` can be callable to support multi-tenants web applications.
 5. Add passkeys to urls.py
    ```python 
 
    urls_patterns= [
    '...',
    url(r'^passkeys/', include('passkeys.urls')),
    '....',
     ]
     ```
 6. To match the look and feel of your project, Passkeys includes `base.html` but it needs blocks named `head` & `content` to added its content to it.
-   **Note:** You can override `PassKeys_base.html` which is used by `Passkeys.html` so you can control the styling better and current `Passkeys_base.html` extends `base.html`
+   **Notes:** 
+    
+    1. You can override `PassKeys_base.html` which is used by `Passkeys.html` so you can control the styling better and current `Passkeys_base.html` extends `base.html`
+    1. Currently, `PassKeys_base.html` needs JQuery and bootstrap. 
 
 7. Somewhere in your app, add a link to 'passkeys:home'
     ```<li><a href="{% url 'passkeys:home' %}">Passkeys</a> </li>```
 8. In your login view, change the authenticate call to include the request as follows
    ```python
     user=authenticate(request, username=request.POST["username"],password=request.POST["password"])
     ```
@@ -141,11 +147,13 @@
 
 To report a security vulnerability, please use the
 [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure.
 
 # Contributors
 * [mahmoodnasr](https://github.com/mahmoodnasr)
+* [jacopsd](https://github.com/jacopsd)   
+* [gasparbrogueira](https://github.com/gasparbrogueira)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-passkeys Version: 1.0.0 Summary: A Django
+Metadata-Version: 2.1 Name: django-passkeys Version: 1.1.0 Summary: A Django
 Authentication Backend for Passkeys Home-page: https://github.com/mkalioby/
 django-passkeys Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby Author-email: mkalioby@mkalioby.com License: MIT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Framework :: Django Classifier: Framework ::
 Django :: 2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework ::
 Django :: 2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework ::
@@ -20,31 +20,36 @@
 pepy.tech/project/django-passkeys) An extension to Django *ModelBackend*
 backend to support passkeys. Passkeys is an extension to Web Authentication API
 that will allow the user to login to a service using another device. This app
 is a slim-down version of [django-mfa2](https://github.com/mkalioby/django-
 mfa2) Passkeys are now supported on * Apple Ecosystem (iPhone 16.0+, iPadOS
 16.1, Mac OS X Ventura) * Chromium based browsers (on PC and Laptop) allows
 picking up credentials from Android and iPhone/iPadOS. * Android Credentials
-creation for ResidentKeys is currently in Beta. # Installation `pip install
-django-passkeys` Currently, it support Django 2.0+, Python 3.7+ # Usage 1. in
-your settings.py add the application to your installed apps ```python
-INSTALLED_APPS=( '......', 'passkeys', '......') ``` 2. Collect Static Files
-`python manage.py collectstatic` 3. Run migrate `python manage.py migrate` 4.
-Add the following settings to your file ```python AUTHENTICATION_BACKENDS =
+creation for ResidentKeys is currently in live now On May 3, 2023, Google
+allowed the use of Passkeys for the users to login, killing the password for
+enrolled users. # Installation `pip install django-passkeys` Currently, it
+support Django 2.0+, Python 3.7+ # Usage 1. in your settings.py add the
+application to your installed apps ```python INSTALLED_APPS=( '......',
+'passkeys', '......') ``` 2. Collect Static Files `python manage.py
+collectstatic` 3. Run migrate `python manage.py migrate` 4. Add the following
+settings to your file ```python AUTHENTICATION_BACKENDS =
 ['passkeys.backend.PasskeyModelBackend'] # Change your authentication backend
 FIDO_SERVER_ID="localhost" # Server rp id for FIDO2, it the full domain of your
 project FIDO_SERVER_NAME="TestApp" import passkeys KEY_ATTACHMENT = NONE |
-passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM ``` 5. Add
-passkeys to urls.py ```python urls_patterns= [ '...', url(r'^passkeys/',
-include('passkeys.urls')), '....', ] ``` 6. To match the look and feel of your
-project, Passkeys includes `base.html` but it needs blocks named `head` &
-`content` to added its content to it. **Note:** You can override
-`PassKeys_base.html` which is used by `Passkeys.html` so you can control the
-styling better and current `Passkeys_base.html` extends `base.html` 7.
-Somewhere in your app, add a link to 'passkeys:home' ```
+passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM ``` **Note**:
+Starting v1.1, `FIDO_SERVER_ID` and/or `FIDO_SERVER_NAME` can be callable to
+support multi-tenants web applications. 5. Add passkeys to urls.py ```python
+urls_patterns= [ '...', url(r'^passkeys/', include('passkeys.urls')), '....', ]
+``` 6. To match the look and feel of your project, Passkeys includes
+`base.html` but it needs blocks named `head` & `content` to added its content
+to it. **Notes:** 1. You can override `PassKeys_base.html` which is used by
+`Passkeys.html` so you can control the styling better and current
+`Passkeys_base.html` extends `base.html` 1. Currently, `PassKeys_base.html`
+needs JQuery and bootstrap. 7. Somewhere in your app, add a link to 'passkeys:
+home' ```
 Passkeys
 ``` 8. In your login view, change the authenticate call to include the request
 as follows ```python user=authenticate(request, username=request.POST
 ["username"],password=request.POST["password"]) ``` 8. Finally, In your
 `login.html` * Give an id to your login form e.g 'loginForm', the id should be
 provided when calling `authn` function * Inside the form, add ```html  [{%
 static 'passkeys/imgs/FIDO-Passkey_Icon-White.png' %}] {%include 'passkeys.js'
@@ -65,8 +70,9 @@
 `platform_authenticator`: if the service requires only a platform authenticator
 (e.g TouchID, Windows Hello or Android SafetyNet) * `success_func`: function to
 call if a platform authenticator is found or if the user didn't login by a
 passkey * `fail_func`: function to call if no platform authenticator is found
 (optional). ## Security contact information To report a security vulnerability,
 please use the [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure. # Contributors * [mahmoodnasr]
-(https://github.com/mahmoodnasr)
+(https://github.com/mahmoodnasr) * [jacopsd](https://github.com/jacopsd) *
+[gasparbrogueira](https://github.com/gasparbrogueira)
```

### Comparing `django-passkeys-1.0.0/django_passkeys.egg-info/SOURCES.txt` & `django-passkeys-1.1.0/django_passkeys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.0.0/passkeys/FIDO2.py` & `django-passkeys-1.1.0/passkeys/FIDO2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 import json
+from base64 import urlsafe_b64encode
 
 import fido2.features
 from django.conf import settings
 from django.http import JsonResponse
 from django.utils import timezone
 from django.views.decorators.csrf import csrf_exempt
 from fido2.server import Fido2Server
 from fido2.utils import websafe_decode, websafe_encode
 from fido2.webauthn import PublicKeyCredentialRpEntity, AttestedCredentialData, RegistrationResponse
 from .models import UserPasskey
 from user_agents.parsers import parse as ua_parse
 
+
 def enable_json_mapping():
     try:
         fido2.features.webauthn_json_mapping.enabled = True
     except:
         pass
 
+
 def getUserCredentials(user):
     return [AttestedCredentialData(websafe_decode(uk.token)) for uk in UserPasskey.objects.filter(user = user)]
 
 
-
-def getServer():
+def getServer(request=None):
     """Get Server Info from settings and returns a Fido2Server"""
-    rp = PublicKeyCredentialRpEntity(id=settings.FIDO_SERVER_ID, name=settings.FIDO_SERVER_NAME)
+    if callable(settings.FIDO_SERVER_ID):
+        fido_server_id = settings.FIDO_SERVER_ID(request)
+    else:
+        fido_server_id = settings.FIDO_SERVER_ID
+
+    if callable(settings.FIDO_SERVER_NAME):
+        fido_server_name = settings.FIDO_SERVER_NAME(request)
+    else:
+        fido_server_name = settings.FIDO_SERVER_NAME
+
+    rp = PublicKeyCredentialRpEntity(id=fido_server_id, name=fido_server_name)
     return Fido2Server(rp)
 
+
 def get_current_platform(request):
     ua = ua_parse(request.META["HTTP_USER_AGENT"])
     if 'Safari' in ua.browser.family:
         return "Apple"
     elif 'Chrome' in ua.browser.family and ua.os.family == "Mac OS X":
         return "Chrome on Apple"
     elif 'Android' in ua.os.family:
@@ -39,18 +52,18 @@
         return "Microsoft"
     else: return "Key"
 
 
 def reg_begin(request):
     """Starts registering a new FIDO Device, called from API"""
     enable_json_mapping()
-    server = getServer()
+    server = getServer(request)
     auth_attachment = getattr(settings,'KEY_ATTACHMENT', None)
     registration_data, state = server.register_begin({
-        u'id': request.user.username.encode("utf8"),
+        u'id':  urlsafe_b64encode(request.user.username.encode("utf8")),
         u'name': request.user.username,
         u'displayName': request.user.username,
     }, getUserCredentials(request.user), authenticator_attachment = auth_attachment, resident_key_requirement=fido2.webauthn.ResidentKeyRequirement.PREFERRED)
     request.session['fido2_state'] = state
     return JsonResponse(dict(registration_data))
     #return HttpResponse(cbor.encode(registration_data), content_type = 'application/octet-stream')
 
@@ -60,15 +73,15 @@
     """Completes the registeration, called by API"""
     try:
         if not "fido2_state" in request.session:
             return JsonResponse({'status': 'ERR', "message": "FIDO Status can't be found, please try again"})
         enable_json_mapping()
         data = json.loads(request.body)
         name = data.pop("key_name",'')
-        server = getServer()
+        server = getServer(request)
         auth_data = server.register_complete(request.session.pop("fido2_state"), response = data)
         encoded = websafe_encode(auth_data.credential_data)
         platform = get_current_platform(request)
         if name == "":
             name = platform
         uk = UserPasskey(user=request.user, token=encoded, name = name,platform=platform)
         if data.get("id"):
@@ -78,57 +91,52 @@
         return JsonResponse({'status': 'OK'})
     except Exception as exp:
         import traceback
         print(traceback.format_exc())
         return JsonResponse({'status': 'ERR', "message": "Error on server, please try again later"})
 
 
-
-
-
-
-
 def auth_begin(request):
     enable_json_mapping()
-    server = getServer()
+    server = getServer(request)
     credentials=[]
     username = None
     if "base_username" in request.session:
         username = request.session["base_username"]
     if request.user.is_authenticated:
         username = request.user.username
     if username:
         credentials = getUserCredentials(request.session.get("base_username", request.user.username))
     auth_data, state = server.authenticate_begin(credentials)
     request.session['fido2_state'] = state
     return JsonResponse(dict(auth_data))
 
 
-
 @csrf_exempt
 def auth_complete(request):
     enable_json_mapping()
     credentials = []
-    server = getServer()
+    server = getServer(request)
     data = json.loads(request.POST["passkeys"])
     key = None
     #userHandle = data.get("response",{}).get('userHandle')
     credential_id = data['id']
     #
     # if userHandle:
     #     if User_Passkey.objects.filter(=userHandle).exists():
     #         credentials = getUserCredentials(userHandle)
     #         username=userHandle
     #     else:
     #         keys = User_Keys.objects.filter(user_handle = userHandle)
     #         if keys.exists():
     #             credentials = [AttestedCredentialData(websafe_decode(keys[0].properties["device"]))]
 
-    keys = UserPasskey.objects.filter(credential_id = credential_id)
+    keys = UserPasskey.objects.filter(credential_id = credential_id,enabled=1)
     if keys.exists():
+
         credentials=[AttestedCredentialData(websafe_decode(keys[0].token))]
         key = keys[0]
 
         try:
             cred = server.authenticate_complete(
                     request.session.pop('fido2_state'), credentials = credentials, response = data
             )
@@ -138,8 +146,8 @@
             raise Exception(excep)
         if key:
             key.last_used = timezone.now()
             request.session["passkey"] = {'passkey': True, 'name': key.name, "id":key.id, "platform": key.platform,
                                            'cross_platform': get_current_platform(request) != key.platform}
             key.save()
             return key.user
-    return None
+    return None
```

### Comparing `django-passkeys-1.0.0/passkeys/backend.py` & `django-passkeys-1.1.0/passkeys/backend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from django.contrib.auth.backends import ModelBackend
-
+from .FIDO2 import auth_complete
 
 class PasskeyModelBackend(ModelBackend):
     def authenticate(self, request, username='',password='', **kwargs):
+
         if request is None:
             raise Exception('request is required for passkeys.backend.PasskeyModelBackend')
+
         if username!='' and password != '':
             request.session["passkey"]={'passkey':False}
             return super().authenticate(request,username=username,password=password, **kwargs)
+
         passkeys = request.POST.get('passkeys')
-        if not passkeys:
+        if passkeys is None:
             raise Exception("Can't find '%s' key in request.POST, did you add the hidden input?")
-        if len(passkeys)>5:
-            from .FIDO2 import auth_complete
-            return auth_complete(request)
+
+        return auth_complete(request)
```

### Comparing `django-passkeys-1.0.0/passkeys/migrations/0001_initial.py` & `django-passkeys-1.1.0/passkeys/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.0.0/passkeys/models.py` & `django-passkeys-1.1.0/passkeys/models.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.0.0/passkeys/static/passkeys/css/bootstrap-toggle.min.css` & `django-passkeys-1.1.0/passkeys/static/passkeys/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.0.0/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png` & `django-passkeys-1.1.0/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.0.0/passkeys/static/passkeys/js/base64url.js` & `django-passkeys-1.1.0/passkeys/static/passkeys/js/base64url.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.0.0/passkeys/static/passkeys/js/bootstrap-toggle.min.js` & `django-passkeys-1.1.0/passkeys/static/passkeys/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.0.0/passkeys/static/passkeys/js/helpers.js` & `django-passkeys-1.1.0/passkeys/static/passkeys/js/helpers.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.0.0/passkeys/templates/PassKeys.html` & `django-passkeys-1.1.0/passkeys/templates/PassKeys.html`

 * *Files 0% similar despite different names*

```diff
@@ -108,45 +108,45 @@
     <script src="{% static 'passkeys/js/bootstrap-toggle.min.js'%}"></script>
 {% endblock %}
 {% block content %}
 {{block.super}}
     <br/>
     <br/>
     <div class="container">
-    <div class="row">
-        <div class="offset-5 col-2" style="text-align: center">
-            <div class="btn-group">
-                <button class="btn btn-success" onclick='start()'> Add Key</button>
+        <div class="row">
+            <div class="offset-5 col-2" style="text-align: center">
+                <div class="btn-group">
+                    <button class="btn btn-success" onclick='start()'> Add Key</button>
+                </div>
             </div>
         </div>
-    </div>
-    <br/>
+        <br/>
        <table class="table table-striped">
            <tr>
-
                <th>Name</th>
                <th>Date Added</th>
                <th>Platform</th>
                <th>Last Used</th>
                <th>Status</th>
                <th>Delete</th>
            </tr>
-        {% if keys %}
-            {% for key in keys %}
-            <tr>
+            {% if keys %}
+                {% for key in keys %}
+                <tr>
 
-                <td>{{ key.name }}</td>
-                <td>{{ key.added_on }}</td>
-                <td>{{ key.platform }}</td>
-                <td>{% if key.last_used %}{{ key.last_used }}{% else %}Never{% endif %}</td>
-                <td><input type="checkbox" id="toggle_{{ key.id }}" {% if key.enabled %}checked{% endif %} data-onstyle="success" data-offstyle="danger"  onchange="toggleKey({{ key.id }})" data-toggle="toggle" class="status_chk"></td>
-                <td><a href="javascript:void(0)" onclick="deleteKey({{ key.id }},'{{ key.key_type }}')"> <span class="fa fa-trash fa-solid fa-trash-can bi bi-trash-fill"></span></a></td>
+                    <td>{{ key.name }}</td>
+                    <td>{{ key.added_on }}</td>
+                    <td>{{ key.platform }}</td>
+                    <td>{% if key.last_used %}{{ key.last_used }}{% else %}Never{% endif %}</td>
+                    <td><input type="checkbox" id="toggle_{{ key.id }}" {% if key.enabled %}checked{% endif %} data-onstyle="success" data-offstyle="danger"  onchange="toggleKey({{ key.id }})" data-toggle="toggle" class="status_chk"></td>
+                    <td><a href="javascript:void(0)" onclick="deleteKey({{ key.id }},'{{ key.key_type }}')"> <span class="fa fa-trash fa-solid fa-trash-can bi bi-trash-fill"></span></a></td>
+                </tr>
+                {% endfor %}
+            {% else %}
+            <tr>
+                <td colspan="7" align="center">You didn't have any keys yet.</td>
             </tr>
-            {% endfor %}
-        {% else %}
-           <tr><td colspan="7" align="center">You didn't have any keys yet.</td> </tr>
-       {% endif %}
+        {% endif %}
         </table>
     </div>
-    </div>
     {% include "modal.html" %}
 {% endblock %}
```

### Comparing `django-passkeys-1.0.0/passkeys/templates/check_passkeys.js` & `django-passkeys-1.1.0/passkeys/templates/check_passkeys.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.0.0/passkeys/templates/modal.html` & `django-passkeys-1.1.0/passkeys/templates/modal.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.0.0/passkeys/templates/passkeys.js` & `django-passkeys-1.1.0/passkeys/templates/passkeys.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.0.0/passkeys/urls.py` & `django-passkeys-1.1.0/passkeys/urls.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.0.0/passkeys/views.py` & `django-passkeys-1.1.0/passkeys/views.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.0.0/setup.py` & `django-passkeys-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='django-passkeys',
-    version='1.0.0',
+    version='1.1.0',
     description='A Django Authentication Backend for Passkeys',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='Mohamed El-Kalioby',
     author_email = 'mkalioby@mkalioby.com',
     url = 'https://github.com/mkalioby/django-passkeys',
     download_url='https://github.com/mkalioby/django-passkeys',
```

