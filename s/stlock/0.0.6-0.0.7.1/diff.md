# Comparing `tmp/stlock-0.0.6.tar.gz` & `tmp/stlock-0.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlock-0.0.6.tar", last modified: Mon May 22 19:49:41 2023, max compression
+gzip compressed data, was "stlock-0.0.7.1.tar", last modified: Tue May 23 16:23:39 2023, max compression
```

## Comparing `stlock-0.0.6.tar` & `stlock-0.0.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:49:41.781059 stlock-0.0.6/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3255 2023-05-22 19:49:41.781059 stlock-0.0.6/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3110 2023-05-22 19:49:35.000000 stlock-0.0.6/README.md
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       38 2023-05-22 19:49:41.781059 stlock-0.0.6/setup.cfg
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      402 2023-05-22 19:49:40.000000 stlock-0.0.6/setup.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:49:41.781059 stlock-0.0.6/stlock/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       31 2023-05-22 16:05:24.000000 stlock-0.0.6/stlock/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2149 2023-05-22 17:38:41.000000 stlock-0.0.6/stlock/stlock.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-22 19:49:41.781059 stlock-0.0.6/stlock.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3255 2023-05-22 19:49:41.000000 stlock-0.0.6/stlock.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      242 2023-05-22 19:49:41.000000 stlock-0.0.6/stlock.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 19:49:41.000000 stlock-0.0.6/stlock.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 16:50:38.000000 stlock-0.0.6/stlock.egg-info/not-zip-safe
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       15 2023-05-22 19:49:41.000000 stlock-0.0.6/stlock.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-22 19:49:41.000000 stlock-0.0.6/stlock.egg-info/top_level.txt
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-23 16:23:39.451447 stlock-0.0.7.1/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5180 2023-05-23 16:23:39.451447 stlock-0.0.7.1/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5033 2023-05-23 16:21:22.000000 stlock-0.0.7.1/README.md
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       38 2023-05-23 16:23:39.451447 stlock-0.0.7.1/setup.cfg
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      404 2023-05-23 16:23:36.000000 stlock-0.0.7.1/setup.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-23 16:23:39.451447 stlock-0.0.7.1/stlock/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       31 2023-05-22 16:05:24.000000 stlock-0.0.7.1/stlock/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2138 2023-05-23 15:50:14.000000 stlock-0.0.7.1/stlock/stlock.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-23 16:23:39.451447 stlock-0.0.7.1/stlock.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5180 2023-05-23 16:23:39.000000 stlock-0.0.7.1/stlock.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      242 2023-05-23 16:23:39.000000 stlock-0.0.7.1/stlock.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-23 16:23:39.000000 stlock-0.0.7.1/stlock.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 16:50:38.000000 stlock-0.0.7.1/stlock.egg-info/not-zip-safe
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       15 2023-05-23 16:23:39.000000 stlock-0.0.7.1/stlock.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-23 16:23:39.000000 stlock-0.0.7.1/stlock.egg-info/top_level.txt
```

### Comparing `stlock-0.0.6/PKG-INFO` & `stlock-0.0.7.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,86 @@
-Metadata-Version: 2.1
-Name: stlock
-Version: 0.0.6
-Summary: oauth2.0 stlock
-Author-email: office@stl.im
-Description-Content-Type: text/markdown
-
 # Библиотека Python stlock
 
 
 # Быстрый старт
 Пример с библиотекой FastAPI
 
 
 ```
 pip install stlock
 pip install fastapi
 pip install uvicorn
 ```
 
-app.py:
+main.py:
 ```
 from fastapi import FastAPI, HTTPException, Body, Query
 from stlock import AuthClient
 
-
 # создание экземпляра класса
-AC = AuthClient(client_id="client",  # id клиента
+AC = AuthClient(
+    client_id="client",  # id клиента
     client_secret="secret",  # secret клиента
     code_redirect_uri="http://localhost:8000/code",  # ссылка перенаправления запроса с кодом
     service_endpoint="https://bba6q6chdp0eatf6n0ms.containers.yandexcloud.net",  # ссылка на сервис авторизации
-    )
+)
 
+# service_endpoint="https://bba6q6chdp0eatf6n0ms.containers.yandexcloud.net"
+# dev версия проекта, очищается каждые 24 часа
 
 app = FastAPI()
 
 
 # Регистрация пользователя
 @app.post("/register", status_code=201)
 def register_user(username=Body(...), password=Body(...)):
    data, status_code = AC.register(username, password)
    if status_code >= 400:
        raise HTTPException(status_code, data["detail"])
    return data
 
 
-#Авторизация пользователя
+# Авторизация пользователя, редирект на http://localhost:8000/code
 @app.post('/login')
 def login(username: str = Body(...), password: str = Body(...)):
    data, status_code = AC.authorize_user(username, password)
    if status_code >= 400:
        raise HTTPException(status_code, data["detail"])
    return data
 
 
+# Получение кода после редиректа, заполняется в code_redirect_uri
 @app.get('/code')
 def getcode(code=Query(None)):
    data, status_code = AC.get_tokens(code)
    if status_code >= 400:
        raise HTTPException(status_code, data["detail"])
    return data
+
+
+# Обмен refresh токена но новые refresh и access токены
+@app.post("/refresh")
+def do_refresh_token(refresh_token=Body(...)):
+    data, status_code = AC.do_refresh(refresh_token['refresh_token'])
+    print(data, status_code)
+    if status_code >= 400:
+        raise HTTPException(status_code, data["detail"])
+    return data
+
+
+# Получение информации из токена
+@app.get("/user")
+def get_user_info(token: str = Query(...)):
+    user_data = AC.decode(token)
+    return user_data
 ```
 
 Для запуска сервера:
 ```
-uvicorn app.py:app
+uvicorn main:app
 ```
 
 # Описание методов:
 
     AC.register(username, password)
 
 Создаёт нового пользователя в базе данных
@@ -86,14 +99,16 @@
 
     AC.do_refresh(token)
 
 Обменивает refresh token на новый access и refresh токены
 
 # примеры запросов :
 создание пользователя:
+
+Input:
 ```
 POST http://localhost:8000/register
 Body {
     "username": "user1",
     "password": "Password123!"
 }
 ```
@@ -101,24 +116,61 @@
 Output:
 ```
 {
     "detail": "User registred"
 }
 ```
 авторизация пользователя:
+
+Input:
 ```
 POST http://localhost:8000/login
 Body {
     "username": "user1",
     "password": "Password123!"
 }
 ```
 
 Output:
 ```
 {
-    "access_token": "eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJjbGllbnQiLCJleHAiOjE2ODQ3ODUwMTUsInN1YiI6ImQ5YjBmYjE1LWJjYmQtNDNkNy1hMDdlLTAxNTIwMjBlZWI2ZiIsInJvbGUiOiJUZXN0In0.kOjADrKuTmLW-MGei4VEhf9Ce16eEzgle0UVB-t_vXoMQAtMQVzdI6iK14Rmds2w1bUMh82Wwru_AmMYS2NYYQ",
+    "access_token": "eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJjbGllbnQiLCJleHAiOjE2ODQ4NTgzNzgsInN1YiI6ImQ5YjBmYjE1LWJjYmQtNDNkNy1hMDdlLTAxNTIwMjBlZWI2ZiIsInJvbGUiOiJUZXN0In0.5_CHG7IR0DDulJcaPF8owduWsVsI2a5Vvbx-gyG_Xi2JIs9tpaPfJircy8WZXkeZ_3Mk8tAuvaxhTn7ytWXtdA",
     "expires_in": 60,
-    "refresh_token": "ZDI5ZMUZNDETNZYYZI01OTUZLTK5MZKTNJVLMDU1OTA5MDFM",
+    "refresh_token": "MJFMYZGWNWQTNDA5MI01NTU0LTHIMMYTYTI4MJM0MTZKMJHM",
     "token_type": "Bearer"
 }
 ```
+Информация о пользователе:
+
+Input:
+```
+GET http://localhost:8000/user?token=eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJjbGllbnQiLCJleHAiOjE2ODQ4NTgzNzgsInN1YiI6ImQ5YjBmYjE1LWJjYmQtNDNkNy1hMDdlLTAxNTIwMjBlZWI2ZiIsInJvbGUiOiJUZXN0In0.5_CHG7IR0DDulJcaPF8owduWsVsI2a5Vvbx-gyG_Xi2JIs9tpaPfJircy8WZXkeZ_3Mk8tAuvaxhTn7ytWXtdA
+```
+
+Output:
+```
+{
+    "aud": "client",
+    "exp": 1684858378,
+    "sub": "d9b0fb15-bcbd-43d7-a07e-0152020eeb6f",
+    "role": "Test"
+}
+```
+Обновление токена:
+
+Input:
+```
+POST http://localhost:8000/refresh
+Body {
+    "refresh_token": "MJFMYZGWNWQTNDA5MI01NTU0LTHIMMYTYTI4MJM0MTZKMJHM"
+}
+```
+
+Output:
+```
+{
+    "access_token": "eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJjbGllbnQiLCJleHAiOjE2ODQ4NTg0MzgsInN1YiI6ImQ5YjBmYjE1LWJjYmQtNDNkNy1hMDdlLTAxNTIwMjBlZWI2ZiIsInJvbGUiOiJUZXN0In0.5hFJg-U6i9E9GFp0Gxsn9ME3Dy-JtqKEyZotHT7WmnAsdZeLrDBjDU20ttb5f5HMLep8SWruTOoWjlfiZuGBKg",
+    "expires_in": 60,
+    "refresh_token": "NTC1ZDY5YJYTZTC0MC01ZJRMLTHJZTUTY2E1MMFJMTAZNZI0",
+    "token_type": "Bearer"
+}
+```
```

### Comparing `stlock-0.0.6/stlock/stlock.py` & `stlock-0.0.7.1/stlock/stlock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 import requests
 import jwt
 
 
 # Main class
 class AuthClient:
     def __init__(self, client_id, client_secret, code_redirect_uri, service_endpoint):
```

